# Comparing `tmp/pyracf-0.7.1.tar.gz` & `tmp/pyracf-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.7.1.tar", last modified: Sat Mar 30 10:34:10 2024, max compression
+gzip compressed data, was "pyracf-0.8.2.tar", last modified: Sun Apr  7 11:10:19 2024, max compression
```

## Comparing `pyracf-0.7.1.tar` & `pyracf-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-03-30 10:34:10.657276 pyracf-0.7.1/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2024-03-30 10:31:52.000000 pyracf-0.7.1/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2024-03-30 10:31:52.000000 pyracf-0.7.1/MANIFEST.in
--rw-r--r--   0 henri     (1000) henri     (1000)    12853 2024-03-30 10:34:10.657276 pyracf-0.7.1/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)    12245 2024-03-30 10:32:07.000000 pyracf-0.7.1/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-03-30 10:34:10.657276 pyracf-0.7.1/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-03-30 10:32:07.000000 pyracf-0.7.1/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-03-30 10:34:10.657276 pyracf-0.7.1/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-03-30 10:34:10.657276 pyracf-0.7.1/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    60684 2024-03-30 10:32:07.000000 pyracf-0.7.1/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-03-30 10:32:07.000000 pyracf-0.7.1/src/pyracf/getOffsets.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-03-30 10:32:07.000000 pyracf-0.7.1/src/pyracf/offsets.json
--rw-rw-r--   0 henri     (1000) henri     (1000)     7994 2024-03-30 10:32:07.000000 pyracf-0.7.1/src/pyracf/profileFieldRules.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-03-30 10:34:10.657276 pyracf-0.7.1/src/pyracf.egg-info/
--rw-r--r--   0 henri     (1000) henri     (1000)    12853 2024-03-30 10:34:09.000000 pyracf-0.7.1/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      311 2024-03-30 10:34:10.000000 pyracf-0.7.1/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-03-30 10:34:09.000000 pyracf-0.7.1/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-03-30 10:34:09.000000 pyracf-0.7.1/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-03-30 10:34:09.000000 pyracf-0.7.1/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-07 11:10:19.286604 pyracf-0.8.2/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2024-03-30 10:31:52.000000 pyracf-0.8.2/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2024-03-30 10:31:52.000000 pyracf-0.8.2/MANIFEST.in
+-rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-07 11:10:19.286604 pyracf-0.8.2/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)    14510 2024-04-07 11:09:44.000000 pyracf-0.8.2/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-07 11:10:19.286604 pyracf-0.8.2/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-07 11:09:44.000000 pyracf-0.8.2/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-07 11:10:19.286604 pyracf-0.8.2/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-07 11:10:19.286604 pyracf-0.8.2/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    56865 2024-04-07 11:09:44.000000 pyracf-0.8.2/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-07 11:09:44.000000 pyracf-0.8.2/src/pyracf/getOffsets.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-07 11:09:44.000000 pyracf-0.8.2/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-07 11:10:19.286604 pyracf-0.8.2/src/pyracf.egg-info/
+-rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      279 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.7.1/LICENSE` & `pyracf-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.7.1/PKG-INFO` & `pyracf-0.8.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: pyracf
-Version: 0.7.1
-Summary: Parsing IRRDBU00 unloads in panda dataframes.
-Home-page: https://github.com/wizardofzos/pyracf
-Author: Wizard of z/OS
-Author-email: wizard@zdevops.com
-Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: wheel
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: xlsxwriter>=3.1.0
-
 # pyracf
 
 ## PyRACF: A Python module for analyzing RACF security
 
 PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database, providing an efficient and intuitive way to analyze security setups on IBM Z systems. By consuming the IRRDBU00 unload, PyRACF generates "Panda DataFrames" for each 'recordtype', which allow for seamless manipulation and analysis of the data.
 
 Pandas is a powerful data manipulation library in Python that allows for easy querying of the DataFrames generated by PyRACF. With Pandas, you can perform complex queries on the security data to extract meaningful insights into the security posture of your system.
@@ -29,14 +11,28 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.2 (property for most application segments)
+- application segments for dataset, group and user entities are avaible with entity prefix, e.g., msys.userTSO, msys.datasetDFP, msys.groupOMVS
+- system related application segments from general resources are published without prefix, e.g., msys.STDATA or msys.MFA
+- old properties msys.installdata and msys.userDistributedMappings are replaced by userUSRDATA and userDistributedIdMappings
+- most of these properties are automatically generated
+
+### 0.8.0 (acl, gfilter, rfilter methods)
+- selection method gfilter (supports RACF generic patterns) and rfilter (for regex patterns)
+  supports as many parameters as there are index columns in the frame
+- reporting method acl, produces frame with access list, may be used on the entity frames or on the access frames
+- internal frames _connectByGroup and _connectByUser, as alternate index on connectData
+- internal frames _grouptreeLines and _ownertreeLines that return all groups up until SYS1 (or upto a user ID)
+- correlate() invoked automatically by parse() and fancycli()
+
 ### 0.7.1 (General instead of Generic)
 - fixed: Generic should be General resource profiles, variables and methods renamed
 - Mapping between IRRDBU00 record types and variables centralized in a dict
 - global constants related to record types removed
 - parsed records internally stored by (decimal) record type, instead of by name
 - add method to retrieve parsed record count for given name
 - _offsets now a RACF class attribute
@@ -44,18 +40,20 @@
 - fixed: status property crashed when used before parse() method used, math.floor call is now conditional
 - fixed: record type '0260' in offset.json was malformed
 - updated offsets.json from https://www.ibm.com/docs/en/SSLTBW_3.1.0/com.ibm.zos.v3r1.icha300/format.htm etc
 - getOffsets.py to update the json model
 - fixed: RACF documentation contains incorrect record type 05k0
 - all known record types parsed and loaded into DataFrames
 - index columns assigned to all DataFrames, assigned by new correlate() method
-- new method correlate() to increase speed of subsequent data access, use after parse() or loading of pickles
-- selection and reporting methods dataset(), group(), general(), user() and connect(), accepts GENERIC and regex patterns 
-- also datasetPermit and datasetConditionalPermit, with parameters profile(mask), id(mask) and access(mask) 
-- also generalPermit and generalConditionalPermit, with parameters resclass(mask), profile(mask), id(mask) and access(mask)
+- new method correlate() to increase speed of subsequent data access, used after parse() or loading of pickles
+- new selection methods similar to user() and group(), that work on index fields.
+    when a parameter is given as None or '**', elements matching the other parameters are returned:
+    datasetPermit and datasetConditionalPermit, with parameters profile(), id() and access() 
+    generalPermit and generalConditionalPermit, with parameters resclass(), profile(), id() and access()
+    connect with parameters group() and user()
 - added GPMEM_AUTH to connectData frame, consolidating all connect info into one line 
 
 ### 0.6.4 (Add 0209)
 - Added 0209 recordtype to parser. (userDistributedMapping)
 
 ### 0.6.3 (Add fields)
 - Added missing USBD_LEG_PWDHIST_CT, USBD_XPW_PWDHIST_CT, USBD_PHR_ALG, USBD_LEG_PHRHIST_CT, USBD_XPW_PHRHIST_CT, USBD_ROAUDIT and USBD_MFA_FALLBACK to Users dataframe
@@ -122,105 +120,109 @@
 Then later, you don't need to parse the same unload again, just do:
 
     >>> from pyracf import RACF
     >>> mysys = RACF(pickles='/tmp/pickles', prefix='mysys-')
     >>> hash(mysys.groups.values.tobytes())
     -8566685915584060910
 
-### Prepare internal data structures for later processing
-
-    >>> mysys.correlate()
 
 ## All functions
 
 | Function/Property | Explanation | Example |
 |---|---|---|
+| acl | Returns DataFrame with access control list for the given frame | msys.datasets.acl(permits=True, explode=False, resolve=False, admin=False, access=None, allows=None, sort="profile")
 | auditors | Returns DataFrame with all user having the auditor bit switched on | mysys.auditors |
-| connect | Returns DataFrame with selected user to group connects | mysys.connect('SYS1',None,'G') or mysys.connect('**','IBM*','G') |
-| connects | Returns DataFrame with all user to group connects | mysys.connects |
+| connect | Returns DataFrame with selected user to group connects | mysys.connect('SYS1',None) or mysys.connect('**','IBMUSER') |
+| connects | Returns DataFrame with all user to group connects, use connect or connectData instead | mysys.connects |
+| connectData | Returns DataFrame with all user to group connect information | mysys.connectData |
 | correlate | assigns index columns and prepares data structures for faster reporting | mysys.correlate() |
 | datasetAccess | Returns DataFrame with all Accesslists for all dataset profiles | mysys.datasetsAccess |
-| dataset | Returns DataFrame with selected datasetprofiles | mysys.dataset('SYS1.**','GEN') |
-| datasetPermit | Returns DataFrame with selected permits on datasetprofiles | mysys.datasetPermit(profile=, id=, access=, pattern='G') |
-| datasetConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on datasetprofiles | mysys.datasetConditionalPermit(profile=, id=, access=, pattern='G') |
+| dataset | Returns DataFrame with selected datasetprofiles | mysys.dataset('SYS1.**') |
+| datasetPermit | Returns DataFrame with selected permits on datasetprofiles | mysys.datasetPermit(profile=, id=, access=) |
+| datasetConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on datasetprofiles | mysys.datasetConditionalPermit(profile=, id=, access=) |
 | datasets | Returns DataFrame with all datasetprofiles | mysys.datasets |
 | generalAccess | Returns DataFrame with with all accesslists for general resource profiles | mysys.generalAccess
 | generalConditionalAccess | Returns DataFrame with with all conditional accesslists for general resource profiles | mysys.generalConditionalAccess
-| general | Returns DataFrame with selected general resource profiles | mysys.general('FACI*','BPX.**','GEN') |
-| generalPermit | Returns DataFrame with selected permits on resource profiles | mysys.generalPermit(resclass=, profile=, id=, access=, pattern='G') |
-| generalConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on resource profiles | mysys.generalConditionalPermit(resclass=, profile=, id=, access=, pattern='G') |
+| general | Returns DataFrame with selected general resource profiles | mysys.general(reclass=, profile=) |
+| generalPermit | Returns DataFrame with selected permits on resource profiles | mysys.generalPermit(resclass=, profile=, id=, access=) |
+| generalConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on resource profiles | mysys.generalConditionalPermit(resclass=, profile=, id=, access=) |
 | generals | Returns DataFrame with with all general resource profiles | mysys.generals 
 | getdatasetrisk | Returns dict with users that have access or administrative authority on a profile | mysys.getdatasetrisk('SYS1.**') |
-| group | Returns DataFrame with with group profiles matching selection | mysys.group('SYS1'), or msys.group('SYS*','G') |
-| groupConnect | Returns DataFrame with with user group connection records (0203 recordtype) | mysys.groupConnect |
+| gfilter | Returns DataFrame with records matching the index fields specified, using RACF generic patterns | mysys.datasets.gfilter('SYS%.**')) or mysys.generals.gfilter('FACI*','BPX.**'))|
+| group | Returns DataFrame with group profiles matching selection | mysys.group('SYS1') |
+| groupConnect | Returns DataFrame with with user group connection records (0203 recordtype), use connect or connectData instead | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | groupsWithoutUsers | Returns DataFrame with groups that have no connected users | mysys.groupsWithoutUsers |
 | grouptree | Returns dict with groups arranged by superior group | mysys.grouptree() |
 | installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for general resources | d, g = mysys.orphans |
 | ownertree | Returns dict with groups arranged by owner group or user ID | mysys.ownertree() |
 | parse | parses the unload. optional specify recordtypes | mysys.parse(recordtypes=['0200']) |
 | parse_fancycli | parses the unload with a fancy cli status update. optional recordtypes can be specified | mysys.parse_fancycli(recorddtypes=['0200']) |
 | revoked | Returns a DataFrame  with all revoked users | mysys.revoked |
+| rfilter | Returns DataFrame with records matching the index fields specified, using regex patterns | mysys.generals.rfilter('FAC.*','BPX\..*')) |
 | save_pickles | Saves all parsed types as pickle files | mysys.save_pickles(path='/tmp', prefix='mysys-') |
 | specials | Returns a DataFrame  with all special users | mysys.specials |
 | status | Returns JSON with parsing status | mysys.status |
 | uacc_read_datasets | Returns a DataFrame  with all dataset profiles having UACC=READ | mysys.uacc_read_datasets |
-| user | Returns DataFrame with with user profiles matching selection | mysys.user('IBM*'), or msys.user('SYS.*','REGEX') |
+| uacc_update_datasets | Returns a DataFrame  with all dataset profiles having UACC=UPDATE | mysys.uacc_update_datasets |
+| user | Returns DataFrame with with user profiles matching selection | mysys.user('IBMUSER') |
 | users | Returns DataFrame with all user base data | mysys.users |
 | xls | Creates an XLSX with all permits per class | mysys.xls(fileName='myxls.xlsx') |
 
 # Example use-case
 
 Get all users that have not logged in (on?) since January 1st 2022. And print userID and last logon...
 
     import time
     from pyracf import IRRDBU
 
     mysys = IRRDBU('/path/to/irrdbu00')
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
-    mysys.correlate()
     selection = mysys.users.loc[mysys.users.USBD_LASTJOB_DATE<="2022-01-01"][['USBD_NAME','USBD_LASTJOB_DATE']]
     for user in selection.values:
       print(f"Userid {user[0]}, last active: {user[1]}")
 
 Create a neat XLSX
 
     import time
     from pyracf import IRRDBU
     mysys = IRRDBU('/path/to/irrdbu00')
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
-    mysys.correlate()
     mysys.xls('/path/to/my.xlsx')
 
 Print z/OS UNIX profiles
 
-    mysys.correlate()
-    mysys.general('FAC*', 'BPX.**', 'G')
-    mysys.general('UNIXPRIV', '**', 'G') # print all in UNIXPRIV
+    mysys.generals.gfilter('FAC*', 'BPX.**')
+    mysys.generals.gfilter('UNIXPRIV') # print all in UNIXPRIV
 
 Show group information
 
-    mysys.correlate()
-    mysys.connect('SYS*', None, 'G')    # users connected to SYSxxxxx groups
-    mysys.general('**', 'IBMUSER', 'G') # connects of user IBMUSER
-    mysys.general(user='IBMUSER', pattern='G') # connects of user IBMUSER
+    mysys.connect('SYS1')            # users connected to SYS1 groups
+    mysys.connect('**','IBMUSER')    # groups IBMUSER is connected to
+    mysys.connectData.gfilter('SYS*','IBM*') # connects using patterns
+    mysys.connectData.rfilter('SYS[AB].*','PROD.*') # regex with alternatives
+    mysys.connectData.query("USCON_GRP_SPECIAL=='YES' & USCON_REVOKE=='YES'")  # group special revoked
+    mysys.connectData.query("GPMEM_AUTH==['CONNECT','JOIN']")  # users with connect authorities
 
 Show access list information
 
-    mysys.correlate()
     mysys.datasetPermit('SYS1.**')    # IDs permitted on SYS1.**
-    mysys.datasetPermit(id='IBMUSER', pattern='GENERIC')    # where is IBMUSER permitted
-    mysys.datasetPermit('SYS1.**', access='ALTER', pattern='G')    # IDs ALTER access on any SYS1 dataset profile
-    mysys.generalPermit('XFAC*', 'CKR.**', pattern='G') # permits on zSecure Admin/Audit profile
+    mysys.datasetPermit(id='IBMUSER', access='ALTER')    # where is IBMUSER permitted
+
+    mysys.datasets.gfilter('SYS1.**').acl(access='ALTER')    # IDs ALTER access on any SYS1 dataset profile
+    mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE')    # IDs with access that allows UPDATE
+    mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE', resolve=True)    # groups and user permits combined 
+    mysys.datasets.gfilter('PROD.**').acl(permits=False, admin=True)    # who can change groups or profiles to change access on PROD data sets
+    mysys.generals.gfilter('XFAC*', 'CKR.**').acl() # permits on zSecure Admin/Audit profile
 
 
 # Updates 
 
 In this version we introduced IRRRDBU as an alternative to RACF. Examples have been updated. The RACF class from previous version is still available, but you're advised to change this to IRRDBU, as future version will have another user of the RACF class.
 
 # Contribute to PyRACF
```

### Comparing `pyracf-0.7.1/README.md` & `pyracf-0.8.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: pyracf
+Version: 0.8.2
+Summary: Parsing IRRDBU00 unloads in panda dataframes.
+Home-page: https://github.com/wizardofzos/pyracf
+Author: Wizard of z/OS
+Author-email: wizard@zdevops.com
+Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: wheel
+Requires-Dist: pandas>=1.5.2
+Requires-Dist: xlsxwriter>=3.1.0
+
 # pyracf
 
 ## PyRACF: A Python module for analyzing RACF security
 
 PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database, providing an efficient and intuitive way to analyze security setups on IBM Z systems. By consuming the IRRDBU00 unload, PyRACF generates "Panda DataFrames" for each 'recordtype', which allow for seamless manipulation and analysis of the data.
 
 Pandas is a powerful data manipulation library in Python that allows for easy querying of the DataFrames generated by PyRACF. With Pandas, you can perform complex queries on the security data to extract meaningful insights into the security posture of your system.
@@ -11,14 +29,28 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.2 (property for most application segments)
+- application segments for dataset, group and user entities are avaible with entity prefix, e.g., msys.userTSO, msys.datasetDFP, msys.groupOMVS
+- system related application segments from general resources are published without prefix, e.g., msys.STDATA or msys.MFA
+- old properties msys.installdata and msys.userDistributedMappings are replaced by userUSRDATA and userDistributedIdMappings
+- most of these properties are automatically generated
+
+### 0.8.0 (acl, gfilter, rfilter methods)
+- selection method gfilter (supports RACF generic patterns) and rfilter (for regex patterns)
+  supports as many parameters as there are index columns in the frame
+- reporting method acl, produces frame with access list, may be used on the entity frames or on the access frames
+- internal frames _connectByGroup and _connectByUser, as alternate index on connectData
+- internal frames _grouptreeLines and _ownertreeLines that return all groups up until SYS1 (or upto a user ID)
+- correlate() invoked automatically by parse() and fancycli()
+
 ### 0.7.1 (General instead of Generic)
 - fixed: Generic should be General resource profiles, variables and methods renamed
 - Mapping between IRRDBU00 record types and variables centralized in a dict
 - global constants related to record types removed
 - parsed records internally stored by (decimal) record type, instead of by name
 - add method to retrieve parsed record count for given name
 - _offsets now a RACF class attribute
@@ -26,18 +58,20 @@
 - fixed: status property crashed when used before parse() method used, math.floor call is now conditional
 - fixed: record type '0260' in offset.json was malformed
 - updated offsets.json from https://www.ibm.com/docs/en/SSLTBW_3.1.0/com.ibm.zos.v3r1.icha300/format.htm etc
 - getOffsets.py to update the json model
 - fixed: RACF documentation contains incorrect record type 05k0
 - all known record types parsed and loaded into DataFrames
 - index columns assigned to all DataFrames, assigned by new correlate() method
-- new method correlate() to increase speed of subsequent data access, use after parse() or loading of pickles
-- selection and reporting methods dataset(), group(), general(), user() and connect(), accepts GENERIC and regex patterns 
-- also datasetPermit and datasetConditionalPermit, with parameters profile(mask), id(mask) and access(mask) 
-- also generalPermit and generalConditionalPermit, with parameters resclass(mask), profile(mask), id(mask) and access(mask)
+- new method correlate() to increase speed of subsequent data access, used after parse() or loading of pickles
+- new selection methods similar to user() and group(), that work on index fields.
+    when a parameter is given as None or '**', elements matching the other parameters are returned:
+    datasetPermit and datasetConditionalPermit, with parameters profile(), id() and access() 
+    generalPermit and generalConditionalPermit, with parameters resclass(), profile(), id() and access()
+    connect with parameters group() and user()
 - added GPMEM_AUTH to connectData frame, consolidating all connect info into one line 
 
 ### 0.6.4 (Add 0209)
 - Added 0209 recordtype to parser. (userDistributedMapping)
 
 ### 0.6.3 (Add fields)
 - Added missing USBD_LEG_PWDHIST_CT, USBD_XPW_PWDHIST_CT, USBD_PHR_ALG, USBD_LEG_PHRHIST_CT, USBD_XPW_PHRHIST_CT, USBD_ROAUDIT and USBD_MFA_FALLBACK to Users dataframe
@@ -104,105 +138,109 @@
 Then later, you don't need to parse the same unload again, just do:
 
     >>> from pyracf import RACF
     >>> mysys = RACF(pickles='/tmp/pickles', prefix='mysys-')
     >>> hash(mysys.groups.values.tobytes())
     -8566685915584060910
 
-### Prepare internal data structures for later processing
-
-    >>> mysys.correlate()
 
 ## All functions
 
 | Function/Property | Explanation | Example |
 |---|---|---|
+| acl | Returns DataFrame with access control list for the given frame | msys.datasets.acl(permits=True, explode=False, resolve=False, admin=False, access=None, allows=None, sort="profile")
 | auditors | Returns DataFrame with all user having the auditor bit switched on | mysys.auditors |
-| connect | Returns DataFrame with selected user to group connects | mysys.connect('SYS1',None,'G') or mysys.connect('**','IBM*','G') |
-| connects | Returns DataFrame with all user to group connects | mysys.connects |
+| connect | Returns DataFrame with selected user to group connects | mysys.connect('SYS1',None) or mysys.connect('**','IBMUSER') |
+| connects | Returns DataFrame with all user to group connects, use connect or connectData instead | mysys.connects |
+| connectData | Returns DataFrame with all user to group connect information | mysys.connectData |
 | correlate | assigns index columns and prepares data structures for faster reporting | mysys.correlate() |
 | datasetAccess | Returns DataFrame with all Accesslists for all dataset profiles | mysys.datasetsAccess |
-| dataset | Returns DataFrame with selected datasetprofiles | mysys.dataset('SYS1.**','GEN') |
-| datasetPermit | Returns DataFrame with selected permits on datasetprofiles | mysys.datasetPermit(profile=, id=, access=, pattern='G') |
-| datasetConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on datasetprofiles | mysys.datasetConditionalPermit(profile=, id=, access=, pattern='G') |
+| dataset | Returns DataFrame with selected datasetprofiles | mysys.dataset('SYS1.**') |
+| datasetPermit | Returns DataFrame with selected permits on datasetprofiles | mysys.datasetPermit(profile=, id=, access=) |
+| datasetConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on datasetprofiles | mysys.datasetConditionalPermit(profile=, id=, access=) |
 | datasets | Returns DataFrame with all datasetprofiles | mysys.datasets |
 | generalAccess | Returns DataFrame with with all accesslists for general resource profiles | mysys.generalAccess
 | generalConditionalAccess | Returns DataFrame with with all conditional accesslists for general resource profiles | mysys.generalConditionalAccess
-| general | Returns DataFrame with selected general resource profiles | mysys.general('FACI*','BPX.**','GEN') |
-| generalPermit | Returns DataFrame with selected permits on resource profiles | mysys.generalPermit(resclass=, profile=, id=, access=, pattern='G') |
-| generalConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on resource profiles | mysys.generalConditionalPermit(resclass=, profile=, id=, access=, pattern='G') |
+| general | Returns DataFrame with selected general resource profiles | mysys.general(reclass=, profile=) |
+| generalPermit | Returns DataFrame with selected permits on resource profiles | mysys.generalPermit(resclass=, profile=, id=, access=) |
+| generalConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on resource profiles | mysys.generalConditionalPermit(resclass=, profile=, id=, access=) |
 | generals | Returns DataFrame with with all general resource profiles | mysys.generals 
 | getdatasetrisk | Returns dict with users that have access or administrative authority on a profile | mysys.getdatasetrisk('SYS1.**') |
-| group | Returns DataFrame with with group profiles matching selection | mysys.group('SYS1'), or msys.group('SYS*','G') |
-| groupConnect | Returns DataFrame with with user group connection records (0203 recordtype) | mysys.groupConnect |
+| gfilter | Returns DataFrame with records matching the index fields specified, using RACF generic patterns | mysys.datasets.gfilter('SYS%.**')) or mysys.generals.gfilter('FACI*','BPX.**'))|
+| group | Returns DataFrame with group profiles matching selection | mysys.group('SYS1') |
+| groupConnect | Returns DataFrame with with user group connection records (0203 recordtype), use connect or connectData instead | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | groupsWithoutUsers | Returns DataFrame with groups that have no connected users | mysys.groupsWithoutUsers |
 | grouptree | Returns dict with groups arranged by superior group | mysys.grouptree() |
 | installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for general resources | d, g = mysys.orphans |
 | ownertree | Returns dict with groups arranged by owner group or user ID | mysys.ownertree() |
 | parse | parses the unload. optional specify recordtypes | mysys.parse(recordtypes=['0200']) |
 | parse_fancycli | parses the unload with a fancy cli status update. optional recordtypes can be specified | mysys.parse_fancycli(recorddtypes=['0200']) |
 | revoked | Returns a DataFrame  with all revoked users | mysys.revoked |
+| rfilter | Returns DataFrame with records matching the index fields specified, using regex patterns | mysys.generals.rfilter('FAC.*','BPX\..*')) |
 | save_pickles | Saves all parsed types as pickle files | mysys.save_pickles(path='/tmp', prefix='mysys-') |
 | specials | Returns a DataFrame  with all special users | mysys.specials |
 | status | Returns JSON with parsing status | mysys.status |
 | uacc_read_datasets | Returns a DataFrame  with all dataset profiles having UACC=READ | mysys.uacc_read_datasets |
-| user | Returns DataFrame with with user profiles matching selection | mysys.user('IBM*'), or msys.user('SYS.*','REGEX') |
+| uacc_update_datasets | Returns a DataFrame  with all dataset profiles having UACC=UPDATE | mysys.uacc_update_datasets |
+| user | Returns DataFrame with with user profiles matching selection | mysys.user('IBMUSER') |
 | users | Returns DataFrame with all user base data | mysys.users |
 | xls | Creates an XLSX with all permits per class | mysys.xls(fileName='myxls.xlsx') |
 
 # Example use-case
 
 Get all users that have not logged in (on?) since January 1st 2022. And print userID and last logon...
 
     import time
     from pyracf import IRRDBU
 
     mysys = IRRDBU('/path/to/irrdbu00')
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
-    mysys.correlate()
     selection = mysys.users.loc[mysys.users.USBD_LASTJOB_DATE<="2022-01-01"][['USBD_NAME','USBD_LASTJOB_DATE']]
     for user in selection.values:
       print(f"Userid {user[0]}, last active: {user[1]}")
 
 Create a neat XLSX
 
     import time
     from pyracf import IRRDBU
     mysys = IRRDBU('/path/to/irrdbu00')
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
-    mysys.correlate()
     mysys.xls('/path/to/my.xlsx')
 
 Print z/OS UNIX profiles
 
-    mysys.correlate()
-    mysys.general('FAC*', 'BPX.**', 'G')
-    mysys.general('UNIXPRIV', '**', 'G') # print all in UNIXPRIV
+    mysys.generals.gfilter('FAC*', 'BPX.**')
+    mysys.generals.gfilter('UNIXPRIV') # print all in UNIXPRIV
 
 Show group information
 
-    mysys.correlate()
-    mysys.connect('SYS*', None, 'G')    # users connected to SYSxxxxx groups
-    mysys.general('**', 'IBMUSER', 'G') # connects of user IBMUSER
-    mysys.general(user='IBMUSER', pattern='G') # connects of user IBMUSER
+    mysys.connect('SYS1')            # users connected to SYS1 groups
+    mysys.connect('**','IBMUSER')    # groups IBMUSER is connected to
+    mysys.connectData.gfilter('SYS*','IBM*') # connects using patterns
+    mysys.connectData.rfilter('SYS[AB].*','PROD.*') # regex with alternatives
+    mysys.connectData.query("USCON_GRP_SPECIAL=='YES' & USCON_REVOKE=='YES'")  # group special revoked
+    mysys.connectData.query("GPMEM_AUTH==['CONNECT','JOIN']")  # users with connect authorities
 
 Show access list information
 
-    mysys.correlate()
     mysys.datasetPermit('SYS1.**')    # IDs permitted on SYS1.**
-    mysys.datasetPermit(id='IBMUSER', pattern='GENERIC')    # where is IBMUSER permitted
-    mysys.datasetPermit('SYS1.**', access='ALTER', pattern='G')    # IDs ALTER access on any SYS1 dataset profile
-    mysys.generalPermit('XFAC*', 'CKR.**', pattern='G') # permits on zSecure Admin/Audit profile
+    mysys.datasetPermit(id='IBMUSER', access='ALTER')    # where is IBMUSER permitted
+
+    mysys.datasets.gfilter('SYS1.**').acl(access='ALTER')    # IDs ALTER access on any SYS1 dataset profile
+    mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE')    # IDs with access that allows UPDATE
+    mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE', resolve=True)    # groups and user permits combined 
+    mysys.datasets.gfilter('PROD.**').acl(permits=False, admin=True)    # who can change groups or profiles to change access on PROD data sets
+    mysys.generals.gfilter('XFAC*', 'CKR.**').acl() # permits on zSecure Admin/Audit profile
 
 
 # Updates 
 
 In this version we introduced IRRRDBU as an alternative to RACF. Examples have been updated. The RACF class from previous version is still available, but you're advised to change this to IRRDBU, as future version will have another user of the RACF class.
 
 # Contribute to PyRACF
```

### Comparing `pyracf-0.7.1/setup.py` & `pyracf-0.8.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.7.1",
+    version="0.8.2",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.7.1/src/pyracf/__init__.py` & `pyracf-0.8.2/src/pyracf/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import importlib.resources
 import json
-import yaml
-import math
 import pandas as pd 
 
+import math
+
+
 # No mess with my header lines
 import pandas.io.formats.excel
 pandas.io.formats.excel.ExcelFormatter.header_style = None
 
 import threading
 import time
 from datetime import datetime
@@ -36,118 +37,126 @@
         return newroutine(*arg,**keywords)
     deprecated_func.func = func
     return deprecated_func
 
 class RACF:
     
     # Our states
-    STATE_BAD     = -1
-    STATE_INIT    =  0
-    STATE_PARSING =  1
-    STATE_READY   =  2
+    STATE_BAD         = -1
+    STATE_INIT        =  0
+    STATE_PARSING     =  1
+    STATE_READY       =  2
+    STATE_CORRELATING =  3
 
     # keep track of names used for a record type, "index" must be a list of field names
+    # A dict with `key` -> RecordType
+    #                   'name' -> Internal name (and prefix for pickle-files, and should match prefix in offsets.json for variables in the table (GPMEM_NAME etc...))
+    #                   'df'   -> name of internal df
+    #                   'index' -> index if different than <name>_NAME
+    #                   'publisher' -> property in class to get the df
+    #                                *         -> as df without the _
+    #                                all but * -> this name as property
     _recordtype_info = {
     '0100': {'name':'GPBD', 'df':'_groups'},
     '0101': {'name':'GPSGRP', 'df':'_subgroups'},
     '0102': {'name':'GPMEM', 'df':'_connects', "index":["GPMEM_NAME","GPMEM_MEMBER_ID"]},
-    '0103': {'name':'GPINSTD', 'df':'_groupUSRDATA'},
-    '0110': {'name':'GPDFP', 'df':'_groupDFP'},
-    '0120': {'name':'GPOMVS', 'df':'_groupOMVS'},
+    '0103': {'name':'GPINSTD', 'df':'_groupUSRDATA', 'publisher':'*'},
+    '0110': {'name':'GPDFP', 'df':'_groupDFP', 'publisher':'*'},
+    '0120': {'name':'GPOMVS', 'df':'_groupOMVS', 'publisher':'*'},
     '0130': {'name':'GPOVM', 'df':'_groupOVM'},
-    '0141': {'name':'GPTME', 'df':'_groupTME'},
-    '0151': {'name':'GPCSD', 'df':'_groupCSDATA'},
+    '0141': {'name':'GPTME', 'df':'_groupTME', 'publisher':'*'},
+    '0151': {'name':'GPCSD', 'df':'_groupCSDATA', 'publisher':'*'},
     '0200': {'name':'USBD', 'df':'_users'},
     '0201': {'name':'USCAT', 'df':'_userCategories'},
     '0202': {'name':'USCLA', 'df':'_userClasses'},
     '0203': {'name':'USGCON', 'df':'_groupConnect', "index":["USGCON_GRP_ID","USGCON_NAME"]},
-    '0204': {'name':'USINSTD', 'df':'_userUSRDATA'},
+    '0204': {'name':'USINSTD', 'df':'_userUSRDATA'},  # , 'publisher':'*'
     '0205': {'name':'USCON', 'df':'_connectData', "index":["USCON_GRP_ID","USCON_NAME"]},
-    '0206': {'name':'USRSF', 'df':'_userRRSFdata'},
-    '0207': {'name':'USCERT', 'df':'_userCERTname'},
-    '0208': {'name':'USNMAP', 'df':'_userAssociationMappings'},
-    '0209': {'name':'USDMAP', 'df':'_userDistributedMapping'},
-    '020A': {'name':'USMFA', 'df':'_userMFAfactor'},
-    '020B': {'name':'USMPOL', 'df':'_userMFApolicies'},
-    '0210': {'name':'USDFP', 'df':'_userDFP'},
-    '0220': {'name':'USTSO', 'df':'_userTSO'},
+    '0206': {'name':'USRSF', 'df':'_userRRSFdata', 'publisher':'userRRSFDATA'},
+    '0207': {'name':'USCERT', 'df':'_userCERTname', 'publisher':'*'},
+    '0208': {'name':'USNMAP', 'df':'_userAssociationMapping', 'publisher':'*'},
+    '0209': {'name':'USDMAP', 'df':'_userDistributedIdMapping'},  # , 'publisher':'*'
+    '020A': {'name':'USMFA', 'df':'_userMFAfactor', 'publisher':'*'},
+    '020B': {'name':'USMPOL', 'df':'_userMFApolicies', 'publisher':'*'},
+    '0210': {'name':'USDFP', 'df':'_userDFP', 'publisher':'*'},
+    '0220': {'name':'USTSO', 'df':'_userTSO', 'publisher':'*'},
     '0230': {'name':'USCICS', 'df':'_userCICS'},
     '0231': {'name':'USCOPC', 'df':'_userCICSoperatorClasses'},
     '0232': {'name':'USCRSL', 'df':'_userCICSrslKeys'},
     '0233': {'name':'USCTSL', 'df':'_userCICStslKeys'},
     '0240': {'name':'USLAN', 'df':'_userLANGUAGE'},
     '0250': {'name':'USOPR', 'df':'_userOPERPARM'},
     '0251': {'name':'USOPRP', 'df':'_userOPERPARMscope'},
-    '0260': {'name':'USWRK', 'df':'_userWORKATTR'},
-    '0270': {'name':'USOMVS', 'df':'_userOMVS'},
+    '0260': {'name':'USWRK', 'df':'_userWORKATTR', 'publisher':'*'},
+    '0270': {'name':'USOMVS', 'df':'_userOMVS', 'publisher':'*'},
     '0280': {'name':'USNETV', 'df':'_userNETVIEW'},
     '0281': {'name':'USNOPC', 'df':'_userNETVIEWopclass'},
     '0282': {'name':'USNDOM', 'df':'_userNETVIEWdomains'},
     '0290': {'name':'USDCE', 'df':'_userDCE'},
     '02A0': {'name':'USOVM', 'df':'_userOVM'},
     '02B0': {'name':'USLNOT', 'df':'_userLNOTES'},
     '02C0': {'name':'USNDS', 'df':'_userNDS'},
     '02D0': {'name':'USKERB', 'df':'_userKERB'},
     '02E0': {'name':'USPROXY', 'df':'_userPROXY'},
     '02F0': {'name':'USEIM', 'df':'_userEIM'},
-    '02G1': {'name':'USCSD', 'df':'_userCSDATA'},
-    '1210': {'name':'USMFAC', 'df':'_user-MFAfactorTags'},
+    '02G1': {'name':'USCSD', 'df':'_userCSDATA', 'publisher':'*'},
+    '1210': {'name':'USMFAC', 'df':'_userMFAfactorTags', 'publisher':'*'},
     '0400': {'name':'DSBD', 'df':'_datasets'},
     '0401': {'name':'DSCAT', 'df':'_datasetCategories'},
     '0402': {'name':'DSCACC', 'df':'_datasetConditionalAccess', "index":["DSCACC_NAME","DSCACC_AUTH_ID","DSCACC_ACCESS"]},
     '0403': {'name':'DSVOL', 'df':'_datasetVolumes'},
     '0404': {'name':'DSACC', 'df':'_datasetAccess', "index":["DSACC_NAME","DSACC_AUTH_ID","DSACC_ACCESS"]},
-    '0405': {'name':'DSINSTD', 'df':'_datasetUSRDATA'},
+    '0405': {'name':'DSINSTD', 'df':'_datasetUSRDATA', 'publisher':'*'},
     '0406': {'name':'DSMEM', 'df':'_datasetMember'},
-    '0410': {'name':'DSDFP', 'df':'_datasetDFP'},
-    '0421': {'name':'DSTME', 'df':'_datasetTME'},
-    '0431': {'name':'DSCSD', 'df':'_datasetCSDATA'},
+    '0410': {'name':'DSDFP', 'df':'_datasetDFP', 'publisher':'*'},
+    '0421': {'name':'DSTME', 'df':'_datasetTME', 'publisher':'*'},
+    '0431': {'name':'DSCSD', 'df':'_datasetCSDATA', 'publisher':'*'},
     '0500': {'name':'GRBD', 'df':'_generals'},
     '0501': {'name':'GRTVOL', 'df':'_generalTAPEvolume'},
     '0502': {'name':'GRCAT', 'df':'_generalCategories'},
     '0503': {'name':'GRMEM', 'df':'_generalMembers'},
-    '0504': {'name':'GRVOL', 'df':'_generalVolumes'},
+    '0504': {'name':'GRVOL', 'df':'_generalTAPEvolumes'},
     '0505': {'name':'GRACC', 'df':'_generalAccess', "index":["GRACC_CLASS_NAME","GRACC_NAME","GRACC_AUTH_ID","GRACC_ACCESS"]},
-    '0506': {'name':'GRINSTD', 'df':'_generalUSRDATA'},
+    '0506': {'name':'GRINSTD', 'df':'_generalUSRDATA', 'publisher':'*'},
     '0507': {'name':'GRCACC', 'df':'_generalConditionalAccess', "index":["GRCACC_CLASS_NAME","GRCACC_NAME","GRCACC_AUTH_ID","GRCACC_ACCESS"]},
-    '0508': {'name':'GRFLTR', 'df':'_generalFILTER'},
-    '0509': {'name':'GRDMAP', 'df':'_generalDistributedMapping'},
-    '0510': {'name':'GRSES', 'df':'_generalSESSION'},
-    '0511': {'name':'GRSESE', 'df':'_generalSESSIONentities'},
-    '0520': {'name':'GRDLF', 'df':'_generalDLF'},
-    '0521': {'name':'GRDLFJ', 'df':'_generalDLFjob-names'},
-    '0530': {'name':'GRSIGN', 'df':'_generalSSIGNON'},
-    '0540': {'name':'GRST', 'df':'_generalSTARTED'},
-    '0550': {'name':'GRSV', 'df':'_generalSYSTEMVIEW'},
-    '0560': {'name':'GRCERT', 'df':'_generalCERT'},
-    '0561': {'name':'CERTR', 'df':'_generalCERTreferences'},
-    '0562': {'name':'KEYR', 'df':'_general-KEYRING'},
-    '0570': {'name':'GRTME', 'df':'_generalTME'},
-    '0571': {'name':'GRTMEC', 'df':'_generalTMEchild'},
-    '0572': {'name':'GRTMER', 'df':'_generalTMEresource'},
-    '0573': {'name':'GRTMEG', 'df':'_generalTMEgroup'},
-    '0574': {'name':'GRTMEE', 'df':'_generalTMErole'},
-    '0580': {'name':'GRKERB', 'df':'_generalKERB'},
-    '0590': {'name':'GRPROXY', 'df':'_generalPROXY'},
-    '05A0': {'name':'GREIM', 'df':'_generalEIM'},
-    '05B0': {'name':'GRALIAS', 'df':'_generalALIAS'},
-    '05C0': {'name':'GRCDT', 'df':'_generalCDTINFO'},
-    '05D0': {'name':'GRICTX', 'df':'_generalICTX'},
-    '05E0': {'name':'GRCFDEF', 'df':'_generalCFDEF', "index":["GRCFDEF_CLASS","GRCFDEF_NAME"]},
-    '05F0': {'name':'GRSIG', 'df':'_generalSIGVER'},
-    '05G0': {'name':'GRCSF', 'df':'_generalICSF'},
-    '05G1': {'name':'GRCSFK', 'df':'_generalICSFkeylabel'},
-    '05G2': {'name':'GRCSFC', 'df':'_generalICSFcertificateIdentifier'},
-    '05H0': {'name':'GRMFA', 'df':'_generalMFAfactor'},
-    '05I0': {'name':'GRMFP', 'df':'_generalMFApolicy'},
-    '05I1': {'name':'GRMPF', 'df':'_generalMFApolicyFactors'},
-    '05J1': {'name':'GRCSD', 'df':'_generalCSDATA'},
-    '05K0': {'name':'GRIDTP', 'df':'_generalIDTFPARMS'},
-    '05L0': {'name':'GRJES', 'df':'_generalJESDATA'},
-    '1560': {'name':'CERTN', 'df':'_generalCERTNAME'}
+    '0508': {'name':'GRFLTR', 'df':'_generalDistributedIdFilter', 'publisher':'DistributedIdFilter'},
+    '0509': {'name':'GRDMAP', 'df':'_generalDistributedIdMapping', 'publisher':'DistributedIdMapping'},
+    '0510': {'name':'GRSES', 'df':'_generalSESSION', 'publisher':'SESSION'}, # APPCLU profiles
+    '0511': {'name':'GRSESE', 'df':'_generalSESSIONentities', 'publisher':'SESSIONentities'},
+    '0520': {'name':'GRDLF', 'df':'_generalDLFDATA', 'publisher':'DLFDATA'},
+    '0521': {'name':'GRDLFJ', 'df':'_generalDLFDATAjobnames', 'publisher':'DLFDATAjobnames'},
+    '0530': {'name':'GRSIGN', 'df':'_generalSSIGNON'}, # needs APPLDATA
+    '0540': {'name':'GRST', 'df':'_generalSTDATA', 'publisher':'STDATA'},
+    '0550': {'name':'GRSV', 'df':'_generalSVFMR', 'publisher':'SVFMR'}, # SYSMVIEW profiles
+    '0560': {'name':'GRCERT', 'df':'_generalCERT', 'publisher':'CERT'},
+    '1560': {'name':'CERTN', 'df':'_generalCERTname', 'publisher':'CERTname'},
+    '0561': {'name':'CERTR', 'df':'_generalCERTreferences', 'publisher':'CERTreferences'},
+    '0562': {'name':'KEYR', 'df':'_generalKEYRING', 'publisher':'KEYRING'},
+    '0570': {'name':'GRTME', 'df':'_generalTME', 'publisher':'TME'},
+    '0571': {'name':'GRTMEC', 'df':'_generalTMEchild', 'publisher':'TMEchild'},
+    '0572': {'name':'GRTMER', 'df':'_generalTMEresource', 'publisher':'TMEresource'},
+    '0573': {'name':'GRTMEG', 'df':'_generalTMEgroup', 'publisher':'TMEgroup'},
+    '0574': {'name':'GRTMEE', 'df':'_generalTMErole', 'publisher':'TMErole'},
+    '0580': {'name':'GRKERB', 'df':'_generalKERB', 'publisher':'KERB'},
+    '0590': {'name':'GRPROXY', 'df':'_generalPROXY', 'publisher':'PROXY'},
+    '05A0': {'name':'GREIM', 'df':'_generalEIM', 'publisher':'EIM'},
+    '05B0': {'name':'GRALIAS', 'df':'_generalALIAS', 'publisher':'ALIAS'}, # IP lookup value in SERVAUTH class
+    '05C0': {'name':'GRCDT', 'df':'_generalCDTINFO', 'publisher':'CDTINFO'},
+    '05D0': {'name':'GRICTX', 'df':'_generalICTX', 'publisher':'ICTX'},
+    '05E0': {'name':'GRCFDEF', 'df':'_generalCFDEF', "index":["GRCFDEF_CLASS","GRCFDEF_NAME"], 'publisher':'CFDEF'},
+    '05F0': {'name':'GRSIG', 'df':'_generalSIGVER', 'publisher':'SIGVER'},
+    '05G0': {'name':'GRCSF', 'df':'_generalICSF', 'publisher':'ICSF'},
+    '05G1': {'name':'GRCSFK', 'df':'_generalICSFsymexportKeylabel', 'publisher':'ICSFsymexportKeylabel'},
+    '05G2': {'name':'GRCSFC', 'df':'_generalICSFsymexportCertificateIdentifier', 'publisher':'ICSFsymexportCertificateIdentifier'},
+    '05H0': {'name':'GRMFA', 'df':'_generalMFA', 'publisher':'MFA'},
+    '05I0': {'name':'GRMFP', 'df':'_generalMFPOLICY', 'publisher':'MFPOLICY'},
+    '05I1': {'name':'GRMPF', 'df':'_generalMFPOLICYfactors', 'publisher':'MFPOLICYfactors'},
+    '05J1': {'name':'GRCSD', 'df':'_generalCSDATA', 'publisher':'*'},
+    '05K0': {'name':'GRIDTP', 'df':'_generalIDTFPARMS', 'publisher':'IDTFPARMS'},
+    '05L0': {'name':'GRJES', 'df':'_generalJES', 'publisher':'JES'}
     }
 
     _recordname_type = {}    # {'GPBD': '0100', ....}
     _recordname_df = {}      # {'GPBD': '_groups', ....}
     for (rtype,rinfo) in _recordtype_info.items():
         _recordname_type.update({rinfo['name']: rtype})
         _recordname_df.update({rinfo['name']: rinfo['df']})
@@ -203,14 +212,21 @@
                     setattr(self, dfname, pd.read_pickle(pickle))
                     recordsRetrieved = len(getattr(self, dfname))
                     self._records[recordtype] = {
                       "seen": recordsRetrieved,
                       "parsed": recordsRetrieved
                     }
                     self._unloadlines += recordsRetrieved
+            for (rtype,rinfo) in RACF._recordtype_info.items():
+                if 'publisher' in rinfo:
+                    publisher = rinfo['publisher'] if rinfo['publisher']!='*' else rinfo['df'].lstrip('_')
+                    if hasattr(self, rinfo['df']):
+                        setattr(self, publisher, getattr(self, rinfo['df']))
+                    else:
+                        setattr(self, publisher, lambda x: warnings.warn(f"{publisher} has not been collected."))
             self._state = self.STATE_READY
             self._stoptime = datetime.now()
 
         else:
             # Running threads
             self.THREAD_COUNT = 0
 
@@ -239,33 +255,41 @@
             status = "Error"
         elif self._state == self.STATE_INIT:
             status = "Initial Object"
         elif self._state == self.STATE_PARSING:
             status = "Still parsing your unload"
             start  = self._starttime
             speed  = math.floor(seen/((datetime.now() -self._starttime).total_seconds()))
+        elif self._state == self.STATE_CORRELATING:
+            status = "Optimizing tables"
+            start = self._starttime
+            speed = math.floor(seen/((datetime.now() -self._starttime).total_seconds()))
         elif self._state == self.STATE_READY:
             status = "Ready"
             speed  = math.floor(seen/((self._stoptime - self._starttime).total_seconds()))
             parsetime = (self._stoptime - self._starttime).total_seconds()
         else:
             status = "Limbo"     
         return {'status': status, 'input-lines': self._unloadlines, 'lines-read': seen, 'lines-parsed': parsed, 'lines-per-second': speed, 'parse-time': parsetime}
 
     def parse_fancycli(self, recordtypes=_recordtype_info.keys(), save_pickles=False, prefix=''):
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - parsing {self._irrdbu00}')
         self.parse(recordtypes=recordtypes)
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - selected recordtypes: {",".join(recordtypes)}')
-        while self._state != self.STATE_READY:
+        while self._state != self.STATE_CORRELATING:
             progress =  math.floor(((sum(r['seen'] for r in self._records.values() if r)) / self._unloadlines) * 63)
             pct = (progress/63) * 100 # not as strange as it seems:)
             done = progress * '▉'
             todo = (63-progress) * ' '
             print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - progress: {done}{todo} ({pct:.2f}%)'.center(80), end="\r")
             time.sleep(0.5)
+        print('')
+        while self._state != self.STATE_READY:
+             print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - correlating data {40*" "}', end="\r")
+             time.sleep(0.5)
         # make completed line always show 100% :)
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - progress: {63*"▉"} ({100:.2f}%)'.center(80))
         for r in recordtypes:
             print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - recordtype {r} -> {self.parsed(self._recordtype_info[r]["name"])} records parsed')
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - total parse time: {(self._stoptime - self._starttime).total_seconds()} seconds')
         if save_pickles:
             self.save_pickles(path=save_pickles,prefix=prefix)
@@ -278,15 +302,14 @@
 
     def parse_t(self, thingswewant=_recordtype_info.keys()):
         # TODO: make this multiple threads (per record-type?)
         if self.THREAD_COUNT == 0:
             self._starttime = datetime.now()
             self._state = self.STATE_PARSING
         self.THREAD_COUNT += 1
-        # TODO: Complete all record-types. Fix offsets.json !
         with open(self._irrdbu00, 'r', encoding="utf-8", errors="replace") as infile:
             for line in infile:
                 r = line[:4]
                 if r in self._records:
                     self._records[r]['seen'] += 1
                 else:
                     self._records[r] = {'seen': 1, 'parsed': 0}
@@ -303,39 +326,46 @@
                         self._parsed[r].append(irrmodel)
                         self._records[r]['parsed'] += 1
         # all models parsed :)
 
         for (rtype,rinfo) in RACF._recordtype_info.items():
             if rtype in thingswewant:
                 setattr(self, rinfo['df'], pd.DataFrame.from_dict(self._parsed[rtype]))
+            if 'publisher' in rinfo:
+                publisher = rinfo['publisher'] if rinfo['publisher']!='*' else rinfo['df'].lstrip('_')
+                if hasattr(self, rinfo['df']):
+                    setattr(self, publisher, getattr(self, rinfo['df']))
+                else:
+                    setattr(self, publisher, lambda x: warnings.warn(f"{publisher} has not been collected."))
 
         # TODO: Reduce memory use, delete self._parsed after dataframes are made
 
+        # We need the correlate anyways all the times so let's run it
         self.THREAD_COUNT -= 1
         if self.THREAD_COUNT == 0:
+            self._state = self.STATE_CORRELATING
+            self._correlate()
             self._state = self.STATE_READY         
             self._stoptime = datetime.now()
         return True
 
     def parsed(self, rname):
         """ how many records with this name (type) were parsed """
         rtype = RACF._recordname_type[rname]
         return self._records[rtype]['parsed'] if rtype in self._records else 0
         
-    def correlate(self, thingswewant=_recordtype_info.keys()):
+    def _correlate(self, thingswewant=_recordtype_info.keys()):
         """ construct tables that combine the raw dataframes for improved processing """
         
         # activate acl() method on our dataframes, so it get called with our instance's variables, the frame, and all optional parms
         # e.g. msys._datasetAccess.loc[['SYS1.**']].acl(permits=True, explode=False, resolve=False, admin=False, sort="user")
         pd.core.base.PandasObject.acl = lambda *x,**y: RACF.acl(self,*x,**y)
-        pd.core.base.PandasObject.ACL = lambda *x,**y: RACF.acl(self,*x,**y)
 
         # generic and regex filter on the index levels of a frame
-        pd.core.base.PandasObject.FILTER = RACF.gfilter
-        pd.core.base.PandasObject.MATCH = RACF.rfilter
+        # e.g. msys._datasets.gfilter('SYS1.**').acl(resolve=True, allows='UPDATE', sort="user")
         pd.core.base.PandasObject.gfilter = RACF.gfilter
         pd.core.base.PandasObject.rfilter = RACF.rfilter
 
 
         # set consistent index columns for existing dfs: profile key, connect group+user, of profile class+key (for G.R.)
         for (rtype,rinfo) in RACF._recordtype_info.items():
             if rtype in thingswewant and rtype in self._records and self._records[rtype]['parsed']>0:
@@ -351,15 +381,15 @@
                 getattr(self,rinfo['df']).set_index(keys,drop=False,inplace=True)
                 getattr(self,rinfo['df']).rename_axis(names,inplace=True)  # prevent ambiguous index / column names 
         
         # copy group auth (USE,CREATE,CONNECT,JOIN) to complete the connectData list, using index alignment
         if self.parsed("GPMEM") == 0 or self.parsed("USCON") == 0:
             raise StoopidException("Need to parse GPMEM and USCON first...")
         else: 
-            self.connectData["GPMEM_AUTH"]=self.connects["GPMEM_AUTH"]
+            self._connectData["GPMEM_AUTH"] = self._connects["GPMEM_AUTH"]
         
         self._connectByUser = self._connectData.set_index("USCON_NAME",drop=False).rename_axis('NAME')
         self._connectByGroup = self._connectData.set_index("USCON_GRP_ID",drop=False).rename_axis('GRP_ID')
             
         # dicts containing lists of groups for printing group structure
         self._ownertree = self.ownertree()
         self._grouptree = self.grouptree()
@@ -437,124 +467,98 @@
 
 
     def giveMeProfiles(self, df, selection=None, option=None):
         ''' Search profiles using the index fields.  selection can be str or tuple.  Tuples check for group + user id in connects, or class + profile key in generals.
         option controls how selection is interpreted, and how data must be returned:
         None is for (expensive) backward compatibility, returns a df with 1 profile.
         LIST returns a series for 1 profile, much faster and easier to process.
-        REGEX returns a df for profile matching selection, starting at beginning of profile name, (general) class, or class+profile, (connect) group, or group+user ID.
-        GENERIC takes the generic pattern for the selection, turns it into regex, and returns a df.
         '''
         if not selection:
             raise StoopidException('profile criteria not specified...')
         if option in (None,'LIST','L'):  # return 1 profile
             # 1 string, several strings in a tuple, or a mix of strings and None, but the latter must be tested with get_level_values
             if type(selection)==str: pass
             elif type(selection)==tuple:
                 selections = len(selection)
-                strings = [type(selection[i])==str for i in range(selections)]
+                strings = [type(selection[i])==str and selection[i]!='**' for i in range(selections)]
                 if all(strings): pass
                 else:
-                    found = False
-                    for i in range(selections):
-                        if all(strings[0:i]) and not any(strings[i+1:]):
-                            if i==0:
-                                selection = selection[0]
-                            else:    
-                                selection = tuple(selection[j] for j in range(i+1))
-                            found = True
-                            break
-                    if not found:
-                        locs = True
-                        for s in range(selections):
-                            if selection[s] not in (None,'**'):
-                                locs &= (df.index.get_level_values(s)==selection[s])
-                        selection = locs
+                    locs = pd.array([True]*df.shape[0], dtype="boolean")
+                    for s in range(selections):
+                        if selection[s] not in (None,'**'):
+                            locs &= (df.index.get_level_values(s)==selection[s])
+                    selection = locs
             else:
                 raise StoopidException(f'specify patterns for profile, (group,userid) or (class,profile), not {selection}')
-            if option == None:  # return DataFrame for 1 profile
+            if option == None and type(selection) in (str,tuple):  # return DataFrame for 1 profile
                 try:
                     return df.loc[[selection]]
                 except KeyError:
                     return pd.DataFrame()
-            elif option in ('LIST','L'):  # return Series for 1 profile
+            else:  # return Series for 1 profile, or use loc[array]
                 try:
                     return df.loc[selection]
                 except KeyError:
                     return []
-        elif option in ('REGEX','R','GENERIC','GEN','G'):
-            if type(selection)==str:
-                return df.loc[df.index.get_level_values(0).str.match(selection if option in ('REGEX','R') else RACF.generic2regex(selection))]
-            elif type(selection)==tuple:
-                locs = True
-                for s in range(len(selection)):
-                    if selection[s] not in (None,'**'):
-                        locs &= (df.index.get_level_values(s).str.match(selection[s] if option in ('REGEX','R') else RACF.generic2regex(selection[s])))
-                return df.loc[locs]
-            else:
-                raise StoopidException(f'specify patterns for profile, (group,userid) or (class,profile), not {selection}')
         else:
             raise StoopidException(f'unexpected last parameter {option}')
 
+
     def gfilter(df, *selection):
         ''' Search profiles using GENERIC pattern on the index fields.  selection can be one or more values, corresponding to index levels of the df '''
-        locs = True
+        locs = pd.array([True]*df.shape[0], dtype="boolean")
         for s in range(len(selection)):
             if selection[s] not in (None,'**'):
                 locs &= (df.index.get_level_values(s).str.match(RACF.generic2regex(selection[s])))
         return df.loc[locs]
 
     def rfilter(df, *selection):
         ''' Search profiles using refex on the index fields.  selection can be one or more values, corresponding to index levels of the df '''
-        locs = True
+        locs = pd.array([True]*df.shape[0], dtype="boolean")
         for s in range(len(selection)):
             if selection[s] not in (None,'**','.*'):
                 locs &= (df.index.get_level_values(s).str.match(selection[s]))
         return df.loc[locs]
 
-
-
+    # user frames
 
     @property
     def users(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         try:
             return self._users
         except:
             raise StoopidException('No USBD records parsed!')
     
     def user(self, userid=None, pattern=None):
         return self.giveMeProfiles(self._users, userid, pattern)
 
-    def OLDuser(self, userid=None):
-        if not userid:
-            raise StoopidException('userid not specified...')
-        try:
-            return self._users.loc[[userid]]
-        except:
-            return []
-        # return self._users.loc[self._users.USBD_NAME==userid]
-
 
     @property
     def connectData(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._connectData
         
     def connect(self, group=None, userid=None, pattern=None):
         return self.giveMeProfiles(self._connectData, (group,userid), pattern)
 
 
     @property
-    def userDistributedMapping(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._userDistributedMapping
+    def userUSRDATA(self):
+        return self._userUSRDATA
+
+    installdata = property(deprecated(userUSRDATA,"installdata"))
+
+    @property
+    def userDistributedIdMapping(self):
+        return self._userDistributedIdMapping
+
+    userDistributedMapping = property(deprecated(userDistributedIdMapping,"userDistributedMapping"))
 
 
     @property
     def specials(self):
         return self._users.loc[self._users['USBD_SPECIAL'] == 'YES']
 
     @property
@@ -565,37 +569,31 @@
     def auditors(self):
         return self._users.loc[self._users['USBD_AUDITOR'] == 'YES']
 
     @property
     def revoked(self):
         return self._users.loc[self._users['USBD_REVOKE'] == 'YES']
 
+
+    # group frames
+
     @property
     def groups(self, query=None):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._groups
     
     def group(self, group=None, pattern=None):
         return self.giveMeProfiles(self._groups, group, pattern)
 
-    def OLDgroup(self, group=None):
-        if not group:
-            raise StoopidException('group not specified...')
-        try:
-            return self._groups.loc[[group]]
-        except:
-            return []
-        # return self._groups.loc[self._groups.GPBD_NAME==group]
-
     @property
     def groupsWithoutUsers(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._groups.loc[-self.groups.GPBD_NAME.isin(self._connectData.USCON_GRP_ID)]
+        return self._groups.loc[~self.groups.GPBD_NAME.isin(self._connectData.USCON_GRP_ID)]
     
     @property
     def groupConnect(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._groupConnect
 
@@ -607,37 +605,16 @@
 
     @property
     def subgroups(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._subgroups
 
-    @property
-    def installdata(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._userUSRDATA
-
-    @property
-    def userOMVS(self, query=None):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._userOMVS
-
-    @property
-    def groupOMVS(self, query=None):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._groupOMVS        
 
-    @property
-    def userTSO(self, query=None):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._userTSO    
+    # dataset frames
         
     @property
     def datasets(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._datasets
 
@@ -661,14 +638,26 @@
 
     def datasetPermit(self, profile=None, id=None, access=None, pattern=None):
         return self.giveMeProfiles(self._datasetAccess, (profile,id,access), pattern)
 
     @property
     def uacc_read_datasets(self):
         return self._datasets.loc[self._datasets.DSBD_UACC=="READ"]
+    @property
+    def uacc_update_datasets(self):
+        return self._datasets.loc[self._datasets.DSBD_UACC=="UPDATE"]
+    @property
+    def uacc_control_datasets(self):
+        return self._datasets.loc[self._datasets.DSBD_UACC=="CONTROL"]
+    @property
+    def uacc_alter_datasets(self):
+        return self._datasets.loc[self._datasets.DSBD_UACC=="ALTER"]
+
+
+    # general resource frames
 
     @property
     def generals(self, query=None):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generals
 
@@ -704,14 +693,20 @@
         return self._generalConditionalAccess
 
     genericConditionalAccess = property(deprecated(generalConditionalAccess,"genericConditionalAccess"))
     
     def generalConditionalPermit(self, resclass=None, profile=None, id=None, access=None, pattern=None):
         return self.giveMeProfiles(self._generalConditionalAccess, (resclass,profile,id,access), pattern)
 
+    @property
+    def SSIGNON(self): # GRSIGN
+        return self._generalSSIGNON.join(self._generals['GRBD_APPL_DATA'])
+
+
+
     def rankedAccess(args):
         ''' translate access levels into integers, add 10 if permit is for the user ID. 
         could be used in .apply() but would be called for each row, so very very slow '''
         (userid,authid,access) = args
         accessNum = RACF.accessKeywords.index(access)
         return accessNum+10 if userid==authid else accessNum
 
@@ -865,109 +860,14 @@
         if access:
             acl = acl.loc[acl["ACCESS"].map(RACF.accessKeywords.index)==RACF.accessKeywords.index(access.upper())]
         if allows:
             acl = acl.loc[acl["ACCESS"].map(RACF.accessKeywords.index)>=RACF.accessKeywords.index(allows.upper())]
         return acl.sort_values(by=sortBy[sort])[tbProfileKeys+returnFields].reset_index(drop=True)
 
     
-    def verify(self, rules=None, domains=None, module=".profileFieldRules"):
-        ''' verify fields in profiles against the expected value, issues are returned in a df
-        rules can be passed as a list of tuples, or dict via parameter, or as function result from external module.
-        '''
-        
-        if not(rules and domains):
-            ruleset = importlib.import_module(module, package="pyracf")
-            ruleset = importlib.reload(ruleset)
-            if not rules:
-                rules = ruleset.rules(self)
-            if not domains:
-                domains = ruleset.domains(self,pd)  # needs pandas
-
-        if type(rules)==str:
-            rules= yaml.safe_load(rules)
-
-        def listMe(item):
-            ''' make list in parameters optional when there is only 1 item '''
-            return item if type(item)==list else [item]
-        
-        brokenSum = pd.DataFrame(columns=['CLASS','PROFILE','FIELD_NAME','EXPECT','VALUE'])
-        for (tbNames,*tbCriteria) in rules:
-            for tbName in listMe(tbNames):
-                dfName = RACF._recordname_df[tbName]
-                if hasattr(self,dfName):
-                    tbDF = getattr(self,dfName)
-                    if tbDF.empty:
-                      continue
-                else:
-                    continue
-                tbEntity = tbName[0:2]
-                tbClassName = {'DS':'dataset', 'GP':'group', 'GR':'general', 'US':'user'}[tbEntity]
-                ixLevel = 1 if tbEntity=='GR' else 0  # GR has CLASS before NAME in the index
-
-                for tbCrit in tbCriteria:
-                    locs = True
-                    matchPattern = None
-                    if 'class' in tbCrit:
-                        if tbEntity!='GR':
-                            print('only for GR')
-                        classPattern = ''
-                        for cl in listMe(tbCrit['class']):
-                            classPattern += RACF.generic2regex(cl) + "|"
-                        locs &= tbDF.index.get_level_values(0).str.match(classPattern[:-1])
-                    if '-class' in tbCrit:
-                        if tbEntity=='GR':
-                            classPattern = ''
-                            for cl in listMe(tbCrit['-class']):
-                                classPattern += RACF.generic2regex(cl) + "|"
-                            locs &= ~ tbDF.index.get_level_values(0).str.match(classPattern[:-1])
-                    if 'profile' in tbCrit:
-                        locs &= tbDF.index.get_level_values(ixLevel).str.match(RACF.generic2regex(tbCrit['profile']))
-                    if '-profile' in tbCrit:
-                        locs &= ~ tbDF.index.get_level_values(ixLevel).str.match(RACF.generic2regex(tbCrit['-profile']))
-                    if 'match' in tbCrit:
-                        matchPattern = tbCrit['match'].replace('.','\.').replace('*','\*')\
-                                                      .replace('(','(?P<').replace(')','>[^.]*)')
-                        matched = tbDF[tbName+'_NAME'].str.extract(matchPattern)
-                    for fldCrit in listMe(tbCrit['field']):
-                        fldName = fldCrit['name'] if matchPattern else tbName+'_'+fldCrit['name']
-                        fldExpect = fldCrit['expect'] if 'expect' in fldCrit else None
-                        if matchPattern:
-                            for fn in matched.columns:
-                                if fn==fldName:
-                                    if fldExpect:
-                                        locs &= matched[fn].gt('') & - matched[fn].isin(domains[fldExpect])
-                                    if 'or' in fldCrit:
-                                        locs &= ~ matched[fn].isin(listMe(fldCrit['or']))
-                        else:
-                            if fldExpect:
-                                locs &= tbDF[fldName].gt('') & - tbDF[fldName].isin(domains[fldExpect])
-                            if 'or' in fldCrit:
-                                locs &= ~ tbDF[fldName].isin(listMe(fldCrit['or']))
-                        if any(locs):
-                            broken = tbDF.loc[locs].copy()
-                            broken['CLASS'] = broken[tbName+'_CLASS_NAME'] if tbEntity=='GR' else tbClassName
-                            broken['PROFILE'] = broken[tbName+'_NAME']
-                            broken['FIELD_NAME'] = fldName
-                            broken['EXPECT'] = fldExpect
-                            broken['VALUE'] = matched[fldName] if matchPattern else broken[fldName]
-                            brokenSum = pd.concat([brokenSum,broken[brokenSum.columns]],
-                                                   sort=False, ignore_index=True)
-        return brokenSum        
-    
-
-    @property
-    def neworphans(self):
-        return self.verify(
-            rules = [
-                (['DSACC','DSCACC','GRACC','GRCACC'],
-                 {'field': {'name':'AUTH_ID', 'expect':'ACLID'}})
-            ]
-        )
-
-
     @property
     def orphans(self):
         
         if self.parsed("DSACC") + self.parsed("GRACC") == 0:
             raise StoopidException('No dataset/general access records parsed! (PEBKAM/ID-10T error)')
             
         datasetOrphans = None
@@ -1106,15 +1006,15 @@
 
         writer.close()   
 
     def tree(self,linkup_field="GPBD_SUPGRP_ID"):
         # get all owners... (group or user) or all superior groups
         tree = {}
         where_is = {}
-        higher_ups = self.groups.groupby(linkup_field)
+        higher_ups = self._groups.groupby(linkup_field)
         for higher_up in higher_ups.groups.keys():
             if higher_up not in tree:
                 tree[higher_up] = []
                 for group in higher_ups.get_group(higher_up)['GPBD_NAME'].values:
                     tree[higher_up].append(group)
                     where_is[group] = tree[higher_up]
         # initially, for an owner tree, anchor can be a user (like IBMUSER) or a group
@@ -1174,34 +1074,34 @@
             if access in peraccess.groups.keys():
                 a = peraccess.get_group(access)['DSACC_AUTH_ID'].values
                 for id in a:
                     if id in self.users.index:
                         accesslist[access].append(id)
                     else:
                         if id in self.groups.index:
-                            g = self.connectData.loc[id][['USCON_NAME','USCON_GRP_SPECIAL']].values
+                            g = self.connect(id)[['USCON_NAME','USCON_GRP_SPECIAL']].values
                             for user,grp_special in g:
                                 accesslist[access].append(user)
                                 # But suppose this user is group_special here?
                                 if grp_special=='YES':
                                     accessmanagers[access].append(user)
                             # And wait a minute... this groups owner, can also add people to the group?
                             [gowner,gsupgroup] = self.group(id)[['GPBD_OWNER_ID','GPBD_SUPGRP_ID']].values[0]
                             if gowner in self.users.index:
                                 accessmanagers[access].append(gowner)
                             else:
                                 # group special propages up
                                 while gowner==gsupgroup:
-                                    g = self.connectData.loc[gowner][['USCON_NAME','USCON_GRP_SPECIAL']].values
+                                    g = self.connect(gowner)[['USCON_NAME','USCON_GRP_SPECIAL']].values
                                     for user,grp_special in g:
                                         if grp_special=='YES':
                                             accessmanagers[access].append(user)
                                     [gowner,gsupgroup] = self.group(gowner)[['GPBD_OWNER_ID','GPBD_SUPGRP_ID']].values[0]
                             # connect authority CONNECT/JOIN allows modification of member list
-                            g = self.connects.loc[id][['GPMEM_MEMBER_ID','GPMEM_AUTH']].values
+                            g = self.connect(id)[['USCON_NAME','GPMEM_AUTH']].values
                             for user,grp_auth in g:
                                 if grp_auth in ('CONNECT','JOIN'):
                                     accessmanagers[access].append(user)
                 # clean up doubles...
                 accesslist[access] = list(set(accesslist[access]))
                 accessmanagers[access] = list(set(accessmanagers[access]))
```

### Comparing `pyracf-0.7.1/src/pyracf/getOffsets.py` & `pyracf-0.8.2/src/pyracf/getOffsets.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.7.1/src/pyracf/offsets.json` & `pyracf-0.8.2/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.7.1/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.8.2/src/pyracf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.7.1
+Version: 0.8.2
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -29,14 +29,28 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.2 (property for most application segments)
+- application segments for dataset, group and user entities are avaible with entity prefix, e.g., msys.userTSO, msys.datasetDFP, msys.groupOMVS
+- system related application segments from general resources are published without prefix, e.g., msys.STDATA or msys.MFA
+- old properties msys.installdata and msys.userDistributedMappings are replaced by userUSRDATA and userDistributedIdMappings
+- most of these properties are automatically generated
+
+### 0.8.0 (acl, gfilter, rfilter methods)
+- selection method gfilter (supports RACF generic patterns) and rfilter (for regex patterns)
+  supports as many parameters as there are index columns in the frame
+- reporting method acl, produces frame with access list, may be used on the entity frames or on the access frames
+- internal frames _connectByGroup and _connectByUser, as alternate index on connectData
+- internal frames _grouptreeLines and _ownertreeLines that return all groups up until SYS1 (or upto a user ID)
+- correlate() invoked automatically by parse() and fancycli()
+
 ### 0.7.1 (General instead of Generic)
 - fixed: Generic should be General resource profiles, variables and methods renamed
 - Mapping between IRRDBU00 record types and variables centralized in a dict
 - global constants related to record types removed
 - parsed records internally stored by (decimal) record type, instead of by name
 - add method to retrieve parsed record count for given name
 - _offsets now a RACF class attribute
@@ -44,18 +58,20 @@
 - fixed: status property crashed when used before parse() method used, math.floor call is now conditional
 - fixed: record type '0260' in offset.json was malformed
 - updated offsets.json from https://www.ibm.com/docs/en/SSLTBW_3.1.0/com.ibm.zos.v3r1.icha300/format.htm etc
 - getOffsets.py to update the json model
 - fixed: RACF documentation contains incorrect record type 05k0
 - all known record types parsed and loaded into DataFrames
 - index columns assigned to all DataFrames, assigned by new correlate() method
-- new method correlate() to increase speed of subsequent data access, use after parse() or loading of pickles
-- selection and reporting methods dataset(), group(), general(), user() and connect(), accepts GENERIC and regex patterns 
-- also datasetPermit and datasetConditionalPermit, with parameters profile(mask), id(mask) and access(mask) 
-- also generalPermit and generalConditionalPermit, with parameters resclass(mask), profile(mask), id(mask) and access(mask)
+- new method correlate() to increase speed of subsequent data access, used after parse() or loading of pickles
+- new selection methods similar to user() and group(), that work on index fields.
+    when a parameter is given as None or '**', elements matching the other parameters are returned:
+    datasetPermit and datasetConditionalPermit, with parameters profile(), id() and access() 
+    generalPermit and generalConditionalPermit, with parameters resclass(), profile(), id() and access()
+    connect with parameters group() and user()
 - added GPMEM_AUTH to connectData frame, consolidating all connect info into one line 
 
 ### 0.6.4 (Add 0209)
 - Added 0209 recordtype to parser. (userDistributedMapping)
 
 ### 0.6.3 (Add fields)
 - Added missing USBD_LEG_PWDHIST_CT, USBD_XPW_PWDHIST_CT, USBD_PHR_ALG, USBD_LEG_PHRHIST_CT, USBD_XPW_PHRHIST_CT, USBD_ROAUDIT and USBD_MFA_FALLBACK to Users dataframe
@@ -122,105 +138,109 @@
 Then later, you don't need to parse the same unload again, just do:
 
     >>> from pyracf import RACF
     >>> mysys = RACF(pickles='/tmp/pickles', prefix='mysys-')
     >>> hash(mysys.groups.values.tobytes())
     -8566685915584060910
 
-### Prepare internal data structures for later processing
-
-    >>> mysys.correlate()
 
 ## All functions
 
 | Function/Property | Explanation | Example |
 |---|---|---|
+| acl | Returns DataFrame with access control list for the given frame | msys.datasets.acl(permits=True, explode=False, resolve=False, admin=False, access=None, allows=None, sort="profile")
 | auditors | Returns DataFrame with all user having the auditor bit switched on | mysys.auditors |
-| connect | Returns DataFrame with selected user to group connects | mysys.connect('SYS1',None,'G') or mysys.connect('**','IBM*','G') |
-| connects | Returns DataFrame with all user to group connects | mysys.connects |
+| connect | Returns DataFrame with selected user to group connects | mysys.connect('SYS1',None) or mysys.connect('**','IBMUSER') |
+| connects | Returns DataFrame with all user to group connects, use connect or connectData instead | mysys.connects |
+| connectData | Returns DataFrame with all user to group connect information | mysys.connectData |
 | correlate | assigns index columns and prepares data structures for faster reporting | mysys.correlate() |
 | datasetAccess | Returns DataFrame with all Accesslists for all dataset profiles | mysys.datasetsAccess |
-| dataset | Returns DataFrame with selected datasetprofiles | mysys.dataset('SYS1.**','GEN') |
-| datasetPermit | Returns DataFrame with selected permits on datasetprofiles | mysys.datasetPermit(profile=, id=, access=, pattern='G') |
-| datasetConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on datasetprofiles | mysys.datasetConditionalPermit(profile=, id=, access=, pattern='G') |
+| dataset | Returns DataFrame with selected datasetprofiles | mysys.dataset('SYS1.**') |
+| datasetPermit | Returns DataFrame with selected permits on datasetprofiles | mysys.datasetPermit(profile=, id=, access=) |
+| datasetConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on datasetprofiles | mysys.datasetConditionalPermit(profile=, id=, access=) |
 | datasets | Returns DataFrame with all datasetprofiles | mysys.datasets |
 | generalAccess | Returns DataFrame with with all accesslists for general resource profiles | mysys.generalAccess
 | generalConditionalAccess | Returns DataFrame with with all conditional accesslists for general resource profiles | mysys.generalConditionalAccess
-| general | Returns DataFrame with selected general resource profiles | mysys.general('FACI*','BPX.**','GEN') |
-| generalPermit | Returns DataFrame with selected permits on resource profiles | mysys.generalPermit(resclass=, profile=, id=, access=, pattern='G') |
-| generalConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on resource profiles | mysys.generalConditionalPermit(resclass=, profile=, id=, access=, pattern='G') |
+| general | Returns DataFrame with selected general resource profiles | mysys.general(reclass=, profile=) |
+| generalPermit | Returns DataFrame with selected permits on resource profiles | mysys.generalPermit(resclass=, profile=, id=, access=) |
+| generalConditionalPermit | Returns DataFrame with selected "PERMIT WHEN()" on resource profiles | mysys.generalConditionalPermit(resclass=, profile=, id=, access=) |
 | generals | Returns DataFrame with with all general resource profiles | mysys.generals 
 | getdatasetrisk | Returns dict with users that have access or administrative authority on a profile | mysys.getdatasetrisk('SYS1.**') |
-| group | Returns DataFrame with with group profiles matching selection | mysys.group('SYS1'), or msys.group('SYS*','G') |
-| groupConnect | Returns DataFrame with with user group connection records (0203 recordtype) | mysys.groupConnect |
+| gfilter | Returns DataFrame with records matching the index fields specified, using RACF generic patterns | mysys.datasets.gfilter('SYS%.**')) or mysys.generals.gfilter('FACI*','BPX.**'))|
+| group | Returns DataFrame with group profiles matching selection | mysys.group('SYS1') |
+| groupConnect | Returns DataFrame with with user group connection records (0203 recordtype), use connect or connectData instead | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | groupsWithoutUsers | Returns DataFrame with groups that have no connected users | mysys.groupsWithoutUsers |
 | grouptree | Returns dict with groups arranged by superior group | mysys.grouptree() |
 | installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for general resources | d, g = mysys.orphans |
 | ownertree | Returns dict with groups arranged by owner group or user ID | mysys.ownertree() |
 | parse | parses the unload. optional specify recordtypes | mysys.parse(recordtypes=['0200']) |
 | parse_fancycli | parses the unload with a fancy cli status update. optional recordtypes can be specified | mysys.parse_fancycli(recorddtypes=['0200']) |
 | revoked | Returns a DataFrame  with all revoked users | mysys.revoked |
+| rfilter | Returns DataFrame with records matching the index fields specified, using regex patterns | mysys.generals.rfilter('FAC.*','BPX\..*')) |
 | save_pickles | Saves all parsed types as pickle files | mysys.save_pickles(path='/tmp', prefix='mysys-') |
 | specials | Returns a DataFrame  with all special users | mysys.specials |
 | status | Returns JSON with parsing status | mysys.status |
 | uacc_read_datasets | Returns a DataFrame  with all dataset profiles having UACC=READ | mysys.uacc_read_datasets |
-| user | Returns DataFrame with with user profiles matching selection | mysys.user('IBM*'), or msys.user('SYS.*','REGEX') |
+| uacc_update_datasets | Returns a DataFrame  with all dataset profiles having UACC=UPDATE | mysys.uacc_update_datasets |
+| user | Returns DataFrame with with user profiles matching selection | mysys.user('IBMUSER') |
 | users | Returns DataFrame with all user base data | mysys.users |
 | xls | Creates an XLSX with all permits per class | mysys.xls(fileName='myxls.xlsx') |
 
 # Example use-case
 
 Get all users that have not logged in (on?) since January 1st 2022. And print userID and last logon...
 
     import time
     from pyracf import IRRDBU
 
     mysys = IRRDBU('/path/to/irrdbu00')
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
-    mysys.correlate()
     selection = mysys.users.loc[mysys.users.USBD_LASTJOB_DATE<="2022-01-01"][['USBD_NAME','USBD_LASTJOB_DATE']]
     for user in selection.values:
       print(f"Userid {user[0]}, last active: {user[1]}")
 
 Create a neat XLSX
 
     import time
     from pyracf import IRRDBU
     mysys = IRRDBU('/path/to/irrdbu00')
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
-    mysys.correlate()
     mysys.xls('/path/to/my.xlsx')
 
 Print z/OS UNIX profiles
 
-    mysys.correlate()
-    mysys.general('FAC*', 'BPX.**', 'G')
-    mysys.general('UNIXPRIV', '**', 'G') # print all in UNIXPRIV
+    mysys.generals.gfilter('FAC*', 'BPX.**')
+    mysys.generals.gfilter('UNIXPRIV') # print all in UNIXPRIV
 
 Show group information
 
-    mysys.correlate()
-    mysys.connect('SYS*', None, 'G')    # users connected to SYSxxxxx groups
-    mysys.general('**', 'IBMUSER', 'G') # connects of user IBMUSER
-    mysys.general(user='IBMUSER', pattern='G') # connects of user IBMUSER
+    mysys.connect('SYS1')            # users connected to SYS1 groups
+    mysys.connect('**','IBMUSER')    # groups IBMUSER is connected to
+    mysys.connectData.gfilter('SYS*','IBM*') # connects using patterns
+    mysys.connectData.rfilter('SYS[AB].*','PROD.*') # regex with alternatives
+    mysys.connectData.query("USCON_GRP_SPECIAL=='YES' & USCON_REVOKE=='YES'")  # group special revoked
+    mysys.connectData.query("GPMEM_AUTH==['CONNECT','JOIN']")  # users with connect authorities
 
 Show access list information
 
-    mysys.correlate()
     mysys.datasetPermit('SYS1.**')    # IDs permitted on SYS1.**
-    mysys.datasetPermit(id='IBMUSER', pattern='GENERIC')    # where is IBMUSER permitted
-    mysys.datasetPermit('SYS1.**', access='ALTER', pattern='G')    # IDs ALTER access on any SYS1 dataset profile
-    mysys.generalPermit('XFAC*', 'CKR.**', pattern='G') # permits on zSecure Admin/Audit profile
+    mysys.datasetPermit(id='IBMUSER', access='ALTER')    # where is IBMUSER permitted
+
+    mysys.datasets.gfilter('SYS1.**').acl(access='ALTER')    # IDs ALTER access on any SYS1 dataset profile
+    mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE')    # IDs with access that allows UPDATE
+    mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE', resolve=True)    # groups and user permits combined 
+    mysys.datasets.gfilter('PROD.**').acl(permits=False, admin=True)    # who can change groups or profiles to change access on PROD data sets
+    mysys.generals.gfilter('XFAC*', 'CKR.**').acl() # permits on zSecure Admin/Audit profile
 
 
 # Updates 
 
 In this version we introduced IRRRDBU as an alternative to RACF. Examples have been updated. The RACF class from previous version is still available, but you're advised to change this to IRRDBU, as future version will have another user of the RACF class.
 
 # Contribute to PyRACF
```

