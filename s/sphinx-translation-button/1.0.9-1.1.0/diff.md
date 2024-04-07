# Comparing `tmp/sphinx-translation-button-1.0.9.tar.gz` & `tmp/sphinx-translation-button-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-translation-button-1.0.9.tar", last modified: Fri Apr  5 14:56:24 2024, max compression
+gzip compressed data, was "sphinx-translation-button-1.1.0.tar", last modified: Sun Apr  7 09:27:53 2024, max compression
```

## Comparing `sphinx-translation-button-1.0.9.tar` & `sphinx-translation-button-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.542926 sphinx-translation-button-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:56:24.542926 sphinx-translation-button-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/src/sphinx-translation-button/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/src/sphinx-translation-button/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/src/sphinx-translation-button/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/src/sphinx-translation-button/static/package_translation_button.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:27:53.133250 sphinx-translation-button-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-07 09:27:48.000000 sphinx-translation-button-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-07 09:27:53.133250 sphinx-translation-button-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-07 09:27:48.000000 sphinx-translation-button-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-07 09:27:48.000000 sphinx-translation-button-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 09:27:53.133250 sphinx-translation-button-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:27:53.129250 sphinx-translation-button-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:27:53.133250 sphinx-translation-button-1.1.0/src/sphinx-translation-button/
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-07 09:27:48.000000 sphinx-translation-button-1.1.0/src/sphinx-translation-button/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:27:53.133250 sphinx-translation-button-1.1.0/src/sphinx-translation-button/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-07 09:27:48.000000 sphinx-translation-button-1.1.0/src/sphinx-translation-button/static/package_translation_button.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:27:53.133250 sphinx-translation-button-1.1.0/src/sphinx_translation_button.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-07 09:27:53.000000 sphinx-translation-button-1.1.0/src/sphinx_translation_button.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 09:27:53.000000 sphinx-translation-button-1.1.0/src/sphinx_translation_button.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:27:53.000000 sphinx-translation-button-1.1.0/src/sphinx_translation_button.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 09:27:53.000000 sphinx-translation-button-1.1.0/src/sphinx_translation_button.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 09:27:53.000000 sphinx-translation-button-1.1.0/src/sphinx_translation_button.egg-info/top_level.txt
```

### Comparing `sphinx-translation-button-1.0.9/src/sphinx-translation-button/__init__.py` & `sphinx-translation-button-1.1.0/src/sphinx-translation-button/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,16 @@
 
         # Write the modified content back to the JavaScript file
         with open(user_js_file, 'w') as js_file:
             js_file.write(new_content)
         
         # Copy all files from static to output directory
         copy_asset_file(user_js_file, static_directory)
-        copy_asset_file(package_js_file, static_directory)
 
-        print("[sphinx-translation-button] copied files to _static directory.")
+        print("[sphinx-translation-button] copied user file to _static directory.")
         
 def createVariable(file_name: str) -> str:
     # Read yaml file
     with open(file_name, 'r') as file:
         data = yaml.load(file, Loader=yaml.FullLoader)
         languages = data['languages'] if 'languages' in data else print('\033[91m' + " [sphinx-translation-button] build failed due to missing languages in _config.yml. Please add languages to _config.yml. "+ '\033[0m')
 
@@ -56,12 +55,11 @@
 
    
 
     
 
 def setup(app: Sphinx) -> dict[str, str]:
     app.add_js_file('user_translation_button.js')
-    app.add_js_file('package_translation_button.js')
 
     print("added this file", 'user_translation_button.js')
     app.connect('build-finished', copy_buttons)
     return {'parallel_read_safe': True, 'parallel_write_safe': True}
```

### Comparing `sphinx-translation-button-1.0.9/src/sphinx-translation-button/static/package_translation_button.js` & `sphinx-translation-button-1.1.0/src/sphinx-translation-button/static/package_translation_button.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,17 +18,16 @@
     if (languages[0].length == 2) languages = languages.map(([language, code]) => [language, code, ""]);
     console.log("[sphinx-translation-button] languages specified: ", languages)
 
     // properly append items to button_data
     button_data.items = languages.map(([language, code, link]) => ({
         "label": language,
         "onclick": () => {
-            console.log("[sphinx-translation-button] adding ", language, " with code ", code)
             if (link != "") {
-                window.location.href = 'link'
+                window.location.href = link
             } else {
                 let currentLanguageCode = languages.find(([language, code]) => window.location.pathname.includes(`/${code}/`))?.[1] || null;
                 currentLanguageCode != null && (window.location.pathname = window.location.pathname.replace(`/${currentLanguageCode}/`, `/${code}/`));
             }
         }
     }))
     addDropdown(button_data)
@@ -74,14 +73,15 @@
         // Check if icon is present, if not add a dot (&#x2022;)
         if (b.icon != undefined) {
             let icon = setSubIcon(b.icon)
             linkItem.appendChild(icon);
         } else {
             linkItem.innerHTML += "&#x2022;";
         }
+        console.log("[sphinx-translation-button] adding ", b.language, " with code ", b.code, " and link ", b.link)
         if (b.label != undefined) linkItem.innerHTML += " " + b.label;
 
         listItem.appendChild(linkItem);
         dropdownList.appendChild(listItem);
     })
 
     container.appendChild(buttonElement);
```

