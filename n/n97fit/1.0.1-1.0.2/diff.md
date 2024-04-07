# Comparing `tmp/n97fit-1.0.1.tar.gz` & `tmp/n97fit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n97fit-1.0.1.tar", last modified: Sat Apr  6 16:06:59 2024, max compression
+gzip compressed data, was "n97fit-1.0.2.tar", last modified: Sun Apr  7 07:04:31 2024, max compression
```

## Comparing `n97fit-1.0.1.tar` & `n97fit-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-06 16:06:59.146545 n97fit-1.0.1/
--rw-r--r--   0 yashiro    (501) staff       (20)      330 2024-03-25 06:38:03.000000 n97fit-1.0.1/AUTHORS
--rw-r--r--   0 yashiro    (501) staff       (20)     1499 2024-03-25 06:38:03.000000 n97fit-1.0.1/LICENSE
--rw-r--r--   0 yashiro    (501) staff       (20)       16 2024-03-25 06:38:03.000000 n97fit-1.0.1/MANIFEST.in
--rw-r--r--   0 yashiro    (501) staff       (20)     7776 2024-04-06 16:06:59.146215 n97fit-1.0.1/PKG-INFO
--rw-r--r--   0 yashiro    (501) staff       (20)     4843 2024-03-25 06:38:03.000000 n97fit-1.0.1/README.md
--rw-r--r--   0 yashiro    (501) staff       (20)     1513 2024-04-06 16:06:49.000000 n97fit-1.0.1/pyproject.toml
--rw-r--r--   0 yashiro    (501) staff       (20)       38 2024-04-06 16:06:59.146620 n97fit-1.0.1/setup.cfg
-drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-06 16:06:59.133103 n97fit-1.0.1/src/
-drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-06 16:06:59.136643 n97fit-1.0.1/src/n97fit/
--rw-r--r--   0 yashiro    (501) staff       (20)      200 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/__init__.py
--rw-r--r--   0 yashiro    (501) staff       (20)     4639 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/__main__.py
-drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-06 16:06:59.140093 n97fit-1.0.1/src/n97fit/date/
--rw-r--r--   0 yashiro    (501) staff       (20)      138 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/date/__init__.py
--rw-r--r--   0 yashiro    (501) staff       (20)      956 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/date/cday.py
--rw-r--r--   0 yashiro    (501) staff       (20)     2304 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/date/ijmapping.py
-drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-06 16:06:59.142915 n97fit-1.0.1/src/n97fit/harmonics/
--rw-r--r--   0 yashiro    (501) staff       (20)      144 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/harmonics/__init__.py
--rw-r--r--   0 yashiro    (501) staff       (20)      704 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/harmonics/fourier.py
--rw-r--r--   0 yashiro    (501) staff       (20)     1016 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/harmonics/frcoef.py
--rw-r--r--   0 yashiro    (501) staff       (20)      510 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/harmonics/harmonic.py
--rw-r--r--   0 yashiro    (501) staff       (20)     1703 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/harmonics/invmat.py
--rw-r--r--   0 yashiro    (501) staff       (20)      560 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/harmonics/smooth.py
-drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-06 16:06:59.144224 n97fit-1.0.1/src/n97fit/io/
--rw-r--r--   0 yashiro    (501) staff       (20)      224 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/io/__init__.py
--rw-r--r--   0 yashiro    (501) staff       (20)      817 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/io/logging.py
--rw-r--r--   0 yashiro    (501) staff       (20)     2019 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/io/read_n97format.py
--rw-r--r--   0 yashiro    (501) staff       (20)     7633 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/io/write_fixedformat.py
-drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-06 16:06:59.145142 n97fit-1.0.1/src/n97fit/misc/
--rw-r--r--   0 yashiro    (501) staff       (20)      115 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/misc/__init__.py
--rw-r--r--   0 yashiro    (501) staff       (20)      850 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/misc/matching.py
--rw-r--r--   0 yashiro    (501) staff       (20)      385 2024-03-25 06:38:03.000000 n97fit-1.0.1/src/n97fit/misc/reviseflag.py
--rw-r--r--   0 yashiro    (501) staff       (20)    34619 2024-03-27 15:53:29.000000 n97fit-1.0.1/src/n97fit/n97fit.py
-drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-06 16:06:59.145746 n97fit-1.0.1/src/n97fit.egg-info/
--rw-r--r--   0 yashiro    (501) staff       (20)     7776 2024-04-06 16:06:59.000000 n97fit-1.0.1/src/n97fit.egg-info/PKG-INFO
--rw-r--r--   0 yashiro    (501) staff       (20)      801 2024-04-06 16:06:59.000000 n97fit-1.0.1/src/n97fit.egg-info/SOURCES.txt
--rw-r--r--   0 yashiro    (501) staff       (20)        1 2024-04-06 16:06:59.000000 n97fit-1.0.1/src/n97fit.egg-info/dependency_links.txt
--rw-r--r--   0 yashiro    (501) staff       (20)       43 2024-04-06 16:06:59.000000 n97fit-1.0.1/src/n97fit.egg-info/entry_points.txt
--rw-r--r--   0 yashiro    (501) staff       (20)       46 2024-04-06 16:06:59.000000 n97fit-1.0.1/src/n97fit.egg-info/requires.txt
--rw-r--r--   0 yashiro    (501) staff       (20)        7 2024-04-06 16:06:59.000000 n97fit-1.0.1/src/n97fit.egg-info/top_level.txt
+drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-07 07:04:31.589205 n97fit-1.0.2/
+-rw-r--r--   0 yashiro    (501) staff       (20)      330 2024-03-25 06:38:03.000000 n97fit-1.0.2/AUTHORS
+-rw-r--r--   0 yashiro    (501) staff       (20)     1499 2024-03-25 06:38:03.000000 n97fit-1.0.2/LICENSE
+-rw-r--r--   0 yashiro    (501) staff       (20)       16 2024-03-25 06:38:03.000000 n97fit-1.0.2/MANIFEST.in
+-rw-r--r--   0 yashiro    (501) staff       (20)     7776 2024-04-07 07:04:31.588831 n97fit-1.0.2/PKG-INFO
+-rw-r--r--   0 yashiro    (501) staff       (20)     4843 2024-03-25 06:38:03.000000 n97fit-1.0.2/README.md
+-rw-r--r--   0 yashiro    (501) staff       (20)     1513 2024-04-07 07:04:02.000000 n97fit-1.0.2/pyproject.toml
+-rw-r--r--   0 yashiro    (501) staff       (20)       38 2024-04-07 07:04:31.589303 n97fit-1.0.2/setup.cfg
+drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-07 07:04:31.577131 n97fit-1.0.2/src/
+drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-07 07:04:31.580223 n97fit-1.0.2/src/n97fit/
+-rw-r--r--   0 yashiro    (501) staff       (20)      200 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/__init__.py
+-rw-r--r--   0 yashiro    (501) staff       (20)     4639 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/__main__.py
+drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-07 07:04:31.583151 n97fit-1.0.2/src/n97fit/date/
+-rw-r--r--   0 yashiro    (501) staff       (20)      138 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/date/__init__.py
+-rw-r--r--   0 yashiro    (501) staff       (20)      956 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/date/cday.py
+-rw-r--r--   0 yashiro    (501) staff       (20)     2304 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/date/ijmapping.py
+drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-07 07:04:31.585094 n97fit-1.0.2/src/n97fit/harmonics/
+-rw-r--r--   0 yashiro    (501) staff       (20)      144 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/harmonics/__init__.py
+-rw-r--r--   0 yashiro    (501) staff       (20)      704 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/harmonics/fourier.py
+-rw-r--r--   0 yashiro    (501) staff       (20)     1016 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/harmonics/frcoef.py
+-rw-r--r--   0 yashiro    (501) staff       (20)      510 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/harmonics/harmonic.py
+-rw-r--r--   0 yashiro    (501) staff       (20)     1703 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/harmonics/invmat.py
+-rw-r--r--   0 yashiro    (501) staff       (20)      560 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/harmonics/smooth.py
+drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-07 07:04:31.586568 n97fit-1.0.2/src/n97fit/io/
+-rw-r--r--   0 yashiro    (501) staff       (20)      224 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/io/__init__.py
+-rw-r--r--   0 yashiro    (501) staff       (20)      817 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/io/logging.py
+-rw-r--r--   0 yashiro    (501) staff       (20)     2019 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/io/read_n97format.py
+-rw-r--r--   0 yashiro    (501) staff       (20)     7633 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/io/write_fixedformat.py
+drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-07 07:04:31.587816 n97fit-1.0.2/src/n97fit/misc/
+-rw-r--r--   0 yashiro    (501) staff       (20)      115 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/misc/__init__.py
+-rw-r--r--   0 yashiro    (501) staff       (20)      850 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/misc/matching.py
+-rw-r--r--   0 yashiro    (501) staff       (20)      385 2024-03-25 06:38:03.000000 n97fit-1.0.2/src/n97fit/misc/reviseflag.py
+-rw-r--r--   0 yashiro    (501) staff       (20)    35642 2024-04-07 07:04:02.000000 n97fit-1.0.2/src/n97fit/n97fit.py
+drwxr-xr-x   0 yashiro    (501) staff       (20)        0 2024-04-07 07:04:31.588292 n97fit-1.0.2/src/n97fit.egg-info/
+-rw-r--r--   0 yashiro    (501) staff       (20)     7776 2024-04-07 07:04:31.000000 n97fit-1.0.2/src/n97fit.egg-info/PKG-INFO
+-rw-r--r--   0 yashiro    (501) staff       (20)      801 2024-04-07 07:04:31.000000 n97fit-1.0.2/src/n97fit.egg-info/SOURCES.txt
+-rw-r--r--   0 yashiro    (501) staff       (20)        1 2024-04-07 07:04:31.000000 n97fit-1.0.2/src/n97fit.egg-info/dependency_links.txt
+-rw-r--r--   0 yashiro    (501) staff       (20)       43 2024-04-07 07:04:31.000000 n97fit-1.0.2/src/n97fit.egg-info/entry_points.txt
+-rw-r--r--   0 yashiro    (501) staff       (20)       46 2024-04-07 07:04:31.000000 n97fit-1.0.2/src/n97fit.egg-info/requires.txt
+-rw-r--r--   0 yashiro    (501) staff       (20)        7 2024-04-07 07:04:31.000000 n97fit-1.0.2/src/n97fit.egg-info/top_level.txt
```

### Comparing `n97fit-1.0.1/LICENSE` & `n97fit-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/PKG-INFO` & `n97fit-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n97fit
-Version: 1.0.1
+Version: 1.0.2
 Summary:  This is a program of data selection and curve fitting by a digital filtering technique including Reinsch-type cubic spline, Fourier harmonics and linear interpolation. It is to derive the fitted curve to the observed data ( CO2, d13C,..), as well as to separate the seasonal, short- and long-term variations from the data. 
 Author: Takakiyo Nakazawa
 Maintainer-email: Hisashi Yashio <yashiro.hisashi@nies.go.jp>
 License: Copyright (c) 1991-2024, n97fit developers
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `n97fit-1.0.1/README.md` & `n97fit-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/pyproject.toml` & `n97fit-1.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "n97fit"
-version = "1.0.1"
+version = "1.0.2"
 license = {file = "LICENSE"}
 
 authors = [
   {name = "Takakiyo Nakazawa"},
 ]
 
 maintainers = [
```

### Comparing `n97fit-1.0.1/src/n97fit/__main__.py` & `n97fit-1.0.2/src/n97fit/__main__.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/date/cday.py` & `n97fit-1.0.2/src/n97fit/date/cday.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/date/ijmapping.py` & `n97fit-1.0.2/src/n97fit/date/ijmapping.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/harmonics/fourier.py` & `n97fit-1.0.2/src/n97fit/harmonics/fourier.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/harmonics/frcoef.py` & `n97fit-1.0.2/src/n97fit/harmonics/frcoef.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/harmonics/invmat.py` & `n97fit-1.0.2/src/n97fit/harmonics/invmat.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/harmonics/smooth.py` & `n97fit-1.0.2/src/n97fit/harmonics/smooth.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/io/logging.py` & `n97fit-1.0.2/src/n97fit/io/logging.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/io/read_n97format.py` & `n97fit-1.0.2/src/n97fit/io/read_n97format.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/io/write_fixedformat.py` & `n97fit-1.0.2/src/n97fit/io/write_fixedformat.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/misc/matching.py` & `n97fit-1.0.2/src/n97fit/misc/matching.py`

 * *Files identical despite different names*

### Comparing `n97fit-1.0.1/src/n97fit/n97fit.py` & `n97fit-1.0.2/src/n97fit/n97fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             itelim = 1
 
         temp_cnt = None
         for iteration in range(0, itelim):
             logger.info("")
             logger.info("* * * * * * * * * * * * * * * * * * * * * * * * * * * *")
             logger.info(
-                "* * *             START FITTING No. %1d             * * *", iteration + 1
+                "* * *              START FITTING No. %1d             * * *", iteration + 1
             )
             logger.info("* * * * * * * * * * * * * * * * * * * * * * * * * * * *")
 
             # * * *   Stage 2 : fit of Spline + fourier to the data
 
             logger.info("")
             logger.info(" *** START Fourier&Spline FITTING ***")
@@ -553,43 +553,63 @@
                         ij = ijmap[i][j]
 
                         if flag[ij] >= 0:
                             dev = de_sphmlohi[i]  # Judge by using averaged
                             flag[ij], cnt = reviseflag(dev, flag[ij], sgm_allow)
                             sumcnt += cnt
 
-            logger.info("")
-            logger.info("  =>Reject data (sigma*%2d): %5d", pl_sigma, sumcnt)
+                logger.info("")
+                logger.info("  =>Reject data (sigma*%2d): %5d", pl_sigma, sumcnt)
 
-            reportrej(rawndata, rawymd, rawy, flag, 2)
+                reportrej(rawndata, rawymd, rawy, flag, 2)
+
+                if sumcnt == temp_cnt:
+                    break
+
+                # Re-Allocate 2D Array (reject flag 1 and 2)
+                ndata, dt, d, t, y, ysdev, ijdata, ijmap = ijmapping(
+                    pl_avgday, rawt, rawd, rawy, flag, asarray=True
+                )
 
-            if sumcnt == temp_cnt:
                 logger.info("")
-                logger.info("* * * * * * * * * * * * * * * * * * * * * * * * * * * *")
-                logger.info("* * *                 END FITTING                 * * *")
-                logger.info("* * * * * * * * * * * * * * * * * * * * * * * * * * * *")
-                break
-
-            # Re-Allocate 2D Array (reject flag 1 and 2)
-            ndata, dt, d, t, y, ysdev, ijdata, ijmap = ijmapping(
-                pl_avgday, rawt, rawd, rawy, flag, asarray=True
-            )
+                logger.info("  =====> BACK TO STAGE 2 =====> ")
+                temp_cnt = sumcnt
 
-            logger.info("")
-            logger.info("  =====> BACK TO STAGE 2 =====> ")
-            temp_cnt = sumcnt
+        logger.info("")
+        logger.info("* * * * * * * * * * * * * * * * * * * * * * * * * * * *")
+        logger.info("* * *                 END FITTING                 * * *")
+        logger.info("* * * * * * * * * * * * * * * * * * * * * * * * * * * *")
 
         # *** Stage 3 : END ***
 
         # * * *      Stage 4 : Output Files       * * *  !
 
         t_tt = matching(rawndata, rawt, xdata, x_t, x_tt, self.day_interval)
         t_tr = matching(rawndata, rawt, xdata, x_t, x_tr, self.day_interval)
         t_ss = matching(rawndata, rawt, xdata, x_t, x_ss, self.day_interval)
 
+        if sw_iteration == 0:
+            dev       = rawy - t_tt
+            sgm_all   = np.std(dev)
+            sgm_allow = sgm_all * pl_sigma
+
+            logger.info("")
+            logger.info("  +Sigma(Y -total) = %12.7E", sgm_all)
+
+            for ij in range(0, rawndata):
+                if flag[ij] >= 0:
+                    flag[ij], cnt = reviseflag(dev[ij], flag[ij], sgm_allow)
+                    sumcnt += cnt
+
+            logger.info("")
+            logger.info("  =>Reject data (sigma*%2d): %5d", pl_sigma, sumcnt)
+
+            reportrej(rawndata, rawymd, rawy, flag, 2)
+            logger.info("")
+
         self.syear = syear
         self.trange = (tstart, tend + 1)
         self.nh = nh
         self.hm_coef = hm_coef
 
         # raw_data : equal to raw data (no average in same day)
         self.raw_data = pd.DataFrame(
@@ -679,17 +699,24 @@
         # convert date to continuous day
         data["d"] = data["date"].apply(
             lambda x: date2cday(x),
         )
 
         # convert date to continuous year
         data["t"] = data["d"].apply(
-            lambda x: (x - date2cday(sdate)) / self.days_in_year,
+            lambda x: ( float( x - date2cday(sdate) ) + 0.5 ) / float( self.days_in_year )
         )
 
+        # convert date to continuous year (exact calculation)
+#         data["t"] = data["date"].apply(
+#             lambda x: float( ( date(x.year,x.month,x.day) - date(x.year,1,1) ).days + 0.5 ) # assume 12:00
+#                     / float( ( date(x.year+1,1,1)         - date(x.year,1,1) ).days )
+#                     + float( x.year - syear )
+#         )
+
         # stop if reverse in time is found
         dt = data["t"].diff()
         if (dt < 0).any():
             revserse = data["ymd"][dt < 0].values
             raise ValueError(f"reverse in time is found. {revserse}")
 
         # check flag and set -1 if value is invalid(<=-999)
```

### Comparing `n97fit-1.0.1/src/n97fit.egg-info/PKG-INFO` & `n97fit-1.0.2/src/n97fit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n97fit
-Version: 1.0.1
+Version: 1.0.2
 Summary:  This is a program of data selection and curve fitting by a digital filtering technique including Reinsch-type cubic spline, Fourier harmonics and linear interpolation. It is to derive the fitted curve to the observed data ( CO2, d13C,..), as well as to separate the seasonal, short- and long-term variations from the data. 
 Author: Takakiyo Nakazawa
 Maintainer-email: Hisashi Yashio <yashiro.hisashi@nies.go.jp>
 License: Copyright (c) 1991-2024, n97fit developers
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `n97fit-1.0.1/src/n97fit.egg-info/SOURCES.txt` & `n97fit-1.0.2/src/n97fit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

