# Comparing `tmp/Bootstrap-Flask-2.3.3.tar.gz` & `tmp/Bootstrap-Flask-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bootstrap-Flask-2.3.3.tar", last modified: Thu Nov 30 15:12:23 2023, max compression
+gzip compressed data, was "Bootstrap-Flask-2.4.0.tar", last modified: Sun Apr  7 13:17:48 2024, max compression
```

## Comparing `Bootstrap-Flask-2.3.3.tar` & `Bootstrap-Flask-2.4.0.tar`

### file list

```diff
@@ -1,299 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.989811 Bootstrap-Flask-2.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.989811 Bootstrap-Flask-2.3.3/Bootstrap_Flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-11-30 15:12:23.000000 Bootstrap-Flask-2.3.3/Bootstrap_Flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15399 2023-11-30 15:12:23.000000 Bootstrap-Flask-2.3.3/Bootstrap_Flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 15:12:23.000000 Bootstrap-Flask-2.3.3/Bootstrap_Flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 15:12:23.000000 Bootstrap-Flask-2.3.3/Bootstrap_Flask.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-30 15:12:23.000000 Bootstrap-Flask-2.3.3/Bootstrap_Flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-30 15:12:23.000000 Bootstrap-Flask-2.3.3/Bootstrap_Flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-11-30 15:12:23.989811 Bootstrap-Flask-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.909810 Bootstrap-Flask-2.3.3/flask_bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.901810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.909810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.909810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/
--rw-r--r--   0 runner    (1001) docker     (127)   162017 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   653535 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.901810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.913810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1308 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   202288 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   163958 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.913810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1678 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   191772 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   154777 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.913810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     4998 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   203947 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   165201 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.917810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     5117 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   203307 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   164810 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.917810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     3331 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   204024 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   165463 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.917810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   200515 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   162339 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.917810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   204433 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   165760 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.921810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2395 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   207845 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   168551 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.921810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     3039 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   193784 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   156467 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.921810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/
--rw-r--r--   0 runner    (1001) docker     (127)    14835 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     3988 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   240391 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   197232 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.925810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   205400 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   166554 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.925810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2481 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   193530 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   156210 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.925810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     4132 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   202572 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   164151 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.929810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2774 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   202308 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   163842 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.929810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     4574 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   206630 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   167654 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.929810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     5011 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   211917 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   172236 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.933810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     5542 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   208810 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   169827 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.933810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1673 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   204173 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   165502 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.933810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     4895 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   203906 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   165185 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.937811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/united/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/united/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1390 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/united/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   200037 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/united/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   161975 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/united/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.937811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2969 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   208339 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   169119 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.937811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/icons/
--rw-r--r--   0 runner    (1001) docker     (127)  1133693 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/icons/bootstrap-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    89476 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   137974 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/jquery.min.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.941810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/js/
--rw-r--r--   0 runner    (1001) docker     (127)    62440 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   187646 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/js/bootstrap.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.941810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/umd/
--rw-r--r--   0 runner    (1001) docker     (127)    21233 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/umd/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   123754 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/umd/popper.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.905810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.941810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/
--rw-r--r--   0 runner    (1001) docker     (127)   232948 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589161 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.905810 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.945811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   283627 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   235495 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.945811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1636 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   270367 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   223612 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.945811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     5565 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   280894 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   232736 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.949811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     5756 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   280851 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   232839 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.949811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     3421 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   282049 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   234074 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.953811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1390 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   281091 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   233208 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.953811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2480 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   283317 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   235055 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.953811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2696 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   287871 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   239085 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.957811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     3120 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   271111 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   224137 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.957811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/
--rw-r--r--   0 runner    (1001) docker     (127)    11998 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     3053 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   308042 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   256798 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.961811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2831 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   282769 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   234670 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.961811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     7226 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   303113 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   252268 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.961811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2172 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   271617 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   224632 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.965811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     6371 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   294218 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   244252 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.965811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     4264 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   283012 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   234860 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.969811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2697 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   282488 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   234361 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.969811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     4456 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   287545 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   238656 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.969811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     5721 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   291526 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   242213 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.973811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     6331 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   281262 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   233231 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.973811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   284892 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   236505 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.973811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     6399 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   281433 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   233237 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.977811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/united/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/united/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1414 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/united/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   280884 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/united/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   233057 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/united/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.977811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     4649 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   297331 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   246800 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.981811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     2718 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   286348 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   237828 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.981811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/_bootswatch.scss
--rwxr-xr-x   0 runner    (1001) docker     (127)     4259 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)   284742 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   236287 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.981811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/icons/
--rw-r--r--   0 runner    (1001) docker     (127)  1133693 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/icons/bootstrap-icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.985811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/js/
--rw-r--r--   0 runner    (1001) docker     (127)    60577 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   220350 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/js/bootstrap.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.985811 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/umd/
--rw-r--r--   0 runner    (1001) docker     (127)    20121 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/umd/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   110046 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/umd/popper.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.905810 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.985811 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/utils.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.985811 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap/table.html
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap/utils.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.985811 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap4/
--rw-r--r--   0 runner    (1001) docker     (127)    16604 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap4/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap4/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap4/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap4/table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap4/utils.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:12:23.989811 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)    16708 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap5/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap5/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap5/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap5/table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap5/utils.html
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-11-30 15:12:23.989811 Bootstrap-Flask-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-11-30 15:12:18.000000 Bootstrap-Flask-2.3.3/setup.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.788245 Bootstrap-Flask-2.4.0/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.778245 Bootstrap-Flask-2.4.0/Bootstrap_Flask.egg-info/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     6038 2024-04-07 13:17:48.000000 Bootstrap-Flask-2.4.0/Bootstrap_Flask.egg-info/PKG-INFO
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    15357 2024-04-07 13:17:48.000000 Bootstrap-Flask-2.4.0/Bootstrap_Flask.egg-info/SOURCES.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)        1 2024-04-07 13:17:48.000000 Bootstrap-Flask-2.4.0/Bootstrap_Flask.egg-info/dependency_links.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       14 2024-04-07 13:17:48.000000 Bootstrap-Flask-2.4.0/Bootstrap_Flask.egg-info/requires.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       16 2024-04-07 13:17:48.000000 Bootstrap-Flask-2.4.0/Bootstrap_Flask.egg-info/top_level.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    13017 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/LICENSE
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      141 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/MANIFEST.in
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     6038 2024-04-07 13:17:48.778245 Bootstrap-Flask-2.4.0/PKG-INFO
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4543 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/README.md
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.648245 Bootstrap-Flask-2.4.0/flask_bootstrap/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    10846 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/__init__.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.638245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.648245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.648245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   162017 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootstrap.min.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   653535 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootstrap.min.css.map
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.638245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.648245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1672 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1308 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   202288 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   163958 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.658245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      604 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1678 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   191772 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   154777 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.658245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4793 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     4998 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   203947 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   165201 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.658245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3726 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     5117 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   203307 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   164810 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.658245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4182 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     3331 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   204024 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   165463 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.658245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1225 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1492 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   200515 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   162339 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.668245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3830 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2656 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   204433 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   165760 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.668245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     8266 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2395 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   207845 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   168551 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.668245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3055 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     3039 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   193784 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   156467 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.668245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    14835 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     3988 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   240391 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   197232 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.678245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5054 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2848 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   205400 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   166554 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.688245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2483 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2481 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   193530 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   156210 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.688245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3505 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     4132 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   202572 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   164151 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.688245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2449 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2774 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   202308 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   163842 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.698245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     8430 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     4574 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   206630 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   167654 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.698245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     9314 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     5011 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   211917 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   172236 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.698245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3961 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     5542 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   208810 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   169827 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.708245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1929 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1673 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   204173 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   165502 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.708245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4646 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     4895 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   203906 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   165185 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.708245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/united/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      270 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/united/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1390 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/united/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   200037 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/united/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   161975 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/united/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.708245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     9191 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2969 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   208339 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   169119 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.708245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/icons/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)  1133693 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/icons/bootstrap-icons.svg
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    89476 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/jquery.min.js
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   137974 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/jquery.min.map
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.708245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/js/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    62440 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/js/bootstrap.min.js
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   187646 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/js/bootstrap.min.js.map
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.708245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/umd/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    21233 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/umd/popper.min.js
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   123754 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/umd/popper.min.js.map
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.648245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.718245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   232948 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootstrap.min.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   589161 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootstrap.min.css.map
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.648245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.718245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1004 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1377 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   283627 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   235495 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.718245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      469 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1636 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   270367 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   223612 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.718245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2040 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     5565 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   280894 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   232736 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.718245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1364 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     5756 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   280851 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   232839 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.728245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1622 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     3421 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   282049 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   234074 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.728245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      676 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1390 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   281091 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   233208 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.728245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1149 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2480 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   283317 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   235055 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.728245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5412 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2696 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   287871 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   239085 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.738245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2148 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     3120 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   271111 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   224137 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.738245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    11998 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     3053 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   308042 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   256798 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.738245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1493 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2831 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   282769 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   234670 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.738245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     9194 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     7226 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   303113 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   252268 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.738245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1995 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2172 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   271617 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   224632 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.748245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4852 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     6371 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   294218 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   244252 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.748245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3151 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     4264 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   283012 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   234860 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.748245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2049 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2697 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   282488 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   234361 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.748245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     7730 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     4456 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   287545 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   238656 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.748245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5752 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     5721 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   291526 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   242213 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.758245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1121 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     6331 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   281262 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   233231 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.758245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1430 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1520 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   284892 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   236505 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.758245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2141 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     6399 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   281433 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   233237 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.758245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/united/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      272 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/united/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     1414 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/united/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   280884 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/united/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   233057 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/united/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.758245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5518 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     4649 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   297331 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   246800 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.768245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5638 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2718 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   286348 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   237828 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.768245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2841 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/_bootswatch.scss
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     4259 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/_variables.scss
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   284742 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/bootstrap.css
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   236287 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/bootstrap.min.css
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.768245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/icons/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)  1133693 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/icons/bootstrap-icons.svg
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.778245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/js/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    60577 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/js/bootstrap.min.js
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   220350 2023-11-30 14:28:19.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/js/bootstrap.min.js.map
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.778245 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/umd/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    20121 2023-07-23 10:34:25.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/umd/popper.min.js
+-rw-r--r--   0 greyli    (1000) greyli    (1000)   110046 2023-07-23 10:34:25.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/umd/popper.min.js.map
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.648245 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.778245 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      948 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/nav.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4118 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/pagination.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     6856 2024-04-07 12:40:18.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/table.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1550 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/utils.html
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.778245 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      258 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap/form.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      260 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap/nav.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      271 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap/pagination.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      261 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap/table.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      260 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap/utils.html
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.778245 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap4/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    16604 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap4/form.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       30 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap4/nav.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      212 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap4/pagination.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       32 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap4/table.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1547 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap4/utils.html
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2024-04-07 13:17:48.778245 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap5/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    16744 2024-04-07 12:40:18.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap5/form.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       30 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap5/nav.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      193 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap5/pagination.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       32 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap5/table.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1321 2023-03-18 09:34:29.000000 Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap5/utils.html
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1655 2024-04-07 12:59:31.000000 Bootstrap-Flask-2.4.0/pyproject.toml
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       38 2024-04-07 13:17:48.788245 Bootstrap-Flask-2.4.0/setup.cfg
```

### Comparing `Bootstrap-Flask-2.3.3/Bootstrap_Flask.egg-info/SOURCES.txt` & `Bootstrap-Flask-2.4.0/Bootstrap_Flask.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
-setup.py
+pyproject.toml
 Bootstrap_Flask.egg-info/PKG-INFO
 Bootstrap_Flask.egg-info/SOURCES.txt
 Bootstrap_Flask.egg-info/dependency_links.txt
-Bootstrap_Flask.egg-info/not-zip-safe
 Bootstrap_Flask.egg-info/requires.txt
 Bootstrap_Flask.egg-info/top_level.txt
 flask_bootstrap/__init__.py
 flask_bootstrap/static/bootstrap4/jquery.min.js
 flask_bootstrap/static/bootstrap4/jquery.min.map
 flask_bootstrap/static/bootstrap4/css/bootstrap.min.css
 flask_bootstrap/static/bootstrap4/css/bootstrap.min.css.map
```

### Comparing `Bootstrap-Flask-2.3.3/LICENSE` & `Bootstrap-Flask-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/README.md` & `Bootstrap-Flask-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/__init__.py` & `Bootstrap-Flask-2.4.0/flask_bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootstrap.min.css.map` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cerulean/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cosmo/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/cyborg/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/darkly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/flatly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/journal/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/litera/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lumen/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/lux/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/materia/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/minty/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/pulse/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sandstone/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/simplex/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/sketchy/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/slate/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/solar/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/spacelab/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/superhero/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/united/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/united/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/united/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/united/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/united/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/united/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/css/bootswatch/yeti/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/icons/bootstrap-icons.svg` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/jquery.min.js` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/jquery.min.js`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/jquery.min.map` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/jquery.min.map`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/js/bootstrap.min.js` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/js/bootstrap.min.js.map` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/umd/popper.min.js` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap4/umd/popper.min.js.map` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap4/umd/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootstrap.min.css.map` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cerulean/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cosmo/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/cyborg/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/darkly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/flatly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/journal/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/litera/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lumen/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/lux/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/materia/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/minty/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/morph/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/pulse/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/quartz/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sandstone/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/simplex/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/sketchy/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/slate/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/solar/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/spacelab/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/superhero/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/united/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/united/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/united/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/united/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/united/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/united/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/vapor/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/yeti/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/_bootswatch.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/_variables.scss` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/_variables.scss`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/bootstrap.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/bootstrap.min.css` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/css/bootswatch/zephyr/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/icons/bootstrap-icons.svg` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/js/bootstrap.min.js` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/js/bootstrap.min.js.map` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/umd/popper.min.js` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/static/bootstrap5/umd/popper.min.js.map` & `Bootstrap-Flask-2.4.0/flask_bootstrap/static/bootstrap5/umd/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/nav.html` & `Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/nav.html`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/pagination.html` & `Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/pagination.html`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/table.html` & `Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/table.html`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 {% macro render_table(data,
                       titles=None,
                       primary_key='id',
                       primary_key_title='#',
                       caption=None,
                       table_classes=None,
                       header_classes=None,
+                      body_classes=None,
                       responsive=False,
                       responsive_class='table-responsive',
                       safe_columns=None,
                       urlize_columns=None,
                       model=None,
                       show_actions=False,
                       actions_title='Actions',
@@ -71,15 +72,15 @@
                 {{ render_icon('plus-circle-fill') }}
             </a>
         {% endif %}
         </th>
     {% endif %}
     </tr>
     </thead>
-    <tbody>
+    <tbody{% if body_classes %} class="{{ body_classes }}"{% endif %}>
     {% for row in data %}
     <tr>
         {% for title in titles %}
         {% set key = title[0] %}
         {% set value = row[key] %}
         {%- if key == primary_key -%}
             <th scope="row">
```

#### html2text {}

```diff
@@ -7,20 +7,20 @@
 in db_field %} {%- set db_field = db_field[1:].split('.') -%} {%- do
 url_params.update({url_parameter: record[db_field[0]][db_field[1]]}) -%} {%
 elif db_field.startswith(':') %} {%- set db_field = db_field[1:] -%} {%- do
 url_params.update({url_parameter: record[db_field]}) -%} {% else %} {%- do
 url_params.update({url_parameter: db_field}) -%} {% endif %} {% endfor %} {
 { arg_url_for(endpoint, url_params) }} {%- endwith %} {%- endmacro %} {% macro
 render_table(data, titles=None, primary_key='id', primary_key_title='#',
-caption=None, table_classes=None, header_classes=None, responsive=False,
-responsive_class='table-responsive', safe_columns=None, urlize_columns=None,
-model=None, show_actions=False, actions_title='Actions', custom_actions=None,
-view_url=None, edit_url=None, delete_url=None, new_url=None,
-action_pk_placeholder=':id') %} {% if not titles %} {% set titles =
-get_table_titles(data, primary_key, primary_key_title) %} {% endif %} {% if
+caption=None, table_classes=None, header_classes=None, body_classes=None,
+responsive=False, responsive_class='table-responsive', safe_columns=None,
+urlize_columns=None, model=None, show_actions=False, actions_title='Actions',
+custom_actions=None, view_url=None, edit_url=None, delete_url=None,
+new_url=None, action_pk_placeholder=':id') %} {% if not titles %} {% set titles
+= get_table_titles(data, primary_key, primary_key_title) %} {% endif %} {% if
 responsive %}
 {% endif %}
                {{{{ aaccttiioonnss__ttiittllee }}}} {{%% iiff nneeww__uurrll
                %%}}
                %% iiff nneeww__uurrll..ssttaarrttsswwiitthh((''//'')) %%}}
                hhrreeff==""{{{{ nneeww__uurrll }}}}"" {{%% eellssee %%}}
 {{{{ ttiittllee[[11]] }}}} hhrreeff==""{{{{ uurrll__ffoorr((nneeww__uurrll)) }}}}"" {{%%
```

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/templates/base/utils.html` & `Bootstrap-Flask-2.4.0/flask_bootstrap/templates/base/utils.html`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap4/form.html` & `Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap4/form.html`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap4/utils.html` & `Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap4/utils.html`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap5/form.html` & `Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap5/form.html`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 {{ field.label(class="form-check-label", for=field.id)|safe }}
                 {%- if field.errors %}
                     {%- for error in field.errors %}
                         <div class="invalid-feedback d-block">{{ error }}</div>
                     {%- endfor %}
                 {%- elif field.description -%}
                     {% call _hz_form_wrap(horizontal_columns, form_type, required=required) %}
-                        <small class="form-text text-muted">{{ field.description|safe }}</small>
+                        <small class="form-text text-body-secondary">{{ field.description|safe }}</small>
                     {% endcall %}
                 {%- endif %}
             </div>
         {% endcall %}
     {%- elif field.type == 'RadioField' -%}
         {# note: A cleaner solution would be rendering depending on the widget,
      this is just a hack for now, until I can think of something better #}
@@ -107,15 +107,15 @@
           </div>
         {% endif %}
         {%- if field.errors %}
             {%- for error in field.errors %}
                 <div class="invalid-feedback d-block">{{ error }}</div>
             {%- endfor %}
         {%- elif field.description -%}
-            <small class="form-text text-muted">{{ field.description|safe }}</small>
+            <small class="form-text text-body-secondary">{{ field.description|safe }}</small>
         {%- endif %}
         </div>
     {%- elif field.type == 'SubmitField' -%}
         {# deal with jinja scoping issues? #}
         {% set field_kwargs = kwargs %}
         {# note: same issue as above - should check widget, not field type #}
         {% call _hz_form_wrap(horizontal_columns, form_type, True, required=required) %}
@@ -192,15 +192,15 @@
                     {%- for error in field.errors %}
                         {% call _hz_form_wrap(horizontal_columns, form_type, required=required) %}
                             <div class="invalid-feedback d-block">{{ error }}</div>
                         {% endcall %}
                     {%- endfor %}
                 {%- elif field.description -%}
                     {% call _hz_form_wrap(horizontal_columns, form_type, required=required) %}
-                        <small class="form-text text-muted">{{ field.description|safe }}</small>
+                        <small class="form-text text-body-secondary">{{ field.description|safe }}</small>
                     {% endcall %}
                 {%- endif %}
             {%- else -%}
                 {{ field.label(class="form-label")|safe }}
                 {%- if field.type in ['DecimalRangeField', 'IntegerRangeField'] %}
                     {% if field.errors %}
                         {{ field(class="form-range is-invalid%s" % extra_classes, **kwargs)|safe }}
@@ -221,15 +221,15 @@
                     {% endif %}
                 {%- endif %}
                 {%- if field.errors %}
                     {%- for error in field.errors %}
                         <div class="invalid-feedback d-block">{{ error }}</div>
                     {%- endfor %}
                 {%- elif field.description -%}
-                    <small class="form-text text-muted">{{ field.description|safe }}</small>
+                    <small class="form-text text-body-secondary">{{ field.description|safe }}</small>
                 {%- endif %}
             {%- endif %}
         </div>
     {% endif %}
 {% endmacro %}
 
 {# valid form types are "basic", "inline" and "horizontal" #}
```

### Comparing `Bootstrap-Flask-2.3.3/flask_bootstrap/templates/bootstrap5/utils.html` & `Bootstrap-Flask-2.4.0/flask_bootstrap/templates/bootstrap5/utils.html`

 * *Files identical despite different names*

### Comparing `Bootstrap-Flask-2.3.3/setup.py` & `Bootstrap-Flask-2.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,46 @@
-"""
-Bootstrap-Flask
----------------
+[project]
+name = "Bootstrap-Flask"
+version = "2.4.0"
+description = "Bootstrap 4 & 5 helper for your Flask projects."
+readme = "README.md"
+license = { text = "MIT" }
+authors = [{ name = "Grey Li", email = "withlihui@gmail.com" }]
+classifiers = [
+    'Development Status :: 5 - Production/Stable',
+    'Environment :: Web Environment',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: MIT License',
+    'Operating System :: OS Independent',
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
+    'Framework :: Flask',
+    'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
+    'Topic :: Software Development :: Libraries :: Python Modules',
+]
+dependencies = ["Flask", "WTForms"]
 
-Bootstrap-Flask is a collection of Jinja macros for Bootstrap 4 & 5 and Flask.
-It helps you to render Flask-related objects and data to Bootstrap HTML more easily.
+[project.urls]
+Documentation = "https://bootstrap-flask.readthedocs.io/en/stable/"
+Changes = "https://bootstrap-flask.readthedocs.io/en/stable/changelog/"
+"Source Code" = "https://github.com/helloflask/bootstrap-flask/"
+"Issue Tracker" = "https://github.com/helloflask/bootstrap-flask/issues/"
+Funding = "https://opencollective.com/bootstrap-flask"
+Discussions = "https://github.com/helloflask/bootstrap-flask/discussions/"
 
-If you come from Flask-Bootstrap, check out
-[this tutorial](https://bootstrap-flask.readthedocs.io/en/stable/migrate/)
-on how to migrate to this extension.
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
-Go to [GitHub page](https://github.com/helloflask/bootstrap-flask), which you
-can check for more details.
-"""
-from setuptools import setup
+[tool.pytest.ini_options]
+testpaths = ["tests"]
 
-setup(
-    name='Bootstrap-Flask',
-    version='2.3.3',
-    url='https://github.com/helloflask/bootstrap-flask',
-    project_urls={
-        'Documentation': 'https://bootstrap-flask.readthedocs.io/en/stable/',
-        'Funding': 'https://opencollective.com/bootstrap-flask',
-        'Changes': 'https://bootstrap-flask.readthedocs.io/en/stable/changelog/',
-        'Source Code': 'https://github.com/helloflask/bootstrap-flask/',
-        'Issue Tracker': 'https://github.com/helloflask/bootstrap-flask/issues/',
-        'Discussions': 'https://github.com/helloflask/bootstrap-flask/discussions/'
-    },
-    license='MIT',
-    author='Grey Li',
-    author_email='withlihui@gmail.com',
-    description='Bootstrap 4 & 5 helper for your Flask projects.',
-    long_description=__doc__,
-    long_description_content_type='text/markdown',
-    platforms='any',
-    packages=['flask_bootstrap'],
-    zip_safe=False,
-    include_package_data=True,
-    test_suite='tests',
-    install_requires=[
-        'Flask',
-        'WTForms'
-    ],
-    keywords='flask extension development',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Framework :: Flask',
-        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
-        'Topic :: Software Development :: Libraries :: Python Modules'
-    ]
-)
+[tool.coverage.run]
+source = ["flask_bootstrap"]
+
+[tool.coverage.report]
+exclude_lines = ["pragma: no cover", " except ImportError:"]
```

