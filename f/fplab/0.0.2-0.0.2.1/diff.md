# Comparing `tmp/fplab-0.0.2.tar.gz` & `tmp/fplab-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplab-0.0.2.tar", last modified: Sat Apr  6 16:19:45 2024, max compression
+gzip compressed data, was "fplab-0.0.2.1.tar", last modified: Sun Apr  7 06:02:59 2024, max compression
```

## Comparing `fplab-0.0.2.tar` & `fplab-0.0.2.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.236638 fplab-0.0.2/
--rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      521 2024-04-06 16:19:45.236638 fplab-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.175407 fplab-0.0.2/fplab/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.205306 fplab-0.0.2/fplab/enhancement/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/enhancement/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/enhancement/frequency.py
--rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.2/fplab/enhancement/spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.205306 fplab-0.0.2/fplab/generation/
--rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2/fplab/generation/__init__.py
--rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2/fplab/generation/tps.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.205306 fplab-0.0.2/fplab/intrinsic/
--rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2/fplab/intrinsic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.220944 fplab-0.0.2/fplab/intrinsic/frequency/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/intrinsic/frequency/__init__.py
--rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/intrinsic/frequency/projection.py
--rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/intrinsic/frequency/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.223622 fplab-0.0.2/fplab/intrinsic/mask/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/intrinsic/mask/__init__.py
--rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2/fplab/intrinsic/mask/mask.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.224125 fplab-0.0.2/fplab/intrinsic/multiple/
--rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2/fplab/intrinsic/multiple/__init__.py
--rw-rw-rw-   0        0        0     7036 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/intrinsic/multiple/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.224125 fplab-0.0.2/fplab/intrinsic/orientation/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/intrinsic/orientation/__init__.py
--rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2/fplab/intrinsic/orientation/gradient.py
--rw-rw-rw-   0        0        0     5490 2024-04-06 09:04:39.000000 fplab-0.0.2/fplab/intrinsic/orientation/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.224125 fplab-0.0.2/fplab/intrinsic/skeleton/
--rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2/fplab/intrinsic/skeleton/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2/fplab/intrinsic/skeleton/skeleton.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.236638 fplab-0.0.2/fplab/matching/
--rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2/fplab/matching/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2/fplab/matching/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.236638 fplab-0.0.2/fplab/minutiae/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/minutiae/__init__.py
--rw-rw-rw-   0        0        0     5997 2024-04-05 16:32:39.000000 fplab-0.0.2/fplab/minutiae/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.236638 fplab-0.0.2/fplab/tools/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/tools/__init__.py
--rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2/fplab/tools/array.py
--rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2/fplab/tools/image.py
--rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2/fplab/tools/nbis.py
--rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2/fplab/tools/tensor.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.192789 fplab-0.0.2/fplab.egg-info/
--rw-rw-rw-   0        0        0      521 2024-04-06 16:19:45.000000 fplab-0.0.2/fplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      986 2024-04-06 16:19:45.000000 fplab-0.0.2/fplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:19:45.000000 fplab-0.0.2/fplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-06 16:19:45.000000 fplab-0.0.2/fplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 16:19:45.236638 fplab-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      799 2024-04-05 16:53:40.000000 fplab-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.140460 fplab-0.0.2.1/
+-rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      523 2024-04-07 06:02:59.140460 fplab-0.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.066566 fplab-0.0.2.1/fplab/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.1/fplab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.083128 fplab-0.0.2.1/fplab/enhancement/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.1/fplab/enhancement/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.1/fplab/enhancement/frequency.py
+-rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.2.1/fplab/enhancement/spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.088801 fplab-0.0.2.1/fplab/generation/
+-rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.1/fplab/generation/__init__.py
+-rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2.1/fplab/generation/tps.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.088801 fplab-0.0.2.1/fplab/intrinsic/
+-rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.1/fplab/intrinsic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.100451 fplab-0.0.2.1/fplab/intrinsic/frequency/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.1/fplab/intrinsic/frequency/__init__.py
+-rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.1/fplab/intrinsic/frequency/projection.py
+-rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.1/fplab/intrinsic/frequency/tools.py
+-rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.1/fplab/intrinsic/frequency/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.105009 fplab-0.0.2.1/fplab/intrinsic/mask/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.1/fplab/intrinsic/mask/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.1/fplab/intrinsic/mask/mask.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.109268 fplab-0.0.2.1/fplab/intrinsic/multiple/
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.1/fplab/intrinsic/multiple/__init__.py
+-rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.1/fplab/intrinsic/multiple/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.109268 fplab-0.0.2.1/fplab/intrinsic/orientation/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.1/fplab/intrinsic/orientation/__init__.py
+-rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2.1/fplab/intrinsic/orientation/gradient.py
+-rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.1/fplab/intrinsic/orientation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.119440 fplab-0.0.2.1/fplab/intrinsic/skeleton/
+-rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.1/fplab/intrinsic/skeleton/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.1/fplab/intrinsic/skeleton/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.119440 fplab-0.0.2.1/fplab/matching/
+-rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.1/fplab/matching/__init__.py
+-rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.1/fplab/matching/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.123234 fplab-0.0.2.1/fplab/minutiae/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.1/fplab/minutiae/__init__.py
+-rw-rw-rw-   0        0        0     5997 2024-04-05 16:32:39.000000 fplab-0.0.2.1/fplab/minutiae/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.140460 fplab-0.0.2.1/fplab/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.1/fplab/tools/__init__.py
+-rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.1/fplab/tools/array.py
+-rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.1/fplab/tools/image.py
+-rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.1/fplab/tools/nbis.py
+-rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.1/fplab/tools/tensor.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:02:59.077602 fplab-0.0.2.1/fplab.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-04-07 06:02:58.000000 fplab-0.0.2.1/fplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2024-04-07 06:02:58.000000 fplab-0.0.2.1/fplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 06:02:58.000000 fplab-0.0.2.1/fplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-07 06:02:58.000000 fplab-0.0.2.1/fplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 06:02:59.140460 fplab-0.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      801 2024-04-07 05:47:19.000000 fplab-0.0.2.1/setup.py
```

### Comparing `fplab-0.0.2/LICENSE.txt` & `fplab-0.0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/PKG-INFO` & `fplab-0.0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2/README.md` & `fplab-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/enhancement/frequency.py` & `fplab-0.0.2.1/fplab/enhancement/frequency.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/enhancement/spatial.py` & `fplab-0.0.2.1/fplab/enhancement/spatial.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/generation/tps.py` & `fplab-0.0.2.1/fplab/generation/tps.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/intrinsic/frequency/projection.py` & `fplab-0.0.2.1/fplab/intrinsic/frequency/projection.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/intrinsic/frequency/tools.py` & `fplab-0.0.2.1/fplab/intrinsic/frequency/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/intrinsic/mask/mask.py` & `fplab-0.0.2.1/fplab/intrinsic/mask/mask.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/intrinsic/multiple/transform.py` & `fplab-0.0.2.1/fplab/intrinsic/multiple/transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """
-基于傅里叶变换的指纹方向场估计方法
-同时可以估计频率场
+基于变换的多目标估计方法
 这里预先假设指纹为灰度图或二值图，不能保证函数在RGB图像的适用性
 """
 import numpy as np
 from fplab.tools.image import type_as
 from fplab.tools.array import ima_minmax, ima_pad_blk, ima_pad_crop, ima_rgb2l, ima_gaussian
 from fplab.tools.array import ima_float2uint, ima_uint2float
 from scipy import fft, ndimage
@@ -47,15 +46,15 @@
         ind = n-n//2
     else:
         ind = c_ind
 
     def filter_function(in_elements):
         """in_elements是待处理元素及其邻域元素"""
         # 这里角度乘2是考虑到方向场的取值范围为Pi
-        out = np.abs(np.cos(2*(in_elements-in_elements[ind]))).sum()/n
+        out = (np.cos(2*(in_elements-in_elements[ind])).sum()/n+1)/2
         return out
 
     return f, filter_function
 
 
 def chikkerur2007(im, blk_sz=(8, 8), wd_sz=(32, 32), smo_sz=(3, 3), smf_sz=(3, 3), smo_itn=1, smf_itn=1, win_c=5):
     """使用2007年chikkerur使用的方法(STFT)分析指纹，输出方向场、频率场、感兴趣区域和方向置信度。
```

### Comparing `fplab-0.0.2/fplab/intrinsic/orientation/gradient.py` & `fplab-0.0.2.1/fplab/intrinsic/orientation/gradient.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/intrinsic/orientation/tools.py` & `fplab-0.0.2.1/fplab/intrinsic/orientation/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """
 与指纹方向场有关的函数
-average_orientation_nd      计算方向场的局部角度平均值
-display_orientation            展示方向场
+average_orientation_nd              计算方向场的局部角度平均值
+display_orientation                 展示方向场
+quick_correctness_estimation        快速估计方向场可信度
+compare_orientation_nd              比较方向场（无朝向）
 """
 import gc
 import torch
 import numpy as np
 import cv2
+from scipy.ndimage import generic_filter
 from fplab.tools.image import type_as
 from fplab.tools.array import ima_pad_blk, ima_l2rgb, ima_pad_crop, ima_show, ima_save
 from fplab.tools.tensor import imt_sum_average
+from fplab.intrinsic.multiple.transform import get_coherence_filter_function
 
 
 def average_orientation_nd(ot, blk_sz, s=(1, 1), keep_shape=True):
     """计算方向场每一个像素点周围像素的角度平均值。
     该函数以张量的形式处理图像，通过二维卷积实现角度平均值的计算
     这个函数期望的取值区间长度为pi，相差pi的两个方向视作一个方向
     函数名中的nd是no direction的缩写，表示方向与反方向视为同一方向"""
@@ -105,14 +109,28 @@
         ima_show(out)
     if "save" in flag and save_path:
         ima_save(out, save_path)
     if "return" in flag:
         return type_as(out, im)
 
 
-def compare_orientation_nd(ot1, ot2, oc):
+def quick_correctness_estimation(ot, ksz=(16, 16)):
+    """快速获取方向场可信度
+    ot          方向场
+    ksz         估计可信度使用的窗口大小，整数或整数序列"""
+    ft, filter_func = get_coherence_filter_function(ksz)
+    ota = type_as(ot, "a")
+    out = generic_filter(ota, filter_func, footprint=ft)
+    return type_as(out, ot)
+
+
+def compare_orientation_nd(ot1, ot2, oc=None):
     """比较两个无向方向场的相似度
     ot1, ot2        无向方向场，可以为数组或张量
     oc              方向场可信度或者mask，可以为数组或张量
     """
-    ota1, ota2, oca = type_as(ot1, "a"), type_as(ot2, "a"), type_as(oc, "a")
+    ota1, ota2 = type_as(ot1, "a"), type_as(ot2, "a")
+    if oc is None:
+        oca = np.ones_like(ota1)
+    else:
+        oca = type_as(oc, "a")
     return ((np.cos(2*(ota1-ota2)))*oca).sum()/oca.sum()
```

### Comparing `fplab-0.0.2/fplab/intrinsic/skeleton/skeleton.py` & `fplab-0.0.2.1/fplab/intrinsic/skeleton/skeleton.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/matching/tools.py` & `fplab-0.0.2.1/fplab/matching/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/minutiae/tools.py` & `fplab-0.0.2.1/fplab/minutiae/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/tools/array.py` & `fplab-0.0.2.1/fplab/tools/array.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/tools/image.py` & `fplab-0.0.2.1/fplab/tools/image.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/tools/nbis.py` & `fplab-0.0.2.1/fplab/tools/nbis.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab/tools/tensor.py` & `fplab-0.0.2.1/fplab/tools/tensor.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2/fplab.egg-info/PKG-INFO` & `fplab-0.0.2.1/fplab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2/fplab.egg-info/SOURCES.txt` & `fplab-0.0.2.1/fplab.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 fplab/enhancement/spatial.py
 fplab/generation/__init__.py
 fplab/generation/tps.py
 fplab/intrinsic/__init__.py
 fplab/intrinsic/frequency/__init__.py
 fplab/intrinsic/frequency/projection.py
 fplab/intrinsic/frequency/tools.py
+fplab/intrinsic/frequency/transform.py
 fplab/intrinsic/mask/__init__.py
 fplab/intrinsic/mask/mask.py
 fplab/intrinsic/multiple/__init__.py
 fplab/intrinsic/multiple/transform.py
 fplab/intrinsic/orientation/__init__.py
 fplab/intrinsic/orientation/gradient.py
 fplab/intrinsic/orientation/tools.py
```

### Comparing `fplab-0.0.2/setup.py` & `fplab-0.0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.2.1'
 DESCRIPTION = 'Python3 Package for Fingerprint Processing'
 LONG_DESCRIPTION = ('This is a python3 package for fingerprint processing,'
                     ' which can be used for fingerprint enhancement.')
 
 setup(
     name="fplab",
     version=VERSION,
```

