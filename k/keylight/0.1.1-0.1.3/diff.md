# Comparing `tmp/keylight-0.1.1.tar.gz` & `tmp/keylight-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keylight-0.1.1.tar", last modified: Thu Feb 29 13:31:13 2024, max compression
+gzip compressed data, was "keylight-0.1.3.tar", max compression
```

## Comparing `keylight-0.1.1.tar` & `keylight-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,9 @@
-drwxrwxr-x   0 andornaut  (1000) andornaut  (1000)        0 2024-02-29 13:31:13.139884 keylight-0.1.1/
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)     1066 2022-07-21 22:06:20.000000 keylight-0.1.1/LICENSE
--rw-r--r--   0 andornaut  (1000) andornaut  (1000)     2352 2024-02-29 13:31:13.139884 keylight-0.1.1/PKG-INFO
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)     1924 2022-07-21 22:09:47.000000 keylight-0.1.1/README.md
-drwxrwxr-x   0 andornaut  (1000) andornaut  (1000)        0 2024-02-29 13:31:13.135884 keylight-0.1.1/keylight/
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)        0 2022-07-21 22:06:20.000000 keylight-0.1.1/keylight/__init__.py
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)     1640 2024-02-29 13:28:53.000000 keylight-0.1.1/keylight/cli.py
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)      189 2022-07-21 22:06:20.000000 keylight-0.1.1/keylight/constants.py
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)     1631 2024-02-29 13:28:53.000000 keylight-0.1.1/keylight/main.py
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)      164 2024-02-29 13:28:53.000000 keylight-0.1.1/keylight/types.py
-drwxrwxr-x   0 andornaut  (1000) andornaut  (1000)        0 2024-02-29 13:31:13.139884 keylight-0.1.1/keylight.egg-info/
--rw-r--r--   0 andornaut  (1000) andornaut  (1000)     2352 2024-02-29 13:31:13.000000 keylight-0.1.1/keylight.egg-info/PKG-INFO
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)      330 2024-02-29 13:31:13.000000 keylight-0.1.1/keylight.egg-info/SOURCES.txt
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)        1 2024-02-29 13:31:13.000000 keylight-0.1.1/keylight.egg-info/dependency_links.txt
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)       48 2024-02-29 13:31:13.000000 keylight-0.1.1/keylight.egg-info/entry_points.txt
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)       16 2024-02-29 13:31:13.000000 keylight-0.1.1/keylight.egg-info/requires.txt
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)        9 2024-02-29 13:31:13.000000 keylight-0.1.1/keylight.egg-info/top_level.txt
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)      104 2022-07-21 22:06:20.000000 keylight-0.1.1/pyproject.toml
--rw-rw-r--   0 andornaut  (1000) andornaut  (1000)      594 2024-02-29 13:31:13.139884 keylight-0.1.1/setup.cfg
+-rw-r--r--   0        0        0     1066 2022-07-21 22:06:20.414850 keylight-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1646 2024-04-07 13:42:12.165677 keylight-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2022-07-21 22:06:20.414850 keylight-0.1.3/keylight/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-07 13:39:25.279515 keylight-0.1.3/keylight/cli.py
+-rw-r--r--   0        0        0      189 2024-03-23 15:04:16.283514 keylight-0.1.3/keylight/constants.py
+-rw-r--r--   0        0        0     2201 2024-04-07 12:37:28.187822 keylight-0.1.3/keylight/main.py
+-rw-r--r--   0        0        0      370 2024-04-07 13:34:41.159804 keylight-0.1.3/keylight/types.py
+-rw-r--r--   0        0        0      437 2024-04-07 13:42:01.937545 keylight-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2062 1970-01-01 00:00:00.000000 keylight-0.1.3/PKG-INFO
```

### Comparing `keylight-0.1.1/LICENSE` & `keylight-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keylight-0.1.1/README.md` & `keylight-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: keylight
+Version: 0.1.3
+Summary: A CLI to control an Elgato Key Light
+Author: andornaut
+Author-email: andornaut@users.noreply.github.com
+Requires-Python: >=3.12,<3.13
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: leglight (>=0.2.0,<0.3.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Description-Content-Type: text/markdown
+
 # Keylight
 
 A CLI to control an [Elgato Key Light](https://www.elgato.com/en/gaming/key-light) for Linux, macOS, and Windows.
 
 Leverages the [pyleglight](https://gitlab.com/obviate.io/pyleglight) library.
 
 ## Requirements
@@ -49,43 +62,36 @@
 Connected to: Elgato Light @ keylight:9123
 Turning Off
 ```
 
 #### Aliases
 
 You may find it convenient to use shell aliases:
+
 ```
 alias koff='keylight --host keylight --off'
 alias kon='keylight --host keylight --on'
 ```
 
 Example usage:
+
 ```
 # Turn on and set brightness to 20%
 $ kon -b20
 Connected to: Elgato Light BW42J1A06055 @ keylight:9123
 Brightness: 20%
 Turning On
 ```
 
 ## Developing
 
 ```bash
-# Initialize venv
-python3 -m venv .venv
-source .venv/bin/activate
-
-# Build
-pip3 install --upgrade build
-python3 -m build
-pip3 install --upgrade dist/*.whl
-
-# If the version hasn't changed, then specify --force-reinstall
-pip3 install --upgrade --force-reinstall dist/*.whl
-
-# Run
-python3 -m keylight.main --on
-
-# Publish
-pip3 install twine
-python3 -m twine upload dist/*
+poetry shell
+
+poetry build
+
+poetry run keylight --on
+
+poetry version patch
+poetry publish
 ```
+
```

### Comparing `keylight-0.1.1/keylight/main.py` & `keylight-0.1.3/keylight/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 import sys
-
 import textwrap
-# https://gitlab.com/obviate.io/pyleglight/
-import leglight
-
-from keylight import cli, types
 
 # Ignore warning:
-# /opt/homebrew/lib/python3.9/site-packages/zeroconf/_services/browser.py:169: 
+# /opt/homebrew/lib/python3.9/site-packages/zeroconf/_services/browser.py:169:
 # FutureWarning: <leglight.discovery.discover.<locals>.thelistener object at 0x101e15a00>
 # has no update_service method. Provide one (it can be empty if you don't care about the updates),
 # it'll become mandatory.
 # https://stackoverflow.com/a/14463362
 import warnings
-warnings.filterwarnings('ignore')
+
+import leglight
+
+# https://gitlab.com/obviate.io/pyleglight/
+from keylight import cli, types
+
+warnings.filterwarnings("ignore")
+
 
 def _connect(host, port):
     return leglight.LegLight(host, port)
 
 
 def _discover():
     lights = leglight.discover(1)
     if not lights:
-        print('Could not find a Key Light', file=sys.stderr)
+        print("Could not find a Key Light", file=sys.stderr)
         exit(1)
     if len(lights) > 1:
-        print(f'Found {len(lights)} Key Lights. Using the first.')
+        print(f"Found {len(lights)} Key Lights. Using the first.")
     return lights[0]
 
 
 def _main(flags: types.Flags):
     light = _connect(flags.host, flags.port) if flags.host else _discover()
     print(f'Connected to "{light.productName}" at {light.address}:{light.port}')
 
-    if flags.brightness is not None:
-        light.brightness(flags.brightness)
-    if flags.color is not None:
-        light.color(flags.color)
+    if flags.brightness_number is not None:
+        if flags.brightness_direction is types.Direction.INCREMENT:
+            light.incBrightness(flags.brightness_number)
+        elif flags.brightness_direction is types.Direction.DECREMENT:
+            light.decBrightness(flags.brightness_number)
+        else:
+            light.brightness(flags.brightness_number)
+    if flags.color_number is not None:
+        if flags.color_direction is types.Direction.INCREMENT:
+            light.incColor(flags.color_number)
+        elif flags.color_direction is types.Direction.DECREMENT:
+            light.decColor(flags.color_number)
+        else:
+            light.color(flags.color_number)
     if flags.on:
         light.on()
     if flags.off:
         light.off()
     if flags.toggle:
         if light.isOn:
             light.off()
         else:
             light.on()
-    print(textwrap.dedent(f'''\
+    print(
+        textwrap.dedent(
+            f"""\
         Brightness: {light.isBrightness}%
         Color temperature: {light.isTemperature:.0f}k
-        On/Off: {"On" if light.isOn else "Off"}'''
-    ))
+        On/Off: {"On" if light.isOn else "Off"}"""
+        )
+    )
 
 
 def main():
     _main(cli.parse())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

