# Comparing `tmp/profiling_decorator-0.0.2.tar.gz` & `tmp/profiling_decorator-0.0.3.tar.gz`

## Comparing `profiling_decorator-0.0.2.tar` & `profiling_decorator-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 profiling_decorator-0.0.2/src/profiling_decorator/__init__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 profiling_decorator-0.0.2/src/profiling_decorator/version.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 profiling_decorator-0.0.2/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 profiling_decorator-0.0.2/LICENSE
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 profiling_decorator-0.0.2/README.md
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 profiling_decorator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 profiling_decorator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 profiling_decorator-0.0.3/src/profiling_decorator/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 profiling_decorator-0.0.3/src/profiling_decorator/version.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 profiling_decorator-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiling_decorator-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 profiling_decorator-0.0.3/README.md
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 profiling_decorator-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 profiling_decorator-0.0.3/PKG-INFO
```

### Comparing `profiling_decorator-0.0.2/src/profiling_decorator/__init__.py` & `profiling_decorator-0.0.3/src/profiling_decorator/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-"""profiling decorator definition"""
-
-# pylint: disable = missing-function-docstring
-import asyncio
-import cProfile
-from functools import wraps
-import io
-import logging
-import pstats
-from pstats import SortKey
-from typing import Any, Callable, List, Optional, Union, Tuple
-
-
-VALID_SORTS = set(
-    val
-    for name, attribute in SortKey.__dict__.items()
-    if not name.startswith("__") and isinstance(attribute, tuple)
-    for val in attribute
-)
-
-
-def profile(
-    n_rows: int = 50,
-    sort_by: Union[str, List[str], Tuple] = "cumulative",
-    output: str = "stdout",
-    filename: Optional[str] = None,
-) -> Callable:
-    """
-    Decorator to profile a function.
-
-    Args:
-        n_rows: Number of rows to reduce profile output to.
-        sort_by: What statistic(s) to sort by in the results.
-        output: How to output the results.
-        filename: The filename to output to if output='file'
-
-    Returns:
-        func return
-
-    Raises:
-        ValueError: Invalid value for parameter.
-        IOError: Error writing to file.
-    """
-    valid_outputs = {"stdout", "file", "log"}
-
-    def decorator(func: Callable) -> Callable:
-
-        @wraps(func)
-        async def async_wrapper(*args: Any, **kwargs: Any) -> Any:
-            with cProfile.Profile() as pr:
-                # Directly await the async function here
-                result = await func(*args, **kwargs)
-                process_profiling_results(pr)
-
-            return result
-
-        @wraps(func)
-        def sync_wrapper(*args: Any, **kwargs: Any) -> Any:
-            with cProfile.Profile() as pr:
-                result = func(*args, **kwargs)
-                process_profiling_results(pr)
-
-            return result
-
-        if asyncio.iscoroutinefunction(func):
-            return async_wrapper
-        return sync_wrapper
-
-    def process_profiling_results(pr: cProfile.Profile) -> None:
-        s = io.StringIO()
-        # Fallback to 'cumulative' if sort_by is invalid
-        if isinstance(sort_by, (list, tuple)):
-            sort_by_valid = [s for s in sort_by if s in VALID_SORTS]
-        else:
-            sort_by_valid = [sort_by] if sort_by in VALID_SORTS else ["cumulative"]
-
-        ps = pstats.Stats(pr, stream=s).sort_stats(*sort_by_valid)
-        ps.print_stats(n_rows)
-
-        # Handle output
-        if output not in valid_outputs:
-            raise ValueError(
-                f"Invalid output option '{output}'. Valid options are {valid_outputs}."
-            )
-
-        if output == "stdout":
-            print(s.getvalue())
-        elif output == "file":
-            if not filename:
-                raise ValueError("Filename must be provided when output is 'file'.")
-            try:
-                with open(filename, "w+", encoding="utf-8") as f:
-                    f.write(s.getvalue())
-            except IOError as e:
-                raise IOError(f"Error writing to file {filename}: {e}") from e
-        elif output == "log":
-            logger = logging.getLogger(__name__)
-            logger.info(s.getvalue())
-        else:
-            raise ValueError("'output' must be one of 'stdout', 'file' or 'log'.")
-
-    # Enable the decorator to be used without parentheses if no arguments are provided
-    if callable(n_rows):
-        temp_func = n_rows
-        n_rows = 50
-        return decorator(temp_func)
-
-    return decorator
+"""profiling decorator definition"""
+
+# pylint: disable = missing-function-docstring
+import asyncio
+import cProfile
+from functools import wraps
+import io
+import logging
+import pstats
+from pstats import SortKey
+from typing import Any, Callable, List, Optional, Union, Tuple
+
+
+VALID_SORTS = set(
+    val
+    for name, attribute in SortKey.__dict__.items()
+    if not name.startswith("__") and isinstance(attribute, tuple)
+    for val in attribute
+)
+
+
+def profile(
+    n_rows: int = 50,
+    sort_by: Union[str, List[str], Tuple] = "cumulative",
+    output: str = "stdout",
+    filename: Optional[str] = None,
+) -> Callable:
+    """
+    Decorator to profile a function.
+
+    Args:
+        n_rows: Number of rows to reduce profile output to.
+        sort_by: What statistic(s) to sort by in the results.
+        output: How to output the results.
+        filename: The filename to output to if output='file'
+
+    Returns:
+        func return
+
+    Raises:
+        ValueError: Invalid value for parameter.
+        IOError: Error writing to file.
+    """
+    valid_outputs = {"stdout", "file", "log"}
+
+    def decorator(func: Callable) -> Callable:
+
+        @wraps(func)
+        async def async_wrapper(*args: Any, **kwargs: Any) -> Any:
+            with cProfile.Profile() as pr:
+                # Directly await the async function here
+                result = await func(*args, **kwargs)
+                process_profiling_results(pr)
+
+            return result
+
+        @wraps(func)
+        def sync_wrapper(*args: Any, **kwargs: Any) -> Any:
+            with cProfile.Profile() as pr:
+                result = func(*args, **kwargs)
+                process_profiling_results(pr)
+
+            return result
+
+        if asyncio.iscoroutinefunction(func):
+            return async_wrapper
+        return sync_wrapper
+
+    def process_profiling_results(pr: cProfile.Profile) -> None:
+        s = io.StringIO()
+        # Fallback to 'cumulative' if sort_by is invalid
+        if isinstance(sort_by, (list, tuple)):
+            sort_by_valid = [s for s in sort_by if s in VALID_SORTS]
+        else:
+            sort_by_valid = [sort_by] if sort_by in VALID_SORTS else ["cumulative"]
+
+        ps = pstats.Stats(pr, stream=s).sort_stats(*sort_by_valid)
+        ps.print_stats(n_rows)
+
+        # Handle output
+        if output not in valid_outputs:
+            raise ValueError(
+                f"Invalid output option '{output}'. Valid options are {valid_outputs}."
+            )
+
+        if output == "stdout":
+            print(s.getvalue())
+        elif output == "file":
+            if not filename:
+                raise ValueError("Filename must be provided when output is 'file'.")
+            try:
+                with open(filename, "w+", encoding="utf-8") as f:
+                    f.write(s.getvalue())
+            except IOError as e:
+                raise IOError(f"Error writing to file {filename}: {e}") from e
+        elif output == "log":
+            logger = logging.getLogger(__name__)
+            logger.info(s.getvalue())
+        else:
+            raise ValueError("'output' must be one of 'stdout', 'file' or 'log'.")
+
+    # Enable the decorator to be used without parentheses if no arguments are provided
+    if callable(n_rows):
+        temp_func = n_rows
+        n_rows = 50
+        return decorator(temp_func)
+
+    return decorator
```

### Comparing `profiling_decorator-0.0.2/LICENSE` & `profiling_decorator-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `profiling_decorator-0.0.2/README.md` & `profiling_decorator-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
-<a name="readme-top"></a>
-[![LinkedIn][linkedin-shield]][linkedin-url]
-<!-- PROJECT LOGO -->
-<br />
-<div align="center">
-<h1 align="center">@profile</h1>
-  <p align="center">
-    Simplifies Method Profiling
-  </p>
-</div>
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-The profile decorator is designed for easy profiling of Python functions, 
-leveraging the built-in cProfile and pstats modules for performance analysis.
-It provides a flexible way to output profiling information either to the
-standard output, logger or to a file and allows for sorting of profiling data
-based on various criteria.
-
-The decorator is designed to be a "no frills" implementation of CProfile that saves you time. Just add
-it to a method, call your endpoint or run your script, and see the output.
-
-## Features
-Features
-Seamless Integration: Just decorate functions you wish to profile without altering their implementation.
-- Flexible Output Options: Choose to print the profiling results to stdout, a logger or save them to a file for further analysis.
-- Customizable Sorting: Sort profiling results by criteria like 'cumulative time', 'number of calls', and more, to focus on the most relevant performance metrics.
-- Adjustable Detail Level: Control the amount of information displayed through optional parameters, tailoring the output to your needs.
-## Prerequisites
-
-There are no external dependancies, profiling is done using the standard library
-package `CProfile`.
-
-## Installation
-
-Install the package
-   ```sh
-   pip install profile-decorator
-   ```
-
-<!-- USAGE EXAMPLES -->
-## Usage
-
-Import the profile decorator:
-
-```python
-from profile_decorator import profile
-```
-
-#### Basic Usage
-
-Basic Usage
-To use the decorator without any customization, simply decorate your function.
-By default, it profiles the function, sorts the results by cumulative time, 
-and prints the results to standard output.
-```python
-@profile
-def example_function():
-    # Function code to profile
-    pass
-
-example_function()
-```
-
-### Limiting Output
-Limit the profiling output to a specific number of rows to focus on the top time-consuming operations.
-```python
-@profile(n_rows=10)
-def example_function():
-    # Function code to profile
-    pass
-
-example_function()
-```
-### Changing Sort Criteria
-Customize the sorting criteria of the profiling report (e.g., by number of calls).
-```python
-@profile(sort_by="calls")
-def example_function():
-    # Function code to profile
-    pass
-
-example_function()
-```
-#### Valid Sort Options
-The valid options for the sort_by parameter align with the SortKey attributes in the pstats module and include:
-
-- 'cumulative' - Total time spent in the function and all sub-functions (default).
-- 'time' - Internal time spent in the function (excluding sub-functions).
-- 'calls' - Number of calls to the function.
-- 'ncalls' - Same as calls, but distinguishes between direct and indirect calls.
-
-See the pstats module for a complete up to date list.
-
-### Output to File
-To save the profiling results to a file, specify the output and filename parameters.
-```python
-@profile(output='file', filename='profile_stats.txt')
-def example_function():
-    # Function code to profile
-    pass
-
-example_function()
-```
-#### Output Options
-- 'stdout' - Print the profiling results to standard output (default).
-- 'file' - Write the profiling results to a file. Requires specifying the filename parameter.
-- 'log' - Log the profiling results using the configured logging system. This is useful for integrating profiling results into application logs. 
-
-#### Configuring Logging
-Before using the log output option, ensure the logging system is configured to handle messages at the INFO level or lower. Here's a basic configuration example:
-```python
-import logging
-
-logging.basicConfig(level=logging.INFO)
-
-@profile(output='log')
-def example_function():
-    # Function code to profile
-    pass
-
-example_function()
-```
-### Async Support
-The profile decorator is enhanced to support profiling of both synchronous and asynchronous 
-functions. This feature allows developers to gain insights into the performance characteristics 
-of their code, whether it operates synchronously or leverages Python's asyncio for 
-asynchronous execution.
-
-Usage is identical:
-```python
-@profile
-async def async_function():
-    # Async function code to profile
-    await some_async_operation()
-
-await async_function()
-```
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-<!-- LICENSE -->
-## License
-
-Distributed under the Apache Software License. See `LICENSE.txt` for more information.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- CONTACT -->
-## Contact
-
-Joshua Brumpton - ja.brumpton@gmail.com
-
-Project Link: [github repo](https://github.com/CTPassion/profile-decorator)
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-[linkedin-url]: https://www.linkedin.com/in/joshua-brumpton-8a6bb619b/
+<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
+<a name="readme-top"></a>
+[![LinkedIn][linkedin-shield]][linkedin-url]
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+<h1 align="center">@profile</h1>
+  <p align="center">
+    Simplifies Method Profiling
+  </p>
+</div>
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+The profile decorator is designed for easy profiling of Python functions, 
+leveraging the built-in cProfile and pstats modules for performance analysis.
+It provides a flexible way to output profiling information either to the
+standard output, logger or to a file and allows for sorting of profiling data
+based on various criteria.
+
+The decorator is designed to be a "no frills" implementation of CProfile that saves you time. Just add
+it to a method, call your endpoint or run your script, and see the output.
+
+## Features
+Features
+Seamless Integration: Just decorate functions you wish to profile without altering their implementation.
+- Flexible Output Options: Choose to print the profiling results to stdout, a logger or save them to a file for further analysis.
+- Customizable Sorting: Sort profiling results by criteria like 'cumulative time', 'number of calls', and more, to focus on the most relevant performance metrics.
+- Adjustable Detail Level: Control the amount of information displayed through optional parameters, tailoring the output to your needs.
+## Prerequisites
+
+There are no external dependancies, profiling is done using the standard library
+package `CProfile`.
+
+## Installation
+
+Install the package
+   ```sh
+   pip install profile-decorator
+   ```
+
+<!-- USAGE EXAMPLES -->
+## Usage
+
+Import the profile decorator:
+
+```python
+from profile_decorator import profile
+```
+
+#### Basic Usage
+
+Basic Usage
+To use the decorator without any customization, simply decorate your function.
+By default, it profiles the function, sorts the results by cumulative time, 
+and prints the results to standard output.
+```python
+@profile
+def example_function():
+    # Function code to profile
+    pass
+
+example_function()
+```
+
+### Limiting Output
+Limit the profiling output to a specific number of rows to focus on the top time-consuming operations.
+```python
+@profile(n_rows=10)
+def example_function():
+    # Function code to profile
+    pass
+
+example_function()
+```
+### Changing Sort Criteria
+Customize the sorting criteria of the profiling report (e.g., by number of calls).
+```python
+@profile(sort_by="calls")
+def example_function():
+    # Function code to profile
+    pass
+
+example_function()
+```
+#### Valid Sort Options
+The valid options for the sort_by parameter align with the SortKey attributes in the pstats module and include:
+
+- 'cumulative' - Total time spent in the function and all sub-functions (default).
+- 'time' - Internal time spent in the function (excluding sub-functions).
+- 'calls' - Number of calls to the function.
+- 'ncalls' - Same as calls, but distinguishes between direct and indirect calls.
+
+See the pstats module for a complete up to date list.
+
+### Output to File
+To save the profiling results to a file, specify the output and filename parameters.
+```python
+@profile(output='file', filename='profile_stats.txt')
+def example_function():
+    # Function code to profile
+    pass
+
+example_function()
+```
+#### Output Options
+- 'stdout' - Print the profiling results to standard output (default).
+- 'file' - Write the profiling results to a file. Requires specifying the filename parameter.
+- 'log' - Log the profiling results using the configured logging system. This is useful for integrating profiling results into application logs. 
+
+#### Configuring Logging
+Before using the log output option, ensure the logging system is configured to handle messages at the INFO level or lower. Here's a basic configuration example:
+```python
+import logging
+
+logging.basicConfig(level=logging.INFO)
+
+@profile(output='log')
+def example_function():
+    # Function code to profile
+    pass
+
+example_function()
+```
+### Async Support
+The profile decorator is enhanced to support profiling of both synchronous and asynchronous 
+functions. This feature allows developers to gain insights into the performance characteristics 
+of their code, whether it operates synchronously or leverages Python's asyncio for 
+asynchronous execution.
+
+Usage is identical:
+```python
+@profile
+async def async_function():
+    # Async function code to profile
+    await some_async_operation()
+
+await async_function()
+```
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+<!-- LICENSE -->
+## License
+
+Distributed under the Apache Software License. See `LICENSE.txt` for more information.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- CONTACT -->
+## Contact
+
+Joshua Brumpton - ja.brumpton@gmail.com
+
+Project Link: [github repo](https://github.com/CTPassion/profile-decorator)
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-url]: https://www.linkedin.com/in/joshua-brumpton-8a6bb619b/
```

### Comparing `profiling_decorator-0.0.2/pyproject.toml` & `profiling_decorator-0.0.3/pyproject.toml`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-
-[project]
-name = "profiling_decorator"
-dynamic = ["version"]
-description = "Simplifies Python code profiling by offering an easy-to-use decorator for measuring function performance. Customize profiling with options for sort criteria and output format. Perfect for quickly identifying bottlenecks."
-readme = "README.md"
-requires-python = ">=3.8"
-authors = [{ name="Joshua Brumpton", email="ja.brumpton@gmail.com" }]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/CTPassion/profiling-decorator"
-Issues = "https://github.com/CTPassion/profiling-decorator/issues"
-
-[project.optional-dependencies]
-dev = [
-    "black"
-]
-test = [
-    "pytest",
-    "pytest-asyncio"
-]
-
-[tool.pytest.ini_options]
-minversion = "6.0"
-addopts = "-ra -q"
-testpaths = [
-    "tests"
-]
-
-[tool.coverage.run]
-source = ["src"]
-
-[tool.pylint]
-max-line-length = 88
-disable = [
-    "C0114", # (missing-module-docstring)
-    "C0115", # (missing-class-docstring)
-    "C0116", # (missing-function-docstring)
-]
-
-[tool.hatch.version]
-path = "src/profiling_decorator/version.py"
-
-[tool.hatch.build.targets.sdist]
-include = ["/src"]
-
-[tool.hatch.build.targets.wheel]
-packages = ["src/profiling_decorator"]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+
+[project]
+name = "profiling_decorator"
+dynamic = ["version"]
+description = "Simplifies Python code profiling by offering an easy-to-use decorator for measuring function performance. Customize profiling with options for sort criteria and output format. Perfect for quickly identifying bottlenecks."
+readme = "README.md"
+requires-python = ">=3.8"
+authors = [{ name="Joshua Brumpton", email="ja.brumpton@gmail.com" }]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+Homepage = "https://github.com/CTPassion/profiling-decorator"
+Issues = "https://github.com/CTPassion/profiling-decorator/issues"
+
+[project.optional-dependencies]
+dev = [
+    "black"
+]
+test = [
+    "pytest",
+    "pytest-asyncio"
+]
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra -q"
+testpaths = [
+    "tests"
+]
+
+[tool.coverage.run]
+source = ["src"]
+
+[tool.pylint]
+max-line-length = 88
+disable = [
+    "C0114", # (missing-module-docstring)
+    "C0115", # (missing-class-docstring)
+    "C0116", # (missing-function-docstring)
+]
+
+[tool.hatch.version]
+path = "src/profiling_decorator/version.py"
+
+[tool.hatch.build.targets.sdist]
+include = ["/src"]
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/profiling_decorator"]
```

### Comparing `profiling_decorator-0.0.2/PKG-INFO` & `profiling_decorator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: profiling_decorator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simplifies Python code profiling by offering an easy-to-use decorator for measuring function performance. Customize profiling with options for sort criteria and output format. Perfect for quickly identifying bottlenecks.
 Project-URL: Homepage, https://github.com/CTPassion/profiling-decorator
 Project-URL: Issues, https://github.com/CTPassion/profiling-decorator/issues
 Author-email: Joshua Brumpton <ja.brumpton@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

