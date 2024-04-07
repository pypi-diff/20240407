# Comparing `tmp/isat-sibyl-1.0.7.tar.gz` & `tmp/isat-sibyl-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isat-sibyl-1.0.7.tar", last modified: Sat Mar 30 20:15:42 2024, max compression
+gzip compressed data, was "isat-sibyl-1.0.8.tar", last modified: Sun Apr  7 11:40:29 2024, max compression
```

## Comparing `isat-sibyl-1.0.7.tar` & `isat-sibyl-1.0.8.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.286660 isat-sibyl-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-30 20:15:42.286660 isat-sibyl-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.286660 isat-sibyl-1.0.7/isat_sibyl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-30 20:15:42.000000 isat-sibyl-1.0.7/isat_sibyl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-30 20:15:42.000000 isat-sibyl-1.0.7/isat_sibyl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:15:42.000000 isat-sibyl-1.0.7/isat_sibyl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-30 20:15:42.000000 isat-sibyl-1.0.7/isat_sibyl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-30 20:15:42.000000 isat-sibyl-1.0.7/isat_sibyl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-30 20:15:42.286660 isat-sibyl-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.274660 isat-sibyl-1.0.7/sibyl/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23636 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.278660 isat-sibyl-1.0.7/sibyl/components/
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Accordion.html
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Address.html
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Button.html
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/ButtonAnchor.html
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/ButtonHref.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/ButtonPage.html
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/ButtonType.html
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Card.html
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Carousel.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/CarouselSlide.html
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Chip.html
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/DoubleImageService.html
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Drawer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/DrawerItem.html
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/DrawerItemInner.html
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Header.html
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/ImageService.html
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Markdown.html
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/MaterialIcon.html
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/SkewedBanner.html
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/SkewedTitle.html
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Social.html
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/components/Spinner.html
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/dev.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.278660 isat-sibyl-1.0.7/sibyl/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/helpers/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/helpers/requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/helpers/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/helpers/shutil_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/helpers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/hot-reload.html
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.278660 isat-sibyl-1.0.7/sibyl/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/layouts/main_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.278660 isat-sibyl-1.0.7/sibyl/locales/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/locales/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/locales/global.json
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/locales/pt.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.278660 isat-sibyl-1.0.7/sibyl/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/pages/start.html
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.282660 isat-sibyl-1.0.7/sibyl/sibyl-static/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/sibyl-static/flex.css
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/sibyl-static/microsite.js
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/sibyl-static/spa.js
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/sibyl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.282660 isat-sibyl-1.0.7/sibyl/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:15:42.282660 isat-sibyl-1.0.7/sibyl/static/favicon/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/mstile-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/mstile-310x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/mstile-310x310.png
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/mstile-70x70.png
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/favicon/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/sibyl.svg
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-30 20:15:33.000000 isat-sibyl-1.0.7/sibyl/static/variables.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.389771 isat-sibyl-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-07 11:40:29.389771 isat-sibyl-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.389771 isat-sibyl-1.0.8/isat_sibyl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-07 11:40:29.000000 isat-sibyl-1.0.8/isat_sibyl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-07 11:40:29.000000 isat-sibyl-1.0.8/isat_sibyl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:40:29.000000 isat-sibyl-1.0.8/isat_sibyl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-07 11:40:29.000000 isat-sibyl-1.0.8/isat_sibyl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 11:40:29.000000 isat-sibyl-1.0.8/isat_sibyl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 11:40:29.389771 isat-sibyl-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.377771 isat-sibyl-1.0.8/sibyl/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23687 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.381771 isat-sibyl-1.0.8/sibyl/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Accordion.html
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Address.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Button.html
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/ButtonAnchor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/ButtonHref.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/ButtonPage.html
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/ButtonType.html
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Card.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Carousel.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/CarouselSlide.html
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Chip.html
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/DoubleImageService.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Drawer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/DrawerItem.html
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/DrawerItemInner.html
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/ImageService.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Markdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/MaterialIcon.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/SkewedBanner.html
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/SkewedTitle.html
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Social.html
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/components/Spinner.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/dev.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.385771 isat-sibyl-1.0.8/sibyl/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/helpers/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/helpers/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/helpers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/helpers/shutil_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/helpers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/hot-reload.html
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.385771 isat-sibyl-1.0.8/sibyl/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/layouts/main_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.385771 isat-sibyl-1.0.8/sibyl/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/locales/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/locales/global.json
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/locales/pt.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.385771 isat-sibyl-1.0.8/sibyl/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/pages/start.html
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.385771 isat-sibyl-1.0.8/sibyl/sibyl-static/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/sibyl-static/flex.css
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/sibyl-static/microsite.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/sibyl-static/spa.js
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/sibyl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.385771 isat-sibyl-1.0.8/sibyl/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:40:29.389771 isat-sibyl-1.0.8/sibyl/static/favicon/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/mstile-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/mstile-310x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/mstile-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/mstile-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/favicon/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/sibyl.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-07 11:40:25.000000 isat-sibyl-1.0.8/sibyl/static/variables.css
```

### Comparing `isat-sibyl-1.0.7/PKG-INFO` & `isat-sibyl-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isat-sibyl
-Version: 1.0.7
+Version: 1.0.8
 Summary: Sibyl static site generator
 Home-page: https://github.com/isat-sibyl/sibyl
 Author: Pedro Cavalheiro
 Author-email: pedro.cavalheiro@isat.pt
 License: All rights reserved
 Project-URL: Bug Tracker, https://github.com/isat-sibyl/sibyl/issues
 Description-Content-Type: text/markdown
```

### Comparing `isat-sibyl-1.0.7/README.md` & `isat-sibyl-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/isat_sibyl.egg-info/PKG-INFO` & `isat-sibyl-1.0.8/isat_sibyl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isat-sibyl
-Version: 1.0.7
+Version: 1.0.8
 Summary: Sibyl static site generator
 Home-page: https://github.com/isat-sibyl/sibyl
 Author: Pedro Cavalheiro
 Author-email: pedro.cavalheiro@isat.pt
 License: All rights reserved
 Project-URL: Bug Tracker, https://github.com/isat-sibyl/sibyl/issues
 Description-Content-Type: text/markdown
```

### Comparing `isat-sibyl-1.0.7/isat_sibyl.egg-info/SOURCES.txt` & `isat-sibyl-1.0.8/isat_sibyl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/setup.py` & `isat-sibyl-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/build.py` & `isat-sibyl-1.0.8/sibyl/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,25 @@
     settings as settings_module,
     component,
     requirement,
     version,
     shutil_compat,
 )
 import bs4
-import markdown
 from typing import List, Set
 
 no_var_attributes = ["for-each", "render-if", "render-elif", "render-else"]
-passable_component_attributes = ["id", "class", "style"]
+passable_component_attributes = [
+    "id",
+    "class",
+    "style",
+    "onclick",
+    "onmouseover",
+    "onmouseout",
+]
 
 
 class dotdict(dict):
     """dot.notation access to dictionary attributes"""
 
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
```

### Comparing `isat-sibyl-1.0.7/sibyl/components/Accordion.html` & `isat-sibyl-1.0.8/sibyl/components/Accordion.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/Button.html` & `isat-sibyl-1.0.8/sibyl/components/Button.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/Carousel.html` & `isat-sibyl-1.0.8/sibyl/components/Carousel.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/Dialog.html` & `isat-sibyl-1.0.8/sibyl/components/Dialog.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/DoubleImageService.html` & `isat-sibyl-1.0.8/sibyl/components/DoubleImageService.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/Drawer.html` & `isat-sibyl-1.0.8/sibyl/components/Drawer.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/DrawerItem.html` & `isat-sibyl-1.0.8/sibyl/components/DrawerItem.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/Footer.html` & `isat-sibyl-1.0.8/sibyl/components/Footer.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/Header.html` & `isat-sibyl-1.0.8/sibyl/components/Header.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/ImageService.html` & `isat-sibyl-1.0.8/sibyl/components/ImageService.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/Markdown.html` & `isat-sibyl-1.0.8/sibyl/components/Markdown.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/components/SkewedBanner.html` & `isat-sibyl-1.0.8/sibyl/components/SkewedBanner.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/dev.py` & `isat-sibyl-1.0.8/sibyl/dev.py`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/helpers/component.py` & `isat-sibyl-1.0.8/sibyl/helpers/component.py`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/helpers/requirement.py` & `isat-sibyl-1.0.8/sibyl/helpers/requirement.py`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/helpers/settings.py` & `isat-sibyl-1.0.8/sibyl/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/init.py` & `isat-sibyl-1.0.8/sibyl/init.py`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/layouts/main_layout.html` & `isat-sibyl-1.0.8/sibyl/layouts/main_layout.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/locales/global.json` & `isat-sibyl-1.0.8/sibyl/locales/global.json`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/pages/index.html` & `isat-sibyl-1.0.8/sibyl/pages/index.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/pages/start.html` & `isat-sibyl-1.0.8/sibyl/pages/start.html`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/sibyl-static/flex.css` & `isat-sibyl-1.0.8/sibyl/sibyl-static/flex.css`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/sibyl-static/spa.js` & `isat-sibyl-1.0.8/sibyl/sibyl-static/spa.js`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/sibyl.py` & `isat-sibyl-1.0.8/sibyl/sibyl.py`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/android-chrome-192x192.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/android-chrome-512x512.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/apple-touch-icon.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/favicon-16x16.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/favicon-32x32.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/favicon.ico` & `isat-sibyl-1.0.8/sibyl/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/mstile-144x144.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/mstile-150x150.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/mstile-310x150.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/mstile-310x310.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/mstile-70x70.png` & `isat-sibyl-1.0.8/sibyl/static/favicon/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/favicon/safari-pinned-tab.svg` & `isat-sibyl-1.0.8/sibyl/static/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/logo.svg` & `isat-sibyl-1.0.8/sibyl/static/logo.svg`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/sibyl.svg` & `isat-sibyl-1.0.8/sibyl/static/sibyl.svg`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/styles.css` & `isat-sibyl-1.0.8/sibyl/static/styles.css`

 * *Files identical despite different names*

### Comparing `isat-sibyl-1.0.7/sibyl/static/variables.css` & `isat-sibyl-1.0.8/sibyl/static/variables.css`

 * *Files identical despite different names*

