# Comparing `tmp/easyoutput-0.0.8.1.tar.gz` & `tmp/easyoutput-0.0.9.tar.gz`

## Comparing `easyoutput-0.0.8.1.tar` & `easyoutput-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/README.MD
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/.github/ISSUE_TEMPLATE/🐞-bug-report.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/.github/ISSUE_TEMPLATE/🚀feature-request.md
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/src/EasyOutput/EasyOutput.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/src/EasyOutput/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/tests/test.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/LICENSE
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 easyoutput-0.0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 easyoutput-0.0.9/README.MD
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.0.9/.github/ISSUE_TEMPLATE/🐞-bug-report.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.0.9/.github/ISSUE_TEMPLATE/🚀feature-request.md
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 easyoutput-0.0.9/img/EasyOutputSmallLogo.png
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 easyoutput-0.0.9/src/EasyOutput/EasyOutput.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 easyoutput-0.0.9/src/EasyOutput/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyoutput-0.0.9/tests/test.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 easyoutput-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 easyoutput-0.0.9/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 easyoutput-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 easyoutput-0.0.9/PKG-INFO
```

### Comparing `easyoutput-0.0.8.1/README.MD` & `easyoutput-0.0.9/README.MD`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&color=55%2C%20117%2C%20169)
 
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)
 
 ![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
-## ChangeLog 📝
-
 <details>
-<summary>Alpha</summary>
+<summary>Change-Log 📝</summary>
 
 [comment]: <> (v0.0.1)
 <details>
 <summary>v0.0.1</summary>
 
     ADDED
     - Success Message
@@ -111,40 +109,48 @@
 <details>
 <summary>v0.0.8.1</summary>
 
     FIXED
     - Leaving all functions at the bottom of the file... IM SORRY
 </details>
 
+[comment]: <> (v0.0.9)
+<details>
+<summary>v0.0.9</summary>
+
+    FIXED
+    - Optioanl Highlight!
+</details>
+
 </details>
 
 # Information
 **EasyOutput** consists of easy colored print options without the hassle of doing
 ```py
-# You can now highlight your message aswell! 
-Success_Message("New Highlight!", highlight=True)
-
-# Or keep it og 😄
-Success_Message("No Highlight!")
-# Same as
-Success_Message("No Highlight!", highlight=False)
-```
-In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing
-```py
 from colorama import Fore, Style
 
 def Success(message):
     print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
 
 # and calling it like so
 
 Success("Your Success Message")
 
+
+# You can now highlight your message aswell! 
+Success_Message("New Highlight!", highlight=True)
+
+# Or keep it og 😄
+Success_Message("No Highlight!")
+# Same as
+Success_Message("No Highlight!", highlight=False)
 ```
 
+In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing
+
 If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!\
 Feel free to use this in any way you like, all I ask is that you show me your project when finished! 😄
 
 [Request a feature](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)\
 [Report an issue](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)
 
 **Updating as much as I can!**
```

### Comparing `easyoutput-0.0.8.1/.github/ISSUE_TEMPLATE/🚀feature-request.md` & `easyoutput-0.0.9/.github/ISSUE_TEMPLATE/🚀feature-request.md`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.8.1/src/EasyOutput/EasyOutput.py` & `easyoutput-0.0.9/src/EasyOutput/EasyOutput.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,126 +3,127 @@
 
 import colorama
 
 reset = Style.RESET_ALL
 brighten = Style.BRIGHT
 dim = Style.DIM
 
-def Info_Message(message, highlight: Optional[bool]):
+def Info_Message(message, highlight: bool = False):  
     """
     Prints a message notifying the user of specific need to know information.
     
     Color: Blue
     
     Highlight: Blue
     """
 
     if highlight == True:
         print(f"{Fore.BLUE + brighten}Info{reset}: {bg.BLUE + message + reset}")
-        
     elif highlight == False:    
         print(f"{Fore.BLUE + brighten}Info{reset}: {message}")
     
-def Error_Message(message, highlight: Optional[bool]):
+def Error_Message(message, highlight: bool = False):
     """
     Prints a message notifying the user of an error.
     
     Color: Red
     
     Highlight: Red
     """
     if highlight == True:
         print(f"{Fore.RED}Error{reset}: {bg.RED + message + reset}")
     elif highlight == False:
         print(f"{Fore.RED}Error{reset}: {Fore.YELLOW + message + reset}")
     
-def Connection_Error_Message(message, highlight: Optional[bool]):
+def Connection_Error_Message(message, highlight: bool = False):
     """
     Prints a message notifying the user of a connection error.
     
     Color: Red
     
     Highlight: Red
     """
     if highlight == True:
         print(f"{Fore.RED}Connection Error{reset}: {bg.RED + message + reset}")
         
     elif highlight == False:    
         print(f"{Fore.RED}Connection Error{reset}: {Fore.YELLOW + message + reset}")
     
-def Success_Message(message, highlight: Optional[bool]):
+def Success_Message(message, highlight: bool = False):
     """
     Prints a message notifying the user of a success.
     
     Color: Bright Green
     
     Highlight: Green
     """
     if highlight == True:
         print(f"{Fore.GREEN + brighten}Success{reset}: {bg.GREEN + message + reset}")
     elif highlight == False:
         print(f"{Fore.GREEN + brighten}Success{reset}: {message}")
     
-def Successful_Connection_Message(message, highlight: Optional[bool]):
+def Successful_Connection_Message(message, highlight: bool = False):
     """
     Prints a message notifying the user of a successful connection.
     
     Color: Bright Green
     
     Highlight: Green
     """
     if highlight == True:
         print(f"{Fore.GREEN + brighten}Successful Connection{reset}: {bg.GREEN + message + reset}")
     elif highlight == False:
         print(f"{Fore.GREEN + brighten}Successful Connection{reset}: {message}")
     
-def Note_Message(message, highlight: Optional[bool]):
+def Note_Message(message, highlight: bool = False):
     """
     Prints a note notifying the user of something they should be made aware of.
     
     Color: Yellow
     
     Highlight: Yellow
     """
     if highlight == True:
         print(f"{Fore.YELLOW}Note{reset}: {bg.YELLOW + message + reset}")
     elif highlight == False:    
         print(f"{Fore.YELLOW}Note{reset}: {message}")
     
-def Warning_Message(message, highlight: Optional[bool]):
+def Warning_Message(message, highlight: bool = False):
     """
     Prints a warning message for the user indicating your code is running.
     
     Color: Yellow
     
     Highlight: Yellow
     """
     if highlight == True:
         print(f"{Fore.YELLOW}Warning{reset}: {bg.YELLOW + message + reset}")    
     elif highlight == False:
         print(f"{Fore.YELLOW}Warning{reset}: {message}")
     
-def Title_Print(title, highlight: Optional[bool]):
+def Title_Print(title, highlight: bool = False):
     """
     Prints a title for grouping lists and anything else you can think of.
     
     Color: Bright Green
     
     Highlight: Green
     """
     if highlight == True:
         print(f"=== {bg.GREEN + brighten + title + reset} ===")    
     elif highlight == False:
         print(f"=== {Fore.GREEN + brighten + title + reset} ===")
      
-def Redacted_Message(message, highlight: Optional[bool]):
+def Redacted_Message(message, highlight: bool = False):
     """
     Prints redacted message 
     
     Color: Bright Green
     
     Highlight: Red
     """
     if highlight == True:
         print(f"{Fore.RED + brighten}REDACTED{reset}: {bg.RED + message + reset}")    
     elif highlight == False:
         print(f"{Fore.RED + brighten}REDACTED{reset}: {message}")
+        
+Info_Message("Test")
```

### Comparing `easyoutput-0.0.8.1/LICENSE` & `easyoutput-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.8.1/README.md` & `easyoutput-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&color=55%2C%20117%2C%20169)
 
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)
 
 ![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
-## ChangeLog 📝
-
 <details>
-<summary>Alpha</summary>
+<summary>Change-Log 📝</summary>
 
 [comment]: <> (v0.0.1)
 <details>
 <summary>v0.0.1</summary>
 
     ADDED
     - Success Message
@@ -111,40 +109,48 @@
 <details>
 <summary>v0.0.8.1</summary>
 
     FIXED
     - Leaving all functions at the bottom of the file... IM SORRY
 </details>
 
+[comment]: <> (v0.0.9)
+<details>
+<summary>v0.0.9</summary>
+
+    FIXED
+    - Optioanl Highlight!
+</details>
+
 </details>
 
 # Information
 **EasyOutput** consists of easy colored print options without the hassle of doing
 ```py
-# You can now highlight your message aswell! 
-Success_Message("New Highlight!", highlight=True)
-
-# Or keep it og 😄
-Success_Message("No Highlight!")
-# Same as
-Success_Message("No Highlight!", highlight=False)
-```
-In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing
-```py
 from colorama import Fore, Style
 
 def Success(message):
     print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
 
 # and calling it like so
 
 Success("Your Success Message")
 
+
+# You can now highlight your message aswell! 
+Success_Message("New Highlight!", highlight=True)
+
+# Or keep it og 😄
+Success_Message("No Highlight!")
+# Same as
+Success_Message("No Highlight!", highlight=False)
 ```
 
+In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing
+
 If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!\
 Feel free to use this in any way you like, all I ask is that you show me your project when finished! 😄
 
 [Request a feature](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)\
 [Report an issue](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)
 
 **Updating as much as I can!**
```

### Comparing `easyoutput-0.0.8.1/pyproject.toml` & `easyoutput-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EasyOutput"
-version = "0.0.8.1"
+version = "0.0.9"
 authors = [
   { name="FrankAustin", email="frankaustindev808@gmail.com" },
 ]
 description = "Colored messages in the palm of your hand"
 readme = "README.md"
+license = {file = "LICENSE.txt"}
+keywords = [
+  "Error Message", "Success Message", "Warning Message", "Easy"
+]
+maintainers = [
+  {name = "FrankAustin", email="frankaustindev808@gmail.com"}
+]
 requires-python = ">=3.12"
-install_requires=['colorama']
+install_requires= ['colorama']
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Operating System :: Unix",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
 ]
+dependencies = [
+  "colorama"
+]
+
 
 [project.urls]
-Homepage = "https://github.com/FrankAustin808/EasyOut/"
-Issues = "https://github.com/FrankAustin808/EasyOut/issues/new/choose"
+"Homepage" = "https://github.com/FrankAustin808/EasyOut/"
+"Issues" = "https://github.com/FrankAustin808/EasyOut/issues/new/choose"
+"Feature Request" = "https://github.com/FrankAustin808/EasyOut/issues/new/choose"
```

