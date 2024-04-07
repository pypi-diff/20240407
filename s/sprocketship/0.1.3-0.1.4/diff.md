# Comparing `tmp/sprocketship-0.1.3.tar.gz` & `tmp/sprocketship-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.1.3.tar", last modified: Sat Apr  6 20:07:15 2024, max compression
+gzip compressed data, was "sprocketship-0.1.4.tar", last modified: Sat Apr  6 22:17:51 2024, max compression
```

## Comparing `sprocketship-0.1.3.tar` & `sprocketship-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:07:15.364867 sprocketship-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 20:07:10.000000 sprocketship-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 20:07:10.000000 sprocketship-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 20:07:15.364867 sprocketship-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-06 20:07:10.000000 sprocketship-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 20:07:10.000000 sprocketship-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:07:15.364867 sprocketship-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:07:15.364867 sprocketship-0.1.3/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 20:07:10.000000 sprocketship-0.1.3/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:07:15.364867 sprocketship-0.1.3/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-06 20:07:10.000000 sprocketship-0.1.3/sprocketship/templates/javascript.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:07:15.364867 sprocketship-0.1.3/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:17:51.763069 sprocketship-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 22:17:47.000000 sprocketship-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 22:17:47.000000 sprocketship-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-06 22:17:51.763069 sprocketship-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-06 22:17:47.000000 sprocketship-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 22:17:47.000000 sprocketship-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 22:17:51.763069 sprocketship-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:17:51.759069 sprocketship-0.1.4/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-06 22:17:47.000000 sprocketship-0.1.4/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:17:51.763069 sprocketship-0.1.4/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-06 22:17:47.000000 sprocketship-0.1.4/sprocketship/templates/javascript.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:17:51.763069 sprocketship-0.1.4/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 22:17:51.000000 sprocketship-0.1.4/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.1.3/LICENSE` & `sprocketship-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.1.3/PKG-INFO` & `sprocketship-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.1.3
+Version: 0.1.4
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,15 @@
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px; text-decoration: none;">
+  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 60px; text-decoration: none;">
     ⚙️ 🚀
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
   </p>
@@ -129,28 +129,25 @@
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
 procedures:
   development:
     - name: create_temp_database
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
     - name: create_database_reader
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
     - name: create_database_writer
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 From here, simply run
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.1.3 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.1.4 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
@@ -32,19 +32,18 @@
 ` directory at the same level in a directory structure. ``` âââ
 dbt_models â âââ customers.sql â âââ products.sql âââ
 procedures â âââ admin â â âââ create_database_writer_role.js
 â â âââ create_database_reader_role.js â âââ development â
 â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
 path to each procedure in the `sprocketship.yml` should follow that of the
 paths to their corresponding files in the `procedures/` directory. ```
-procedures: development: - name: create_temp_database replace_if_exists: true
-database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
-admin: - name: create_database_reader replace_if_exists: true database:
-!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... - name:
-create_database_writer replace_if_exists: true database: !env_var
+procedures: development: - name: create_temp_database database: !env_var
+SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name:
+create_database_reader database: !env_var SNOWFLAKE_DATABASE schema: !env_var
+SNOWFLAKE_SCHEMA ... - name: create_database_writer database: !env_var
 SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
 run `$ sprocketship liftoff` from the project directory (or provide the
 directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
 launch your stored procedures into the given directory. ### Exhaustive Options
 for Stored Procedure Configuration ``` name: The name of the procedure
 database: The name of the database where the procedure will be stored schema:
 The name of the schema where the procedure will be stored language: The
```

### Comparing `sprocketship-0.1.3/README.md` & `sprocketship-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px; text-decoration: none;">
+  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 60px; text-decoration: none;">
     ⚙️ 🚀
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
   </p>
@@ -111,28 +111,25 @@
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
 procedures:
   development:
     - name: create_temp_database
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
     - name: create_database_reader
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
     - name: create_database_writer
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 From here, simply run
```

#### html2text {}

```diff
@@ -23,19 +23,18 @@
 ` directory at the same level in a directory structure. ``` âââ
 dbt_models â âââ customers.sql â âââ products.sql âââ
 procedures â âââ admin â â âââ create_database_writer_role.js
 â â âââ create_database_reader_role.js â âââ development â
 â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
 path to each procedure in the `sprocketship.yml` should follow that of the
 paths to their corresponding files in the `procedures/` directory. ```
-procedures: development: - name: create_temp_database replace_if_exists: true
-database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
-admin: - name: create_database_reader replace_if_exists: true database:
-!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... - name:
-create_database_writer replace_if_exists: true database: !env_var
+procedures: development: - name: create_temp_database database: !env_var
+SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name:
+create_database_reader database: !env_var SNOWFLAKE_DATABASE schema: !env_var
+SNOWFLAKE_SCHEMA ... - name: create_database_writer database: !env_var
 SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
 run `$ sprocketship liftoff` from the project directory (or provide the
 directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
 launch your stored procedures into the given directory. ### Exhaustive Options
 for Stored Procedure Configuration ``` name: The name of the procedure
 database: The name of the database where the procedure will be stored schema:
 The name of the schema where the procedure will be stored language: The
```

### Comparing `sprocketship-0.1.3/pyproject.toml` & `sprocketship-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-0.1.3/sprocketship/cli.py` & `sprocketship-0.1.4/sprocketship/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,41 +34,43 @@
 
 def create_javascript_stored_procedure(**kwargs):
     path = os.path.join(kwargs['project_dir'], get_full_file_path(kwargs))
     procedure_def_dict = {'procedure_definition': get_file_contents(path)}
     return render_file(os.path.join(Path(__file__).parent, "templates/javascript.sql"), **kwargs, **procedure_def_dict)
 
 
-@click.command()
-@click.argument("subcommand", type=click.Choice(["liftoff"]))
+@click.group()
+def main():
+    pass
+
+@main.command()
 @click.argument("dir", default=".")
 @click.option('--show', is_flag=True)
-def main(subcommand, dir, show):
-    if subcommand == "liftoff":
-        click.echo(click.style(f"🚀 Sprocketship lifting off!", fg='white', bold=True))
-        # Open config in current directory
-
-        data = render_file(os.path.join(dir, '.sprocketship.yml'), return_dict=True)
-
-        con = connector.connect(**data["snowflake"])
-
-        # Get the configurations for each procedure and attach relative path to file directory
-        configs_with_paths = extract_configs(data["procedures"])
-        procs = list(itertools.chain(*configs_with_paths.values()))
-
-        for proc in procs:
-            try:
-                rendered_proc = create_javascript_stored_procedure(**proc, **{'project_dir': dir})
-                con.cursor().execute(rendered_proc)
-                msg = click.style(f"{proc['name']} ", fg='green', bold=True)
-                msg += click.style(f"launched into schema ", fg='white', bold=True)
-                msg += click.style(f"{proc['database']}.{proc['schema']}", fg='blue', bold=True)
-                click.echo(msg)
-                if show:
-                    click.echo(rendered_proc)
-            except Exception as e:
-                msg = click.style(f"{proc['name']} ", fg='red', bold=True)
-                msg += click.style(f"could not be launched into schema ", fg='white', bold=True)
-                msg += click.style(f"{proc['database']}.{proc['schema']}", fg='blue', bold=True)
-                click.echo(msg)
-                click.echo(e, err=True)
+def liftoff(dir, show):
+    click.echo(click.style(f"🚀 Sprocketship lifting off!", fg='white', bold=True))
+    # Open config in current directory
+
+    data = render_file(os.path.join(dir, '.sprocketship.yml'), return_dict=True)
+
+    con = connector.connect(**data["snowflake"])
+
+    # Get the configurations for each procedure and attach relative path to file directory
+    configs_with_paths = extract_configs(data["procedures"])
+    procs = list(itertools.chain(*configs_with_paths.values()))
+
+    for proc in procs:
+        try:
+            rendered_proc = create_javascript_stored_procedure(**proc, **{'project_dir': dir})
+            con.cursor().execute(rendered_proc)
+            msg = click.style(f"{proc['name']} ", fg='green', bold=True)
+            msg += click.style(f"launched into schema ", fg='white', bold=True)
+            msg += click.style(f"{proc['database']}.{proc['schema']}", fg='blue', bold=True)
+            click.echo(msg)
+            if show:
                 click.echo(rendered_proc)
+        except Exception as e:
+            msg = click.style(f"{proc['name']} ", fg='red', bold=True)
+            msg += click.style(f"could not be launched into schema ", fg='white', bold=True)
+            msg += click.style(f"{proc['database']}.{proc['schema']}", fg='blue', bold=True)
+            click.echo(msg)
+            click.echo(e, err=True)
+            click.echo(rendered_proc)
```

### Comparing `sprocketship-0.1.3/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.1.4/sprocketship.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.1.3
+Version: 0.1.4
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,15 @@
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px; text-decoration: none;">
+  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 60px; text-decoration: none;">
     ⚙️ 🚀
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
   </p>
@@ -129,28 +129,25 @@
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
 procedures:
   development:
     - name: create_temp_database
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
     - name: create_database_reader
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
     - name: create_database_writer
-      replace_if_exists: true
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 From here, simply run
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.1.3 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.1.4 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
@@ -32,19 +32,18 @@
 ` directory at the same level in a directory structure. ``` âââ
 dbt_models â âââ customers.sql â âââ products.sql âââ
 procedures â âââ admin â â âââ create_database_writer_role.js
 â â âââ create_database_reader_role.js â âââ development â
 â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
 path to each procedure in the `sprocketship.yml` should follow that of the
 paths to their corresponding files in the `procedures/` directory. ```
-procedures: development: - name: create_temp_database replace_if_exists: true
-database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
-admin: - name: create_database_reader replace_if_exists: true database:
-!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... - name:
-create_database_writer replace_if_exists: true database: !env_var
+procedures: development: - name: create_temp_database database: !env_var
+SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name:
+create_database_reader database: !env_var SNOWFLAKE_DATABASE schema: !env_var
+SNOWFLAKE_SCHEMA ... - name: create_database_writer database: !env_var
 SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
 run `$ sprocketship liftoff` from the project directory (or provide the
 directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
 launch your stored procedures into the given directory. ### Exhaustive Options
 for Stored Procedure Configuration ``` name: The name of the procedure
 database: The name of the database where the procedure will be stored schema:
 The name of the schema where the procedure will be stored language: The
```

