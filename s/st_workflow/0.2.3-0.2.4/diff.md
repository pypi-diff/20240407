# Comparing `tmp/st_workflow-0.2.3.tar.gz` & `tmp/st_workflow-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_workflow-0.2.3.tar", max compression
+gzip compressed data, was "st_workflow-0.2.4.tar", max compression
```

## Comparing `st_workflow-0.2.3.tar` & `st_workflow-0.2.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    17491 2024-02-03 14:36:59.062198 st_workflow-0.2.3/README.md
--rw-r--r--   0        0        0      457 2024-04-06 19:17:20.859484 st_workflow-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7250 2024-04-06 19:05:38.199522 st_workflow-0.2.3/st_workflow/__init__.py
--rw-r--r--   0        0        0    18149 1970-01-01 00:00:00.000000 st_workflow-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    18209 2024-04-07 03:54:39.961861 st_workflow-0.2.4/README.md
+-rw-r--r--   0        0        0      457 2024-04-07 03:56:52.171856 st_workflow-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7250 2024-04-07 03:50:47.961878 st_workflow-0.2.4/st_workflow/__init__.py
+-rw-r--r--   0        0        0    18867 1970-01-01 00:00:00.000000 st_workflow-0.2.4/PKG-INFO
```

### Comparing `st_workflow-0.2.3/README.md` & `st_workflow-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,32 +24,49 @@
 
 Use `asyncio.run` to execute the workflow:
 
 ```python
 import asyncio
 from st_workflow import Workflow, Scope
 
-# Define your steps
-async def step1(ctx):
-    # Your code here
-    pass
-
-async def error_step(ctx):
-    # Your code here
-    pass
-
-# Create a workflow with a context
-wf = Workflow(ctx={'initial_data': 'data_value'})
-
-# Add steps to the workflow
-wf.add_step(step1)
-wf.add_error_step(error_step)
-
-# Run the workflow using asyncio.run
-asyncio.run(wf.run())
+# Simulate an asynchronous API call
+async def fetch_data(ctx):
+    print("Fetching data...")
+    await asyncio.sleep(1)  # Simulates the API call delay
+    ctx["fetched_data"] = "Data from API"
+
+# Process the fetched data
+async def process_data(data):
+    print(f"Processing data: {data}")
+    await asyncio.sleep(1)  # Simulate processing delay
+    # Imagine a condition where processing could fail
+    if not data:
+        raise ValueError("No data to process")
+    ctx["processed_data"] = data.upper()
+
+# An example error handling step
+async def handle_error(ctx):
+    error_info = ctx.get(f'{Scope.NORMAL.value}_error', {})
+    print(f"Handling error from step {error_info.get('step')}: {error_info.get('error')}")
+
+# Define the workflow
+async def main():
+    wf = Workflow(ctx={})
+    
+    # Adding steps and an error handler to the workflow
+    wf.add_step(fetch_data, name="data")
+    wf.add_step(process_data)
+    wf.add_error_step(handle_error)
+
+    # Execute the workflow
+    await wf.run()
+
+# Run the workflow
+if __name__ == "__main__":
+    asyncio.run(main())
 ```
 
 ## Detailed Usage
 
 ### Enums
 
 - `Scope`: Determines the scope of a step. Available values:
```

### Comparing `st_workflow-0.2.3/st_workflow/__init__.py` & `st_workflow-0.2.4/st_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `st_workflow-0.2.3/PKG-INFO` & `st_workflow-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_workflow
-Version: 0.2.3
+Version: 0.2.4
 Summary: Library for creating complex workflows in Python
 Home-page: https://github.com/safari12/st_workflow
 License: MIT
 Author: Reza Safari
 Author-email: rsafari.s@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -42,32 +42,49 @@
 
 Use `asyncio.run` to execute the workflow:
 
 ```python
 import asyncio
 from st_workflow import Workflow, Scope
 
-# Define your steps
-async def step1(ctx):
-    # Your code here
-    pass
-
-async def error_step(ctx):
-    # Your code here
-    pass
-
-# Create a workflow with a context
-wf = Workflow(ctx={'initial_data': 'data_value'})
-
-# Add steps to the workflow
-wf.add_step(step1)
-wf.add_error_step(error_step)
-
-# Run the workflow using asyncio.run
-asyncio.run(wf.run())
+# Simulate an asynchronous API call
+async def fetch_data(ctx):
+    print("Fetching data...")
+    await asyncio.sleep(1)  # Simulates the API call delay
+    ctx["fetched_data"] = "Data from API"
+
+# Process the fetched data
+async def process_data(data):
+    print(f"Processing data: {data}")
+    await asyncio.sleep(1)  # Simulate processing delay
+    # Imagine a condition where processing could fail
+    if not data:
+        raise ValueError("No data to process")
+    ctx["processed_data"] = data.upper()
+
+# An example error handling step
+async def handle_error(ctx):
+    error_info = ctx.get(f'{Scope.NORMAL.value}_error', {})
+    print(f"Handling error from step {error_info.get('step')}: {error_info.get('error')}")
+
+# Define the workflow
+async def main():
+    wf = Workflow(ctx={})
+    
+    # Adding steps and an error handler to the workflow
+    wf.add_step(fetch_data, name="data")
+    wf.add_step(process_data)
+    wf.add_error_step(handle_error)
+
+    # Execute the workflow
+    await wf.run()
+
+# Run the workflow
+if __name__ == "__main__":
+    asyncio.run(main())
 ```
 
 ## Detailed Usage
 
 ### Enums
 
 - `Scope`: Determines the scope of a step. Available values:
```

