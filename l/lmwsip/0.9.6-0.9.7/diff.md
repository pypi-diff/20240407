# Comparing `tmp/lmwsip-0.9.6.tar.gz` & `tmp/lmwsip-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmwsip-0.9.6.tar", last modified: Wed Nov  2 09:58:43 2022, max compression
+gzip compressed data, was "lmwsip-0.9.7.tar", last modified: Sun Apr  7 21:03:48 2024, max compression
```

## Comparing `lmwsip-0.9.6.tar` & `lmwsip-0.9.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dronerun   (801) dronerun   (801)        0 2022-11-02 09:58:43.698998 lmwsip-0.9.6/
--rw-r--r--   0 dronerun   (801) dronerun   (801)     1060 2022-11-02 09:58:39.000000 lmwsip-0.9.6/LICENSE
--rw-r--r--   0 dronerun   (801) dronerun   (801)     2359 2022-11-02 09:58:43.698998 lmwsip-0.9.6/PKG-INFO
--rw-r--r--   0 dronerun   (801) dronerun   (801)     1888 2022-11-02 09:58:39.000000 lmwsip-0.9.6/README.md
--rw-r--r--   0 dronerun   (801) dronerun   (801)      104 2022-11-02 09:58:39.000000 lmwsip-0.9.6/pyproject.toml
--rw-r--r--   0 dronerun   (801) dronerun   (801)      618 2022-11-02 09:58:43.699998 lmwsip-0.9.6/setup.cfg
--rw-r--r--   0 dronerun   (801) dronerun   (801)       69 2022-11-02 09:58:39.000000 lmwsip-0.9.6/setup.py
-drwxr-xr-x   0 dronerun   (801) dronerun   (801)        0 2022-11-02 09:58:43.697998 lmwsip-0.9.6/src/
-drwxr-xr-x   0 dronerun   (801) dronerun   (801)        0 2022-11-02 09:58:43.698998 lmwsip-0.9.6/src/lmwsip/
--rw-r--r--   0 dronerun   (801) dronerun   (801)    34675 2022-11-02 09:58:39.000000 lmwsip-0.9.6/src/lmwsip/__init__.py
--rwxr-xr-x   0 dronerun   (801) dronerun   (801)     2462 2022-11-02 09:58:39.000000 lmwsip-0.9.6/src/lmwsip/run.py
-drwxr-xr-x   0 dronerun   (801) dronerun   (801)        0 2022-11-02 09:58:43.698998 lmwsip-0.9.6/src/lmwsip.egg-info/
--rw-r--r--   0 dronerun   (801) dronerun   (801)     2359 2022-11-02 09:58:43.000000 lmwsip-0.9.6/src/lmwsip.egg-info/PKG-INFO
--rw-r--r--   0 dronerun   (801) dronerun   (801)      261 2022-11-02 09:58:43.000000 lmwsip-0.9.6/src/lmwsip.egg-info/SOURCES.txt
--rw-r--r--   0 dronerun   (801) dronerun   (801)        1 2022-11-02 09:58:43.000000 lmwsip-0.9.6/src/lmwsip.egg-info/dependency_links.txt
--rw-r--r--   0 dronerun   (801) dronerun   (801)       16 2022-11-02 09:58:43.000000 lmwsip-0.9.6/src/lmwsip.egg-info/requires.txt
--rw-r--r--   0 dronerun   (801) dronerun   (801)        7 2022-11-02 09:58:43.000000 lmwsip-0.9.6/src/lmwsip.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 21:03:48.644086 lmwsip-0.9.7/
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-07 21:03:44.000000 lmwsip-0.9.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-07 21:03:48.644086 lmwsip-0.9.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-07 21:03:44.000000 lmwsip-0.9.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-07 21:03:44.000000 lmwsip-0.9.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      618 2024-04-07 21:03:48.644086 lmwsip-0.9.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-07 21:03:44.000000 lmwsip-0.9.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 21:03:48.641086 lmwsip-0.9.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 21:03:48.643086 lmwsip-0.9.7/src/lmwsip/
+-rw-r--r--   0 root         (0) root         (0)    35613 2024-04-07 21:03:44.000000 lmwsip-0.9.7/src/lmwsip/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2462 2024-04-07 21:03:44.000000 lmwsip-0.9.7/src/lmwsip/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 21:03:48.644086 lmwsip-0.9.7/src/lmwsip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/top_level.txt
```

### Comparing `lmwsip-0.9.6/LICENSE` & `lmwsip-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lmwsip-0.9.6/PKG-INFO` & `lmwsip-0.9.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: lmwsip
-Version: 0.9.6
+Version: 0.9.7
 Summary: Interface for the lmw sip protocol
 Home-page: https://git.marceln.org/Werk/lmwsip
 Author: Marcel Nijenhof
 Author-email: pypi@marceln.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
 
 # lmwsip
 ## Introduction
 
 lmwsip is a python library for the lmw sip protocol.
 
 ## Package
```

### Comparing `lmwsip-0.9.6/README.md` & `lmwsip-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `lmwsip-0.9.6/setup.cfg` & `lmwsip-0.9.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmwsip
-version = 0.9.6
+version = 0.9.7
 author = Marcel Nijenhof
 author_email = pypi@marceln.org
 description = Interface for the lmw sip protocol
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://git.marceln.org/Werk/lmwsip
 classifiers =
```

### Comparing `lmwsip-0.9.6/src/lmwsip/__init__.py` & `lmwsip-0.9.7/src/lmwsip/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,35 @@
 import time
 import re
 import logging
 from datetime import datetime, timedelta
 from dateutil import tz
 
 """ Version info changed by git hook """
-__version__ = '0.9.6'
+__version__ = '0.9.7'
 
 class LmwSip:
     """Class to connect to the LMW Standard Interface prototcol (sip)
     
 This class iplement connection to the Rijkswaterstaat Meetnet
 Water (LMW) with the Standard Interface Protocol using the
 Rijkswaterstaat Meetnet Infrastructuur (RMI).
 
 https://waterberichtgeving.rws.nl/water-en-weer/metingen
 
 Support for:
     ti
     cmd(wn, vw, as)
 
+lmwParameters:
+ - Type: WN, VW, AS
+ - Array size: [1-201]
+ - Periode: 1, 10
 """
+
     lmwParameters = {
         'Tm02_MV': ('VW', 1, 0),
         'xH1': ('WN', 1, 1),
         'HH1S': ('WN', 1, 1),
         'SRV1': ('WN', 1, 1),
         'TL1': ('WN', 1, 1),
         'SRV1w1': ('WN', 1, 1),
@@ -589,15 +594,15 @@
            # At the moment no support for parameters other than 1 or 10 minutes.
            raise LmwParmWarn(parameter)
         time_of_day=time.strftime("%H:%M", time.gmtime(now))
         return { "day": time.strftime("%d-%m-%Y", time.gmtime(now)),
                  "time_of_day": time.strftime("%H:%M", time.gmtime(now)) }
 
     def connect(self):
-        """connect()
+        """Setup the network connection
 
 connects to lmw with tcp using the values of the object creation.
 """
         try:
             self._tcp         = socket.create_connection((self.host, self.port))
             self._connecttime = time.time()
         except Exception as e:
@@ -625,15 +630,15 @@
             self.log.debug("LmwSip.closesocket")
             self._socket.close()
         except Exception as e:
             pass
         self._socket = None
 
     def send(self, sipcmd):
-        """send(sipcmd)
+        """Send a sip command to the server
 
 send a sip command to the server
 """
         self._idletime = time.time()
         if self._socket != None:
             try:
                 logcmd = sipcmd.strip('\r')
@@ -655,15 +660,15 @@
             self._socket.sendall(a)
         except Exception as e:
             self.log.error("LmwSip.telnetheader(%s) --> %s failed: %s" % (header, a, e))
             self.closesocket()
             raise LmwSipConnectError("LmwSip.telnetheader: Socket connection lost")
 
     def recv(self):
-        """recv()
+        """Recieve the results
 
 recieve a answer from the sip server
 """
         c = 0
         bytebuf=b''
         stringbuf=""
         while (self._socket != None) and (stringbuf.find("\r") == -1) and (c < 3):
@@ -698,15 +703,15 @@
         elif stringbuf[0] != '!':
             self.log.warning("LmwSip.recv: Sip error: %s" % stringbuf.strip('\r'))
         else:
             self.log.debug("LmwSip.recv: result: %s" % stringbuf.strip('\r'))
         return(stringbuf)
 
     def login(self):
-        """login()
+        """Login the sip server
 
 Login lmw using the object creation user, password.
 Raises a LmwLoginFailure exception on failure
 """
         li="LI " + self.user + ","  + self.password + "\r"
         #
         # TODO: Check connect
@@ -722,15 +727,15 @@
     def reconnect(self):
         self.logout()
         time.sleep(1)
         self.connect()
         self.login()
 
     def reconnectcheck(self):
-        """reconnectcheck()
+        """Check if we need to reconnect.
 
 Checks if a reconnect is nessecery.
 
 There are two timeouts:
     The maxium connect time (reconnecttime)
     The maxium idle time (idlereconnect)
 """
@@ -740,15 +745,15 @@
             self.reconnect()
         it = time.time() - self._idletime
         if (self.idlereconnect > 0) and (it > self.idlereconnect):
             self.log.debug("LmwSip.reconnectcheck: idle reconnect after %i seconds" % it)
             self.reconnect()
 
     def sendrecv(self, cmd):
-        """sendrecv(cmd)
+        """Send a a command and recieve the result.
 
 send the command and recieve the answer. 
 retry on socket failure.
 """
         c = 0
         ret = ""
         self.reconnectcheck()
@@ -769,27 +774,27 @@
                     ret=""
                 else:
                     c=3
                     raise(e)
         return(ret)
 
     def ti(self):
-        """ti()
+        """Recieve the time from the sipserver.
 
 Request the time from lmw and returns the string.
 
 Raises a LmwCmdWarn of failure
 """
         ti="TI " + self.meetnet + "\r"
         d = self.sendrecv(ti)
         return (d[2:-1])
 
     def cmd(self, process, location, parameter, time_delta, day,
                                                 time_of_day, cmd_type="DATA"):
-        """cmd(process, location, parameter, time_delta, day, time_of_day)
+        """Create a sip command from the paramters
 
 Send a cmd to LMW and returns the lmw string
 
     process:      <WN|VW|AS>
     location:     <lmw location (e.g. HOEK)>
     parameter:    <lmw parameter (e.g. H10)>
     time_delta:   <Time windows (max 23:59, e.g. +01:00>
@@ -813,17 +818,43 @@
                time_of_day + data + "\r" 
 
         d = self.sendrecv(cmdstr)
         if (d[0] != '!'):
             raise LmwCmdWarn(cmdstr, d)
         return (d[2:-1])
 
+    def cmdWrite(self, process, location, parameter, time_delta, day,
+                 time_of_day, values):
+        """Write data to LMW
+
+    process:      <WNT|VWT|AST>
+    location:     <lmw location (e.g. HOEK)>
+    parameter:    <lmw parameter (e.g. H10)>
+    time_delta:   <Time windows (max 23:59, e.g. +01:00>
+    day:          <Date>
+    time_of_day:  <Time>
+    data:         Values to be writen (e.g. 33/10;35/10).
+
+Example:
+    lmw.cmd("WNT", "HOEK", "H10", "+00:20", "13-08-2018", "16:00", "33/10;35/10")
+
+Returns:
+    The LMW answer string
+"""
+        cmdstr=process + " " + self.meetnet + "," + location + "," + \
+               parameter + "," + time_delta + "," + day + "," + \
+               time_of_day + values + "\r" 
+        d = self.sendrecv(cmdstr)
+        if (d[0] != '!'):
+            raise LmwCmdWarn(cmdstr, d)
+        return (d[2:-1])
+
     def valueStr(self, process, location, parameter, day = None,
                     time_of_day = None):
-        """value(process, location, parameter, [day], [time_of_day]):
+        """Get string of values from sip
 
 Parameters:
     process:      <WN|VW|AS>
     location:     <lmw location (e.g. HOEK)>
     parameter:    <lmw parameter (e.g. H10)>
     day:          [date = now()]
     time_of_day:  [time = now()]
@@ -842,15 +873,15 @@
             if (time_of_day==None):
                 time_of_day=last["time_of_day"]
         return(self.cmd(process, location, parameter, "+00:00", day,
                        time_of_day, "DATA"))
 
     def value(self, process, location, parameter, day = None,
                     time_of_day = None):
-        """value(process, location, parameter, [day], [time_of_day]):
+        """Get one value from sip
 
 Parameters:
     process:      <WN|VW|AS>
     location:     <lmw location (e.g. HOEK)>
     parameter:    <lmw parameter (e.g. H10)>
     day:          [date = now()]
     time_of_day:  [time = now()]
@@ -886,15 +917,15 @@
             time += timedelta(seconds=60-time.second)
         if (delta == timedelta(minutes=10)) and (time.minute % 10 != 0):
                 time += timedelta(minutes=(10-time.minute%10))
         return(time)
 
     def timeSerie(self, process, location, parameter,
                         startTime, endTime, cmd_type="DATB"):
-        """timeSerie(process, location, parameter, startTime, endTime, cmd_type="DATA")
+        """Get a python data structure with the results.
 
 Parameters:
     process:      <WN|VW|AS>
     location:     <lmw location (e.g. HOEK)>
     parameter:    <lmw parameter (e.g. H10)>
     startTime:    Start time (datetime)
     endTime:      End time (datetime)
@@ -955,15 +986,15 @@
                               cmd_type)
             res.addvalues(startTime, values)
             startTime += window + delta
             
         return(res)
 
     def logout(self):
-        """logout()
+        """Logut of the sip server,
 
 Logs of
 """
         self.send("LO\r")
         self.closesocket()
 
 class lmwTimeSerie:
@@ -979,28 +1010,28 @@
     * For most measurements there is only one value (e.g H10).
     * Additionale kwaliteit is optional and may contain None.
     * Result times in UTC
 
 """
 
     def __init__(self, start, delta, values=""):
-        """lmwTimeSerie(start, delta, values)
+        """lmwTimeSerie init
 
 Create a lmwTimeSerie object with:
     start:  Start time
     delta:  Period of the measurements
     values: lmw result string
 """
         self.ts    = []
         self.delta = delta
         if values != "":
             self.addvalues(start, values)
 
     def addvalues(self, start, values):
-        """addvalues(start, delta, values)
+        """Add values
 
 Add values to a timeserie
     start:  Start time
     delta:  Period of the measurements
     values: lmw result string
 
 """
```

### Comparing `lmwsip-0.9.6/src/lmwsip/run.py` & `lmwsip-0.9.7/src/lmwsip/run.py`

 * *Files identical despite different names*

### Comparing `lmwsip-0.9.6/src/lmwsip.egg-info/PKG-INFO` & `lmwsip-0.9.7/src/lmwsip.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: lmwsip
-Version: 0.9.6
+Version: 0.9.7
 Summary: Interface for the lmw sip protocol
 Home-page: https://git.marceln.org/Werk/lmwsip
 Author: Marcel Nijenhof
 Author-email: pypi@marceln.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
 
 # lmwsip
 ## Introduction
 
 lmwsip is a python library for the lmw sip protocol.
 
 ## Package
```

