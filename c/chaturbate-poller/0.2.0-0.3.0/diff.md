# Comparing `tmp/chaturbate_poller-0.2.0.tar.gz` & `tmp/chaturbate_poller-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.2.0.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.3.0.tar", max compression
```

## Comparing `chaturbate_poller-0.2.0.tar` & `chaturbate_poller-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/LICENSE
--rw-r--r--   0        0        0     2251 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/README.md
--rw-r--r--   0        0        0     3080 2024-04-04 01:21:00.383548 chaturbate_poller-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      818 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     1572 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/__main__.py
--rw-r--r--   0        0        0     2800 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      724 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     1429 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     3480 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 chaturbate_poller-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-07 16:07:26.724817 chaturbate_poller-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2251 2024-04-07 16:07:26.724817 chaturbate_poller-0.3.0/README.md
+-rw-r--r--   0        0        0     3080 2024-04-07 16:07:37.464866 chaturbate_poller-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      764 2024-04-07 16:07:26.728817 chaturbate_poller-0.3.0/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     1476 2024-04-07 16:07:26.728817 chaturbate_poller-0.3.0/src/chaturbate_poller/__main__.py
+-rw-r--r--   0        0        0     4014 2024-04-07 16:07:26.728817 chaturbate_poller-0.3.0/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0      669 2024-04-07 16:07:26.728817 chaturbate_poller-0.3.0/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     1429 2024-04-07 16:07:26.728817 chaturbate_poller-0.3.0/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     3428 2024-04-07 16:07:26.728817 chaturbate_poller-0.3.0/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.0/PKG-INFO
```

### Comparing `chaturbate_poller-0.2.0/LICENSE` & `chaturbate_poller-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.2.0/README.md` & `chaturbate_poller-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.2.0/pyproject.toml` & `chaturbate_poller-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.2.0"
+version = "0.3.0"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.2.0/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.3.0/src/chaturbate_poller/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# chaturbate_poller/src/chaturbate_poller/__init__.py
 """chaturbate_poller package."""
 
 import logging.config
 
 # Read version from installed package
 from importlib.metadata import version
```

### Comparing `chaturbate_poller-0.2.0/src/chaturbate_poller/__main__.py` & `chaturbate_poller-0.3.0/src/chaturbate_poller/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-# chaturbate_poller/src/chaturbate_poller/__main__.py
-"""Main module for the Chaturbate Poller.
-
-This module fetches Chaturbate events.
-
-"""
+"""Main module for the Chaturbate Poller."""
 
 import asyncio
 import contextlib
 import logging
 import os
 
 import httpx
```

### Comparing `chaturbate_poller-0.2.0/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.3.0/src/chaturbate_poller/chaturbate_poller.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,134 @@
-# chaturbate_poller/src/chaturbate_poller/chaturbate_poller.py
-"""Chaturbate poller."""
+"""Chaturbate poller module."""
 
 from __future__ import annotations
 
 import logging
+from types import TracebackType  # noqa: TCH003
 
 import backoff
 import httpx
 from httpx import HTTPStatusError, RequestError
 from typing_extensions import Self
 
-from .constants import API_TIMEOUT, BASE_URL, ERROR_RANGE_END, ERROR_RANGE_START
+from .constants import BASE_URL, ERROR_RANGE_END, ERROR_RANGE_START
 from .models import EventsAPIResponse
 
 logger = logging.getLogger(__name__)
 
 
 class ChaturbateClient:
-    """Client for fetching Chaturbate events."""
+    """Client for fetching Chaturbate events.
+
+    Args:
+        username: Chaturbate username.
+        token: Chaturbate token.
+        timeout: Timeout in seconds for the API request.
+
+    Attributes:
+        base_url: Base URL for the Chaturbate API.
+        timeout: Timeout in seconds for the API request.
+        username: Chaturbate username.
+        token: Chaturbate token.
+        client: HTTPX AsyncClient instance.
+    """
 
     def __init__(self, username: str, token: str, timeout: int | None = None) -> None:
-        """Initialize client."""
+        """Initialize client.
+
+        Raises:
+            ValueError: If username or token are not provided.
+        """
         if not username or not token:
-            msg = "Chaturbate username and token are required."
-            raise ValueError(msg)
+            error_msg = "Chaturbate username and token are required."
+            raise ValueError(error_msg)
         self.base_url = BASE_URL
-        self.timeout = timeout or API_TIMEOUT
+        self.timeout = timeout
         self.username = username
         self.token = token
         self.client = httpx.AsyncClient()
 
     async def __aenter__(self) -> Self:
-        """Enter client."""
-        if self.client.is_closed:
-            self.client = httpx.AsyncClient()
-            logger.debug("HTTP client re-opened.")
+        """Enter client.
+
+        Returns:
+            ChaturbateClient: Client instance.
+        """
+        self.client = httpx.AsyncClient()
         logger.debug("Client opened.")
         return self
 
-    async def __aexit__(self, exc_type, exc_value, traceback) -> None:  # noqa: ANN001
-        """Exit client."""
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
+    ) -> None:
+        """Exit client.
+
+        Args:
+            exc_type: Exception type.
+            exc_value: Exception value.
+            traceback: Traceback.
+        """
         await self.client.aclose()
-        logger.debug("Client closed.")
 
     @backoff.on_exception(
         backoff.expo,
         (HTTPStatusError, RequestError),
         max_time=20,
         giveup=lambda e: not need_retry(e),
-        on_backoff=lambda details: logger.debug(
+        on_backoff=lambda details: logger.info(
             "Backoff triggered. Retry: %s, Waiting: %s sec. before retrying.",
             details.get("tries", ""),
             int(details.get("wait", 0)),
         ),
-        on_giveup=lambda details: logger.debug(
+        on_giveup=lambda details: logger.info(
             "Retry stopped: %s after %s attempts.",
             details.get("exception", ""),
             details.get("tries", ""),
         ),
     )
     async def fetch_events(self, url: str | None = None) -> EventsAPIResponse:
-        """Fetch events."""
-        if not url:
-            url = (
-                f"{self.base_url.format(username=self.username, token=self.token)}?timeout={self.timeout}"  # noqa: E501
-                if self.timeout
-                else self.base_url.format(username=self.username, token=self.token)
-            )
-        logger.debug("Fetching events from %s", url)
+        """Fetch events from the Chaturbate API.
+
+        Args:
+            url: URL to fetch events from.
+
+        Returns:
+            EventsAPIResponse: Response from the API.
 
-        response = await self.client.get(url, timeout=None)
+        Raises:
+            HTTPStatusError: If the response status code is in the error range.
+            RequestError: If an error occurs during the request.
+        """
+        if url is None:
+            url = self._construct_url()
+        response = await self.client.get(url, timeout=self.timeout)
         response.raise_for_status()
         return EventsAPIResponse.model_validate(response.json())
 
+    def _construct_url(self) -> str:
+        """Construct URL with username, token, and timeout.
+
+        Returns:
+            str: Constructed URL.
+        """
+        base_url = self.base_url.format(username=self.username, token=self.token)
+        if self.timeout:
+            return f"{base_url}?timeout={self.timeout}"
+        return base_url
+
 
 def need_retry(exception: Exception) -> bool:
-    """Retries requests on 500 series errors."""
-    return (
-        isinstance(exception, HTTPStatusError)
-        and ERROR_RANGE_START <= exception.response.status_code < ERROR_RANGE_END
-    )
+    """Retries requests on 500 series errors.
+
+    Args:
+        exception: Exception raised by the request.
+
+    Returns:
+        bool: True if the request should be retried, False otherwise.
+    """
+    if isinstance(exception, HTTPStatusError):
+        status_code = exception.response.status_code
+        return ERROR_RANGE_START <= status_code < ERROR_RANGE_END
+    return False
```

### Comparing `chaturbate_poller-0.2.0/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.3.0/src/chaturbate_poller/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# chaturbate_poller/src/chaturbate_poller/constants.py
 """Constants for the chaturbate_poller module."""
 
 BASE_URL = "https://events.testbed.cb.dev/events/{username}/{token}/"
 """str: The base URL for fetching Chaturbate events."""
 
 ERROR_RANGE_START = 500
 """int: Start of the range of HTTP status codes that are considered errors."""
```

### Comparing `chaturbate_poller-0.2.0/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.3.0/src/chaturbate_poller/logging_config.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.2.0/src/chaturbate_poller/models.py` & `chaturbate_poller-0.3.0/src/chaturbate_poller/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# chaturbate_poller/src/chaturbate_poller/models.py
 """Pydantic models for the Chaturbate Events API."""
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Field
```

### Comparing `chaturbate_poller-0.2.0/PKG-INFO` & `chaturbate_poller-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.2.0
+Version: 0.3.0
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

