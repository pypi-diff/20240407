# Comparing `tmp/djangocms_katex-0.5.2.tar.gz` & `tmp/djangocms_katex-0.5.3.tar.gz`

## Comparing `djangocms_katex-0.5.2.tar` & `djangocms_katex-0.5.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/cms_plugins.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/forms.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/models.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/migrations/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/admin/css/preview.css
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/admin/js/preview.js
--rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/README.md
--rw-r--r--   0        0        0    26829 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.css
--rw-r--r--   0        0        0   630116 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.js
--rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.min.css
--rw-r--r--   0        0        0   277038 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.min.js
--rw-r--r--   0        0        0   604861 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.mjs
--rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.js
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.min.js
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.mjs
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.js
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.min.js
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.mjs
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.js
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.min.js
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.mjs
--rw-r--r--   0        0        0    79571 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.js
--rw-r--r--   0        0        0    33730 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.min.js
--rw-r--r--   0        0        0    75577 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.mjs
--rw-r--r--   0        0        0    24145 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.js
--rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.min.js
--rw-r--r--   0        0        0    20283 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.mjs
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.ttf
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.woff
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.ttf
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.ttf
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.ttf
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.ttf
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.ttf
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.ttf
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.ttf
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.ttf
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.ttf
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.ttf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.ttf
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.ttf
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.ttf
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.ttf
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.ttf
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/templates/djangocms_katex/formula.html
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/djangocms_katex/templates/djangocms_katex/admin/katex_widget.html
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/LICENSE
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/README.md
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 djangocms_katex-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/__init__.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/cms_plugins.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/forms.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/models.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/migrations/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/admin/css/preview.css
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/admin/js/preview.js
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/README.md
+-rw-r--r--   0        0        0    26829 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.css
+-rw-r--r--   0        0        0   630116 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.js
+-rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.min.css
+-rw-r--r--   0        0        0   277038 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.min.js
+-rw-r--r--   0        0        0   604861 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.mjs
+-rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.js
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.min.js
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.mjs
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.js
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.min.js
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.mjs
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.js
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.mjs
+-rw-r--r--   0        0        0    79571 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.js
+-rw-r--r--   0        0        0    33730 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.min.js
+-rw-r--r--   0        0        0    75577 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.mjs
+-rw-r--r--   0        0        0    24145 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.js
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.min.js
+-rw-r--r--   0        0        0    20283 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.mjs
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.ttf
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.woff
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.ttf
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.ttf
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.ttf
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.ttf
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.woff2
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.woff2
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.ttf
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.woff2
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.ttf
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.ttf
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.woff2
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.ttf
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.ttf
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.ttf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.woff2
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.ttf
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.ttf
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.ttf
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.ttf
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.ttf
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.woff2
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/templates/djangocms_katex/formula.html
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/djangocms_katex/templates/djangocms_katex/admin/katex_widget.html
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/README.md
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 djangocms_katex-0.5.3/PKG-INFO
```

### Comparing `djangocms_katex-0.5.2/djangocms_katex/forms.py` & `djangocms_katex-0.5.3/djangocms_katex/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/models.py` & `djangocms_katex-0.5.3/djangocms_katex/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/locale/de/LC_MESSAGES/django.po` & `djangocms_katex-0.5.3/djangocms_katex/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/locale/en/LC_MESSAGES/django.po` & `djangocms_katex-0.5.3/djangocms_katex/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/migrations/0001_initial.py` & `djangocms_katex-0.5.3/djangocms_katex/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/admin/css/preview.css` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/admin/css/preview.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 /* static/djangocms_katex/admin/css/preview.css */
+.katex-widget {
+    width: 100%;
+}
 
 .katex-preview {
     width: 100%;
     padding-top: 0.5em;
     padding-bottom: 1em;
     background: var(--dca-gray-lightest, var(--darkened-bg, #f2f2f2));
     border: solid 1px var(--dca-gray-lighter, var(--border-color, #ddd));
```

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/admin/js/preview.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/admin/js/preview.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/README.md` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.css` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.css`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.min.css` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.min.css`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.min.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/katex.mjs` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/katex.mjs`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.min.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.min.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.mjs` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/auto-render.mjs`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.min.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.min.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.mjs` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/copy-tex.mjs`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.min.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.mjs` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mathtex-script-type.mjs`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.min.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.min.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.mjs` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/mhchem.mjs`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.min.js` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.min.js`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.mjs` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/contrib/render-a11y-string.mjs`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.ttf` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.woff` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.woff2` & `djangocms_katex-0.5.3/djangocms_katex/static/djangocms_katex/vendor/katex/fonts/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/djangocms_katex/templates/djangocms_katex/formula.html` & `djangocms_katex-0.5.3/djangocms_katex/templates/djangocms_katex/formula.html`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/.gitignore` & `djangocms_katex-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/LICENSE` & `djangocms_katex-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/README.md` & `djangocms_katex-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/pyproject.toml` & `djangocms_katex-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms_katex-0.5.2/PKG-INFO` & `djangocms_katex-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: djangocms-katex
-Version: 0.5.2
+Version: 0.5.3
 Summary: Provides plugin to render formulae in django CMS
 Project-URL: Homepage, https://github.com/fsbraun/djangocms-katex
 Author-email: Fabian Braun <fsbraun@gmx.de>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: KaTeX,django CMS
 Classifier: Development Status :: 5 - Production/Stable
```

