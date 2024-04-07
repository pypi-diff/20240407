# Comparing `tmp/special-octo-robot-0.0.1.tar.gz` & `tmp/special-octo-robot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special-octo-robot-0.0.1.tar", last modified: Wed Apr  3 14:59:19 2024, max compression
+gzip compressed data, was "special-octo-robot-0.0.4.tar", last modified: Sun Apr  7 13:16:26 2024, max compression
```

## Comparing `special-octo-robot-0.0.1.tar` & `special-octo-robot-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.1/LICENSE
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.1/MANIFEST.in
--rw-r--r--   0 nginx     (1000) nginx     (1000)     3382 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     2840 2024-03-18 09:00:15.000000 special-octo-robot-0.0.1/README.md
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/app/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.1/app/__init__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.1/app/__main__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-04-03 14:56:33.000000 special-octo-robot-0.0.1/app/__version__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     5661 2024-04-03 13:26:57.000000 special-octo-robot-0.0.1/app/application.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1676 2024-04-03 14:45:02.000000 special-octo-robot-0.0.1/app/console.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1949 2024-04-03 13:30:37.000000 special-octo-robot-0.0.1/app/database.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     5279 2024-04-02 13:03:22.000000 special-octo-robot-0.0.1/devcord.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/setup.cfg
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1053 2024-04-03 14:57:12.000000 special-octo-robot-0.0.1/setup.py
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/special_octo_robot.egg-info/
--rw-r--r--   0 nginx     (1000) nginx     (1000)     3382 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      404 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/SOURCES.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/dependency_links.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/entry_points.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       26 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/requires.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/top_level.txt
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.4/LICENSE
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.4/MANIFEST.in
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     3564 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     3022 2024-04-07 04:26:45.000000 special-octo-robot-0.0.4/README.md
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/app/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.4/app/__init__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.4/app/__main__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-04-07 12:40:37.000000 special-octo-robot-0.0.4/app/__version__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     6022 2024-04-07 12:36:04.000000 special-octo-robot-0.0.4/app/application.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     3423 2024-04-07 11:46:37.000000 special-octo-robot-0.0.4/app/console.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      396 2024-04-07 11:44:42.000000 special-octo-robot-0.0.4/app/constants.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1904 2024-04-07 12:35:34.000000 special-octo-robot-0.0.4/app/database.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     5662 2024-04-07 12:36:04.000000 special-octo-robot-0.0.4/devcord.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/setup.cfg
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1053 2024-04-03 14:57:12.000000 special-octo-robot-0.0.4/setup.py
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/special_octo_robot.egg-info/
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     3564 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      421 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/SOURCES.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/dependency_links.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/entry_points.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       26 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/requires.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/top_level.txt
```

### Comparing `special-octo-robot-0.0.1/LICENSE` & `special-octo-robot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.1/PKG-INFO` & `special-octo-robot-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0.0.1
+Version: 0.0.4
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
@@ -59,15 +59,15 @@
 Complete by today:
 
 ```bash
 $ devcord tasks -a "task name" -t
 $ devcord tasks --add "task name" --today
 ```
 
-Complete in next 7 days:
+Complete in current week:
 
 ```bash
 $ devcord tasks -a "task name" -w
 $ devcord tasks --add "task name" --week
 ```
 
 With priority (1-5):
@@ -119,61 +119,73 @@
 List today's tasks:
 
 ```bash
 $ devcord tasks -l -t
 $ devcord tasks --list --today
 ```
 
-List tasks due in next 7 days:
+List tasks due in current week:
 
 ```bash
 $ devcord tasks -l -w
 $ devcord tasks --list --week
 ```
 
 List tasks by status:
 
 ```bash
 $ devcord tasks -l -i
-$ devcord tasks --list --complete
+$ devcord tasks --list --completed
 $ devcord tasks -l --pending
 ```
 
+Specify Output Format:
+
+```bash
+$ devcord tasks -l -o json
+$ devcord tasks --list --output text
+```
+
+Specify Output File:
+
+```bash
+$ devcord tasks -l --path "path/to/file"
+```
 ## For managing tasks
 
 Pass the task ID after the **"task"** keyword to perform any action on the task.
 
 Viewing description:
 
 ```bash
 $ devcord task 1 -d
 $ devcord task 1 --desc
 ```
 
 _Opens a scrollable text box with description_
 
-Show substask:
+Show substasks:
 
 ```bash
 $ devcord task 4 -st
-$ devcord task 4 --subtask
+$ devcord task 4 --subtasks
 ```
 
 Mark as inprogress:
 
 ```bash
 $ devcord task 3 -i
 $ devcord task 3 --inprogress
 ```
 
 Mark as complete:
 
 ```bash
 $ devcord task 2 -c
-$ devcord task 2 --complete
+$ devcord task 2 --completed
 ```
 
 Mark as pending:
 
 ```bash
 $ devcord task 10 -pd
 $ devcord task 10 --pending
```

### Comparing `special-octo-robot-0.0.1/README.md` & `special-octo-robot-0.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 Complete by today:
 
 ```bash
 $ devcord tasks -a "task name" -t
 $ devcord tasks --add "task name" --today
 ```
 
-Complete in next 7 days:
+Complete in current week:
 
 ```bash
 $ devcord tasks -a "task name" -w
 $ devcord tasks --add "task name" --week
 ```
 
 With priority (1-5):
@@ -103,61 +103,73 @@
 List today's tasks:
 
 ```bash
 $ devcord tasks -l -t
 $ devcord tasks --list --today
 ```
 
-List tasks due in next 7 days:
+List tasks due in current week:
 
 ```bash
 $ devcord tasks -l -w
 $ devcord tasks --list --week
 ```
 
 List tasks by status:
 
 ```bash
 $ devcord tasks -l -i
-$ devcord tasks --list --complete
+$ devcord tasks --list --completed
 $ devcord tasks -l --pending
 ```
 
+Specify Output Format:
+
+```bash
+$ devcord tasks -l -o json
+$ devcord tasks --list --output text
+```
+
+Specify Output File:
+
+```bash
+$ devcord tasks -l --path "path/to/file"
+```
 ## For managing tasks
 
 Pass the task ID after the **"task"** keyword to perform any action on the task.
 
 Viewing description:
 
 ```bash
 $ devcord task 1 -d
 $ devcord task 1 --desc
 ```
 
 _Opens a scrollable text box with description_
 
-Show substask:
+Show substasks:
 
 ```bash
 $ devcord task 4 -st
-$ devcord task 4 --subtask
+$ devcord task 4 --subtasks
 ```
 
 Mark as inprogress:
 
 ```bash
 $ devcord task 3 -i
 $ devcord task 3 --inprogress
 ```
 
 Mark as complete:
 
 ```bash
 $ devcord task 2 -c
-$ devcord task 2 --complete
+$ devcord task 2 --completed
 ```
 
 Mark as pending:
 
 ```bash
 $ devcord task 10 -pd
 $ devcord task 10 --pending
```

### Comparing `special-octo-robot-0.0.1/app/application.py` & `special-octo-robot-0.0.4/app/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from datetime import datetime
 
-from . import console
 from . import database
 
 
 def list_tasks(
     priority=None,
     today=None,
     week=None,
@@ -12,15 +11,15 @@
     completed=None,
     pending=None,
     label=None,
 ) -> list:
     """
     List all the tasks based on the filters.
     """
-    order_by = "completed ASC, priority DESC"
+    order_by = "completed ASC, status ASC, priority DESC"
     where_clause = ["parent_id ISNULL"]
     if week:
         where_clause.append(
             "(deadline >= date('now', 'weekday 0', '-7 days') AND deadline < date('now', 'weekday 1'))",
         )
     elif today:
         where_clause.append("(deadline = date('now'))")
@@ -49,14 +48,15 @@
         columns=[
             "id",
             "title",
             "status",
             "deadline",
             "priority",
             "label",
+            "description",
         ],
         where_clause=where_clause,
         order_by=f"ORDER BY {order_by}",
     )
 
     final_results = []
     for result in results:
@@ -68,14 +68,15 @@
                 "deadline": (
                     result[3]
                     if str(result[3]) == "None"
                     else convert_to_console_date(result[3])
                 ),
                 "priority": result[4],
                 "label": result[5] if result[5] else "None",
+                "description": result[6],
             },
         )
     return final_results
 
 
 def add_tasks(
     title,
@@ -90,18 +91,18 @@
     label=None,
     parent=None,
 ):
     """
     Add a task to the database.
     """
     columns = ["title"]
-    values = [title]
+    values = [f'"{sanitize_text(title)}"' ""]
     if description:
         columns.append("description")
-        values.append(f'"{description}"')
+        values.append(f'"{sanitize_text(description)}"')
     if priority:
         columns.append("priority")
         values.append(str(priority))
     if today:
         columns.append("deadline")
         values.append("date('now')")
     elif week:
@@ -117,15 +118,15 @@
         columns.append("status")
         values.append("'Completed'")
     elif pending:
         columns.append("status")
         values.append("'Pending'")
     if label:
         columns.append("label")
-        values.append(f'"{label}"')
+        values.append(f'"{sanitize_text(label)}"')
     if parent:
         columns.append("parent_id")
         values.append(str(parent))
     database.insert_into_table(table="tasks", columns=columns, values=values)
 
 
 def search_task(task_id) -> dict:
@@ -152,15 +153,15 @@
     if task:
         task = task[0]
         task_details = {
             "id": task[0],
             "title": task[1],
             "description": task[2],
             "status": task[3],
-            "deadline": (task[4]),
+            "deadline": task[4],
             "priority": task[5],
             "label": task[6] if task[6] else "None",
             "completed": (task[7]),
         }
     return task_details
 
 
@@ -194,21 +195,31 @@
             },
         )
     return final_results
 
 
 def update_task(updated_data: dict):
     """If marked as completed then set datetime as now else prev value retain"""
+    updated_data["deadline"] = str(updated_data["deadline"])
     if updated_data["status"] == "Completed":
         current_date = datetime.now().strftime("%Y-%m-%d")
-        updated_data["completed"] = current_date
+        updated_data["completed"] = str(current_date)
     else:
         updated_data["completed"] = updated_data["deadline"]
+
+    for key, value in updated_data.items():
+        if type(value) is str:
+            updated_data[key] = f'"{value}"'
+
     database.update_table("tasks", updated_data)
 
 
 def convert_to_console_date(date_str):
     """
     Convert date from "YYYY-MM-DD" to "dd/mm/yyyy"
     """
     date_obj = datetime.strptime(date_str, "%Y-%m-%d")
     return date_obj.strftime("%d/%m/%Y")
+
+
+def sanitize_text(text):
+    return text.replace('"', "'")
```

### Comparing `special-octo-robot-0.0.1/app/database.py` & `special-octo-robot-0.0.4/app/database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import os
 import sqlite3
 
-import click
-
-path = os.path.join(os.getenv("HOME"), ".devcord", "data.db")
+from .constants import path
 
 
 def initialize():
     """
     Initialize the database with all the necessary tables.
     """
     conn = sqlite3.connect(path)
@@ -16,15 +13,15 @@
         """CREATE TABLE tasks(
         id INTEGER PRIMARY KEY AUTOINCREMENT,
         title VARCHAR NOT NULL, parent_id INTEGER,
         description TEXT,
         status VARCHAR DEFAULT 'Pending',
         deadline DATE DEFAULT 'None',
         priority INTEGER DEFAULT 0,
-        label VARCHAR,
+        label VARCHAR DEFAULT 'None',
         completed DATE
         )""",
     )
     cur.execute(
         """
         CREATE TRIGGER initialize_completed_column
         AFTER INSERT ON tasks
@@ -65,14 +62,14 @@
 
 
 def update_table(table: str, new_data: dict) -> None:
     """
     Update Values Of Given Table
     """
     set_clause = ", ".join(
-        [f"{key} = '{value}'" for key, value in new_data.items() if key != "id"],
+        [f"{key} = {value}" for key, value in new_data.items() if key != "id"],
     )
     query = f"UPDATE {table} SET {set_clause} WHERE id = {new_data['id']}"
     conn = sqlite3.connect(path)
     cur = conn.cursor()
     cur.execute(query)
     conn.commit()
```

### Comparing `special-octo-robot-0.0.1/devcord.py` & `special-octo-robot-0.0.4/devcord.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 import os
 from datetime import datetime
 
 import click
 
 import app.application as application
 from app.console import print_tasks
+from app.constants import path
 from app.database import initialize
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 @click.pass_context
 def cli(ctx):
     """
     Devcord is a CLI tool for developers to help them with their daily tasks.
     """
     ctx.ensure_object(dict)
-    path = os.path.join(os.getenv("HOME"), ".devcord", "data.db")
+    if not path:
+        click.echo(
+            click.style(
+                "Error: Could not find the path to the database, raise an issue with the developers.",
+                fg="red",
+            ),
+        )
+        ctx.abort()
+        return
+
     if not os.path.exists(path):
         os.makedirs(os.path.dirname(path), exist_ok=True)
         initialize()
 
 
 @cli.command()
 @click.pass_context
@@ -62,28 +72,32 @@
 )
 @click.option(
     "-lb",
     "--label",
     help="Perform for all the tasks with a specific label",
     type=str,
 )
+@click.option("-o", "--output", help="Specify Output Format", type=str)
+@click.option("--path", help="Specify Output File", type=str)
 @click.option("-pid", "--parent", help="Set the parent of a task", type=int)
 def tasks(
     ctx,
     list=None,
     add=None,
     desc=None,
     priority=None,
     today=None,
     week=None,
     deadline=None,
     inprogress=None,
     completed=None,
     pending=None,
     label=None,
+    output=None,
+    path=None,
     parent=None,
 ):
     """
     Create and List tasks.
     """
     if deadline:
         try:
@@ -105,18 +119,20 @@
                 today=today,
                 week=week,
                 inprogress=inprogress,
                 completed=completed,
                 pending=pending,
                 label=label,
             ),
+            output,
+            path,
         )
     elif add:
         description = None
-        add = f'"{add}"'
+        add = add
         if desc:
             description = click.edit()
         if parent:
             val = application.search_task(parent)
             if not val:
                 click.echo(
                     click.style(
@@ -165,31 +181,31 @@
     "-pd",
     "--pending",
     is_flag=True,
     help="Mark Task As Pending",
 )
 @click.option(
     "-st",
-    "--subtask",
+    "--subtasks",
     is_flag=True,
     help="List All Subtask Of Task",
 )
 def task(
     ctx,
     task_id,
     desc=None,
     inprogress=None,
     completed=None,
     pending=None,
-    subtask=None,
+    subtasks=None,
 ):
     """
     Modify a specific task.
     """
-    if subtask:
+    if subtasks:
         print_tasks(application.get_subtasks(task_id))
         return
 
     current_task = application.search_task(task_id)
     if not current_task:
         click.echo(
             click.style(
@@ -199,16 +215,15 @@
         )
         return
 
     if desc:
         description = "No given description"
         if current_task["description"]:
             description = current_task["description"]
-        description = click.edit(description)
-        current_task["description"] = description
+        current_task["description"] = click.edit(description)
 
     if inprogress:
         current_task["status"] = "In Progress"
     elif pending:
         current_task["status"] = "Pending"
     elif completed:
         current_task["status"] = "Completed"
```

### Comparing `special-octo-robot-0.0.1/setup.py` & `special-octo-robot-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.1/special_octo_robot.egg-info/PKG-INFO` & `special-octo-robot-0.0.4/special_octo_robot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0.0.1
+Version: 0.0.4
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
@@ -59,15 +59,15 @@
 Complete by today:
 
 ```bash
 $ devcord tasks -a "task name" -t
 $ devcord tasks --add "task name" --today
 ```
 
-Complete in next 7 days:
+Complete in current week:
 
 ```bash
 $ devcord tasks -a "task name" -w
 $ devcord tasks --add "task name" --week
 ```
 
 With priority (1-5):
@@ -119,61 +119,73 @@
 List today's tasks:
 
 ```bash
 $ devcord tasks -l -t
 $ devcord tasks --list --today
 ```
 
-List tasks due in next 7 days:
+List tasks due in current week:
 
 ```bash
 $ devcord tasks -l -w
 $ devcord tasks --list --week
 ```
 
 List tasks by status:
 
 ```bash
 $ devcord tasks -l -i
-$ devcord tasks --list --complete
+$ devcord tasks --list --completed
 $ devcord tasks -l --pending
 ```
 
+Specify Output Format:
+
+```bash
+$ devcord tasks -l -o json
+$ devcord tasks --list --output text
+```
+
+Specify Output File:
+
+```bash
+$ devcord tasks -l --path "path/to/file"
+```
 ## For managing tasks
 
 Pass the task ID after the **"task"** keyword to perform any action on the task.
 
 Viewing description:
 
 ```bash
 $ devcord task 1 -d
 $ devcord task 1 --desc
 ```
 
 _Opens a scrollable text box with description_
 
-Show substask:
+Show substasks:
 
 ```bash
 $ devcord task 4 -st
-$ devcord task 4 --subtask
+$ devcord task 4 --subtasks
 ```
 
 Mark as inprogress:
 
 ```bash
 $ devcord task 3 -i
 $ devcord task 3 --inprogress
 ```
 
 Mark as complete:
 
 ```bash
 $ devcord task 2 -c
-$ devcord task 2 --complete
+$ devcord task 2 --completed
 ```
 
 Mark as pending:
 
 ```bash
 $ devcord task 10 -pd
 $ devcord task 10 --pending
```

