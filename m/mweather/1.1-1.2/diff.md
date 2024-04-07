# Comparing `tmp/mweather-1.1.tar.gz` & `tmp/mweather-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mweather-1.1.tar", last modified: Thu Apr  4 20:24:11 2024, max compression
+gzip compressed data, was "mweather-1.2.tar", last modified: Sun Apr  7 19:14:30 2024, max compression
```

## Comparing `mweather-1.1.tar` & `mweather-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 20:24:11.534556 mweather-1.1/
--rw-rw-rw-   0        0        0       28 2024-04-04 20:24:09.000000 mweather-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2968 2024-04-04 20:24:11.533523 mweather-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2553 2024-04-04 20:22:32.000000 mweather-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 20:24:11.430553 mweather-1.1/mweather/
--rw-rw-rw-   0        0        0     1392 2024-04-04 20:13:26.000000 mweather-1.1/mweather/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:24:11.514558 mweather-1.1/mweather/__pycache__/
--rw-rw-rw-   0        0        0     2161 2024-04-04 20:20:43.000000 mweather-1.1/mweather/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-04 20:24:11.528537 mweather-1.1/mweather.egg-info/
--rw-rw-rw-   0        0        0     2968 2024-04-04 20:24:10.000000 mweather-1.1/mweather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-04 20:24:11.000000 mweather-1.1/mweather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 20:24:10.000000 mweather-1.1/mweather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-04 20:24:10.000000 mweather-1.1/mweather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 20:24:11.568508 mweather-1.1/setup.cfg
--rw-rw-rw-   0        0        0      686 2024-04-04 20:24:09.000000 mweather-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:14:30.036995 mweather-1.2/
+-rw-rw-rw-   0        0        0       28 2024-04-07 19:14:29.000000 mweather-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    10128 2024-04-07 19:14:30.036995 mweather-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9713 2024-04-07 19:03:08.000000 mweather-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 19:14:29.982142 mweather-1.2/mweather/
+-rw-rw-rw-   0        0        0     1843 2024-04-07 19:04:35.000000 mweather-1.2/mweather/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:14:30.032009 mweather-1.2/mweather/__pycache__/
+-rw-rw-rw-   0        0        0     2161 2024-04-04 20:20:43.000000 mweather-1.2/mweather/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 19:14:30.035999 mweather-1.2/mweather.egg-info/
+-rw-rw-rw-   0        0        0    10128 2024-04-07 19:14:29.000000 mweather-1.2/mweather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-07 19:14:29.000000 mweather-1.2/mweather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 19:14:29.000000 mweather-1.2/mweather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 19:14:29.000000 mweather-1.2/mweather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 19:14:30.038991 mweather-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      686 2024-04-07 19:14:29.000000 mweather-1.2/setup.py
```

### Comparing `mweather-1.1/mweather/__init__.py` & `mweather-1.2/mweather/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,36 +5,42 @@
 try:
 	from bs4 import BeautifulSoup
 except:
 	os.system("pip install bs4")
 	from bs4 import BeautifulSoup
 
 def weather(city, output='string', lang='en'):
-    try:
-        city = city.replace(' ', '+')
-        if lang == 'en': lang = 'weather'; reqlan = 'en-US,en;q=0.8'
-        elif lang =='ru': lang = 'погода'; reqlan = 'ru-RU,ru;q=0.9'
-        headers = {
-        'Accept-Language': reqlan
-        }
-        last_time = time.time()
-        req = requests.get(f'https://google.com/search?q={city}+{lang}', headers=headers)
-        now_time = time.time() - last_time
-        now_time = round(now_time, 2)
-        soup = BeautifulSoup(req.text, 'html.parser')
-
-        info = soup.select('.BNeawe.tAd8D.AP7Wnd')[1].getText().strip().split('\n')
-        weather = soup.select('.BNeawe.iBp4i.AP7Wnd')[1].getText().strip()
-
-        if output == 'string':
-            return f'{info[1]}, {weather}'
-        elif output == 'json':
-            return {"weather": info[1], "temp": weather, "response-time": now_time}
-        elif output == 'temp':
-            return weather
-        elif output == 'weather':
-            return info[1]
-    except IndexError as ex:
-        return f'Error: this city was not found./Этот город не найден.'
-    except Exception as ex:
-        return f'Error: {ex}'
-    
+    if output != 'calendar':
+        try:
+            city = city.replace(' ', '+')
+            if lang == 'en': lang = 'weather'; reqlan = 'en-US,en;q=0.8'
+            elif lang =='ru': lang = 'погода'; reqlan = 'ru-RU,ru;q=0.9'
+            headers = {
+            'Accept-Language': reqlan
+            }
+            last_time = time.time()
+            req = requests.get(f'https://google.com/search?q={city}+{lang}', headers=headers)
+            now_time = time.time() - last_time
+            now_time = round(now_time, 2)
+            soup = BeautifulSoup(req.text, 'html.parser')
+    
+            info = soup.select('.BNeawe.tAd8D.AP7Wnd')[1].getText().strip().split('\n')
+            weather = soup.select('.BNeawe.iBp4i.AP7Wnd')[1].getText().strip()
+    
+            if output == 'string':
+                return f'{info[1]}, {weather}'
+            elif output == 'json':
+                return {"weather": info[1], "temp": weather, "response-time": now_time}
+            elif output == 'temp':
+                return weather
+            elif output == 'weather':
+                return info[1]
+        except IndexError as ex:
+            return f'Error: this city was not found./Этот город не найден.'
+        except Exception as ex:
+            return f'Error: {ex}'
+    elif output == 'calendar':
+        city = city.replace(' ', '%20')
+        req = requests.get(f'https://wttr.in/{city}?lang={lang}')
+        retrn = req.text
+        retrn = retrn.replace('Все новые фичи публикуются здесь', '').replace('@igor_chubin', '')
+        return retrn
```

### Comparing `mweather-1.1/mweather/__pycache__/__init__.cpython-312.pyc` & `mweather-1.2/mweather/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `mweather-1.1/setup.py` & `mweather-1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 with open(r'C:\Users\say gex\Desktop\проектыц\weather\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='mweather',
-	version='1.1',
-	author='mc_c0rp',
+	version='1.2',
+	author='mc.c0rp',
 	author_email='mc.c0rp@icloud.com',
 	description='Бесплатное и быстрое api для получения погоды.',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=['mweather'],
 	include_package_data=True,
 	classifiers=[
```

