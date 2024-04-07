# Comparing `tmp/GraphSpy-1.1.2.tar.gz` & `tmp/GraphSpy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSpy-1.1.2.tar", last modified: Sun Mar 17 21:00:44 2024, max compression
+gzip compressed data, was "GraphSpy-1.1.3.tar", last modified: Sun Apr  7 13:03:08 2024, max compression
```

## Comparing `GraphSpy-1.1.2.tar` & `GraphSpy-1.1.3.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-03-17 21:00:44.167870 GraphSpy-1.1.2/
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-03-17 21:00:44.167870 GraphSpy-1.1.2/GraphSpy/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    39739 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/GraphSpy.py
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)        0 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/__init__.py
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-03-17 21:00:44.167870 GraphSpy-1.1.2/GraphSpy/static/
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-03-17 21:00:44.167870 GraphSpy-1.1.2/GraphSpy/static/css/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      340 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/static/css/style.css
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-03-17 21:00:44.167870 GraphSpy-1.1.2/GraphSpy/static/js/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    10585 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/static/js/functions.js
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     2430 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/static/js/theme.js
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-03-17 21:00:44.167870 GraphSpy-1.1.2/GraphSpy/templates/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7456 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/OneDrive.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     8263 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/SharePoint.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5466 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/SharePointDrives.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6088 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/SharePointSites.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     9595 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/access_tokens.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17064 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/custom_requests.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5969 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/device_codes.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7642 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/generic_search.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      847 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/index.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17495 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/layout.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1695 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/outlook.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     4803 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/recent_files.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6820 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/refresh_tokens.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7018 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/settings.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     4817 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/templates/shared_with_me.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)        5 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/GraphSpy/version.txt
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-03-17 21:00:44.167870 GraphSpy-1.1.2/GraphSpy.egg-info/
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     6464 2024-03-17 21:00:44.000000 GraphSpy-1.1.2/GraphSpy.egg-info/PKG-INFO
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)      950 2024-03-17 21:00:44.000000 GraphSpy-1.1.2/GraphSpy.egg-info/SOURCES.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)        1 2024-03-17 21:00:44.000000 GraphSpy-1.1.2/GraphSpy.egg-info/dependency_links.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       52 2024-03-17 21:00:44.000000 GraphSpy-1.1.2/GraphSpy.egg-info/entry_points.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       28 2024-03-17 21:00:44.000000 GraphSpy-1.1.2/GraphSpy.egg-info/requires.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)        9 2024-03-17 21:00:44.000000 GraphSpy-1.1.2/GraphSpy.egg-info/top_level.txt
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1527 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/LICENSE.txt
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)       54 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/MANIFEST.in
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     6464 2024-03-17 21:00:44.167870 GraphSpy-1.1.2/PKG-INFO
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6341 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/README.md
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)       28 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/requirements.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       38 2024-03-17 21:00:44.171871 GraphSpy-1.1.2/setup.cfg
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      916 2024-03-17 21:00:40.000000 GraphSpy-1.1.2/setup.py
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    41189 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/GraphSpy.py
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/__init__.py
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/static/
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/static/css/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      340 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/static/css/style.css
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/static/js/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    11164 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/static/js/functions.js
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     2430 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/static/js/theme.js
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/templates/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7747 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/OneDrive.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     8554 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/SharePoint.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5757 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/SharePointDrives.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6379 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/SharePointSites.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5966 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/access_token_modal.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     9657 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/access_tokens.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17378 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/custom_requests.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5969 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/device_codes.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7933 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/generic_search.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      847 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/index.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17710 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/layout.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1923 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/outlook.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5094 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/recent_files.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5679 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/refresh_token_modal.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6820 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/refresh_tokens.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7886 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/settings.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5108 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/shared_with_me.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)        5 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/version.txt
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy.egg-info/
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     6914 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/PKG-INFO
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     1037 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/SOURCES.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)        1 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/dependency_links.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       52 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/entry_points.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       28 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/requires.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)        9 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/top_level.txt
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1527 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/LICENSE.txt
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)       54 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/MANIFEST.in
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     6914 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/PKG-INFO
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6800 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/README.md
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)       28 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/requirements.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       38 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/setup.cfg
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      916 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/setup.py
```

### Comparing `GraphSpy-1.1.2/GraphSpy/GraphSpy.py` & `GraphSpy-1.1.3/GraphSpy/GraphSpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def init_db():
     con = sqlite3.connect(app.config['graph_spy_db_path'])
     con.execute('CREATE TABLE accesstokens (id INTEGER PRIMARY KEY AUTOINCREMENT, stored_at TEXT, issued_at TEXT, expires_at TEXT, description TEXT, user TEXT, resource TEXT, accesstoken TEXT)')
     con.execute('CREATE TABLE refreshtokens (id INTEGER PRIMARY KEY AUTOINCREMENT, stored_at TEXT, description TEXT, user TEXT, tenant_id TEXT, resource TEXT, foci INTEGER, refreshtoken TEXT)')
     con.execute('CREATE TABLE devicecodes (id INTEGER PRIMARY KEY AUTOINCREMENT, generated_at INTEGER, expires_at INTEGER, user_code TEXT, device_code TEXT, interval INTEGER, client_id TEXT, status TEXT, last_poll INTEGER)')
     con.execute('CREATE TABLE request_templates (id INTEGER PRIMARY KEY AUTOINCREMENT, template_name TEXT, uri TEXT, method TEXT, request_type TEXT, body TEXT, headers TEXT, variables TEXT)')
     con.execute('CREATE TABLE settings (setting TEXT UNIQUE, value TEXT)')
-    # Valid Settings: active_access_token_id, active_refresh_token_id, schema_version
+    # Valid Settings: active_access_token_id, active_refresh_token_id, schema_version, user_agent
     cur = con.cursor()
     cur.execute("INSERT INTO settings (setting, value) VALUES ('schema_version', '2')")
     con.commit()
     con.close()
 
 def get_db():
     db = getattr(g, '_database', None)
@@ -79,31 +79,46 @@
         print("[*] Current database is schema version 1, updating to schema version 2")
         execute_db("CREATE TABLE request_templates (id INTEGER PRIMARY KEY AUTOINCREMENT, template_name TEXT, uri TEXT, method TEXT, request_type TEXT, body TEXT, headers TEXT, variables TEXT)")
         execute_db("UPDATE settings SET value = '2' WHERE setting = 'schema_version'")
         print("[*] Updated database to schema version 2")
 
 # ========== Helper Functions ==========
 
+def get_user_agent():
+    user_agent = query_db("SELECT value FROM settings where setting = 'user_agent'",one=True)
+    if user_agent:
+        return user_agent[0]
+    else:
+        return "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
+
+def set_user_agent(user_agent):
+    execute_db("INSERT OR REPLACE INTO settings (setting, value) VALUES ('user_agent',?)",(user_agent,))
+    if get_user_agent() == user_agent:
+        return True
+    else:
+        return False
+
 def graph_request(graph_uri, access_token_id):
     access_token = query_db("SELECT accesstoken FROM accesstokens where id = ?",[access_token_id],one=True)[0]
-    headers =  {"Authorization":f"Bearer {access_token}"}
+    headers = {"Authorization":f"Bearer {access_token}", "User-Agent":get_user_agent()}
     response = requests.get(graph_uri, headers=headers)
     resp_json = response.json()
     return json.dumps(resp_json)
 
 def graph_request_post(graph_uri, access_token_id, body):
     access_token = query_db("SELECT accesstoken FROM accesstokens where id = ?",[access_token_id],one=True)[0]
-    headers = {"Authorization":f"Bearer {access_token}"}
+    headers = {"Authorization":f"Bearer {access_token}", "User-Agent":get_user_agent()}
     response = requests.post(graph_uri, headers=headers, json=body)
     resp_json = response.json()
     return json.dumps(resp_json)
     
 def generic_request(uri, access_token_id, method, request_type, body, headers):
     access_token = query_db("SELECT accesstoken FROM accesstokens where id = ?",[access_token_id],one=True)[0]
     headers["Authorization"] = f"Bearer {access_token}"
+    headers["User-Agent"] = get_user_agent()
 
     # Empty body
     if not body:
         response = requests.request(method, uri, headers=headers)
     # Text, XML or urlencoded request
     elif request_type in ["text", "urlencoded", "xml"]:
         if request_type == "urlencoded" and not "Content-Type" in headers:
@@ -175,15 +190,16 @@
     try:
         uuid.UUID(str(val))
         return True
     except ValueError:
         return False
 
 def get_tenant_id(tenant_domain):
-    response = requests.get(f"https://login.microsoftonline.com/{tenant_domain}/.well-known/openid-configuration")
+    headers = {"User-Agent":get_user_agent()}
+    response = requests.get(f"https://login.microsoftonline.com/{tenant_domain}/.well-known/openid-configuration", headers=headers)
     resp_json = response.json()
     tenant_id = resp_json["authorization_endpoint"].split("/")[3]
     return tenant_id
 
 def refresh_to_access_token(refresh_token_id, resource = "defined_in_token", client_id = "d3590ed6-52b3-4102-aeff-aad2292ab01c", store_refresh_token = True):
     refresh_token = query_db("SELECT refreshtoken FROM refreshtokens where id = ?",[refresh_token_id],one=True)[0]
     tenant_id = query_db("SELECT tenant_id FROM refreshtokens where id = ?",[refresh_token_id],one=True)[0]
@@ -192,15 +208,16 @@
         "resource": resource,
         "client_id": client_id,
         "grant_type": "refresh_token",
         "refresh_token": refresh_token,
         "scope": "openid"
     }
     url = f"https://login.microsoftonline.com/{tenant_id}/oauth2/token?api-version=1.0"
-    response = requests.post(url, data=body)
+    headers = {"User-Agent":get_user_agent()}
+    response = requests.post(url, data=body, headers=headers)
     access_token = response.json()["access_token"]
     save_access_token(access_token, f"Created using refresh token {refresh_token_id}")
     access_token_id = query_db("SELECT id FROM accesstokens where accesstoken = ?",[access_token],one=True)[0]
     if store_refresh_token:
         decoded_accesstoken = jwt.decode(access_token, options={"verify_signature": False})
         user = "unknown"
         # If the idtype is user, use the unique_name or upn
@@ -221,15 +238,16 @@
 
 def generate_device_code(resource = "https://graph.microsoft.com", client_id = "d3590ed6-52b3-4102-aeff-aad2292ab01c"):
     body =  {
         "resource": resource,
         "client_id": client_id
     }
     url = "https://login.microsoftonline.com/common/oauth2/devicecode?api-version=1.0"
-    response = requests.post(url, data=body)
+    headers = {"User-Agent":get_user_agent()}
+    response = requests.post(url, data=body,headers=headers)
 
     execute_db("INSERT INTO devicecodes (generated_at, expires_at, user_code, device_code, interval, client_id, status, last_poll) VALUES (?,?,?,?,?,?,?,?)",(
             int(datetime.now().timestamp()),
             int(datetime.now().timestamp()) + int(response.json()["expires_in"]),
             response.json()["user_code"],
             response.json()["device_code"],
             int(response.json()["interval"]),
@@ -260,15 +278,16 @@
                     execute_db("UPDATE devicecodes SET status = ? WHERE device_code = ?",("POLLING",row["device_code"]))
                 body = {
                     "client_id": row["client_id"],
                     "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
                     "code": row["device_code"]
                 }
                 url = "https://login.microsoftonline.com/Common/oauth2/token?api-version=1.0"
-                response = requests.post(url, data=body)
+                headers = {"User-Agent":get_user_agent()}
+                response = requests.post(url, data=body, headers=headers)
                 execute_db("UPDATE devicecodes SET last_poll = ? WHERE device_code = ?",(int(datetime.now().timestamp()),row["device_code"]))
                 if response.status_code == 200 and "access_token" in response.json():
                     access_token = response.json()["access_token"]
                     user_code = row["user_code"]
                     save_access_token(access_token, f"Created using device code auth ({user_code})")
                     decoded_accesstoken = jwt.decode(access_token, options={"verify_signature": False})
                     user = "unknown"
@@ -707,14 +726,27 @@
     
     @app.get("/api/get_settings")
     def api_get_settings():
         settings_raw = query_db_json("SELECT * FROM settings")
         #settings_json = [{setting["setting"] : setting["value"]} for setting in settings_raw]
         settings_json = {setting["setting"] : setting["value"] for setting in settings_raw}
         return settings_json
+        
+    @app.get("/api/get_user_agent")
+    def api_get_user_agent():
+        return get_user_agent()
+
+    @app.post("/api/set_user_agent")
+    def api_set_user_agent():
+        user_agent = request.form['user_agent'] if "user_agent" in request.form else ""
+        if not user_agent:
+            return "[Error] User agent not specified!", 400 
+        if not set_user_agent(user_agent):
+            return f"[Error] Unable to set user agent to '{user_agent}'!", 400 
+        return f"[Success] User agent set to '{user_agent}'!" 
 
     # ========== Other ==========
 
     @app.teardown_appcontext
     def close_connection(exception):
         db = getattr(g, '_database', None)
         if db is not None:
```

### Comparing `GraphSpy-1.1.2/GraphSpy/static/js/functions.js` & `GraphSpy-1.1.3/GraphSpy/static/js/functions.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -215,14 +215,40 @@
         }
     });
     bootstrapToast("DataTable Error Messages", response.responseText)
     $('#dt-error-message-button-disabled').toggleClass("active")
     $('#dt-error-message-button-enabled').toggleClass("active")
 }
 
+// ========== User Agent ==========
+
+function getUserAgent() {
+    let response = $.ajax({
+        type: "GET",
+        async: false,
+        url: "/api/get_user_agent"
+    });
+    if (response.status == 200) {
+        return response.responseText
+    }
+    return "Unable to obtain user agent."
+}
+
+function setUserAgent(userAgent) {
+    let response = $.ajax({
+        type: "POST",
+        async: false,
+        url: "/api/set_user_agent",
+        data: {
+            "user_agent": userAgent
+        }
+    });
+    bootstrapToast("Set User Agent", response.responseText)
+}
+
 // ========== Cookies ==========
 
 function getCookie(name) {
     const value = `; ${document.cookie}`;
     const parts = value.split(`; ${name}=`);
     if (parts.length === 2) return parts.pop().split(';').shift();
 };
```

### Comparing `GraphSpy-1.1.2/GraphSpy/static/js/theme.js` & `GraphSpy-1.1.3/GraphSpy/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/OneDrive.html` & `GraphSpy-1.1.3/GraphSpy/templates/OneDrive.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,18 @@
     <form id="onedrive_form" class="row g-3">
         <div>
             <label for="path" class="form-label">Path:</label>
             <input type="text" id="path" name="path" value="/" class="form-control">
         </div>
         <div class="col-3">
             <label for="access_token_id" class="form-label">Access token id *</label>
-            <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+            <div class="input-group">
+                <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
+            </div>
         </div>
         <div>
             <button type="Button" class="btn btn-primary" onclick="generateTable()">Browse</button>
         </div>
     </form>
     <br>
     <button onclick="openParentFolder()" class="btn btn-primary">Parent Folder</button>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'layout.html'%} {%block content%}
 ************ OOnneeDDrriivvee FFiilleess ************
 Path:[/                   ]
-Access token id *[access_token_id     ]
+Access token id *
+[access_token_id     ]Select...
 Browse
 
 Parent Folder
 
 ********** FFiilleess **********
   CCrreeaatteedd LLaasstt MMooddiiffiieedd FFiillee NNaammee FFiillee SSiizzee UURRLL
 {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/SharePoint.html` & `GraphSpy-1.1.3/GraphSpy/templates/SharePoint.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,18 @@
     <form id="sharepoint_form" class="row g-3">
         <div class="col-md-9">
             <label for="drive_id" class="form-label">Drive ID *</label>
             <input type="text" id="drive_id" name="drive_id" class="form-control" required>
         </div>
         <div class="col-md-3">
             <label for="access_token_id" class="form-label">Access token id *</label>
-            <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+            <div class="input-group">
+                <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
+            </div>
         </div>
         <div>
             <label for="path" class="form-label">Path *</label>
             <input type="text" id="path" name="path" value="/" class="form-control" required>
         </div>
         <div>
             <button type="Button" class="btn btn-primary" onclick="generateTable()">Browse</button>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'layout.html'%} {%block content%}
 ************ SShhaarreePPooiinntt FFiilleess ************
 Drive ID *[drive_id            ]
-Access token id *[access_token_id     ]
+Access token id *
+[access_token_id     ]Select...
 Path *[/                   ]
 Browse
 
 Parent Folder
 
 ********** FFiilleess TTaabbllee **********
   CCrreeaatteedd LLaasstt MMooddiiffiieedd FFiillee NNaammee FFiillee SSiizzee UURRLL
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/SharePointDrives.html` & `GraphSpy-1.1.3/GraphSpy/templates/SharePointDrives.html`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,18 @@
     <form id="sharepoint_form" class="row g-3">
         <div>
             <label for="site_id" class="form-label">Site ID *</label>
             <input type="text" id="site_id" name="site_id" class="form-control" required>
         </div>
         <div class="col-3">
             <label for="access_token_id" class="form-label">Access token id *</label>
-            <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+            <div class="input-group">
+                <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
+            </div>
         </div>
         <div>
             <button type="Button" class="btn btn-primary" onclick="generateTable()">Browse</button>
         </div>
     </form>
     <script>
         getActiveAccessToken(document.getElementById("sharepoint_form").access_token_id)
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'layout.html'%} {%block content%}
 ************ SShhaarreePPooiinntt DDrriivveess ************
 Site ID *[site_id             ]
-Access token id *[access_token_id     ]
+Access token id *
+[access_token_id     ]Select...
 Browse
 
 ********** DDrriivveess TTaabbllee **********
   CCrreeaatteedd LLaasstt MMooddiiffiieedd DDrriivvee NNaammee UURRLL
 {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/SharePointSites.html` & `GraphSpy-1.1.3/GraphSpy/templates/SharePointSites.html`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,18 @@
         <div class="col-sm-4">
             <label for="search_limit" class="form-label">Limit *</label>
             <input type="text" id="search_limit" name="search_limit" class="form-control" value="100" required>
             <i class="form-text">Max 1000</i>
         </div>
         <div class="col-sm-4">
             <label for="access_token_id" class="form-label">Access token id *</label>
-            <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+            <div class="input-group">
+                <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
+            </div>
         </div>
         <div>
             <button type="Button" class="btn btn-primary" onclick="generateTable()">Browse</button>
         </div>
     </form>
     <script>
         getActiveAccessToken(document.getElementById("sharepoint_form").access_token_id)
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'layout.html'%} {%block content%}
 ************ SShhaarreePPooiinntt SSiitteess ************
 Site Filter *[*                   ]
 Limit * [100                 ]Max 1000
-Access token id *[access_token_id     ]
+Access token id *
+[access_token_id     ]Select...
 Browse
 
 ********** SSiitteess TTaabbllee **********
   CCrreeaatteedd LLaasstt MMooddiiffiieedd SSiittee NNaammee DDiissppllaayy NNaammee UURRLL
 {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/access_tokens.html` & `GraphSpy-1.1.3/GraphSpy/templates/access_tokens.html`

 * *Files 4% similar despite different names*

```diff
@@ -196,24 +196,22 @@
     function format(d) {
         // `d` is the original data object for the row
         let response = $.ajax({
             type: "GET",
             async: false,
             url: "/api/decode_token/" + d.id
         });
-        return (
-            //'<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
+        var formatWrapper = $(
             '<dl>' +
             '<dt>Raw Token:</dt>' +
-            '<dd><code>' +
-            d.accesstoken +
-            '</code></dd>' +
-            '<dt>Decoded Token:</dt>' +
-            '<dd><pre>' +
-            JSON.stringify(JSON.parse(response.responseText), undefined, 4) +
-            '</pre></dd>' +
             '</dl>'
         );
+        var formatCode = $('<code></code>').text(d.accesstoken);
+        formatWrapper.append($('<dd></dd>').append(formatCode));
+        formatWrapper.append($('<dt>Decoded Token:</dt>'));
+        var formatPre = $('<pre></pre>').text(JSON.stringify(JSON.parse(response.responseText), undefined, 4));
+        formatWrapper.append($('<dd></dd>').append(formatPre));
+        return formatWrapper;
     }
 </script>
 
 {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/custom_requests.html` & `GraphSpy-1.1.3/GraphSpy/templates/custom_requests.html`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 
 <br>
 <div class="col-md-11">
     <h1>Custom Requests</h1>
     <form id="custom_request_form" class="row g-3">
         <div class="col-2">
             <label for="method" class="form-label">Method *</label>
-            <input list="methods" id="method" placeholder="GET" class="form-control" required>
-            <datalist id="methods">
+            <select id="method" placeholder="GET" class="form-select" required>
                 <option value="GET">GET</option>
                 <option value="POST">POST</option>
                 <option value="PUT">PUT</option>
                 <option value="PATCH">PATCH</option>
                 <option value="HEAD">HEAD</option>
                 <option value="DELETE">DELETE</option>
                 <option value="OPTIONS">OPTIONS</option>
-            </datalist>
+            </select>
         </div>
         <div class="col-2">
             <label for="request_type" class="form-label">Body type</label>
-            <select id="request_type" class="form-select" aria-label="Request body">
+            <select id="request_type" class="form-select">
                 <option value="text">Text</option>
                 <option value="urlencoded">URL Encoded</option>
                 <option value="json">JSON</option>
                 <option value="xml">XML</option>
             </select>
         </div>
         <div class="col-2">
             <label for="access_token_id" class="form-label">Access token id *</label>
-            <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+            <div class="input-group">
+                <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
+            </div>
         </div>
         <div class="col-3"></div>
         <div class="col-3">
             <label for="request_template_name" class="form-label">Request Template</label>
             <div class="input-group">
                 <input type="text" id="request_template_name" placeholder="Template Name" class="form-control">
                 <button class="btn btn-outline-primary" type="button" onclick="saveRequestTemplate()">Save</button>
@@ -91,155 +93,14 @@
             </div>
             <div class="card-body">
                 <pre id="response_body" class="mb-0"></pre>
             </div>
         </div>
     </div>
 </div>
-<!-- Modal -->
-<div class="modal fade" id="request_template_modal" tabindex="-1" aria-labelledby="request_template_modal_label" aria-hidden="true">
-    <div class="modal-dialog modal-xl">
-        <div class="modal-content">
-            <div class="modal-header">
-                <h1 class="modal-title fs-5" id="request_template_modal_label">Request Templates</h1>
-                <div style="float: right">
-                    <i class="fi fi-br-expand px-3" id="expand-icon" style="cursor: pointer; float: left; opacity: 0.5"></i>
-                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
-                </div>
-            </div>
-            <div class="modal-body">
-                <div id="dTable" class="box-body table-responsive" style="padding:20px;">
-                    <table id="request_templates" class="display" style="width:100%">
-                        <thead>
-                            <tr>
-                                <th></th>
-                                <th></th>
-                                <th></th>
-                                <th>ID</th>
-                                <th>Name</th>
-                                <th>Body type</th>
-                                <th>Method</th>
-                                <th>URI</th>
-                            </tr>
-                        </thead>
-                    </table>
-                </div>
-            </div>
-            <div class="modal-footer">
-                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
-            </div>
-        </div>
-    </div>
-</div>
-<script type="text/javascript" class="init">
-    // Populate the request_templates table
-    let myTable = new DataTable('#request_templates', {
-        ajax: {
-            url: '/api/list_request_templates', dataSrc: ""
-        },
-        columns: [
-            {
-                className: 'dt-control',
-                orderable: false,
-                data: null,
-                defaultContent: '',
-                'width': '20px'
-            },
-            {
-                className: 'active-control',
-                orderable: false,
-                data: null,
-                defaultContent: '<i class="fi fi-br-check" style="cursor: pointer"></i>',
-                'width': '20px'
-            },
-            {
-                className: 'delete-control',
-                orderable: false,
-                data: null,
-                defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
-                'width': '20px'
-            },
-            { data: 'id', 'width': '30px' },
-            { data: 'template_name', 'width': '150px' },
-            { data: 'request_type', 'width': '150px' },
-            { data: 'method', 'width': '100px' },
-            { data: 'uri'}
-        ],
-        order: [[3, 'desc']]
-    })
-
-    myTable.on('click', 'td.dt-control', function (e) {
-        let tr = e.target.closest('tr');
-        let row = myTable.row(tr);
-
-        if (row.child.isShown()) {
-            // This row is already open - close it
-            row.child.hide();
-        }
-        else {
-            // Open this row
-            row.child(format(row.data())).show();
-        }
-    });
-
-    myTable.on('click', 'td.active-control', function (e) {
-        let tr = e.target.closest('tr');
-        let row = myTable.row(tr);
-        request_template_info = row.data();
-        $("#request_uri").val(request_template_info.uri);
-        $("#method").val(request_template_info.method);
-        $("#request_type").val(request_template_info.request_type);
-        $("#body").val(request_template_info.body);
-        $("#request_template_name").val(request_template_info.template_name);
-        $('#header_fields').empty();
-        $('#variable_fields').empty();
-        for (var header_name in request_template_info.headers) {
-            if (request_template_info.headers.hasOwnProperty(header_name)) {
-                addHeaderRow(header_name, request_template_info.headers[header_name]);
-            }
-        }
-        for (var variable_name in request_template_info.variables) {
-            if (request_template_info.variables.hasOwnProperty(variable_name)) {
-                addVariableRow(variable_name, request_template_info.variables[variable_name]);
-            }
-        }
-        $('#request_template_modal').modal('hide');
-    });
-
-    myTable.on('click', 'td.delete-control', function (e) {
-        let tr = e.target.closest('tr');
-        let row = myTable.row(tr);
-        if (!confirm("Are you sure you want to delete request template '" + row.data().template_name + "'?")) { return }
-        deleteRequestTemplate(row.data().id);
-    });
-
-    function format(d) {
-        var descList = $(
-            '<dl>' +
-            '<dt>Request Template:</dt>' +
-            '</dl>');
-        var descDetails = $('<dd></dd>');
-        var preText = $('<pre></pre>');
-        preText.text(JSON.stringify(d, undefined, 4));
-        descDetails.append(preText);
-        descList.append(descDetails);
-        return descList
-    }
-
-    function deleteRequestTemplate(id) {
-        let response = $.ajax({
-            type: "POST",
-            async: false,
-            url: "/api/delete_request_template",
-            data: {"template_id": id}
-        });
-        $('#request_templates').DataTable().ajax.reload(null, false);
-        bootstrapToast("Delete Request Template", response.responseText)
-    }
-</script>
 <script>
     function getHeaders() {
         let headers = {};
         for (const header of $("#header_fields").children()) {
             if (header.getElementsByClassName("header_name")[0].value != "") {
                 headers[header.getElementsByClassName("header_name")[0].value] = header.getElementsByClassName("header_value")[0].value;
             };
@@ -285,15 +146,15 @@
             if (responseJSON.response_type == "json") {
                 $("#response_body").text(JSON.stringify(JSON.parse(responseJSON.response_text), undefined, 4));
             } else if (responseJSON.response_type == "xml") {
                 $("#response_body").text(prettifyXml(responseJSON.response_text));
             } else {
                 $("#response_body").text(responseJSON.response_text);
             }
-        }catch (e) {
+        } catch (e) {
             $("#response_body").text(responseJSON.response_text);
         }
         $("#response_status_code").text(responseJSON.response_status_code);
         $("#response-card").show();
     }
 
     function saveRequestTemplate() {
@@ -370,15 +231,158 @@
         variableWrapper.append(variableButton);
         $("#variable_fields").append(variableWrapper);
     }
 
     $("#response-card").on('click', 'i#copy-icon', function (e) {
         copyToClipboard($("#response_body").text());
     })
+</script>
 
-    $("#request_template_modal").on('click', 'i#expand-icon', function (e) {
-        $("#request_template_modal").find('.modal-dialog').toggleClass('modal-xl').toggleClass('modal-fullscreen')
-        $("i#expand-icon").toggleClass('fi-br-expand').toggleClass('fi-br-compress')
+<!-- Request Template Modal -->
+<div class="modal fade" id="request_template_modal" tabindex="-1" aria-labelledby="request_template_modal_label" aria-hidden="true">
+    <div class="modal-dialog modal-xl">
+        <div class="modal-content">
+            <div class="modal-header">
+                <h1 class="modal-title fs-5" id="request_template_modal_label">Request Templates</h1>
+                <div style="float: right">
+                    <i class="fi fi-br-expand px-3" id="expand-icon" style="cursor: pointer; float: left; opacity: 0.5"></i>
+                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
+                </div>
+            </div>
+            <div class="modal-body">
+                <div id="dTable" class="box-body table-responsive" style="padding:20px;">
+                    <table id="request_templates" class="display" style="width:100%">
+                        <thead>
+                            <tr>
+                                <th></th>
+                                <th></th>
+                                <th></th>
+                                <th>ID</th>
+                                <th>Name</th>
+                                <th>Body type</th>
+                                <th>Method</th>
+                                <th>URI</th>
+                            </tr>
+                        </thead>
+                    </table>
+                </div>
+            </div>
+            <div class="modal-footer">
+                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
+            </div>
+        </div>
+    </div>
+</div>
+<script type="text/javascript" class="init">
+    // Populate the request_templates table
+    let myTable = new DataTable('#request_templates', {
+        ajax: {
+            url: '/api/list_request_templates', dataSrc: ""
+        },
+        columns: [
+            {
+                className: 'dt-control',
+                orderable: false,
+                data: null,
+                defaultContent: '',
+                'width': '20px'
+            },
+            {
+                className: 'active-control',
+                orderable: false,
+                data: null,
+                defaultContent: '<i class="fi fi-br-check" style="cursor: pointer"></i>',
+                'width': '20px'
+            },
+            {
+                className: 'delete-control',
+                orderable: false,
+                data: null,
+                defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
+                'width': '20px'
+            },
+            { data: 'id', 'width': '30px' },
+            { data: 'template_name', 'width': '150px' },
+            { data: 'request_type', 'width': '130px' },
+            { data: 'method', 'width': '80px' },
+            { data: 'uri' }
+        ],
+        order: [[3, 'desc']],
+        autoWidth: false
     })
 
+    myTable.on('click', 'td.dt-control', function (e) {
+        let tr = e.target.closest('tr');
+        let row = myTable.row(tr);
+
+        if (row.child.isShown()) {
+            // This row is already open - close it
+            row.child.hide();
+        }
+        else {
+            // Open this row
+            row.child(formatRequestTemplate(row.data())).show();
+        }
+    });
+
+    myTable.on('click', 'td.active-control', function (e) {
+        let tr = e.target.closest('tr');
+        let row = myTable.row(tr);
+        request_template_info = row.data();
+        $("#request_uri").val(request_template_info.uri);
+        $("#method").val(request_template_info.method);
+        $("#request_type").val(request_template_info.request_type);
+        $("#body").val(request_template_info.body);
+        $("#request_template_name").val(request_template_info.template_name);
+        $('#header_fields').empty();
+        $('#variable_fields').empty();
+        for (var header_name in request_template_info.headers) {
+            if (request_template_info.headers.hasOwnProperty(header_name)) {
+                addHeaderRow(header_name, request_template_info.headers[header_name]);
+            }
+        }
+        for (var variable_name in request_template_info.variables) {
+            if (request_template_info.variables.hasOwnProperty(variable_name)) {
+                addVariableRow(variable_name, request_template_info.variables[variable_name]);
+            }
+        }
+        $('#request_template_modal').modal('hide');
+    });
+
+    myTable.on('click', 'td.delete-control', function (e) {
+        let tr = e.target.closest('tr');
+        let row = myTable.row(tr);
+        if (!confirm("Are you sure you want to delete request template '" + row.data().template_name + "'?")) { return }
+        deleteRequestTemplate(row.data().id);
+    });
+
+    function formatRequestTemplate(d) {
+        var descList = $(
+            '<dl>' +
+            '<dt>Request Template:</dt>' +
+            '</dl>');
+        var descDetails = $('<dd></dd>');
+        var preText = $('<pre></pre>');
+        preText.text(JSON.stringify(d, undefined, 4));
+        descDetails.append(preText);
+        descList.append(descDetails);
+        return descList
+    }
+
+    function deleteRequestTemplate(id) {
+        let response = $.ajax({
+            type: "POST",
+            async: false,
+            url: "/api/delete_request_template",
+            data: { "template_id": id }
+        });
+        $('#request_templates').DataTable().ajax.reload(null, false);
+        bootstrapToast("Delete Request Template", response.responseText)
+    }
+
+    $("#request_template_modal").on('click', 'i#expand-icon', function (e) {
+        $("#request_template_modal .modal-dialog").toggleClass('modal-xl').toggleClass('modal-fullscreen')
+        $("#request_template_modal i#expand-icon").toggleClass('fi-br-expand').toggleClass('fi-br-compress')
+    })
 </script>
+
     {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/device_codes.html` & `GraphSpy-1.1.3/GraphSpy/templates/device_codes.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/generic_search.html` & `GraphSpy-1.1.3/GraphSpy/templates/generic_search.html`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,18 @@
         <div class="col-sm-4">
             <label for="search_limit" class="form-label">Limit *</label>
             <input type="text" id="search_limit" name="search_limit" class="form-control" value="25" required>
             <i class="form-text">Max 1000</i>
         </div>
         <div class="col-sm-4">
             <label for="access_token_id" class="form-label">Access token id *</label>
-            <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+            <div class="input-group">
+                <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
+            </div>
         </div>
         <div>
             <label for="search_query" class="form-label">Search Query *</label>
             <input type="text" id="search_query" name="search_query" class="form-control" value="*" required>
         </div>
         <div>
             <button type="Button" class="btn btn-primary" onclick="generateTable()">Request</button>
```

#### html2text {}

```diff
@@ -6,14 +6,15 @@
 Email message
 Teams messages
 Calendar events
 Sharepoint Sites
 Lists
 List Items
 Limit * [25                  ]Max 1000
-Access token id *[access_token_id     ]
+Access token id *
+[access_token_id     ]Select...
 Search Query *[*                   ]
 Request
 
 ********** RReessppoonnssee **********
   CCrreeaatteedd UUsseerr NNaammee SSuummmmaarryy UURRLL
 {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/index.html` & `GraphSpy-1.1.3/GraphSpy/templates/index.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/layout.html` & `GraphSpy-1.1.3/GraphSpy/templates/layout.html`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                         </ul>
                     </li>
                     <li class="nav-item">
                         <a class="nav-link" href="{{url_for('device_codes')}}">Device Codes</a>
                     </li>
                     <li class="nav-item dropdown">
                         <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
-                            Graph
+                            Custom
                         </a>
                         <ul class="dropdown-menu">
                             <li><a class="dropdown-item" href="{{url_for('custom_requests')}}">Custom Requests</a></li>
                             <li><a class="dropdown-item" href="{{url_for('generic_search')}}">Generic MSGraph Search</a></li>
                         </ul>
                     </li>
                     <li class="nav-item dropdown">
@@ -75,15 +75,15 @@
                             <li><a class="dropdown-item" href="{{url_for('sharepoint')}}">SharePoint Files</a></li>
                         </ul>
                     </li>
                     <li class="nav-item">
                         <a class="nav-link" href="{{url_for('outlook')}}">Outlook</a>
                     </li>
                     <li class="nav-item">
-                        <span class="d-inline-block" id="nav-teams-disabled" data-bs-toggle="popover" data-bs-trigger="hover focus" data-bs-content="Coming soon!" data-bs-placement="bottom" >
+                        <span class="d-inline-block" id="nav-teams-disabled" data-bs-toggle="popover" data-bs-trigger="hover focus" data-bs-content="Coming soon!" data-bs-placement="bottom">
                             <a class="nav-link disabled">Teams</a>
                         </span>
                     </li>
                 </ul>
             </div>
             <div>
                 <ul class="navbar-nav justify-content-end">
@@ -142,16 +142,16 @@
                 </form>
                 <br>
             </div>
             <div>
                 <h4>Access Token</h4>
                 <form id="side_menu_access_token_form" class="row row-cols-auto">
                     <div class="input-group">
-                        <input type="text" id="access_token_id_side" class="form-control" size="1" required>
-                        <button type="Button" class="btn btn-outline-primary" onclick="setActiveAccessToken(access_token_id_side.value);">Set active access token</button>
+                        <input type="text" id="access_token_id_side" class="form-control" size="1" readonly>
+                        <button type="Button" class="btn btn-outline-primary" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
                     </div>
                 </form>
                 <div class="card text-bg-secondary mb-3 mt-3" id="access_token_card">
                     <div class="card-body">
                         <dl>
                             <dt>User</dt>
                             <dd id="access_token_info_user"></dd>
@@ -168,15 +168,15 @@
                 </div>
             </div>
             <div>
                 <h4>Refresh Token</h4>
                 <form id="side_menu_refresh_token_form" class="row row-cols-auto">
                     <div class="input-group">
                         <input type="text" id="refresh_token_id_side" class="form-control" size="1" required>
-                        <button type="Button" class="btn btn-outline-primary" onclick="setActiveRefreshToken(refresh_token_id_side.value);obtainRefreshTokenInfo()">Set active refresh token</button>
+                        <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#refresh_token_modal" onclick="$('#refresh_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
                     </div>
                 </form>
                 <div class="card text-bg-secondary mb-3 mt-3" id="refresh_token_card">
                     <div class="card-body">
                         <dl>
                             <dt>User</dt>
                             <dd id="refresh_token_info_user"></dd>
@@ -262,14 +262,17 @@
             $('#refresh_token_info_description').text(refresh_token_info.description);
             $('#refresh_token_info_tenant_id').text(refresh_token_info.tenant_id);
             $('#refresh_token_info_foci').text(refresh_token_info.foci);
         }
         obtainAccessTokenInfo();
         obtainRefreshTokenInfo();
     </script>
+    <!-- Modals -->
+    {% include 'access_token_modal.html' %}
+    {% include 'refresh_token_modal.html' %}
     <!-- Template Content -->
     <div class="container-fluid">
         {%block content%}
         {%endblock content%}
     </div>
     <!-- Enable/Disable Datatable Error Messages -->
     <script>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 _G_r_a_p_h_S_p_y
     * _S_e_t_t_i_n_g_s
     * _T_o_k_e_n_s
           o _R_e_f_r_e_s_h_ _T_o_k_e_n_s
           o _A_c_c_e_s_s_ _T_o_k_e_n_s
     * _D_e_v_i_c_e_ _C_o_d_e_s
-    * _G_r_a_p_h
+    * _C_u_s_t_o_m
           o _C_u_s_t_o_m_ _R_e_q_u_e_s_t_s
           o _G_e_n_e_r_i_c_ _M_S_G_r_a_p_h_ _S_e_a_r_c_h
     * _F_i_l_e_s
           o _R_e_c_e_n_t_ _F_i_l_e_s
           o _F_i_l_e_s_ _S_h_a_r_e_d_ _W_i_t_h_ _M_e
           o _O_n_e_D_r_i_v_e
     * _S_h_a_r_e_P_o_i_n_t
@@ -35,21 +35,23 @@
 SharePoint
 Office 365 Management
 Microsoft Azure CLI
 Microsoft Azure PowerShell
 Refresh and activate
 
 ****** AAcccceessss TTookkeenn ******
-[ ]Set active access token
+[ ]Select...
   User
   Resource
   Client ID
   Scope
   Expires At
 ****** RReeffrreesshh TTookkeenn ******
-[ ]Set active refresh token
+[ ]Select...
   User
   Resource
   Tenant ID
   Foci
   Description
+{% include 'access_token_modal.html' %} {% include 'refresh_token_modal.html'
+%}
 {%block content%} {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/outlook.html` & `GraphSpy-1.1.3/GraphSpy/templates/outlook.html`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 <br>
 <div class="col-md-6">
     <h1>Outlook</h1>
     <form id="access_token_form" class="row g-3">
         <div class="col-md-6">
             <div class="input-group">
                 <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
                 <button type="Button" class="btn btn-outline-primary" onclick="fillAccessToken(this.closest('form'))">Set access token</button>
             </div>
         </div>
     </form>
     <br>
     <form id="outlook_form" action="https://outlook.office365.com/owa/" method="POST" target="_blank" class="row g-3">
         <div>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 {% extends 'layout.html'%} {%block content%}
 ************ OOuuttllooookk ************
-[access_token_id     ]Set access token
+[access_token_id     ]Select... Set access token
 
 Open outlook
 {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/recent_files.html` & `GraphSpy-1.1.3/GraphSpy/templates/recent_files.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 <br>
 <div class="col-6">
     <h1>Recent Files</h1>
     <form id="recent_file_form" class="row g-3">
         <div class="col-6">
             <label for="access_token_id" class="form-label">Access token id *</label>
-            <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+            <div class="input-group">
+                <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
+            </div>
         </div>
         <div>
             <button type="Button" class="btn btn-primary" onclick="generateTable()">Request</button>
         </div>
     </form>
     <script>
         getActiveAccessToken(document.getElementById("recent_file_form").access_token_id)
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% extends 'layout.html'%} {%block content%}
 ************ RReecceenntt FFiilleess ************
-Access token id *[access_token_id     ]
+Access token id *
+[access_token_id     ]Select...
 Request
 
 ********** FFiilleess **********
   CCrreeaatteedd LLaasstt MMooddiiffiieedd FFiillee NNaammee FFiillee SSiizzee UURRLL
 {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/refresh_tokens.html` & `GraphSpy-1.1.3/GraphSpy/templates/refresh_tokens.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/settings.html` & `GraphSpy-1.1.3/GraphSpy/templates/settings.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,48 +2,56 @@
 
 {%block content%}
 
 <div class="row g-5">
     <div class="col-6">
         <h1>Settings</h1>
         <div class="row g-4">
-            <div class="dropdown col-12">
-                <button class="btn btn-primary dropdown-toggle" id="bd-theme" type="button" aria-expanded="false" data-bs-toggle="dropdown" data-bs-display="static" aria-label="Toggle theme (dark)">
-                    Select theme
-                </button>
-                <ul class="dropdown-menu" aria-labelledby="bd-theme-text">
-                    <li>
-                        <button type="button" class="dropdown-item" data-bs-theme-value="light" aria-pressed="false">
-                            <i class="fi fi-rr-sun"></i> Light Mode
-                        </button>
-                    </li>
-                    <li>
-                        <button type="button" class="dropdown-item active" data-bs-theme-value="dark" aria-pressed="true">
-                            <i class="fi fi-rr-moon-stars"></i> Dark Mode
-                        </button>
-                    </li>
-                    <li>
-                        <button type="button" class="dropdown-item" data-bs-theme-value="auto" aria-pressed="false">
-                            <i class="fi fi-rr-magic-wand"></i> Auto
-                        </button>
-                    </li>
-                </ul>
-            </div>
-            <div class="dropdown col-12">
-                <button class="btn btn-primary dropdown-toggle" id="dt-error-message-dropdown" type="button" data-bs-toggle="dropdown" aria-expanded="false">
-                    DataTable Error Messages
-                </button>
-                <ul class="dropdown-menu">
-                    <li><button class="dropdown-item" id="dt-error-message-button-enabled" type="button" onclick="setTableErorMessages('enabled')">Enabled</button></li>
-                    <li><button class="dropdown-item" id="dt-error-message-button-disabled" type="button" onclick="setTableErorMessages('disabled')">Disabled</button></li>
-                </ul>
+            <div class="col-12">
+                <div class="btn-group me-3 mt-3">
+                    <button class="btn btn-primary dropdown-toggle" id="bd-theme" type="button" aria-expanded="false" data-bs-toggle="dropdown" data-bs-display="static" aria-label="Toggle theme (dark)">
+                        Select theme
+                    </button>
+                    <ul class="dropdown-menu" aria-labelledby="bd-theme-text">
+                        <li>
+                            <button type="button" class="dropdown-item" data-bs-theme-value="light" aria-pressed="false">
+                                <i class="fi fi-rr-sun"></i> Light Mode
+                            </button>
+                        </li>
+                        <li>
+                            <button type="button" class="dropdown-item active" data-bs-theme-value="dark" aria-pressed="true">
+                                <i class="fi fi-rr-moon-stars"></i> Dark Mode
+                            </button>
+                        </li>
+                        <li>
+                            <button type="button" class="dropdown-item" data-bs-theme-value="auto" aria-pressed="false">
+                                <i class="fi fi-rr-magic-wand"></i> Auto
+                            </button>
+                        </li>
+                    </ul>
+                </div>
+                <div class="btn-group me-3 mt-3">
+                    <button class="btn btn-primary dropdown-toggle" id="dt-error-message-dropdown" type="button" data-bs-toggle="dropdown" aria-expanded="false">
+                        DataTable Error Messages
+                    </button>
+                    <ul class="dropdown-menu">
+                        <li><button class="dropdown-item" id="dt-error-message-button-enabled" type="button" onclick="setTableErorMessages('enabled')">Enabled</button></li>
+                        <li><button class="dropdown-item" id="dt-error-message-button-disabled" type="button" onclick="setTableErorMessages('disabled')">Disabled</button></li>
+                    </ul>
+                </div>
+            </div>
+            <div class="col-12">
+                <div class="input-group">
+                    <input type="text" id="user_agent_field" placeholder="User Agent" class="form-control">
+                    <button class="btn btn-outline-primary" type="button" onclick="update_user_agent_button()">Set User Agent</button>
+                </div>
             </div>
         </div>
     </div>
-    <div class="col-auto ms-auto">
+    <div class="col-auto ms-auto" style="max-width: 33%;">
         <div class="card mt-3">
             <div class="card-header" style="text-align: center"><b>Persistent Settings</b></div>
             <div class="card-body">
                 <pre id="settings_json" class="mb-0"></pre>
                 <script>
                     function obtainPersistentSettings() {
                         response = $.ajax({
@@ -55,17 +63,17 @@
                         $("#settings_json").text(JSON.stringify(responseJSON, undefined, 4));
                     }
                     obtainPersistentSettings();
                 </script>
             </div>
         </div>
     </div>
-    <div class="col-lg-9">
+    <div class="col-lg-8">
         <h1>Databases</h1>
-        <div class="col-md-6">
+        <div class="col-md-9">
             <div class="input-group">
                 <span class="input-group-text">Database Folder</span>
                 <input class="form-control" id="db_folder" type="text" value="{{ config['graph_spy_db_folder'] }}" readonly>
             </div>
         </div>
         <table id="databases" class="display" style="table-layout:fixed; width:100%">
             <thead>
@@ -77,15 +85,15 @@
                     <th>Size</th>
                     <th>State</th>
                     <th>Database</th>
                 </tr>
             </thead>
         </table>
     </div>
-    <div class="col-lg-3">
+    <div class="col-lg-4">
         <h1>New Database</h1>
         <form class="row g-3">
             <div>
                 <label for="database" class="form-label">Database Name *</label>
                 <input type="text" id="database" name="database" class="form-control" required placeholder="database.db">
             </div>
             <div>
@@ -155,9 +163,19 @@
     // Activate the correct option in the dt-error-message-dropdown on page load
     var table_error_messages = "{{ config['table_error_messages'] }}";
     if (table_error_messages == "disabled") {
         $('#dt-error-message-button-disabled').addClass("active")
     } else {
         $('#dt-error-message-button-enabled').addClass("active")
     }
+
+    // User Agent
+    // Populate the user agent field
+    $("#user_agent_field").val(getUserAgent());
+    // Update User Agent
+    function update_user_agent_button() {
+        setUserAgent($("#user_agent_field").val());
+        $("#user_agent_field").val(getUserAgent());
+    }
+
 </script>
     {%endblock content%}
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
 Select theme
     * Light Mode
     * Dark Mode
     * Auto
 DataTable Error Messages
     * Enabled
     * Disabled
+[                    ]Set User Agent
 PPeerrssiisstteenntt SSeettttiinnggss
 ************ DDaattaabbaasseess ************
 Database Folder[{{ config['graph_spy_db_folder'] }}]
    LLaasstt MMooddiiffiieedd SSiizzee SSttaattee DDaattaabbaassee
 ************ NNeeww DDaattaabbaassee ************
 Database Name *[database            ]
 Create Database
```

### Comparing `GraphSpy-1.1.2/GraphSpy/templates/shared_with_me.html` & `GraphSpy-1.1.3/GraphSpy/templates/shared_with_me.html`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 <br>
 <div class="col-6">
     <h1>Files Shared with Me</h1>
     <form id="shared_file_form" class="row g-3">
         <div class="col-6">
             <label for="access_token_id" class="form-label">Access token id *</label>
-            <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+            <div class="input-group">
+                <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
+                <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
+            </div>
         </div>
         <div>
             <button type="Button" class="btn btn-primary" onclick="generateTable()">Request</button>
         </div>
     </form>
     <script>
         getActiveAccessToken(document.getElementById("shared_file_form").access_token_id)
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% extends 'layout.html'%} {%block content%}
 ************ FFiilleess SShhaarreedd wwiitthh MMee ************
-Access token id *[access_token_id     ]
+Access token id *
+[access_token_id     ]Select...
 Request
 
 ********** FFiilleess **********
   CCrreeaatteedd LLaasstt MMooddiiffiieedd FFiillee NNaammee FFiillee SSiizzee UURRLL
 {%endblock content%}
```

### Comparing `GraphSpy-1.1.2/GraphSpy.egg-info/PKG-INFO` & `GraphSpy-1.1.3/GraphSpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSpy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Initial Access and Post-Exploitation Tool for AAD and O365 with a browser-based GUI
 Home-page: https://github.com/RedByte1337/GraphSpy
 Author: RedByte1337
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GraphSpy
@@ -69,14 +69,20 @@
 graphspy -i 192.168.0.10 -p 80
 # Run GraphSpy on port 8080 on all interfaces
 graphspy -i 0.0.0.0 -p 8080
 ```
 
 For detailed instructions and other command line arguments, please refer to the [Execution page](https://github.com/RedByte1337/GraphSpy/wiki/Execution) on the wiki.
 
+## Usage
+
+Please refer to the [Github Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
+
+For a quick feature overview, check out the [official release blog post](https://insights.spotit.be/2024/04/05/graphspy-the-swiss-army-knife-for-attacking-m365-entra/).
+
 # Features
 
 ## Access and Refresh Tokens
 
 Store your access and refresh tokens for multiple users and scopes in one location. 
 
 ![Access Tokens](images/access_tokens_1.png)
@@ -111,25 +117,29 @@
 
 ![Outlook GraphSpy](images/outlook_1.png)
 
 ![Outlook](images/outlook_2.png)
 
 ## Graph Searching
 
-Search for keywords through all Microsoft 365 applications using the Microsoft 365 API.
+Search for keywords through all Microsoft 365 applications using the Microsoft Search API.
 
 For instance, use this to search for any files or emails containing keywords such as "password", "secret", ...
 
 ![Graph Search](images/graph_search_2.png)
 
-## Generic Graph Requests
+## Custom Requests
+
+Perform custom API requests towards any endpoint using access tokens stored in GraphSpy.
+
+![Custom Request](images/custom_requests.png)
 
-Perform any other MS Graph requests and display the raw response.
+Custom request templates with variables can be stored in the database to allow easy reuse of common custom API requests.
 
-![Graph Request](images/generic_graph_requests.png)
+![Custom Request](images/custom_request_templates.png)
 
 ## Multiple Databases
 
 GraphSpy supports multiple databases. This is useful when working on multiple assessments at once to keep your tokens and device codes organized.
 
 ![Graph Request](images/settings.png)
 
@@ -140,15 +150,14 @@
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
-* Set a custom user agent
 * Microsoft Teams
 	* Sadly, most MSGrapgh scopes required for Microsoft Teams can not be obtained through a FOCI client id, limiting the usecases where it could be accessed.
 	* So the best option would be to use the Skype API, which is a FOCI resource, although this API is not documented by Microsoft or intended for public use
 * Azure AD
 	* List Users, Groups, Applications, Devices, Conditional Access Policies, ...
 * Cleaner exception handling
 	* While this should not have any direct impact on the user, edge cases might currently throw exceptions to the GraphSpy output instead of handling them in a cleaner way.
```

### Comparing `GraphSpy-1.1.2/GraphSpy.egg-info/SOURCES.txt` & `GraphSpy-1.1.3/GraphSpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 GraphSpy/static/css/style.css
 GraphSpy/static/js/functions.js
 GraphSpy/static/js/theme.js
 GraphSpy/templates/OneDrive.html
 GraphSpy/templates/SharePoint.html
 GraphSpy/templates/SharePointDrives.html
 GraphSpy/templates/SharePointSites.html
+GraphSpy/templates/access_token_modal.html
 GraphSpy/templates/access_tokens.html
 GraphSpy/templates/custom_requests.html
 GraphSpy/templates/device_codes.html
 GraphSpy/templates/generic_search.html
 GraphSpy/templates/index.html
 GraphSpy/templates/layout.html
 GraphSpy/templates/outlook.html
 GraphSpy/templates/recent_files.html
+GraphSpy/templates/refresh_token_modal.html
 GraphSpy/templates/refresh_tokens.html
 GraphSpy/templates/settings.html
 GraphSpy/templates/shared_with_me.html
```

### Comparing `GraphSpy-1.1.2/LICENSE.txt` & `GraphSpy-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.2/PKG-INFO` & `GraphSpy-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSpy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Initial Access and Post-Exploitation Tool for AAD and O365 with a browser-based GUI
 Home-page: https://github.com/RedByte1337/GraphSpy
 Author: RedByte1337
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GraphSpy
@@ -69,14 +69,20 @@
 graphspy -i 192.168.0.10 -p 80
 # Run GraphSpy on port 8080 on all interfaces
 graphspy -i 0.0.0.0 -p 8080
 ```
 
 For detailed instructions and other command line arguments, please refer to the [Execution page](https://github.com/RedByte1337/GraphSpy/wiki/Execution) on the wiki.
 
+## Usage
+
+Please refer to the [Github Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
+
+For a quick feature overview, check out the [official release blog post](https://insights.spotit.be/2024/04/05/graphspy-the-swiss-army-knife-for-attacking-m365-entra/).
+
 # Features
 
 ## Access and Refresh Tokens
 
 Store your access and refresh tokens for multiple users and scopes in one location. 
 
 ![Access Tokens](images/access_tokens_1.png)
@@ -111,25 +117,29 @@
 
 ![Outlook GraphSpy](images/outlook_1.png)
 
 ![Outlook](images/outlook_2.png)
 
 ## Graph Searching
 
-Search for keywords through all Microsoft 365 applications using the Microsoft 365 API.
+Search for keywords through all Microsoft 365 applications using the Microsoft Search API.
 
 For instance, use this to search for any files or emails containing keywords such as "password", "secret", ...
 
 ![Graph Search](images/graph_search_2.png)
 
-## Generic Graph Requests
+## Custom Requests
+
+Perform custom API requests towards any endpoint using access tokens stored in GraphSpy.
+
+![Custom Request](images/custom_requests.png)
 
-Perform any other MS Graph requests and display the raw response.
+Custom request templates with variables can be stored in the database to allow easy reuse of common custom API requests.
 
-![Graph Request](images/generic_graph_requests.png)
+![Custom Request](images/custom_request_templates.png)
 
 ## Multiple Databases
 
 GraphSpy supports multiple databases. This is useful when working on multiple assessments at once to keep your tokens and device codes organized.
 
 ![Graph Request](images/settings.png)
 
@@ -140,15 +150,14 @@
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
-* Set a custom user agent
 * Microsoft Teams
 	* Sadly, most MSGrapgh scopes required for Microsoft Teams can not be obtained through a FOCI client id, limiting the usecases where it could be accessed.
 	* So the best option would be to use the Skype API, which is a FOCI resource, although this API is not documented by Microsoft or intended for public use
 * Azure AD
 	* List Users, Groups, Applications, Devices, Conditional Access Policies, ...
 * Cleaner exception handling
 	* While this should not have any direct impact on the user, edge cases might currently throw exceptions to the GraphSpy output instead of handling them in a cleaner way.
```

### Comparing `GraphSpy-1.1.2/README.md` & `GraphSpy-1.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,20 @@
 graphspy -i 192.168.0.10 -p 80
 # Run GraphSpy on port 8080 on all interfaces
 graphspy -i 0.0.0.0 -p 8080
 ```
 
 For detailed instructions and other command line arguments, please refer to the [Execution page](https://github.com/RedByte1337/GraphSpy/wiki/Execution) on the wiki.
 
+## Usage
+
+Please refer to the [Github Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
+
+For a quick feature overview, check out the [official release blog post](https://insights.spotit.be/2024/04/05/graphspy-the-swiss-army-knife-for-attacking-m365-entra/).
+
 # Features
 
 ## Access and Refresh Tokens
 
 Store your access and refresh tokens for multiple users and scopes in one location. 
 
 ![Access Tokens](images/access_tokens_1.png)
@@ -102,25 +108,29 @@
 
 ![Outlook GraphSpy](images/outlook_1.png)
 
 ![Outlook](images/outlook_2.png)
 
 ## Graph Searching
 
-Search for keywords through all Microsoft 365 applications using the Microsoft 365 API.
+Search for keywords through all Microsoft 365 applications using the Microsoft Search API.
 
 For instance, use this to search for any files or emails containing keywords such as "password", "secret", ...
 
 ![Graph Search](images/graph_search_2.png)
 
-## Generic Graph Requests
+## Custom Requests
+
+Perform custom API requests towards any endpoint using access tokens stored in GraphSpy.
+
+![Custom Request](images/custom_requests.png)
 
-Perform any other MS Graph requests and display the raw response.
+Custom request templates with variables can be stored in the database to allow easy reuse of common custom API requests.
 
-![Graph Request](images/generic_graph_requests.png)
+![Custom Request](images/custom_request_templates.png)
 
 ## Multiple Databases
 
 GraphSpy supports multiple databases. This is useful when working on multiple assessments at once to keep your tokens and device codes organized.
 
 ![Graph Request](images/settings.png)
 
@@ -131,15 +141,14 @@
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
-* Set a custom user agent
 * Microsoft Teams
 	* Sadly, most MSGrapgh scopes required for Microsoft Teams can not be obtained through a FOCI client id, limiting the usecases where it could be accessed.
 	* So the best option would be to use the Skype API, which is a FOCI resource, although this API is not documented by Microsoft or intended for public use
 * Azure AD
 	* List Users, Groups, Applications, Devices, Conditional Access Policies, ...
 * Cleaner exception handling
 	* While this should not have any direct impact on the user, edge cases might currently throw exceptions to the GraphSpy output instead of handling them in a cleaner way.
```

### Comparing `GraphSpy-1.1.2/setup.py` & `GraphSpy-1.1.3/setup.py`

 * *Files identical despite different names*

