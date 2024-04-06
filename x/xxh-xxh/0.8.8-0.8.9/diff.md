# Comparing `tmp/xxh-xxh-0.8.8.tar.gz` & `tmp/xxh-xxh-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxh-xxh-0.8.8.tar", last modified: Sun Dec 19 21:39:57 2021, max compression
+gzip compressed data, was "xxh-xxh-0.8.9.tar", last modified: Sun Feb 13 10:21:48 2022, max compression
```

## Comparing `xxh-xxh-0.8.8.tar` & `xxh-xxh-0.8.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 21:39:57.115692 xxh-xxh-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    17857 2021-12-19 21:39:57.115692 xxh-xxh-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17048 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-19 21:39:57.115692 xxh-xxh-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 21:39:57.115692 xxh-xxh-0.8.8/xxh/
--rwxr-xr-x   0 runner    (1001) docker     (121)      296 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/xxh/xxh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 21:39:57.115692 xxh-xxh-0.8.8/xxh/xxh_xxh/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/xxh/xxh_xxh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/xxh/xxh_xxh/config.xxhc
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/xxh/xxh_xxh/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/xxh/xxh_xxh/xxh.bash
--rw-r--r--   0 runner    (1001) docker     (121)    55052 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/xxh/xxh_xxh/xxh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/xxh/xxh_xxh/xxh.xsh
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-12-19 21:39:45.000000 xxh-xxh-0.8.8/xxh/xxh_xxh/xxh.zsh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 21:39:57.115692 xxh-xxh-0.8.8/xxh_xxh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17857 2021-12-19 21:39:56.000000 xxh-xxh-0.8.8/xxh_xxh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      349 2021-12-19 21:39:57.000000 xxh-xxh-0.8.8/xxh_xxh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-19 21:39:56.000000 xxh-xxh-0.8.8/xxh_xxh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-19 21:39:56.000000 xxh-xxh-0.8.8/xxh_xxh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-12-19 21:39:56.000000 xxh-xxh-0.8.8/xxh_xxh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 10:21:48.223040 xxh-xxh-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    18000 2022-02-13 10:21:48.223040 xxh-xxh-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17191 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-13 10:21:48.223040 xxh-xxh-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 10:21:48.219040 xxh-xxh-0.8.9/xxh/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      296 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/xxh/xxh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 10:21:48.219040 xxh-xxh-0.8.9/xxh/xxh_xxh/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/xxh/xxh_xxh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/xxh/xxh_xxh/config.xxhc
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/xxh/xxh_xxh/shell.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/xxh/xxh_xxh/xxh.bash
+-rw-r--r--   0 runner    (1001) docker     (121)    55052 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/xxh/xxh_xxh/xxh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/xxh/xxh_xxh/xxh.xsh
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-02-13 10:21:37.000000 xxh-xxh-0.8.9/xxh/xxh_xxh/xxh.zsh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 10:21:48.223040 xxh-xxh-0.8.9/xxh_xxh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    18000 2022-02-13 10:21:47.000000 xxh-xxh-0.8.9/xxh_xxh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-02-13 10:21:48.000000 xxh-xxh-0.8.9/xxh_xxh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 10:21:47.000000 xxh-xxh-0.8.9/xxh_xxh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-13 10:21:47.000000 xxh-xxh-0.8.9/xxh_xxh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-13 10:21:47.000000 xxh-xxh-0.8.9/xxh_xxh.egg-info/top_level.txt
```

### Comparing `xxh-xxh-0.8.8/LICENSE` & `xxh-xxh-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xxh-xxh-0.8.8/PKG-INFO` & `xxh-xxh-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xxh-xxh
-Version: 0.8.8
+Version: 0.8.9
 Summary: Bring your favorite shell wherever you go through the ssh
 Home-page: https://github.com/xxh/xxh
 Author: xxh
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/xxh/xxh/blob/master/README.md
 Project-URL: Code, https://github.com/xxh/xxh
@@ -105,15 +105,15 @@
 | **[elvish](https://github.com/krageon/xxh-shell-elvish)**   | alpha      |             | | |
 
 [Search xxh shell on Github](https://github.com/search?q=xxh-shell&type=Repositories) or [Bitbucket](https://bitbucket.org/repo/all?name=xxh-shell) or [create your shell entrypoint](https://github.com/xxh/xxh-shell-example) to use another portable shell.  
 
 ### Prerun plugins
 [Prerun plugins](https://github.com/xxh/xxh/wiki#plugins) allow you to bring any portable tools, dotfiles or aliases to xxh session before running shell. 
 
-Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **[xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-plugin-prerun-zoxide)**. There is [cookiecutter template to create prerun plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun).
+Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **[xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-plugin-prerun-zoxide)**, **[starship](https://github.com/izissise/xxh-plugin-prerun-starship)**. There is [cookiecutter template to create prerun plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun).
 
 ## Usage
 Use `xxh` instead of `ssh` when connecting to Linux hosts without changing ssh arguments:
 ```
 xxh <host from ~/.ssh/config>
 xxh [ssh arguments] [user@]host[:port] [xxh arguments]
 xxh local [xxh arguments]
@@ -129,16 +129,16 @@
 xxh anyhost +if +q                                # Force reinstall xxh on the host in quiet mode
 xxh anyhost +hh /tmp/xxh +hhr                     # Upload xxh to /tmp/xxh and remove when disconnecting
 source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh  # Connect in seamless mode with ohmyzsh plugin
 xxh local +s xonsh                                # Experimental: build xxh environment inplace and without ssh
 ```
 For reusing arguments and simplifying xxh usage (like shortening to `xxh anyhost`) there is a [config file](https://github.com/xxh/xxh/wiki#config-file).
 
-**Why the plus sign for the xxh arguments?** The xxh is using the plus sign for the xxh arguments to save the ability to use minus sign for the original ssh arguments. This allows just replace the first two letters in the `ssh` command to convert it to the `xxh` command.
-
+**Why the plus sign for the xxh arguments?** The xxh is using the plus sign for the xxh arguments to save the ability to use the minus sign for the original ssh arguments. This allows just replace the first two letters in the `ssh` command to convert it to the `xxh` command. Also see the [discussion](https://github.com/xxh/xxh/issues/129).
+ 
 ### Installing xxh packages
 ```bash
 xxh [+I xxh-package +I ...] [+L] [+RI xxh-package +RI ...] [+R xxh-package +R ...]
 ```
 Different ways to set the xxh package source:
 ```yaml
 xxh +I xxh-shell-example                                         # install from https://github.com/xxh
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xxh-xxh Version: 0.8.8 Summary: Bring your favorite
+Metadata-Version: 2.1 Name: xxh-xxh Version: 0.8.9 Summary: Bring your favorite
 shell wherever you go through the ssh Home-page: https://github.com/xxh/xxh
 Author: xxh Author-email: author@example.com License: BSD Project-URL:
 Documentation, https://github.com/xxh/xxh/blob/master/README.md Project-URL:
 Code, https://github.com/xxh/xxh Project-URL: Issue tracker, https://
 github.com/xxh/xxh/issues Platform: Unix-like Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Unix Shell Classifier: Topic
 :: System :: Shells Classifier: Topic :: System :: System Shells Classifier:
@@ -83,36 +83,38 @@
 bring any portable tools, dotfiles or aliases to xxh session before running
 shell. Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-
 core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-
 prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-
 docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **
 [xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://
 github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-
-plugin-prerun-zoxide)**. There is [cookiecutter template to create prerun
-plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun). ## Usage Use
-`xxh` instead of `ssh` when connecting to Linux hosts without changing ssh
-arguments: ``` xxh xxh [ssh arguments] [user@]host[:port] [xxh arguments] xxh
-local [xxh arguments] ``` Common examples (use `xxh --help` to get info about
-arguments): ```yaml xxh anyhost # Connect to the host xxh -i id_rsa -p 2222
-anyhost # Using ssh arguments: port and key xxh anyhost +s zsh +i # Set the
-shell and install it without yes/no question xxh anyhost +s xonsh +hhh "~" #
-Set /home/user as home directory (read Q&A) xxh anyhost +s bash +I xxh-plugin-
-bash-vim # Preinstall a plugin xxh anyhost +if +q # Force reinstall xxh on the
-host in quiet mode xxh anyhost +hh /tmp/xxh +hhr # Upload xxh to /tmp/xxh and
-remove when disconnecting source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh #
-Connect in seamless mode with ohmyzsh plugin xxh local +s xonsh # Experimental:
-build xxh environment inplace and without ssh ``` For reusing arguments and
+plugin-prerun-zoxide)**, **[starship](https://github.com/izissise/xxh-plugin-
+prerun-starship)**. There is [cookiecutter template to create prerun plugin]
+(https://github.com/xxh/cookiecutter-xxh-plugin-prerun). ## Usage Use `xxh`
+instead of `ssh` when connecting to Linux hosts without changing ssh arguments:
+``` xxh xxh [ssh arguments] [user@]host[:port] [xxh arguments] xxh local [xxh
+arguments] ``` Common examples (use `xxh --help` to get info about arguments):
+```yaml xxh anyhost # Connect to the host xxh -i id_rsa -p 2222 anyhost # Using
+ssh arguments: port and key xxh anyhost +s zsh +i # Set the shell and install
+it without yes/no question xxh anyhost +s xonsh +hhh "~" # Set /home/user as
+home directory (read Q&A) xxh anyhost +s bash +I xxh-plugin-bash-vim #
+Preinstall a plugin xxh anyhost +if +q # Force reinstall xxh on the host in
+quiet mode xxh anyhost +hh /tmp/xxh +hhr # Upload xxh to /tmp/xxh and remove
+when disconnecting source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh # Connect
+in seamless mode with ohmyzsh plugin xxh local +s xonsh # Experimental: build
+xxh environment inplace and without ssh ``` For reusing arguments and
 simplifying xxh usage (like shortening to `xxh anyhost`) there is a [config
 file](https://github.com/xxh/xxh/wiki#config-file). **Why the plus sign for the
 xxh arguments?** The xxh is using the plus sign for the xxh arguments to save
-the ability to use minus sign for the original ssh arguments. This allows just
-replace the first two letters in the `ssh` command to convert it to the `xxh`
-command. ### Installing xxh packages ```bash xxh [+I xxh-package +I ...] [+L]
-[+RI xxh-package +RI ...] [+R xxh-package +R ...] ``` Different ways to set the
-xxh package source: ```yaml xxh +I xxh-shell-example # install from https://
+the ability to use the minus sign for the original ssh arguments. This allows
+just replace the first two letters in the `ssh` command to convert it to the
+`xxh` command. Also see the [discussion](https://github.com/xxh/xxh/issues/
+129). ### Installing xxh packages ```bash xxh [+I xxh-package +I ...] [+L] [+RI
+xxh-package +RI ...] [+R xxh-package +R ...] ``` Different ways to set the xxh
+package source: ```yaml xxh +I xxh-shell-example # install from https://
 github.com/xxh xxh +I https://github.com/xxh/xxh-shell-example # short url for
 github only, for other sources use examples below or add support xxh +I https:/
 /github.com/xxh/xxh-shell-example/tree/mybranch # short url for github only,
 for other sources use examples below or add support xxh +I xxh-shell-
 example+git+https://github.com/xxh/xxh-shell-example # long url for any git
 repo xxh +I xxh-shell-example+git+https://github.com/xxh/xxh-shell-example/
 tree/mybranch # github only branch support xxh +I xxh-shell-
```

### Comparing `xxh-xxh-0.8.8/README.md` & `xxh-xxh-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 | **[elvish](https://github.com/krageon/xxh-shell-elvish)**   | alpha      |             | | |
 
 [Search xxh shell on Github](https://github.com/search?q=xxh-shell&type=Repositories) or [Bitbucket](https://bitbucket.org/repo/all?name=xxh-shell) or [create your shell entrypoint](https://github.com/xxh/xxh-shell-example) to use another portable shell.  
 
 ### Prerun plugins
 [Prerun plugins](https://github.com/xxh/xxh/wiki#plugins) allow you to bring any portable tools, dotfiles or aliases to xxh session before running shell. 
 
-Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **[xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-plugin-prerun-zoxide)**. There is [cookiecutter template to create prerun plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun).
+Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **[xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-plugin-prerun-zoxide)**, **[starship](https://github.com/izissise/xxh-plugin-prerun-starship)**. There is [cookiecutter template to create prerun plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun).
 
 ## Usage
 Use `xxh` instead of `ssh` when connecting to Linux hosts without changing ssh arguments:
 ```
 xxh <host from ~/.ssh/config>
 xxh [ssh arguments] [user@]host[:port] [xxh arguments]
 xxh local [xxh arguments]
@@ -106,16 +106,16 @@
 xxh anyhost +if +q                                # Force reinstall xxh on the host in quiet mode
 xxh anyhost +hh /tmp/xxh +hhr                     # Upload xxh to /tmp/xxh and remove when disconnecting
 source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh  # Connect in seamless mode with ohmyzsh plugin
 xxh local +s xonsh                                # Experimental: build xxh environment inplace and without ssh
 ```
 For reusing arguments and simplifying xxh usage (like shortening to `xxh anyhost`) there is a [config file](https://github.com/xxh/xxh/wiki#config-file).
 
-**Why the plus sign for the xxh arguments?** The xxh is using the plus sign for the xxh arguments to save the ability to use minus sign for the original ssh arguments. This allows just replace the first two letters in the `ssh` command to convert it to the `xxh` command.
-
+**Why the plus sign for the xxh arguments?** The xxh is using the plus sign for the xxh arguments to save the ability to use the minus sign for the original ssh arguments. This allows just replace the first two letters in the `ssh` command to convert it to the `xxh` command. Also see the [discussion](https://github.com/xxh/xxh/issues/129).
+ 
 ### Installing xxh packages
 ```bash
 xxh [+I xxh-package +I ...] [+L] [+RI xxh-package +RI ...] [+R xxh-package +R ...]
 ```
 Different ways to set the xxh package source:
 ```yaml
 xxh +I xxh-shell-example                                         # install from https://github.com/xxh
```

#### html2text {}

```diff
@@ -72,36 +72,38 @@
 bring any portable tools, dotfiles or aliases to xxh session before running
 shell. Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-
 core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-
 prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-
 docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **
 [xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://
 github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-
-plugin-prerun-zoxide)**. There is [cookiecutter template to create prerun
-plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun). ## Usage Use
-`xxh` instead of `ssh` when connecting to Linux hosts without changing ssh
-arguments: ``` xxh xxh [ssh arguments] [user@]host[:port] [xxh arguments] xxh
-local [xxh arguments] ``` Common examples (use `xxh --help` to get info about
-arguments): ```yaml xxh anyhost # Connect to the host xxh -i id_rsa -p 2222
-anyhost # Using ssh arguments: port and key xxh anyhost +s zsh +i # Set the
-shell and install it without yes/no question xxh anyhost +s xonsh +hhh "~" #
-Set /home/user as home directory (read Q&A) xxh anyhost +s bash +I xxh-plugin-
-bash-vim # Preinstall a plugin xxh anyhost +if +q # Force reinstall xxh on the
-host in quiet mode xxh anyhost +hh /tmp/xxh +hhr # Upload xxh to /tmp/xxh and
-remove when disconnecting source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh #
-Connect in seamless mode with ohmyzsh plugin xxh local +s xonsh # Experimental:
-build xxh environment inplace and without ssh ``` For reusing arguments and
+plugin-prerun-zoxide)**, **[starship](https://github.com/izissise/xxh-plugin-
+prerun-starship)**. There is [cookiecutter template to create prerun plugin]
+(https://github.com/xxh/cookiecutter-xxh-plugin-prerun). ## Usage Use `xxh`
+instead of `ssh` when connecting to Linux hosts without changing ssh arguments:
+``` xxh xxh [ssh arguments] [user@]host[:port] [xxh arguments] xxh local [xxh
+arguments] ``` Common examples (use `xxh --help` to get info about arguments):
+```yaml xxh anyhost # Connect to the host xxh -i id_rsa -p 2222 anyhost # Using
+ssh arguments: port and key xxh anyhost +s zsh +i # Set the shell and install
+it without yes/no question xxh anyhost +s xonsh +hhh "~" # Set /home/user as
+home directory (read Q&A) xxh anyhost +s bash +I xxh-plugin-bash-vim #
+Preinstall a plugin xxh anyhost +if +q # Force reinstall xxh on the host in
+quiet mode xxh anyhost +hh /tmp/xxh +hhr # Upload xxh to /tmp/xxh and remove
+when disconnecting source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh # Connect
+in seamless mode with ohmyzsh plugin xxh local +s xonsh # Experimental: build
+xxh environment inplace and without ssh ``` For reusing arguments and
 simplifying xxh usage (like shortening to `xxh anyhost`) there is a [config
 file](https://github.com/xxh/xxh/wiki#config-file). **Why the plus sign for the
 xxh arguments?** The xxh is using the plus sign for the xxh arguments to save
-the ability to use minus sign for the original ssh arguments. This allows just
-replace the first two letters in the `ssh` command to convert it to the `xxh`
-command. ### Installing xxh packages ```bash xxh [+I xxh-package +I ...] [+L]
-[+RI xxh-package +RI ...] [+R xxh-package +R ...] ``` Different ways to set the
-xxh package source: ```yaml xxh +I xxh-shell-example # install from https://
+the ability to use the minus sign for the original ssh arguments. This allows
+just replace the first two letters in the `ssh` command to convert it to the
+`xxh` command. Also see the [discussion](https://github.com/xxh/xxh/issues/
+129). ### Installing xxh packages ```bash xxh [+I xxh-package +I ...] [+L] [+RI
+xxh-package +RI ...] [+R xxh-package +R ...] ``` Different ways to set the xxh
+package source: ```yaml xxh +I xxh-shell-example # install from https://
 github.com/xxh xxh +I https://github.com/xxh/xxh-shell-example # short url for
 github only, for other sources use examples below or add support xxh +I https:/
 /github.com/xxh/xxh-shell-example/tree/mybranch # short url for github only,
 for other sources use examples below or add support xxh +I xxh-shell-
 example+git+https://github.com/xxh/xxh-shell-example # long url for any git
 repo xxh +I xxh-shell-example+git+https://github.com/xxh/xxh-shell-example/
 tree/mybranch # github only branch support xxh +I xxh-shell-
```

### Comparing `xxh-xxh-0.8.8/setup.py` & `xxh-xxh-0.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `xxh-xxh-0.8.8/xxh/xxh_xxh/config.xxhc` & `xxh-xxh-0.8.9/xxh/xxh_xxh/config.xxhc`

 * *Files identical despite different names*

### Comparing `xxh-xxh-0.8.8/xxh/xxh_xxh/shell.py` & `xxh-xxh-0.8.9/xxh/xxh_xxh/shell.py`

 * *Files identical despite different names*

### Comparing `xxh-xxh-0.8.8/xxh/xxh_xxh/xxh.bash` & `xxh-xxh-0.8.9/xxh/xxh_xxh/xxh.bash`

 * *Files identical despite different names*

### Comparing `xxh-xxh-0.8.8/xxh/xxh_xxh/xxh.py` & `xxh-xxh-0.8.9/xxh/xxh_xxh/xxh.py`

 * *Files identical despite different names*

### Comparing `xxh-xxh-0.8.8/xxh/xxh_xxh/xxh.xsh` & `xxh-xxh-0.8.9/xxh/xxh_xxh/xxh.xsh`

 * *Files identical despite different names*

### Comparing `xxh-xxh-0.8.8/xxh/xxh_xxh/xxh.zsh` & `xxh-xxh-0.8.9/xxh/xxh_xxh/xxh.zsh`

 * *Files identical despite different names*

### Comparing `xxh-xxh-0.8.8/xxh_xxh.egg-info/PKG-INFO` & `xxh-xxh-0.8.9/xxh_xxh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xxh-xxh
-Version: 0.8.8
+Version: 0.8.9
 Summary: Bring your favorite shell wherever you go through the ssh
 Home-page: https://github.com/xxh/xxh
 Author: xxh
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/xxh/xxh/blob/master/README.md
 Project-URL: Code, https://github.com/xxh/xxh
@@ -105,15 +105,15 @@
 | **[elvish](https://github.com/krageon/xxh-shell-elvish)**   | alpha      |             | | |
 
 [Search xxh shell on Github](https://github.com/search?q=xxh-shell&type=Repositories) or [Bitbucket](https://bitbucket.org/repo/all?name=xxh-shell) or [create your shell entrypoint](https://github.com/xxh/xxh-shell-example) to use another portable shell.  
 
 ### Prerun plugins
 [Prerun plugins](https://github.com/xxh/xxh/wiki#plugins) allow you to bring any portable tools, dotfiles or aliases to xxh session before running shell. 
 
-Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **[xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-plugin-prerun-zoxide)**. There is [cookiecutter template to create prerun plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun).
+Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **[xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-plugin-prerun-zoxide)**, **[starship](https://github.com/izissise/xxh-plugin-prerun-starship)**. There is [cookiecutter template to create prerun plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun).
 
 ## Usage
 Use `xxh` instead of `ssh` when connecting to Linux hosts without changing ssh arguments:
 ```
 xxh <host from ~/.ssh/config>
 xxh [ssh arguments] [user@]host[:port] [xxh arguments]
 xxh local [xxh arguments]
@@ -129,16 +129,16 @@
 xxh anyhost +if +q                                # Force reinstall xxh on the host in quiet mode
 xxh anyhost +hh /tmp/xxh +hhr                     # Upload xxh to /tmp/xxh and remove when disconnecting
 source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh  # Connect in seamless mode with ohmyzsh plugin
 xxh local +s xonsh                                # Experimental: build xxh environment inplace and without ssh
 ```
 For reusing arguments and simplifying xxh usage (like shortening to `xxh anyhost`) there is a [config file](https://github.com/xxh/xxh/wiki#config-file).
 
-**Why the plus sign for the xxh arguments?** The xxh is using the plus sign for the xxh arguments to save the ability to use minus sign for the original ssh arguments. This allows just replace the first two letters in the `ssh` command to convert it to the `xxh` command.
-
+**Why the plus sign for the xxh arguments?** The xxh is using the plus sign for the xxh arguments to save the ability to use the minus sign for the original ssh arguments. This allows just replace the first two letters in the `ssh` command to convert it to the `xxh` command. Also see the [discussion](https://github.com/xxh/xxh/issues/129).
+ 
 ### Installing xxh packages
 ```bash
 xxh [+I xxh-package +I ...] [+L] [+RI xxh-package +RI ...] [+R xxh-package +R ...]
 ```
 Different ways to set the xxh package source:
 ```yaml
 xxh +I xxh-shell-example                                         # install from https://github.com/xxh
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xxh-xxh Version: 0.8.8 Summary: Bring your favorite
+Metadata-Version: 2.1 Name: xxh-xxh Version: 0.8.9 Summary: Bring your favorite
 shell wherever you go through the ssh Home-page: https://github.com/xxh/xxh
 Author: xxh Author-email: author@example.com License: BSD Project-URL:
 Documentation, https://github.com/xxh/xxh/blob/master/README.md Project-URL:
 Code, https://github.com/xxh/xxh Project-URL: Issue tracker, https://
 github.com/xxh/xxh/issues Platform: Unix-like Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Unix Shell Classifier: Topic
 :: System :: Shells Classifier: Topic :: System :: System Shells Classifier:
@@ -83,36 +83,38 @@
 bring any portable tools, dotfiles or aliases to xxh session before running
 shell. Pinned plugins: **[core](https://github.com/xxh/xxh-plugin-prerun-
 core)** (xxh-sudo, xxh-screen), **[dotfiles](https://github.com/xxh/xxh-plugin-
 prerun-dotfiles)**, **[docker](https://github.com/xxh/xxh-plugin-prerun-
 docker)**, **[python](https://github.com/xxh/xxh-plugin-prerun-python)**, **
 [xxh](https://github.com/xxh/xxh-plugin-prerun-xxh)**, **[vim](https://
 github.com/xxh/xxh-plugin-prerun-vim)**, **[zoxide](https://github.com/xxh/xxh-
-plugin-prerun-zoxide)**. There is [cookiecutter template to create prerun
-plugin](https://github.com/xxh/cookiecutter-xxh-plugin-prerun). ## Usage Use
-`xxh` instead of `ssh` when connecting to Linux hosts without changing ssh
-arguments: ``` xxh xxh [ssh arguments] [user@]host[:port] [xxh arguments] xxh
-local [xxh arguments] ``` Common examples (use `xxh --help` to get info about
-arguments): ```yaml xxh anyhost # Connect to the host xxh -i id_rsa -p 2222
-anyhost # Using ssh arguments: port and key xxh anyhost +s zsh +i # Set the
-shell and install it without yes/no question xxh anyhost +s xonsh +hhh "~" #
-Set /home/user as home directory (read Q&A) xxh anyhost +s bash +I xxh-plugin-
-bash-vim # Preinstall a plugin xxh anyhost +if +q # Force reinstall xxh on the
-host in quiet mode xxh anyhost +hh /tmp/xxh +hhr # Upload xxh to /tmp/xxh and
-remove when disconnecting source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh #
-Connect in seamless mode with ohmyzsh plugin xxh local +s xonsh # Experimental:
-build xxh environment inplace and without ssh ``` For reusing arguments and
+plugin-prerun-zoxide)**, **[starship](https://github.com/izissise/xxh-plugin-
+prerun-starship)**. There is [cookiecutter template to create prerun plugin]
+(https://github.com/xxh/cookiecutter-xxh-plugin-prerun). ## Usage Use `xxh`
+instead of `ssh` when connecting to Linux hosts without changing ssh arguments:
+``` xxh xxh [ssh arguments] [user@]host[:port] [xxh arguments] xxh local [xxh
+arguments] ``` Common examples (use `xxh --help` to get info about arguments):
+```yaml xxh anyhost # Connect to the host xxh -i id_rsa -p 2222 anyhost # Using
+ssh arguments: port and key xxh anyhost +s zsh +i # Set the shell and install
+it without yes/no question xxh anyhost +s xonsh +hhh "~" # Set /home/user as
+home directory (read Q&A) xxh anyhost +s bash +I xxh-plugin-bash-vim #
+Preinstall a plugin xxh anyhost +if +q # Force reinstall xxh on the host in
+quiet mode xxh anyhost +hh /tmp/xxh +hhr # Upload xxh to /tmp/xxh and remove
+when disconnecting source xxh.zsh anyhost +I xxh-plugin-zsh-ohmyzsh # Connect
+in seamless mode with ohmyzsh plugin xxh local +s xonsh # Experimental: build
+xxh environment inplace and without ssh ``` For reusing arguments and
 simplifying xxh usage (like shortening to `xxh anyhost`) there is a [config
 file](https://github.com/xxh/xxh/wiki#config-file). **Why the plus sign for the
 xxh arguments?** The xxh is using the plus sign for the xxh arguments to save
-the ability to use minus sign for the original ssh arguments. This allows just
-replace the first two letters in the `ssh` command to convert it to the `xxh`
-command. ### Installing xxh packages ```bash xxh [+I xxh-package +I ...] [+L]
-[+RI xxh-package +RI ...] [+R xxh-package +R ...] ``` Different ways to set the
-xxh package source: ```yaml xxh +I xxh-shell-example # install from https://
+the ability to use the minus sign for the original ssh arguments. This allows
+just replace the first two letters in the `ssh` command to convert it to the
+`xxh` command. Also see the [discussion](https://github.com/xxh/xxh/issues/
+129). ### Installing xxh packages ```bash xxh [+I xxh-package +I ...] [+L] [+RI
+xxh-package +RI ...] [+R xxh-package +R ...] ``` Different ways to set the xxh
+package source: ```yaml xxh +I xxh-shell-example # install from https://
 github.com/xxh xxh +I https://github.com/xxh/xxh-shell-example # short url for
 github only, for other sources use examples below or add support xxh +I https:/
 /github.com/xxh/xxh-shell-example/tree/mybranch # short url for github only,
 for other sources use examples below or add support xxh +I xxh-shell-
 example+git+https://github.com/xxh/xxh-shell-example # long url for any git
 repo xxh +I xxh-shell-example+git+https://github.com/xxh/xxh-shell-example/
 tree/mybranch # github only branch support xxh +I xxh-shell-
```

