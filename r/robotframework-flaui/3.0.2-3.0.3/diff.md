# Comparing `tmp/robotframework-flaui-3.0.2.tar.gz` & `tmp/robotframework-flaui-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-flaui-3.0.2.tar", last modified: Fri Mar  8 21:00:38 2024, max compression
+gzip compressed data, was "robotframework-flaui-3.0.3.tar", last modified: Sun Apr  7 17:06:55 2024, max compression
```

## Comparing `robotframework-flaui-3.0.2.tar` & `robotframework-flaui-3.0.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.157792 robotframework-flaui-3.0.2/
--rw-rw-rw-   0        0        0     1079 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/LICENSE
--rw-rw-rw-   0        0        0       40 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8998 2024-03-08 21:00:38.157792 robotframework-flaui-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7921 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/README.md
--rw-rw-rw-   0        0        0       81 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      103 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.157792 robotframework-flaui-3.0.2/robotframework_flaui.egg-info/
--rw-rw-rw-   0        0        0     8998 2024-03-08 21:00:37.000000 robotframework-flaui-3.0.2/robotframework_flaui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3054 2024-03-08 21:00:37.000000 robotframework-flaui-3.0.2/robotframework_flaui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 21:00:37.000000 robotframework-flaui-3.0.2/robotframework_flaui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-03-08 21:00:37.000000 robotframework-flaui-3.0.2/robotframework_flaui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-08 21:00:37.000000 robotframework-flaui-3.0.2/robotframework_flaui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-08 21:00:38.157792 robotframework-flaui-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1988 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:37.966845 robotframework-flaui-3.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:37.998075 robotframework-flaui-3.0.2/src/FlaUILibrary/
--rw-rw-rw-   0        0        0     8747 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:37.998075 robotframework-flaui-3.0.2/src/FlaUILibrary/bin/
--rw-rw-rw-   0        0        0   256512 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/bin/FlaUI.Core.dll
--rw-rw-rw-   0        0        0    76288 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/bin/FlaUI.UIA2.dll
--rw-rw-rw-   0        0        0   105984 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/bin/FlaUI.UIA3.dll
--rw-rw-rw-   0        0        0   151040 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:37.998075 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/
--rw-rw-rw-   0        0        0        0 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.093914 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/automation/
--rw-rw-rw-   0        0        0       46 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/automation/__init__.py
--rw-rw-rw-   0        0        0     5479 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/automation/uia.py
--rw-rw-rw-   0        0        0     1062 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/automation/uia2.py
--rw-rw-rw-   0        0        0     1062 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/automation/uia3.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.093914 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/enum/
--rw-rw-rw-   0        0        0      127 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/enum/__init__.py
--rw-rw-rw-   0        0        0      305 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/enum/interfacetype.py
--rw-rw-rw-   0        0        0      163 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/enum/screenshotmode.py
--rw-rw-rw-   0        0        0      229 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/enum/treeitemaction.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.109490 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/exception/
--rw-rw-rw-   0        0        0       36 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/exception/__init__.py
--rw-rw-rw-   0        0        0     3107 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/exception/flauierror.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.109490 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/interface/
--rw-rw-rw-   0        0        0      158 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/interface/__init__.py
--rw-rw-rw-   0        0        0      737 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/interface/moduleinterface.py
--rw-rw-rw-   0        0        0      248 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/interface/valuecontainer.py
--rw-rw-rw-   0        0        0     1289 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.126425 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/
--rw-rw-rw-   0        0        0      484 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/__init__.py
--rw-rw-rw-   0        0        0    12745 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/application.py
--rw-rw-rw-   0        0        0     2512 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/checkbox.py
--rw-rw-rw-   0        0        0     2146 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/combobox.py
--rw-rw-rw-   0        0        0     2179 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/debug.py
--rw-rw-rw-   0        0        0    18162 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/element.py
--rw-rw-rw-   0        0        0     6762 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/grid.py
--rw-rw-rw-   0        0        0     7598 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/keyboard.py
--rw-rw-rw-   0        0        0    17116 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/mouse.py
--rw-rw-rw-   0        0        0    18010 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/property.py
--rw-rw-rw-   0        0        0     8595 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/screenshot.py
--rw-rw-rw-   0        0        0     9645 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/selector.py
--rw-rw-rw-   0        0        0     3224 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/tab.py
--rw-rw-rw-   0        0        0     2613 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/textbox.py
--rw-rw-rw-   0        0        0     1698 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/tooglebutton.py
--rw-rw-rw-   0        0        0     6711 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/tree.py
--rw-rw-rw-   0        0        0     1925 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/window.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.142074 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/
--rw-rw-rw-   0        0        0      262 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/__init__.py
--rw-rw-rw-   0        0        0     1183 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/automationelement.py
--rw-rw-rw-   0        0        0     1103 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/automationinterfacecontainer.py
--rw-rw-rw-   0        0        0     2101 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/converter.py
--rw-rw-rw-   0        0        0     7532 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/keyboardinputconverter.py
--rw-rw-rw-   0        0        0     5525 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/treeitems.py
--rw-rw-rw-   0        0        0     1728 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/treeitemsparser.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.157792 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/
--rw-rw-rw-   0        0        0      668 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0    10568 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/application.py
--rw-rw-rw-   0        0        0     2643 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/checkbox.py
--rw-rw-rw-   0        0        0    10343 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/combobox.py
--rw-rw-rw-   0        0        0     2473 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/debug.py
--rw-rw-rw-   0        0        0    17790 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/element.py
--rw-rw-rw-   0        0        0     5545 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/grid.py
--rw-rw-rw-   0        0        0    10868 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/keyboard.py
--rw-rw-rw-   0        0        0     8242 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/listbox.py
--rw-rw-rw-   0        0        0    22978 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/mouse.py
--rw-rw-rw-   0        0        0    33400 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/property.py
--rw-rw-rw-   0        0        0     2692 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/radiobutton.py
--rw-rw-rw-   0        0        0     4427 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/screenshot.py
--rw-rw-rw-   0        0        0     2532 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/tab.py
--rw-rw-rw-   0        0        0     2527 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/textbox.py
--rw-rw-rw-   0        0        0     1505 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/togglebutton.py
--rw-rw-rw-   0        0        0    13454 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/tree.py
--rw-rw-rw-   0        0        0     1247 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/uia.py
--rw-rw-rw-   0        0        0     1357 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/window.py
--rw-rw-rw-   0        0        0      838 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/pythonnetwrapper.py
-drwxrwxrwx   0        0        0        0 2024-03-08 21:00:38.157792 robotframework-flaui-3.0.2/src/FlaUILibrary/robotframework/
--rw-rw-rw-   0        0        0        0 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/robotframework/__init__.py
--rw-rw-rw-   0        0        0     1041 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/robotframework/robotlog.py
--rw-rw-rw-   0        0        0       18 2024-03-08 20:59:54.000000 robotframework-flaui-3.0.2/src/FlaUILibrary/version.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/
+-rw-rw-rw-   0        0        0     1079 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0       40 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8998 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7921 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/README.md
+-rw-rw-rw-   0        0        0       81 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      103 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/
+-rw-rw-rw-   0        0        0     8998 2024-04-07 17:06:54.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3054 2024-04-07 17:06:55.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 17:06:54.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-04-07 17:06:54.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-07 17:06:54.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1988 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.021331 robotframework-flaui-3.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/
+-rw-rw-rw-   0        0        0     8747 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/
+-rw-rw-rw-   0        0        0   256512 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.Core.dll
+-rw-rw-rw-   0        0        0    76288 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.UIA2.dll
+-rw-rw-rw-   0        0        0   105984 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.UIA3.dll
+-rw-rw-rw-   0        0        0   151040 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/
+-rw-rw-rw-   0        0        0       46 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/__init__.py
+-rw-rw-rw-   0        0        0     5479 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia.py
+-rw-rw-rw-   0        0        0     1062 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia2.py
+-rw-rw-rw-   0        0        0     1062 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia3.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/
+-rw-rw-rw-   0        0        0      127 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/__init__.py
+-rw-rw-rw-   0        0        0      305 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/interfacetype.py
+-rw-rw-rw-   0        0        0      163 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/screenshotmode.py
+-rw-rw-rw-   0        0        0      229 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/treeitemaction.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.068210 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/exception/
+-rw-rw-rw-   0        0        0       36 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/exception/__init__.py
+-rw-rw-rw-   0        0        0     3268 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/exception/flauierror.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.068210 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/
+-rw-rw-rw-   0        0        0      158 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/__init__.py
+-rw-rw-rw-   0        0        0      737 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/moduleinterface.py
+-rw-rw-rw-   0        0        0      248 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/valuecontainer.py
+-rw-rw-rw-   0        0        0     1289 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.083830 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/
+-rw-rw-rw-   0        0        0      484 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/__init__.py
+-rw-rw-rw-   0        0        0    12745 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/application.py
+-rw-rw-rw-   0        0        0     2512 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/checkbox.py
+-rw-rw-rw-   0        0        0     2146 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/combobox.py
+-rw-rw-rw-   0        0        0     2179 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/debug.py
+-rw-rw-rw-   0        0        0    18162 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/element.py
+-rw-rw-rw-   0        0        0     7948 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/grid.py
+-rw-rw-rw-   0        0        0     7598 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/keyboard.py
+-rw-rw-rw-   0        0        0    17116 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/mouse.py
+-rw-rw-rw-   0        0        0    18010 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/property.py
+-rw-rw-rw-   0        0        0     8595 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/screenshot.py
+-rw-rw-rw-   0        0        0     9645 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/selector.py
+-rw-rw-rw-   0        0        0     3224 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tab.py
+-rw-rw-rw-   0        0        0     2613 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/textbox.py
+-rw-rw-rw-   0        0        0     1698 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tooglebutton.py
+-rw-rw-rw-   0        0        0     6756 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tree.py
+-rw-rw-rw-   0        0        0     1925 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/window.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.083830 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/
+-rw-rw-rw-   0        0        0      262 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/__init__.py
+-rw-rw-rw-   0        0        0     1183 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/automationelement.py
+-rw-rw-rw-   0        0        0     1103 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/automationinterfacecontainer.py
+-rw-rw-rw-   0        0        0     2101 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/converter.py
+-rw-rw-rw-   0        0        0     7532 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/keyboardinputconverter.py
+-rw-rw-rw-   0        0        0     5617 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/treeitems.py
+-rw-rw-rw-   0        0        0     1825 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/treeitemsparser.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.099455 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/
+-rw-rw-rw-   0        0        0      668 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0    10568 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/application.py
+-rw-rw-rw-   0        0        0     2643 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/checkbox.py
+-rw-rw-rw-   0        0        0    10343 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/combobox.py
+-rw-rw-rw-   0        0        0     2473 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/debug.py
+-rw-rw-rw-   0        0        0    17790 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/element.py
+-rw-rw-rw-   0        0        0     6805 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/grid.py
+-rw-rw-rw-   0        0        0    10868 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/keyboard.py
+-rw-rw-rw-   0        0        0     8242 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/listbox.py
+-rw-rw-rw-   0        0        0    22978 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/mouse.py
+-rw-rw-rw-   0        0        0    33400 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/property.py
+-rw-rw-rw-   0        0        0     2692 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/radiobutton.py
+-rw-rw-rw-   0        0        0     4427 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     2532 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/tab.py
+-rw-rw-rw-   0        0        0     2527 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/textbox.py
+-rw-rw-rw-   0        0        0     1505 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/togglebutton.py
+-rw-rw-rw-   0        0        0    14122 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/tree.py
+-rw-rw-rw-   0        0        0     1247 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/uia.py
+-rw-rw-rw-   0        0        0     1357 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/window.py
+-rw-rw-rw-   0        0        0      838 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/pythonnetwrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/src/FlaUILibrary/robotframework/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/robotframework/__init__.py
+-rw-rw-rw-   0        0        0     1041 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/robotframework/robotlog.py
+-rw-rw-rw-   0        0        0       18 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/version.py
```

### Comparing `robotframework-flaui-3.0.2/LICENSE` & `robotframework-flaui-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/PKG-INFO` & `robotframework-flaui-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-flaui
-Version: 3.0.2
+Version: 3.0.3
 Summary: Windows GUI testing library for Robot Framework
 Home-page: https://github.com/GDATASoftwareAG/robotframework-flaui
 Author: G DATA CyberDefense AG
 Author-email: opensource@gdata.de
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-flaui-3.0.2/README.md` & `robotframework-flaui-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/robotframework_flaui.egg-info/PKG-INFO` & `robotframework-flaui-3.0.3/robotframework_flaui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-flaui
-Version: 3.0.2
+Version: 3.0.3
 Summary: Windows GUI testing library for Robot Framework
 Home-page: https://github.com/GDATASoftwareAG/robotframework-flaui
 Author: G DATA CyberDefense AG
 Author-email: opensource@gdata.de
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-flaui-3.0.2/robotframework_flaui.egg-info/SOURCES.txt` & `robotframework-flaui-3.0.3/robotframework_flaui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/setup.py` & `robotframework-flaui-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/__init__.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/bin/FlaUI.Core.dll` & `robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.Core.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/bin/FlaUI.UIA2.dll` & `robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.UIA2.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/bin/FlaUI.UIA3.dll` & `robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.UIA3.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll` & `robotframework-flaui-3.0.3/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/automation/uia.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/automation/uia2.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia2.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/automation/uia3.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia3.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/exception/flauierror.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/exception/flauierror.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     FalseSyntax = "Incorrect syntax usage '{}'"
     ArgumentShouldBeList = "The given argument should be an array"
     ArgumentShouldNotBeList = "The given argument should not be an array"
     PropertyNotSupported = "Property from element is not supported"
     PropertyNotEqual = "Property value '{}' not equal to expected value '{}'"
     InvalidPropertyArgument = "Set Property can not be executed by Get Property From Element"
     PatternNotSupported = "Supports '{}' Pattern only, method cannot be used with invalid Pattern"
+    InvalidSeparator = "Try to set invalid separator"
+    GridIsSingleSelect = "The Grid only supports single select. Change the muliselect argument to false"
 
     @staticmethod
     def raise_fla_ui_error(message):
         """
         Static method usage to raise an FlaUI exception
 
         Args:
```

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/interface/moduleinterface.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/moduleinterface.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/application.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/application.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/checkbox.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/checkbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/combobox.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/combobox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/debug.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/element.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/element.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/keyboard.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/keyboard.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/mouse.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/mouse.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/property.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/property.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/screenshot.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/screenshot.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/selector.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/selector.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/tab.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tab.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/textbox.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/textbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/tooglebutton.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tooglebutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/tree.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,24 @@
 
 class Tree(ModuleInterface):
     """
     Tree control wrapper for FlaUI usage.
     Wrapper module executes methods from Tree.cs implementation.
     """
 
+    def __init__(self):
+        self._seperator = "->"
+
     class Container(ValueContainer):
         """
         Value container from tree module.
         """
         element: Optional[Any]
         item: Optional[str]
+        seperator: Optional[str]
 
     class Action(Enum):
         """
         Supported actions for execute action implementation.
         """
         GET_ROOT_ITEMS_COUNT = "GET_ROOT_ITEMS_COUNT"
         GET_VISIBLE_ITEMS_COUNT = "GET_VISIBLE_ITEMS_COUNT"
@@ -32,75 +36,36 @@
         COLLAPSE_ALL = "COLLAPSE_ALL"
         SELECT_ITEM_BY_NAME = "SELECT_ITEM_BY_NAME"
         SELECT_ITEM = "SELECT_ITEM"
         EXPAND_ITEM = "EXPAND_ITEM"
         COLLAPSE_ITEM = "COLLAPSE_ITEM"
         SELECTED_ITEM_SHOULD_BE = "SELECTED_ITEM_SHOULD_BE"
         GET_SELECTED_ITEMS_NAME = "GET_SELECTED_ITEMS_NAME"
+        SET_SEPERATOR = "SET_SEPERATOR"
 
     @staticmethod
-    def create_value_container(element=None, item=None):
+    def create_value_container(element=None, item=None, seperator=None):
         """
         Helper to create container object.
 
         Raises:
             FlaUiError: If creation from container object failed by invalid values.
 
         Args:
             element (Object): Tree element to execute action
             item (String): Value from item to use
+            seperator (String): Seperator to split up tree items.
         """
         return Tree.Container(element=element,
-                              item=Converter.cast_to_string(item))
+                              item=Converter.cast_to_string(item),
+                              seperator=seperator)
 
     def execute_action(self, action: Action, values: Container):
         """If action is not supported an ActionNotSupported error will be raised.
 
-        Supported actions for checkbox usages are:
-
-          *  Action.GET_ROOT_ITEMS_COUNT
-            * values ["element"]
-            * Returns : (integer) count of tree items in the root level
-
-          *  Action.GET_VISIBLE_ITEMS_COUNT
-            * values ["element"]
-            * Returns : (integer) count of every visible tree item.
-
-          *  Action.GET_VISIBLE_ITEMS_NAME
-            * values ["element"]
-            * Returns : (Array) names of every visible tree item.
-
-        *  Action.ITEM_SHOULD_BE_VISIBLE
-            * values ["element", "item"]
-            * Returns : None
-
-          *  Action.EXPAND_ALL
-            * values ["element"]
-            * Returns : None
-
-          *  Action.COLLAPSE_ALL
-            * values ["element"]
-            * Returns : None
-
-          *  Action.SELECT_ITEM_BY_NAME
-            * values ["element", "item"]
-            * Returns : None
-
-          *  Action.SELECT_ITEM
-            * values ["element", "item"]
-            * Returns : None
-
-        *  Action.SELECTED_ITEM_SHOULD_BE
-            * values ["element", "item"]
-            * Returns : None
-
-        *  Action.GET_SELECTED_ITEMS_NAME
-            * values ["element"]
-            * Returns : String the name of selected items.
-
         Raises:
             FlaUiError: If action is not supported.
 
         Args:
             action (Action): Action to use.
             values (Object): See action definitions for value usage.
         """
@@ -116,27 +81,54 @@
             self.Action.GET_VISIBLE_ITEMS_COUNT:
                 lambda: TreeItems.get_visible_leaf_count(values["element"].Items),
             self.Action.ITEM_SHOULD_BE_VISIBLE:
                 lambda: self._should_be_visible(values["element"], values["item"]),
             self.Action.SELECT_ITEM_BY_NAME:
                 lambda: TreeItems.select_visible_node_by_name(values["element"].Items, values["item"]),
             self.Action.SELECT_ITEM:
-                lambda: TreeItems.execute_by_location(values["element"].Items, values["item"], TreeItemAction.SELECT),
+                lambda: TreeItems.execute_by_location(values["element"].Items,
+                                                      values["item"],
+                                                      self._seperator,
+                                                      TreeItemAction.SELECT),
             self.Action.EXPAND_ITEM:
-                lambda: TreeItems.execute_by_location(values["element"].Items, values["item"], TreeItemAction.EXPAND),
+                lambda: TreeItems.execute_by_location(values["element"].Items,
+                                                      values["item"],
+                                                      self._seperator,
+                                                      TreeItemAction.EXPAND),
             self.Action.COLLAPSE_ITEM:
-                lambda: TreeItems.execute_by_location(values["element"].Items, values["item"], TreeItemAction.COLLAPSE),
+                lambda: TreeItems.execute_by_location(values["element"].Items,
+                                                      values["item"],
+                                                      self._seperator,
+                                                      TreeItemAction.COLLAPSE),
             self.Action.SELECTED_ITEM_SHOULD_BE:
                 lambda: self._selected_item_should_be(values["element"], values["item"]),
             self.Action.GET_SELECTED_ITEMS_NAME:
                 lambda: self._get_selected_items_name(values["element"]),
+            self.Action.SET_SEPERATOR:
+                lambda: self._set_seperator(values["seperator"]),
         }
 
         return switcher.get(action, lambda: FlaUiError.raise_fla_ui_error(FlaUiError.ActionNotSupported))()
 
+    def _set_seperator(self, seperator):
+        """
+        Sets specific seperator to split up tree items.
+
+        Args:
+            seperator (Object): Seperator to split items.
+
+        Raises:
+            FlaUiError: If seperator is invalid to set
+        """
+        if seperator is None:
+            raise FlaUiError(FlaUiError.InvalidSeparator)
+
+        self._seperator = seperator
+
+
     @staticmethod
     def _should_be_visible(control: Any, name: str):
         """
         Checks if Tree contains a given item by name.
 
         Args:
             control (Object): Tree control element from FlaUI.
```

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/module/window.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/window.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/automationelement.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/automationelement.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/automationinterfacecontainer.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/automationinterfacecontainer.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/converter.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/converter.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/keyboardinputconverter.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/keyboardinputconverter.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/treeitems.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/treeitems.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,29 +86,30 @@
         Raises:
             FlaUiError: If node by a given name could not be found.
         """
         if not TreeItems._find_visible_node_by_name(nodes, name):
             raise FlaUiError(FlaUiError.ElementNameNotFound.format(name))
 
     @staticmethod
-    def execute_by_location(nodes: Any, location: str, action: TreeItemAction):
+    def execute_by_location(nodes: Any, location: str, seperator: str, action: TreeItemAction):
         """
         Executes the given TreeItemAction to the last element from a tree location.
 
         Args:
             nodes (Object): TreeItems[] from current node
             location (String): Location string to execute operations on nodes.
+            seperator (String): Seperator to split up tree items
             action (TreeItemAction) : Action to operate on node.
 
         Raises:
             FlaUiError: If action is not supported.
             FlaUiError: If location syntax is wrong.
             FlaUiError: If node is not expandable.
         """
-        parser = TreeItemsParser(location)
+        parser = TreeItemsParser(location, seperator)
         current_nodes = nodes
 
         for index in range(len(parser.location)):
             node = parser.get_treeitem(current_nodes, index)
             if parser.is_last_element(index):
                 try:
                     if action == TreeItemAction.EXPAND:
```

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/flaui/util/treeitemsparser.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/treeitemsparser.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,33 +8,36 @@
     The location is used to locate the exact tree item in the tree control.
     Examples:
     location = N:Nameofitem1->N:Nameofitem2->N:Nameofitem3
     location = I:indexofitem1->I:indexofitem2->I:indexofitem3
     location = N:Nameofitem1->I:indexofitem2->I:indexofitem3
     """
 
-    def __init__(self, location):
-        self.location = location.split("->")
+    IndexSeperator = "I:"
+    NameSeperator = "N:"
+
+    def __init__(self, location, seperator):
+        self.location = location.split(seperator)
 
     def get_treeitem(self, treeitems: Any, index: Any):
         """
         This function gets the index of the location, the location can either be a name or index,
         and returns the corresponding tree item to that name or index.
         if the given name or index is not found a flauierror will be thrown.
         """
         loc = self.location[index]
 
-        if loc.startswith("I:"):
+        if loc.startswith(self.IndexSeperator):
             loc = loc[2:]
             try:
                 return treeitems[int(loc)]
             except IndexError:
                 raise FlaUiError(FlaUiError.ArrayOutOfBoundException.format(int(loc))) from None
 
-        elif loc.startswith("N:"):
+        elif loc.startswith(self.NameSeperator):
             loc = loc[2:]
             for item in treeitems:
                 if item.Name == loc:
                     return item
             raise FlaUiError(FlaUiError.ElementNameNotFound.format(loc))
         else:
             raise FlaUiError(FlaUiError.FalseSyntax.format(loc)) from None
```

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/__init__.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/application.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/application.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/checkbox.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/checkbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/combobox.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/combobox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/debug.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/element.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/element.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/grid.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/grid.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,14 +44,44 @@
         """
         module = self._container.create_or_get_module()
         element = module.get_element(identifier, InterfaceType.LISTVIEW, msg)
         return module.action(Grid.Action.GET_ALL_DATA, Grid.create_value_container(element=element),
                              msg)
 
     @keyword
+    def get_header_from_grid(self, identifier, msg=None):
+        """
+        Get header from a grid as an array collection.
+
+        Includes all header values as first element from list.
+
+        For example data grid:
+        [
+          [ "Value_1", "Value_2", "Value_3" ],
+          [ "Data_1", "Data_2", "Data_3" ],
+        ]
+
+        XPaths syntax is explained in `XPath locator`.
+
+        If element could not be found by xpath an error message will be thrown.
+
+        Arguments:
+        | Argument   | Type   | Description                   |
+        | identifier | string | XPath identifier from element |
+        | msg        | string | Custom error message          |
+
+        Examples:
+        | ${data}  Get Header From Grid  <XPath>   |
+        """
+        module = self._container.create_or_get_module()
+        element = module.get_element(identifier, InterfaceType.LISTVIEW, msg)
+        return module.action(Grid.Action.GET_HEADER, Grid.create_value_container(element=element),
+                             msg)
+
+    @keyword
     def get_selected_grid_rows(self, identifier, msg=None):
         """
         Get all selected rows as string. Representation for each cell is a pipe. If nothing is selected empty string
         will be returned.
 
         For example:
           | Value_1 | Value_2 | Value_3 |
@@ -70,62 +100,64 @@
         """
         module = self._container.create_or_get_module()
         element = module.get_element(identifier, InterfaceType.LISTVIEW, msg)
         return module.action(Grid.Action.GET_SELECTED_ROWS, Grid.create_value_container(element=element),
                              msg)
 
     @keyword
-    def select_grid_row_by_index(self, identifier, index, msg=None):
+    def select_grid_row_by_index(self, identifier, index, multiselect=True, msg=None):
         """
         Select rows from data grid with the given index.
 
         XPaths syntax is explained in `XPath locator`.
 
         If element could not be found by xpath an error message will be thrown.
 
         Arguments:
         | Argument   | Type   | Description                   |
         | identifier | string | XPath identifier from element |
         | index      | string | IndexNumber                   |
+        | multiselect | bool   | Multiselect availble or not  |
         | msg        | string | Custom error message          |
 
         Examples:
         | Select Grid Row By Index  <XPath>  <INDEX>      |
 
         """
         module = self._container.create_or_get_module()
         element = module.get_element(identifier, InterfaceType.LISTVIEW, msg)
         module.action(Grid.Action.SELECT_ROW_BY_INDEX,
-                      Grid.create_value_container(element=element, index=index),
+                      Grid.create_value_container(element=element, index=index, multiselect=multiselect),
                       msg)
 
     @keyword
-    def select_grid_row_by_name(self, identifier, index, name, msg=None):
+    def select_grid_row_by_name(self, identifier, index, name, multiselect=True, msg=None):
         """
         Select specific row by name from data grid.
 
         XPaths syntax is explained in `XPath locator`.
 
         If element could not be found by xpath an error message will be thrown.
 
         Arguments:
         | Argument   | Type   | Description                   |
         | identifier | string | XPath identifier from element |
         | index      | string | Column IndexNumber            |
         | name       | string | Column items Name             |
+        | multiselect | bool   | Multiselect availble or not  |
         | msg        | string | Custom error message          |
 
         Examples:
         | Select Grid Row By Name  <XPath>  <INDEX>      |
 
         """
         module = self._container.create_or_get_module()
         element = module.get_element(identifier, InterfaceType.LISTVIEW, msg)
         module.action(Grid.Action.SELECT_ROW_BY_NAME,
-                      Grid.create_value_container(element=element, index=index, name=name),
+                      Grid.create_value_container(element=element, index=index, name=name, multiselect=multiselect),
                       msg)
 
     @keyword
     def get_grid_rows_count(self, identifier, msg=None):
         """
         Return count of rows from data grid.
```

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/keyboard.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/keyboard.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/listbox.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/listbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/mouse.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/mouse.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/property.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/property.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/radiobutton.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/radiobutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/screenshot.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/screenshot.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/tab.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/tab.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/textbox.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/textbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/togglebutton.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/togglebutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/tree.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -332,7 +332,26 @@
         | Selected TreeItem Should Be  <XPATH>  <item>                 |
         """
         module = self._container.create_or_get_module()
         element = module.get_element(identifier, InterfaceType.TREE, msg=msg)
         module.action(Tree.Action.SELECTED_ITEM_SHOULD_BE,
                       Tree.create_value_container(element=element, item=item),
                       msg)
+
+    @keyword
+    def set_tree_item_seperator(self, seperator, msg=None):
+        """
+        Sets specific tree item seperator to split.
+
+        XPaths syntax is explained in `XPath locator`.
+
+        Arguments:
+        | Argument   | Type            | Description                   |
+        | seperator  | string          | Seperator to set to split up  |
+
+        Examples:
+        | Set Tree Item Seperator  <seperator>                         |
+        """
+        module = self._container.create_or_get_module()
+        module.action(Tree.Action.SET_SEPERATOR,
+                      Tree.create_value_container(seperator=seperator),
+                      msg)
```

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/uia.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/uia.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/keywords/window.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/window.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/pythonnetwrapper.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/pythonnetwrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.2/src/FlaUILibrary/robotframework/robotlog.py` & `robotframework-flaui-3.0.3/src/FlaUILibrary/robotframework/robotlog.py`

 * *Files identical despite different names*

