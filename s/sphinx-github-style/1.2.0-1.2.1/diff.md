# Comparing `tmp/sphinx-github-style-1.2.0.tar.gz` & `tmp/sphinx-github-style-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-github-style-1.2.0.tar", last modified: Sun Feb 18 22:55:31 2024, max compression
+gzip compressed data, was "sphinx-github-style-1.2.1.tar", last modified: Sun Apr  7 11:29:53 2024, max compression
```

## Comparing `sphinx-github-style-1.2.0.tar` & `sphinx-github-style-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-18 22:55:31.658551 sphinx-github-style-1.2.0/
--rw-rw-rw-   0        0        0     1087 2023-04-27 12:00:21.000000 sphinx-github-style-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     6620 2024-02-18 22:55:31.658551 sphinx-github-style-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5870 2024-02-18 22:55:14.000000 sphinx-github-style-1.2.0/README.rst
--rw-rw-rw-   0        0        0       42 2024-02-18 22:55:31.658551 sphinx-github-style-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1519 2024-01-21 05:39:18.000000 sphinx-github-style-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-18 22:55:31.642930 sphinx-github-style-1.2.0/sphinx_github_style/
--rw-rw-rw-   0        0        0     8606 2024-02-18 22:53:53.000000 sphinx-github-style-1.2.0/sphinx_github_style/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-18 22:55:31.658551 sphinx-github-style-1.2.0/sphinx_github_style/_static/
--rw-rw-rw-   0        0        0     1128 2023-08-25 05:08:55.000000 sphinx-github-style-1.2.0/sphinx_github_style/_static/github_style.css
--rw-rw-rw-   0        0        0     1239 2023-09-26 03:04:50.000000 sphinx-github-style-1.2.0/sphinx_github_style/add_linkcode_class.py
--rw-rw-rw-   0        0        0     5672 2024-02-18 22:51:01.000000 sphinx-github-style-1.2.0/sphinx_github_style/github_style.py
--rw-rw-rw-   0        0        0     1977 2024-02-18 22:51:01.000000 sphinx-github-style-1.2.0/sphinx_github_style/lexer.py
-drwxrwxrwx   0        0        0        0 2024-02-18 22:55:31.642930 sphinx-github-style-1.2.0/sphinx_github_style.egg-info/
--rw-rw-rw-   0        0        0     6620 2024-02-18 22:55:31.000000 sphinx-github-style-1.2.0/sphinx_github_style.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2024-02-18 22:55:31.000000 sphinx-github-style-1.2.0/sphinx_github_style.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-18 22:55:31.000000 sphinx-github-style-1.2.0/sphinx_github_style.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-02-18 22:55:31.000000 sphinx-github-style-1.2.0/sphinx_github_style.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-02-18 22:55:31.000000 sphinx-github-style-1.2.0/sphinx_github_style.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.084973 sphinx-github-style-1.2.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-27 12:00:21.000000 sphinx-github-style-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     7123 2024-04-07 11:29:53.084973 sphinx-github-style-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6373 2024-04-07 11:29:26.000000 sphinx-github-style-1.2.1/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-07 11:29:53.084973 sphinx-github-style-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1519 2024-01-21 05:39:18.000000 sphinx-github-style-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.053723 sphinx-github-style-1.2.1/sphinx_github_style/
+-rw-rw-rw-   0        0        0     1881 2024-04-07 11:23:50.000000 sphinx-github-style-1.2.1/sphinx_github_style/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.069351 sphinx-github-style-1.2.1/sphinx_github_style/_static/
+-rw-rw-rw-   0        0        0     1128 2023-08-25 05:08:55.000000 sphinx-github-style-1.2.1/sphinx_github_style/_static/github_style.css
+-rw-rw-rw-   0        0        0      931 2024-04-07 10:42:36.000000 sphinx-github-style-1.2.1/sphinx_github_style/add_linkcode_class.py
+-rw-rw-rw-   0        0        0     5464 2024-04-07 10:42:36.000000 sphinx-github-style-1.2.1/sphinx_github_style/github_style.py
+-rw-rw-rw-   0        0        0     1977 2024-02-18 22:51:01.000000 sphinx-github-style-1.2.1/sphinx_github_style/lexer.py
+drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.084973 sphinx-github-style-1.2.1/sphinx_github_style/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-07 10:47:00.000000 sphinx-github-style-1.2.1/sphinx_github_style/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-04-07 10:51:38.000000 sphinx-github-style-1.2.1/sphinx_github_style/utils/git.py
+-rw-rw-rw-   0        0        0     4658 2024-04-07 10:57:21.000000 sphinx-github-style-1.2.1/sphinx_github_style/utils/linkcode.py
+-rw-rw-rw-   0        0        0      733 2024-04-07 11:17:17.000000 sphinx-github-style-1.2.1/sphinx_github_style/utils/sphinx.py
+drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.069351 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/
+-rw-rw-rw-   0        0        0     7123 2024-04-07 11:29:52.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-04-07 11:29:53.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 11:29:52.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 11:29:52.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-07 11:29:52.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/top_level.txt
```

### Comparing `sphinx-github-style-1.2.0/LICENSE` & `sphinx-github-style-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.0/PKG-INFO` & `sphinx-github-style-1.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-github-style
-Version: 1.2.0
+Version: 1.2.1
 Summary: GitHub source code links and syntax highlighting for Sphinx documentation
 Home-page: https://github.com/tdkorn/sphinx-github-style
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-github-style/tarball/master
 Keywords: sphinx,sphinx-extension,sphinx-theme,pygments,pygments-style,github,linkcode
@@ -12,34 +12,47 @@
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
+.. |.add_linkcode_class+styled with CSS| replace:: styled with CSS
+.. _.add_linkcode_class+styled with CSS: https://sphinx-github-style.readthedocs.io/en/latest/add_linkcode_class.html
 .. |.~.get_linkcode_resolve| replace:: get_linkcode_resolve()
-.. _.~.get_linkcode_resolve: https://sphinx-github-style.readthedocs.io/en/latest/modules.html#sphinx_github_style.__init__.get_linkcode_resolve
+.. _.~.get_linkcode_resolve: https://sphinx-github-style.readthedocs.io/en/latest/linkcode.html#sphinx_github_style.utils.linkcode.get_linkcode_resolve
+.. |.linkcode_blob| replace:: linkcode_blob
+.. _.linkcode_blob: https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_blob
+.. |.linkcode_link_text| replace:: linkcode_link_text
+.. _.linkcode_link_text: https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_link_text
+.. |.linkcode_resolve| replace:: linkcode_resolve
+.. _.linkcode_resolve: https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_resolve
+.. |.linkcode_url| replace:: linkcode_url
+.. _.linkcode_url: https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_url
+.. |.sphinx+html_context| replace:: html_context
+.. _.sphinx+html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 .. |.sphinx.ext.linkcode| replace:: sphinx.ext.linkcode
 .. _.sphinx.ext.linkcode: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.sphinx.ext.viewcode| replace:: sphinx.ext.viewcode
 .. _.sphinx.ext.viewcode: https://www.sphinx-doc.org/en/master/usage/extensions/viewcode.html#module-sphinx.ext.viewcode
 
+
 ..  Title: Sphinx Github Style
 ..  Description: A Sphinx extension to add GitHub source code links and syntax highlighting
 ..  Author: TDKorn (Adam Korn)
 
 .. meta::
    :title: Sphinx Github Style
    :description: A Sphinx extension to add GitHub source code links and syntax highlighting
 
 
 sphinx-github-style - GitHub source code links and syntax highlighting for Sphinx documentation
 -------------------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.0/docs/source/_static/logo_pypi.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/logo_pypi.png
    :alt: Sphinx GitHub Style: GitHub Integration and Pygments Style for Sphinx Documentation
    :width: 50%
    :align: center
 
 
 
 
@@ -96,44 +109,44 @@
 
 Using |.sphinx.ext.linkcode|_,  a ``View on GitHub`` link is added to the documentation of every class, method, function, and property:
 
 |
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.0/docs/source/_static/github_link.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_link.png
    :alt: sphinx-github-style adds a "View on GitHub" link
 
 
 They link to and highlight the corresponding code block in your GitHub repository:
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.0/docs/source/_static/github_linked_code.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_linked_code.png
    :alt: The linked corresponding highlighted source code block on GitHub
 
 
 
 .. list-table::
    :header-rows: 1
    
    * - 📝 Note
-   * - These links can be `styled with CSS <https://sphinx-github-style.readthedocs.io/en/latest/add_linkcode_class.html>`_ and used with/instead
+   * - These links can be |.add_linkcode_class+styled with CSS|_ and used with/instead
        of the links added by |.sphinx.ext.viewcode|_
 
 
 
 Syntax Highlighting
 ====================
 
 ``sphinx-github-style`` also contains a ``Pygments`` style to highlight code blocks similar to GitHub:
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.0/docs/source/_static/syntax_highlighting.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/syntax_highlighting.png
    :alt: A code block highlighted by the Pygments style. It looks identical to GitHub.
 
 
 
 Installation
 ~~~~~~~~~~~~~~~~
 
@@ -157,49 +170,50 @@
 ===================================
 
 Add any (or none) of the following configuration variables to your ``conf.py``
 
 
 
 
-`linkcode_blob <https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_blob>`_
+|.linkcode_blob|_
  The blob to link to on GitHub - any of ``"head"``, ``"last_tag"``, or ``"{blob}"``
 
   **Type:** ``str``
 
   **Default:** ``"head"``
 
  * ``"head"`` (default): links to the most recent commit hash; if this commit is tagged, uses the tag instead
  * ``"last_tag"``: links to the most recent commit tag on the currently checked out branch
  * ``"blob"``: links to any blob you want, for example ``"master"`` or ``"v2.0.1"``
 
 |
 
-`linkcode_url <https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_url>`_
+|.linkcode_url|_
  The link to your GitHub repository formatted as ``https://github.com/user/repo``
 
   **Type:** ``str``
 
   **Default:** ``f"https://github.com/{html_context['github_user']}/{html_context['github_repo']}/{html_context['github_version']}"``
 
- * If not provided, will attempt to create the link from the `html_context <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context>`_ dict
+ * If not provided, will attempt to create the link from the |.sphinx+html_context|_ dict
 
 |
 
-`linkcode_link_text <https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_link_text>`_
+|.linkcode_link_text|_
  The text to use for the linkcode link
 
   **Type:** ``str``
 
   **Default:** ``"View on GitHub"``
 
 |
 
-`linkcode_resolve <https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_resolve>`_
+|.linkcode_resolve|_
  A ``linkcode_resolve()`` function to use when resolving the link target with |.sphinx.ext.linkcode|_
 
   **Type:** ``Callable``
 
   **Default:** Return value from |.~.get_linkcode_resolve|_
 
 
 
+
```

### Comparing `sphinx-github-style-1.2.0/setup.py` & `sphinx-github-style-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.0/sphinx_github_style/_static/github_style.css` & `sphinx-github-style-1.2.1/sphinx_github_style/_static/github_style.css`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.0/sphinx_github_style/add_linkcode_class.py` & `sphinx-github-style-1.2.1/sphinx_github_style/add_linkcode_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import sphinx
 from sphinx.locale import _
 from sphinx.application import Sphinx
 from docutils.nodes import Node, Text
 from docutils import nodes
-from typing import Any, Dict
 
 
 def add_linkcode_node_class(app: Sphinx, doctree: Node, docname: str) -> None:
     """Changes every :class:`~.Node` added by :mod:`sphinx.ext.linkcode` to use the ``"linkcode-link"`` class
 
     This creates separation from the nodes added by :mod:`sphinx.ext.viewcode`, allowing
     for different link text and CSS styling
@@ -18,13 +16,7 @@
     link_text = getattr(env.config, 'linkcode_link_text')
 
     for node in list(doctree.findall(nodes.inline)):
         if 'viewcode-link' in node['classes']:
             if node.parent.get('internal', None) is False:
                 node['classes'] = ['linkcode-link']
                 node.children = [Text(_(f'{link_text}'))]
-
-
-def setup(app: Sphinx) -> Dict[str, Any]:
-    app.connect('doctree-resolved', add_linkcode_node_class)
-    app.add_config_value('linkcode_link_text', 'View on GitHub', 'html')
-    return {'version': sphinx.__display_version__, 'parallel_read_safe': True}
```

### Comparing `sphinx-github-style-1.2.0/sphinx_github_style/github_style.py` & `sphinx-github-style-1.2.1/sphinx_github_style/github_style.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,12 +135,7 @@
         String.Other: pl["syntax-string"],
         String.Regex: pl["syntax-string"],
         String.Single: pl["syntax-string"],
         String.Symbol: pl["syntax-string"],
         Text: pl["syntax-markup-bold"],
     }
 
-
-def setup(app):
-    app.config.pygments_style = 'sphinx_github_style.GitHubStyle'
-    app.add_css_file('github_style.css')
-    return {'version': sphinx.__display_version__, 'parallel_read_safe': True}
```

### Comparing `sphinx-github-style-1.2.0/sphinx_github_style/lexer.py` & `sphinx-github-style-1.2.1/sphinx_github_style/lexer.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.0/sphinx_github_style.egg-info/PKG-INFO` & `sphinx-github-style-1.2.1/sphinx_github_style.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-github-style
-Version: 1.2.0
+Version: 1.2.1
 Summary: GitHub source code links and syntax highlighting for Sphinx documentation
 Home-page: https://github.com/tdkorn/sphinx-github-style
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-github-style/tarball/master
 Keywords: sphinx,sphinx-extension,sphinx-theme,pygments,pygments-style,github,linkcode
@@ -12,34 +12,47 @@
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
+.. |.add_linkcode_class+styled with CSS| replace:: styled with CSS
+.. _.add_linkcode_class+styled with CSS: https://sphinx-github-style.readthedocs.io/en/latest/add_linkcode_class.html
 .. |.~.get_linkcode_resolve| replace:: get_linkcode_resolve()
-.. _.~.get_linkcode_resolve: https://sphinx-github-style.readthedocs.io/en/latest/modules.html#sphinx_github_style.__init__.get_linkcode_resolve
+.. _.~.get_linkcode_resolve: https://sphinx-github-style.readthedocs.io/en/latest/linkcode.html#sphinx_github_style.utils.linkcode.get_linkcode_resolve
+.. |.linkcode_blob| replace:: linkcode_blob
+.. _.linkcode_blob: https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_blob
+.. |.linkcode_link_text| replace:: linkcode_link_text
+.. _.linkcode_link_text: https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_link_text
+.. |.linkcode_resolve| replace:: linkcode_resolve
+.. _.linkcode_resolve: https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_resolve
+.. |.linkcode_url| replace:: linkcode_url
+.. _.linkcode_url: https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_url
+.. |.sphinx+html_context| replace:: html_context
+.. _.sphinx+html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 .. |.sphinx.ext.linkcode| replace:: sphinx.ext.linkcode
 .. _.sphinx.ext.linkcode: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.sphinx.ext.viewcode| replace:: sphinx.ext.viewcode
 .. _.sphinx.ext.viewcode: https://www.sphinx-doc.org/en/master/usage/extensions/viewcode.html#module-sphinx.ext.viewcode
 
+
 ..  Title: Sphinx Github Style
 ..  Description: A Sphinx extension to add GitHub source code links and syntax highlighting
 ..  Author: TDKorn (Adam Korn)
 
 .. meta::
    :title: Sphinx Github Style
    :description: A Sphinx extension to add GitHub source code links and syntax highlighting
 
 
 sphinx-github-style - GitHub source code links and syntax highlighting for Sphinx documentation
 -------------------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.0/docs/source/_static/logo_pypi.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/logo_pypi.png
    :alt: Sphinx GitHub Style: GitHub Integration and Pygments Style for Sphinx Documentation
    :width: 50%
    :align: center
 
 
 
 
@@ -96,44 +109,44 @@
 
 Using |.sphinx.ext.linkcode|_,  a ``View on GitHub`` link is added to the documentation of every class, method, function, and property:
 
 |
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.0/docs/source/_static/github_link.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_link.png
    :alt: sphinx-github-style adds a "View on GitHub" link
 
 
 They link to and highlight the corresponding code block in your GitHub repository:
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.0/docs/source/_static/github_linked_code.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_linked_code.png
    :alt: The linked corresponding highlighted source code block on GitHub
 
 
 
 .. list-table::
    :header-rows: 1
    
    * - 📝 Note
-   * - These links can be `styled with CSS <https://sphinx-github-style.readthedocs.io/en/latest/add_linkcode_class.html>`_ and used with/instead
+   * - These links can be |.add_linkcode_class+styled with CSS|_ and used with/instead
        of the links added by |.sphinx.ext.viewcode|_
 
 
 
 Syntax Highlighting
 ====================
 
 ``sphinx-github-style`` also contains a ``Pygments`` style to highlight code blocks similar to GitHub:
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.0/docs/source/_static/syntax_highlighting.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/syntax_highlighting.png
    :alt: A code block highlighted by the Pygments style. It looks identical to GitHub.
 
 
 
 Installation
 ~~~~~~~~~~~~~~~~
 
@@ -157,49 +170,50 @@
 ===================================
 
 Add any (or none) of the following configuration variables to your ``conf.py``
 
 
 
 
-`linkcode_blob <https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_blob>`_
+|.linkcode_blob|_
  The blob to link to on GitHub - any of ``"head"``, ``"last_tag"``, or ``"{blob}"``
 
   **Type:** ``str``
 
   **Default:** ``"head"``
 
  * ``"head"`` (default): links to the most recent commit hash; if this commit is tagged, uses the tag instead
  * ``"last_tag"``: links to the most recent commit tag on the currently checked out branch
  * ``"blob"``: links to any blob you want, for example ``"master"`` or ``"v2.0.1"``
 
 |
 
-`linkcode_url <https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_url>`_
+|.linkcode_url|_
  The link to your GitHub repository formatted as ``https://github.com/user/repo``
 
   **Type:** ``str``
 
   **Default:** ``f"https://github.com/{html_context['github_user']}/{html_context['github_repo']}/{html_context['github_version']}"``
 
- * If not provided, will attempt to create the link from the `html_context <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context>`_ dict
+ * If not provided, will attempt to create the link from the |.sphinx+html_context|_ dict
 
 |
 
-`linkcode_link_text <https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_link_text>`_
+|.linkcode_link_text|_
  The text to use for the linkcode link
 
   **Type:** ``str``
 
   **Default:** ``"View on GitHub"``
 
 |
 
-`linkcode_resolve <https://sphinx-github-style.readthedocs.io/en/latest/index.html#confval-linkcode_resolve>`_
+|.linkcode_resolve|_
  A ``linkcode_resolve()`` function to use when resolving the link target with |.sphinx.ext.linkcode|_
 
   **Type:** ``Callable``
 
   **Default:** Return value from |.~.get_linkcode_resolve|_
 
 
 
+
```

