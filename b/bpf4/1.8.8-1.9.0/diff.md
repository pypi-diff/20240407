# Comparing `tmp/bpf4-1.8.8-cp39-cp39-win_amd64.whl.zip` & `tmp/bpf4-1.9.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,24 @@
-Zip file size: 417670 bytes, number of entries: 19
--rw-rw-rw-  2.0 fat      204 b- defN 24-Feb-28 19:04 bpf4/__init__.py
--rw-rw-rw-  2.0 fat    16180 b- defN 24-Feb-28 19:04 bpf4/api.py
--rw-rw-rw-  2.0 fat     1937 b- defN 24-Feb-28 19:04 bpf4/arraytools.py
--rw-rw-rw-  2.0 fat      415 b- defN 24-Feb-28 19:04 bpf4/bench.py
--rw-rw-rw-  2.0 fat      356 b- defN 24-Feb-28 19:04 bpf4/config.py
--rw-rw-rw-  2.0 fat   922624 b- defN 24-Feb-28 19:08 bpf4/core.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     9973 b- defN 24-Feb-28 19:04 bpf4/core.pyi
--rw-rw-rw-  2.0 fat   182502 b- defN 24-Feb-28 19:04 bpf4/core.pyx
--rw-rw-rw-  2.0 fat     8380 b- defN 24-Feb-28 19:04 bpf4/csvtools.py
--rw-rw-rw-  2.0 fat     4168 b- defN 24-Feb-28 19:04 bpf4/plot.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-28 19:04 bpf4/py.typed
--rw-rw-rw-  2.0 fat     1334 b- defN 24-Feb-28 19:04 bpf4/pyinterp.py
--rw-rw-rw-  2.0 fat     1466 b- defN 24-Feb-28 19:04 bpf4/tests.py
--rw-rw-rw-  2.0 fat    31458 b- defN 24-Feb-28 19:04 bpf4/util.py
--rw-rw-rw-  2.0 fat       89 b- defN 24-Feb-28 19:04 bpf4/version.py
--rw-rw-rw-  2.0 fat     5354 b- defN 24-Feb-28 19:08 bpf4-1.8.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Feb-28 19:08 bpf4-1.8.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Feb-28 19:08 bpf4-1.8.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1362 b- defN 24-Feb-28 19:08 bpf4-1.8.8.dist-info/RECORD
-19 files, 1187907 bytes uncompressed, 415526 bytes compressed:  65.0%
+Zip file size: 2485080 bytes, number of entries: 22
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-07 19:29 bpf4/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-07 19:29 bpf4.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-07 19:29 bpf4-1.9.0.dist-info/
+-rw-r--r--  2.0 unx     4025 b- defN 24-Apr-07 19:29 bpf4/plot.py
+-rw-r--r--  2.0 unx    30349 b- defN 24-Apr-07 19:29 bpf4/util.py
+-rw-r--r--  2.0 unx       85 b- defN 24-Apr-07 19:29 bpf4/version.py
+-rw-r--r--  2.0 unx     8159 b- defN 24-Apr-07 19:29 bpf4/csvtools.py
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-07 19:29 bpf4/tests.py
+-rw-r--r--  2.0 unx      192 b- defN 24-Apr-07 19:29 bpf4/__init__.py
+-rw-r--r--  2.0 unx    15595 b- defN 24-Apr-07 19:29 bpf4/api.py
+-rw-r--r--  2.0 unx      392 b- defN 24-Apr-07 19:29 bpf4/bench.py
+-rwxr-xr-x  2.0 unx  8865608 b- defN 24-Apr-07 19:29 bpf4/core.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     9640 b- defN 24-Apr-07 19:29 bpf4/core.pyi
+-rwxr-xr-x  2.0 unx   176933 b- defN 24-Apr-07 19:29 bpf4/core.pyx
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:29 bpf4/py.typed
+-rw-r--r--  2.0 unx     1859 b- defN 24-Apr-07 19:29 bpf4/arraytools.py
+-rw-r--r--  2.0 unx      341 b- defN 24-Apr-07 19:29 bpf4/config.py
+-rw-r--r--  2.0 unx     1289 b- defN 24-Apr-07 19:29 bpf4/pyinterp.py
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-07 19:29 bpf4-1.9.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     5126 b- defN 24-Apr-07 19:29 bpf4-1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      148 b- defN 24-Apr-07 19:29 bpf4-1.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1394 b- defN 24-Apr-07 19:29 bpf4-1.9.0.dist-info/RECORD
+22 files, 9122560 bytes uncompressed, 2482612 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -1,58 +1,67 @@
-Filename: bpf4/__init__.py
+Filename: bpf4/
 Comment: 
 
-Filename: bpf4/api.py
+Filename: bpf4.libs/
 Comment: 
 
-Filename: bpf4/arraytools.py
+Filename: bpf4-1.9.0.dist-info/
 Comment: 
 
-Filename: bpf4/bench.py
+Filename: bpf4/plot.py
 Comment: 
 
-Filename: bpf4/config.py
+Filename: bpf4/util.py
 Comment: 
 
-Filename: bpf4/core.cp39-win_amd64.pyd
+Filename: bpf4/version.py
 Comment: 
 
-Filename: bpf4/core.pyi
+Filename: bpf4/csvtools.py
 Comment: 
 
-Filename: bpf4/core.pyx
+Filename: bpf4/tests.py
 Comment: 
 
-Filename: bpf4/csvtools.py
+Filename: bpf4/__init__.py
 Comment: 
 
-Filename: bpf4/plot.py
+Filename: bpf4/api.py
 Comment: 
 
-Filename: bpf4/py.typed
+Filename: bpf4/bench.py
 Comment: 
 
-Filename: bpf4/pyinterp.py
+Filename: bpf4/core.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: bpf4/tests.py
+Filename: bpf4/core.pyi
 Comment: 
 
-Filename: bpf4/util.py
+Filename: bpf4/core.pyx
 Comment: 
 
-Filename: bpf4/version.py
+Filename: bpf4/py.typed
+Comment: 
+
+Filename: bpf4/arraytools.py
+Comment: 
+
+Filename: bpf4/config.py
+Comment: 
+
+Filename: bpf4/pyinterp.py
 Comment: 
 
-Filename: bpf4-1.8.8.dist-info/METADATA
+Filename: bpf4-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bpf4-1.8.8.dist-info/WHEEL
+Filename: bpf4-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: bpf4-1.8.8.dist-info/top_level.txt
+Filename: bpf4-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: bpf4-1.8.8.dist-info/RECORD
+Filename: bpf4-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## bpf4/__init__.py

 * *Ordering differences only*

```diff
@@ -1,12 +1,12 @@
-from . import core
-from .core import (
-    BpfInterface,
-    BpfBase,
-    blend,
-    
-)
-
-from .api import *
-from .config import CONFIG
-from .version import __version__
-from .util import asbpf
+from . import core
+from .core import (
+    BpfInterface,
+    BpfBase,
+    blend,
+    
+)
+
+from .api import *
+from .config import CONFIG
+from .version import __version__
+from .util import asbpf
```

## bpf4/api.py

 * *Ordering differences only*

```diff
@@ -1,585 +1,585 @@
-"""
-## High-level API for bpf4
-
-The API allows a high-level and flexible interface to the core of bpf4,
-which is implemented in cython for efficiency. 
-
-### API vs core
-
-These three curves, *a*, *b* and *c* define the same linear break-point-function
-The first two definitions, *a* and *b*, use the high-level API, which allows for
-points to be defined as a flat sequence, as tuples of (x, y). The *core* classes
-need to be instantiated with two arrays of *x* and *y* values, as in *c*
-
-```python
-
-from bpf4 import *
-a = linear(0, 0, 1, 2.5, 3, 10)
-b = linear((0, 0), (1, 2.5), (3, 10))
-c = core.Linear([0, 1, 3], [0, 2.5, 10])
-```
-
-"""
-from __future__ import annotations
-
-from . import core
-from . import util
-
-
-
-def linear(*args) -> core.Linear:
-    """
-    Construct a Linear bpf.
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-    
-    A bpf can be constructed in multiple ways, all of which result
-    in the same Linear instance:
-
-    ```python
-
-    linear(x0, y0, x1, y1, ...)
-    linear((x0, y0), (x1, y1), ...)
-    linear({x0:y0, x1:y1, ...})
-    ```
-
-    Example
-    -------
-
-    ```python
-    from bpf4 import *
-    a = linear([0, 2, 3.5, 10], [0.1, 0.5, -3.5,  4])
-    a.plot()
-    ```
-    ![](assets/Linear.png)
-    """
-    X, Y, kws = util.parseargs(*args)
-    if kws:
-        raise ValueError("linear does not take any keyword")
-    return core.Linear(X, Y)
-    
-
-def expon(*args, **kws) -> core.Expon:
-    """
-    Construct an Expon bpf (a bpf with exponential interpolation)
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-        exp: the exponent to use
-        numiter: Number of iterations. A higher number accentuates the effect
-        
-    A bpf can be constructed in multiple ways:
-
-    ```python
-    expon(x0, y0, x1, y1, ..., exp=exponent)
-    expon(exponent, x0, y0, x1, y1, ...)
-    expon((x0, y0), (x1, y1), ..., exp=exponent)
-    expon({x0:y0, x1:y1, ...}, exp=exponent)
-    ```
-    
-    Example
-    -------
-
-    ```python
-    from bpf4 import *
-    import matplotlib.pyplot as plt
-    numplots = 5
-    fig, axs = plt.subplots(2, numplots, tight_layout=True, figsize=(20, 8))
-    for i in range(numplots):
-        exp = i+1
-        expon(0, 0, 1, 1, exp=exp).plot(show=False, axes=axs[0, i])
-        expon(0, 0, 1, 1, exp=1/exp).plot(show=False, axes=axs[1, i])
-        axs[0, i].set_title(f'{exp=}')
-        axs[1, i].set_title(f'exp={1/exp:.2f}')
-        
-    plot.show()
-    ```
-    ![](assets/expon-grid.png)
-
-    """
-    X, Y, kws = util.parseargs(*args, **kws)
-    assert "exp" in kws
-    return core.Expon(X, Y, **kws)
-    
-
-def halfcos(*args, exp=1, numiter=1, **kws) -> core.Halfcos:
-    """
-    Construct a half-cosine bpf (a bpf with half-cosine interpolation)
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-        exp: the exponent to use
-        numiter: Number of iterations. A higher number accentuates the effect
-    
-    A bpf can be constructed in multiple ways:
-
-    ```python
-
-    halfcos(x0, y0, x1, y1, ...)
-    halfcos((x0, y0), (x1, y1), ...)
-    halfcos({x0:y0, x1:y1, ...})
-    ```
-
-    ```python
-    a = halfcos([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
-    b = halfcos(*a.points(), exp=2)
-    c = halfcos(*a.points(), exp=0.5)
-    fig, axes = plt.subplots(1, 3, figsize=(16, 4), tight_layout=True)
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1], show=False)
-    c.plot(axes=axes[2])
-    ```
-    ![](assets/Halfcos.png)
-
-    
-    """
-    X, Y, kws = util.parseargs(*args, **kws)
-    return core.Halfcos(X, Y, exp=exp, numiter=numiter, **kws)  
-
-
-halfcosexp = halfcos
-
-
-def halfcosm(*args, **kws) -> core.Halfcosm:
-    """
-    Halfcos interpolation with symmetric exponent
-
-    When used with an exponent, the exponent is inverted for downwards 
-    segments `(y1 > y0)`
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-        exp: exponent to apply prior to cosine interpolation. The higher the exponent, the
-            more skewed to the right the shape will be
-        numiter: Number of iterations. A higher number accentuates the effect
-    
-    Returns:
-        (core.Halfcosm) A bpf with symmetric cosine interpolation
-
-
-    A bpf can be constructed in multiple ways:
-
-    ```python
-
-    halfcosm(x0, y0, x1, y1, ..., exp=2.0)
-    halfcosm(2.0, x0, y0, x1, y1, ...)    # The exponent can be placed first
-    halfcosm((x0, y0), (x1, y1), ...)
-    halfcosm({x0:y0, x1:y1, ...})
-    ```
-
-    ```python
-    from bpf4 import *
-    a = halfcosm(0, 0.1,
-                 1, 0.5,
-                 3, 3.5,
-                 10, 1, exp=2)
-    b = halfcosm(*a.points(), exp=2)
-    fig, axes = plt.subplots(1, 2, figsize=(16, 4))
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1])
-    ```
-    ![](assets/Halfcosm.png)
-
-
-    """
-    X, Y, kws = util.parseargs(*args, **kws)
-    return core.Halfcosm(X, Y, **kws)
-
-
-def spline(*args) -> core.Spline:
-    """
-    Construct a cubic-spline bpf 
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-    
-    Returns:
-        (core.Spline) A Spline bpf
-    
-
-    A bpf can be constructed in multiple ways:
-
-    ```python
-    spline(x0, y0, x1, y1, ...)
-    spline((x0, y0), (x1, y1), ...)
-    spline({x0:y0, x1:y1, ...})
-    ```
-
-    ```python
-    from bpf4 import *
-    a = smooth(0, 0.1, 1, 0.5, 3, -3.5, 10, 1)
-    b = spline(*a.points())
-    fig, axes = plt.subplots(1, 2, figsize=(12, 4))
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1])
-    ```
-    ![](assets/Spline.png)
-    """
-    X, Y, kws = util.parseargs(*args)
-    return core.Spline(X, Y)
-
-
-def uspline(*args) -> core.USpline: 
-    """
-    Construct a univariate cubic-spline bpf 
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-    
-    Returns:
-        (core.USpline) A USpline bpf
-
-    A bpf can be constructed in multiple ways:
-
-    ```python
-    uspline(x0, y0, x1, y1, ...)
-    uspline((x0, y0), (x1, y1), ...)
-    uspline({x0:y0, x1:y1, ...})
-    ```
-
-    ```python
-    from bpf4 import *
-    a = spline(0, 0.1, 1, 0.5, 3, -3.5, 10, 1)
-    b = uspline(*a.points())
-    
-    fig, axes = plt.subplots(1, 2, figsize=(12, 4), sharey=True, tight_layout=True)
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1])
-    ```
-    ![](assets/Uspline.png)
-
-    !!! info "See Also"
-
-        * [spline](#spline)
-        * [pchip](#pchip)
-
-    """
-    X, Y, kws = util.parseargs(*args)
-    return core.USpline(X, Y)
-
-
-def nointerpol(*args) -> core.NoInterpol:
-    """
-    A bpf with floor interpolation
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-    
-    A bpf can be constructed in multiple ways:
-
-        nointerpol(x0, y0, x1, y1, ...)
-        nointerpol((x0, y0), (x1, y1), ...)
-        nointerpol({x0:y0, x1:y1, ...})
-
-    ```python
-    a = linear([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
-    b = nointerpol(*a.points())
-    c = nearest(*a.points())
-    fig, axes = plt.subplots(1, 3, figsize=(15, 4), tight_layout=True)
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1], show=False)
-    c.plot(axes=axes[2])
-    ```
-    ![](assets/NoInterpol.png)
-    """
-    X, Y, kws = util.parseargs(*args)
-    return core.NoInterpol(X, Y, **kws)
-    
-
-def nearest(*args) -> core.Nearest:
-    """
-    A bpf with floor interpolation
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-                a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-                or two arrays `xs` and `ys`
-
-    A bpf can be constructed in multiple ways:
-
-        nearest(x0, y0, x1, y1, ...)
-        nearest((x0, y0), (x1, y1), ...)
-        nearest({x0:y0, x1:y1, ...})
-
-    ```python
-    a = linear([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
-    b = nointerpol(*a.points())
-    c = nearest(*a.points())
-    fig, axes = plt.subplots(1, 3, figsize=(15, 4), tight_layout=True)
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1], show=False)
-    c.plot(axes=axes[2])
-    ```
-    ![](assets/NoInterpol.png)
-    """
-    X, Y, kws = util.parseargs(*args)
-    return core.Nearest(X, Y, **kws)
-
-
-def smooth(*args, numiter=1) -> core.Smooth:
-    """
-    A bpf with smoothstep interpolation. 
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-        numiter: determines the number of smoothstep steps applied 
-            (see https://en.wikipedia.org/wiki/Smoothstep)
-
-    Returns:
-        (core.Smooth) A bpf with smoothstep interpolation
-
-    ```python
-
-    from bpf4.api import *
-    a = smooth((0, 0.1), (1, 0.5), (3, -3.5), (10, 1))
-    a.plot()
-    ```
-    ![](assets/Smooth.png)
-
-    !!! info "See Also"
-
-        * [smoother](#smoother)
-    """
-    X, Y, kws = util.parseargs(*args)
-    return core.Smooth(X, Y, numiter=numiter)
-
-
-def smoother(*args) -> core.Smoother:
-    """
-    A bpf with smootherstep interpolation 
-
-    This bpf uses Perlin's variation on smoothstep,
-    see https://en.wikipedia.org/wiki/Smoothstep)
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-    
-    Returns:
-        (core.Smoother) A bpf with smootherstep interpolation
-    
-
-    ```python
-    from bpf4 import *
-    a = smooth(0, 0.1, 
-               1, 0.5, 
-               3, -3.5, 
-               10, 1)
-    b = smoother(*a.points())
-    fig, axes = plt.subplots(1, 2, figsize=(12, 4))
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1])
-    ```
-    ![](assets/Smoother.png)
-    """
-    X, Y, kws = util.parseargs(*args)
-    return core.Smoother(X, Y)
-
-
-def multi(*args):
-    """
-    A bpf with a per-pair interpolation
-
-    Example
-    -------
-
-    ```python
-    
-    # (0,0) --linear-- (1,10) --expon(3)-- (2,3) --expon(3)-- (10, -1) --halfcos-- (20,0)
-
-    multi(0, 0,   'linear' 
-          1, 10,  'expon(3)', 
-          2, 3,   # assumes previous interpolation 
-          10, -1, 'halfcos'      
-          20, 0)
-    
-    # also the following syntax is possible
-    multi((0, 0, 'linear')
-          (1, 10, 'expon(3)'), 
-          (2, 3), 
-          (10, -1, 'halfcos'), 
-          (20, 0))
-    ```
-    """
-    xs, ys, interpolations = util.multi_parseargs(args)
-    return core.Multi(xs, ys, interpolations)
-
-
-def pchip(*args):
-    """
-    Monotonic Cubic Hermite Intepolation
-
-    Args:
-        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
-            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
-            or two arrays `xs` and `ys`
-    
-    A bpf can be constructed in multiple ways:
-
-    ```python
-
-    pchip(x0, y0, x1, y1, ...)
-    pchip((x0, y0), (x1, y1), ...)
-    pchip({x0:y0, x1:y1, ...})
-
-
-    >>> a = core.Smoother([0, 1, 3, 10, 12, 12.5], [0.1, 0.5, -3.5,  1, 4.5, -1])
-    >>> b = core.Spline(*a.points())
-    >>> c = pchip(*a.points())
-
-    >>> fig, axes = plt.subplots(1, 3, figsize=(16, 4), sharey=True, tight_layout=True)
-    >>> a.plot(axes=axes[0], show=False)
-    >>> b.plot(axes=axes[1], show=False)
-    >>> c.plot()
-    ``` 
-    ![](assets/pchip.png)   
-    """
-    from . import pyinterp
-    xs, ys, kws = util.parseargs(*args)
-    return pyinterp.Pchip(xs, ys, **kws)
-
-
-def const(value) -> core.Const:
-    """
-    A bpf which always returns a constant value
-
-    Args:
-        value: the constant value
-
-    Example
-    -------
-
-    ```python
-    
-    >>> c5 = const(5)
-    >>> c5(10) 
-    5
-    ```
-    
-    """
-    return core.Const(value)
-
-
-def slope(slope:float, offset=0., bounds: tuple[float, float] = None) -> core.Slope:
-    """
-    Generate a straight line with the given slope and offset 
-
-    This is the same as linear(0, offset, 1, slope)
-
-    Example
-    -------
-
-    ```python
-
-    >>> a = slope(0.5, 1)
-    >>> a
-    Slope[-inf:inf]
-    >>> a[0:10].plot()
-    ```
-    ![](assets/slope-plot.png)
-    """
-    return core.Slope(slope, offset, bounds=bounds)
-
-
-def stack(*bpfs) -> core.Stack:
-    """
-    A bpf representing a stack of bpf
-
-    Within a Stack, a bpf does not have outbound values. When evaluated
-    outside its bounds the bpf below is used, iteratively until the
-    lowest bpf is reached. Only the lowest bpf is evaluated outside its
-    bounds
-
-    Args:
-        bpfs: a sequence of bpfs
-
-    Returns:
-        (core.Stack) A stacked bpf
-
-
-    Example
-    -------
-
-    ```python
-    # Interval    bpf
-    # [0, 3]      a
-    # (3, 4]      b
-    # (4, 10]     c
-
-    from bpf4 import *
-    import matplotlib.pyplot as plt
-    a = linear(0, 0, 3, 1)
-    b = linear(2, 9, 4, 10)
-    c = halfcos(0, 0, 10, 10)
-    s = core.Stack((a, b, c))
-
-    ax = plt.subplot(111)
-    a.plot(color="#f00", alpha=0.4, axes=ax, linewidth=4, show=False)
-    b.plot(color="#00f", alpha=0.4, axes=ax, linewidth=4, show=False)
-    c.plot(color="#f0f", alpha=0.4, axes=ax, linewidth=4, show=False)
-    s.plot(axes=ax, linewidth=2, color="#000", linestyle='dotted')
-    ```
-    ![](assets/stack2.png)
-
-    """
-    if len(bpfs) == 1 and isinstance(bpfs[0], (list, tuple)):
-        bpfs = bpfs[0]
-    return core.Stack(bpfs)
-
-
-def blendshape(shape0:str, shape1:str, mix, points) -> core.BpfInterface:
-    """
-    Create a bpf blending two interpolation forms
-
-    Args:
-        shape0: a description of the first interpolation
-        shape1: a description of the second interpolation
-        mix (float | core.BpfInterface): blend factor. 
-            A value between 0 (use only `shape0`)
-            and 1 (use only `shape1`). A value of `0.5` will result in
-            an average between the first and second interpolation kind.
-            Can be a bpf itself, returning the mix value at any x value
-        points: either a tuple `(x0, y0, x1, y1, ...)` or a tuple `(xs, ys)`
-            where *xs* and *ys* are lists/arrays containing the *x* and *y*
-            coordinates of the points
-
-    Returns:
-        (core.BpfInterface) A bpf blending two different interpolation kinds
-
-    Example
-    -------
-
-    ```python
-
-    from bpf4 import *
-    a = blendshape('halfcos(2.0)', 'linear', mix=0.5, points=(0, 0, 1, 1))
-    halfcos(0, 0, 1, 1, exp=2).plot(color='red')
-    linear(0, 0, 1, 1).plot(color='blue')
-    a.plot(color='green')
-    ```
-    ![](assets/blend1.png)
-    """
-    X, Y, kws = util.parseargs(*points)
-    a = makebpf(shape0, X, Y)
-    b = makebpf(shape1, X, Y)
-    return core.blend(a, b, mix)
-
-
+"""
+## High-level API for bpf4
+
+The API allows a high-level and flexible interface to the core of bpf4,
+which is implemented in cython for efficiency. 
+
+### API vs core
+
+These three curves, *a*, *b* and *c* define the same linear break-point-function
+The first two definitions, *a* and *b*, use the high-level API, which allows for
+points to be defined as a flat sequence, as tuples of (x, y). The *core* classes
+need to be instantiated with two arrays of *x* and *y* values, as in *c*
+
+```python
+
+from bpf4 import *
+a = linear(0, 0, 1, 2.5, 3, 10)
+b = linear((0, 0), (1, 2.5), (3, 10))
+c = core.Linear([0, 1, 3], [0, 2.5, 10])
+```
+
+"""
+from __future__ import annotations
+
+from . import core
+from . import util
+
+
+
+def linear(*args) -> core.Linear:
+    """
+    Construct a Linear bpf.
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+    
+    A bpf can be constructed in multiple ways, all of which result
+    in the same Linear instance:
+
+    ```python
+
+    linear(x0, y0, x1, y1, ...)
+    linear((x0, y0), (x1, y1), ...)
+    linear({x0:y0, x1:y1, ...})
+    ```
+
+    Example
+    -------
+
+    ```python
+    from bpf4 import *
+    a = linear([0, 2, 3.5, 10], [0.1, 0.5, -3.5,  4])
+    a.plot()
+    ```
+    ![](assets/Linear.png)
+    """
+    X, Y, kws = util.parseargs(*args)
+    if kws:
+        raise ValueError("linear does not take any keyword")
+    return core.Linear(X, Y)
+    
+
+def expon(*args, **kws) -> core.Expon:
+    """
+    Construct an Expon bpf (a bpf with exponential interpolation)
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+        exp: the exponent to use
+        numiter: Number of iterations. A higher number accentuates the effect
+        
+    A bpf can be constructed in multiple ways:
+
+    ```python
+    expon(x0, y0, x1, y1, ..., exp=exponent)
+    expon(exponent, x0, y0, x1, y1, ...)
+    expon((x0, y0), (x1, y1), ..., exp=exponent)
+    expon({x0:y0, x1:y1, ...}, exp=exponent)
+    ```
+    
+    Example
+    -------
+
+    ```python
+    from bpf4 import *
+    import matplotlib.pyplot as plt
+    numplots = 5
+    fig, axs = plt.subplots(2, numplots, tight_layout=True, figsize=(20, 8))
+    for i in range(numplots):
+        exp = i+1
+        expon(0, 0, 1, 1, exp=exp).plot(show=False, axes=axs[0, i])
+        expon(0, 0, 1, 1, exp=1/exp).plot(show=False, axes=axs[1, i])
+        axs[0, i].set_title(f'{exp=}')
+        axs[1, i].set_title(f'exp={1/exp:.2f}')
+        
+    plot.show()
+    ```
+    ![](assets/expon-grid.png)
+
+    """
+    X, Y, kws = util.parseargs(*args, **kws)
+    assert "exp" in kws
+    return core.Expon(X, Y, **kws)
+    
+
+def halfcos(*args, exp=1, numiter=1, **kws) -> core.Halfcos:
+    """
+    Construct a half-cosine bpf (a bpf with half-cosine interpolation)
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+        exp: the exponent to use
+        numiter: Number of iterations. A higher number accentuates the effect
+    
+    A bpf can be constructed in multiple ways:
+
+    ```python
+
+    halfcos(x0, y0, x1, y1, ...)
+    halfcos((x0, y0), (x1, y1), ...)
+    halfcos({x0:y0, x1:y1, ...})
+    ```
+
+    ```python
+    a = halfcos([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
+    b = halfcos(*a.points(), exp=2)
+    c = halfcos(*a.points(), exp=0.5)
+    fig, axes = plt.subplots(1, 3, figsize=(16, 4), tight_layout=True)
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1], show=False)
+    c.plot(axes=axes[2])
+    ```
+    ![](assets/Halfcos.png)
+
+    
+    """
+    X, Y, kws = util.parseargs(*args, **kws)
+    return core.Halfcos(X, Y, exp=exp, numiter=numiter, **kws)  
+
+
+halfcosexp = halfcos
+
+
+def halfcosm(*args, **kws) -> core.Halfcosm:
+    """
+    Halfcos interpolation with symmetric exponent
+
+    When used with an exponent, the exponent is inverted for downwards 
+    segments `(y1 > y0)`
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+        exp: exponent to apply prior to cosine interpolation. The higher the exponent, the
+            more skewed to the right the shape will be
+        numiter: Number of iterations. A higher number accentuates the effect
+    
+    Returns:
+        (core.Halfcosm) A bpf with symmetric cosine interpolation
+
+
+    A bpf can be constructed in multiple ways:
+
+    ```python
+
+    halfcosm(x0, y0, x1, y1, ..., exp=2.0)
+    halfcosm(2.0, x0, y0, x1, y1, ...)    # The exponent can be placed first
+    halfcosm((x0, y0), (x1, y1), ...)
+    halfcosm({x0:y0, x1:y1, ...})
+    ```
+
+    ```python
+    from bpf4 import *
+    a = halfcosm(0, 0.1,
+                 1, 0.5,
+                 3, 3.5,
+                 10, 1, exp=2)
+    b = halfcosm(*a.points(), exp=2)
+    fig, axes = plt.subplots(1, 2, figsize=(16, 4))
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1])
+    ```
+    ![](assets/Halfcosm.png)
+
+
+    """
+    X, Y, kws = util.parseargs(*args, **kws)
+    return core.Halfcosm(X, Y, **kws)
+
+
+def spline(*args) -> core.Spline:
+    """
+    Construct a cubic-spline bpf 
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+    
+    Returns:
+        (core.Spline) A Spline bpf
+    
+
+    A bpf can be constructed in multiple ways:
+
+    ```python
+    spline(x0, y0, x1, y1, ...)
+    spline((x0, y0), (x1, y1), ...)
+    spline({x0:y0, x1:y1, ...})
+    ```
+
+    ```python
+    from bpf4 import *
+    a = smooth(0, 0.1, 1, 0.5, 3, -3.5, 10, 1)
+    b = spline(*a.points())
+    fig, axes = plt.subplots(1, 2, figsize=(12, 4))
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1])
+    ```
+    ![](assets/Spline.png)
+    """
+    X, Y, kws = util.parseargs(*args)
+    return core.Spline(X, Y)
+
+
+def uspline(*args) -> core.USpline: 
+    """
+    Construct a univariate cubic-spline bpf 
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+    
+    Returns:
+        (core.USpline) A USpline bpf
+
+    A bpf can be constructed in multiple ways:
+
+    ```python
+    uspline(x0, y0, x1, y1, ...)
+    uspline((x0, y0), (x1, y1), ...)
+    uspline({x0:y0, x1:y1, ...})
+    ```
+
+    ```python
+    from bpf4 import *
+    a = spline(0, 0.1, 1, 0.5, 3, -3.5, 10, 1)
+    b = uspline(*a.points())
+    
+    fig, axes = plt.subplots(1, 2, figsize=(12, 4), sharey=True, tight_layout=True)
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1])
+    ```
+    ![](assets/Uspline.png)
+
+    !!! info "See Also"
+
+        * [spline](#spline)
+        * [pchip](#pchip)
+
+    """
+    X, Y, kws = util.parseargs(*args)
+    return core.USpline(X, Y)
+
+
+def nointerpol(*args) -> core.NoInterpol:
+    """
+    A bpf with floor interpolation
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+    
+    A bpf can be constructed in multiple ways:
+
+        nointerpol(x0, y0, x1, y1, ...)
+        nointerpol((x0, y0), (x1, y1), ...)
+        nointerpol({x0:y0, x1:y1, ...})
+
+    ```python
+    a = linear([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
+    b = nointerpol(*a.points())
+    c = nearest(*a.points())
+    fig, axes = plt.subplots(1, 3, figsize=(15, 4), tight_layout=True)
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1], show=False)
+    c.plot(axes=axes[2])
+    ```
+    ![](assets/NoInterpol.png)
+    """
+    X, Y, kws = util.parseargs(*args)
+    return core.NoInterpol(X, Y, **kws)
+    
+
+def nearest(*args) -> core.Nearest:
+    """
+    A bpf with floor interpolation
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+                a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+                or two arrays `xs` and `ys`
+
+    A bpf can be constructed in multiple ways:
+
+        nearest(x0, y0, x1, y1, ...)
+        nearest((x0, y0), (x1, y1), ...)
+        nearest({x0:y0, x1:y1, ...})
+
+    ```python
+    a = linear([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
+    b = nointerpol(*a.points())
+    c = nearest(*a.points())
+    fig, axes = plt.subplots(1, 3, figsize=(15, 4), tight_layout=True)
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1], show=False)
+    c.plot(axes=axes[2])
+    ```
+    ![](assets/NoInterpol.png)
+    """
+    X, Y, kws = util.parseargs(*args)
+    return core.Nearest(X, Y, **kws)
+
+
+def smooth(*args, numiter=1) -> core.Smooth:
+    """
+    A bpf with smoothstep interpolation. 
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+        numiter: determines the number of smoothstep steps applied 
+            (see https://en.wikipedia.org/wiki/Smoothstep)
+
+    Returns:
+        (core.Smooth) A bpf with smoothstep interpolation
+
+    ```python
+
+    from bpf4.api import *
+    a = smooth((0, 0.1), (1, 0.5), (3, -3.5), (10, 1))
+    a.plot()
+    ```
+    ![](assets/Smooth.png)
+
+    !!! info "See Also"
+
+        * [smoother](#smoother)
+    """
+    X, Y, kws = util.parseargs(*args)
+    return core.Smooth(X, Y, numiter=numiter)
+
+
+def smoother(*args) -> core.Smoother:
+    """
+    A bpf with smootherstep interpolation 
+
+    This bpf uses Perlin's variation on smoothstep,
+    see https://en.wikipedia.org/wiki/Smoothstep)
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+    
+    Returns:
+        (core.Smoother) A bpf with smootherstep interpolation
+    
+
+    ```python
+    from bpf4 import *
+    a = smooth(0, 0.1, 
+               1, 0.5, 
+               3, -3.5, 
+               10, 1)
+    b = smoother(*a.points())
+    fig, axes = plt.subplots(1, 2, figsize=(12, 4))
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1])
+    ```
+    ![](assets/Smoother.png)
+    """
+    X, Y, kws = util.parseargs(*args)
+    return core.Smoother(X, Y)
+
+
+def multi(*args):
+    """
+    A bpf with a per-pair interpolation
+
+    Example
+    -------
+
+    ```python
+    
+    # (0,0) --linear-- (1,10) --expon(3)-- (2,3) --expon(3)-- (10, -1) --halfcos-- (20,0)
+
+    multi(0, 0,   'linear' 
+          1, 10,  'expon(3)', 
+          2, 3,   # assumes previous interpolation 
+          10, -1, 'halfcos'      
+          20, 0)
+    
+    # also the following syntax is possible
+    multi((0, 0, 'linear')
+          (1, 10, 'expon(3)'), 
+          (2, 3), 
+          (10, -1, 'halfcos'), 
+          (20, 0))
+    ```
+    """
+    xs, ys, interpolations = util.multi_parseargs(args)
+    return core.Multi(xs, ys, interpolations)
+
+
+def pchip(*args):
+    """
+    Monotonic Cubic Hermite Intepolation
+
+    Args:
+        args: either a flat list of coordinates in the form `x0, y0, x1, y1, ...`,
+            a list of tuples `(x0, y0), (x1, y1), ...`, a dict `{x0:y0, x1:y1, ...}`
+            or two arrays `xs` and `ys`
+    
+    A bpf can be constructed in multiple ways:
+
+    ```python
+
+    pchip(x0, y0, x1, y1, ...)
+    pchip((x0, y0), (x1, y1), ...)
+    pchip({x0:y0, x1:y1, ...})
+
+
+    >>> a = core.Smoother([0, 1, 3, 10, 12, 12.5], [0.1, 0.5, -3.5,  1, 4.5, -1])
+    >>> b = core.Spline(*a.points())
+    >>> c = pchip(*a.points())
+
+    >>> fig, axes = plt.subplots(1, 3, figsize=(16, 4), sharey=True, tight_layout=True)
+    >>> a.plot(axes=axes[0], show=False)
+    >>> b.plot(axes=axes[1], show=False)
+    >>> c.plot()
+    ``` 
+    ![](assets/pchip.png)   
+    """
+    from . import pyinterp
+    xs, ys, kws = util.parseargs(*args)
+    return pyinterp.Pchip(xs, ys, **kws)
+
+
+def const(value) -> core.Const:
+    """
+    A bpf which always returns a constant value
+
+    Args:
+        value: the constant value
+
+    Example
+    -------
+
+    ```python
+    
+    >>> c5 = const(5)
+    >>> c5(10) 
+    5
+    ```
+    
+    """
+    return core.Const(value)
+
+
+def slope(slope:float, offset=0., bounds: tuple[float, float] = None) -> core.Slope:
+    """
+    Generate a straight line with the given slope and offset 
+
+    This is the same as linear(0, offset, 1, slope)
+
+    Example
+    -------
+
+    ```python
+
+    >>> a = slope(0.5, 1)
+    >>> a
+    Slope[-inf:inf]
+    >>> a[0:10].plot()
+    ```
+    ![](assets/slope-plot.png)
+    """
+    return core.Slope(slope, offset, bounds=bounds)
+
+
+def stack(*bpfs) -> core.Stack:
+    """
+    A bpf representing a stack of bpf
+
+    Within a Stack, a bpf does not have outbound values. When evaluated
+    outside its bounds the bpf below is used, iteratively until the
+    lowest bpf is reached. Only the lowest bpf is evaluated outside its
+    bounds
+
+    Args:
+        bpfs: a sequence of bpfs
+
+    Returns:
+        (core.Stack) A stacked bpf
+
+
+    Example
+    -------
+
+    ```python
+    # Interval    bpf
+    # [0, 3]      a
+    # (3, 4]      b
+    # (4, 10]     c
+
+    from bpf4 import *
+    import matplotlib.pyplot as plt
+    a = linear(0, 0, 3, 1)
+    b = linear(2, 9, 4, 10)
+    c = halfcos(0, 0, 10, 10)
+    s = core.Stack((a, b, c))
+
+    ax = plt.subplot(111)
+    a.plot(color="#f00", alpha=0.4, axes=ax, linewidth=4, show=False)
+    b.plot(color="#00f", alpha=0.4, axes=ax, linewidth=4, show=False)
+    c.plot(color="#f0f", alpha=0.4, axes=ax, linewidth=4, show=False)
+    s.plot(axes=ax, linewidth=2, color="#000", linestyle='dotted')
+    ```
+    ![](assets/stack2.png)
+
+    """
+    if len(bpfs) == 1 and isinstance(bpfs[0], (list, tuple)):
+        bpfs = bpfs[0]
+    return core.Stack(bpfs)
+
+
+def blendshape(shape0:str, shape1:str, mix, points) -> core.BpfInterface:
+    """
+    Create a bpf blending two interpolation forms
+
+    Args:
+        shape0: a description of the first interpolation
+        shape1: a description of the second interpolation
+        mix (float | core.BpfInterface): blend factor. 
+            A value between 0 (use only `shape0`)
+            and 1 (use only `shape1`). A value of `0.5` will result in
+            an average between the first and second interpolation kind.
+            Can be a bpf itself, returning the mix value at any x value
+        points: either a tuple `(x0, y0, x1, y1, ...)` or a tuple `(xs, ys)`
+            where *xs* and *ys* are lists/arrays containing the *x* and *y*
+            coordinates of the points
+
+    Returns:
+        (core.BpfInterface) A bpf blending two different interpolation kinds
+
+    Example
+    -------
+
+    ```python
+
+    from bpf4 import *
+    a = blendshape('halfcos(2.0)', 'linear', mix=0.5, points=(0, 0, 1, 1))
+    halfcos(0, 0, 1, 1, exp=2).plot(color='red')
+    linear(0, 0, 1, 1).plot(color='blue')
+    a.plot(color='green')
+    ```
+    ![](assets/blend1.png)
+    """
+    X, Y, kws = util.parseargs(*points)
+    a = makebpf(shape0, X, Y)
+    b = makebpf(shape1, X, Y)
+    return core.blend(a, b, mix)
+
+
```

## bpf4/arraytools.py

 * *Ordering differences only*

```diff
@@ -1,78 +1,78 @@
-from __future__ import annotations
-import numpy as np
-
-
-def arrayslice(x0:float, x1:float, X:np.ndarray, *Ys:np.ndarray) -> np.ndarray:
-    """
-    Slice a sorted array and linked arrays as if they where a bpf
-
-    Args:
-        x0, x1: where to perform the slices
-        x: the array used to perform the slice
-        ys: one or more secondary arrays which represent a linear bpf,
-            where y = f(x) 
-        
-    Example
-    =======
-
-    X = np.linspace(0, 10, 11, dtype=float)
-    Y = X*2
-
-    x, y = arrayslice(3.5, 7, X, Y)
-   
-    """
-    if x0 >= x1:
-        raise ValueError("x0 should be less than x1")
-
-    if x0 > X[0]:
-        i0 = np.searchsorted(X, x0) - 1    
-    else:
-        i0 = 0
-        x0 = X[0]
-
-    if x1 < X[-1]:
-        i1 = np.searchsorted(X, x1) + 1
-    else:
-        i1 = len(X)
-        x1 = X[-1]
-
-    X2 = X[i0:i1].copy()
-    X2[0] = x0
-    X2[-1] = min(x1, X2[-1])
-    out = [X2]  
-    for Y in Ys:
-        Y2 = Y[i0:i1].copy()
-        y0, y1 = np.interp((x0, x1), X, Y)
-        Y2[0] = y0
-        Y2[-1] = y1
-        out.append(Y2)
-    return out 
-
-
-def interlace_arrays(*arrays: np.ndarray) -> np.ndarray:
-    """
-    Interweave multiple arrays into a flat array in the form
-
-    Example::
-
-        A = [a0, a1, a2, ...]
-        B = [b0, b1, b2, ...]
-        C = [c0, c1, c2, ...]
-        interlace(A, B, C)
-        -> [a0, b0, c0, a1, b1, c1, ...]
-
-    Args:
-        *arrays (): the arrays to interleave. They should be 1D arrays of the
-            same length
-
-    Returns:
-        a 1D array with the elements of the given arrays interleaved
-
-    """
-    assert all(a.size == arrays[0].size and a.dtype == arrays[0].dtype for a in arrays)
-    size = arrays[0].size * len(arrays)
-    out = np.empty((size,), dtype=arrays[0].dtype)
-    for i, a in enumerate(arrays):
-        out[i::len(arrays)] = a
-    return out
-
+from __future__ import annotations
+import numpy as np
+
+
+def arrayslice(x0:float, x1:float, X:np.ndarray, *Ys:np.ndarray) -> np.ndarray:
+    """
+    Slice a sorted array and linked arrays as if they where a bpf
+
+    Args:
+        x0, x1: where to perform the slices
+        x: the array used to perform the slice
+        ys: one or more secondary arrays which represent a linear bpf,
+            where y = f(x) 
+        
+    Example
+    =======
+
+    X = np.linspace(0, 10, 11, dtype=float)
+    Y = X*2
+
+    x, y = arrayslice(3.5, 7, X, Y)
+   
+    """
+    if x0 >= x1:
+        raise ValueError("x0 should be less than x1")
+
+    if x0 > X[0]:
+        i0 = np.searchsorted(X, x0) - 1    
+    else:
+        i0 = 0
+        x0 = X[0]
+
+    if x1 < X[-1]:
+        i1 = np.searchsorted(X, x1) + 1
+    else:
+        i1 = len(X)
+        x1 = X[-1]
+
+    X2 = X[i0:i1].copy()
+    X2[0] = x0
+    X2[-1] = min(x1, X2[-1])
+    out = [X2]  
+    for Y in Ys:
+        Y2 = Y[i0:i1].copy()
+        y0, y1 = np.interp((x0, x1), X, Y)
+        Y2[0] = y0
+        Y2[-1] = y1
+        out.append(Y2)
+    return out 
+
+
+def interlace_arrays(*arrays: np.ndarray) -> np.ndarray:
+    """
+    Interweave multiple arrays into a flat array in the form
+
+    Example::
+
+        A = [a0, a1, a2, ...]
+        B = [b0, b1, b2, ...]
+        C = [c0, c1, c2, ...]
+        interlace(A, B, C)
+        -> [a0, b0, c0, a1, b1, c1, ...]
+
+    Args:
+        *arrays (): the arrays to interleave. They should be 1D arrays of the
+            same length
+
+    Returns:
+        a 1D array with the elements of the given arrays interleaved
+
+    """
+    assert all(a.size == arrays[0].size and a.dtype == arrays[0].dtype for a in arrays)
+    size = arrays[0].size * len(arrays)
+    out = np.empty((size,), dtype=arrays[0].dtype)
+    for i, a in enumerate(arrays):
+        out[i::len(arrays)] = a
+    return out
+
```

## bpf4/bench.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-import bpf3
-import numpy
-from bpf3 import bpf
-
-def run1():
-    xs = numpy.arange(0, 10, 0.1)
-    ys = numpy.sin(xs)
-    points = zip(xs, ys)
-
-    a = bpf3.Linear(xs, ys)
-    b = bpf.linear(*points)
-
-    xs2 = numpy.arange(0, 10, 0.01)
-    ys2 = a.map(xs2)
-    ys3 = b.map(xs2)
-    c = a * b
-    ys4 = c.map(xs2)
-
-if __name__ == '__main__':
-    run1()
-
-#a.plot(show=False)
-#b.plot(show=False)
+import bpf3
+import numpy
+from bpf3 import bpf
+
+def run1():
+    xs = numpy.arange(0, 10, 0.1)
+    ys = numpy.sin(xs)
+    points = zip(xs, ys)
+
+    a = bpf3.Linear(xs, ys)
+    b = bpf.linear(*points)
+
+    xs2 = numpy.arange(0, 10, 0.01)
+    ys2 = a.map(xs2)
+    ys3 = b.map(xs2)
+    c = a * b
+    ys4 = c.map(xs2)
+
+if __name__ == '__main__':
+    run1()
+
+#a.plot(show=False)
+#b.plot(show=False)
```

## bpf4/config.py

 * *Ordering differences only*

```diff
@@ -1,15 +1,15 @@
-OUTBOUND_DONOTHING = 0
-OUTBOUND_CACHE = 1
-OUTBOUND_SET = 2
-
-CONFIG = {
-    'plot.always_show': False,
-    'preapply.calculate_bounds': True,
-    'crop.outbound_mode': OUTBOUND_CACHE,
-    'integrate.oversample': 10,
-    'integrate.trapz_intervals': 400,
-    'integrate.default_mode':2  # -1: calibrate, 0: trapz, 1: quad, 2: simpsons
-}   
-
-
-
+OUTBOUND_DONOTHING = 0
+OUTBOUND_CACHE = 1
+OUTBOUND_SET = 2
+
+CONFIG = {
+    'plot.always_show': False,
+    'preapply.calculate_bounds': True,
+    'crop.outbound_mode': OUTBOUND_CACHE,
+    'integrate.oversample': 10,
+    'integrate.trapz_intervals': 400,
+    'integrate.default_mode':2  # -1: calibrate, 0: trapz, 1: quad, 2: simpsons
+}   
+
+
+
```

## bpf4/core.pyi

 * *Ordering differences only*

```diff
@@ -1,333 +1,333 @@
-import numpy as np
-from typing import Union, Optional
-
-
-class BpfPointsError(ValueError): pass
-class BpfInversionError(ValueError): pass
-
-
-class BpfInterface:
-    def ntodx(self, N: int) -> float: ...
-    def dxton(self, dx: float) -> int: ...
-    def bounds(self) -> tuple[float, float]: ...
-        
-    @property
-    def x0(self) -> float: ...
-       
-    
-    @property
-    def x1(self) -> float: ...
-       
-    def __add__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
-    
-    def __sub__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
-    
-    def __mul__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
-
-    def __div__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
-
-    def __truediv__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
-
-    def __pow__(a: BpfInterface | float, b: BpfInterface | float, module: float) -> BpfInterface: ...
-
-    def __neg__(self: BpfInterface) -> BpfInterface: ...
-    
-    def __mod__(self, other: BpfInterface | float) -> BpfInterface: ...
-    
-    def __abs__(self) -> BpfInterface: ...
-    
-    def __or__(a: BpfInterface, b: BpfInterface|float) -> BpfInterface: ...
-    
-    def __rshift__(a: BpfInterace, b: BpfInterface|float) -> BpfInterface: ...
-
-    def __lshift__(a: BpfInterace, b: BpfInterface|float) -> BpfInterface: ...
-
-    def __xor__(a: BpfInterace, b: BpfInterface|float) -> BpfInterface: ...
-                
-    def _get_points_for_rendering(self, n: int = -1) -> tuple[np.ndarray, np.ndarray]: ...
-        
-    def render(self, xs: int | np.ndarray | list[float], interpolation: str = 'linear') -> np.ndarray: ...
-    
-    def sampled(self, dx: float, interpolation='linear') -> BpfInterface: ...
-
-    def plot(self, kind: str = 'line', n: int = -1, show: bool = True, axes=None, **keys) -> None: ...
-        
-    def sample_between(self, x0: float, x1: float, dx: float, out: np.ndarray | float | None = None) -> np.ndarray: ...
-        
-    def sampled_between(self, x0: float, x1: float, dx: float, interpolation='linear') -> BpfInterface: ...
-
-    def mapn_between(self, n: int, x0: float, x1: float, out: np.ndarray | None = None) -> np.ndarray: ...
-        
-    def map(self, xs: int | np.ndarray, out: np.ndarray | None = None) -> np.ndarray: ...
-        
-    def concat(self, other: BpfInterface)-> BpfInterface: ...
-        
-    def round(self) -> BpfInterface: ...
-        
-    def rand(self) -> BpfInterface: ...
-        
-    def cos(self) -> BpfInterface: ...
-        
-    def sin(self) -> BpfInterface: ...  
-        
-    def ceil(self) -> BpfInterface: ...
-     
-    def expon(self) -> BpfInterface: ...
-        
-    def floor(self) -> BpfInterface: ...
-    
-    def tanh(self) -> BpfInterface: ... 
-        
-    def abs(self) -> BpfInterface: ...  
-    
-    def sqrt(self) -> BpfInterface: ... 
-        
-    def acos(self) -> BpfInterface: ... 
-        
-    def asin(self) -> BpfInterface: ... 
-        
-    def tan(self) -> BpfInterface: ...  
-        
-    def sinh(self) -> BpfInterface: ... 
-
-    def log10(self) -> BpfInterface: ... 
-
-    def log(self, base: float = 2.718281828459045) -> BpfInterface: ... 
-    
-    def m2f(self) -> BpfInterface: ... 
-
-    def f2m(self) -> BpfInterface: ... 
-    def db2amp(self) -> BpfInterface: ... 
-    def amp2db(self) -> BpfInterface: ... 
-    def clip(self, y0: float = float('-inf'), y1: float = float('inf')) -> BpfInterface: ...
-    def derivative(self) -> BpfInterface: ...
-    def integrated(self) -> BpfInterface: ...
-    def integrate(self) -> float: ...
-    def integrate_between(self, x0: float, x1: float, N: int = 0) -> float: ...
-    def mean(self) -> float: ...
-    def zeros(self, h: float = 0.01, N: int = 0, 
-              x0: float = float('nan'), x1: float = float('nan'), maxzeros: int = 0) -> list[float]: ...
-    def max(self, b: BpfInterface|float) -> BpfInterface: ...
-    def min(self, b: BpfInterface|float) -> BpfInterface: ...
-    def __call__(self, other: float) -> float: ...
-    
-    def keep_slope(self, epsilon: float = 0.) -> BpfInterface: ...
-        
-    def outbound(self, y0: float, y1: float) -> BpfInterface: ...
-        
-    def apply(self, func) -> BpfInterface: ...
-        
-    def preapply(self, func) -> BpfInterface: ...
-        
-    def periodic(self) -> BpfInterface: ...
-       
-    def stretched(self, rx: float, fixpoint: float = 0.) -> BpfInterface: ...
-        
-    def fit_between(self, x0: float, x1: float) -> BpfInterface: ...
-      
-    def shifted(self, dx: float) -> BpfInterface: ...
-        
-    def inverted(self) -> BpfInterface: ...
-        
-    @classmethod
-    def fromseq(cls, *points: float|tuple[float, float], **kws) -> BpfInterface: ...
-        
-    def copy(self) -> BpfInterface: ...
-
-        
-class BpfBase(BpfInterface):
-
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]]
-                 ): ...
-        
-    @property
-    def descriptor(self) -> str: ... 
-            
-    def mapn_between(self, n: int, xstart: float, xend: float, out: np.ndarray|None = None) -> np.ndarray: ...
-       
-    def points(self) -> tuple[np.ndarray, np.ndarray]: ...
-        
-    def clone_with_new_data(self, xs: np.ndarray, ys: np.ndarray) -> BpfInterface: ...
-        
-    def insertpoint(self, x: float, y: float) -> BpfInterface: ...
-        
-    def removepoint(self, x: float) -> BpfInterface: ...
-        
-    def segments(self) -> Iterator[tuple[float, float, float]]: ...
-
-    @property
-    def exp(self) -> float: ...
-        
-
-class Linear(BpfBase): 
-
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]]
-                 ): ...
-
-
-    def inverted(self) -> Linear: ...
-        
-    def flatpairs(self) -> np.ndarray: ...
-        
-
-class Smooth(BpfBase): ...
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]]
-                 ): ...
-
-   
-class Smoother(BpfBase): ...
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]]
-                 ): ...
-
-    
-class Halfcos(BpfBase):
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]],
-                 exp: float = 1.0, numiter: int =1): ...
-    
-
-class Halfcosm(Halfcos):
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]],
-                 exp: float = 1.0, numiter: int =1): ...
-
-
-class Expon(BpfBase):
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]],
-                 exp: float = 1.0, numiter: int =1): ...
-
-
-class Exponm(Expon):
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]],
-                 exp: float = 1.0, numiter: int =1): ...
-
-
-class NoInterpol(BpfBase): ...
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]]
-                 ): ...
-
-    
-class Nearest(BpfBase): ...
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]]
-                 ): ...
-
-
-class Sampled(BpfInterface): 
-    def __init__(self,
-                 samples: np.ndarray,
-                 dx: float,
-                 x0: float = 0.,
-                 interpolation: str = 'linear'): ...
-
-    @property
-    def ys(self) -> np.ndarray: ...
-    
-
-    @property
-    def samplerate(self) -> float: ...
-        
-    @property
-    def xs(self) -> np.ndarray: ...
-        
-    
-    @property
-    def dx(self) -> float: ...
-    
-    def set_interpolation(self, interpolation: str) -> Sampled: ...
-        
-    
-    def flatpairs(self) -> np.ndarray: ...
-        
-
-
-class Spline(BpfInterface): ...
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]]
-                 ): ...
-
-    
-
-class USpline(BpfInterface): ...
-    def __init__(self,
-                 xs: Union[np.ndarray, list[float]],
-                 ys: Union[np.ndarray, list[float]]
-                 ): ...
-
-    
-class Slope(BpfInterface):
-
-    @property
-    def slope(self) -> float: ...
-
-    @slope.setter
-    def slope(self, value: float) -> None: ...
-    
-    @property
-    def offset(self) -> float: ...
-
-    @offset.setter
-    def offset(self, value: float) -> None: ...
-    
-
-    
-class _BpfCompose(BpfInterface): ...
-
-
-class _BpfConcat(BpfInterface): ...
-
-
-class _BpfBlend(BpfInterface): ...
-
-        
-class Multi(BpfInterface): ...
-
-
-class Const(BpfInterface): ...
-
-
-class _MultipleBpfs(BpfInterface):
-
-    def __init__(self, bpfs: list[BpfInterface]): ...
-    
-
-class Max(_MultipleBpfs): ...
-    
-class Min(_MultipleBpfs): ...
-
-class Stack(_MultipleBpfs): ...
-
-
-def brentq(bpf: BpfInterface, x0: float, xa: float, xb: float, xtol=9.9999999999999998e-13, 
-           rtol=4.4408920985006262e-16, max_iter=100) -> tuple[float,int]: ...
-    
-
-def blend(a: BpfInterface, b: BpfInterface, mix=0.5) -> BpfInterface: ...
-
-
-
-def bpf_zero_crossings(b: BpfInterface, 
-                       h: float = 0.01, N: int = 0, 
-                       x0: float = float('nan'), 
-                       x1: float = float('nan'), 
-                       maxzeros: int = 0
-                       ) -> list[float]: ...
-    
+import numpy as np
+from typing import Union, Optional
+
+
+class BpfPointsError(ValueError): pass
+class BpfInversionError(ValueError): pass
+
+
+class BpfInterface:
+    def ntodx(self, N: int) -> float: ...
+    def dxton(self, dx: float) -> int: ...
+    def bounds(self) -> tuple[float, float]: ...
+        
+    @property
+    def x0(self) -> float: ...
+       
+    
+    @property
+    def x1(self) -> float: ...
+       
+    def __add__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
+    
+    def __sub__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
+    
+    def __mul__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
+
+    def __div__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
+
+    def __truediv__(a: BpfInterface | float, b: BpfInterface | float) -> BpfInterface: ...
+
+    def __pow__(a: BpfInterface | float, b: BpfInterface | float, module: float) -> BpfInterface: ...
+
+    def __neg__(self: BpfInterface) -> BpfInterface: ...
+    
+    def __mod__(self, other: BpfInterface | float) -> BpfInterface: ...
+    
+    def __abs__(self) -> BpfInterface: ...
+    
+    def __or__(a: BpfInterface, b: BpfInterface|float) -> BpfInterface: ...
+    
+    def __rshift__(a: BpfInterace, b: BpfInterface|float) -> BpfInterface: ...
+
+    def __lshift__(a: BpfInterace, b: BpfInterface|float) -> BpfInterface: ...
+
+    def __xor__(a: BpfInterace, b: BpfInterface|float) -> BpfInterface: ...
+                
+    def _get_points_for_rendering(self, n: int = -1) -> tuple[np.ndarray, np.ndarray]: ...
+        
+    def render(self, xs: int | np.ndarray | list[float], interpolation: str = 'linear') -> np.ndarray: ...
+    
+    def sampled(self, dx: float, interpolation='linear') -> BpfInterface: ...
+
+    def plot(self, kind: str = 'line', n: int = -1, show: bool = True, axes=None, **keys) -> None: ...
+        
+    def sample_between(self, x0: float, x1: float, dx: float, out: np.ndarray | float | None = None) -> np.ndarray: ...
+        
+    def sampled_between(self, x0: float, x1: float, dx: float, interpolation='linear') -> BpfInterface: ...
+
+    def mapn_between(self, n: int, x0: float, x1: float, out: np.ndarray | None = None) -> np.ndarray: ...
+        
+    def map(self, xs: int | np.ndarray, out: np.ndarray | None = None) -> np.ndarray: ...
+        
+    def concat(self, other: BpfInterface)-> BpfInterface: ...
+        
+    def round(self) -> BpfInterface: ...
+        
+    def rand(self) -> BpfInterface: ...
+        
+    def cos(self) -> BpfInterface: ...
+        
+    def sin(self) -> BpfInterface: ...  
+        
+    def ceil(self) -> BpfInterface: ...
+     
+    def expon(self) -> BpfInterface: ...
+        
+    def floor(self) -> BpfInterface: ...
+    
+    def tanh(self) -> BpfInterface: ... 
+        
+    def abs(self) -> BpfInterface: ...  
+    
+    def sqrt(self) -> BpfInterface: ... 
+        
+    def acos(self) -> BpfInterface: ... 
+        
+    def asin(self) -> BpfInterface: ... 
+        
+    def tan(self) -> BpfInterface: ...  
+        
+    def sinh(self) -> BpfInterface: ... 
+
+    def log10(self) -> BpfInterface: ... 
+
+    def log(self, base: float = 2.718281828459045) -> BpfInterface: ... 
+    
+    def m2f(self) -> BpfInterface: ... 
+
+    def f2m(self) -> BpfInterface: ... 
+    def db2amp(self) -> BpfInterface: ... 
+    def amp2db(self) -> BpfInterface: ... 
+    def clip(self, y0: float = float('-inf'), y1: float = float('inf')) -> BpfInterface: ...
+    def derivative(self) -> BpfInterface: ...
+    def integrated(self) -> BpfInterface: ...
+    def integrate(self) -> float: ...
+    def integrate_between(self, x0: float, x1: float, N: int = 0) -> float: ...
+    def mean(self) -> float: ...
+    def zeros(self, h: float = 0.01, N: int = 0, 
+              x0: float = float('nan'), x1: float = float('nan'), maxzeros: int = 0) -> list[float]: ...
+    def max(self, b: BpfInterface|float) -> BpfInterface: ...
+    def min(self, b: BpfInterface|float) -> BpfInterface: ...
+    def __call__(self, other: float) -> float: ...
+    
+    def keep_slope(self, epsilon: float = 0.) -> BpfInterface: ...
+        
+    def outbound(self, y0: float, y1: float) -> BpfInterface: ...
+        
+    def apply(self, func) -> BpfInterface: ...
+        
+    def preapply(self, func) -> BpfInterface: ...
+        
+    def periodic(self) -> BpfInterface: ...
+       
+    def stretched(self, rx: float, fixpoint: float = 0.) -> BpfInterface: ...
+        
+    def fit_between(self, x0: float, x1: float) -> BpfInterface: ...
+      
+    def shifted(self, dx: float) -> BpfInterface: ...
+        
+    def inverted(self) -> BpfInterface: ...
+        
+    @classmethod
+    def fromseq(cls, *points: float|tuple[float, float], **kws) -> BpfInterface: ...
+        
+    def copy(self) -> BpfInterface: ...
+
+        
+class BpfBase(BpfInterface):
+
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]]
+                 ): ...
+        
+    @property
+    def descriptor(self) -> str: ... 
+            
+    def mapn_between(self, n: int, xstart: float, xend: float, out: np.ndarray|None = None) -> np.ndarray: ...
+       
+    def points(self) -> tuple[np.ndarray, np.ndarray]: ...
+        
+    def clone_with_new_data(self, xs: np.ndarray, ys: np.ndarray) -> BpfInterface: ...
+        
+    def insertpoint(self, x: float, y: float) -> BpfInterface: ...
+        
+    def removepoint(self, x: float) -> BpfInterface: ...
+        
+    def segments(self) -> Iterator[tuple[float, float, float]]: ...
+
+    @property
+    def exp(self) -> float: ...
+        
+
+class Linear(BpfBase): 
+
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]]
+                 ): ...
+
+
+    def inverted(self) -> Linear: ...
+        
+    def flatpairs(self) -> np.ndarray: ...
+        
+
+class Smooth(BpfBase): ...
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]]
+                 ): ...
+
+   
+class Smoother(BpfBase): ...
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]]
+                 ): ...
+
+    
+class Halfcos(BpfBase):
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]],
+                 exp: float = 1.0, numiter: int =1): ...
+    
+
+class Halfcosm(Halfcos):
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]],
+                 exp: float = 1.0, numiter: int =1): ...
+
+
+class Expon(BpfBase):
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]],
+                 exp: float = 1.0, numiter: int =1): ...
+
+
+class Exponm(Expon):
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]],
+                 exp: float = 1.0, numiter: int =1): ...
+
+
+class NoInterpol(BpfBase): ...
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]]
+                 ): ...
+
+    
+class Nearest(BpfBase): ...
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]]
+                 ): ...
+
+
+class Sampled(BpfInterface): 
+    def __init__(self,
+                 samples: np.ndarray,
+                 dx: float,
+                 x0: float = 0.,
+                 interpolation: str = 'linear'): ...
+
+    @property
+    def ys(self) -> np.ndarray: ...
+    
+
+    @property
+    def samplerate(self) -> float: ...
+        
+    @property
+    def xs(self) -> np.ndarray: ...
+        
+    
+    @property
+    def dx(self) -> float: ...
+    
+    def set_interpolation(self, interpolation: str) -> Sampled: ...
+        
+    
+    def flatpairs(self) -> np.ndarray: ...
+        
+
+
+class Spline(BpfInterface): ...
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]]
+                 ): ...
+
+    
+
+class USpline(BpfInterface): ...
+    def __init__(self,
+                 xs: Union[np.ndarray, list[float]],
+                 ys: Union[np.ndarray, list[float]]
+                 ): ...
+
+    
+class Slope(BpfInterface):
+
+    @property
+    def slope(self) -> float: ...
+
+    @slope.setter
+    def slope(self, value: float) -> None: ...
+    
+    @property
+    def offset(self) -> float: ...
+
+    @offset.setter
+    def offset(self, value: float) -> None: ...
+    
+
+    
+class _BpfCompose(BpfInterface): ...
+
+
+class _BpfConcat(BpfInterface): ...
+
+
+class _BpfBlend(BpfInterface): ...
+
+        
+class Multi(BpfInterface): ...
+
+
+class Const(BpfInterface): ...
+
+
+class _MultipleBpfs(BpfInterface):
+
+    def __init__(self, bpfs: list[BpfInterface]): ...
+    
+
+class Max(_MultipleBpfs): ...
+    
+class Min(_MultipleBpfs): ...
+
+class Stack(_MultipleBpfs): ...
+
+
+def brentq(bpf: BpfInterface, x0: float, xa: float, xb: float, xtol=9.9999999999999998e-13, 
+           rtol=4.4408920985006262e-16, max_iter=100) -> tuple[float,int]: ...
+    
+
+def blend(a: BpfInterface, b: BpfInterface, mix=0.5) -> BpfInterface: ...
+
+
+
+def bpf_zero_crossings(b: BpfInterface, 
+                       h: float = 0.01, N: int = 0, 
+                       x0: float = float('nan'), 
+                       x1: float = float('nan'), 
+                       maxzeros: int = 0
+                       ) -> list[float]: ...
+
```

## bpf4/core.pyx

```diff
@@ -1,5551 +1,5551 @@
-# cython: binding=True
-# cython: boundscheck=False
-# cython: embedsignature=True
-# cython: wraparound=False
-# cython: infer_types=True
-# cython: profile=False
-# cython: c_string_type=str, c_string_encoding=ascii
-# cython: language_level=3
-# cython: annotation_typing=True 
-
-cdef extern from "math.h":
-    double cos(double x) nogil
-    double sin(double x) nogil
-    double pow(double x, double y) nogil
-    double ceil(double x) nogil
-    double log(double x) nogil
-    double exp(double x) nogil
-    double floor(double x) nogil
-    double fmod(double x, double y) nogil
-    double hypot(double x, double y) nogil
-    double atan2(double x, double y) nogil
-    double tanh (double x ) nogil
-    double fabs (double x) nogil
-    double sqrt(double x) nogil
-    double INFINITY, NAN, M_E, M_PI
-    int isfinite(double x) nogil
-    int isinf(double x) nogil
-    int isnan(double x) nogil
-    double acos(double x) nogil
-    double asin(double x) nogil
-    double cosh(double x) nogil
-    double log10(double x) nogil
-    double tan(double x) nogil
-    double sinh(double x) nogil
-    double log1p(double x) nogil
-    
-#cdef extern from "string.h":
-#    ctypedef void* const_void_ptr "const void *"
-#    void *memcpy(void *s1, const_void_ptr s2, size_t n) nogil
-
-# ----------------------------------------------  cimports
-from libc.stdlib cimport malloc, free # , realloc
-from libc.stdlib cimport rand, srand, RAND_MAX
-from libc.stdio cimport printf, fflush, stdout
-from libc.stdint cimport int64_t
-
-from cpython cimport PyList_GET_SIZE, PyList_GET_ITEM, PyTuple_New, PyTuple_SetItem
-cimport cython
-cimport numpy as c_numpy
-from cython.view cimport array as cvarray
-from numpy cimport (
-    ndarray,
-    npy_intp,
-    PyArray_DIM,
-    float_t,
-    PyArray_ISCONTIGUOUS,
-    import_array,
-    PyArray_GETCONTIGUOUS,
-    PyArray_ContiguousFromAny,  # object PyArray_ContiguousFromAny(op, int, int min_depth, int max_depth)
-    NPY_DOUBLE,
-    PyArray_SimpleNew,          # PyArray_SimpleNew(int nd, npy_intp *dims, int type_num)
-    PyArray_SimpleNewFromData,  # PyArray_SimpleNewFromData(int nd, npy_intp *dims, int type_num, void *data)
-    PyArray_EMPTY,              # PyArray_EMPTY(int nd, npy_intp* dims, int typenum, int fortran)
-    PyArray_ISCARRAY,           # int PyArray_ISCARRAY( c_numpy.ndarray instance )
-    PyArray_ZEROS,              # PyArray_ZEROS(int nd, npy_intp* dims, int type_num, int fortran)
-    PyArray_FILLWBYTE           # PyArray_FILLWBYTE(obj, int val)
-    )
-
-# ---------------------------- import std-lib
-# import math
-import sys
-import random
-
-# ---------------------------- import others
-import numpy
-from numpy import array
-from . import arraytools
-
-# ---------------------------- own imports
-from .config import CONFIG
-
-# ---------------------------- init
-import_array()
-srand(random.randint(0, 99999))
-
-# ---------------------------- platform specific constants
-
-cdef double EPS = sys.float_info.epsilon
-cdef double SQRT_EPS = sqrt(EPS)
-
-# ---------------------------- DEFs
-DEF PI = 3.141592653589793238462643383279502884197169399375105
-DEF BRENTQ_ZERO = 2.221e-16
-DEF BRENTQ_XTOL = 9.9999999999999998e-13
-DEF BRENTQ_RTOL = 4.4408920985006262e-16
-DEF BRENTQ_MAXITER = 100
-DEF QUAD_LIMIT = 100
-DEF SIMPSONS_ACCURACY = 1e-10
-DEF SIMPSONS_MAXITER = 100
-
-
-# -------------------------------------------------------------------
-#       ERROR TYPES
-# -------------------------------------------------------------------
-class BpfPointsError(ValueError): pass
-class BpfInversionError(ValueError): pass
-
-# -------------------------------------------------------------------
-#       INLINE FUNCS
-# -------------------------------------------------------------------
-ctypedef struct InterpolFunc
-
-@cython.cdivision(True)
-cdef inline double intrp_linear(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    return y0 + (y1 - y0) * ((x - x0) / (x1 - x0))
-
-cdef inline double intrp_nointerpol(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    return y0 if x < x1 else y1
-
-cdef inline double intrp_nearest(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    if (x - x0) <= (x1 - x):
-        return y0
-    return y1
-
-@cython.cdivision(True)
-cdef inline double intrp_halfcos(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    cdef:
-        double dx, y
-        double x1x0 = x1 - x0
-        int i
-    if self.numiter > 1:
-        for i in range(self.numiter - 1):
-            dx = (x - x0) / x1x0    
-            dx = (dx + 1) * 3.14159265358979323846
-            x = x0 + x1x0 * (1 + cos(dx)) / 2.0
-    dx = (x - x0) / x1x0    
-    dx = (dx + 1) * 3.14159265358979323846
-    y = y0 + (y1 - y0) * (1 + cos(dx)) / 2.0
-    return y
-
-@cython.cdivision(True)
-cdef inline double intrp_halfcosexp(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    cdef:
-        double dx
-        double x1x0 = x1 - x0
-        int i
-        double exp = self.exp
-    if self.numiter > 1:
-        for i in range(self.numiter - 1):
-            dx = pow((x - x0) / x1x0, exp)    
-            dx = (dx + 1) * 3.14159265358979323846
-            x = x0 + x1x0 * (1 + cos(dx)) / 2.0
-    dx = pow((x - x0) / x1x0, exp)    
-    dx = (dx + 1) * 3.14159265358979323846        
-    return y0 + (y1 - y0) * (1 + cos(dx)) / 2.0
-
-
-@cython.cdivision(True)
-cdef inline double intrp_halfcosexpm(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    cdef:
-        double dx
-        double x1x0 = x1 - x0
-        double exp = self.exp
-        int i
-    if y1 < y0:
-        exp = 1/exp    
-    if self.numiter > 1:
-        for i in range(self.numiter - 1):
-            dx = pow((x - x0) / x1x0, exp)    
-            dx = (dx + 1) * 3.14159265358979323846
-            x = x0 + x1x0 * (1 + cos(dx)) / 2.0
-    dx = pow((x - x0) / x1x0, exp)    
-    dx = (dx + 1) * 3.14159265358979323846        
-    return y0 + (y1 - y0) * (1 + cos(dx)) / 2.0
-
-    
-
-@cython.cdivision(True)
-cdef inline double intrp_expon(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    cdef: 
-        double exp = self.exp
-        double dx
-        double x1x0 = x1 - x0
-        int i
-    if self.numiter > 1:
-        for i in range(self.numiter - 1):
-            dx = (x - x0) / x1x0
-            x = x0 + pow(dx, exp) * x1x0
-    dx = (x - x0) / x1x0
-    return y0 + pow(dx, exp) * (y1 - y0)
-
-
-@cython.cdivision(True)
-cdef inline double intrp_exponm(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    cdef: 
-        double exp = self.exp
-        double dx
-        double x1x0 = x1 - x0
-        int i
-    if y1 < y0:
-        exp = 1/exp
-    if self.numiter > 1:
-        for i in range(self.numiter - 1):
-            dx = (x - x0) / x1x0
-            x = x0 + pow(dx, exp) * x1x0
-    dx = (x - x0) / x1x0
-    return y0 + pow(dx, exp) * (y1 - y0)
-
-    
-@cython.cdivision(True)
-cdef inline double intrp_smooth(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    """
-    #define SMOOTHSTEP(x) (x) * (x) * (3 - 2 * x)
-    for (i = 0; i < N; i++) {
-      v = i / N;
-      v = SMOOTHSTEP(v);
-      X = (A * v) + (B * (1 - v));
-    }   --> http://sol.gfxile.net/interpolation/
-    """
-    cdef:
-        double x1x0 = x1 - x0
-        double v
-        int i
-
-    if self.numiter > 1:
-        for i in range(self.numiter - 1):
-            v = (x - x0) / x1x0
-            v = v*v*(3 - 2*v)
-            x = x0 + x1x0 * v
-    v = (x - x0) / x1x0
-    v = v*v*(3 - 2*v)
-    return y0 + (y1 - y0) * v
-
-@cython.cdivision(True)
-cdef inline double intrp_smoother(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    cdef:
-        double x1x0 = x1 - x0
-        double v
-    # x * x * x * (x * (x * 6 - 15) + 10);
-    v = (x - x0) / x1x0
-    v = v*v*v*(v*(v*6 - 15) + 10)
-    return y0 + (y1 - y0) * v
-
-# ------------------------------------------------------------------------------------------------
-
-@cython.cdivision(True)
-cdef inline double _integr_trapz(double *xs, int xs_size, double dx) nogil:
-    """
-    area of a trapezium (trapezoid)
-
-        a + b
-    A = ----- h
-          2 
-
-    where
-    A: area of the trapezium
-    a: length of one of the sides
-    b: length of the other side
-    h: distance between a and b (height)
-
-    In a function
-
-      /|
-     / |
-    |  |
-    |  |
-    ----
-
-    The curve is divided by a grid of dx. 
-    a: f(x)
-    b: f(x+dx)
-    h: dx
-
-    trapz = (f(x) + f(x+dx)) / 2 * dx
-    """
-    cdef int i
-    cdef double x0, x1, accum
-    cdef double r = 0.5 * dx
-    x0 = xs[0]
-    accum = 0
-    for i in range(1, xs_size):
-        x1 = xs[i]
-        accum += (x0 + x1) * r
-        x0 = x1
-    return accum
-
-@cython.cdivision(True)
-cdef inline double _integr_trapz_between(double *xs, int xs_size, double dx, double offset, double a, double b) nogil:
-    """
-    integrate sampled values `xs`, spaced at `dx` with an offset of `offset` in the range
-    [a, b] -- both a and b included
-
-    NB: the definition of xs is used, no oversampling takes place for better accuracy
-    in the cases where a and/or b do not fall exactly on the grid specified by offset+i*dx
-    """
-    cdef int i
-    cdef double x0, x1, accum
-    cdef double r = 0.5 * dx
-    cdef int i0 = <int>((a - offset) / dx)
-    cdef int i1 = <int>((b - offset) / dx) + 1
-    accum = 0
-    if i1 > xs_size:
-        i1 = xs_size
-    x0 = xs[i0]
-    for i in range(i0+1, i1):
-        x1 = xs[i]
-        accum += (x0 + x1) * r
-        x0 = x1
-    return accum
-
-@cython.cdivision(True)
-cdef inline double _integr_trapz_between_exact(double *xs, int xs_size, double dx, double offset, double a, double b) nogil:
-    """
-    integrate sampled values `xs`, spaced at `dx` with an offset of `offset` in the range
-    [a, b] -- both a and b included
-    """
-    cdef int i
-    cdef double x0, x1, accum, y
-    cdef double r = 0.5 * dx
-    cdef int i0 = <int>((a - offset) / dx + 0.999999999)
-    cdef int i1 = <int>((b - offset) / dx) + 1
-    cdef double rest_a = ((a - offset) % dx) / dx
-    cdef double rest_b = ((b - offset) % dx) / dx
-    accum = 0
-    if i1 > xs_size:
-        i1 = xs_size
-    x0 = xs[i0]
-    for i in range(i0+1, i1):
-        x1 = xs[i]
-        accum += (x0 + x1) * r
-        x0 = x1
-    if rest_a > 0 and i0 > 0:
-        y0 = xs[i0-1]
-        y1 = xs[i0]
-        y = y0 + (y1-y0) * rest_a
-        accum += (y + y1) * 0.5 * dx * (1 - rest_a)
-    if rest_b > 0 and (i1 + 1) < xs_size:
-        y0 = xs[i1]
-        y1 = xs[i1+1]
-        y = y0 + (y1-y0) * rest_a
-        accum += (y0 + y) * 0.5 * dx * rest_b
-    return accum
-
-cdef inline double _clip(double x, double x0, double x1) nogil:
-    return x1 if x > x1 else x0 if x < x0 else x
-
-cdef inline double _ntodx(size_t n, double x0, double x1):
-    return (x1 - x0) / (n - 1)
-
-cdef inline size_t _dxton(double dx, double x0, double x1):
-    return <size_t>round((x1-x0)/dx+1)
-    
-cdef double _a4 = 442.0
-DEF loge_2 = 0.6931471805599453094172321214581766
-
-
-def setA4(double freq):
-    """
-    Set the reference freq used
-
-    Args:
-        freq (float): the reference frequency for A4
-    """
-    global _a4
-    _a4 = freq
-
-
-@cython.cdivision(True)
-cdef double m2f(double midinote) nogil:
-    global _a4
-    if 0.0 <= midinote:
-        return _a4 * pow(2.0, (midinote - 69.0) / 12.0)
-    return 0.
-
-@cython.cdivision(True)
-cdef double f2m(double freq) nogil:
-    global _a4
-    if 8.2129616379875419 < freq:    # this is the freq. of midi 0
-        return 12 * (log(freq / _a4) / loge_2) + 69.0
-    return 0
-
-# ---------------------------- TYPES
-ctypedef double(*t_unfunc)(double) nogil
-
-cdef t_unfunc UNFUNCS[14]
-UNFUNCS[:] = [
-    cos,    # 0
-    sin,    # 1
-    ceil,   # 2
-    log,    # 3
-    exp,    # 4
-    floor,  # 5
-    tanh,   # 6
-    fabs,   # 7
-    sqrt,   # 8
-    acos,   # 9
-    asin,   # 10
-    tan,    # 11
-    sinh,   # 12
-    log10,  # 13
-    # m2f,    # 14
-    # f2m     # 15
-]
-
-ctypedef double(*t_func0)(double, double, double, double, double, double) nogil
-ctypedef double(*t_func)(InterpolFunc *, double, double, double, double, double) nogil
-
-ctypedef struct InterpolFunc:
-    t_func func
-    double exp
-    int numiter
-    double mix
-    InterpolFunc* blend_func
-    char *name
-    unsigned int needs_free
-
-DTYPE = numpy.float64  #np.float64
-ctypedef c_numpy.float_t DTYPE_t
-
-# InterpolFunc
-cdef inline void InterpolFunc_init(InterpolFunc *self, t_func func, double exp, char *name, unsigned int needs_free):
-    self.func = func
-    self.exp = exp
-    self.numiter = 1
-    self.mix = -1
-    self.blend_func = NULL
-    self.name = name
-    self.needs_free = needs_free
-
-cdef inline InterpolFunc* InterpolFunc_new(t_func func, double exp, char *name, unsigned int needs_free):
-    cdef InterpolFunc* out
-    out = <InterpolFunc *>malloc(sizeof(InterpolFunc))
-    InterpolFunc_init(out, func, exp, name, needs_free)
-    return out
-
-cdef inline InterpolFunc* InterpolFunc_new_blend_from_descr(str descr0, str descr1, double mix):
-    cdef InterpolFunc* out = InterpolFunc_new_from_descriptor(descr0, 1)  # force new 
-    cdef InterpolFunc* blend = InterpolFunc_new_from_descriptor(descr1, 1)  # force new
-    out.blend_func = blend
-    out.mix = mix
-    return out
-
-cdef InterpolFunc* InterpolFunc_new_from_descriptor(str descr, int forcenew=0):
-    cdef InterpolFunc* out = NULL
-    cdef double exp = 1.0
-    cdef str func_name
-    if "(" in descr:
-        func_name, param = descr.split("(")
-        exp = float(param[:len(param)-1])
-    else:
-        func_name = descr
-    if func_name == 'linear':
-        if not forcenew:
-            out = InterpolFunc_linear
-        else:
-            out = InterpolFunc_new(intrp_linear, 1, '', 1)
-    elif func_name == 'expon':
-        out = InterpolFunc_new(intrp_expon, exp, 'expon', 1)
-    elif func_name == 'halfcos':
-        if exp == 1.0 and not forcenew:
-            out = InterpolFunc_halfcos
-        else:
-            out = InterpolFunc_new(intrp_halfcosexp, exp, 'halfcosexp', 1)
-    elif func_name == 'halfcosexp':
-        out = InterpolFunc_new(intrp_halfcosexp, exp, 'halfcosexp', 1)
-    elif func_name == 'nointerpol':
-        out = InterpolFunc_nointerpol
-    elif func_name == 'nearest':
-        out = InterpolFunc_nearest
-    elif func_name == 'smooth':
-        out = InterpolFunc_smooth
-    return out
-
-cdef inline double InterpolFunc_call(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-    cdef double v0, v1
-    if self.mix <= 0:
-        return self.func(self, x, x0, y0, x1, y1)
-    else:
-        v0 = self.func(self, x, x0, y0, x1, y1)
-        v1 = self.blend_func.func(self.blend_func, x, x0, y0, x1, y1)
-        return v0 * (1 - self.mix) + v1 * self.mix
-
-#cdef inline double InterpolFunc_call(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
-#    cdef double y = self.func(self, x, x0, y0, x1, y1)
-#    return y
-
-cdef inline void InterpolFunc_free(InterpolFunc *self):
-    if self is not NULL:
-        if self.blend_func is not NULL:
-            InterpolFunc_free(self.blend_func)
-        if self.needs_free == 1:
-            free(self)
-
-cdef inline str InterpolFunc_get_descriptor(InterpolFunc *self):
-    if self.exp != 1.0:
-        return "%s(%s)" % (self.name, str(self.exp))
-    else:
-        return self.name   
-
-# create the most used interpolation functions, which are shared across BPFs
-cdef InterpolFunc* InterpolFunc_linear    = InterpolFunc_new(intrp_linear, 1.0, 'linear',  0)
-cdef InterpolFunc* InterpolFunc_halfcos    = InterpolFunc_new(intrp_halfcos, 1.0, 'halfcos', 0)
-cdef InterpolFunc* InterpolFunc_nointerpol = InterpolFunc_new(intrp_nointerpol,  1.0, 'nointerpol',  0)
-cdef InterpolFunc* InterpolFunc_nearest   = InterpolFunc_new(intrp_nearest,  1.0, 'nearest',  0)
-cdef InterpolFunc* InterpolFunc_smooth    = InterpolFunc_new(intrp_smooth, 1.0, 'smooth', 0)
-cdef InterpolFunc* InterpolFunc_smoother  = InterpolFunc_new(intrp_smoother, 1.0, 'smoother', 0)
-
-
-cdef inline ndarray EMPTY1D(int size): #new_empty_doublearray_1D(int size):
-    cdef npy_intp *dims = [size]
-    return PyArray_EMPTY(1, dims, NPY_DOUBLE, 0)
-
-DEF NUM_XS_FOR_RENDERING = 200
-DEF DEFAULT_EPSILON = 1e-4
-DEF INF = float('inf')
-DEF INFNEG = float('-inf')
-cdef double MAX_FLOAT = 3.40282346638528860e+38
-CONST_XS_FOR_RENDERING = numpy.linspace(0., 1., NUM_XS_FOR_RENDERING)
-DEF NOCOPY = False
-
-# behaviour for cropping
-DEF OUTBOUND_DEFAULT    = -1
-DEF OUTBOUND_DONOTHING  = 0     # do nothing, just return the value of the original bpf. in this case, cropping only sets the bounds
-DEF OUTBOUND_CACHE      = 1     # cache the value of the bpf at creation time and return this value outside the bounds
-DEF OUTBOUND_SET        = 2     # set the value outside the bounds
-
-
-cpdef int _array_issorted(double[:] xs):
-    """
-    Is this array sorted?
-
-    Returns:
-        status value: -1=not sorted, 0=array is sorted, with dups, 1=array is sorted, no dups
-
-    """
-    cdef int i
-    cdef double x0, x1
-    cdef int nodups = 1
-    x1 = xs[0]
-    with nogil:
-        for i in range(1, xs.shape[0]):
-            x0 = x1
-            x1 = xs[i]
-            if x1 < x0:
-                return -1
-            elif x1 == x0:
-                nodups = 0
-    return nodups
-
-
-cdef inline int _searchsorted(double [:]xs, double x) nogil:
-    cdef int imin = 0
-    cdef int imax = xs.shape[0]
-    cdef int imid
-    while imin < imax:
-        imid = imin + ((imax - imin) >> 2)
-        if xs[imid] < x:
-            imin = imid + 1
-        else:
-            imax = imid
-    return imin
-
-
-cdef inline int _csearchlinear(DTYPE_t *xs, int xs_length, DTYPE_t x, int index) nogil:
-    # returns -1 if x is left from index
-    cdef int i = index
-    cdef double x0 = xs[i]
-    if x < x0:
-        return -1
-    cdef double x1
-    for i in range(index, xs_length-1):
-        x1 = xs[i+1]
-        if x0 <= x < x1:
-            return i
-        x0 = x1
-    return xs_length-1
-
-
-
-cdef inline int _csearchsorted(DTYPE_t *xs, int xs_length, DTYPE_t x) nogil:
-    """
-    equivalent to bisect_right. 
-    xs[out] > x
-    """
-    cdef int imin = 0
-    cdef int imax = xs_length
-    cdef int imid
-    while imin < imax:
-        imid = imin + ((imax - imin) >> 2)
-        if (<DTYPE_t *>(xs))[imid] < x:
-            imin = imid + 1
-        else:
-            imax = imid
-    return imin
-
-
-cdef inline int _csearchsorted_left(DTYPE_t *xs, int xs_length, DTYPE_t x) nogil:
-    cdef int imin = 0
-    cdef int imax = xs_length
-    cdef int imid
-    while imin < imax:
-        imid = imin + ((imax - imin) >> 2)
-        if xs[imid] <= x:
-            imin = imid + 1
-        else:
-            imax = imid
-    return imin
-
-
-cdef inline double* _seq_to_doubles(xs):
-    cdef int size, i
-    cdef double* out
-    cdef double* data
-    if isinstance(xs, ndarray):
-        size = PyArray_DIM(<ndarray>xs, 0)
-        out = <double *>malloc(sizeof(double) * size)
-        if PyArray_ISCONTIGUOUS(<ndarray>xs):
-            data = <DTYPE_t *>((<ndarray>xs).data)
-            for i in range(size):
-                out[i] = data[i]
-        else:
-            for i in range(size):
-                out[i] = xs[i]
-    else:
-        if isinstance(xs, list):
-            size = len(<list>xs)
-            out = <double *>malloc(sizeof(double) * size)
-            for i in range(size):
-                out[i] = (<list>xs)[i]
-        elif isinstance(xs, tuple):
-            size = len(<tuple>xs)
-            out = <double *>malloc(sizeof(double) * size)
-            for i in range(size):
-                out[i] = (<tuple>xs)[i]
-        else:
-            size = len(xs)
-            out = <double *>malloc(sizeof(double) * size)
-            for i in range(size):
-                out[i] = xs[i]
-    return out
-
-def _get_bounds(a, b):
-    cdef double start, end, b_start, b_end
-    start, end = a.bounds()
-    try:
-        b_start, b_end = b.bounds()
-        start = start if start < b_start else b_start
-        end = end if end > b_end else b_end
-    except:
-        pass
-    return (start, end)
-
-
-# ~~~~~~~~~~~~~~~~~~~ BpfInterface ~~~~~~~~~~~~~~~~~~~~~
-
-cdef class BpfInterface:
-    """
-    Base class for all Break-Point Functions
-
-    !!! note
-
-        BpfInterace is an abstract class. It is not possible to create 
-        an instance of it. 
-
-    """
-    cdef double _x0, _x1
-    cdef int _integration_mode  # 0: dont use scipy, 1: use scipy, -1: calibrate
-    cpdef BpfInterface _asbpf(self): return self
-    cdef void _bounds_changed(self): pass
-    
-    cdef inline void _set_bounds(self, double x0, double x1):
-        self._x0 = x0
-        self._x1 = x1
-        self._integration_mode = CONFIG['integrate.default_mode']
-    
-    cdef inline void _set_bounds_like(self, BpfInterface a):
-        self._set_bounds(a._x0, a._x1)
-    
-    cpdef double ntodx(self, int N):
-        """
-        Calculate the sampling period `dx` 
-
-        Calculate sampling period *dx* so that the bounds of 
-        this bpf are divided into *N* parts: `dx = (x1-x0) / (N-1)`.
-        The period is calculated so that lower and upper bounds are
-        included, following numpy's `linspace`
-
-        Args:
-            N (int): The number of points to sample within the bounds of
-                this bpf
-
-        Returns:
-            (float) The sampling period *dx*
-
-        !!! info "See Also"
-
-            [dxton()](#dxton)
-
-        Example
-        -------
-
-        ```python
-        >>> a = linear(0, 0, 1, 1)
-        >>> dx = a.ntodx(10)
-        >>> dx
-        0.11111111
-        >>> np.arange(a.x0, a.x1, dx)
-        array([0.        , 0.11111111, 0.22222222, 0.33333333, 0.44444444,
-       0.55555556, 0.66666667, 0.77777778, 0.88888889, 1.        ])
-
-        """
-        return (self._x1 - self._x0) / (N - 1)
-    
-    cpdef int dxton(self, double dx):
-        """
-        Split the bounds of this bpf according to a given sampling period *dx*
-
-        Args:
-            dx (float): the sampling period
-
-        Returns:
-            (int) The number of points to sample
-
-
-        Calculate the number of points in as a result of dividing the 
-        bounds of this bpf by the sampling period `dx`:
-
-            n = (x1 + dx - x0) / dx
-
-        where *x0* and *x1* are the *x* coord start and end points and *dx* 
-        is the sampling period.
-
-        ```python
-        >>> from bpf4 import *
-        >>> a = linear(0, 0, 1,  10, 2, 5)
-        # Sample a with a period of 0.1
-        >>> ys = a.map(a.dxton(0.1))
-        >>> len(ys)
-        21
-        >>> ys
-        array([ 0.,  1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.,  9., 10.,  9.,  8.,
-        7.,  6.,  5.,  4.,  3.,  2.,  1.,  0.])
-        ```
-
-        !!! info "See Also"
-
-            [ntodx()](#ntodx)
-        """
-        return <int>(((self._x1 + dx) - self._x0) / dx)
-    
-    def bounds(self):
-        """
-        Returns a tuple (xstart, xend) representing the bounds of this bpf
-
-        Returns:
-            (tuple[float, float]) The bounbs of this bpf
-
-        The returned bounds indicate the range within which this bpf is defined, but
-        any bpf can be evaluated outside those bounds. In such a case the out-of-bound
-        result will depend on the concrete subclass being evaluated. For most cases
-        the out-of-bound result is the same as the result at the bounds
-
-        ## Example
-        
-        ```python
-
-        >>> from bpf4 import *
-        >>> a = linear(1, 10, 2, 25)
-        >>> a.bounds()
-        (1.0, 2.0)
-        ```
-
-        """
-        return self._x0, self._x1
-
-    @property
-    def x0(self) -> float:
-        """The lower bound of the x coordinate"""
-        return self._x0
-    
-    
-    @property
-    def x1(self) -> float: 
-        """The upper bound of the x coordinate"""
-        return self._x1
-    
-    def __add__(a, b):
-        return _create_lambda_unordered(a, b, _BpfLambdaAdd, _BpfLambdaAddConst)
-    
-    def __sub__(a, b):
-        return _create_rlambda(a, b, _BpfLambdaSub, _BpfLambdaSubConst, _BpfLambdaRSub, _BpfLambdaRSubConst)
-    
-    def __mul__(a, b):
-        cdef float v
-        try:
-            v = float(b)  # are we a?
-            if v == 0:
-                return Const(0).set_bounds(a.x0, a.x1)
-            elif v == 1:
-                return a
-            else:
-                return _BpfLambdaMulConst(a, b, a.bounds())
-        except (TypeError, ValueError):
-            try:
-                v = float(a) # are we b?
-                if v == 0:
-                    return Const(0).set_bounds(b.x0, b.x1)
-                elif v == 1:
-                    return b
-                else:
-                    return _BpfLambdaMulConst(b, a, b.bounds())
-            except (TypeError, ValueError):
-                return _create_lambda_unordered(a, b, _BpfLambdaMul, _BpfLambdaMulConst)  # two bpfs
-    
-    def __div__(a, b):
-        cdef float v
-        try:
-            v = float(b)  # are we a?
-            if v == 0:
-                raise ZeroDivisionError("Can't divide by 0")
-            elif v == 1:
-                return a
-            else:
-                return _BpfLambdaDivConst(a, b, a.bounds())
-        except (TypeError, ValueError):
-            try:
-                v = float(a) # are we b?
-                if v == 0:
-                    return 0
-                else:
-                    return _BpfLambdaRDivConst(b, a, b.bounds())
-            except (TypeError, ValueError):
-                return _create_rlambda(a, b, _BpfLambdaDiv, _BpfLambdaDivConst, _BpfLambdaRDiv, _BpfLambdaRDivConst)
-    
-    def __truediv__(a, b):
-        return _create_rlambda(a, b, _BpfLambdaDiv, _BpfLambdaDivConst, _BpfLambdaRDiv, _BpfLambdaRDivConst)
-    
-    def __pow__(a, b, modulo):
-        cdef double tmp
-        if isinstance(a, BpfInterface):
-            if isinstance(b, BpfInterface):
-                return _BpfLambdaPow(a, b, _get_bounds(a, b))
-            elif callable(b):
-                return _BpfLambdaPow(a, _FunctionWrap(b), a.bounds())
-            elif b == 2:
-                return a*a
-            elif b == 3:
-                return a*a*a
-            elif b == 4:
-                tmp = a*a
-                return tmp*tmp
-            elif b == 0:
-                return a
-            elif b == -1:
-                return 1/a
-            elif b == -2:
-                return 1/(a*a)
-            else:
-                return _BpfLambdaPowConst(a, b, a.bounds())
-        elif isinstance(b, BpfInterface):
-            if callable(a):
-                return _BpfLambdaPow(_FunctionWrap(a), b, b.bounds())
-            return _BpfLambdaRPowConst(b, a, (INFNEG, INF))
-        return NotImplemented
-
-    def __neg__(self):
-        return self * -1
-    
-    def __mod__(self, other):
-        return _create_lambda(self, other, _BpfLambdaMod, _BpfLambdaModConst)
-    
-    def __abs__(self):
-        return self.abs()
-    
-    def __or__(a, b):
-        """
-        a | b
-        """
-        if isinstance(a, BpfInterface) and isinstance(b, BpfInterface):
-            out = _BpfCompose_new(a, b)
-        elif isinstance(a, BpfInterface) and callable(b):
-            out = _BpfCompose_new(a, _FunctionWrap(b))
-        elif callable(a) and isinstance(b, BpfInterface):
-            out = _BpfCompose_new(_FunctionWrap(b), a)
-        else:
-            return NotImplemented 
-        return out
-    
-    def __rshift__(a, b):
-        if isinstance(a, BpfInterface):
-            return a.shifted(b)
-        return NotImplemented
-
-    def __lshift__(a, b):
-        if isinstance(a, BpfInterface):
-            return a.shifted(-b)
-        return NotImplemented
-        
-    def __xor__(a, b): # ^
-        if isinstance(a, BpfInterface):
-            return a.stretched(b)
-        return NotImplemented
-
-    def __richcmp__(BpfInterface self, other, int t):
-        if t == 0:      # <
-            return _create_lambda(self, other, _BpfLambdaLowerThan, _BpfLambdaLowerThanConst)
-        elif t == 2:    # ==
-            return _create_lambda(self, other, _BpfLambdaEqual, _BpfLambdaEqualConst)
-        elif t == 4:    # >
-            return _create_lambda(self, other, _BpfLambdaGreaterThan, _BpfLambdaGreaterThanConst)
-        elif t == 1:    # <=
-            return _create_lambda(self, other, _BpfLambdaLowerOrEqualThan, _BpfLambdaLowerOrEqualThanConst)       # (self > other) == 0
-        elif t == 3:    # !=
-            return _create_lambda(self, other, _BpfLambdaUnequal, _BpfLambdaUnequalConst)
-        elif t == 5:    # >=
-            return _create_lambda(self, other, _BpfLambdaGreaterOrEqualThan, _BpfLambdaGreaterOrEqualThanConst) # (self < other) == 0
-    
-    def _get_points_for_rendering(self, int n= -1):
-        # BpfInterface
-        if n == -1:
-            n = NUM_XS_FOR_RENDERING
-        xs = numpy.linspace(self._x0, self._x1, n)
-        ys = self.mapn_between(n, self._x0, self._x1)
-        return xs, ys
-    
-    def render(self, xs, interpolation='linear'):
-        """
-        Create a new bpf representing this bpf rendered at the given points
-
-        The difference between `.render` and `.sampled` is that this method
-        creates a Linear/NoInterpol bpf whereas `.sampled` returns a 
-        `Sampled` bpf (a `Sampled` bpf works only for regularly sampled data,
-        a Linear or NoInterpol bpfs accept any data as its x coordinate)
-
-        Args:
-            xs (int | list | np.ndarray): a seq of points at which this bpf 
-                is sampled or a number, in which case an even grid is calculated 
-                with that number of points. In the first case a Linear or NoInterpol
-                bpf is returned depending on the `interpolation` parameter (see below).
-                In the second case a `Sampled` bpf is returned.
-            interpolation (str): the interpoltation type of the returned bpf. 
-                One of 'linear', 'nointerpol'
-
-        Returns:
-            (BpfInterface) a new bpf representing this bpf. Depending on the interpolation
-            this new bpf will be a Sampled, a Linear or a NoInterpol bpf
-
-        Example
-        -------
-
-        ```python
-
-        >>> from bpf4 import *
-        >>> from math import *
-        >>> a = slope(1)[0:4*pi].sin()
-        >>> b = a.render(20)   # Sample this bpf at 20 points within its bounds
-        >>> b
-        Sampled[0.0:12.566370614359172]
-        >>> b.plot()
-        ```
-        ![](assets/render1.png)
-
-        !!! info "See Also"
-
-            [BpfInterface.sampled](#sampled)
-
-        """
-        if isinstance(xs, (int, long)):
-            dx = (self._x1 - self._x0) / (xs - 1)
-            return self.sampled(dx, interpolation=interpolation)
-        else:
-            ys = self.map(xs)
-            if interpolation == 'linear':
-                return Linear(xs, ys)
-            elif interpolation == 'nointerpol':
-                return NoInterpol(xs, ys)
-            else:
-                raise ValueError("interpolation %s not implemented" % interpolation)
-
-    def plot(self, kind='line', int n=-1, show=True, axes=None, **keys):
-        """
-        Plot the bpf using matplotlib.pyplot. Any key is passed to plot.plot_coords
-
-        Args:
-            kind (str): one of 'line', 'bar'
-            n (int): the number of points to plot
-            show (bool): if the plot should be shown immediately after (default is True). 
-                If you want to display multiple BPFs sharing an axes you can call 
-                plot on each of the bpfs with show=False, and then either
-                call the last one with plot=True or call bpf4.plot.show().
-            axes (matplotlib.pyplot.Axes): if given, will be used to plot onto it,
-                otherwise an ad-hoc axes is created
-            kws: any keyword will be passed to plot.plot_coords, which is passed
-                to ``axes.plot`` (or axes.bar, etc)
-
-        Returns:
-        	the pyplot.Axes object. This will be the axes passed as argument,
-        	if given, or a new axes created for this plot
-        	 
-        ## Example
-
-        ```python
-
-        from bpf4 import *
-        a = linear(0, 0, 1, 10, 2, 0.5)
-        a.plot()
-
-        # Plot to a preexistent axes
-        ax = plt.subplot()
-        a.plot(axes=ax)
-        ```
-        """
-        xs, ys = self._get_points_for_rendering(n)
-        from . import plot
-        return plot.plot_coords(xs, ys, kind=kind, show=show, axes=axes, **keys)
-        
-    cpdef BpfInterface sampled(self, double dx, interpolation='linear'):
-        """
-        Sample this bpf at a regular interval, returns a Sampled bpf
-
-        Sample this bpf at an interval of dx (samplerate = 1 / dx)
-        returns a Sampled bpf with the given interpolation between the samples
-
-        Args:
-            dx (float): the sample interval
-            interpolation (str): the interpolation kind. One of 'linear',
-                'nointerpol', 'halfcos', 'expon(XX)', 'halfcos(XX)' (where
-                XX is an exponential passed to the interpolation function)
-
-        Returns:
-            (Sampled) The sampled bpf
-        
-        !!! note
-
-            If you need to sample a portion of the bpf, use [sampled_between](#sampled_between)
-
-        The same results can be achieved via indexing, in which case the resulting
-        bpf will be linearly interpolated:
-
-        ```python
-        bpf[::0.1]    # returns a sampled version of this bpf with a dx of 0.1
-        bpf[:10:0.1]  # samples this bpf between (x0, 10) at a dx of 0.1
-        ```
-
-        !!! info "See Also"
-
-            [ntodx](#ntodx), [dxton](#dxton)
-        """
-        # we need to account for the edge (x1 IS INCLUDED)
-        cdef int n = int((self._x1 - self._x0) / dx + 0.5) + 1
-        ys = self.mapn_between(n, self._x0, self._x1) 
-        return Sampled(ys, dx=dx, x0=self._x0, interpolation=interpolation)
-    
-    cpdef ndarray sample_between(self, double x0, double x1, double dx, ndarray out=None):
-        """
-        Sample this bpf at an interval of dx between x0 and x1 
-
-        !!! note
-
-            The interface is similar to numpy's `linspace`
-        
-        Args:
-            x0 (float): point to start sampling (included)
-            x1 (float): point to stop sampling (included)
-            dx (float): the sampling period
-            out (ndarray): if given, the result will be placed here and no new array will
-                be allocated
-
-        Returns:
-            (ndarray) An array with the values of this bpf sampled at at a regular grid of 
-            period `dx` from `x0` to `x1`. If out is given the result is placed in it
-
-        ## Example
-        
-        ```python
-        
-        >>> a = linear(0, 0, 10, 10)
-        >>> a.sample_between(0, 10, 1)
-        [0 1 2 3 4 5 6 7 8 9 10]
-        ```
-        
-        This is the same as `a.mapn_between(11, 0, 10)`
-        """
-        cdef int n
-        n = int((x1 - x0) / dx + 0.5) + 1
-        return self.mapn_between(n, x0, x1, out)
-    
-    cpdef BpfInterface sampled_between(self, double x0, double x1, double dx, interpolation='linear'):
-        """
-        Sample a portion of this bpf, returns a `Sampled` bpf
-
-        **NB**: This is the same as `thisbpf[x0:x1:dx]`
-        
-        Args:
-            x0 (float): point to start sampling (included)
-            x1 (float): point to stop sampling (included)
-            dx (float): the sampling period
-            interpolation (str): the interpolation kind. One of 'linear',
-                'nointerpol', 'halfcos', 'expon(XX)', 'halfcos(XX)' (where
-                XX is an exponential passed to the interpolation function). For 
-                example: 'expon(2.0)' or 'halfcos(0.5)'
-        
-        Returns:
-            (Sampled) The `Sampled` bpf, representing this bpf sampled at a grid of `[x0:x1:dx]`
-            with the given interpolation
-
-        """
-        cdef int n = int((x1 - x0) / dx + 0.5) + 1
-        ys = self.mapn_between(n, x0, x1)
-        return Sampled(ys, dx=dx, x0=x0, interpolation=interpolation)
-
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        """
-        Calculate an array of `n` values representing this bpf between `x0` and `x1`
-
-        Args:
-            x0 (float): lower bound to map this bpf
-            x1 (float): upper bound to map this bpf
-            out (ndarray): if included, results are placed here. 
-
-        Returns:
-            (ndarray) An array of `n` elements representing this bpf at the given 
-            values within the range `x0:x1`. This is `out` if it was passed 
-
-        x0 and x1 are included
-
-        Example
-        =======
-
-        ```python
-        
-        out = numpy.empty((100,), dtype=float)
-        out = thisbpf.mapn_between(100, 0, 10, out)
-        
-        ```
-        """
-        cdef double[::1] result = out if out is not None else EMPTY1D(n)
-        cdef double dx = _ntodx(n, x0, x1)
-        cdef size_t i
-        cdef double x
-        for i in range(n):
-            x = x0 + i*dx
-            result[i] = self.__ccall__(x)
-        return numpy.asarray(result)
-
-    cpdef ndarray map(self, xs, ndarray out=None):
-        """
-        The same as map(self, xs) but faster
-
-        Args:
-            xs (ndarray | int): the x coordinates at which to sample this bpf,
-                or an integer representing the number of elements to calculate
-                in an evenly spaced grid between the bounds of this bpf
-            out (ndarray): if given, an attempt will be done to use it as destination
-                for the result. The user should not trust that this actually happens
-                (see example)
-
-        ```python
-
-        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
-        ```
-
-        ## Example
-        
-        ```python
-
-        >>> out = numpy.empty((100,), dtype=float)
-        >>> xs = numpy.linspace(0, 10, 100)
-        # This is the right way to pass an output array
-        >>> out = thisbpf.map(xs, out)   
-        
-        ```
-        """
-        if isinstance(xs, int):
-            return self.mapn_between(xs, self._x0, self._x1, out)
-        
-        cdef double[::1] _xs = <ndarray>xs if isinstance(xs, ndarray) else numpy.asarray(xs)
-        cdef int nx  = len(_xs)
-        cdef double[::1] result = out if out is not None else EMPTY1D(nx)
-        cdef int i
-        cdef double x0,x1, dx
-        with nogil:
-            for i in range(nx):
-                result[i] = self.__ccall__(_xs[i])
-        return numpy.asarray(result)
-    
-    cpdef BpfInterface concat(self, BpfInterface other):
-        """
-        Concatenate this bpf to other
-
-        `other` is shifted to start at the end of `self`
-
-        ## Example
-        
-        ```python
-
-        >>> a = linear(0, 0, 1, 10)
-        >>> b = linear(3, 100, 10, 200)
-        >>> c = a.concat(b)
-        >>> c
-        _BpfConcat2[0.0:8.0]
-        >>> c(1 - 1e-12), c(1)
-        (9.99999999999, 100.0)
-        >>> c.plot()
-        ```
-        ![](assets/concat1.png)
-
-        """
-        cdef BpfInterface other2 = other.fit_between(self._x1, self._x1 + (other._x1 - other._x0))
-        return _BpfConcat2_new(self, other2, other2._x0)
-        
-    cpdef _BpfLambdaRound round(self):
-        """
-        A bpf representing round(self(x))
-
-        Returns:
-            (BpfInterface) A bpf representing the operation `round(self(x))`
-        """
-        return _BpfLambdaRound(self)
-
-    cpdef _BpfRand rand(self):
-        """
-        A bpf representing rand(self(x))
-
-        Returns:
-            (BpfInterface) A bpf representing the operation ``rand(self(x))`
-        """
-        return _BpfRand(self)
-    
-    cpdef _BpfUnaryFunc cos(self):  
-        """
-        Returns a bpf representing the cosine of this bpf
-
-        ```python
-        from bpf4 import *
-        from math import pi
-        a = slope(1).cos()
-        a[0:8*pi].plot()
-        ```
-        ![](assets/cos.png)
-        """
-        return _BpfUnaryFunc_new_from_index(self, 0)
-    
-    cpdef _BpfUnaryFunc sin(self):  
-        """Returns a bpf representing the sine of this bpf
-
-        ```
-        from bpf4 import *
-        from math import pi
-        a = slope(1).sin()
-        a[0:8*pi].plot()
-        ```
-        ![](assets/sin.png)
-        """    
-        return _BpfUnaryFunc_new_from_index(self, 1)
-    
-    cpdef _BpfUnaryFunc ceil(self): 
-        """Returns a bpf representing the ceil of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 2)
-    
-    cpdef _BpfUnaryFunc expon(self):
-        """Returns a bpf representing the exp operation with this bpf
-
-        ## Example
-
-        ```python
-
-        >>> from bpf4 import *
-        >>> a = linear(0, 0, 1, 10)
-        >>> a(0.1)
-        1.0
-        >>> exp(1.0)
-        2.718281828459045
-        >>> a.expon()(0.1)
-        2.718281828459045
-        ```
-        """
-        return _BpfUnaryFunc_new_from_index(self, 4)
-    
-    cpdef _BpfUnaryFunc floor(self): 
-        """Returns a bpf representing the floor of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 5)
-    
-    cpdef _BpfUnaryFunc tanh(self): 
-        """Returns a bpf representing the tanh of this bpf
-
-        ```python
-        from bpf4 import *
-        a = slope(1).tanh()
-        a[-4:4].plot()
-        ```
-        ![](assets/tanh.png)
-        """
-        return _BpfUnaryFunc_new_from_index(self, 6)
-    
-    cpdef _BpfUnaryFunc abs(self):  
-        """Returns a bpf representing the absolute value of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 7)
-    
-    cpdef _BpfUnaryFunc sqrt(self): 
-        """Returns a bpf representing the sqrt of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 8)
-    
-    cpdef _BpfUnaryFunc acos(self): 
-        """Returns a bpf representing the arc cosine of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 9)
-    
-    cpdef _BpfUnaryFunc asin(self): 
-        """Returns a bpf representing the arc sine of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 10)
-    
-    cpdef _BpfUnaryFunc tan(self):  
-        """Returns a bpf representing the tan of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 11)
-    
-    cpdef _BpfUnaryFunc sinh(self): 
-        """Returns a bpf representing the sinh of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 12)
-    
-    cpdef _BpfUnaryFunc log10(self): 
-        """Returns a bpf representing the log10 of this bpf"""
-        return _BpfUnaryFunc_new_from_index(self, 13)
-    
-    cpdef _BpfLambdaLog log(self, double base=M_E): 
-        """
-        Returns a bpf representing the log of this bpf
-
-        Args:
-            base (float): the base of the log
-
-        Returns:
-            (BpfInterface) A bpf representing `\\x -> log(self(x), base)`
-
-        """
-        return _BpfLambdaLog(self, base, self.bounds())
-    
-    cpdef _BpfM2F m2f(self):
-        """Returns a bpf converting from midinotes to frequency
-
-        Returns:
-            (BpfInterface) A bpf representing `\\x -> m2f(self(x))`
-
-        ## Example
-
-        ```python
-        >>> from bpf4 import *
-        >>> midinotes = linear(0, 60, 1, 65)
-        >>> freqs = midinotes.m2f()
-        >>> freqs.map(10)
-        array([262.81477242, 271.38531671, 280.23535149, 289.37399111,
-               298.81064715, 308.55503809, 318.61719934, 329.0074936 ,
-               339.73662146, 350.81563248])
-        ```
-        """
-        return _BpfM2F(self)
-    
-    cpdef _BpfF2M f2m(self): 
-        """Returns a bpf converting frequencies to midinotes
-        
-        Returns:
-            (BpfInterface) A bpf representing `\\x -> f2m(self(x))`
-
-        ## Example
-        
-        ```python
-        >>> from bpf4 import *
-        >>> freqs = linear(0, 442, 1, 882)
-        >>> freqs.f2m().map(10)
-        array([69.        , 70.82403712, 72.47407941, 73.98044999, 75.3661766 ,
-               76.64915905, 77.84358713, 78.96089998, 80.01045408, 81.        ])
-        ```
-        """
-        return _BpfF2M(self)
-    
-    cpdef _Bpf_db2amp db2amp(self): 
-        """
-        Returns a bpf converting decibels to linear amplitudes
-
-        Returns:
-            (BpfInterface) A bpf representing `\\x -> db2amp(self(x))`
-
-        ## Example
-
-        ```python
-        >>> linear(0, 0, 1, -60).db2amp().map(10)
-        array([1.        , 0.46415888, 0.21544347, 0.1       , 0.04641589,
-               0.02154435, 0.01      , 0.00464159, 0.00215443, 0.001     ])
-        ```
-        """
-        return _Bpf_db2amp(self)
-    
-    cpdef _Bpf_amp2db amp2db(self):
-        """
-        Returns a bpf converting linear amplitudes to decibels
-
-        Returns:
-            (BpfInterface) A bpf representing `\\x -> amp2db(self(x))`
-
-        ## Example
-
-        ```python
-        >>> linear(0, 0, 1, 1).amp2db().map(10)
-        array([-280.        ,  -19.08485019,  -13.06425028,   -9.54242509,
-               -7.04365036,   -5.1054501 ,   -3.52182518,   -2.18288939,
-               -1.02305045,    0.        ])
-        ```
-        """    
-        return _Bpf_amp2db(self)
-    
-    cpdef _BpfLambdaClip clip(self, double y0=INFNEG, double y1=INF): 
-        """
-        Return a bpf clipping the result between y0 and y1
-
-        Args:
-            y0 (float): the min. *y* value
-            y1 (float): the max. *y* value
-
-        Returns:
-            (BpfInterface) A view of this bpf clipped to the given
-            *y* values
-
-        ```python
-
-        >>> a = linear(0, -1, 1, 1).clip(0, 1)
-        >>> a.map(20)
-        array([0.        , 0.        , 0.        , 0.        , 0.        ,
-               0.        , 0.        , 0.        , 0.        , 0.        ,
-               0.05263158, 0.15789474, 0.26315789, 0.36842105, 0.47368421,
-               0.57894737, 0.68421053, 0.78947368, 0.89473684, 1.        ])
-        >>> a.plot()
-        ```
-        ![](assets/clip1.png)
-        """
-        return _BpfLambdaClip_new(self, y0, y1)
-
-    cpdef BpfInterface derivative(self):
-        """
-        Create a curve which represents the derivative of this curve
-
-        Returns:
-            (BpfInterface) A bpf which returns the derivative of this 
-            bpf at any given x coord
-
-        It implements Newtons difference quotiont, so that:
-
-        ```
-
-                        bpf(x + h) - bpf(x)
-        derivative(x) = -------------------
-                                  h
-        ```
-
-        Example
-        -------
-
-        ```python
-        
-        >>> from bpf4 import *
-        >>> a = slope(1)[0:6.28].sin()
-        >>> a.plot(show=False, color="red")
-        >>> b = a.derivative()
-        >>> b.plot(color="blue")
-
-        ```
-        ![](assets/derivative1.png)
-        """
-        return _BpfDeriv(self)
-
-    cpdef BpfInterface integrated(self):
-        """
-        Return a bpf representing the integration of this bpf at a given point
-
-        Returns:
-            (BpfInterface) A bpf representing the integration of this bpf
-
-        Example
-        -------
-
-        ```python
-        a = linear(0, 0, 5, 5)
-        b = a.integrated()
-        a.plot(show=False, color="red")
-        b.plot(color="blue")
-        ```
-        ![](assets/integrated1.png)
-
-        !!! info "See Also"
-
-            * [.integrate](#integrate)
-        """
-
-        if self._x0 == INFNEG:
-            raise ValueError("Cannot integrate a function with an infinite negative bound")
-        return _BpfIntegrate(self)
-    
-    cpdef double integrate(self):
-        """
-        Return the result of the integration of this bpf. 
-
-        If any of the bounds is `inf`, the result is also `inf`.
-
-        !!! note
-
-            To set the bounds of the integration, first crop the bpf by slicing it: `bpf[start:end]`
-        
-        Returns:
-            (float) The result of the integration
-
-        ## Example
-
-        ```python
-
-        >>> linear(0, 0, 10, 10).sin()[0:2*pi].integrate()
-        -1.7099295055304798e-17
-        
-        ```
-        """
-        if isinf(self._x0) or isinf(self._x1):
-            return INFINITY
-        return self.integrate_between(self._x0, self._x1)
-    
-    cdef double _trapz_integrate_between(self, double x0, double x1, size_t N=0):
-        """
-        Integrate this bpf between [x0, x1] using the traptz method
-
-        Args:
-            x0 (float): start of integration period
-            x1 (float): end of the integration period
-            N (int): number of subdivisions used to calculate the integral. If not given, 
-               a default is used (default defined in `CONFIG['integrate.trapz_intervals']`)
-
-        Returns:
-            (float) The result of the integration
-        """
-        cdef:
-            double dx
-            double [::1] ys
-        if N == 0:
-            N = CONFIG['integrate.trapz_intervals']
-        dx = (x1 - x0) / N
-        if dx <= 0:
-            return 0.0
-        ys = self.sample_between(x0, x1, dx)
-        return _integr_trapz(&ys[0], ys.shape[0], dx)
-    
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        """
-        Integrate this bpf between x0 and x1
-
-        Args:
-            x0: start x of the integration range
-            x1: end x of the integration range
-            N: number of intervals to use for integration
-
-        Returns:
-            (float) The result of the integration
-        """
-
-        cdef double out
-        cdef int get_mode
-        cdef int mode = self._integration_mode
-        cdef double outbound0, outbound1, inbound
-        if x1 > self._x1:
-            outbound1 = self.__ccall__(x1) * (x1 - self._x1)
-            x1 = self._x1
-        else:
-            outbound1 = 0
-        if x0 < self._x0:
-            outbound0 = self.__ccall__(x0) * (self._x0 - x0)
-            x0 = self._x0
-        else:
-            outbound0 = 0
-        # override mode when N is given
-        if N > 0:
-            mode = 0
-        if mode == 1 or mode == 2:
-            inbound = integrate_simpsons(self, x0, x1, SIMPSONS_ACCURACY, SIMPSONS_MAXITER)
-        else:
-            inbound = self._trapz_integrate_between(x0, x1, N)
-        return outbound0 + inbound + outbound1
-
-    cpdef double mean(self):
-        """
-        Calculate the mean value of this bpf. 
-
-        Returns:
-            (float) The average value of this bpf along its bounds
-
-        To constrain the calculation to a given portion, use:
-
-        ```python
-
-        bpf.integrate_between(start, end) / (end-start)
-        
-        ```
-        """
-        return self.integrate() / (self._x1 - self._x0)
-
-    cpdef list zeros(self, double h=0.01, int N=0, double x0=NAN, double x1=NAN, int maxzeros=0):
-        """
-        Find the zeros of this bpf
-        
-        Args:
-            h: the accuracy to scan for zero-crossings. If two zeros are within 
-                this distance, they will be resolved as one.
-            N: alternatively, you can give the number of intervals to scan. 
-                h will be derived from this
-            x0: the point to start searching. If not given, the starting point of this bpf
-                will be used
-            x1: the point to stop searching. If not given, the end point of this bpf is used
-            maxzeros: if > 0, stop the search when this number of zeros have been found
-            
-        Returns:
-            (List[float]) A list with the zeros of this bpf
-
-
-        ## Example
-        
-        ```python
-        
-        >>> a = bpf.linear(0, -1, 1, 1)
-        >>> a.zeros()
-        [0.5]
-        
-        ```
-
-        """
-        return bpf_zero_crossings(self, h=h, N=N, x0=x0, x1=x1, maxzeros=maxzeros)
-
-    def max(self, b):
-        """
-        Returns a bpf representing `max(self, b)`
-
-        Args:
-            b (float | BpfInterface): a const float or a bpf
-
-        Returns:
-            (Max) A Max bpf representing `max(self, b)`, which can be
-            evaluated at any x coord
-        
-        ## Example
-        
-        ```python
-        >>> from bpf4 import *
-        >>> a = linear(0, 0, 1, 10)
-        >>> b = a.max(4)
-        >>> b(0), b(0.5), b(1)
-        (4.0, 5.0, 10.0)
-        >>> b.plot()
-        ```
-        ![](assets/maxconst.png)
-        """
-        
-        if isinstance(b, BpfInterface):
-            return Max(self, b)
-        return _BpfMaxConst(self, b, self.bounds())
-
-    def min(self, b):
-        """
-        Returns a bpf representing `min(self, b)`
-
-        Args:
-            b (float | BpfInterface): a const float or a bpf
-
-        Returns:
-            (Min) A Min bpf representing `min(self, b)`, which can be
-            evaluated at any x coord
-        
-        ## Example
-        
-        ```python
-        >>> from bpf4 import *
-        >>> a = linear(0, 0, 1, 10)
-        >>> b = a.min(4)
-        >>> b(0), b(0.5), b(1)
-        (0, 4.0, 5.0)
-        >>> b.plot()
-        ```
-        ![](assets/minconst.png)
-        """
-        if isinstance(b, BpfInterface):
-            return Min(self, b)
-        return _BpfMinConst(self, b, self.bounds())
-
-    def __reduce__(self):
-        return type(self), self.__getstate__()
-
-    cdef double __ccall__(self, double other) nogil:
-        return 0.0
-
-    def __call__(BpfInterface self, double x):
-        """
-        BpfInterface.__call__(self, double x)
-
-        Args:
-            x (float): evaluate this bpf at the given x coord
-
-        Returns:
-            (float) The value of this bpf at x
-        """
-        return self.__ccall__(x)
-
-    def keep_slope(self, double epsilon=DEFAULT_EPSILON):
-        """
-        A view of this bpf where the slope is continued outside its bounds
-
-
-        Return a new bpf which is a copy of this bpf when inside
-        bounds() but outside bounds() it behaves as a linear bpf
-        with a slope equal to the slope of this bpf at its extremes
-        
-        Args:
-            epsilon (float): an epsilon value to use when deriving the
-                this bpf to calculate its slope
-
-        Returns:
-            (BpfInterface) A view of this bpf which keeps its slope outside
-            its bounds (instead of just returning the last defined value)
-
-        Example
-        -------
-
-        ```python
-
-        a = expon(1, 1, 2, 2, exp=2)
-        b = a.keep_slope()
-        b[0:3].plot(show=False, color="grey")
-        a.plot(color="black", linewidth=3)
-        ```
-        ![](assets/keepslope1.png)
-        """
-        return _BpfKeepSlope(self, epsilon)
-
-    def outbound(self, double y0, double y1):
-        """
-        Return a new Bpf with the given values outside the bounds
-
-        ## Examples
-        
-        ```python
-
-        >>> from bpf4 import *
-        >>> a = linear(0, 1, 1, 10).outbound(-1, 0)
-        >>> a(-0.5)
-        -1
-        >>> a(1.1)
-        0
-        >>> a(0)
-        1
-        >>> a(1)
-        10
-
-        # fallback to another curve outside self
-        >>> a = linear(0, 1, 1, 10).outbound(0, 0) + expon(-1, 2, 4, 10, exp=2)
-        >>> a.plot()
-        ```
-        ![](assets/outbound1.png)
-        """
-        return _BpfCrop_new(self, self._x0, self._x1, OUTBOUND_SET, y0, y1)
-
-    def apply(self, func):
-        """
-        Create a bpf where `func` is applied to the result of this pdf
-        
-        Args:
-            func (callable): a function to apply to the result of this bpf
-
-        Returns:
-            (BpfInterface) A bpf representing `func(self(x))` 
-
-        **NB**: `a.apply(b)` is the same as `a | b`
-        
-        ## Example
-        
-        ```python
-
-        >>> from bpf4 import *
-        >>> from math import *
-        >>> a = linear(0, 0, 1, 10)
-        >>> def func(x):
-        ...     return sin(x) + 1
-        >>> b = a.apply(func)
-        >>> b(1)
-        0.4559788891106302
-        >>> sin(a(1)) + 1
-        0.4559788891106302
-        
-        ```
-
-        """
-        return _BpfCompose_new(self, _FunctionWrap(func))
-
-    def preapply(self, func):
-        """
-        Create a bpf where `func` is applied to the argument before it is passed
-
-        This is equivalent to `func(x) | self`
-        
-        Args:
-            func (callable): a function `func(x: float) -> float` which is applied to
-                the argument before passing it to this bpf
-
-        Returns:
-            (BpfInterface) A bpf following the pattern `lambda x: bpf(func(x))`
-
-        ## Example
-        
-        ```python
-
-        >>> bpf = Linear((0, 1, 2), (0, 10, 20))
-        >>> bpf(0.5)
-        5
-
-        >>> shifted_bpf = bpf.preapply(lambda x: x + 1)
-        >>> shifted_bpf(0.5)
-        15
-        ```
-
-        **NB**: `bpf1.preapply(bpf2)` is the same as `bpf2 | bpf1`
-        """
-        return _BpfCompose_new(_FunctionWrap(func), self)
-
-    def periodic(self):
-        """
-        Create a new bpf which replicates this in a periodic way
-
-        Returns:
-            (BpfInterface) A periodic view of this bpf
-
-        The new bpf is a copy of this bpf when inside its bounds 
-        and outside it, it replicates it in a periodic way, with no bounds.
-
-        ## Example
-            
-        ```python
-
-        >>> from bpf4 import *
-        >>> a = core.Linear((0, 1), (-1, 1)).periodic()
-        >>> a
-        _BpfPeriodic[-inf:inf]
-        >>> a.plot()
-        ```
-        ![](assets/periodic1.png)
-        """
-        return _BpfPeriodic(self)
-
-    def stretched(self, double rx, double fixpoint=0.):
-        """
-        Returns a view of this bpf stretched over the x axis. 
-
-        **NB**: to stretch over the y-axis, just multiply this bpf
-        
-        !!! info "See Also"
-
-            [fit_between()](#fit_between)
-
-        Args:
-            rx (float): the stretch factor
-            fixpoint (float): the point to use as reference
-
-        Returns:
-            (BpfInterface) A projection of this bpf stretched/compressed by
-            by the given factor
-
-        ## Example
-
-        Stretch the shape of the bpf, but preserve the start position
-        
-        ```python
-            
-        >>> a = linear(1, 1, 2, 2)
-        >>> b = a.stretched(4, fixpoint=a.x0)
-        >>> b.bounds()
-        (1, 9)
-        >>> a.plot(show=False); b.plot()
-
-        ```
-        """
-        if rx == 0:
-            raise ValueError("the stretch factor cannot be 0")
-        
-        if self._x0 == INF or self._x0 == INFNEG or self._x1 == INF or self._x1 == INFNEG:
-            qrx = 1/rx
-            return _BpfProjection(rx=qrx, dx=0, offset=fixpoint)
-        
-        cdef double x0 = self._x0
-        cdef double x1 = self._x1
-        cdef double p0 = (x0 - fixpoint)*rx + fixpoint
-        cdef double p1 = (x1 - x0) * rx + p0
-        return self.fit_between(p0, p1)
-        
-    cpdef BpfInterface fit_between(self, double x0, double x1):
-        """
-        Returns a view of this bpf fitted within the interval `x0:x1`
-
-        This operation only makes sense if the bpf is bounded
-        (none of its bounds is `inf`)
-
-        Args:
-            x0: the lower bound to fit this bpf
-            x1: the upper bound to fit this bpf
-
-        Returns:
-            (BpfInterface) The projected bpf
-
-        ## Example
-        
-        ```python
-
-        >>> from bpf4 import *
-        >>> a = linear(1, 1, 2, 5)
-        >>> a.bounds()
-        (1, 5)
-        >>> b = a.fit_between(0, 10)
-        >>> b.bounds()
-        0, 10
-        >>> b(10)
-        5
-        ```
-        """
-        cdef double rx
-        if self._x0 == INF or self._x0 == INFNEG or self._x1 == INF or self._x1 == INFNEG:
-            raise ValueError("This bpf is unbounded, cannot be fitted."
-                             "Use thisbpf[x0:x1].fit_between(...)")
-        rx = (self._x1 - self._x0) / (x1 - x0)
-        dx = self._x0
-        offset = x0
-        return _BpfProjection(self, rx=rx, dx=dx, offset=offset)
-
-
-    cpdef BpfInterface shifted(self, dx):
-        """
-        Returns a view of this bpf shifted by `dx` over the x-axes
-
-        This is the same as [.shift](#shift), but a new bpf is returned
-
-        ## Example
-        
-        ```python
-
-        >>> from bpf4 import *
-        >>> a = linear(0, 1, 1, 5)
-        >>> b = a.shifted(2)
-        >>> b(3) == a(1)
-        ```
-        """
-        return _BpfProjection(self, rx=1, dx=-dx)
-
-    def inverted(self):
-        """
-        Return a view on this bpf with the coords inverted
-
-        Returns:
-            (BpfInterface) a view on this bpf with the coords inverted
-
-        In an inverted function the coordinates are swaped: the inverted version of a 
-        bpf indicates which *x* corresponds to a given *y*
-        
-        Returns None if the function is not invertible. For a function to be invertible, 
-        it must be strictly increasing or decreasing, with no local maxima or minima.
-        
-        ```
-        f.inverted()(f(x)) = x
-        ```
-        
-        So if `y(1) == 2`, then `y.inverted()(2) == 1`
-
-        ![](assets/inverted.png)
-        """
-        try:
-            return _BpfInverted(self)
-        except ValueError:
-            return None
-
-    cpdef BpfInterface _slice(self, double x0, double x1):
-        return _BpfCrop_new(self, x0, x1, OUTBOUND_DEFAULT, 0, 0)
-
-    def __getitem__(self, slice):
-        cdef double x0, x1
-        cdef BpfInterface out
-        x0 = self._x0
-        x1 = self._x1
-        try:
-            if slice.start is not None:
-                x0 = slice.start
-            if slice.stop is not None:
-                x1 = slice.stop
-            if slice.step is not None:
-                return self.sampled_between(x0, x1, slice.step, 'linear')
-            return self._slice(x0, x1)
-        except AttributeError:
-            raise ValueError("BPFs accept only slices, not single items.")
-    
-    @classmethod
-    def fromseq(cls, *points, **kws):
-        """
-        A helper constructor with points given as tuples or as a flat sequence. 
-
-        ## Example
-
-        These operations result in the same bpf:
-
-        ```python
-        Linear.fromseq(x0, y0, x1, y1, x2, y2, ...)
-        Linear.fromseq((x0, y0), (x1, y1), (x2, y2), ...)
-        Linear((x0, x1, ...), (y0, y1, ...))
-        ```
-
-        Args:
-            points (ndarray | list[float]): either the interleaved x and y points, or each point as a
-                2D tuple
-            `**kws` (dict): any keyword will be passed to the default constructor (for 
-                example, `exp` in the case of an `Expon` bpf)
-
-        Returns:
-            (BpfBase) The constructed bpf
-        """
-        cdef ndarray data
-        cdef int lenpoints
-        if isinstance(points[0], (list, tuple)):
-            # (x0, y0), (x1, y1), ...
-            data = numpy.asarray(points, dtype=DTYPE)
-            return cls(data[:,0], data[:,1], **kws)
-        else:
-            # x0, y0, x1, y1, ...
-            lenpoints = len(points)
-            if lenpoints % 2 != 0:
-                raise ValueError(
-                    "The instantiation form x0, y0, x1, y1 should have an even number of args"
-                )
-            if lenpoints == 2:
-                return cls((points[0], points[1]), (points[0], points[1]), **kws)
-            elif lenpoints == 1:
-                return cls((0, 0), (0, points[0]), **kws)
-            else:
-                return cls(points[::2], points[1::2], **kws)
-
-    def copy(self):
-        """
-        Create a copy of this bpf
-
-        Returns:
-            (BpfInterface) A copy of this bpf
-        """
-        state = self.__getstate__()
-        obj = self.__class__(*state)
-        obj.__setstate__(state)
-        return obj
-    
-    def __repr__(self):
-        x0, x1 = self.bounds()
-        return "%s[%s:%s]" % (self.__class__.__name__, str(x0), str(x1))
-
-    
-
-cdef BpfInterface _asbpf(obj):
-    if isinstance(obj, BpfInterface):
-        return obj
-    if hasattr(obj, '__call__'):
-        return _FunctionWrap(obj, (INFNEG, INF))
-    elif hasattr(obj, '__float__'):
-        return Const(float(obj))
-    else:
-        return None
-
-   
-cdef inline ndarray _asarray(obj): 
-    return <ndarray>(PyArray_GETCONTIGUOUS(array(obj, DTYPE, False)))
-
-
-cdef class BpfBase(BpfInterface):
-    cdef ndarray xs, ys
-    cdef DTYPE_t* xs_data
-    cdef DTYPE_t* ys_data
-    cdef int outbound_mode
-    cdef double outbound0, outbound1
-    cdef double lastbin_x0, lastbin_x1
-    cdef InterpolFunc *interpol_func
-    cdef Py_ssize_t xs_size
-    cdef size_t lastbin_idx1
-
-
-    def __cinit__(self):
-        self.interpol_func = NULL
-        self.ys_data = NULL
-        self.xs_data = NULL
-        self.xs = None
-        self.ys = None
-
-    def __dealloc__(self):
-        InterpolFunc_free(self.interpol_func)
-
-    def __init__(BpfBase self, xs, ys):
-        """
-        Base constructor for bpfs
-
-        xs and ys should be of the same size
-
-        Args:
-            xs (list[float] | numpy.ndarray): x data 
-            ys (list[float] | numpy.ndarray): y data
-
-
-        """
-        cdef int len_xs, len_ys
-        cdef ndarray [DTYPE_t, ndim=1] _xs = numpy.ascontiguousarray(xs, DTYPE)
-        if _array_issorted(_xs) < 1:
-            raise BpfPointsError(f"Points along the x coord should be sorted without duplicates.\n xs:\n{xs}")
-        cdef ndarray [DTYPE_t, ndim=1] _ys = numpy.ascontiguousarray(ys, DTYPE)
-        len_xs = PyArray_DIM(_xs, 0)
-        len_ys = PyArray_DIM(_ys, 0)
-        if len_xs != len_ys:
-            raise ValueError("xs and ys must be of equal length, but xs has %d items "
-                             "and ys has %d items" % (len_xs, len_ys))
-        if len_xs < 1:
-            raise ValueError("Can't creat a BPF of 0 points")
-        self.xs = _xs
-        self.ys = _ys
-        self.xs_size = PyArray_DIM(_xs, 0)
-        self._set_bounds(_xs[0], _xs[len_xs - 1])
-        self.outbound_mode = OUTBOUND_CACHE
-        self.outbound0 = _ys[0]
-        self.outbound1 = _ys[len_ys - 1]
-        self.xs_data = <DTYPE_t*>(self.xs.data)
-        self.ys_data = <DTYPE_t*>(self.ys.data)
-        self.lastbin_x0 = self.xs[0]
-        self.lastbin_x1 = self.xs[1]
-        self.lastbin_idx1 = 1
-
-    @property
-    def descriptor(self) -> str: 
-        """
-        A string describing the interpolation function of this bpf
-        """
-        return InterpolFunc_get_descriptor(self.interpol_func)
-
-    cdef void _bounds_changed(self):
-        self._invalidate_cache()
-
-    cdef void _invalidate_cache(self):
-        cdef int last_index = PyArray_DIM(self.xs, 0) - 1
-        self.lastbin_x0 = 0
-        self.lastbin_x1 = 0
-        self.lastbin_idx1 = 0
-        if self.ys_data != NULL and self.outbound_mode == OUTBOUND_CACHE:
-            self.outbound0 = (<DTYPE_t *>(self.ys_data))[0]
-            self.outbound1 = (<DTYPE_t *>(self.ys_data))[last_index]
-        
-    def outbound(self, double y0, double y1):
-        """
-        Set the values **inplace** returned when this bpf is evaluated outside its bounds.
-
-        The default behaviour is to interpret the values at the bounds to extend to infinity.
-
-        In order to not change this bpf inplace, use `b.copy().outbound(y0, y1)`
-        """
-        self.outbound_mode = OUTBOUND_SET
-        self.outbound0 = y0
-        self.outbound1 = y1
-        return self
-
-    def __getstate__(self):
-        return (self.xs, self.ys)
-
-    def __setstate__(self, state):
-        self.xs, self.ys = state
-
-    cdef double __ccall__(BpfBase self, double x) nogil:
-        cdef double res, x0, y0, x1, y1
-        cdef int index0, index1, nx
-        if self.lastbin_x0 <= x < self.lastbin_x1:
-            res = InterpolFunc_call(self.interpol_func, x, self.lastbin_x0, self.ys_data[self.lastbin_idx1-1], 
-                                    self.lastbin_x1, self.ys_data[self.lastbin_idx1])
-        elif x < self._x0:
-            res = self.outbound0
-        elif x > self._x1:
-            res = self.outbound1
-        elif (self.lastbin_idx1 < self.xs_size - 2) and (self.lastbin_x1 <= x < self.xs_data[self.lastbin_idx1+1]):
-            # usual situation: cross to next bin
-            index1 = self.lastbin_idx1 + 1
-            x1 = self.xs_data[index1]
-            res = InterpolFunc_call(self.interpol_func, x, self.lastbin_x1, self.ys_data[index1-1], x1, self.ys_data[index1])
-            self.lastbin_x0 = self.lastbin_x1
-            self.lastbin_x1 = x1
-            self.lastbin_idx1 = index1
-        else:
-            # out of cache call, find new boundaries and update cache
-            index1 = _csearchsorted(self.xs_data, self.xs_size, x)
-            x0 = self.xs_data[index1-1]
-            x1 = self.xs_data[index1]
-            res = InterpolFunc_call(self.interpol_func, x, x0, self.ys_data[index1-1], x1, self.ys_data[index1])
-            self.lastbin_x0 = x0
-            self.lastbin_x1 = x1
-            self.lastbin_idx1 = index1
-        return res
-
-    cpdef ndarray mapn_between(self, int n, double xstart, double xend, ndarray out=None):
-        cdef double[::1] result = out if out is not None else EMPTY1D(n)
-        cdef double dx = _ntodx(n, xstart, xend)
-        cdef double x = xstart, y
-        cdef size_t i = 0, j
-        cdef double outbound1 = self.outbound1
-        cdef double outbound0 = self.outbound0
-        cdef DTYPE_t *xs_data = self.xs_data
-        cdef DTYPE_t *ys_data = self.ys_data
-        cdef double xs_data0, xs_data1, ys_data0, ys_data1
-        cdef double x1 = self._x1
-        cdef int64_t index0 = 0
-        cdef double interpmix = self.interpol_func.mix
-        with nogil:
-            if xstart < self._x0:
-                j = min(n, <int>((self._x0 - xstart) / dx) + 1)
-                for i in range(j):
-                    result[i] = outbound0
-                i = j
-            x = xstart + i*dx
-            if self._x0 <= x <= self._x1:
-                index0 = _csearchsorted(self.xs_data, self.xs_size, x) - 1
-            elif x > self._x1:
-                for j in range(i, n):
-                    result[j] = outbound1
-                i = n
-                
-            xs_data0 = xs_data[index0]
-            xs_data1 = xs_data[index0+1]
-            ys_data0 = ys_data[index0]
-            ys_data1 = ys_data[index0+1]
-            while x <= x1 and i < n:
-                if x > xs_data1:
-                    index0 = _csearchlinear(xs_data, self.xs_size, x, index0)
-                    xs_data0 = xs_data[index0]
-                    xs_data1 = xs_data[index0+1]
-                    ys_data0 = ys_data[index0]
-                    ys_data1 = ys_data[index0+1]
-                
-                result[i] = InterpolFunc_call(self.interpol_func, x, xs_data0, ys_data0, xs_data1, ys_data1)
-                i += 1
-                x = xstart + i*dx
-            if i < n - 1:
-                for j in range(i, n):
-                    result[j] = outbound1  
-        return numpy.asarray(result)
-        
-    cpdef ndarray _mapn_between(self, int n, double xstart, double xend, ndarray out=None):
-        """
-        Return an array of `n` elements resulting of evaluating this bpf regularly
-
-        The x coordinates at which this bpf is evaluated are equivalent to `linspace(xstart, xend, n)`
-
-        Args:
-            n (int): the number of elements to generate
-            xstart (float): x to start mapping
-            xend (float): x to end mapping
-            out (ndarray): if given, result is put here
-
-        Returns:
-            (ndarray) An array of this bpf evaluated at a grid [xstart:xend:dx], where *dx*
-            is `(xend-xstart)/n`
-        """
-        cdef double[:] result = out if out is not None else EMPTY1D(n)
-        cdef double dx = (xend - xstart) / (n - 1)   # we account for the edge (x1 IS INCLUDED)
-        with nogil:        
-            for i in range(n):
-                result[i] = self.__ccall__(xstart + dx*i)
-        return numpy.asarray(result)
-        
-    def __repr__(self):
-        return "%s[%s:%s]" % (self.__class__.__name__, str(self._x0), str(self._x1))
-
-    def stretch(self, double rx):
-        """
-        Stretch or compress this bpf in the x-coordinate **INPLACE**
-
-        **NB**: use `stretched` to create a new bpf
-
-        Args:
-            rx (float): the stretch/compression factor
-
-        """
-        if rx == 0:
-            raise ValueError("the stretch factor cannot be 0")
-        self.xs *= rx
-        self._recalculate_bounds()
-    
-    def shift(self, double dx):
-        """
-        Shift the bpf along the x-coords, **INPLACE**
-        
-        Use [.shifted](#shifted) to create a new bpf
-
-        Args:
-            dx (float): the shift interval
-
-        """
-        self.xs += dx
-        self._recalculate_bounds()
-
-    cdef void _recalculate_bounds(self):
-        cdef DTYPE_t* data
-        cdef int nx
-        nx = PyArray_DIM(self.xs, 0)
-        self.xs_data = <DTYPE_t*>self.xs.data
-        self._x0 = self.xs_data[0]
-        self._x1 = self.xs_data[nx - 1]
-        self._invalidate_cache()
-
-    def points(BpfBase self):
-        """
-        Returns a tuple with the points defining this bpf
-
-        Returns:
-            (tuple[ndarray, ndarray]) a tuple (xs, ys) where `xs` is an array
-            holding the values for the *x* coordinate, and `ys` holds the values for
-            the *y* coordinate
-
-        ## Example
-        
-        ```python
-
-        >>> b = Linear.fromseq(0, 0, 1, 100, 2, 50)
-        >>> b.points()
-        ([0, 1, 2], [0, 100, 50])
-        ```
-
-        """
-        return self.xs, self.ys
-
-    def clone_with_new_data(self, xs: ndarray, ys: ndarray) -> BpfInterface:
-        """
-        Create a new bpf with the same attributes as self but with new data
-
-        Args:
-            xs (ndarray): the x-coord data
-            ys (ndarray): the y-coord data
-
-        Returns:
-            (BpfInterface) The new bpf. It will be of the same class as self
-
-        """
-        state = self.__getstate__()
-        newstate = (xs, ys) + state[2:]
-        return self.__class__(*newstate)
-        
-    def insertpoint(self, double x, double y):
-        """
-        Return **a copy** of this bpf with the point `(x, y)` inserted
-
-        !!! note
-
-            *self* is not modified
-
-        Args:
-            x (float): x coord
-            y (float): y coord
-
-        Returns:
-            (BpfInterface) A clone of this bpf with the point inserted
-        """
-        cdef int index = _searchsorted(self.xs, x)
-        new_xs = numpy.insert(self.xs, index, x)
-        new_ys = numpy.insert(self.ys, index, y)
-        return self.clone_with_new_data(new_xs, new_ys)
-
-    def removepoint(self, double x):
-        """
-        Return a copy of this bpf with point at x removed
-
-        Args:
-            x (float): the x point to remove
-
-        Returns:
-            (BpfInterface) A copy of this bpf with the given point removed
-        
-        Raises `ValueError` if x is not in this bpf
-        
-        To remove elements by index, do:
-
-        ```python
-
-        xs, ys = mybpf.points()
-        xs = numpy.delete(xs, indices)
-        ys = numpy.delete(ys, indices)
-        mybpf = mybpf.clone_with_new_data(xs, ys)
-
-        ```
-        """
-        cdef int index = _csearchsorted_left(self.xs_data, self.xs.size, x)
-        if self.xs_data[index] != x:
-            raise ValueError("%f is not in points" % x)
-        newxs = numpy.delete(self.xs, index)
-        newys = numpy.delete(self.ys, index)
-        return self.clone_with_new_data(newxs, newys)
-
-    def segments(self):
-        """
-        Return an iterator over the segments of this bpf
-
-        Returns:
-            (Iterable[tuple[float, float, str, float]]) An iterator of segments, 
-            where each segment has the form `(x, y, interpoltype:str, exponent)`
-
-        Each segment is a tuple `(x: float, y: float, interpoltype: str, exponent: float)`
-
-        Exponent is only of value if the interpolation type makes use of it.
-        """
-        cdef size_t i
-        cdef size_t num_segments
-        num_segments = len(self.xs) - 1
-        interpoltype = self.__class__.__name__.lower()
-        for i in range(num_segments):
-            yield (float(self.xs[i]), float(self.ys[i]), interpoltype, self.interpol_func.exp)
-        yield (float(self.xs[num_segments]), float(self.ys[num_segments]), '', 0)
-
-    @property
-    def exp(self) -> float:
-        """
-        The exponential of the interpolation function of this bpf
-        """
-        return self.interpol_func.exp
-
-
-cdef class Linear(BpfBase):
-    """
-    A bpf with linear interpolation
-
-    ```python
-    from bpf4 import *
-    a = core.Linear([0, 2, 3.5, 10], [0.1, 0.5, -3.5,  4])
-    a.plot()
-    ```
-    ![](assets/Linear.png)
-
-    """
-    def __init__(self, xs, ys):
-        """
-        Args:
-            xs (ndarray): the x-coord data
-            ys (ndarray): the y-coord data
-        """
-        self.interpol_func = InterpolFunc_linear
-        BpfBase.__init__(self, xs, ys)
-
-    def _get_points_for_rendering(self, int n= -1):
-        return self.xs, self.ys
-
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        """
-        Integrate this bpf between the given x coords
-
-        Args:
-            x0 (float): start of integration
-            x1 (float): end of integration
-            N (int): number of integration steps
-
-        Returns:
-            (float) The result representing the area beneath the curve
-            between *x0* and *x1*
-        """
-        cdef double pre, mid, post
-        cdef size_t index0, index1
-        if x0 <= self._x0:
-            pre = self.__ccall__(x0) * (self._x0 - x0)
-            index0 = 0
-        else:
-            index0 = _csearchsorted(self.xs_data, self.xs_size, x0)
-            # trapezium = (a+b)/2 * h (where h is the distance between a and b)
-            pre = (self.ys_data[index0] + self.__ccall__(x0)) * 0.5 * (self.xs_data[index0] - x0)
-        if x1 >= self._x1:
-            post = self.__ccall__(x1) * (x1 - self._x1)
-            index1 = self.xs_size - 1
-        else:
-            index1 = _csearchsorted_left(self.xs_data, self.xs_size, x1) - 1
-            post = (self.ys_data[index1] + self.__ccall__(x1)) * 0.5 * (x1-self.xs_data[index1])
-        mid = 0
-        for i in range(index0, index1):
-            mid += (self.ys_data[i] + self.ys_data[i+1]) * 0.5 * (self.xs_data[i+1] - self.xs_data[i])
-        return pre + mid + post
-
-    cpdef Linear sliced(self, double x0, double x1):
-        """
-        Cut this bpf at the given points
-
-        Args:
-            x0 (float): start x to cut
-            x1 (float): end x to cut
-
-        Returns:
-            (Linear) Copy of this bpf cut at the given x-coords
-
-        If needed it inserts points at the given coordinates to limit this bpf to 
-        the range `x0:x1`.
-
-        **NB**: this is different from crop, which is just a "view" into the underlying
-        bpf. In this case a real `Linear` bpf is returned. 
-        """
-        X, Y = arraytools.arrayslice(x0, x1, self.xs, self.ys)
-        return Linear(X, Y)
-        
-    def inverted(self):
-        """
-        Return a new Linear bpf where x and y coordinates are inverted. 
-
-        This is only possible if y never decreases in value. Otherwise
-        a `ValueError` is thrown
-        
-        Returns:
-            (Linear) The inverted bpf
-
-        ![](assets/inverted.png)
-        """
-        res = _array_issorted(self.ys)
-        if res == -1 or res == 0:  # not sorted or has dups
-            raise ValueError(f"bpf can't be inverted, ys must always increase.\nys={self.ys}")
-        return Linear(self.ys, self.xs)
-        
-    def flatpairs(self):
-        """
-        Returns a flat 1D array with x and y values interlaced
-
-        Returns:
-            (ndarray) A 1D array representing the points of this bpf with *xs* and
-            *ys* interleaved
-
-        ```python
-
-        >>> a = linear(0, 0, 1, 10, 2, 20)
-        >>> a.flatpairs()
-        array([0, 0, 1, 10, 2, 20])
-
-        ```
-        """
-        return arraytools.interlace_arrays(self.xs, self.ys)
-
-
-cdef class Smooth(BpfBase):
-    """
-    A bpf with smoothstep interpolation. 
-
-    ```python
-
-    >>> a = Smooth([0, 1, 3, 10], [0.1, 0.5, -3.5,  1])
-    >>> a.plot()
-    ```
-    ![](assets/Smooth.png)
-
-    ```python
-    >>> a = core.Smooth([0, 1, 3, 10], [0.1, 0.5, -3.5,  1], numiter=3)
-    >>> a.plot()
-    ```
-    ![](assets/Smooth_numiter3.png)
-
-    """
-        
-    def __init__(self, xs, ys, int numiter=1):
-        """
-        Args:
-            xs (ndarray): the x-coord data
-            ys (ndarray): the y-coord data
-            numiter (int): the number of smoothstep steps
-
-        """
-        if numiter == 1:
-            self.interpol_func = InterpolFunc_smooth
-        else:
-            self.interpol_func = InterpolFunc_new(intrp_smooth, 1, "smooth", 1)
-            self.interpol_func.numiter = numiter
-        BpfBase.__init__(self, xs, ys)
-
-
-cdef class Smoother(BpfBase):
-    """
-    A bpf with smootherstep interpolation (perlin's variation of smoothstep) 
-
-    ```python
-
-    a = core.Smooth([0, 1, 3, 10], [0.1, 0.5, -3.5,  1])
-    b = core.Smoother(*a.points())
-    fig, axes = plt.subplots(1, 2, figsize=(12, 4))
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1])
-    ```
-    ![](assets/Smoother.png)
-
-    """
-    def __init__(self, xs, ys):
-        self.interpol_func = InterpolFunc_smoother
-        BpfBase.__init__(self, xs, ys)
-
-
-cdef class Halfcos(BpfBase):
-    """
-    A bpf with half-cosine interpolation
-
-    [HalfcosExp](#HalfcosExp) is the same as Halfcos. It exists with two
-    names for compatibility
-
-    ```python
-    a = core.Halfcos([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
-    b = core.Halfcos(*a.points(), exp=2)
-    c = core.Halfcos(*a.points(), exp=0.5)
-    fig, axes = plt.subplots(1, 3, figsize=(16, 4), tight_layout=True)
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1], show=False)
-    c.plot(axes=axes[2])
-    ```
-    ![](assets/Halfcos.png)
-    """
-    def __init__(self, xs, ys, double exp=1.0, int numiter=1):
-        """
-        Args:
-            xs (ndarray): the x-coord data
-            ys (ndarray): the y-coord data
-            exp (float): an exponent applied to the halfcosine interpolation
-            numiter (int): how many times to apply the interpolation
-
-        """
-        if exp == 1.0 and numiter == 1:
-            self.interpol_func = InterpolFunc_halfcos
-        elif exp == 1:
-            self.interpol_func = InterpolFunc_new(intrp_halfcos, 1, 'halfcos', 1)
-        else:
-            self.interpol_func = InterpolFunc_new(intrp_halfcosexp, exp, 'halfcosexp', 1)
-        self.interpol_func.numiter = numiter
-        super().__init__(xs, ys)
-    
-    def __getstate__(self):
-        return self.xs, self.ys, self.interpol_func.exp, self.interpol_func.numiter
-
-    def __repr__(self):
-        exp = self.interpol_func.exp
-        return "%s[%s:%s] exp=%s" % (self.__class__.__name__, str(self._x0), str(self._x1), str(exp))
-    
-
-HalfcosExp = Halfcos
-    
-
-cdef class Halfcosm(Halfcos):
-    """
-    A bpf with half-cosine and exponent depending on the orientation of the interpolation
-
-    When interpolating between two y values, y0 and y1, if  y1 < y0 the exponent
-    is inverted, resulting in a symmetrical interpolation shape
-
-    ```python
-    a = core.Halfcos([0, 1, 3, 10], [0.1, 0.5, 3.5,  1], exp=2)
-    b = core.Halfcosm(*a.points(), exp=2)
-    fig, axes = plt.subplots(1, 2, figsize=(16, 4))
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1])
-    ```
-    ![](assets/Halfcosm.png)
-
-    """
-    def __init__(self, xs, ys, double exp=1.0, int numiter=1):
-        self.interpol_func = InterpolFunc_new(intrp_halfcosexpm, exp, 'halfcosexpm', 1)
-        self.interpol_func.numiter = numiter
-        BpfBase.__init__(self, xs, ys)
-
-
-cdef class Expon(BpfBase):
-    """
-    A bpf with exponential interpolation
-
-    Example
-    -------
-
-    ```python
-    from bpf4 import *
-    import matplotlib.pyplot as plt
-    numplots = 5
-    fig, axs = plt.subplots(2, numplots, tight_layout=True, figsize=(20, 8))
-    for i in range(numplots):
-        exp = i+1
-        core.Expon([0, 1, 2], [0, 1, 0], exp=exp).plot(show=False, axes=axs[0, i])
-        core.Expon([0, 1, 2], [0, 1, 0], exp=1/exp).plot(show=False, axes=axs[1, i])
-        axs[0, i].set_title(f'{exp=}')
-        axs[1, i].set_title(f'exp={1/exp:.2f}')
-
-    plot.show()
-
-    ```
-    ![](assets/expon-grid2.png)
-    """
-    def __init__(self, xs, ys, double exp, int numiter=1):
-        """
-        Args:
-            xs (ndarray): the x-coord data
-            ys (ndarray): the y-coord data
-            exp (float): an exponent applied to the halfcosine interpolation
-            numiter (int): how many times to apply the interpolation
-        """
-        BpfBase.__init__(self, xs, ys)
-        self.interpol_func = InterpolFunc_new(intrp_expon, exp, 'expon', 1)  # must be freed
-        self.interpol_func.numiter = numiter
-    
-    def __getstate__(self): return self.xs, self.ys, self.interpol_func.exp
-    
-    def __setstate__(self, state):
-        self.xs, self.ys, exp = state
-        self.interpol_func.exp = exp
-
-    def __repr__(self):
-        return "%s[%s:%s] exp=%s" % (self.__class__.__name__, str(self._x0), str(self._x1), str(self.interpol_func.exp))
-
-
-cdef class Exponm(Expon):
-    """
-    A bpf with symmetrical exponential interpolation 
-
-    ```python
-    from bpf4 import *
-    import matplotlib.pyplot as plt
-    numplots = 5
-    fig, axs = plt.subplots(2, numplots, tight_layout=True, figsize=(20, 8))
-    for i in range(numplots):
-        exp = i+1
-        core.Exponm([0, 1, 2], [0, 1, 0], exp=exp).plot(show=False, axes=axs[0, i])
-        core.Exponm([0, 1, 2], [0, 1, 0], exp=1/exp).plot(show=False, axes=axs[1, i])
-        axs[0, i].set_title(f'{exp=}')
-        axs[1, i].set_title(f'exp={1/exp:.2f}')
-
-    plot.show()
-    ```
-
-    ![](assets/exponm-grid.png)
-    
-    """
-    def __init__(self, xs, ys, double exp, int numiter=1):
-        """
-        Args:
-            xs (ndarray): the x-coord data
-            ys (ndarray): the y-coord data
-            exp (float): an exponent applied to the halfcosine interpolation
-            numiter (int): how many times to apply the interpolation
-        """
-        BpfBase.__init__(self, xs, ys)
-        self.interpol_func = InterpolFunc_new(intrp_exponm, exp, 'exponm', 1)  # must be freed
-        self.interpol_func.numiter = numiter
-
-
-cdef class NoInterpol(BpfBase):
-    """
-    A bpf without interpolation
-
-    ```python
-    a = core.Linear([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
-    b = core.NoInterpol(*a.points())
-    c = core.Nearest(*a.points())
-    fig, axes = plt.subplots(1, 3, figsize=(15, 4), tight_layout=True)
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1], show=False)
-    c.plot(axes=axes[2])
-    ```
-    ![](assets/NoInterpol.png)
-    """
-    def __init__(self, xs, ys):
-        """
-        A bpf without interpolation
-
-        Args:
-            xs (ndarray): the x coord data
-            ys (ndarray): the y coord data
-        """
-        BpfBase.__init__(self, xs, ys)
-        self.interpol_func = InterpolFunc_nointerpol
-        
-
-cdef class Nearest(BpfBase):
-    """
-    A bpf with nearest interpolation
-
-    ```python
-    a = core.Linear([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
-    b = core.NoInterpol(*a.points())
-    c = core.Nearest(*a.points())
-    fig, axes = plt.subplots(1, 3, figsize=(15, 4), tight_layout=True)
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1], show=False)
-    c.plot(axes=axes[2])
-    ```
-    ![](assets/NoInterpol.png)
-    
-    """
-    def __init__(self, xs, ys):
-        """
-        A bpf with nearest interpolation
-
-        Args:
-            xs (ndarray): the x coord data
-            ys (ndarray): the y coord data
-        """
-        super().__init__(xs, ys)
-        self.interpol_func = InterpolFunc_nearest
-
-    def __getstate__(self): return self.xs, self.ys
-    
-
-ctypedef struct SplineS:
-    int use_low_slope
-    int use_high_slope
-    double low_slope
-    double high_slope
-    DTYPE_t *xs
-    DTYPE_t *ys
-    DTYPE_t *ys2
-    int length
-    npy_intp last_index
-
-
-cdef SplineS* SplineS_new(xs, ys, Py_ssize_t xs_size, double low_slope=0, double high_slope=0, int use_low_slope=0, int use_high_slope=0):
-    cdef SplineS *s = <SplineS *>malloc(sizeof(SplineS))
-    cdef int length = xs_size
-    cdef int i
-    cdef DTYPE_t * _xs = <DTYPE_t *>malloc(sizeof(DTYPE_t) * length)
-    cdef DTYPE_t * _ys = <DTYPE_t *>malloc(sizeof(DTYPE_t) * length)
-    for i in range(length):
-        _xs[i] = xs[i]
-        _ys[i] = ys[i]
-    s.xs = _xs
-    s.ys = _ys
-    s.low_slope = low_slope
-    s.high_slope = high_slope
-    s.use_low_slope = use_low_slope
-    s.use_high_slope = use_high_slope
-    s.last_index = length - 1
-    s.length = length
-    SplineS_calc_ypp(s)
-    return s
-
-
-cdef void SplineS_destroy(SplineS *self):
-    free(self.xs)
-    free(self.ys)
-    free(self.ys2)
-
-
-@cython.boundscheck(False)
-@cython.cdivision(True)
-cdef void SplineS_calc_ypp(SplineS *self) nogil:
-    cdef DTYPE_t *x_vals = self.xs
-    cdef DTYPE_t *y_vals = self.ys
-    cdef int n = self.length
-    cdef DTYPE_t *y2_vals = <DTYPE_t *>malloc(sizeof(DTYPE_t) * n)
-    cdef DTYPE_t *u =       <DTYPE_t *>malloc(sizeof(DTYPE_t) * (n - 1))  # this is a temporary array
-    cdef double x1_minus_x0, denom, sig, p, qn, un
-    cdef int i, k
-    if self.use_low_slope == 1:
-        x1_minus_x0 = x_vals[1] - x_vals[0]
-        # u[0] = (3.0/(x_vals[1]-x_vals[0])) * ((y_vals[1]-y_vals[0]) / (x_vals[1]-x_vals[0])-self.low_slope)
-        x1_minus_x0 += 1e-12
-        u[0] =(3.0 / x1_minus_x0) * ( (y_vals[1]-y_vals[0]) / x1_minus_x0 - self.low_slope)
-        y2_vals[0] = -0.5
-    else:
-        u[0] = 0.0
-        y2_vals[0] = 0.0   # natural spline
-    for i in range(1, n-1):
-        denom = x_vals[i+1] - x_vals[i-1] + 1e-12
-        sig = (x_vals[i]-x_vals[i-1]) / denom
-        p = sig*y2_vals[i-1]+2.0
-        y2_vals[i] = (sig-1.0)/p
-        if x_vals[i+1] == x_vals[i]:
-            x_vals[i+1] += 1e-12
-        u[i] = (y_vals[i+1]-y_vals[i]) / (x_vals[i+1]-x_vals[i]) - (y_vals[i]-y_vals[i-1]) / (x_vals[i]-x_vals[i-1])
-        u[i] = (6.0 * u[i] / denom - sig * u[i-1]) / p
-    if self.use_high_slope == 1:
-        qn = 0.5
-        un = (3.0/(x_vals[n-1]-x_vals[n-2])) * (self.high_slope - (y_vals[n-1]-y_vals[n-2]) / (x_vals[n-1]-x_vals[n-2]))
-    else:
-        qn = 0.0
-        un = 0.0    # natural spline
-    y2_vals[n-1] = (un-qn*u[n-2])/(qn*y2_vals[n-1]+1.0)
-    for k in range(n-2, -1, -1):
-        y2_vals[k] = y2_vals[k]*y2_vals[k+1]+u[k]
-    free(u)
-    self.ys2 = y2_vals
-
-
-@cython.boundscheck(False)
-@cython.cdivision(True)
-cdef inline double SplineS_at(SplineS *self, double x) nogil:
-    # if out of range, return endpoint
-    cdef double a, b, out
-    if x <= self.xs[0]:
-        return self.ys[0]
-    if x >= self.xs[self.last_index]:
-        return self.ys[self.last_index]
-    cdef int pos = _csearchsorted(self.xs, self.length, x)
-    cdef double h = self.xs[pos] - self.xs[pos-1]
-    if h == 0.0:
-        out = INFINITY
-    else:
-        a = (self.xs[pos] - x) / h
-        b = (x - self.xs[pos-1]) / h
-        out = (a* self.ys[pos-1] + b*self.ys[pos] + \
-              ((a*a*a - a)*self.ys2[pos-1] + \
-              (b*b*b - b)*self.ys2[pos]) * h*h/6.0)
-    return out
-
-
-cdef class Sampled(BpfInterface):
-    """
-    A bpf with regularly sampled data
-
-    When evaluated, values between the samples are interpolated with
-    a given function: linear, expon(x), halfcos, halfcos(x), etc.
-
-    """
-    cdef readonly ndarray ys
-    cdef double y0, y1
-    cdef double grid_dx, grid_x0, grid_x1
-    cdef int samples_size
-    cdef int nointerpol
-    cdef InterpolFunc* interpolfunc
-    cdef DTYPE_t* data
-    cdef ndarray _cached_xs
-
-    def __init__(self, samples, double dx, double x0=0, str interpolation='linear'):
-        """
-        Args:
-            samples (ndarray): the y-coord sampled data
-            dx (float): the sampling **period**
-            x0 (float): the first x-value
-            interpolation (str): the interpolation function used. One of 'linear',
-                'nointerpol', 'expon(X)', 'halfcos', 'halfcos(X)', 'smooth',
-                'halfcosm', etc.
-        """
-        self.ys = numpy.ascontiguousarray(samples, dtype=DTYPE)
-        self.data = <DTYPE_t *>self.ys.data
-        l = PyArray_DIM(self.ys, 0)
-        self.samples_size = l
-        self.grid_x0 = x0
-        self.grid_dx = dx
-        self.grid_x1 = x0 + dx * (l - 1)
-        self._set_bounds(x0, self.grid_x1)
-        self._cached_xs = None
-        if interpolation == 'nointerpol':
-            self.nointerpol = 1
-            self.interpolfunc = NULL
-        elif interpolation == 'linear':
-            self.nointerpol = 0
-            self.interpolfunc = InterpolFunc_linear
-        else:
-            self.nointerpol = 0
-            self.interpolfunc = InterpolFunc_new_from_descriptor(interpolation)
-            if self.interpolfunc is NULL:
-                raise ValueError("interpolation type not understood")
-        self.y0 = self.data[0]
-        self.y1 = self.data[l - 1]
-
-    @cython.cdivision(True)
-    @property
-    def samplerate(self) -> float: 
-        """
-        The samplerate of this bpf
-        """
-        return 1.0 / self.grid_dx
-
-    @property
-    def xs(self) -> numpy.ndarray:
-        """
-        The x-coord array of this bpf
-        """
-        if self._cached_xs is not None:
-            return self._cached_xs
-        self._cached_xs = numpy.linspace(self.grid_x0, self.grid_x1, self.samples_size)
-        return self._cached_xs
-
-    def points(self):
-        """
-        Returns a tuple with the points defining this bpf
-
-        Returns:
-            (tuple[ndarray, ndarray]) A tuple `(xs, ys)` where `xs` is an array
-            holding the values for the *x* coordinate, and `ys` holds the values for
-            the *y* coordinate
-
-        ## Example
-        
-        ```python
-
-        >>> b = Linear.fromseq(0, 0, 1, 100, 2, 50)
-        >>> b.points()
-        ([0, 1, 2], [0, 100, 50])
-        ```
-
-        """
-        return self.xs, self.ys
-    
-    property interpolation:
-        def __get__(self):
-            """
-            The interpolation kind of this bpf
-            """
-            if self.interpolfunc is not NULL:
-                return InterpolFunc_get_descriptor(self.interpolfunc)
-            return 'nointerpol'
-        def __set__(self, interpolation):
-            self.set_interpolation(interpolation)
-
-    @property
-    def dx(self) -> float: 
-        """
-        The sampling period (delta x)
-        """
-        return self.grid_dx
-
-    cpdef Sampled set_interpolation(self, str interpolation):
-        """
-        Sets the interpolation of this Sampled bpf, inplace
-
-        Args:
-            interpolation (str): the interpolation kind
-
-        Returns:
-            (Sampled) self
-
-        Returns *self*, so you can do:
-
-        ```python
-
-        sampled = bpf[x0:x1:dx].set_interpolation('expon(2)')
-        
-        ```
-        """
-        InterpolFunc_free(self.interpolfunc)
-        if interpolation == 'nointerpol':
-            self.nointerpol = 1
-            self.interpolfunc = NULL
-        else:
-            self.nointerpol = 0
-            self.interpolfunc = InterpolFunc_new_from_descriptor(interpolation)
-        return self
-
-    def __dealloc__(self):
-        InterpolFunc_free(self.interpolfunc)
-
-    def __getstate__(self):
-        return (self.ys, self.grid_dx, self.grid_x0, self.interpolation)
-
-    @cython.cdivision(True)
-    cdef double __ccall__(self, double x) nogil:
-        cdef int index0
-        cdef double y0, y1, x0
-        cdef double out
-        if x <= self.grid_x0:
-            out = self.y0
-        elif x >= self.grid_x1:
-            out = self.y1
-        else:
-            index0 = int((x - self.grid_x0) / self.grid_dx)
-            if self.nointerpol == 1:
-                out = self.data[index0]
-            else:
-                y0 = self.data[index0]
-                y1 = self.data[index0 + 1]
-                x0 = self.grid_x0 + index0 * self.grid_dx
-                out = InterpolFunc_call(self.interpolfunc, x, x0, y0, x0+self.grid_dx, y1)
-        return out
-
-    @cython.cdivision(True)
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        """
-        Return an array of `n` elements resulting of evaluating this bpf regularly
-
-        The x coordinates at which this bpf is evaluated are equivalent to `linspace(xstart, xend, n)`
-
-        Args:
-            n (int): the number of elements to generate
-            x0 (float): x to start mapping
-            x1 (float): x to end mapping
-            out (ndarray): if given, result is put here
-
-        Returns:
-            (ndarray) An array of this bpf evaluated at a grid [xstart:xend:dx], where *dx*
-            is `(xend-xstart)/n`
-        """
-        
-        cdef DTYPE_t *data
-        cdef DTYPE_t *selfdata
-        cdef int i, j, index0, nointerpol
-        cdef double x, y
-        cdef double grid_x0, grid_x1, self_y0, self_y1, grid_dx, interp_x0, interp_y0, interp_y1
-        cdef double dx = (x1 - x0) / (n - 1) # we account for the edge (x1 IS INCLUDED)
-        cdef double interpolfunc_exp
-        cdef t_func interpolfunc
-        if out is None:
-            out = EMPTY1D(n)
-            data = <DTYPE_t *>out.data
-        elif PyArray_ISCONTIGUOUS(out):
-            data = <DTYPE_t *>out.data
-        else:
-            for i in range(n):
-                out[i] = self.__ccall__(x0 + dx*i)
-            return out
-        grid_x0 = self.grid_x0
-        grid_x1 = self.grid_x1
-        self_y0 = self.y0
-        self_y1 = self.y1
-        grid_dx = self.grid_dx
-        selfdata = self.data
-        nointerpol = self.nointerpol
-        interpolfunc = self.interpolfunc.func
-        interpolfunc_exp = self.interpolfunc.exp
-        cdef size_t datasize = self.samples_size
-        i = 0
-        with nogil:
-            while i < n:
-                x = x0 + dx * i
-                if x > grid_x0:
-                    break
-                data[i] = self_y0
-                i += 1
-            while i < n:
-                x = x0 + dx * i
-                if x >= grid_x1:
-                    break
-                index0 = int((x - grid_x0) / grid_dx)
-                if nointerpol == 1:
-                    y = selfdata[index0]
-                else:
-                    interp_x0 = grid_x0 + index0 * grid_dx
-                    y = InterpolFunc_call(self.interpolfunc, x, interp_x0, selfdata[index0],
-                                          interp_x0 + grid_dx, selfdata[index0+1])
-                data[i] = y
-                i += 1
-            for j in range(i, n):
-                data[j] = self_y1
-        return out
-
-    @classmethod
-    def fromseq(cls, *args, **kws): raise NotImplementedError
-    
-    def _get_points_for_rendering(self, int n= -1): 
-        if self.interpolation == 'linear':
-            return self.xs, self.ys
-        else:
-            if n < 0:
-                n = NUM_XS_FOR_RENDERING
-            return numpy.linspace(self.x0, self.x1, n), self.mapn_between(n, self.x0, self.x1)
-    
-    def segments(self):
-        """
-        Returns an iterator over the segments of this bpf
-
-        Returns:
-            (Iterable[tuple[float, float, str, float]]) An iterator of segments, 
-            where each segment has the form `(x, y, interpoltype:str, exponent)`
-
-
-        Each item is a tuple `(float x, float y, str interpolation_type, float exponent)`
-
-        **NB**: exponent is only relevant if the interpolation type makes use of it
-        """
-        cdef int i
-        cdef double x0 = self.grid_x0
-        cdef double dx = self.grid_dx
-        descr = self.interpolation
-        exp = self.interpolfunc.exp if self.interpolfunc is not NULL else 0.0
-        for i in range(self.samples_size):
-            yield (x0 + i*dx, self.data[i], descr, exp)
-
-    cpdef double integrate(self):
-        """
-        Return the result of the integration of this bpf. 
-
-        If any of the bounds is `inf`, the result is also `inf`.
-
-        **NB**: to determine the limits of the integration, first crop the bpf via a slice
-        
-        ## Example
-        
-        Integrate this bpf from its lower bound to 10 (inclusive)
-        
-        ```python
-        b[:10].integrate()  
-        ```
-        """
-        return _integr_trapz(self.data, self.samples_size, self.grid_dx) 
-
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        """
-        The same as integrate() but between the (included) bounds x0-x1
-
-        It is effectively the same as `bpf[x0:x1].integrate()`, but more efficient
-        
-        **NB**: N has no effect. It is put here to comply with the signature of the function. 
-        """
-        dx = self.grid_dx
-        return _integr_trapz_between_exact(self.data, self.samples_size, dx, self.grid_x0, x0, x1)
-
-    cpdef BpfInterface derivative(self):
-        """
-        Return a curve which represents the derivative of this curve
-
-        It implements Newtons difference quotiont, so that:
-
-
-            derivative(x) = bpf(x + h) - bpf(x)
-                            -------------------
-                                      h
-        
-        Example
-        -------
-
-        ```python
-        
-        >>> from bpf4 import *
-        >>> a = slope(1)[0:6.28].sin()
-        >>> a.plot(show=False, color="red")
-        >>> b = a.derivative()
-        >>> b.plot(color="blue")
-
-        ```
-        ![](assets/derivative1.png)
-        """
-        return _BpfDeriv(self, self.grid_dx*0.99)
-
-    def inverted(self):
-        """
-        Return a view on this bpf with the coords inverted
-
-        Returns:
-            (BpfInterface) a view on this bpf with the coords inverted
-
-        In an inverted function the coordinates are swaped: the inverted version of a 
-        bpf indicates which *x* corresponds to a given *y*
-        
-        Returns None if the function is not invertible. For a function to be invertible, 
-        it must be strictly increasing or decreasing, with no local maxima or minima.
-        
-
-            f.inverted()(f(x)) = x
-        
-        
-        So if `y(1) == 2`, then `y.inverted()(2) == 1`
-
-        ![](assets/inverted.png)
-        """
-        
-        return Linear(self.xs, self.ys).inverted()
-
-    def flatpairs(self):
-        """
-        Returns a flat 1D array with x and y values interlaced
-
-        Returns:
-            (ndarray) A 1D array with x and y values interlaced
-
-        ```python
-        >>> a = linear(0, 0, 1, 10, 2, 20)
-        >>> a.flatpairs()
-        array([0, 0, 1, 10, 2, 20])
-        ```
-        """
-        return arraytools.interlace_arrays(self.xs, self.ys)
-
-    
-cdef class Spline(BpfInterface):
-    """
-    A bpf with cubic spline interpolation
-
-    With cubic spline interpolation, for each point `(x, y)` 
-    it is ensured that `bpf(x) == y`. Between the defined points,
-    depending on their proximity, this bpf can overshoot
-    
-    Example
-    -------
-
-    ```python
-    a = core.Smooth([0, 1, 3, 10], [0.1, 0.5, -3.5,  1])
-    b = core.Spline(*a.points())
-    fig, axes = plt.subplots(1, 2, figsize=(12, 4))
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1])
-    ```
-    ![](assets/Spline.png)
-
-    """
-    cdef SplineS* _spline
-
-    def __init__(self, xs, ys):
-        """
-        A bpf with cubic spline interpolation
-
-        Args:
-            xs (ndarray): the x coord data
-            ys (ndarray): the y coord data
-        """
-        
-        cdef ndarray [DTYPE_t, ndim=1] _xs = numpy.asarray(xs, dtype=DTYPE)
-        cdef ndarray [DTYPE_t, ndim=1] _ys = numpy.asarray(ys, dtype=DTYPE)
-        cdef int N = len(xs)
-        self._set_bounds(_xs[0], _xs[N - 1])
-        self._integration_mode = 1  # use quad
-        if _array_issorted(_xs) < 1:
-            raise ValueError(f"Points along the x coord should be sorted without duplicates. \n{xs}")
-        self._spline = SplineS_new(_xs, _ys, N)
-    
-    def __dealloc__(self):
-        SplineS_destroy(self._spline)
-    
-    @cython.boundscheck(False)
-    cdef double __ccall__(self, double x) nogil:
-        return SplineS_at(self._spline, x)
-    
-    cdef inline tuple _points(self):
-        cdef int i
-        xs = [self._spline.xs[i] for i in range(self._spline.length)]
-        ys = [self._spline.ys[i] for i in range(self._spline.length)]
-        return (xs, ys)
-    
-    def __getstate__(self):
-        return self._points()
-    
-    def points(self):
-        """
-        Returns a tuple with the points defining this bpf
-
-        Returns:
-            (tuple[ndarray, ndarray]) a tuple (xs, ys) where `xs` is an array
-            holding the values for the *x* coordinate, and `ys` holds the values for
-            the *y* coordinate
-
-        ## Example
-        
-        ```python
-
-        >>> b = Linear.fromseq(0, 0, 1, 100, 2, 50)
-        >>> b.points()
-        ([0, 1, 2], [0, 100, 50])
-        ```
-
-        """
-        return self._points()
-
-    def segments(self):
-        """
-        Returns an iterator over the segments of this bpf
-
-        Returns:
-            (Iterable[tuple[float, float, str, float]]) An iterator of segments, 
-            where each segment has the form `(x, y, interpoltype:str, exponent)`
-
-
-        Each segment is a tuple `(float x, float y, str interpolation_type, float exponent)`
-
-        !!! note
-        
-            Exponent is only relevant if the interpolation type makes use of it
-        
-        """
-        cdef size_t i
-        cdef size_t num_segments
-        exp = 0
-        num_segments = self._spline.length - 1
-        interpoltype = self.__class__.__name__.lower()
-        for i in range(num_segments):
-            yield (float(self._spline.xs[i]), float(self._spline.ys[i]), interpoltype, 0)
-        yield (float(self._spline.xs[num_segments]), float(self._spline.ys[num_segments]), '', 0)
-
-
-cdef class USpline(BpfInterface):
-    """
-    bpf with univariate spline interpolation. 
-
-    ```python
-    a = core.Spline([0, 1, 3, 10], [0.1, 0.5, -3.5,  1])
-    b = core.USpline(*a.points())
-
-    fig, axes = plt.subplots(1, 2, figsize=(12, 4), sharey=True, tight_layout=True)
-    a.plot(axes=axes[0], show=False)
-    b.plot(axes=axes[1])
-    ```
-    ![](assets/Uspline.png)
-    """
-    cdef object spline
-    cdef object spline__call__
-    cdef ndarray xs, ys
-    
-    def __init__(self, xs, ys):
-        """
-        Args:
-            xs (ndarray): the x coord data
-            ys (ndarray): the y coord data
-        """
-        
-        try:
-            from scipy.interpolate import UnivariateSpline
-        except ImportError:
-            raise ImportError("could not import scipy. USpline is a wrapper of UnivariateSpline"
-                              " and cant be used without scipy")
-        self.spline = UnivariateSpline(xs, ys)
-        self.spline__call__ = self.spline.__call__
-        self.xs = numpy.asarray(xs)
-        self.ys = numpy.asarray(ys)
-        self._set_bounds(xs[0], xs[len(xs) - 1])
-        self._integration_mode = 1  # use quad
-    
-    def __call__(self, x):
-        return self.spline(x)
-    
-    cdef double __ccall__(self, double x) nogil:
-        with gil:
-            return self.spline__call__(x)
-    
-    cpdef ndarray map(self, xs, ndarray out=None):
-        if out is not None:
-            out[...] = self.spline__call__(xs)
-            return out
-        else:
-            return self.spline__call__(xs)
-    
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        """
-        Return an array of `n` elements resulting of evaluating this bpf regularly
-
-        The x coordinates at which this bpf is evaluated are equivalent to `linspace(x0, x1, n)`
-
-        Args:
-            n (int): the number of elements to generate
-            x0 (float): x to start mapping
-            x1 (float): x to end mapping
-            out (ndarray): if given, result is put here
-
-        Returns:
-            (ndarray) An array of this bpf evaluated at a grid [xstart:xend:dx], where *dx*
-            is `(xend-xstart)/n`
-        """
-        
-        xs = numpy.linspace(x0, x1, n)
-        return self.map(xs, out)
-    
-    property _spline:
-        def __get__(self):
-            return self.spline
-    
-    def segments(self):
-        """
-        Returns an iterator over the segments of this bpf
-
-        Returns:
-            (Iterable[tuple[float, float, str, float]]) An iterator of segments, 
-            where each segment has the form `(x, y, interpoltype:str, exponent)`
-
-        """
-        cdef size_t i
-        cdef size_t num_segments
-        exp = 0
-        num_segments = len(self.xs) - 1
-        interpoltype = self.__class__.__name__.lower()
-        for i in range(num_segments):
-            yield (float(self.xs[i]), float(self.ys[i]), interpoltype, 0)
-        yield (float(self.xs[num_segments]), float(self.ys[num_segments]), '', 0)
-
-
-cdef class _BpfConcat2(BpfInterface):
-    cdef BpfInterface a
-    cdef BpfInterface b
-    cdef double splitpoint
-    cdef double __ccall__(self, double x) nogil:
-        if x < self.splitpoint:
-            return self.a.__ccall__(x)
-        return self.b.__ccall__(x)
-    
-    def __getstate__(self):
-        return self.a, self.b, self.splitpoint
-    
-    def __setstate__(self, state):
-        self.a, self.b, self.splitpoint = state
-        cdef double x0 = self.a._x0 if self.a._x0 < self.b._x0 else self.b._x0
-        cdef double x1 = self.b._x1 if self.b._x1 > self.a._x1 else self.a._x1
-        self._set_bounds(x0, x1)
-    
-
-cdef class Slope(BpfInterface):
-    """
-    A bpf representing a linear equation `y = slope * x + offset`
-
-    ```python
-
-    >>> from bpf4.core import *
-    >>> a = Slope(0.5, 1)
-    >>> a
-    Slope[-inf:inf]
-    >>> a[0:10].plot()
-    ```
-    ![](assets/slope-plot.png)
-    """
-    cdef public double slope
-    cdef public double offset
-    
-    def __init__(self, double slope, double offset=0, tuple bounds=None):
-        """
-        A bpf representing a linear equation `y = slope * x + offset`
-
-        Args:
-            slope (float): the slope of the line
-            offset (float): an offset added 
-            bounds (tuple): if given, the line is clipped on the x axis to the
-                given bounds
-        """
-        
-        self.slope = slope
-        self.offset = offset
-        if bounds is not None:
-            self._set_bounds(bounds[0], bounds[1])
-        else:
-            self._set_bounds(INFNEG, INF)
-        
-    cdef double __ccall__(self, double x) nogil:
-        return self.offset + x*self.slope
-
-    cpdef Slope _slice(self, double x0, double x1):
-        return Slope(self.slope, self.offset, bounds=(x0, x1))
-
-    def __add__(a, b):
-        if isnumber(a):
-            # we are b
-            return Slope(b.slope, b.offset + a, b.bounds())
-        elif isnumber(b):
-            return Slope(a.slope, a.offset + b, a.bounds())
-        else:
-            return _create_lambda(a, b, _BpfLambdaAdd, _BpfLambdaAddConst)
-
-    def __sub__(a, b):
-        if isnumber(a):
-            return b + (-a)
-        elif isnumber(b):
-            return a + (-b)
-        else:
-            return _create_rlambda(a, b, _BpfLambdaSub, _BpfLambdaSubConst, _BpfLambdaRSub, _BpfLambdaRSubConst)
-
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        """
-        Return an array of `n` elements resulting of evaluating this bpf regularly
-
-        The x coordinates at which this bpf is evaluated are equivalent to `linspace(x0, 1, n)`
-
-        Args:
-            n (int): the number of elements to generate
-            x0 (float): x to start mapping
-            x1 (float): x to end mapping
-            out (ndarray): if given, result is put here
-
-        Returns:
-            (ndarray) An array of this bpf evaluated at a grid [x0:x1:dx], where *dx*
-            is `(xend-xstart)/n`
-
-        """
-        cdef double[::1] result = out if out is not None else EMPTY1D(n)
-        cdef double offset = self.offset
-        cdef double slope = self.slope
-        cdef int i
-        cdef double x
-        cdef double dx = _ntodx(n, x0, x1)
-        cdef double slopex0 = slope * x0
-        cdef double slopedx = slope * dx
-        cdef double offset2 = offset + slopex0
-        with nogil:
-            for i in range(n):
-                # x = x0 + i * dx
-                # y = offset + (x0 + i*dx)*slope
-                # y = offset + slope*x0 + i*(dx*slope)
-                result[i] = offset2 + i * slopedx
-        return numpy.asarray(result)
-
-
-    def __mul__(a, b):
-        if isnumber(a):
-            return Slope(b.slope*a, b.offset*a, b.bounds())
-        elif isnumber(b):
-            return Slope(a.slope*b, a.offset*b, a.bounds())
-        return BpfInterface.__mul__(a, b)
-
-    def __getstate__(self):
-        return self.slope, self.offset, self.bounds()
-
-    
-cdef class _BpfCompose(BpfInterface):
-    """
-    A bpf representing function composition `f(x) = b(a(x))`
-    """
-    cdef BpfInterface a
-    cdef BpfInterface b
-
-    cdef double __ccall__(self, double x) nogil:
-        x = self.a.__ccall__(x)
-        return self.b.__ccall__(x)
-
-    def __getstate__(self):
-        return self.a, self.b
-
-    def __setstate__(self, state):
-        self.a, self.b = state
-        self._set_bounds(self.a._x0, self.a._x1)
-
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        """
-        Return an array of `n` elements resulting of evaluating this bpf regularly
-
-        The x coordinates at which this bpf is evaluated are equivalent to `linspace(x0, 1, n)`
-
-        Args:
-            n (int): the number of elements to generate
-            x0 (float): x to start mapping
-            x1 (float): x to end mapping
-            out (ndarray): if given, result is put here
-
-        Returns:
-            (ndarray) An array of this bpf evaluated at a grid [x0:x1:dx], where *dx*
-            is `(xend-xstart)/n`
-        """
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A
-        if out is not None:
-            self.a.mapn_between(n, x0, x1, out)
-            self.b.map(out, out)
-            return out
-        else:
-            A = self.a.mapn_between(n, x0, x1)
-            self.b.map(A, A)
-            return A
- 
-
-cdef _BpfCompose _BpfCompose_new(BpfInterface a, BpfInterface b):
-    cdef _BpfCompose self = _BpfCompose()
-    self.a = a
-    self.b = b
-    self._set_bounds(a._x0, a._x1)
-    return self
-
-
-cdef _BpfConcat2 _BpfConcat2_new(BpfInterface bpf_a, BpfInterface bpf_b, double splitpoint):
-    cdef _BpfConcat2 self = _BpfConcat2()
-    cdef double x0 = bpf_a._x0 if bpf_a._x0 < bpf_b._x0 else bpf_b._x0
-    cdef double x1 = bpf_b._x1 if bpf_b._x1 > bpf_a._x1 else bpf_a._x1
-    self._set_bounds(x0, x1)
-    self.a = bpf_a
-    self.b = bpf_b
-    self.splitpoint = splitpoint
-    return self
-
-
-cdef class _BpfConcat(BpfInterface):
-    """
-    A bpf representing the concatenation of multiple bpfs
-    """
-    cdef list bpfs
-    cdef double *xs
-    cdef Py_ssize_t size
-    cdef double last_x0, last_x1
-    cdef BpfInterface last_bpf, bpf0, bpf1
-
-    def __cinit__(self, xs, bpfs):
-        self.size = len(xs)
-        self.xs = <double *>malloc(sizeof(double) * self.size)
-
-    def __init__(self, xs, bpfs):
-        """
-        Args:
-            xs (list|ndarray):  the offset of each bpf
-            bpfs (list[BpfInterface]): a list of bpfs to concatenate
-        """
-        cdef int i
-        cdef BpfInterface bpf
-        self.bpfs = list(bpfs)
-        i = 0
-        for x in xs:
-            self.xs[i] = x
-            i += 1
-        cdef double x0 = INF
-        cdef double x1 = INFNEG
-        for i in range(self.size):
-            bpf = self.bpfs[i]
-            if bpf._x0 < x0:
-                x0 = bpf._x0
-            if bpf._x1 > x1:
-                x1 = bpf._x1
-        self._set_bounds(x0, x1)
-        self.bpf0 = self.bpfs[0]
-        self.bpf1 = self.bpfs[self.size - 1]
-        self.last_bpf = self.bpf0
-        self.last_x0 = self.xs[0]
-        self.last_x1 = self.xs[1]
-
-    def __dealloc__(self):
-        free(self.xs)
-
-    cdef double __ccall__(self, double x) nogil:
-        cdef int index
-        if x <= self._x0:
-            return self.bpf0.__ccall__(x)
-        elif x >= self._x1:
-            return self.bpf1.__ccall__(x)
-        elif x >= self.last_x0 and x < self.last_x1:
-            return self.last_bpf.__ccall__(x)
-        else:
-            index = _csearchsorted_left(self.xs, self.size, x) - 1
-            with gil:
-                self.last_bpf = self.bpfs[index]
-            self.last_x0 = self.xs[index]
-            self.last_x1 = self.xs[index+1]
-            return self.last_bpf.__ccall__(x)
-
-    cpdef BpfInterface concat(self, BpfInterface other, double fadetime=0, fadeshape='expon(3)'):
-        cdef BpfInterface other2 = other.fit_between(self._x1, self._x1 + (other._x1 - other._x0))
-        cdef int i
-        cdef list xs
-        cdef list bpfs
-        if fadetime == 0:
-            xs = [self.xs[i] for i in range(self.size)]
-            bpfs = self.bpfs[:]
-            bpfs.append(other2)
-            return _BpfConcat(xs, bpfs)
-        raise NotImplementedError("fade is not implemented")
-
-    def __getstate__(self):
-        cdef list xs
-        cdef int i
-        xs = [self.xs[i] for i in range(self.size)]
-        return xs, self.bpfs
-
-
-cdef class _BpfBlend(BpfInterface):
-    cdef BpfInterface a, b
-    cdef BpfInterface which
-
-    def __init__(self, a: BpfInterface, b: BpfInterface, which: BpfInterface):
-        """
-        Args:
-            a: the first bpf
-            b: the second bpf
-            which: a bpf returning a value between 0-1; indicates the mix factor
-                at any x-point
-        """
-        self.a = a
-        self.b = b
-        self.which = which
-        cdef double x0 = min(a.x0, b.x0)
-        cdef double x1 = max(a.x1, b.x1)
-        self._set_bounds(x0, x1)
-
-    cdef double __ccall__(self, double x) nogil:
-        cdef double ya, yb, mix
-        mix = self.which.__ccall__(x)
-        ya = self.a.__ccall__(x) * (1 - mix)
-        yb = self.b.__ccall__(x) * mix
-        return ya + yb
-
-    def __getstate__(self):
-        return self.a, self.b, self.which
-
-        
-cdef class _BpfBlendConst(BpfInterface):
-    cdef BpfInterface a, b
-    cdef double which
-
-    def __init__(_BpfBlendConst self, BpfInterface a, BpfInterface b, double which):
-        """
-        Args:
-            a (BpfInterface): the first bpf
-            b (BpfInterface): the second bpf
-            which (float): a constant mix factor between 0-1
-        """
-        self.a = a
-        self.b = b
-        self.which = which
-        cdef double x0 = min(a._x0, b._x0)
-        cdef double x1 = max(a._x1, b._x1)
-        self._set_bounds(x0, x1)
-
-    cdef double __ccall__(self, double x) nogil:
-        return self.a.__ccall__(x) * (1 - self.which) + self.b.__ccall__(x) * self.which
-
-    def __getstate__(self): return self.a, self.b, self.which
-
-        
-cdef class Multi(BpfInterface):
-    """
-    A bpf where each segment can have its own interpolation kind
-    """
-    cdef DTYPE_t* xs
-    cdef DTYPE_t* ys
-    cdef InterpolFunc** interpolations
-    cdef int size
-    cdef DTYPE_t y0, y1, last_x0, last_x1, last_y0, last_y1
-    cdef InterpolFunc* last_interpol
-
-    def __cinit__(self, xs, ys, interpolations):
-        self.size = len(xs)
-        self.interpolations = <InterpolFunc **>malloc(sizeof(InterpolFunc*) * (self.size - 1))
-
-    def __init__(self, xs, ys, interpolations):
-        """
-        Args:
-            xs (ndarray): the sequence of x points
-            ys (ndarray): the sequence of y points
-            interpolations (list[str]): the interpolation used between these points
-
-        !!! note
-
-            ```python
-            
-            len(interpolations) == len(xs) - 1
-
-            ```
-
-        The interpelation is indicated via a descriptor: `'linear'` (linear), `'expon(x)'` 
-        (exponential with exp=x), `'halfcos'`, `'halfcos(x)'` (cosine interpol with exp=x),
-        `'nointerpol'`, ``'smooth'` (smoothstep)
-        """
-        cdef int i
-        cdef list interpolations_list
-        self.xs = _seq_to_doubles(xs)
-        self.ys = _seq_to_doubles(ys)
-        assert len(interpolations) == self.size - 1
-        i = 0
-        for interpolation in interpolations:
-            self.interpolations[i] = InterpolFunc_new_from_descriptor(interpolation)
-            i += 1
-        self._set_bounds(self.xs[0], self.xs[self.size - 1])
-        self.y0 = self.ys[0]
-        self.y1 = self.ys[self.size - 1]
-        self.last_x0 = self.xs[0]
-        self.last_x1 = self.xs[1]
-        self.last_y0 = self.ys[0]
-        self.last_y1 = self.ys[1]
-        self.last_interpol = self.interpolations[0]
-
-    def __dealloc__(self):
-        free(self.xs)
-        free(self.ys)
-        cdef int i
-        for i in range(self.size - 1):
-            InterpolFunc_free(self.interpolations[i])
-        free(self.interpolations)
-
-    def __getstate__(self):
-        cdef int i
-        xs = [self.xs[i] for i in range(self.size)]
-        ys = [self.ys[i] for i in range(self.size)]
-        interpolations = [InterpolFunc_get_descriptor(self.interpolations[i]) for i in range(self.size - 1)]
-        return xs, ys, interpolations
-
-    cdef double __ccall__(self, double x) nogil:
-        cdef double res, x0, x1, y0, y1
-        cdef int index1, index0
-        if x <= self._x0:
-            res = self.y0
-        elif x >= self._x1:
-            res = self.y1
-        else:
-            if self.last_x0 <= x < self.last_x1:
-                # res = self.last_interpol.func(x, self.last_x0, self.last_y0, self.last_x1, self.last_y1, self.last_interpol.exp)
-                res = InterpolFunc_call(self.last_interpol, x, self.last_x0, self.last_y0, self.last_x1, self.last_y1)
-            else:
-                index1 = _csearchsorted(self.xs, self.size, x)
-                index0 = index1 - 1
-                self.last_x0 = x0 = self.xs[index0]
-                self.last_x1 = x1 = self.xs[index1]
-                self.last_y0 = y0 = self.ys[index0]
-                self.last_y1 = y1 = self.ys[index1]
-                self.last_interpol = self.interpolations[index0]
-                # res = self.last_interpol.func(x, x0, y0, x1, y1, self.last_interpol.exp)
-                res = InterpolFunc_call(self.last_interpol, x, x0, y0, x1, y1)
-        return res
-
-    def segments(self):
-        """
-        Returns an iterator over the segments of this bpf
-
-        Returns:
-            (Iterator[tuple[float, float, str, float]]) An iterator of segments, 
-            where each segment has the form `(x, y, interpoltype:str, exponent)`
-
-        """
-        cdef int i
-        cdef InterpolFunc* func
-        for i in range(self.size - 1):
-            func = self.interpolations[i]
-            yield self.xs[i], self.ys[i], func.name, func.exp
-        yield (self.xs[self.size-1], self.ys[self.size-1], '', 0)
-
-
-ctypedef double(*dfunc)(double) nogil
-
-
-def _FunctionWrap(f, bounds=(INFNEG, INF)):
-    return _FunctionWrap_Object(f, bounds)
-
-
-cdef class _FunctionWrap_Object(BpfInterface):
-    cdef object f
-
-    def __init__(self, f, bounds=(INFNEG, INF)):
-        """
-        Args:
-            f (callable): a function to wrap as a bpf
-            bounds (tuple[float, float]): the bounds of this bpf
-        """
-        self._set_bounds(bounds[0], bounds[1])
-        self.f = f.__call__
-
-    cdef double __ccall__(self, double x) nogil:
-        with gil:
-            return self.f(x)
-
-    def __getstate__(self):
-        return (self.f, (self._x0, self._x1))
-
-    cpdef BpfInterface _slice(self, double x0, double x1):
-        return _FunctionWrap_Object_OutboundConst_new(self, x0, x1)
-
-    cpdef ndarray map(self, xs, ndarray out=None):
-        """
-        the same as map(self, xs) but somewhat faster
-
-        xs can also be a number, in which case it is interpreted as
-        the number of elements to calculate in an evenly spaced
-        grid between the bounds of this bpf.
-        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
-
-        if out is given, the result if put into it. it must have the 
-        same shape as xs
-        """
-        cdef ndarray [DTYPE_t, ndim=1] _xs
-        cdef ndarray [DTYPE_t, ndim=1] result
-        cdef DTYPE_t *data1
-        cdef DTYPE_t *data0
-        cdef list xs_as_list
-        cdef tuple xs_as_tuple
-        cdef int i, nx
-        cdef double x0,x1, dx
-        cdef object f = self.f
-        if isinstance(xs, (int, long)):
-            return self.mapn_between(xs, self._x0, self._x1, out)
-        else:
-            if out is None:
-                nx = len(xs)
-                result = EMPTY1D(nx)
-            else:
-                result = <ndarray>out
-                nx = PyArray_DIM(<ndarray>result, 0)
-            if isinstance(xs, ndarray):
-                if PyArray_ISCONTIGUOUS(<ndarray>xs):
-                    data1 = <DTYPE_t *>((<ndarray>xs).data)
-                    if PyArray_ISCONTIGUOUS(result):
-                        data0 = <DTYPE_t *>result.data
-                        for i in range(nx):
-                            data0[i] = f(data1[i])
-                    else:
-                        nx = PyArray_DIM(<ndarray>xs, 0)
-                        for i in range(nx):
-                            result[i] = f(data1[i])
-                else:
-                    _xs = <ndarray>xs
-                    for i in range(PyArray_DIM(xs, 0)):
-                        result[i] = f(_xs[i])
-            else:
-                if isinstance(xs, list):
-                    for i in range(nx):
-                        result[i] = f((<list>xs)[i])
-                elif isinstance(xs, tuple):
-                    xs_as_tuple = xs
-                    for i in range(len(xs_as_tuple)):
-                        result[i] = f(xs_as_tuple[i])
-                else:
-                    for i in range(nx):
-                        result[i] = f(xs[i])
-        return result
-        
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        xs = numpy.linspace(x0, x1, n)
-        return self.map(xs, out=out)
-
-
-cdef class _FunctionWrap_Object_OutboundConst(_FunctionWrap_Object):
-    cdef double y0, y1
-    cdef double __ccall__(self, double x) nogil:
-        if x < self._x0:
-            return self.y0
-        elif x > self._x1:
-            return self.y1
-        else:
-            with gil:
-                return self.f(x)
-
-
-cdef _FunctionWrap_Object_OutboundConst _FunctionWrap_Object_OutboundConst_new(_FunctionWrap_Object bpf, double x0, double x1):
-    cdef _FunctionWrap_Object_OutboundConst out = _FunctionWrap_Object_OutboundConst(bpf.f, (x0, x1))
-    out.y0 = out.f(x0)
-    out.y1 = out.f(x1)
-    return out
-
-
-cdef class Const(BpfInterface):
-    """
-    A bpf representing a constant value
-    """
-
-    cdef double value
-    
-    def __init__(self, double value, bounds: tuple[float, float]=None):
-        """
-        Args:
-            value (float): the constant value of this bpf
-        """
-        if bounds:
-            self._set_bounds(bounds[0], bounds[1])
-        else:
-            self._set_bounds(INFNEG, INF)
-        self.value = value
-    
-    def __call__(self, x): return self.value
-    
-    cdef double __ccall__(self, double x) nogil:
-        return self.value
-    
-    def __getstate__(self):
-        return (self.value,)
-    
-    def _get_points_for_rendering(self, int n):
-        x0 = self._x0 if self._x0 > INFNEG else 0.
-        x1 = self._x1 if self._x1 < INF else 1.
-        return numpy.array([x0, x1]), numpy.array([self.value, self.value])
-    
-    def __getitem__(self, slice):
-        if not hasattr(slice, 'start'):
-            raise ValueError("BPFs accept only slices, not single items.")    
-        cdef double x0 = slice.start if slice.start is not None else self._x0
-        cdef double x1 = slice.stop if slice.stop is not None else self._x1
-        cdef BpfInterface out = Const(self.value)
-        out._set_bounds(x0, x1)
-        return out
-            
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        if out is not None:
-            out[...] = self.value
-            return out
-        cdef double[::1] out2 = EMPTY1D(n)
-        cdef int i
-        for i in range(n):
-            out2[i] = self.value
-        return numpy.asarray(out2)
-        
-cdef _create_lambda_unordered(a, b, class_bin, class_const):
-    if isinstance(a, BpfInterface):        
-        if isinstance(b, BpfInterface):
-            out = class_bin(a, b, _get_bounds(a, b))
-        elif callable(b):
-            out = class_bin(a, _FunctionWrap(b), a.bounds())
-        else:
-            out = class_const(a, b, a.bounds())
-        return out
-    elif isinstance(b, BpfInterface):
-        if callable(a):
-            out = class_bin(b, _FunctionWrap(a), a.bounds())
-        else:
-            out = class_const(b, a, b.bounds())
-        return out
-
-cdef _create_lambda(BpfInterface a, object b, class_bin, class_const):
-    if isinstance(b, BpfInterface):
-        out = class_bin(a, b, _get_bounds(a, b))
-    elif callable(b):
-        out = class_bin(a, _FunctionWrap(b), a.bounds())
-    else:
-        out = class_const(a, b, a.bounds())
-    return out
-
-cdef _create_rlambda(object a, object b, class_bin, class_const, class_rbin=None, class_rconst=None):
-    if isinstance(a, BpfInterface):
-        if isinstance(b, BpfInterface):
-            out = class_bin(a, b, _get_bounds(a, b))
-        elif callable(b):
-            out = class_bin(a, _FunctionWrap(b), a.bounds())
-        else:
-            out = class_const(a, b, a.bounds())
-        return out
-    else:
-        if callable(a):
-            out = class_rbin(_FunctionWrap(a), b, b.bounds())
-        else:
-            out = class_rconst(b, a, b.bounds())
-    return out
-
-cdef class _BpfBinOp(BpfInterface):
-    """
-    A bpf representing a binary operation between two bpfs
-    """
-    cdef BpfInterface a, b
-
-    def __init__(self, BpfInterface a, BpfInterface b, tuple bounds):
-        self.a = a
-        self.b = b
-        self._x0, self._x1 = bounds
-    
-    def __getstate__(self):
-        return self.a, self.b, (self._x0, self._x1)
-    
-    def _get_xs_for_rendering(self, int n):
-        return numpy.unique(numpy.append(self.a._get_xs_for_rendering(n), self.b._get_xs_for_rendering(n)))
-
-    cdef double __ccall__(self, double x) nogil:
-        cdef double A = self.a.__ccall__(x)
-        cdef double B = self.b.__ccall__(x)
-        self._apply(&A, &B, 1)
-        return A
-
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        # the result should be put in A
-        pass
-    
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = <ndarray>out if out is not None else EMPTY1D(n)
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] B = EMPTY1D(n)
-        self.a.mapn_between(n, x0, x1, A)
-        self.b.mapn_between(n, x0, x1, B)
-        #cdef c_numpy.ndarray[DTYPE_t, ndim=1] ys_a = self.a.mapn_between(n, x0, x1, out)
-        #cdef c_numpy.ndarray[DTYPE_t, ndim=1] ys_b = self.b.mapn_between(n, x0, x1)
-        with nogil:
-            self._apply(<DTYPE_t*>A.data, <DTYPE_t*>B.data, n)
-            # self._apply(&A[0], &B[0], n)
-        return A
-        
-    cpdef ndarray map(self, xs, ndarray out=None):
-        """
-        the same as map(self, xs) but somewhat faster
-
-        xs can also be a number, in which case it is interpreted as
-        the number of elements to calculate in an evenly spaced
-        grid between the bounds of this bpf.
-        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
-        ( this is the same as bpf.mapn_between(10, bpf.x0, bpf.x1) )
-        """
-        cdef int len_xs
-        if isinstance(xs, (int, long)):
-            return self.mapn_between(xs, self._x0, self._x1, out)
-        len_xs = len(xs)
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = out if out is not None else EMPTY1D(len_xs)
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] B = EMPTY1D(len_xs)
-        self.a.map(xs, A)
-        self.b.map(xs, B)
-        with nogil:
-            self._apply(<DTYPE_t *>(A.data), <DTYPE_t *>(B.data), len_xs)
-        return numpy.asarray(A)
-
-
-cdef class _BpfUnaryFunc(BpfInterface):
-    cdef BpfInterface a
-    cdef t_unfunc func
-    cdef int funcindex
-    
-    def __reduce__(self):
-        return type(self), (), self.a, self.funcindex 
-    
-    def __setstate__(self, state):
-        bpf, funcindex = state
-        return _BpfUnaryFunc_new_from_index(bpf, funcindex)
-    
-    cdef void _apply(self, DTYPE_t *A, int n) nogil:
-        cdef t_unfunc func = self.func
-        for i in range(n):
-            A[i] = func(A[i])
-    
-    cdef double __ccall__(self, double x) nogil:
-        return self.func(self.a.__ccall__(x))
-    
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = self.a.mapn_between(n, x0, x1, out)
-        cdef t_unfunc func = self.func
-        with nogil:
-            self._apply(<DTYPE_t *>(A.data), n)
-        return A
-    
-    cpdef ndarray map(self, xs, ndarray out=None):
-        """
-        the same as map(self, xs) but somewhat faster
-
-        xs can also be a number, in which case it is interpreted as
-        the number of elements to calculate in an evenly spaced
-        grid between the bounds of this bpf.
-        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
-        ( this is the same as bpf.mapn_between(10, bpf.x0, bpf.x1) )
-        """
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A
-        if isinstance(xs, (int, long)):
-            return self.mapn_between(xs, self._x0, self._x1, out)
-        A = self.a.map(xs, out)
-        self._apply(<DTYPE_t *>(A.data), len(xs))
-        return A
-     
-
-cdef _BpfUnaryFunc _BpfUnaryFunc_new(BpfInterface a, t_unfunc func, int funcindex):
-    cdef _BpfUnaryFunc self = _BpfUnaryFunc()
-    self.a = a
-    self.func = func
-    self.funcindex = funcindex
-    cdef double x0, x1
-    x0, x1 = a.bounds()
-    self._set_bounds(x0, x1)
-    return self
-    
-
-cdef _BpfUnaryFunc _BpfUnaryFunc_new_from_index (BpfInterface a, int funcindex):
-    cdef t_unfunc func = _unfunc_from_index(funcindex)
-    return _BpfUnaryFunc_new(a, func, funcindex)
-    
-
-cdef t_unfunc _unfunc_from_index(int funcindex):
-    return UNFUNCS [funcindex]
-
-
-cdef class _BpfUnaryOp(BpfInterface):
-    """
-    A bpf representing a unary operation on a bpf
-    """
-    cdef BpfInterface a
-
-    def __init__(self, BpfInterface a):
-        self.a = a
-        cdef double x0, x1
-        x0, x1 = a.bounds()
-        self._set_bounds(x0, x1)
-    
-    cdef double __ccall__(self, double x) nogil:
-        cdef double X = self.a.__ccall__(x)
-        self._apply(&X, 1)
-        return X
-    
-    def __getstate__(self):
-        return (self.a,)
-    
-    def _get_xs_for_rendering(self, int n):
-        return self.a._get_xs_for_rendering(n)
-    
-    cdef void _apply(self, DTYPE_t *A, int n) nogil:
-        pass
-    
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = self.a.mapn_between(n, x0, x1, out)
-        with nogil:
-            self._apply(<DTYPE_t *>(A.data), n)
-        return A
-    
-    cpdef ndarray map(self, xs, ndarray out=None):
-        """
-        the same as map(self, xs) but somewhat faster
-
-        xs can also be a number, in which case it is interpreted as
-        the number of elements to calculate in an evenly spaced
-        grid between the bounds of this bpf.
-        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
-        ( this is the same as bpf.mapn_between(10, bpf.x0, bpf.x1) )
-        """
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A
-        if isinstance(xs, (int, long)):
-            return self.mapn_between(xs, self._x0, self._x1, out)
-        A = self.a.map(xs, out)
-        self._apply(<DTYPE_t *>(A.data), len(xs))
-        return A
-
-
-cdef class _BpfBinOpConst(BpfInterface):
-    """
-    A bpf representing a binary operation between a bpf and a constant value
-    """
-    cdef double b_const
-    cdef BpfInterface a
-    
-    def __init__(_BpfBinOpConst self, BpfInterface a, double b, tuple bounds, str op=''):
-        self.a = a
-        self.b_const = b
-        self._x0, self._x1 = bounds
-    
-    def __getstate__(self):
-        return self.a, self.b_const, (self._x0, self._x1)
-    
-    def _get_xs_for_rendering(self, int n):
-        return self.a._get_xs_for_rendering(n)
-    
-    cdef void _apply(self, DTYPE_t *A, int n, double x) nogil:
-        pass
-    
-    cpdef ndarray map(self, xs, ndarray out=None):
-        """
-        the same as map(self, xs) but somewhat faster
-
-        Args:
-            xs (ndarray | int): the points to evaluate this bpf at, or an
-                int indicating the number of points to sample this bpf
-                at within its bounds
-            out (ndarray): if given, the results of the evaluation
-                are placed here. It must be the same size as `xs`
-
-        Returns:
-            (ndarray) The resulting array
-
-        **NB**: `xs`` can be a number, in which case it is interpreted as
-        the number of elements to calculate in an evenly spaced
-        grid between the bounds of this bpf.
-        
-        `bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))`
-
-        This is the same as `bpf.mapn_between(10, bpf.x0, bpf.x1)`
-        """
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A
-        cdef int len_xs
-        if isinstance(xs, (int, long)):
-            return self.mapn_between(xs, self._x0, self._x1, out)
-        A = self.a.map(xs, out)
-        len_xs = len(xs)
-        with nogil:
-            self._apply(<DTYPE_t *>(A.data), len_xs, self.b_const)
-        return A
-    
-    cdef double __ccall__(self, double x) nogil:
-        cdef double A = self.a.__ccall__(x)
-        self._apply(&A, 1, self.b_const)
-        return A
-
-
-cdef class _BpfLambdaAdd(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] += B[i]
-
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        return self.a.integrate_between(x0, x1, N) + self.b.integrate_between(x0, x1, N)
-
-    
-cdef class _BpfLambdaAddConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] += b
-
-    def __add__(a, b):
-        cdef double c
-        if isinstance(a, BpfInterface):
-            try:
-                c = float(b)
-                return _BpfLambdaAddConst(a.a, a.b + c)
-            except:
-                return _BpfBinOpConst.__add__(a, b)
-        else:
-            try:
-                c = float(a)
-                return _BpfLambdaAddConst(b.a, b.b + a)
-            except:
-                return _BpfBinOpConst.__add__(b, a)
-
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        return self.a.integrate_between(x0, x1, N) + (x1 - x0) * self.b_const
-
-
-cdef class _BpfLambdaSub(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] -= B[i]
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        return self.a.integrate_between(x0, x1, N) - self.b.integrate_between(x0, x1, N) 
-
-
-cdef class _BpfLambdaRSub(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            B[i] -= A[i]
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        return self.b.integrate_between(x0, x1, N) - self.a.integrate_between(x0, x1, N)
-
-
-cdef class _BpfLambdaSubConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] -= b
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        return self.a.integrate_between(x0, x1, N) - (x1-x0)*self.b_const
-
-
-cdef class _BpfLambdaRSubConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = b - A[i]
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        return self.b_const*(x1-x0) - self.a.integrate_between(x0, x1, N)
-
-
-cdef class _BpfLambdaMul(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] *= B[i]
-
-            
-cdef class _BpfLambdaMulConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] *= b
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        return self.a.integrate_between(x0, x1, N) * self.b_const
-
-
-cdef class _BpfLambdaPow(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = A[i] ** B[i]
-
-
-cdef class _BpfLambdaPowConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = A[i] ** b
-
-
-cdef class _BpfLambdaRPowConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = b ** A[i]
-
-
-cdef class _BpfLambdaDiv(_BpfBinOp):
-    @cython.cdivision(True)
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] /= B[i]
-
-
-cdef class _BpfLambdaDivConst(_BpfBinOpConst):
-    @cython.cdivision(True)
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] /= b
-
-
-cdef class _BpfLambdaMod(_BpfBinOp):
-    @cython.cdivision(True)
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = fmod(A[i], B[i])
-
-
-cdef class _BpfLambdaModConst(_BpfBinOpConst):
-    @cython.cdivision(True)
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = fmod(A[i], b)
-
-
-cdef class _BpfLambdaRDiv(_BpfBinOp):
-    @cython.cdivision(True)
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = B[i] / A[i]
-
-
-cdef class _BpfLambdaRDivConst(_BpfBinOpConst):
-    @cython.cdivision(True)
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = b / A[i]
-
-
-cdef class _BpfLambdaGreaterThan(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = A[i] > B[i]
-
-    
-cdef class _BpfLambdaGreaterOrEqualThan(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = A[i] >= B[i]
-
-
-cdef class _BpfLambdaGreaterThanConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = A[i] > b
-
-
-cdef class _BpfLambdaGreaterOrEqualThanConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = A[i] >= b
-
-
-cdef class _BpfLambdaLowerThan(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = A[i] < B[i]
-
-
-cdef class _BpfLambdaLowerThanConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = A[i] < b
-
-
-cdef class _BpfLambdaLowerOrEqualThan(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = A[i] <= B[i]
-
-
-cdef class _BpfLambdaLowerOrEqualThanConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = A[i] <= b
-
-
-cdef class _BpfLambdaEqual(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = A[i] == B[i]
-
-
-cdef class _BpfLambdaEqualConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = A[i] == b
-
-
-cdef class _BpfLambdaUnequal(_BpfBinOp):
-    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
-        for i in range(n):
-            A[i] = A[i] != B[i]
-
-
-cdef class _BpfLambdaUnequalConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = A[i] != b
-
-            
-cdef class _BpfMaxConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        cdef double y
-        for i in range(n):
-            y = A[i]
-            A[i] = y if y > b else b
-
-        
-cdef class _BpfMinConst(_BpfBinOpConst):
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        cdef double y
-        for i in range(n):
-            y = A[i]
-            A[i] = y if y < b else b
-
-
-cdef class _BpfLambdaLog(_BpfBinOpConst):
-    def __init__(_BpfBinOpConst self, BpfInterface a, double b, tuple bounds, str op=''):
-        _BpfBinOpConst.__init__(self, a, b, bounds, op)
-        self.b_const = m_log(b)
-    
-    @cython.cdivision(True)
-    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
-        for i in range(n):
-            A[i] = m_log(A[i]) / b
-
-
-cdef class _BpfLambdaRound(_BpfUnaryOp):
-    cdef void _apply(self, DTYPE_t *A, int n) nogil:
-        for i in range(n):
-            A[i] = floor(A[i] + 0.5)
-
-
-cdef class _BpfRand(_BpfUnaryOp):
-    @cython.cdivision(True)
-    cdef void _apply(self, DTYPE_t *A, int n) nogil:
-        for i in range(n):
-            A[i] = (rand()/<double>RAND_MAX) * A[i]
-
-
-cdef class _BpfM2F(_BpfUnaryOp):
-    cdef void _apply(self, DTYPE_t *A, int n) nogil:
-        for i in range(n):
-            A[i] = m2f(A[i])
-
-
-cdef class _BpfF2M(_BpfUnaryOp):
-    cdef void _apply(self, DTYPE_t *A, int n) nogil:
-        for i in range(n):
-            A[i] = f2m(A[i])
-
-
-cdef class _Bpf_db2amp(_BpfUnaryOp):
-    cdef void _apply(self, DTYPE_t *A, int n) nogil:
-        for i in range(n):
-            A[i] = 10.0 ** (0.05*A[i])
-
-
-cdef class _Bpf_amp2db(_BpfUnaryOp):
-    cdef void _apply(self, DTYPE_t *A, int n) nogil:
-        cdef double x
-        for i in range(n):
-            x = max(A[i], 1e-14)
-            A[i] = log10(x) * 20.0
-            
-
-cdef class _BpfLambdaClip(BpfInterface):
-    cdef BpfInterface bpf
-    cdef double y0, y1
-    cdef double __ccall__(self, double x) nogil:
-        cdef double y = self.bpf.__ccall__(x)
-        if y > self.y1:
-            return self.y1
-        elif y < self.y0:
-            return self.y0
-        return y
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        cdef:
-            ndarray [DTYPE_t, ndim=1] result
-            DTYPE_t *data
-            int i
-            # we account for the edge (x1 IS INCLUDED)
-            double dx = (x1 - x0) / (n - 1) 
-            double y1 = self.y1
-            double y0 = self.y0
-            double y
-            BpfInterface bpf = self.bpf
-        if out is None:
-            result = EMPTY1D(n)
-            data = <DTYPE_t *>result.data
-            with nogil:
-                for i in range(n):
-                    y = bpf.__ccall__(x0 + dx * i)
-                    y = _clip(y, y0, y1)
-                    data[i] = y
-            return result
-        else:
-            if PyArray_ISCONTIGUOUS(out):
-                data = <DTYPE_t *>out.data
-                with nogil:
-                    for i in range(n):
-                        y = bpf.__ccall__(x0 + dx * i)
-                        y = _clip(y, y0, y1)
-                        data[i] = y
-            else:
-                for i in range(n):
-                    for i in range(n):
-                        y = bpf.__ccall__(x0 + dx * i)
-                        y = _clip(y, y0, y1)
-                        out[i] = y
-            return out
-
-    def __reduce__(self):
-        return type(self), (), (self.bpf, self.y0, self.y1)
-    
-    def __setstate__(self, state):
-        self.bpf, self.y0, self.y1 = state
-        self._set_bounds_like(self.bpf)
-
-
-cdef _BpfLambdaClip _BpfLambdaClip_new(BpfInterface bpf, double y0, double y1):
-    cdef _BpfLambdaClip self = _BpfLambdaClip()
-    self._set_bounds_like(bpf)
-    self.bpf = bpf
-    self.y0 = y0
-    self.y1 = y1
-    return self
-
-
-cdef class _BpfDeriv(BpfInterface):
-    """
-    A bpf representing the derivative of another bpf
-
-    The derivative at a point x is the forward derivative: `d = (f(x) + f(x+h)) / 2`
-    """
-    cdef BpfInterface bpf
-    cdef double h
-
-    def __init__(self, BpfInterface bpf, double h=0):
-        """
-        Args:
-            bpf (BpfInterface): the bpf to take the derivative
-            h (float): the delta x used to calculate the derivative
-        """
-        self.h = h
-        self.bpf = bpf
-        self._x0, self._x1 = bpf.bounds()
-
-
-    @cython.cdivision(True)
-    cdef double __ccall__(self, double x) nogil:
-        cdef double h = self.h if self.h > 0 else (SQRT_EPS if x == 0 else SQRT_EPS*x)
-        cdef double xh = x+h
-        cdef double f0, f1
-        cdef double x1 = self._x1
-        if x <= x1 and xh > x1:
-            # Prevent discontinuities at the boundaries
-            f1 = self.bpf.__ccall__(x1)
-            f0 = self.bpf.__ccall__(x1-h)
-        else:
-            f1 = self.bpf.__ccall__(x+h)
-            f0 = self.bpf.__ccall__(x)
-        return (f1 - f0) / h   
-       
-    def __getstate__(self):
-        return (self.bpf,)
-
-
-cdef class _BpfInverted(BpfInterface):
-    cdef BpfInterface bpf
-    cdef double bpf_x0, bpf_x1
-    
-    def __init__(self, BpfInterface bpf):
-        cdef double x0, x1
-        self.bpf = bpf
-        self.bpf_x0, self.bpf_x1 = bpf.bounds()
-        x0 = bpf(self.bpf_x0)
-        x1 = bpf(self.bpf_x1)
-        if x0 >= x1:
-            raise BpfInversionError("could not invert bpf")
-        self._set_bounds(x0, x1)
-
-    cdef double __ccall__(self, double x) nogil:
-        cdef double out
-        cdef int outerror, funcalls
-        if x < self._x0:
-            return self.bpf_x0
-        elif x > self._x1:
-            return self.bpf_x1
-        out = _bpf_brentq(self.bpf, -x, self.bpf_x0, self.bpf_x1, &outerror, BRENTQ_XTOL, BRENTQ_RTOL, BRENTQ_MAXITER, &funcalls)
-        if outerror == 1:   # error
-            return NAN
-        return out
-    
-    def __getstate__(self): return (self.bpf,)
-
-
-cdef class _BpfIntegrate(BpfInterface):
-    """
-    A bpf representing the integration of another bpf
-    """
-    cdef BpfInterface bpf
-    cdef double bpf_at_x0, width, min_N_ratio, Nexp
-    cdef int N, N0, Nwidth
-    cdef public int debug
-    cdef public size_t oversample
-    
-    def __init__(self, BpfInterface bpf, N=None, bounds=None, double min_N_ratio=0.3, 
-                 double Nexp=0.8, int oversample=0):
-        """
-        Args:
-            bpf: the bpf to integrate
-            N (int): the number of intervals to integrate
-            bounds (tuple(float, float)): the bounds of this bpf
-            min_N_ratio (float): ??
-            Nexp (float): ??
-            oversample (int): oversampling index
-        """
-        cdef double x0, x1, dx
-        cdef int i
-        cdef BpfInterface tmpbpf
-        cdef int _N
-        if bounds is None:
-            bounds = bpf.bounds()
-        _N = N if N is not None else CONFIG['integrate.trapz_intervals']
-        x0, x1 = bounds
-        self._set_bounds(x0, x1)
-        self.bpf = bpf
-        self.N = _N
-        self.bpf_at_x0 = bpf.__ccall__(x0)
-        self.min_N_ratio = min_N_ratio
-        self.N0 = <int>(_N * min_N_ratio)
-        self.Nexp = Nexp
-        self.width = x1 - x0
-        self.Nwidth = _N - self.N0
-        self.oversample = oversample if oversample > 0 else CONFIG['integrate.oversample']
-        if x0 == INFNEG or x0 == INF:
-            raise ValueError("cannot integrate a function with an infinite lower bound")
-        self.debug = 0
-    
-    @cython.cdivision(True)
-    cdef int get_integration_steps(self, double x) nogil:
-        return <int>(self.N0 + pow((x - self._x0) / self.width, self.Nexp) * self.Nwidth)
-    
-    @cython.cdivision(True)
-    cdef double __ccall__(self, double x) nogil:
-        with gil:
-            return self.bpf.integrate_between(self._x0, x)
-        
-    @cython.cdivision(True)
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        cdef double [::1] accums
-        cdef double dx0, dx1, dy
-        cdef double dx = (x1 - x0) / (n-1)
-        cdef int i, return_out
-        cdef double accum = self.bpf.integrate_between(self._x0, x0) if x0 > self._x0 else self.__ccall__(self._x0)
-        cdef size_t subn = self.oversample
-        if out is not None and out.shape[0] == n and PyArray_ISCONTIGUOUS(out):
-            accums = out
-            return_out = 1
-        else:
-            accums = EMPTY1D(n)
-            return_out = 0
-        accums[0] = accum
-        for i in range(1, n):
-            dx1 = x0 + i*dx
-            dx0 = dx1 - dx            
-            dy = self.bpf.integrate_between(dx0, dx1, subn)
-            accum += dy
-            accums[i] = accum
-        if return_out:
-            return out
-        else:
-            return numpy.asarray(accums)
-
-    cpdef BpfInterface derivative(self):
-        return self.bpf
-
-    def __getstate__(self):
-        return (self.bpf, self.N, self.bounds(), self.min_N_ratio, self.Nexp)
-
-
-cdef class _BpfPeriodic(BpfInterface):
-    cdef BpfInterface bpf
-    cdef double x0
-    cdef double period
-
-    def __init__(self, BpfInterface bpf):
-        self._set_bounds(INFNEG, INF)
-        self.bpf = bpf
-        cdef double x0, x1
-        x0, x1 = bpf.bounds()
-        self.x0 = x0
-        self.period = x1 - x0
-    
-    @cython.cdivision(True)
-    cdef double __ccall__(self, double x) nogil:
-        # the C equivalent of self.x0 + ((x - self.x0) % self.period)
-        # python n % M | c ((n % M) + M) % M
-        cdef double n = x - self.x0
-        cdef double p = self.x0 + ( (n % self.period + self.period) % self.period )
-        return self.bpf.__ccall__( p )
-
-    def __getstate__(self): return (self.bpf,)
-
-
-cdef class _BpfProjection(BpfInterface):
-    cdef BpfInterface bpf
-    cdef double bpf_x0
-    cdef readonly double dx, rx, offset
-
-    def __init__(self, BpfInterface bpf, double rx, double dx=0, double offset=0, bounds=None):
-        """
-        equation:
-
-        x2 = (x - offset) * rx + dx
-        self(x) = bpf(x2)
-
-        stretched 3: rx=3, offset=0, dx=0
-        shifted 2: rx=1, offset=0, dx=1
-        """
-        self.bpf = bpf
-        self.rx = rx
-        self.dx = dx
-        self.offset = offset
-        cdef double x0, x1
-        if bounds:
-            self._set_bounds(bounds[0], bounds[1])
-        else:
-            x0 = (bpf._x0 - dx)/rx + offset
-            x1 = (bpf._x1 - dx)/rx + offset
-            if x0 < x1:
-                self._set_bounds(x0, x1)
-            else:
-                self._set_bounds(x1, x0)
-
-    @cython.cdivision(True)
-    cdef double __ccall__(self, double x) nogil:
-        x = (x - self.offset) * self.rx + self.dx
-        return self.bpf.__ccall__(x)
-
-    def fixpoint(self):
-        return 1 - (self.fx - self.offset*self.rx)/self.rx
-
-    def __getstate__(self): return (self.bpf, self.rx, self.dx, self.bounds())
-
-
-cdef double m_log(double x) nogil:
-    # taken from python implementation (in C)
-    if isfinite(x):  # INFNEG > x < INF:
-        if x > 0:
-            return log(x)
-        if x == 0:
-            return INFNEG
-        else:
-            return NAN
-    elif isnan(x):
-        return x
-    elif x > 0:
-        return x
-    else:
-        return NAN
-
-
-cdef class _BpfKeepSlope(BpfInterface):
-    cdef BpfInterface bpf
-    cdef double EPSILON
-
-    def __init__(self, BpfInterface bpf, double EPSILON=DEFAULT_EPSILON):
-        #BpfInterface.__init__(self, INFNEG, INF)
-        self._set_bounds(INFNEG, INF)
-        self.bpf = bpf
-        self.EPSILON = EPSILON
-
-    @cython.cdivision(True)
-    cdef double __ccall__(self, double x) nogil:
-        cdef double slope
-        cdef double x0 = self.bpf._x0
-        cdef double x1 = self.bpf._x1
-        if x0 <= x <= x1:
-            return self.bpf.__ccall__(x)
-        elif x > x1:
-            slope = (self.bpf.__ccall__(x1) - self.bpf.__ccall__(x1 - self.EPSILON)) / self.EPSILON
-            return self.bpf.__ccall__(x1) + slope * (x - x1)
-        else:
-            slope = (self.bpf.__ccall__(x0 + self.EPSILON) - self.bpf.__ccall__(x0)) / self.EPSILON
-            return self.bpf.__ccall__(x0) + slope * (x - x0)
-
-    def __getstate__(self): return self.bpf, self.EPSILON
-
-
-cdef class _BpfCrop(BpfInterface):
-    cdef BpfInterface bpf
-    cdef readonly double _y0, _y1
-    cdef readonly int outbound_mode
-
-    cdef double __ccall__(self, double x) nogil:
-        if self.outbound_mode == 0:
-            return self.bpf.__ccall__(x)
-        else:
-            if x < self._x0:
-                return self._y0
-            elif x > self._x1:
-                return self._y1
-            return self.bpf.__ccall__(x)
-
-    def __reduce__(self):
-        return type(self), (), (self.bpf, self._x0, self._x1, self.outbound_mode, self._y0, self._y1)
-
-    def __setstate__(self, state):
-        self.bpf, x0, x1, self.outbound_mode, self._y0, self._y1 = state
-        self._set_bounds(x0, x1)
-
-    cpdef _BpfCrop outbound_set(self, double y0, double y1):
-        """
-        set the value returned by this BPF outside its defined bounds (inplace)
-        """
-        self.outbound_mode = OUTBOUND_SET
-        self._y0 = y0
-        self._y1 = y1
-        return self
-
-    def outbound(self, double y0, y1=None):
-        """
-        return a new Bpf with the given values outside the bounds
-
-        !!! note
-    
-            One can specify one value for lower and one for upper bounds, 
-            or just one value for both
-        """
-        if y1 is None:
-            y1 = y0
-        return _BpfCrop_new(self.bpf, self._x0, self._x1, OUTBOUND_SET, y0, y1)
-
-    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
-        if x0 >= self.bpf._x0 and x1 <= self.bpf._x1:
-            return self.bpf.integrate_between(x0, x1)
-        cdef double integr0=0., integr1=0., integr2=0., _x0, _x1
-        if x0 < self.bpf._x0:
-            integr0 = self.__ccall__(x0) * (self.bpf._x0 - x0)
-            _x0 = self.bpf._x0
-        else:
-            _x0 = x0
-        if self._x1 > self.bpf._x1:
-            integr2 = self.__ccall__(x1) * (x1 - self.bpf._x1)
-            _x1 = self.bpf._x1
-        else:
-            _x1 = x1
-        integr1 = self.bpf.integrate_between(_x0, _x1)
-        return integr0 + integr1 + integr2
-
-    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
-        if self.outbound_mode == OUTBOUND_DONOTHING:
-            return self.bpf.mapn_between(n, x0, x1, out)
-        if x0 >= self._x1:
-            return numpy.ones((n,), dtype=float) * self.__ccall__(x0)
-        if x1 <= self._x0:
-            return numpy.ones((n,), dtype=float) * self.__ccall__(x1)
-
-        cdef double x, y0, y1, intersect_x0, intersect_x1, dx
-        cdef int i = 0
-        cdef int intersect_n, intersect_i0, intersect_i
-         
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = out if out is not None else EMPTY1D(n)
-        cdef c_numpy.ndarray[DTYPE_t, ndim=1] intersection
-        
-        cdef DTYPE_t *data = <DTYPE_t*>(A.data)
-        
-        dx = (x1 - x0) / (n - 1)
-        
-        if x0 < self._x0:
-            i = <int>((self._x0 - x0) / dx)
-            for j in range(i):
-                data[j] = self._y0
-            intersect_x0_quant = x0 + dx*i
-        else:
-            intersect_x0_quant = x0
-
-        intersect_x1 = min(x1, self._x1)
-        cdef double diff = ((intersect_x1 - x0) % dx)
-        if diff < 1e-15 or (dx - diff) < 1e-15:
-            diff = 0
-        intersect_x1_quant = intersect_x1 - diff
-        intersect_n = _dxton(dx, intersect_x0_quant, intersect_x1_quant)
-        intersection = self.bpf.mapn_between(intersect_n, intersect_x0_quant, intersect_x1_quant)
-        cdef DTYPE_t *intersection_data = <DTYPE_t*>(intersection.data)
-        cdef double intersect_dx = _ntodx(intersect_n, intersect_x0_quant, intersect_x1_quant)
-        # print("dx: %f, intersect_dx: %f, intersect_x1: %f, intersect_x1_quant: %f, x1: %f, diff:%f" % (dx, intersect_dx, intersect_x1, intersect_x1_quant, x1, diff))
-        for j in range(intersect_n):
-            A[i+j] = intersection_data[j]
-
-        y1 = self._y1
-        for j in range(i+intersect_n, n):
-            data[j] = y1
-
-        return A
-        
-
-cpdef _BpfCrop _BpfCrop_new(BpfInterface bpf, double x0, double x1, int outbound_mode, 
-                            double outbound0=0, double outbound1=0):
-    """
-    Create a cropped bpf. 
-    
-    Args:
-        bpf: the bpf to crop
-        x0: the lower bound
-        x1: the upper bound
-        outbound_mode: -1=use the default; 0=do nothing (the bpf is evaluated at the cropping 
-            point each time it is called outside the bounds); 1=cache the values; 2=set (in  
-            this case the last parameters outbount0 and outbound1 are used when called outside 
-            the bounds) 
-        outbound0: lower outbound value, returned when called with `x < x0` and *outbound_mode* is 2
-        outbound1: upper outbound value, returned when called with `x > x1` and *outbound_mode* is 2
-    
-    Returns:
-        (_BpfCrop) a cropped bpf
-    """
-    self = _BpfCrop()
-    self._set_bounds(x0, x1)
-    self.bpf = bpf
-    # -1: use the default, 0: do nothing, call __ccall__ each time, 
-    # 1: cache y0 and y1 for values outside the bounds, 
-    # 2: set y0 and y1 for values outside the bounds
-    if outbound_mode == OUTBOUND_DEFAULT:
-        outbound_mode = CONFIG['crop.outbound_mode']
-    self.outbound_mode = outbound_mode
-    if outbound_mode == OUTBOUND_CACHE:
-        self._y0 = self.bpf.__ccall__(x0)
-        self._y1 = self.bpf.__ccall__(x1)
-    elif outbound_mode == OUTBOUND_SET:
-        self._y0 = outbound0
-        self._y1 = outbound1
-    return self
-    
-
-cdef class _MultipleBpfs(BpfInterface):
-    cdef tuple _bpfs
-    cdef void** bpfpointers
-    cdef BpfInterface tmp
-    cdef int _numbpfs
-    
-    def __init__(self, bpfs):
-        self._numbpfs = len(bpfs)
-        self._bpfs = tuple(bpfs)
-        self._calculate_bounds()
-        self.bpfpointers = <void**>malloc(sizeof(void*) * self._numbpfs)
-        cdef int i
-        for i in range(self._numbpfs):
-            self.bpfpointers[i] = <void*>bpfs[i]
-    
-    def __dealloc__(self):
-        free(self.bpfpointers)
-    
-    def _calculate_bounds(self):
-        cdef double bounds0, bounds1
-        cdef double x0=INF, x1=INFNEG
-        for bpf in self._bpfs:
-            bound0, bound1 = bpf.bounds()
-            if bound0 < x0:
-                x0 = bound0
-            if bound1 > x1:
-                x1 = bound1
-        self._set_bounds(x0, x1)
-    
-    def __getstate__(self): return (self._bpfs,)
-    
-    cdef double __ccall__(self, double x) nogil:
-        with gil:
-            raise NotImplementedError
-
-
-cdef class Max(_MultipleBpfs):
-    """
-    A bpf which returns the max of multiple bpfs at a given point
-
-    ```python
-    a = linear(0, 0, 1, 0.5, 2, 0)
-    b = expon(0, 0, 2, 1, exp=3)
-    a.plot(show=False, color="red", linewidth=4, alpha=0.3)
-    b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
-    core.Max((a, b)).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
-    ```
-    ![](assets/Max.png)
-    """
-    def __init__(self, *bpfs):
-        if len(bpfs) == 1 and isinstance(bpfs[0], (list, tuple)):
-            bpfs = bpfs[0]
-        _MultipleBpfs.__init__(self, bpfs)
-
-    cdef double __ccall__(self, double x) nogil:
-        cdef double y = INFNEG
-        cdef double res
-        cdef int i
-        for i in range(self._numbpfs):
-            with gil:
-                self.tmp = <BpfInterface>(self.bpfpointers[i])
-            res = self.tmp.__ccall__(x)
-            if res > y:
-                y = res
-        return y
-
-
-cdef class Min(_MultipleBpfs):
-    """
-    A bpf which returns the min of multiple bpfs at a given point
-
-    ```python
-    a = linear(0, 0, 1, 0.5, 2, 0)
-    b = expon(0, 0, 2, 1, exp=3)
-    a.plot(show=False, color="red", linewidth=4, alpha=0.3)
-    b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
-    core.Min((a, b)).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
-    ```
-    ![](assets/Min.png)
-    
-    """
-    def __init__(self, *bpfs):
-        if len(bpfs) == 1 and isinstance(bpfs[0], (list, tuple)):
-            bpfs = bpfs[0]
-        _MultipleBpfs.__init__(self, bpfs)
-    
-    cdef double __ccall__(self, double x) nogil:
-        cdef double y = INF
-        cdef double res
-        cdef int i
-        for i in range(self._numbpfs):
-            with gil:
-                tmp = <BpfInterface>(self.bpfpointers[i])
-            res = tmp.__ccall__(x)
-            if res < y:
-                y = res
-        return y
-
-
-cdef class Stack(_MultipleBpfs):
-    """
-    A bpf representing a stack of bpf
-
-    Within a Stack, a bpf does not have outbound values. When evaluated
-    outside its bounds the bpf below is used, iteratively until the
-    lowest bpf is reached. Only the lowest bpf is evaluated outside its
-    bounds
-
-    Example
-    -------
-
-    ```python
-    # Interval    bpf
-    # [0, 3]      a
-    # (3, 4]      b
-    # (4, 10]     c
-
-    from bpf4 import *
-    import matplotlib.pyplot as plt
-    
-    a = linear(0, 0, 3, 1)
-    b = linear(2, 9, 4, 10)
-    c = halfcos(0, 0, 10, 10)
-    s = core.Stack((a, b, c))
-
-    ax = plt.subplot(111)
-    a.plot(color="#f00", alpha=0.4, axes=ax, linewidth=4, show=False)
-    b.plot(color="#00f", alpha=0.4, axes=ax, linewidth=4, show=False)
-    c.plot(color="#f0f", alpha=0.4, axes=ax, linewidth=4, show=False)
-    s.plot(axes=ax, linewidth=2, color="#000", linestyle='dotted')
-    ```
-    ![](assets/stack2.png)
-
-    """
-    cdef double[::1] flatbounds
-
-    def __init__(self, bpfs):
-        """
-        Args:
-            bpfs (list|tuple): A sequence of bpfs. The order defined the evaluation
-                order. The first bpf is on top, the last bpf is on bottom. Only
-                the last bpf is evaluated outside its bounds
-
-        """
-        self.flatbounds = EMPTY1D(len(bpfs)*2)
-        _MultipleBpfs.__init__(self, bpfs)
-
-    def _calculate_bounds(self):
-        cdef double x0 = INF, x1 = INFNEG
-        cdef BpfInterface b
-        cdef int i = 0
-        for b in self._bpfs:
-            if b.x0 < x0:
-                x0 = b.x0
-            if b.x1 > x1:
-                x1 = b.x1
-            self.flatbounds[i] = b.x0
-            self.flatbounds[i+1] = b.x1
-            i += 2
-        self._set_bounds(x0, x1)
-
-    cdef double __ccall__(self, double x) nogil:
-        cdef double out = 0.
-        for i in range(self._numbpfs):
-            if self.flatbounds[i*2] <= x <= self.flatbounds[i*2+1] or i == self._numbpfs - 1:
-                with gil:
-                    self.tmp = <BpfInterface>(self.bpfpointers[i])
-                out = self.tmp.__ccall__(x)
-                break
-        return out
-
-
-cdef class _BpfSelect(_MultipleBpfs):
-    cdef BpfInterface which
-    cdef InterpolFunc* func
-    cdef int numbpfs
-    
-    def __init__(self, which, bpfs, shape='linear'):
-        """
-        Interpolate between adjacent bpfs
-
-        Args:
-            which: a bpf mapping x->bpf index, where the index can
-                be fractionl and will interpolate between adjacent
-                bpfs
-            bpfs: the bpfs to select from
-            shape: the interpolation shape when dealing with fractional indexes
-        """
-        self.which = which
-        self.numbpfs = len(bpfs)
-        self.func = InterpolFunc_new_from_descriptor(shape)
-        _MultipleBpfs.__init__(self, bpfs)
-    
-    cdef double __ccall__(self, double x) nogil:
-        cdef double index = self.which.__ccall__(x)
-        cdef double y0, y1, x0
-        if index <= 0:
-            with gil:
-                b0 = <BpfInterface>(self.bpfpointers[0])
-            return b0.__ccall__(x)
-        elif index >= self.numbpfs - 1:
-            with gil:
-                b0 = <BpfInterface>(self.bpfpointers[self.numbpfs-1])
-            return b0.__ccall__(x)
-        else:
-            x0 = floor(index)
-            if x0 == index:
-                with gil:
-                    b0 = <BpfInterface>(self.bpfpointers[<int>x0])
-                    return b0.__ccall__(x)
-
-            with gil:
-                b0 = <BpfInterface>(self.bpfpointers[<int>x0])
-                b1 = <BpfInterface>(self.bpfpointers[<int>x0 + 1])
-
-            y0 = b0.__ccall__(x)
-            y1 = b1.__ccall__(x)
-            return InterpolFunc_call(self.func, index, x0, y0, x0+1, y1)
-
-def brentq(bpf, double x0, double xa, double xb, double xtol=9.9999999999999998e-13, 
-           double rtol=4.4408920985006262e-16, max_iter=100):
-    """
-    Calculate the zero of `bpf + x0` in the interval `(xa, xb)` using brentq algorithm
-
-    !!! note 
-
-        To calculate all the zeros of a bpf, use [.zeros()](#zeros)
-
-    Args:
-        bpf (BpfInterface): the bpf to evaluate
-        x0 (float): an offset so that bpf(x) + x0 = 0
-        xa (float): the starting point to look for a zero
-        xb (float): the end point
-        xtol (float): The computed root x0 will satisfy np.allclose(x, x0, atol=xtol, rtol=rtol)
-        rtol (float): The computed root x0 will satisfy np.allclose(x, x0, atol=xtol, rtol=rtol)
-        max_iter (int): the max. number of iterations
-
-    Returns:
-        (tuple[float, int]) A tuple (zero of the bpf, number of function calls)
-
-
-    ## Example
-    
-    ```python
-
-    # calculate the x where a == 0.5
-    >>> from bpf4 import *
-    >>> a = linear(0, 0, 10, 1)
-    >>> xzero, numcalls = brentq(a, -0.5, 0, 1)
-    >>> xzero
-    5
-    ```
-    """
-    cdef int outerror, funcalls
-    cdef double result
-    result = _bpf_brentq(bpf, x0, xa, xb, &outerror, xtol, rtol, max_iter, &funcalls)
-    if outerror:
-        raise ValueError("zero of function cannot be found within the interval given")
-    return result, funcalls
-
-
-cpdef BpfInterface blend(a, b, mix=0.5):
-    """
-    Blend these BPFs
-
-    Args:
-        a (BpfInterface): first bpf
-        b (BpfInterface): second bpf
-        mix (float | BpfInterface): how to mix the bpfs. Can be fixed or
-            itself a bpf (or any function) returning a value between 0-1 
-
-    Returns:
-        (BpfInterface) The blended bpf
-    
-    
-    !!! note
-
-        if mix == 0: the result is *a*
-        if mix == 1: the result is *b*
-    
-    
-    ## Example
-    
-    Create a curve which is in between a halfcos and a linear interpolation
-    
-    ```python
-    from bpf4 import *
-    a = halfcos(0, 0, 1, 1, exp=2)
-    b = linear(0, 0, 1, 1)
-    c = blend(a, b, 0.5)
-
-    a.plot(show=False, color="red")
-    b.plot(show=False, color="blue")
-    c.plot(color="green")
-
-    ```
-    ![](assets/blend1.png)
-
-    Closer to halfcos
-
-    ```python
-    c = blend(a, b, 0.2)
-    a.plot(show=False, color="red")
-    b.plot(show=False, color="blue")
-    c.plot(color="green")
-    ```
-    ![](assets/blend2.png)
-    """
-    if isinstance(mix, (int, float)):
-        return _BpfBlendConst(_asbpf(a), _asbpf(b), mix)
-    return _BpfBlend(_asbpf(a), _asbpf(b), _asbpf(mix))
-        
-
-
-cdef inline int isnumber(obj):
-    return isinstance(obj, (int, float))
-
-
-@cython.cdivision(True)
-cdef inline double _bpf_brentq(BpfInterface bpf, double x0, double xa, double xb, int* outerror, 
-                               double xtol, double rtol, int max_iter, int *outfuncalls) nogil:
-    # original values: xtol=9.9999999999999998e-13, rtol=4.4408920985006262e-16, max_iter=100
-    # calculate the 0 of the function bpf + x0 in the interval (xa, xb)
-    # if it is not possible, outerror is set to 1, otherwise it is 0
-    cdef:
-        double xpre = xa
-        double xcur = xb
-        double xblk = 0
-        double fpre, fcur, stry, dpre, dblk, sbis, tol
-        double fblk = 0
-        double spre = 0
-        double scur = 0
-        double a, b
-        int funcalls = 2
-        int i
-    outerror[0] = 0
-    fpre = bpf.__ccall__(xpre) + x0
-    fcur = bpf.__ccall__(xcur) + x0
-    outfuncalls[0] = 2
-    if fpre * fcur > 0:
-        outerror[0] = 1
-        return 0
-    if fpre == 0:
-        return xpre
-    if fcur == 0:
-        return xcur
-    for i in range(max_iter):
-        if fpre * fcur < 0:
-            xblk = xpre
-            fblk = fpre
-            spre = scur = xcur - xpre
-        if fabs(fblk) < fabs(fcur):
-            xpre = xcur
-            xcur = xblk
-            xblk = xpre
-            fpre = fcur
-            fcur = fblk
-            fblk = fpre
-        tol = xtol + rtol * fabs(xcur)
-        sbis = (xblk - xcur) / 2
-        if fabs(fcur) == 0 or fabs(sbis) < tol:
-            return xcur
-        if fabs(spre) > tol and fabs(fcur) < fabs(fpre):
-            if xpre == xblk:    # interpolate
-                stry = -fcur * (xcur - xpre) / (fcur - fpre)
-            else:               # extrapolate
-                dpre = (fpre - fcur)/(xpre - xcur)
-                dblk = (fblk - fcur)/(xblk - xcur)
-                stry = -fcur*(fblk*dblk - fpre*dpre) / (dblk*dpre*(fblk - fpre))     
-            # if (2*fabs(stry) < DMIN(fabs(spre), 3*fabs(sbis) - tol)):
-            a = fabs(spre)
-            b = 3*fabs(sbis) - tol
-            if (2*fabs(stry) < (a if a < b else b)):
-            #if (2*fabs(stry) < DMIN(fabs(spre), 3*fabs(sbis) - tol)):   
-                spre = scur
-                scur = stry  # good short step
-            else:
-                spre = sbis
-                scur = sbis  # bisect 
-        else:
-            spre = sbis
-            scur = sbis
-        xpre = xcur
-        fpre = fcur
-        if fabs(scur) > tol:
-            xcur += scur
-        else:
-            xcur += tol if sbis > 0 else -tol
-        fcur = bpf.__ccall__(xcur) + x0
-        funcalls += 1
-    outfuncalls[0] = funcalls
-    return xcur
-
-
-@cython.boundscheck(False)
-@cython.cdivision(True)
-cpdef list bpf_zero_crossings(BpfInterface b, double h=0.01, int N=0, 
-                              double x0=NAN, double x1=NAN, int maxzeros=0):
-    """
-    Return the zeros if b in the interval defined
-
-    Args:
-        b (BpfInterface): a bpf
-        h (float): the interval to scan for zeros. for each interval only one zero will be found
-        N (int): alternatively you can give the number of intervals to scan. *h* will be calculated 
-            from *N* (the *h* parameter is not used)
-        x0 (float): If given, the bounds to search within 
-        x1 (float): If given, the bounds to search within
-        maxzeros (int): if given, search will stop if this number of zeros is found
-
-    Returns:
-        (List[float]) A list of zeros (x coord points where the bpf is 0)
-    """
-    if isnan(x0):
-        x0 = b._x0
-    if isnan(x1):
-        x1 = b._x1
-    if h > (x1 - x0) * 0.5:
-        h = (x1 - x0) * 0.25
-    if N == 0:
-        N = <int>((x1 - x0) / h) + 1
-    else:
-        h = (x1 - x0) / (N - 1)
-    cdef list out = []
-    cdef double y0, y1, xa, xb, zero
-    cdef int outerror, funcalls
-    y1 = b.__ccall__(x0)
-    cdef double last_zero = 0
-    cdef int numzeros = 0
-    cdef int add_it
-    for i in range(N - 1):
-        xa = x0 + i * h
-        xb = xa + h - EPS
-        y0 = b.__ccall__(xa)
-        y1 = b.__ccall__(xb)
-        add_it = 0
-        if y0 * y1 < 0:
-            outerror = -1
-            zero = _bpf_brentq(b, 0, xa, xb, &outerror, 9.9999999999999998e-13, 4.4408920985006262e-16, 100, &funcalls)
-            if outerror == 0:
-                add_it = 1
-        elif y1 == 0 and y0 != 0:
-            zero = xb
-            add_it = 1
-        elif y0 == 0 and y1 != 0 and xa > last_zero:
-            zero = xa
-            add_it = 1
-        if add_it:
-            last_zero = zero
-            out.append(zero)
-            numzeros += 1
-            if maxzeros > 0 and numzeros >= maxzeros:
-                break
-    return out
-
-
-cdef inline double _integrate_adaptive_simpsons_inner(BpfInterface f, double a, double b, double epsilon, 
-                                                      double S, double fa, double fb, double fc, int bottom):
-    cdef: 
-        double c = (a + b) / 2
-        double h = b - a
-        double d = (a + c) / 2
-        double g = (c + b) / 2
-        double fd = f.__ccall__(d)
-        double fe = f.__ccall__(g)
-        double Sleft = (h / 12) * (fa + 4 * fd + fc)
-        double Sright = (h / 12) * (fc + 4 * fe + fb)
-    S2 = Sleft + Sright
-    if bottom <= 0 or abs(S2 - S) <= 15 * epsilon:
-        return S2 + (S2 - S) / 15.
-    return _integrate_adaptive_simpsons_inner(f, a, c, epsilon / 2, Sleft, fa, fc, fd, bottom - 1) + \
-           _integrate_adaptive_simpsons_inner(f, c, b, epsilon / 2, Sright, fc, fb, fe, bottom - 1)
-
-
-cdef double integrate_simpsons(BpfInterface f, double a, double b, double accuracy=10e-10, int max_iterations=50):
-    cdef:
-        double c = (a + b) / 2
-        double h = b - a
-        double fa = f.__ccall__(a)
-        double fb = f.__ccall__(b)
-        double fc = f.__ccall__(c)
-        double S = (h / 6) * (fa + 4 * fc + fb)
-    return _integrate_adaptive_simpsons_inner(f, a, b, accuracy, S, fa, fb, fc, max_iterations)
+# cython: binding=True
+# cython: boundscheck=False
+# cython: embedsignature=True
+# cython: wraparound=False
+# cython: infer_types=True
+# cython: profile=False
+# cython: c_string_type=str, c_string_encoding=ascii
+# cython: language_level=3
+# cython: annotation_typing=True 
+
+cdef extern from "math.h":
+    double cos(double x) nogil
+    double sin(double x) nogil
+    double pow(double x, double y) nogil
+    double ceil(double x) nogil
+    double log(double x) nogil
+    double exp(double x) nogil
+    double floor(double x) nogil
+    double fmod(double x, double y) nogil
+    double hypot(double x, double y) nogil
+    double atan2(double x, double y) nogil
+    double tanh (double x ) nogil
+    double fabs (double x) nogil
+    double sqrt(double x) nogil
+    double INFINITY, NAN, M_E, M_PI
+    int isfinite(double x) nogil
+    int isinf(double x) nogil
+    int isnan(double x) nogil
+    double acos(double x) nogil
+    double asin(double x) nogil
+    double cosh(double x) nogil
+    double log10(double x) nogil
+    double tan(double x) nogil
+    double sinh(double x) nogil
+    double log1p(double x) nogil
+    
+#cdef extern from "string.h":
+#    ctypedef void* const_void_ptr "const void *"
+#    void *memcpy(void *s1, const_void_ptr s2, size_t n) nogil
+
+# ----------------------------------------------  cimports
+from libc.stdlib cimport malloc, free # , realloc
+from libc.stdlib cimport rand, srand, RAND_MAX
+from libc.stdio cimport printf, fflush, stdout
+from libc.stdint cimport int64_t
+
+from cpython cimport PyList_GET_SIZE, PyList_GET_ITEM, PyTuple_New, PyTuple_SetItem
+cimport cython
+cimport numpy as c_numpy
+from cython.view cimport array as cvarray
+from numpy cimport (
+    ndarray,
+    npy_intp,
+    PyArray_DIM,
+    float_t,
+    PyArray_ISCONTIGUOUS,
+    import_array,
+    PyArray_GETCONTIGUOUS,
+    PyArray_ContiguousFromAny,  # object PyArray_ContiguousFromAny(op, int, int min_depth, int max_depth)
+    NPY_DOUBLE,
+    PyArray_SimpleNew,          # PyArray_SimpleNew(int nd, npy_intp *dims, int type_num)
+    PyArray_SimpleNewFromData,  # PyArray_SimpleNewFromData(int nd, npy_intp *dims, int type_num, void *data)
+    PyArray_EMPTY,              # PyArray_EMPTY(int nd, npy_intp* dims, int typenum, int fortran)
+    PyArray_ISCARRAY,           # int PyArray_ISCARRAY( c_numpy.ndarray instance )
+    PyArray_ZEROS,              # PyArray_ZEROS(int nd, npy_intp* dims, int type_num, int fortran)
+    PyArray_FILLWBYTE           # PyArray_FILLWBYTE(obj, int val)
+    )
+
+# ---------------------------- import std-lib
+# import math
+import sys
+import random
+
+# ---------------------------- import others
+import numpy
+from numpy import array
+from . import arraytools
+
+# ---------------------------- own imports
+from .config import CONFIG
+
+# ---------------------------- init
+import_array()
+srand(random.randint(0, 99999))
+
+# ---------------------------- platform specific constants
+
+cdef double EPS = sys.float_info.epsilon
+cdef double SQRT_EPS = sqrt(EPS)
+
+# ---------------------------- DEFs
+DEF PI = 3.141592653589793238462643383279502884197169399375105
+DEF BRENTQ_ZERO = 2.221e-16
+DEF BRENTQ_XTOL = 9.9999999999999998e-13
+DEF BRENTQ_RTOL = 4.4408920985006262e-16
+DEF BRENTQ_MAXITER = 100
+DEF QUAD_LIMIT = 100
+DEF SIMPSONS_ACCURACY = 1e-10
+DEF SIMPSONS_MAXITER = 100
+
+
+# -------------------------------------------------------------------
+#       ERROR TYPES
+# -------------------------------------------------------------------
+class BpfPointsError(ValueError): pass
+class BpfInversionError(ValueError): pass
+
+# -------------------------------------------------------------------
+#       INLINE FUNCS
+# -------------------------------------------------------------------
+ctypedef struct InterpolFunc
+
+@cython.cdivision(True)
+cdef inline double intrp_linear(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    return y0 + (y1 - y0) * ((x - x0) / (x1 - x0))
+
+cdef inline double intrp_nointerpol(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    return y0 if x < x1 else y1
+
+cdef inline double intrp_nearest(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    if (x - x0) <= (x1 - x):
+        return y0
+    return y1
+
+@cython.cdivision(True)
+cdef inline double intrp_halfcos(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    cdef:
+        double dx, y
+        double x1x0 = x1 - x0
+        int i
+    if self.numiter > 1:
+        for i in range(self.numiter - 1):
+            dx = (x - x0) / x1x0    
+            dx = (dx + 1) * 3.14159265358979323846
+            x = x0 + x1x0 * (1 + cos(dx)) / 2.0
+    dx = (x - x0) / x1x0    
+    dx = (dx + 1) * 3.14159265358979323846
+    y = y0 + (y1 - y0) * (1 + cos(dx)) / 2.0
+    return y
+
+@cython.cdivision(True)
+cdef inline double intrp_halfcosexp(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    cdef:
+        double dx
+        double x1x0 = x1 - x0
+        int i
+        double exp = self.exp
+    if self.numiter > 1:
+        for i in range(self.numiter - 1):
+            dx = pow((x - x0) / x1x0, exp)    
+            dx = (dx + 1) * 3.14159265358979323846
+            x = x0 + x1x0 * (1 + cos(dx)) / 2.0
+    dx = pow((x - x0) / x1x0, exp)    
+    dx = (dx + 1) * 3.14159265358979323846        
+    return y0 + (y1 - y0) * (1 + cos(dx)) / 2.0
+
+
+@cython.cdivision(True)
+cdef inline double intrp_halfcosexpm(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    cdef:
+        double dx
+        double x1x0 = x1 - x0
+        double exp = self.exp
+        int i
+    if y1 < y0:
+        exp = 1/exp    
+    if self.numiter > 1:
+        for i in range(self.numiter - 1):
+            dx = pow((x - x0) / x1x0, exp)    
+            dx = (dx + 1) * 3.14159265358979323846
+            x = x0 + x1x0 * (1 + cos(dx)) / 2.0
+    dx = pow((x - x0) / x1x0, exp)    
+    dx = (dx + 1) * 3.14159265358979323846        
+    return y0 + (y1 - y0) * (1 + cos(dx)) / 2.0
+
+    
+
+@cython.cdivision(True)
+cdef inline double intrp_expon(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    cdef: 
+        double exp = self.exp
+        double dx
+        double x1x0 = x1 - x0
+        int i
+    if self.numiter > 1:
+        for i in range(self.numiter - 1):
+            dx = (x - x0) / x1x0
+            x = x0 + pow(dx, exp) * x1x0
+    dx = (x - x0) / x1x0
+    return y0 + pow(dx, exp) * (y1 - y0)
+
+
+@cython.cdivision(True)
+cdef inline double intrp_exponm(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    cdef: 
+        double exp = self.exp
+        double dx
+        double x1x0 = x1 - x0
+        int i
+    if y1 < y0:
+        exp = 1/exp
+    if self.numiter > 1:
+        for i in range(self.numiter - 1):
+            dx = (x - x0) / x1x0
+            x = x0 + pow(dx, exp) * x1x0
+    dx = (x - x0) / x1x0
+    return y0 + pow(dx, exp) * (y1 - y0)
+
+    
+@cython.cdivision(True)
+cdef inline double intrp_smooth(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    """
+    #define SMOOTHSTEP(x) (x) * (x) * (3 - 2 * x)
+    for (i = 0; i < N; i++) {
+      v = i / N;
+      v = SMOOTHSTEP(v);
+      X = (A * v) + (B * (1 - v));
+    }   --> http://sol.gfxile.net/interpolation/
+    """
+    cdef:
+        double x1x0 = x1 - x0
+        double v
+        int i
+
+    if self.numiter > 1:
+        for i in range(self.numiter - 1):
+            v = (x - x0) / x1x0
+            v = v*v*(3 - 2*v)
+            x = x0 + x1x0 * v
+    v = (x - x0) / x1x0
+    v = v*v*(3 - 2*v)
+    return y0 + (y1 - y0) * v
+
+@cython.cdivision(True)
+cdef inline double intrp_smoother(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    cdef:
+        double x1x0 = x1 - x0
+        double v
+    # x * x * x * (x * (x * 6 - 15) + 10);
+    v = (x - x0) / x1x0
+    v = v*v*v*(v*(v*6 - 15) + 10)
+    return y0 + (y1 - y0) * v
+
+# ------------------------------------------------------------------------------------------------
+
+@cython.cdivision(True)
+cdef inline double _integr_trapz(double *xs, int xs_size, double dx) nogil:
+    """
+    area of a trapezium (trapezoid)
+
+        a + b
+    A = ----- h
+          2 
+
+    where
+    A: area of the trapezium
+    a: length of one of the sides
+    b: length of the other side
+    h: distance between a and b (height)
+
+    In a function
+
+      /|
+     / |
+    |  |
+    |  |
+    ----
+
+    The curve is divided by a grid of dx. 
+    a: f(x)
+    b: f(x+dx)
+    h: dx
+
+    trapz = (f(x) + f(x+dx)) / 2 * dx
+    """
+    cdef int i
+    cdef double x0, x1, accum
+    cdef double r = 0.5 * dx
+    x0 = xs[0]
+    accum = 0
+    for i in range(1, xs_size):
+        x1 = xs[i]
+        accum += (x0 + x1) * r
+        x0 = x1
+    return accum
+
+@cython.cdivision(True)
+cdef inline double _integr_trapz_between(double *xs, int xs_size, double dx, double offset, double a, double b) nogil:
+    """
+    integrate sampled values `xs`, spaced at `dx` with an offset of `offset` in the range
+    [a, b] -- both a and b included
+
+    NB: the definition of xs is used, no oversampling takes place for better accuracy
+    in the cases where a and/or b do not fall exactly on the grid specified by offset+i*dx
+    """
+    cdef int i
+    cdef double x0, x1, accum
+    cdef double r = 0.5 * dx
+    cdef int i0 = <int>((a - offset) / dx)
+    cdef int i1 = <int>((b - offset) / dx) + 1
+    accum = 0
+    if i1 > xs_size:
+        i1 = xs_size
+    x0 = xs[i0]
+    for i in range(i0+1, i1):
+        x1 = xs[i]
+        accum += (x0 + x1) * r
+        x0 = x1
+    return accum
+
+@cython.cdivision(True)
+cdef inline double _integr_trapz_between_exact(double *xs, int xs_size, double dx, double offset, double a, double b) nogil:
+    """
+    integrate sampled values `xs`, spaced at `dx` with an offset of `offset` in the range
+    [a, b] -- both a and b included
+    """
+    cdef int i
+    cdef double x0, x1, accum, y
+    cdef double r = 0.5 * dx
+    cdef int i0 = <int>((a - offset) / dx + 0.999999999)
+    cdef int i1 = <int>((b - offset) / dx) + 1
+    cdef double rest_a = ((a - offset) % dx) / dx
+    cdef double rest_b = ((b - offset) % dx) / dx
+    accum = 0
+    if i1 > xs_size:
+        i1 = xs_size
+    x0 = xs[i0]
+    for i in range(i0+1, i1):
+        x1 = xs[i]
+        accum += (x0 + x1) * r
+        x0 = x1
+    if rest_a > 0 and i0 > 0:
+        y0 = xs[i0-1]
+        y1 = xs[i0]
+        y = y0 + (y1-y0) * rest_a
+        accum += (y + y1) * 0.5 * dx * (1 - rest_a)
+    if rest_b > 0 and (i1 + 1) < xs_size:
+        y0 = xs[i1]
+        y1 = xs[i1+1]
+        y = y0 + (y1-y0) * rest_a
+        accum += (y0 + y) * 0.5 * dx * rest_b
+    return accum
+
+cdef inline double _clip(double x, double x0, double x1) nogil:
+    return x1 if x > x1 else x0 if x < x0 else x
+
+cdef inline double _ntodx(size_t n, double x0, double x1):
+    return (x1 - x0) / (n - 1)
+
+cdef inline size_t _dxton(double dx, double x0, double x1):
+    return <size_t>round((x1-x0)/dx+1)
+    
+cdef double _a4 = 442.0
+DEF loge_2 = 0.6931471805599453094172321214581766
+
+
+def setA4(double freq):
+    """
+    Set the reference freq used
+
+    Args:
+        freq (float): the reference frequency for A4
+    """
+    global _a4
+    _a4 = freq
+
+
+@cython.cdivision(True)
+cdef double m2f(double midinote) nogil:
+    global _a4
+    if 0.0 <= midinote:
+        return _a4 * pow(2.0, (midinote - 69.0) / 12.0)
+    return 0.
+
+@cython.cdivision(True)
+cdef double f2m(double freq) nogil:
+    global _a4
+    if 8.2129616379875419 < freq:    # this is the freq. of midi 0
+        return 12 * (log(freq / _a4) / loge_2) + 69.0
+    return 0
+
+# ---------------------------- TYPES
+ctypedef double(*t_unfunc)(double) nogil
+
+cdef t_unfunc UNFUNCS[14]
+UNFUNCS[:] = [
+    cos,    # 0
+    sin,    # 1
+    ceil,   # 2
+    log,    # 3
+    exp,    # 4
+    floor,  # 5
+    tanh,   # 6
+    fabs,   # 7
+    sqrt,   # 8
+    acos,   # 9
+    asin,   # 10
+    tan,    # 11
+    sinh,   # 12
+    log10,  # 13
+    # m2f,    # 14
+    # f2m     # 15
+]
+
+ctypedef double(*t_func0)(double, double, double, double, double, double) nogil
+ctypedef double(*t_func)(InterpolFunc *, double, double, double, double, double) nogil
+
+ctypedef struct InterpolFunc:
+    t_func func
+    double exp
+    int numiter
+    double mix
+    InterpolFunc* blend_func
+    char *name
+    unsigned int needs_free
+
+DTYPE = numpy.float64  #np.float64
+ctypedef c_numpy.float_t DTYPE_t
+
+# InterpolFunc
+cdef inline void InterpolFunc_init(InterpolFunc *self, t_func func, double exp, char *name, unsigned int needs_free):
+    self.func = func
+    self.exp = exp
+    self.numiter = 1
+    self.mix = -1
+    self.blend_func = NULL
+    self.name = name
+    self.needs_free = needs_free
+
+cdef inline InterpolFunc* InterpolFunc_new(t_func func, double exp, char *name, unsigned int needs_free):
+    cdef InterpolFunc* out
+    out = <InterpolFunc *>malloc(sizeof(InterpolFunc))
+    InterpolFunc_init(out, func, exp, name, needs_free)
+    return out
+
+cdef inline InterpolFunc* InterpolFunc_new_blend_from_descr(str descr0, str descr1, double mix):
+    cdef InterpolFunc* out = InterpolFunc_new_from_descriptor(descr0, 1)  # force new 
+    cdef InterpolFunc* blend = InterpolFunc_new_from_descriptor(descr1, 1)  # force new
+    out.blend_func = blend
+    out.mix = mix
+    return out
+
+cdef InterpolFunc* InterpolFunc_new_from_descriptor(str descr, int forcenew=0):
+    cdef InterpolFunc* out = NULL
+    cdef double exp = 1.0
+    cdef str func_name
+    if "(" in descr:
+        func_name, param = descr.split("(")
+        exp = float(param[:len(param)-1])
+    else:
+        func_name = descr
+    if func_name == 'linear':
+        if not forcenew:
+            out = InterpolFunc_linear
+        else:
+            out = InterpolFunc_new(intrp_linear, 1, '', 1)
+    elif func_name == 'expon':
+        out = InterpolFunc_new(intrp_expon, exp, 'expon', 1)
+    elif func_name == 'halfcos':
+        if exp == 1.0 and not forcenew:
+            out = InterpolFunc_halfcos
+        else:
+            out = InterpolFunc_new(intrp_halfcosexp, exp, 'halfcosexp', 1)
+    elif func_name == 'halfcosexp':
+        out = InterpolFunc_new(intrp_halfcosexp, exp, 'halfcosexp', 1)
+    elif func_name == 'nointerpol':
+        out = InterpolFunc_nointerpol
+    elif func_name == 'nearest':
+        out = InterpolFunc_nearest
+    elif func_name == 'smooth':
+        out = InterpolFunc_smooth
+    return out
+
+cdef inline double InterpolFunc_call(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+    cdef double v0, v1
+    if self.mix <= 0:
+        return self.func(self, x, x0, y0, x1, y1)
+    else:
+        v0 = self.func(self, x, x0, y0, x1, y1)
+        v1 = self.blend_func.func(self.blend_func, x, x0, y0, x1, y1)
+        return v0 * (1 - self.mix) + v1 * self.mix
+
+#cdef inline double InterpolFunc_call(InterpolFunc *self, double x, double x0, double y0, double x1, double y1) nogil:
+#    cdef double y = self.func(self, x, x0, y0, x1, y1)
+#    return y
+
+cdef inline void InterpolFunc_free(InterpolFunc *self):
+    if self is not NULL:
+        if self.blend_func is not NULL:
+            InterpolFunc_free(self.blend_func)
+        if self.needs_free == 1:
+            free(self)
+
+cdef inline str InterpolFunc_get_descriptor(InterpolFunc *self):
+    if self.exp != 1.0:
+        return "%s(%s)" % (self.name, str(self.exp))
+    else:
+        return self.name   
+
+# create the most used interpolation functions, which are shared across BPFs
+cdef InterpolFunc* InterpolFunc_linear    = InterpolFunc_new(intrp_linear, 1.0, 'linear',  0)
+cdef InterpolFunc* InterpolFunc_halfcos    = InterpolFunc_new(intrp_halfcos, 1.0, 'halfcos', 0)
+cdef InterpolFunc* InterpolFunc_nointerpol = InterpolFunc_new(intrp_nointerpol,  1.0, 'nointerpol',  0)
+cdef InterpolFunc* InterpolFunc_nearest   = InterpolFunc_new(intrp_nearest,  1.0, 'nearest',  0)
+cdef InterpolFunc* InterpolFunc_smooth    = InterpolFunc_new(intrp_smooth, 1.0, 'smooth', 0)
+cdef InterpolFunc* InterpolFunc_smoother  = InterpolFunc_new(intrp_smoother, 1.0, 'smoother', 0)
+
+
+cdef inline ndarray EMPTY1D(int size): #new_empty_doublearray_1D(int size):
+    cdef npy_intp *dims = [size]
+    return PyArray_EMPTY(1, dims, NPY_DOUBLE, 0)
+
+DEF NUM_XS_FOR_RENDERING = 200
+DEF DEFAULT_EPSILON = 1e-4
+DEF INF = float('inf')
+DEF INFNEG = float('-inf')
+cdef double MAX_FLOAT = 3.40282346638528860e+38
+CONST_XS_FOR_RENDERING = numpy.linspace(0., 1., NUM_XS_FOR_RENDERING)
+DEF NOCOPY = False
+
+# behaviour for cropping
+DEF OUTBOUND_DEFAULT    = -1
+DEF OUTBOUND_DONOTHING  = 0     # do nothing, just return the value of the original bpf. in this case, cropping only sets the bounds
+DEF OUTBOUND_CACHE      = 1     # cache the value of the bpf at creation time and return this value outside the bounds
+DEF OUTBOUND_SET        = 2     # set the value outside the bounds
+
+
+cpdef int _array_issorted(double[:] xs):
+    """
+    Is this array sorted?
+
+    Returns:
+        status value: -1=not sorted, 0=array is sorted, with dups, 1=array is sorted, no dups
+
+    """
+    cdef int i
+    cdef double x0, x1
+    cdef int nodups = 1
+    x1 = xs[0]
+    with nogil:
+        for i in range(1, xs.shape[0]):
+            x0 = x1
+            x1 = xs[i]
+            if x1 < x0:
+                return -1
+            elif x1 == x0:
+                nodups = 0
+    return nodups
+
+
+cdef inline int _searchsorted(double [:]xs, double x) nogil:
+    cdef int imin = 0
+    cdef int imax = xs.shape[0]
+    cdef int imid
+    while imin < imax:
+        imid = imin + ((imax - imin) >> 2)
+        if xs[imid] < x:
+            imin = imid + 1
+        else:
+            imax = imid
+    return imin
+
+
+cdef inline int _csearchlinear(DTYPE_t *xs, int xs_length, DTYPE_t x, int index) nogil:
+    # returns -1 if x is left from index
+    cdef int i = index
+    cdef double x0 = xs[i]
+    if x < x0:
+        return -1
+    cdef double x1
+    for i in range(index, xs_length-1):
+        x1 = xs[i+1]
+        if x0 <= x < x1:
+            return i
+        x0 = x1
+    return xs_length-1
+
+
+
+cdef inline int _csearchsorted(DTYPE_t *xs, int xs_length, DTYPE_t x) nogil:
+    """
+    equivalent to bisect_right. 
+    xs[out] > x
+    """
+    cdef int imin = 0
+    cdef int imax = xs_length
+    cdef int imid
+    while imin < imax:
+        imid = imin + ((imax - imin) >> 2)
+        if (<DTYPE_t *>(xs))[imid] < x:
+            imin = imid + 1
+        else:
+            imax = imid
+    return imin
+
+
+cdef inline int _csearchsorted_left(DTYPE_t *xs, int xs_length, DTYPE_t x) nogil:
+    cdef int imin = 0
+    cdef int imax = xs_length
+    cdef int imid
+    while imin < imax:
+        imid = imin + ((imax - imin) >> 2)
+        if xs[imid] <= x:
+            imin = imid + 1
+        else:
+            imax = imid
+    return imin
+
+
+cdef inline double* _seq_to_doubles(xs):
+    cdef int size, i
+    cdef double* out
+    cdef double* data
+    if isinstance(xs, ndarray):
+        size = PyArray_DIM(<ndarray>xs, 0)
+        out = <double *>malloc(sizeof(double) * size)
+        if PyArray_ISCONTIGUOUS(<ndarray>xs):
+            data = <DTYPE_t *>((<ndarray>xs).data)
+            for i in range(size):
+                out[i] = data[i]
+        else:
+            for i in range(size):
+                out[i] = xs[i]
+    else:
+        if isinstance(xs, list):
+            size = len(<list>xs)
+            out = <double *>malloc(sizeof(double) * size)
+            for i in range(size):
+                out[i] = (<list>xs)[i]
+        elif isinstance(xs, tuple):
+            size = len(<tuple>xs)
+            out = <double *>malloc(sizeof(double) * size)
+            for i in range(size):
+                out[i] = (<tuple>xs)[i]
+        else:
+            size = len(xs)
+            out = <double *>malloc(sizeof(double) * size)
+            for i in range(size):
+                out[i] = xs[i]
+    return out
+
+def _get_bounds(a, b):
+    cdef double start, end, b_start, b_end
+    start, end = a.bounds()
+    try:
+        b_start, b_end = b.bounds()
+        start = start if start < b_start else b_start
+        end = end if end > b_end else b_end
+    except:
+        pass
+    return (start, end)
+
+
+# ~~~~~~~~~~~~~~~~~~~ BpfInterface ~~~~~~~~~~~~~~~~~~~~~
+
+cdef class BpfInterface:
+    """
+    Base class for all Break-Point Functions
+
+    !!! note
+
+        BpfInterace is an abstract class. It is not possible to create 
+        an instance of it. 
+
+    """
+    cdef double _x0, _x1
+    cdef int _integration_mode  # 0: dont use scipy, 1: use scipy, -1: calibrate
+    cpdef BpfInterface _asbpf(self): return self
+    cdef void _bounds_changed(self): pass
+    
+    cdef inline void _set_bounds(self, double x0, double x1):
+        self._x0 = x0
+        self._x1 = x1
+        self._integration_mode = CONFIG['integrate.default_mode']
+    
+    cdef inline void _set_bounds_like(self, BpfInterface a):
+        self._set_bounds(a._x0, a._x1)
+    
+    cpdef double ntodx(self, int N):
+        """
+        Calculate the sampling period `dx` 
+
+        Calculate sampling period *dx* so that the bounds of 
+        this bpf are divided into *N* parts: `dx = (x1-x0) / (N-1)`.
+        The period is calculated so that lower and upper bounds are
+        included, following numpy's `linspace`
+
+        Args:
+            N (int): The number of points to sample within the bounds of
+                this bpf
+
+        Returns:
+            (float) The sampling period *dx*
+
+        !!! info "See Also"
+
+            [dxton()](#dxton)
+
+        Example
+        -------
+
+        ```python
+        >>> a = linear(0, 0, 1, 1)
+        >>> dx = a.ntodx(10)
+        >>> dx
+        0.11111111
+        >>> np.arange(a.x0, a.x1, dx)
+        array([0.        , 0.11111111, 0.22222222, 0.33333333, 0.44444444,
+       0.55555556, 0.66666667, 0.77777778, 0.88888889, 1.        ])
+
+        """
+        return (self._x1 - self._x0) / (N - 1)
+    
+    cpdef int dxton(self, double dx):
+        """
+        Split the bounds of this bpf according to a given sampling period *dx*
+
+        Args:
+            dx (float): the sampling period
+
+        Returns:
+            (int) The number of points to sample
+
+
+        Calculate the number of points in as a result of dividing the 
+        bounds of this bpf by the sampling period `dx`:
+
+            n = (x1 + dx - x0) / dx
+
+        where *x0* and *x1* are the *x* coord start and end points and *dx* 
+        is the sampling period.
+
+        ```python
+        >>> from bpf4 import *
+        >>> a = linear(0, 0, 1,  10, 2, 5)
+        # Sample a with a period of 0.1
+        >>> ys = a.map(a.dxton(0.1))
+        >>> len(ys)
+        21
+        >>> ys
+        array([ 0.,  1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.,  9., 10.,  9.,  8.,
+        7.,  6.,  5.,  4.,  3.,  2.,  1.,  0.])
+        ```
+
+        !!! info "See Also"
+
+            [ntodx()](#ntodx)
+        """
+        return <int>(((self._x1 + dx) - self._x0) / dx)
+    
+    def bounds(self):
+        """
+        Returns a tuple (xstart, xend) representing the bounds of this bpf
+
+        Returns:
+            (tuple[float, float]) The bounbs of this bpf
+
+        The returned bounds indicate the range within which this bpf is defined, but
+        any bpf can be evaluated outside those bounds. In such a case the out-of-bound
+        result will depend on the concrete subclass being evaluated. For most cases
+        the out-of-bound result is the same as the result at the bounds
+
+        ## Example
+        
+        ```python
+
+        >>> from bpf4 import *
+        >>> a = linear(1, 10, 2, 25)
+        >>> a.bounds()
+        (1.0, 2.0)
+        ```
+
+        """
+        return self._x0, self._x1
+
+    @property
+    def x0(self) -> float:
+        """The lower bound of the x coordinate"""
+        return self._x0
+    
+    
+    @property
+    def x1(self) -> float: 
+        """The upper bound of the x coordinate"""
+        return self._x1
+    
+    def __add__(a, b):
+        return _create_lambda_unordered(a, b, _BpfLambdaAdd, _BpfLambdaAddConst)
+    
+    def __sub__(a, b):
+        return _create_rlambda(a, b, _BpfLambdaSub, _BpfLambdaSubConst, _BpfLambdaRSub, _BpfLambdaRSubConst)
+    
+    def __mul__(a, b):
+        cdef float v
+        try:
+            v = float(b)  # are we a?
+            if v == 0:
+                return Const(0).set_bounds(a.x0, a.x1)
+            elif v == 1:
+                return a
+            else:
+                return _BpfLambdaMulConst(a, b, a.bounds())
+        except (TypeError, ValueError):
+            try:
+                v = float(a) # are we b?
+                if v == 0:
+                    return Const(0).set_bounds(b.x0, b.x1)
+                elif v == 1:
+                    return b
+                else:
+                    return _BpfLambdaMulConst(b, a, b.bounds())
+            except (TypeError, ValueError):
+                return _create_lambda_unordered(a, b, _BpfLambdaMul, _BpfLambdaMulConst)  # two bpfs
+    
+    def __div__(a, b):
+        cdef float v
+        try:
+            v = float(b)  # are we a?
+            if v == 0:
+                raise ZeroDivisionError("Can't divide by 0")
+            elif v == 1:
+                return a
+            else:
+                return _BpfLambdaDivConst(a, b, a.bounds())
+        except (TypeError, ValueError):
+            try:
+                v = float(a) # are we b?
+                if v == 0:
+                    return 0
+                else:
+                    return _BpfLambdaRDivConst(b, a, b.bounds())
+            except (TypeError, ValueError):
+                return _create_rlambda(a, b, _BpfLambdaDiv, _BpfLambdaDivConst, _BpfLambdaRDiv, _BpfLambdaRDivConst)
+    
+    def __truediv__(a, b):
+        return _create_rlambda(a, b, _BpfLambdaDiv, _BpfLambdaDivConst, _BpfLambdaRDiv, _BpfLambdaRDivConst)
+    
+    def __pow__(a, b, modulo):
+        cdef double tmp
+        if isinstance(a, BpfInterface):
+            if isinstance(b, BpfInterface):
+                return _BpfLambdaPow(a, b, _get_bounds(a, b))
+            elif callable(b):
+                return _BpfLambdaPow(a, _FunctionWrap(b), a.bounds())
+            elif b == 2:
+                return a*a
+            elif b == 3:
+                return a*a*a
+            elif b == 4:
+                tmp = a*a
+                return tmp*tmp
+            elif b == 0:
+                return a
+            elif b == -1:
+                return 1/a
+            elif b == -2:
+                return 1/(a*a)
+            else:
+                return _BpfLambdaPowConst(a, b, a.bounds())
+        elif isinstance(b, BpfInterface):
+            if callable(a):
+                return _BpfLambdaPow(_FunctionWrap(a), b, b.bounds())
+            return _BpfLambdaRPowConst(b, a, (INFNEG, INF))
+        return NotImplemented
+
+    def __neg__(self):
+        return self * -1
+    
+    def __mod__(self, other):
+        return _create_lambda(self, other, _BpfLambdaMod, _BpfLambdaModConst)
+    
+    def __abs__(self):
+        return self.abs()
+    
+    def __or__(a, b):
+        """
+        a | b
+        """
+        if isinstance(a, BpfInterface) and isinstance(b, BpfInterface):
+            out = _BpfCompose_new(a, b)
+        elif isinstance(a, BpfInterface) and callable(b):
+            out = _BpfCompose_new(a, _FunctionWrap(b))
+        elif callable(a) and isinstance(b, BpfInterface):
+            out = _BpfCompose_new(_FunctionWrap(b), a)
+        else:
+            return NotImplemented 
+        return out
+    
+    def __rshift__(a, b):
+        if isinstance(a, BpfInterface):
+            return a.shifted(b)
+        return NotImplemented
+
+    def __lshift__(a, b):
+        if isinstance(a, BpfInterface):
+            return a.shifted(-b)
+        return NotImplemented
+        
+    def __xor__(a, b): # ^
+        if isinstance(a, BpfInterface):
+            return a.stretched(b)
+        return NotImplemented
+
+    def __richcmp__(BpfInterface self, other, int t):
+        if t == 0:      # <
+            return _create_lambda(self, other, _BpfLambdaLowerThan, _BpfLambdaLowerThanConst)
+        elif t == 2:    # ==
+            return _create_lambda(self, other, _BpfLambdaEqual, _BpfLambdaEqualConst)
+        elif t == 4:    # >
+            return _create_lambda(self, other, _BpfLambdaGreaterThan, _BpfLambdaGreaterThanConst)
+        elif t == 1:    # <=
+            return _create_lambda(self, other, _BpfLambdaLowerOrEqualThan, _BpfLambdaLowerOrEqualThanConst)       # (self > other) == 0
+        elif t == 3:    # !=
+            return _create_lambda(self, other, _BpfLambdaUnequal, _BpfLambdaUnequalConst)
+        elif t == 5:    # >=
+            return _create_lambda(self, other, _BpfLambdaGreaterOrEqualThan, _BpfLambdaGreaterOrEqualThanConst) # (self < other) == 0
+    
+    def _get_points_for_rendering(self, int n= -1):
+        # BpfInterface
+        if n == -1:
+            n = NUM_XS_FOR_RENDERING
+        xs = numpy.linspace(self._x0, self._x1, n)
+        ys = self.mapn_between(n, self._x0, self._x1)
+        return xs, ys
+    
+    def render(self, xs, interpolation='linear'):
+        """
+        Create a new bpf representing this bpf rendered at the given points
+
+        The difference between `.render` and `.sampled` is that this method
+        creates a Linear/NoInterpol bpf whereas `.sampled` returns a 
+        `Sampled` bpf (a `Sampled` bpf works only for regularly sampled data,
+        a Linear or NoInterpol bpfs accept any data as its x coordinate)
+
+        Args:
+            xs (int | list | np.ndarray): a seq of points at which this bpf 
+                is sampled or a number, in which case an even grid is calculated 
+                with that number of points. In the first case a Linear or NoInterpol
+                bpf is returned depending on the `interpolation` parameter (see below).
+                In the second case a `Sampled` bpf is returned.
+            interpolation (str): the interpoltation type of the returned bpf. 
+                One of 'linear', 'nointerpol'
+
+        Returns:
+            (BpfInterface) a new bpf representing this bpf. Depending on the interpolation
+            this new bpf will be a Sampled, a Linear or a NoInterpol bpf
+
+        Example
+        -------
+
+        ```python
+
+        >>> from bpf4 import *
+        >>> from math import *
+        >>> a = slope(1)[0:4*pi].sin()
+        >>> b = a.render(20)   # Sample this bpf at 20 points within its bounds
+        >>> b
+        Sampled[0.0:12.566370614359172]
+        >>> b.plot()
+        ```
+        ![](assets/render1.png)
+
+        !!! info "See Also"
+
+            [BpfInterface.sampled](#sampled)
+
+        """
+        if isinstance(xs, (int, long)):
+            dx = (self._x1 - self._x0) / (xs - 1)
+            return self.sampled(dx, interpolation=interpolation)
+        else:
+            ys = self.map(xs)
+            if interpolation == 'linear':
+                return Linear(xs, ys)
+            elif interpolation == 'nointerpol':
+                return NoInterpol(xs, ys)
+            else:
+                raise ValueError("interpolation %s not implemented" % interpolation)
+
+    def plot(self, kind='line', int n=-1, show=True, axes=None, **keys):
+        """
+        Plot the bpf using matplotlib.pyplot. Any key is passed to plot.plot_coords
+
+        Args:
+            kind (str): one of 'line', 'bar'
+            n (int): the number of points to plot
+            show (bool): if the plot should be shown immediately after (default is True). 
+                If you want to display multiple BPFs sharing an axes you can call 
+                plot on each of the bpfs with show=False, and then either
+                call the last one with plot=True or call bpf4.plot.show().
+            axes (matplotlib.pyplot.Axes): if given, will be used to plot onto it,
+                otherwise an ad-hoc axes is created
+            kws: any keyword will be passed to plot.plot_coords, which is passed
+                to ``axes.plot`` (or axes.bar, etc)
+
+        Returns:
+        	the pyplot.Axes object. This will be the axes passed as argument,
+        	if given, or a new axes created for this plot
+        	 
+        ## Example
+
+        ```python
+
+        from bpf4 import *
+        a = linear(0, 0, 1, 10, 2, 0.5)
+        a.plot()
+
+        # Plot to a preexistent axes
+        ax = plt.subplot()
+        a.plot(axes=ax)
+        ```
+        """
+        xs, ys = self._get_points_for_rendering(n)
+        from . import plot
+        return plot.plot_coords(xs, ys, kind=kind, show=show, axes=axes, **keys)
+        
+    cpdef BpfInterface sampled(self, double dx, interpolation='linear'):
+        """
+        Sample this bpf at a regular interval, returns a Sampled bpf
+
+        Sample this bpf at an interval of dx (samplerate = 1 / dx)
+        returns a Sampled bpf with the given interpolation between the samples
+
+        Args:
+            dx (float): the sample interval
+            interpolation (str): the interpolation kind. One of 'linear',
+                'nointerpol', 'halfcos', 'expon(XX)', 'halfcos(XX)' (where
+                XX is an exponential passed to the interpolation function)
+
+        Returns:
+            (Sampled) The sampled bpf
+        
+        !!! note
+
+            If you need to sample a portion of the bpf, use [sampled_between](#sampled_between)
+
+        The same results can be achieved via indexing, in which case the resulting
+        bpf will be linearly interpolated:
+
+        ```python
+        bpf[::0.1]    # returns a sampled version of this bpf with a dx of 0.1
+        bpf[:10:0.1]  # samples this bpf between (x0, 10) at a dx of 0.1
+        ```
+
+        !!! info "See Also"
+
+            [ntodx](#ntodx), [dxton](#dxton)
+        """
+        # we need to account for the edge (x1 IS INCLUDED)
+        cdef int n = int((self._x1 - self._x0) / dx + 0.5) + 1
+        ys = self.mapn_between(n, self._x0, self._x1) 
+        return Sampled(ys, dx=dx, x0=self._x0, interpolation=interpolation)
+    
+    cpdef ndarray sample_between(self, double x0, double x1, double dx, ndarray out=None):
+        """
+        Sample this bpf at an interval of dx between x0 and x1 
+
+        !!! note
+
+            The interface is similar to numpy's `linspace`
+        
+        Args:
+            x0 (float): point to start sampling (included)
+            x1 (float): point to stop sampling (included)
+            dx (float): the sampling period
+            out (ndarray): if given, the result will be placed here and no new array will
+                be allocated
+
+        Returns:
+            (ndarray) An array with the values of this bpf sampled at at a regular grid of 
+            period `dx` from `x0` to `x1`. If out is given the result is placed in it
+
+        ## Example
+        
+        ```python
+        
+        >>> a = linear(0, 0, 10, 10)
+        >>> a.sample_between(0, 10, 1)
+        [0 1 2 3 4 5 6 7 8 9 10]
+        ```
+        
+        This is the same as `a.mapn_between(11, 0, 10)`
+        """
+        cdef int n
+        n = int((x1 - x0) / dx + 0.5) + 1
+        return self.mapn_between(n, x0, x1, out)
+    
+    cpdef BpfInterface sampled_between(self, double x0, double x1, double dx, interpolation='linear'):
+        """
+        Sample a portion of this bpf, returns a `Sampled` bpf
+
+        **NB**: This is the same as `thisbpf[x0:x1:dx]`
+        
+        Args:
+            x0 (float): point to start sampling (included)
+            x1 (float): point to stop sampling (included)
+            dx (float): the sampling period
+            interpolation (str): the interpolation kind. One of 'linear',
+                'nointerpol', 'halfcos', 'expon(XX)', 'halfcos(XX)' (where
+                XX is an exponential passed to the interpolation function). For 
+                example: 'expon(2.0)' or 'halfcos(0.5)'
+        
+        Returns:
+            (Sampled) The `Sampled` bpf, representing this bpf sampled at a grid of `[x0:x1:dx]`
+            with the given interpolation
+
+        """
+        cdef int n = int((x1 - x0) / dx + 0.5) + 1
+        ys = self.mapn_between(n, x0, x1)
+        return Sampled(ys, dx=dx, x0=x0, interpolation=interpolation)
+
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        """
+        Calculate an array of `n` values representing this bpf between `x0` and `x1`
+
+        Args:
+            x0 (float): lower bound to map this bpf
+            x1 (float): upper bound to map this bpf
+            out (ndarray): if included, results are placed here. 
+
+        Returns:
+            (ndarray) An array of `n` elements representing this bpf at the given 
+            values within the range `x0:x1`. This is `out` if it was passed 
+
+        x0 and x1 are included
+
+        Example
+        =======
+
+        ```python
+        
+        out = numpy.empty((100,), dtype=float)
+        out = thisbpf.mapn_between(100, 0, 10, out)
+        
+        ```
+        """
+        cdef double[::1] result = out if out is not None else EMPTY1D(n)
+        cdef double dx = _ntodx(n, x0, x1)
+        cdef size_t i
+        cdef double x
+        for i in range(n):
+            x = x0 + i*dx
+            result[i] = self.__ccall__(x)
+        return numpy.asarray(result)
+
+    cpdef ndarray map(self, xs, ndarray out=None):
+        """
+        The same as map(self, xs) but faster
+
+        Args:
+            xs (ndarray | int): the x coordinates at which to sample this bpf,
+                or an integer representing the number of elements to calculate
+                in an evenly spaced grid between the bounds of this bpf
+            out (ndarray): if given, an attempt will be done to use it as destination
+                for the result. The user should not trust that this actually happens
+                (see example)
+
+        ```python
+
+        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
+        ```
+
+        ## Example
+        
+        ```python
+
+        >>> out = numpy.empty((100,), dtype=float)
+        >>> xs = numpy.linspace(0, 10, 100)
+        # This is the right way to pass an output array
+        >>> out = thisbpf.map(xs, out)   
+        
+        ```
+        """
+        if isinstance(xs, int):
+            return self.mapn_between(xs, self._x0, self._x1, out)
+        
+        cdef double[::1] _xs = <ndarray>xs if isinstance(xs, ndarray) else numpy.asarray(xs)
+        cdef int nx  = len(_xs)
+        cdef double[::1] result = out if out is not None else EMPTY1D(nx)
+        cdef int i
+        cdef double x0,x1, dx
+        with nogil:
+            for i in range(nx):
+                result[i] = self.__ccall__(_xs[i])
+        return numpy.asarray(result)
+    
+    cpdef BpfInterface concat(self, BpfInterface other):
+        """
+        Concatenate this bpf to other
+
+        `other` is shifted to start at the end of `self`
+
+        ## Example
+        
+        ```python
+
+        >>> a = linear(0, 0, 1, 10)
+        >>> b = linear(3, 100, 10, 200)
+        >>> c = a.concat(b)
+        >>> c
+        _BpfConcat2[0.0:8.0]
+        >>> c(1 - 1e-12), c(1)
+        (9.99999999999, 100.0)
+        >>> c.plot()
+        ```
+        ![](assets/concat1.png)
+
+        """
+        cdef BpfInterface other2 = other.fit_between(self._x1, self._x1 + (other._x1 - other._x0))
+        return _BpfConcat2_new(self, other2, other2._x0)
+        
+    cpdef _BpfLambdaRound round(self):
+        """
+        A bpf representing round(self(x))
+
+        Returns:
+            (BpfInterface) A bpf representing the operation `round(self(x))`
+        """
+        return _BpfLambdaRound(self)
+
+    cpdef _BpfRand rand(self):
+        """
+        A bpf representing rand(self(x))
+
+        Returns:
+            (BpfInterface) A bpf representing the operation ``rand(self(x))`
+        """
+        return _BpfRand(self)
+    
+    cpdef _BpfUnaryFunc cos(self):  
+        """
+        Returns a bpf representing the cosine of this bpf
+
+        ```python
+        from bpf4 import *
+        from math import pi
+        a = slope(1).cos()
+        a[0:8*pi].plot()
+        ```
+        ![](assets/cos.png)
+        """
+        return _BpfUnaryFunc_new_from_index(self, 0)
+    
+    cpdef _BpfUnaryFunc sin(self):  
+        """Returns a bpf representing the sine of this bpf
+
+        ```
+        from bpf4 import *
+        from math import pi
+        a = slope(1).sin()
+        a[0:8*pi].plot()
+        ```
+        ![](assets/sin.png)
+        """    
+        return _BpfUnaryFunc_new_from_index(self, 1)
+    
+    cpdef _BpfUnaryFunc ceil(self): 
+        """Returns a bpf representing the ceil of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 2)
+    
+    cpdef _BpfUnaryFunc expon(self):
+        """Returns a bpf representing the exp operation with this bpf
+
+        ## Example
+
+        ```python
+
+        >>> from bpf4 import *
+        >>> a = linear(0, 0, 1, 10)
+        >>> a(0.1)
+        1.0
+        >>> exp(1.0)
+        2.718281828459045
+        >>> a.expon()(0.1)
+        2.718281828459045
+        ```
+        """
+        return _BpfUnaryFunc_new_from_index(self, 4)
+    
+    cpdef _BpfUnaryFunc floor(self): 
+        """Returns a bpf representing the floor of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 5)
+    
+    cpdef _BpfUnaryFunc tanh(self): 
+        """Returns a bpf representing the tanh of this bpf
+
+        ```python
+        from bpf4 import *
+        a = slope(1).tanh()
+        a[-4:4].plot()
+        ```
+        ![](assets/tanh.png)
+        """
+        return _BpfUnaryFunc_new_from_index(self, 6)
+    
+    cpdef _BpfUnaryFunc abs(self):  
+        """Returns a bpf representing the absolute value of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 7)
+    
+    cpdef _BpfUnaryFunc sqrt(self): 
+        """Returns a bpf representing the sqrt of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 8)
+    
+    cpdef _BpfUnaryFunc acos(self): 
+        """Returns a bpf representing the arc cosine of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 9)
+    
+    cpdef _BpfUnaryFunc asin(self): 
+        """Returns a bpf representing the arc sine of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 10)
+    
+    cpdef _BpfUnaryFunc tan(self):  
+        """Returns a bpf representing the tan of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 11)
+    
+    cpdef _BpfUnaryFunc sinh(self): 
+        """Returns a bpf representing the sinh of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 12)
+    
+    cpdef _BpfUnaryFunc log10(self): 
+        """Returns a bpf representing the log10 of this bpf"""
+        return _BpfUnaryFunc_new_from_index(self, 13)
+    
+    cpdef _BpfLambdaLog log(self, double base=M_E): 
+        """
+        Returns a bpf representing the log of this bpf
+
+        Args:
+            base (float): the base of the log
+
+        Returns:
+            (BpfInterface) A bpf representing `\\x -> log(self(x), base)`
+
+        """
+        return _BpfLambdaLog(self, base, self.bounds())
+    
+    cpdef _BpfM2F m2f(self):
+        """Returns a bpf converting from midinotes to frequency
+
+        Returns:
+            (BpfInterface) A bpf representing `\\x -> m2f(self(x))`
+
+        ## Example
+
+        ```python
+        >>> from bpf4 import *
+        >>> midinotes = linear(0, 60, 1, 65)
+        >>> freqs = midinotes.m2f()
+        >>> freqs.map(10)
+        array([262.81477242, 271.38531671, 280.23535149, 289.37399111,
+               298.81064715, 308.55503809, 318.61719934, 329.0074936 ,
+               339.73662146, 350.81563248])
+        ```
+        """
+        return _BpfM2F(self)
+    
+    cpdef _BpfF2M f2m(self): 
+        """Returns a bpf converting frequencies to midinotes
+        
+        Returns:
+            (BpfInterface) A bpf representing `\\x -> f2m(self(x))`
+
+        ## Example
+        
+        ```python
+        >>> from bpf4 import *
+        >>> freqs = linear(0, 442, 1, 882)
+        >>> freqs.f2m().map(10)
+        array([69.        , 70.82403712, 72.47407941, 73.98044999, 75.3661766 ,
+               76.64915905, 77.84358713, 78.96089998, 80.01045408, 81.        ])
+        ```
+        """
+        return _BpfF2M(self)
+    
+    cpdef _Bpf_db2amp db2amp(self): 
+        """
+        Returns a bpf converting decibels to linear amplitudes
+
+        Returns:
+            (BpfInterface) A bpf representing `\\x -> db2amp(self(x))`
+
+        ## Example
+
+        ```python
+        >>> linear(0, 0, 1, -60).db2amp().map(10)
+        array([1.        , 0.46415888, 0.21544347, 0.1       , 0.04641589,
+               0.02154435, 0.01      , 0.00464159, 0.00215443, 0.001     ])
+        ```
+        """
+        return _Bpf_db2amp(self)
+    
+    cpdef _Bpf_amp2db amp2db(self):
+        """
+        Returns a bpf converting linear amplitudes to decibels
+
+        Returns:
+            (BpfInterface) A bpf representing `\\x -> amp2db(self(x))`
+
+        ## Example
+
+        ```python
+        >>> linear(0, 0, 1, 1).amp2db().map(10)
+        array([-280.        ,  -19.08485019,  -13.06425028,   -9.54242509,
+               -7.04365036,   -5.1054501 ,   -3.52182518,   -2.18288939,
+               -1.02305045,    0.        ])
+        ```
+        """    
+        return _Bpf_amp2db(self)
+    
+    cpdef _BpfLambdaClip clip(self, double y0=INFNEG, double y1=INF): 
+        """
+        Return a bpf clipping the result between y0 and y1
+
+        Args:
+            y0 (float): the min. *y* value
+            y1 (float): the max. *y* value
+
+        Returns:
+            (BpfInterface) A view of this bpf clipped to the given
+            *y* values
+
+        ```python
+
+        >>> a = linear(0, -1, 1, 1).clip(0, 1)
+        >>> a.map(20)
+        array([0.        , 0.        , 0.        , 0.        , 0.        ,
+               0.        , 0.        , 0.        , 0.        , 0.        ,
+               0.05263158, 0.15789474, 0.26315789, 0.36842105, 0.47368421,
+               0.57894737, 0.68421053, 0.78947368, 0.89473684, 1.        ])
+        >>> a.plot()
+        ```
+        ![](assets/clip1.png)
+        """
+        return _BpfLambdaClip_new(self, y0, y1)
+
+    cpdef BpfInterface derivative(self):
+        """
+        Create a curve which represents the derivative of this curve
+
+        Returns:
+            (BpfInterface) A bpf which returns the derivative of this 
+            bpf at any given x coord
+
+        It implements Newtons difference quotiont, so that:
+
+        ```
+
+                        bpf(x + h) - bpf(x)
+        derivative(x) = -------------------
+                                  h
+        ```
+
+        Example
+        -------
+
+        ```python
+        
+        >>> from bpf4 import *
+        >>> a = slope(1)[0:6.28].sin()
+        >>> a.plot(show=False, color="red")
+        >>> b = a.derivative()
+        >>> b.plot(color="blue")
+
+        ```
+        ![](assets/derivative1.png)
+        """
+        return _BpfDeriv(self)
+
+    cpdef BpfInterface integrated(self):
+        """
+        Return a bpf representing the integration of this bpf at a given point
+
+        Returns:
+            (BpfInterface) A bpf representing the integration of this bpf
+
+        Example
+        -------
+
+        ```python
+        a = linear(0, 0, 5, 5)
+        b = a.integrated()
+        a.plot(show=False, color="red")
+        b.plot(color="blue")
+        ```
+        ![](assets/integrated1.png)
+
+        !!! info "See Also"
+
+            * [.integrate](#integrate)
+        """
+
+        if self._x0 == INFNEG:
+            raise ValueError("Cannot integrate a function with an infinite negative bound")
+        return _BpfIntegrate(self)
+    
+    cpdef double integrate(self):
+        """
+        Return the result of the integration of this bpf. 
+
+        If any of the bounds is `inf`, the result is also `inf`.
+
+        !!! note
+
+            To set the bounds of the integration, first crop the bpf by slicing it: `bpf[start:end]`
+        
+        Returns:
+            (float) The result of the integration
+
+        ## Example
+
+        ```python
+
+        >>> linear(0, 0, 10, 10).sin()[0:2*pi].integrate()
+        -1.7099295055304798e-17
+        
+        ```
+        """
+        if isinf(self._x0) or isinf(self._x1):
+            return INFINITY
+        return self.integrate_between(self._x0, self._x1)
+    
+    cdef double _trapz_integrate_between(self, double x0, double x1, size_t N=0):
+        """
+        Integrate this bpf between [x0, x1] using the traptz method
+
+        Args:
+            x0 (float): start of integration period
+            x1 (float): end of the integration period
+            N (int): number of subdivisions used to calculate the integral. If not given, 
+               a default is used (default defined in `CONFIG['integrate.trapz_intervals']`)
+
+        Returns:
+            (float) The result of the integration
+        """
+        cdef:
+            double dx
+            double [::1] ys
+        if N == 0:
+            N = CONFIG['integrate.trapz_intervals']
+        dx = (x1 - x0) / N
+        if dx <= 0:
+            return 0.0
+        ys = self.sample_between(x0, x1, dx)
+        return _integr_trapz(&ys[0], ys.shape[0], dx)
+    
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        """
+        Integrate this bpf between x0 and x1
+
+        Args:
+            x0: start x of the integration range
+            x1: end x of the integration range
+            N: number of intervals to use for integration
+
+        Returns:
+            (float) The result of the integration
+        """
+
+        cdef double out
+        cdef int get_mode
+        cdef int mode = self._integration_mode
+        cdef double outbound0, outbound1, inbound
+        if x1 > self._x1:
+            outbound1 = self.__ccall__(x1) * (x1 - self._x1)
+            x1 = self._x1
+        else:
+            outbound1 = 0
+        if x0 < self._x0:
+            outbound0 = self.__ccall__(x0) * (self._x0 - x0)
+            x0 = self._x0
+        else:
+            outbound0 = 0
+        # override mode when N is given
+        if N > 0:
+            mode = 0
+        if mode == 1 or mode == 2:
+            inbound = integrate_simpsons(self, x0, x1, SIMPSONS_ACCURACY, SIMPSONS_MAXITER)
+        else:
+            inbound = self._trapz_integrate_between(x0, x1, N)
+        return outbound0 + inbound + outbound1
+
+    cpdef double mean(self):
+        """
+        Calculate the mean value of this bpf. 
+
+        Returns:
+            (float) The average value of this bpf along its bounds
+
+        To constrain the calculation to a given portion, use:
+
+        ```python
+
+        bpf.integrate_between(start, end) / (end-start)
+        
+        ```
+        """
+        return self.integrate() / (self._x1 - self._x0)
+
+    cpdef list zeros(self, double h=0.01, int N=0, double x0=NAN, double x1=NAN, int maxzeros=0):
+        """
+        Find the zeros of this bpf
+        
+        Args:
+            h: the accuracy to scan for zero-crossings. If two zeros are within 
+                this distance, they will be resolved as one.
+            N: alternatively, you can give the number of intervals to scan. 
+                h will be derived from this
+            x0: the point to start searching. If not given, the starting point of this bpf
+                will be used
+            x1: the point to stop searching. If not given, the end point of this bpf is used
+            maxzeros: if > 0, stop the search when this number of zeros have been found
+            
+        Returns:
+            (List[float]) A list with the zeros of this bpf
+
+
+        ## Example
+        
+        ```python
+        
+        >>> a = bpf.linear(0, -1, 1, 1)
+        >>> a.zeros()
+        [0.5]
+        
+        ```
+
+        """
+        return bpf_zero_crossings(self, h=h, N=N, x0=x0, x1=x1, maxzeros=maxzeros)
+
+    def max(self, b):
+        """
+        Returns a bpf representing `max(self, b)`
+
+        Args:
+            b (float | BpfInterface): a const float or a bpf
+
+        Returns:
+            (Max) A Max bpf representing `max(self, b)`, which can be
+            evaluated at any x coord
+        
+        ## Example
+        
+        ```python
+        >>> from bpf4 import *
+        >>> a = linear(0, 0, 1, 10)
+        >>> b = a.max(4)
+        >>> b(0), b(0.5), b(1)
+        (4.0, 5.0, 10.0)
+        >>> b.plot()
+        ```
+        ![](assets/maxconst.png)
+        """
+        
+        if isinstance(b, BpfInterface):
+            return Max(self, b)
+        return _BpfMaxConst(self, b, self.bounds())
+
+    def min(self, b):
+        """
+        Returns a bpf representing `min(self, b)`
+
+        Args:
+            b (float | BpfInterface): a const float or a bpf
+
+        Returns:
+            (Min) A Min bpf representing `min(self, b)`, which can be
+            evaluated at any x coord
+        
+        ## Example
+        
+        ```python
+        >>> from bpf4 import *
+        >>> a = linear(0, 0, 1, 10)
+        >>> b = a.min(4)
+        >>> b(0), b(0.5), b(1)
+        (0, 4.0, 5.0)
+        >>> b.plot()
+        ```
+        ![](assets/minconst.png)
+        """
+        if isinstance(b, BpfInterface):
+            return Min(self, b)
+        return _BpfMinConst(self, b, self.bounds())
+
+    def __reduce__(self):
+        return type(self), self.__getstate__()
+
+    cdef double __ccall__(self, double other) nogil:
+        return 0.0
+
+    def __call__(BpfInterface self, double x):
+        """
+        BpfInterface.__call__(self, double x)
+
+        Args:
+            x (float): evaluate this bpf at the given x coord
+
+        Returns:
+            (float) The value of this bpf at x
+        """
+        return self.__ccall__(x)
+
+    def keep_slope(self, double epsilon=DEFAULT_EPSILON):
+        """
+        A view of this bpf where the slope is continued outside its bounds
+
+
+        Return a new bpf which is a copy of this bpf when inside
+        bounds() but outside bounds() it behaves as a linear bpf
+        with a slope equal to the slope of this bpf at its extremes
+        
+        Args:
+            epsilon (float): an epsilon value to use when deriving the
+                this bpf to calculate its slope
+
+        Returns:
+            (BpfInterface) A view of this bpf which keeps its slope outside
+            its bounds (instead of just returning the last defined value)
+
+        Example
+        -------
+
+        ```python
+
+        a = expon(1, 1, 2, 2, exp=2)
+        b = a.keep_slope()
+        b[0:3].plot(show=False, color="grey")
+        a.plot(color="black", linewidth=3)
+        ```
+        ![](assets/keepslope1.png)
+        """
+        return _BpfKeepSlope(self, epsilon)
+
+    def outbound(self, double y0, double y1):
+        """
+        Return a new Bpf with the given values outside the bounds
+
+        ## Examples
+        
+        ```python
+
+        >>> from bpf4 import *
+        >>> a = linear(0, 1, 1, 10).outbound(-1, 0)
+        >>> a(-0.5)
+        -1
+        >>> a(1.1)
+        0
+        >>> a(0)
+        1
+        >>> a(1)
+        10
+
+        # fallback to another curve outside self
+        >>> a = linear(0, 1, 1, 10).outbound(0, 0) + expon(-1, 2, 4, 10, exp=2)
+        >>> a.plot()
+        ```
+        ![](assets/outbound1.png)
+        """
+        return _BpfCrop_new(self, self._x0, self._x1, OUTBOUND_SET, y0, y1)
+
+    def apply(self, func):
+        """
+        Create a bpf where `func` is applied to the result of this pdf
+        
+        Args:
+            func (callable): a function to apply to the result of this bpf
+
+        Returns:
+            (BpfInterface) A bpf representing `func(self(x))` 
+
+        **NB**: `a.apply(b)` is the same as `a | b`
+        
+        ## Example
+        
+        ```python
+
+        >>> from bpf4 import *
+        >>> from math import *
+        >>> a = linear(0, 0, 1, 10)
+        >>> def func(x):
+        ...     return sin(x) + 1
+        >>> b = a.apply(func)
+        >>> b(1)
+        0.4559788891106302
+        >>> sin(a(1)) + 1
+        0.4559788891106302
+        
+        ```
+
+        """
+        return _BpfCompose_new(self, _FunctionWrap(func))
+
+    def preapply(self, func):
+        """
+        Create a bpf where `func` is applied to the argument before it is passed
+
+        This is equivalent to `func(x) | self`
+        
+        Args:
+            func (callable): a function `func(x: float) -> float` which is applied to
+                the argument before passing it to this bpf
+
+        Returns:
+            (BpfInterface) A bpf following the pattern `lambda x: bpf(func(x))`
+
+        ## Example
+        
+        ```python
+
+        >>> bpf = Linear((0, 1, 2), (0, 10, 20))
+        >>> bpf(0.5)
+        5
+
+        >>> shifted_bpf = bpf.preapply(lambda x: x + 1)
+        >>> shifted_bpf(0.5)
+        15
+        ```
+
+        **NB**: `bpf1.preapply(bpf2)` is the same as `bpf2 | bpf1`
+        """
+        return _BpfCompose_new(_FunctionWrap(func), self)
+
+    def periodic(self):
+        """
+        Create a new bpf which replicates this in a periodic way
+
+        Returns:
+            (BpfInterface) A periodic view of this bpf
+
+        The new bpf is a copy of this bpf when inside its bounds 
+        and outside it, it replicates it in a periodic way, with no bounds.
+
+        ## Example
+            
+        ```python
+
+        >>> from bpf4 import *
+        >>> a = core.Linear((0, 1), (-1, 1)).periodic()
+        >>> a
+        _BpfPeriodic[-inf:inf]
+        >>> a.plot()
+        ```
+        ![](assets/periodic1.png)
+        """
+        return _BpfPeriodic(self)
+
+    def stretched(self, double rx, double fixpoint=0.):
+        """
+        Returns a view of this bpf stretched over the x axis. 
+
+        **NB**: to stretch over the y-axis, just multiply this bpf
+        
+        !!! info "See Also"
+
+            [fit_between()](#fit_between)
+
+        Args:
+            rx (float): the stretch factor
+            fixpoint (float): the point to use as reference
+
+        Returns:
+            (BpfInterface) A projection of this bpf stretched/compressed by
+            by the given factor
+
+        ## Example
+
+        Stretch the shape of the bpf, but preserve the start position
+        
+        ```python
+            
+        >>> a = linear(1, 1, 2, 2)
+        >>> b = a.stretched(4, fixpoint=a.x0)
+        >>> b.bounds()
+        (1, 9)
+        >>> a.plot(show=False); b.plot()
+
+        ```
+        """
+        if rx == 0:
+            raise ValueError("the stretch factor cannot be 0")
+        
+        if self._x0 == INF or self._x0 == INFNEG or self._x1 == INF or self._x1 == INFNEG:
+            qrx = 1/rx
+            return _BpfProjection(rx=qrx, dx=0, offset=fixpoint)
+        
+        cdef double x0 = self._x0
+        cdef double x1 = self._x1
+        cdef double p0 = (x0 - fixpoint)*rx + fixpoint
+        cdef double p1 = (x1 - x0) * rx + p0
+        return self.fit_between(p0, p1)
+        
+    cpdef BpfInterface fit_between(self, double x0, double x1):
+        """
+        Returns a view of this bpf fitted within the interval `x0:x1`
+
+        This operation only makes sense if the bpf is bounded
+        (none of its bounds is `inf`)
+
+        Args:
+            x0: the lower bound to fit this bpf
+            x1: the upper bound to fit this bpf
+
+        Returns:
+            (BpfInterface) The projected bpf
+
+        ## Example
+        
+        ```python
+
+        >>> from bpf4 import *
+        >>> a = linear(1, 1, 2, 5)
+        >>> a.bounds()
+        (1, 5)
+        >>> b = a.fit_between(0, 10)
+        >>> b.bounds()
+        0, 10
+        >>> b(10)
+        5
+        ```
+        """
+        cdef double rx
+        if self._x0 == INF or self._x0 == INFNEG or self._x1 == INF or self._x1 == INFNEG:
+            raise ValueError("This bpf is unbounded, cannot be fitted."
+                             "Use thisbpf[x0:x1].fit_between(...)")
+        rx = (self._x1 - self._x0) / (x1 - x0)
+        dx = self._x0
+        offset = x0
+        return _BpfProjection(self, rx=rx, dx=dx, offset=offset)
+
+
+    cpdef BpfInterface shifted(self, dx):
+        """
+        Returns a view of this bpf shifted by `dx` over the x-axes
+
+        This is the same as [.shift](#shift), but a new bpf is returned
+
+        ## Example
+        
+        ```python
+
+        >>> from bpf4 import *
+        >>> a = linear(0, 1, 1, 5)
+        >>> b = a.shifted(2)
+        >>> b(3) == a(1)
+        ```
+        """
+        return _BpfProjection(self, rx=1, dx=-dx)
+
+    def inverted(self):
+        """
+        Return a view on this bpf with the coords inverted
+
+        Returns:
+            (BpfInterface) a view on this bpf with the coords inverted
+
+        In an inverted function the coordinates are swaped: the inverted version of a 
+        bpf indicates which *x* corresponds to a given *y*
+        
+        Returns None if the function is not invertible. For a function to be invertible, 
+        it must be strictly increasing or decreasing, with no local maxima or minima.
+        
+        ```
+        f.inverted()(f(x)) = x
+        ```
+        
+        So if `y(1) == 2`, then `y.inverted()(2) == 1`
+
+        ![](assets/inverted.png)
+        """
+        try:
+            return _BpfInverted(self)
+        except ValueError:
+            return None
+
+    cpdef BpfInterface _slice(self, double x0, double x1):
+        return _BpfCrop_new(self, x0, x1, OUTBOUND_DEFAULT, 0, 0)
+
+    def __getitem__(self, slice):
+        cdef double x0, x1
+        cdef BpfInterface out
+        x0 = self._x0
+        x1 = self._x1
+        try:
+            if slice.start is not None:
+                x0 = slice.start
+            if slice.stop is not None:
+                x1 = slice.stop
+            if slice.step is not None:
+                return self.sampled_between(x0, x1, slice.step, 'linear')
+            return self._slice(x0, x1)
+        except AttributeError:
+            raise ValueError("BPFs accept only slices, not single items.")
+    
+    @classmethod
+    def fromseq(cls, *points, **kws):
+        """
+        A helper constructor with points given as tuples or as a flat sequence. 
+
+        ## Example
+
+        These operations result in the same bpf:
+
+        ```python
+        Linear.fromseq(x0, y0, x1, y1, x2, y2, ...)
+        Linear.fromseq((x0, y0), (x1, y1), (x2, y2), ...)
+        Linear((x0, x1, ...), (y0, y1, ...))
+        ```
+
+        Args:
+            points (ndarray | list[float]): either the interleaved x and y points, or each point as a
+                2D tuple
+            `**kws` (dict): any keyword will be passed to the default constructor (for 
+                example, `exp` in the case of an `Expon` bpf)
+
+        Returns:
+            (BpfBase) The constructed bpf
+        """
+        cdef ndarray data
+        cdef int lenpoints
+        if isinstance(points[0], (list, tuple)):
+            # (x0, y0), (x1, y1), ...
+            data = numpy.asarray(points, dtype=DTYPE)
+            return cls(data[:,0], data[:,1], **kws)
+        else:
+            # x0, y0, x1, y1, ...
+            lenpoints = len(points)
+            if lenpoints % 2 != 0:
+                raise ValueError(
+                    "The instantiation form x0, y0, x1, y1 should have an even number of args"
+                )
+            if lenpoints == 2:
+                return cls((points[0], points[1]), (points[0], points[1]), **kws)
+            elif lenpoints == 1:
+                return cls((0, 0), (0, points[0]), **kws)
+            else:
+                return cls(points[::2], points[1::2], **kws)
+
+    def copy(self):
+        """
+        Create a copy of this bpf
+
+        Returns:
+            (BpfInterface) A copy of this bpf
+        """
+        state = self.__getstate__()
+        obj = self.__class__(*state)
+        obj.__setstate__(state)
+        return obj
+    
+    def __repr__(self):
+        x0, x1 = self.bounds()
+        return "%s[%s:%s]" % (self.__class__.__name__, str(x0), str(x1))
+
+    
+
+cdef BpfInterface _asbpf(obj):
+    if isinstance(obj, BpfInterface):
+        return obj
+    if hasattr(obj, '__call__'):
+        return _FunctionWrap(obj, (INFNEG, INF))
+    elif hasattr(obj, '__float__'):
+        return Const(float(obj))
+    else:
+        return None
+
+   
+cdef inline ndarray _asarray(obj): 
+    return <ndarray>(PyArray_GETCONTIGUOUS(array(obj, DTYPE, False)))
+
+
+cdef class BpfBase(BpfInterface):
+    cdef ndarray xs, ys
+    cdef DTYPE_t* xs_data
+    cdef DTYPE_t* ys_data
+    cdef int outbound_mode
+    cdef double outbound0, outbound1
+    cdef double lastbin_x0, lastbin_x1
+    cdef InterpolFunc *interpol_func
+    cdef Py_ssize_t xs_size
+    cdef size_t lastbin_idx1
+
+
+    def __cinit__(self):
+        self.interpol_func = NULL
+        self.ys_data = NULL
+        self.xs_data = NULL
+        self.xs = None
+        self.ys = None
+
+    def __dealloc__(self):
+        InterpolFunc_free(self.interpol_func)
+
+    def __init__(BpfBase self, xs, ys):
+        """
+        Base constructor for bpfs
+
+        xs and ys should be of the same size
+
+        Args:
+            xs (list[float] | numpy.ndarray): x data 
+            ys (list[float] | numpy.ndarray): y data
+
+
+        """
+        cdef int len_xs, len_ys
+        cdef ndarray [DTYPE_t, ndim=1] _xs = numpy.ascontiguousarray(xs, DTYPE)
+        if _array_issorted(_xs) == -1:
+            raise BpfPointsError(f"Points along the x coord should be sorted\nxs: \n{xs}")
+        cdef ndarray [DTYPE_t, ndim=1] _ys = numpy.ascontiguousarray(ys, DTYPE)
+        len_xs = PyArray_DIM(_xs, 0)
+        len_ys = PyArray_DIM(_ys, 0)
+        if len_xs != len_ys:
+            raise ValueError("xs and ys must be of equal length, but xs has %d items "
+                             "and ys has %d items" % (len_xs, len_ys))
+        if len_xs < 1:
+            raise ValueError("Can't creat a BPF of 0 points")
+        self.xs = _xs
+        self.ys = _ys
+        self.xs_size = PyArray_DIM(_xs, 0)
+        self._set_bounds(_xs[0], _xs[len_xs - 1])
+        self.outbound_mode = OUTBOUND_CACHE
+        self.outbound0 = _ys[0]
+        self.outbound1 = _ys[len_ys - 1]
+        self.xs_data = <DTYPE_t*>(self.xs.data)
+        self.ys_data = <DTYPE_t*>(self.ys.data)
+        self.lastbin_x0 = self.xs[0]
+        self.lastbin_x1 = self.xs[1]
+        self.lastbin_idx1 = 1
+
+    @property
+    def descriptor(self) -> str: 
+        """
+        A string describing the interpolation function of this bpf
+        """
+        return InterpolFunc_get_descriptor(self.interpol_func)
+
+    cdef void _bounds_changed(self):
+        self._invalidate_cache()
+
+    cdef void _invalidate_cache(self):
+        cdef int last_index = PyArray_DIM(self.xs, 0) - 1
+        self.lastbin_x0 = 0
+        self.lastbin_x1 = 0
+        self.lastbin_idx1 = 0
+        if self.ys_data != NULL and self.outbound_mode == OUTBOUND_CACHE:
+            self.outbound0 = (<DTYPE_t *>(self.ys_data))[0]
+            self.outbound1 = (<DTYPE_t *>(self.ys_data))[last_index]
+        
+    def outbound(self, double y0, double y1):
+        """
+        Set the values **inplace** returned when this bpf is evaluated outside its bounds.
+
+        The default behaviour is to interpret the values at the bounds to extend to infinity.
+
+        In order to not change this bpf inplace, use `b.copy().outbound(y0, y1)`
+        """
+        self.outbound_mode = OUTBOUND_SET
+        self.outbound0 = y0
+        self.outbound1 = y1
+        return self
+
+    def __getstate__(self):
+        return (self.xs, self.ys)
+
+    def __setstate__(self, state):
+        self.xs, self.ys = state
+
+    cdef double __ccall__(BpfBase self, double x) nogil:
+        cdef double res, x0, y0, x1, y1
+        cdef int index0, index1, nx
+        if self.lastbin_x0 <= x < self.lastbin_x1:
+            res = InterpolFunc_call(self.interpol_func, x, self.lastbin_x0, self.ys_data[self.lastbin_idx1-1], 
+                                    self.lastbin_x1, self.ys_data[self.lastbin_idx1])
+        elif x < self._x0:
+            res = self.outbound0
+        elif x > self._x1:
+            res = self.outbound1
+        elif (self.lastbin_idx1 < self.xs_size - 2) and (self.lastbin_x1 <= x < self.xs_data[self.lastbin_idx1+1]):
+            # usual situation: cross to next bin
+            index1 = self.lastbin_idx1 + 1
+            x1 = self.xs_data[index1]
+            res = InterpolFunc_call(self.interpol_func, x, self.lastbin_x1, self.ys_data[index1-1], x1, self.ys_data[index1])
+            self.lastbin_x0 = self.lastbin_x1
+            self.lastbin_x1 = x1
+            self.lastbin_idx1 = index1
+        else:
+            # out of cache call, find new boundaries and update cache
+            index1 = _csearchsorted(self.xs_data, self.xs_size, x)
+            x0 = self.xs_data[index1-1]
+            x1 = self.xs_data[index1]
+            res = InterpolFunc_call(self.interpol_func, x, x0, self.ys_data[index1-1], x1, self.ys_data[index1])
+            self.lastbin_x0 = x0
+            self.lastbin_x1 = x1
+            self.lastbin_idx1 = index1
+        return res
+
+    cpdef ndarray mapn_between(self, int n, double xstart, double xend, ndarray out=None):
+        cdef double[::1] result = out if out is not None else EMPTY1D(n)
+        cdef double dx = _ntodx(n, xstart, xend)
+        cdef double x = xstart, y
+        cdef size_t i = 0, j
+        cdef double outbound1 = self.outbound1
+        cdef double outbound0 = self.outbound0
+        cdef DTYPE_t *xs_data = self.xs_data
+        cdef DTYPE_t *ys_data = self.ys_data
+        cdef double xs_data0, xs_data1, ys_data0, ys_data1
+        cdef double x1 = self._x1
+        cdef int64_t index0 = 0
+        cdef double interpmix = self.interpol_func.mix
+        with nogil:
+            if xstart < self._x0:
+                j = min(n, <int>((self._x0 - xstart) / dx) + 1)
+                for i in range(j):
+                    result[i] = outbound0
+                i = j
+            x = xstart + i*dx
+            if self._x0 <= x <= self._x1:
+                index0 = _csearchsorted(self.xs_data, self.xs_size, x) - 1
+            elif x > self._x1:
+                for j in range(i, n):
+                    result[j] = outbound1
+                i = n
+                
+            xs_data0 = xs_data[index0]
+            xs_data1 = xs_data[index0+1]
+            ys_data0 = ys_data[index0]
+            ys_data1 = ys_data[index0+1]
+            while x <= x1 and i < n:
+                if x > xs_data1:
+                    index0 = _csearchlinear(xs_data, self.xs_size, x, index0)
+                    xs_data0 = xs_data[index0]
+                    xs_data1 = xs_data[index0+1]
+                    ys_data0 = ys_data[index0]
+                    ys_data1 = ys_data[index0+1]
+                
+                result[i] = InterpolFunc_call(self.interpol_func, x, xs_data0, ys_data0, xs_data1, ys_data1)
+                i += 1
+                x = xstart + i*dx
+            if i < n - 1:
+                for j in range(i, n):
+                    result[j] = outbound1  
+        return numpy.asarray(result)
+        
+    cpdef ndarray _mapn_between(self, int n, double xstart, double xend, ndarray out=None):
+        """
+        Return an array of `n` elements resulting of evaluating this bpf regularly
+
+        The x coordinates at which this bpf is evaluated are equivalent to `linspace(xstart, xend, n)`
+
+        Args:
+            n (int): the number of elements to generate
+            xstart (float): x to start mapping
+            xend (float): x to end mapping
+            out (ndarray): if given, result is put here
+
+        Returns:
+            (ndarray) An array of this bpf evaluated at a grid [xstart:xend:dx], where *dx*
+            is `(xend-xstart)/n`
+        """
+        cdef double[:] result = out if out is not None else EMPTY1D(n)
+        cdef double dx = (xend - xstart) / (n - 1)   # we account for the edge (x1 IS INCLUDED)
+        with nogil:        
+            for i in range(n):
+                result[i] = self.__ccall__(xstart + dx*i)
+        return numpy.asarray(result)
+        
+    def __repr__(self):
+        return "%s[%s:%s]" % (self.__class__.__name__, str(self._x0), str(self._x1))
+
+    def stretch(self, double rx):
+        """
+        Stretch or compress this bpf in the x-coordinate **INPLACE**
+
+        **NB**: use `stretched` to create a new bpf
+
+        Args:
+            rx (float): the stretch/compression factor
+
+        """
+        if rx == 0:
+            raise ValueError("the stretch factor cannot be 0")
+        self.xs *= rx
+        self._recalculate_bounds()
+    
+    def shift(self, double dx):
+        """
+        Shift the bpf along the x-coords, **INPLACE**
+        
+        Use [.shifted](#shifted) to create a new bpf
+
+        Args:
+            dx (float): the shift interval
+
+        """
+        self.xs += dx
+        self._recalculate_bounds()
+
+    cdef void _recalculate_bounds(self):
+        cdef DTYPE_t* data
+        cdef int nx
+        nx = PyArray_DIM(self.xs, 0)
+        self.xs_data = <DTYPE_t*>self.xs.data
+        self._x0 = self.xs_data[0]
+        self._x1 = self.xs_data[nx - 1]
+        self._invalidate_cache()
+
+    def points(BpfBase self):
+        """
+        Returns a tuple with the points defining this bpf
+
+        Returns:
+            (tuple[ndarray, ndarray]) a tuple (xs, ys) where `xs` is an array
+            holding the values for the *x* coordinate, and `ys` holds the values for
+            the *y* coordinate
+
+        ## Example
+        
+        ```python
+
+        >>> b = Linear.fromseq(0, 0, 1, 100, 2, 50)
+        >>> b.points()
+        ([0, 1, 2], [0, 100, 50])
+        ```
+
+        """
+        return self.xs, self.ys
+
+    def clone_with_new_data(self, xs: ndarray, ys: ndarray) -> BpfInterface:
+        """
+        Create a new bpf with the same attributes as self but with new data
+
+        Args:
+            xs (ndarray): the x-coord data
+            ys (ndarray): the y-coord data
+
+        Returns:
+            (BpfInterface) The new bpf. It will be of the same class as self
+
+        """
+        state = self.__getstate__()
+        newstate = (xs, ys) + state[2:]
+        return self.__class__(*newstate)
+        
+    def insertpoint(self, double x, double y):
+        """
+        Return **a copy** of this bpf with the point `(x, y)` inserted
+
+        !!! note
+
+            *self* is not modified
+
+        Args:
+            x (float): x coord
+            y (float): y coord
+
+        Returns:
+            (BpfInterface) A clone of this bpf with the point inserted
+        """
+        cdef int index = _searchsorted(self.xs, x)
+        new_xs = numpy.insert(self.xs, index, x)
+        new_ys = numpy.insert(self.ys, index, y)
+        return self.clone_with_new_data(new_xs, new_ys)
+
+    def removepoint(self, double x):
+        """
+        Return a copy of this bpf with point at x removed
+
+        Args:
+            x (float): the x point to remove
+
+        Returns:
+            (BpfInterface) A copy of this bpf with the given point removed
+        
+        Raises `ValueError` if x is not in this bpf
+        
+        To remove elements by index, do:
+
+        ```python
+
+        xs, ys = mybpf.points()
+        xs = numpy.delete(xs, indices)
+        ys = numpy.delete(ys, indices)
+        mybpf = mybpf.clone_with_new_data(xs, ys)
+
+        ```
+        """
+        cdef int index = _csearchsorted_left(self.xs_data, self.xs.size, x)
+        if self.xs_data[index] != x:
+            raise ValueError("%f is not in points" % x)
+        newxs = numpy.delete(self.xs, index)
+        newys = numpy.delete(self.ys, index)
+        return self.clone_with_new_data(newxs, newys)
+
+    def segments(self):
+        """
+        Return an iterator over the segments of this bpf
+
+        Returns:
+            (Iterable[tuple[float, float, str, float]]) An iterator of segments, 
+            where each segment has the form `(x, y, interpoltype:str, exponent)`
+
+        Each segment is a tuple `(x: float, y: float, interpoltype: str, exponent: float)`
+
+        Exponent is only of value if the interpolation type makes use of it.
+        """
+        cdef size_t i
+        cdef size_t num_segments
+        num_segments = len(self.xs) - 1
+        interpoltype = self.__class__.__name__.lower()
+        for i in range(num_segments):
+            yield (float(self.xs[i]), float(self.ys[i]), interpoltype, self.interpol_func.exp)
+        yield (float(self.xs[num_segments]), float(self.ys[num_segments]), '', 0)
+
+    @property
+    def exp(self) -> float:
+        """
+        The exponential of the interpolation function of this bpf
+        """
+        return self.interpol_func.exp
+
+
+cdef class Linear(BpfBase):
+    """
+    A bpf with linear interpolation
+
+    ```python
+    from bpf4 import *
+    a = core.Linear([0, 2, 3.5, 10], [0.1, 0.5, -3.5,  4])
+    a.plot()
+    ```
+    ![](assets/Linear.png)
+
+    """
+    def __init__(self, xs, ys):
+        """
+        Args:
+            xs (ndarray): the x-coord data
+            ys (ndarray): the y-coord data
+        """
+        self.interpol_func = InterpolFunc_linear
+        BpfBase.__init__(self, xs, ys)
+
+    def _get_points_for_rendering(self, int n= -1):
+        return self.xs, self.ys
+
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        """
+        Integrate this bpf between the given x coords
+
+        Args:
+            x0 (float): start of integration
+            x1 (float): end of integration
+            N (int): number of integration steps
+
+        Returns:
+            (float) The result representing the area beneath the curve
+            between *x0* and *x1*
+        """
+        cdef double pre, mid, post
+        cdef size_t index0, index1
+        if x0 <= self._x0:
+            pre = self.__ccall__(x0) * (self._x0 - x0)
+            index0 = 0
+        else:
+            index0 = _csearchsorted(self.xs_data, self.xs_size, x0)
+            # trapezium = (a+b)/2 * h (where h is the distance between a and b)
+            pre = (self.ys_data[index0] + self.__ccall__(x0)) * 0.5 * (self.xs_data[index0] - x0)
+        if x1 >= self._x1:
+            post = self.__ccall__(x1) * (x1 - self._x1)
+            index1 = self.xs_size - 1
+        else:
+            index1 = _csearchsorted_left(self.xs_data, self.xs_size, x1) - 1
+            post = (self.ys_data[index1] + self.__ccall__(x1)) * 0.5 * (x1-self.xs_data[index1])
+        mid = 0
+        for i in range(index0, index1):
+            mid += (self.ys_data[i] + self.ys_data[i+1]) * 0.5 * (self.xs_data[i+1] - self.xs_data[i])
+        return pre + mid + post
+
+    cpdef Linear sliced(self, double x0, double x1):
+        """
+        Cut this bpf at the given points
+
+        Args:
+            x0 (float): start x to cut
+            x1 (float): end x to cut
+
+        Returns:
+            (Linear) Copy of this bpf cut at the given x-coords
+
+        If needed it inserts points at the given coordinates to limit this bpf to 
+        the range `x0:x1`.
+
+        **NB**: this is different from crop, which is just a "view" into the underlying
+        bpf. In this case a real `Linear` bpf is returned. 
+        """
+        X, Y = arraytools.arrayslice(x0, x1, self.xs, self.ys)
+        return Linear(X, Y)
+        
+    def inverted(self):
+        """
+        Return a new Linear bpf where x and y coordinates are inverted. 
+
+        This is only possible if y never decreases in value. Otherwise
+        a `ValueError` is thrown
+        
+        Returns:
+            (Linear) The inverted bpf
+
+        ![](assets/inverted.png)
+        """
+        res = _array_issorted(self.ys)
+        if res == -1 or res == 0:  # not sorted or has dups
+            raise ValueError(f"bpf can't be inverted, ys must always increase.\nys={self.ys}")
+        return Linear(self.ys, self.xs)
+        
+    def flatpairs(self):
+        """
+        Returns a flat 1D array with x and y values interlaced
+
+        Returns:
+            (ndarray) A 1D array representing the points of this bpf with *xs* and
+            *ys* interleaved
+
+        ```python
+
+        >>> a = linear(0, 0, 1, 10, 2, 20)
+        >>> a.flatpairs()
+        array([0, 0, 1, 10, 2, 20])
+
+        ```
+        """
+        return arraytools.interlace_arrays(self.xs, self.ys)
+
+
+cdef class Smooth(BpfBase):
+    """
+    A bpf with smoothstep interpolation. 
+
+    ```python
+
+    >>> a = Smooth([0, 1, 3, 10], [0.1, 0.5, -3.5,  1])
+    >>> a.plot()
+    ```
+    ![](assets/Smooth.png)
+
+    ```python
+    >>> a = core.Smooth([0, 1, 3, 10], [0.1, 0.5, -3.5,  1], numiter=3)
+    >>> a.plot()
+    ```
+    ![](assets/Smooth_numiter3.png)
+
+    """
+        
+    def __init__(self, xs, ys, int numiter=1):
+        """
+        Args:
+            xs (ndarray): the x-coord data
+            ys (ndarray): the y-coord data
+            numiter (int): the number of smoothstep steps
+
+        """
+        if numiter == 1:
+            self.interpol_func = InterpolFunc_smooth
+        else:
+            self.interpol_func = InterpolFunc_new(intrp_smooth, 1, "smooth", 1)
+            self.interpol_func.numiter = numiter
+        BpfBase.__init__(self, xs, ys)
+
+
+cdef class Smoother(BpfBase):
+    """
+    A bpf with smootherstep interpolation (perlin's variation of smoothstep) 
+
+    ```python
+
+    a = core.Smooth([0, 1, 3, 10], [0.1, 0.5, -3.5,  1])
+    b = core.Smoother(*a.points())
+    fig, axes = plt.subplots(1, 2, figsize=(12, 4))
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1])
+    ```
+    ![](assets/Smoother.png)
+
+    """
+    def __init__(self, xs, ys):
+        self.interpol_func = InterpolFunc_smoother
+        BpfBase.__init__(self, xs, ys)
+
+
+cdef class Halfcos(BpfBase):
+    """
+    A bpf with half-cosine interpolation
+
+    [HalfcosExp](#HalfcosExp) is the same as Halfcos. It exists with two
+    names for compatibility
+
+    ```python
+    a = core.Halfcos([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
+    b = core.Halfcos(*a.points(), exp=2)
+    c = core.Halfcos(*a.points(), exp=0.5)
+    fig, axes = plt.subplots(1, 3, figsize=(16, 4), tight_layout=True)
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1], show=False)
+    c.plot(axes=axes[2])
+    ```
+    ![](assets/Halfcos.png)
+    """
+    def __init__(self, xs, ys, double exp=1.0, int numiter=1):
+        """
+        Args:
+            xs (ndarray): the x-coord data
+            ys (ndarray): the y-coord data
+            exp (float): an exponent applied to the halfcosine interpolation
+            numiter (int): how many times to apply the interpolation
+
+        """
+        if exp == 1.0 and numiter == 1:
+            self.interpol_func = InterpolFunc_halfcos
+        elif exp == 1:
+            self.interpol_func = InterpolFunc_new(intrp_halfcos, 1, 'halfcos', 1)
+        else:
+            self.interpol_func = InterpolFunc_new(intrp_halfcosexp, exp, 'halfcosexp', 1)
+        self.interpol_func.numiter = numiter
+        super().__init__(xs, ys)
+    
+    def __getstate__(self):
+        return self.xs, self.ys, self.interpol_func.exp, self.interpol_func.numiter
+
+    def __repr__(self):
+        exp = self.interpol_func.exp
+        return "%s[%s:%s] exp=%s" % (self.__class__.__name__, str(self._x0), str(self._x1), str(exp))
+    
+
+HalfcosExp = Halfcos
+    
+
+cdef class Halfcosm(Halfcos):
+    """
+    A bpf with half-cosine and exponent depending on the orientation of the interpolation
+
+    When interpolating between two y values, y0 and y1, if  y1 < y0 the exponent
+    is inverted, resulting in a symmetrical interpolation shape
+
+    ```python
+    a = core.Halfcos([0, 1, 3, 10], [0.1, 0.5, 3.5,  1], exp=2)
+    b = core.Halfcosm(*a.points(), exp=2)
+    fig, axes = plt.subplots(1, 2, figsize=(16, 4))
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1])
+    ```
+    ![](assets/Halfcosm.png)
+
+    """
+    def __init__(self, xs, ys, double exp=1.0, int numiter=1):
+        self.interpol_func = InterpolFunc_new(intrp_halfcosexpm, exp, 'halfcosexpm', 1)
+        self.interpol_func.numiter = numiter
+        BpfBase.__init__(self, xs, ys)
+
+
+cdef class Expon(BpfBase):
+    """
+    A bpf with exponential interpolation
+
+    Example
+    -------
+
+    ```python
+    from bpf4 import *
+    import matplotlib.pyplot as plt
+    numplots = 5
+    fig, axs = plt.subplots(2, numplots, tight_layout=True, figsize=(20, 8))
+    for i in range(numplots):
+        exp = i+1
+        core.Expon([0, 1, 2], [0, 1, 0], exp=exp).plot(show=False, axes=axs[0, i])
+        core.Expon([0, 1, 2], [0, 1, 0], exp=1/exp).plot(show=False, axes=axs[1, i])
+        axs[0, i].set_title(f'{exp=}')
+        axs[1, i].set_title(f'exp={1/exp:.2f}')
+
+    plot.show()
+
+    ```
+    ![](assets/expon-grid2.png)
+    """
+    def __init__(self, xs, ys, double exp, int numiter=1):
+        """
+        Args:
+            xs (ndarray): the x-coord data
+            ys (ndarray): the y-coord data
+            exp (float): an exponent applied to the halfcosine interpolation
+            numiter (int): how many times to apply the interpolation
+        """
+        BpfBase.__init__(self, xs, ys)
+        self.interpol_func = InterpolFunc_new(intrp_expon, exp, 'expon', 1)  # must be freed
+        self.interpol_func.numiter = numiter
+    
+    def __getstate__(self): return self.xs, self.ys, self.interpol_func.exp
+    
+    def __setstate__(self, state):
+        self.xs, self.ys, exp = state
+        self.interpol_func.exp = exp
+
+    def __repr__(self):
+        return "%s[%s:%s] exp=%s" % (self.__class__.__name__, str(self._x0), str(self._x1), str(self.interpol_func.exp))
+
+
+cdef class Exponm(Expon):
+    """
+    A bpf with symmetrical exponential interpolation 
+
+    ```python
+    from bpf4 import *
+    import matplotlib.pyplot as plt
+    numplots = 5
+    fig, axs = plt.subplots(2, numplots, tight_layout=True, figsize=(20, 8))
+    for i in range(numplots):
+        exp = i+1
+        core.Exponm([0, 1, 2], [0, 1, 0], exp=exp).plot(show=False, axes=axs[0, i])
+        core.Exponm([0, 1, 2], [0, 1, 0], exp=1/exp).plot(show=False, axes=axs[1, i])
+        axs[0, i].set_title(f'{exp=}')
+        axs[1, i].set_title(f'exp={1/exp:.2f}')
+
+    plot.show()
+    ```
+
+    ![](assets/exponm-grid.png)
+    
+    """
+    def __init__(self, xs, ys, double exp, int numiter=1):
+        """
+        Args:
+            xs (ndarray): the x-coord data
+            ys (ndarray): the y-coord data
+            exp (float): an exponent applied to the halfcosine interpolation
+            numiter (int): how many times to apply the interpolation
+        """
+        BpfBase.__init__(self, xs, ys)
+        self.interpol_func = InterpolFunc_new(intrp_exponm, exp, 'exponm', 1)  # must be freed
+        self.interpol_func.numiter = numiter
+
+
+cdef class NoInterpol(BpfBase):
+    """
+    A bpf without interpolation
+
+    ```python
+    a = core.Linear([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
+    b = core.NoInterpol(*a.points())
+    c = core.Nearest(*a.points())
+    fig, axes = plt.subplots(1, 3, figsize=(15, 4), tight_layout=True)
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1], show=False)
+    c.plot(axes=axes[2])
+    ```
+    ![](assets/NoInterpol.png)
+    """
+    def __init__(self, xs, ys):
+        """
+        A bpf without interpolation
+
+        Args:
+            xs (ndarray): the x coord data
+            ys (ndarray): the y coord data
+        """
+        BpfBase.__init__(self, xs, ys)
+        self.interpol_func = InterpolFunc_nointerpol
+        
+
+cdef class Nearest(BpfBase):
+    """
+    A bpf with nearest interpolation
+
+    ```python
+    a = core.Linear([0, 1, 3, 10], [0.1, 0.5, 3.5,  1])
+    b = core.NoInterpol(*a.points())
+    c = core.Nearest(*a.points())
+    fig, axes = plt.subplots(1, 3, figsize=(15, 4), tight_layout=True)
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1], show=False)
+    c.plot(axes=axes[2])
+    ```
+    ![](assets/NoInterpol.png)
+    
+    """
+    def __init__(self, xs, ys):
+        """
+        A bpf with nearest interpolation
+
+        Args:
+            xs (ndarray): the x coord data
+            ys (ndarray): the y coord data
+        """
+        super().__init__(xs, ys)
+        self.interpol_func = InterpolFunc_nearest
+
+    def __getstate__(self): return self.xs, self.ys
+    
+
+ctypedef struct SplineS:
+    int use_low_slope
+    int use_high_slope
+    double low_slope
+    double high_slope
+    DTYPE_t *xs
+    DTYPE_t *ys
+    DTYPE_t *ys2
+    int length
+    npy_intp last_index
+
+
+cdef SplineS* SplineS_new(xs, ys, Py_ssize_t xs_size, double low_slope=0, double high_slope=0, int use_low_slope=0, int use_high_slope=0):
+    cdef SplineS *s = <SplineS *>malloc(sizeof(SplineS))
+    cdef int length = xs_size
+    cdef int i
+    cdef DTYPE_t * _xs = <DTYPE_t *>malloc(sizeof(DTYPE_t) * length)
+    cdef DTYPE_t * _ys = <DTYPE_t *>malloc(sizeof(DTYPE_t) * length)
+    for i in range(length):
+        _xs[i] = xs[i]
+        _ys[i] = ys[i]
+    s.xs = _xs
+    s.ys = _ys
+    s.low_slope = low_slope
+    s.high_slope = high_slope
+    s.use_low_slope = use_low_slope
+    s.use_high_slope = use_high_slope
+    s.last_index = length - 1
+    s.length = length
+    SplineS_calc_ypp(s)
+    return s
+
+
+cdef void SplineS_destroy(SplineS *self):
+    free(self.xs)
+    free(self.ys)
+    free(self.ys2)
+
+
+@cython.boundscheck(False)
+@cython.cdivision(True)
+cdef void SplineS_calc_ypp(SplineS *self) nogil:
+    cdef DTYPE_t *x_vals = self.xs
+    cdef DTYPE_t *y_vals = self.ys
+    cdef int n = self.length
+    cdef DTYPE_t *y2_vals = <DTYPE_t *>malloc(sizeof(DTYPE_t) * n)
+    cdef DTYPE_t *u =       <DTYPE_t *>malloc(sizeof(DTYPE_t) * (n - 1))  # this is a temporary array
+    cdef double x1_minus_x0, denom, sig, p, qn, un
+    cdef int i, k
+    if self.use_low_slope == 1:
+        x1_minus_x0 = x_vals[1] - x_vals[0]
+        # u[0] = (3.0/(x_vals[1]-x_vals[0])) * ((y_vals[1]-y_vals[0]) / (x_vals[1]-x_vals[0])-self.low_slope)
+        x1_minus_x0 += 1e-12
+        u[0] =(3.0 / x1_minus_x0) * ( (y_vals[1]-y_vals[0]) / x1_minus_x0 - self.low_slope)
+        y2_vals[0] = -0.5
+    else:
+        u[0] = 0.0
+        y2_vals[0] = 0.0   # natural spline
+    for i in range(1, n-1):
+        denom = x_vals[i+1] - x_vals[i-1] + 1e-12
+        sig = (x_vals[i]-x_vals[i-1]) / denom
+        p = sig*y2_vals[i-1]+2.0
+        y2_vals[i] = (sig-1.0)/p
+        if x_vals[i+1] == x_vals[i]:
+            x_vals[i+1] += 1e-12
+        u[i] = (y_vals[i+1]-y_vals[i]) / (x_vals[i+1]-x_vals[i]) - (y_vals[i]-y_vals[i-1]) / (x_vals[i]-x_vals[i-1])
+        u[i] = (6.0 * u[i] / denom - sig * u[i-1]) / p
+    if self.use_high_slope == 1:
+        qn = 0.5
+        un = (3.0/(x_vals[n-1]-x_vals[n-2])) * (self.high_slope - (y_vals[n-1]-y_vals[n-2]) / (x_vals[n-1]-x_vals[n-2]))
+    else:
+        qn = 0.0
+        un = 0.0    # natural spline
+    y2_vals[n-1] = (un-qn*u[n-2])/(qn*y2_vals[n-1]+1.0)
+    for k in range(n-2, -1, -1):
+        y2_vals[k] = y2_vals[k]*y2_vals[k+1]+u[k]
+    free(u)
+    self.ys2 = y2_vals
+
+
+@cython.boundscheck(False)
+@cython.cdivision(True)
+cdef inline double SplineS_at(SplineS *self, double x) nogil:
+    # if out of range, return endpoint
+    cdef double a, b, out
+    if x <= self.xs[0]:
+        return self.ys[0]
+    if x >= self.xs[self.last_index]:
+        return self.ys[self.last_index]
+    cdef int pos = _csearchsorted(self.xs, self.length, x)
+    cdef double h = self.xs[pos] - self.xs[pos-1]
+    if h == 0.0:
+        out = INFINITY
+    else:
+        a = (self.xs[pos] - x) / h
+        b = (x - self.xs[pos-1]) / h
+        out = (a* self.ys[pos-1] + b*self.ys[pos] + \
+              ((a*a*a - a)*self.ys2[pos-1] + \
+              (b*b*b - b)*self.ys2[pos]) * h*h/6.0)
+    return out
+
+
+cdef class Sampled(BpfInterface):
+    """
+    A bpf with regularly sampled data
+
+    When evaluated, values between the samples are interpolated with
+    a given function: linear, expon(x), halfcos, halfcos(x), etc.
+
+    """
+    cdef readonly ndarray ys
+    cdef double y0, y1
+    cdef double grid_dx, grid_x0, grid_x1
+    cdef int samples_size
+    cdef int nointerpol
+    cdef InterpolFunc* interpolfunc
+    cdef DTYPE_t* data
+    cdef ndarray _cached_xs
+
+    def __init__(self, samples, double dx, double x0=0, str interpolation='linear'):
+        """
+        Args:
+            samples (ndarray): the y-coord sampled data
+            dx (float): the sampling **period**
+            x0 (float): the first x-value
+            interpolation (str): the interpolation function used. One of 'linear',
+                'nointerpol', 'expon(X)', 'halfcos', 'halfcos(X)', 'smooth',
+                'halfcosm', etc.
+        """
+        self.ys = numpy.ascontiguousarray(samples, dtype=DTYPE)
+        self.data = <DTYPE_t *>self.ys.data
+        l = PyArray_DIM(self.ys, 0)
+        self.samples_size = l
+        self.grid_x0 = x0
+        self.grid_dx = dx
+        self.grid_x1 = x0 + dx * (l - 1)
+        self._set_bounds(x0, self.grid_x1)
+        self._cached_xs = None
+        if interpolation == 'nointerpol':
+            self.nointerpol = 1
+            self.interpolfunc = NULL
+        elif interpolation == 'linear':
+            self.nointerpol = 0
+            self.interpolfunc = InterpolFunc_linear
+        else:
+            self.nointerpol = 0
+            self.interpolfunc = InterpolFunc_new_from_descriptor(interpolation)
+            if self.interpolfunc is NULL:
+                raise ValueError("interpolation type not understood")
+        self.y0 = self.data[0]
+        self.y1 = self.data[l - 1]
+
+    @cython.cdivision(True)
+    @property
+    def samplerate(self) -> float: 
+        """
+        The samplerate of this bpf
+        """
+        return 1.0 / self.grid_dx
+
+    @property
+    def xs(self) -> numpy.ndarray:
+        """
+        The x-coord array of this bpf
+        """
+        if self._cached_xs is not None:
+            return self._cached_xs
+        self._cached_xs = numpy.linspace(self.grid_x0, self.grid_x1, self.samples_size)
+        return self._cached_xs
+
+    def points(self):
+        """
+        Returns a tuple with the points defining this bpf
+
+        Returns:
+            (tuple[ndarray, ndarray]) A tuple `(xs, ys)` where `xs` is an array
+            holding the values for the *x* coordinate, and `ys` holds the values for
+            the *y* coordinate
+
+        ## Example
+        
+        ```python
+
+        >>> b = Linear.fromseq(0, 0, 1, 100, 2, 50)
+        >>> b.points()
+        ([0, 1, 2], [0, 100, 50])
+        ```
+
+        """
+        return self.xs, self.ys
+    
+    property interpolation:
+        def __get__(self):
+            """
+            The interpolation kind of this bpf
+            """
+            if self.interpolfunc is not NULL:
+                return InterpolFunc_get_descriptor(self.interpolfunc)
+            return 'nointerpol'
+        def __set__(self, interpolation):
+            self.set_interpolation(interpolation)
+
+    @property
+    def dx(self) -> float: 
+        """
+        The sampling period (delta x)
+        """
+        return self.grid_dx
+
+    cpdef Sampled set_interpolation(self, str interpolation):
+        """
+        Sets the interpolation of this Sampled bpf, inplace
+
+        Args:
+            interpolation (str): the interpolation kind
+
+        Returns:
+            (Sampled) self
+
+        Returns *self*, so you can do:
+
+        ```python
+
+        sampled = bpf[x0:x1:dx].set_interpolation('expon(2)')
+        
+        ```
+        """
+        InterpolFunc_free(self.interpolfunc)
+        if interpolation == 'nointerpol':
+            self.nointerpol = 1
+            self.interpolfunc = NULL
+        else:
+            self.nointerpol = 0
+            self.interpolfunc = InterpolFunc_new_from_descriptor(interpolation)
+        return self
+
+    def __dealloc__(self):
+        InterpolFunc_free(self.interpolfunc)
+
+    def __getstate__(self):
+        return (self.ys, self.grid_dx, self.grid_x0, self.interpolation)
+
+    @cython.cdivision(True)
+    cdef double __ccall__(self, double x) nogil:
+        cdef int index0
+        cdef double y0, y1, x0
+        cdef double out
+        if x <= self.grid_x0:
+            out = self.y0
+        elif x >= self.grid_x1:
+            out = self.y1
+        else:
+            index0 = int((x - self.grid_x0) / self.grid_dx)
+            if self.nointerpol == 1:
+                out = self.data[index0]
+            else:
+                y0 = self.data[index0]
+                y1 = self.data[index0 + 1]
+                x0 = self.grid_x0 + index0 * self.grid_dx
+                out = InterpolFunc_call(self.interpolfunc, x, x0, y0, x0+self.grid_dx, y1)
+        return out
+
+    @cython.cdivision(True)
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        """
+        Return an array of `n` elements resulting of evaluating this bpf regularly
+
+        The x coordinates at which this bpf is evaluated are equivalent to `linspace(xstart, xend, n)`
+
+        Args:
+            n (int): the number of elements to generate
+            x0 (float): x to start mapping
+            x1 (float): x to end mapping
+            out (ndarray): if given, result is put here
+
+        Returns:
+            (ndarray) An array of this bpf evaluated at a grid [xstart:xend:dx], where *dx*
+            is `(xend-xstart)/n`
+        """
+        
+        cdef DTYPE_t *data
+        cdef DTYPE_t *selfdata
+        cdef int i, j, index0, nointerpol
+        cdef double x, y
+        cdef double grid_x0, grid_x1, self_y0, self_y1, grid_dx, interp_x0, interp_y0, interp_y1
+        cdef double dx = (x1 - x0) / (n - 1) # we account for the edge (x1 IS INCLUDED)
+        cdef double interpolfunc_exp
+        cdef t_func interpolfunc
+        if out is None:
+            out = EMPTY1D(n)
+            data = <DTYPE_t *>out.data
+        elif PyArray_ISCONTIGUOUS(out):
+            data = <DTYPE_t *>out.data
+        else:
+            for i in range(n):
+                out[i] = self.__ccall__(x0 + dx*i)
+            return out
+        grid_x0 = self.grid_x0
+        grid_x1 = self.grid_x1
+        self_y0 = self.y0
+        self_y1 = self.y1
+        grid_dx = self.grid_dx
+        selfdata = self.data
+        nointerpol = self.nointerpol
+        interpolfunc = self.interpolfunc.func
+        interpolfunc_exp = self.interpolfunc.exp
+        cdef size_t datasize = self.samples_size
+        i = 0
+        with nogil:
+            while i < n:
+                x = x0 + dx * i
+                if x > grid_x0:
+                    break
+                data[i] = self_y0
+                i += 1
+            while i < n:
+                x = x0 + dx * i
+                if x >= grid_x1:
+                    break
+                index0 = int((x - grid_x0) / grid_dx)
+                if nointerpol == 1:
+                    y = selfdata[index0]
+                else:
+                    interp_x0 = grid_x0 + index0 * grid_dx
+                    y = InterpolFunc_call(self.interpolfunc, x, interp_x0, selfdata[index0],
+                                          interp_x0 + grid_dx, selfdata[index0+1])
+                data[i] = y
+                i += 1
+            for j in range(i, n):
+                data[j] = self_y1
+        return out
+
+    @classmethod
+    def fromseq(cls, *args, **kws): raise NotImplementedError
+    
+    def _get_points_for_rendering(self, int n= -1): 
+        if self.interpolation == 'linear':
+            return self.xs, self.ys
+        else:
+            if n < 0:
+                n = NUM_XS_FOR_RENDERING
+            return numpy.linspace(self.x0, self.x1, n), self.mapn_between(n, self.x0, self.x1)
+    
+    def segments(self):
+        """
+        Returns an iterator over the segments of this bpf
+
+        Returns:
+            (Iterable[tuple[float, float, str, float]]) An iterator of segments, 
+            where each segment has the form `(x, y, interpoltype:str, exponent)`
+
+
+        Each item is a tuple `(float x, float y, str interpolation_type, float exponent)`
+
+        **NB**: exponent is only relevant if the interpolation type makes use of it
+        """
+        cdef int i
+        cdef double x0 = self.grid_x0
+        cdef double dx = self.grid_dx
+        descr = self.interpolation
+        exp = self.interpolfunc.exp if self.interpolfunc is not NULL else 0.0
+        for i in range(self.samples_size):
+            yield (x0 + i*dx, self.data[i], descr, exp)
+
+    cpdef double integrate(self):
+        """
+        Return the result of the integration of this bpf. 
+
+        If any of the bounds is `inf`, the result is also `inf`.
+
+        **NB**: to determine the limits of the integration, first crop the bpf via a slice
+        
+        ## Example
+        
+        Integrate this bpf from its lower bound to 10 (inclusive)
+        
+        ```python
+        b[:10].integrate()  
+        ```
+        """
+        return _integr_trapz(self.data, self.samples_size, self.grid_dx) 
+
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        """
+        The same as integrate() but between the (included) bounds x0-x1
+
+        It is effectively the same as `bpf[x0:x1].integrate()`, but more efficient
+        
+        **NB**: N has no effect. It is put here to comply with the signature of the function. 
+        """
+        dx = self.grid_dx
+        return _integr_trapz_between_exact(self.data, self.samples_size, dx, self.grid_x0, x0, x1)
+
+    cpdef BpfInterface derivative(self):
+        """
+        Return a curve which represents the derivative of this curve
+
+        It implements Newtons difference quotiont, so that:
+
+
+            derivative(x) = bpf(x + h) - bpf(x)
+                            -------------------
+                                      h
+        
+        Example
+        -------
+
+        ```python
+        
+        >>> from bpf4 import *
+        >>> a = slope(1)[0:6.28].sin()
+        >>> a.plot(show=False, color="red")
+        >>> b = a.derivative()
+        >>> b.plot(color="blue")
+
+        ```
+        ![](assets/derivative1.png)
+        """
+        return _BpfDeriv(self, self.grid_dx*0.99)
+
+    def inverted(self):
+        """
+        Return a view on this bpf with the coords inverted
+
+        Returns:
+            (BpfInterface) a view on this bpf with the coords inverted
+
+        In an inverted function the coordinates are swaped: the inverted version of a 
+        bpf indicates which *x* corresponds to a given *y*
+        
+        Returns None if the function is not invertible. For a function to be invertible, 
+        it must be strictly increasing or decreasing, with no local maxima or minima.
+        
+
+            f.inverted()(f(x)) = x
+        
+        
+        So if `y(1) == 2`, then `y.inverted()(2) == 1`
+
+        ![](assets/inverted.png)
+        """
+        
+        return Linear(self.xs, self.ys).inverted()
+
+    def flatpairs(self):
+        """
+        Returns a flat 1D array with x and y values interlaced
+
+        Returns:
+            (ndarray) A 1D array with x and y values interlaced
+
+        ```python
+        >>> a = linear(0, 0, 1, 10, 2, 20)
+        >>> a.flatpairs()
+        array([0, 0, 1, 10, 2, 20])
+        ```
+        """
+        return arraytools.interlace_arrays(self.xs, self.ys)
+
+    
+cdef class Spline(BpfInterface):
+    """
+    A bpf with cubic spline interpolation
+
+    With cubic spline interpolation, for each point `(x, y)` 
+    it is ensured that `bpf(x) == y`. Between the defined points,
+    depending on their proximity, this bpf can overshoot
+    
+    Example
+    -------
+
+    ```python
+    a = core.Smooth([0, 1, 3, 10], [0.1, 0.5, -3.5,  1])
+    b = core.Spline(*a.points())
+    fig, axes = plt.subplots(1, 2, figsize=(12, 4))
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1])
+    ```
+    ![](assets/Spline.png)
+
+    """
+    cdef SplineS* _spline
+
+    def __init__(self, xs, ys):
+        """
+        A bpf with cubic spline interpolation
+
+        Args:
+            xs (ndarray): the x coord data
+            ys (ndarray): the y coord data
+        """
+        
+        cdef ndarray [DTYPE_t, ndim=1] _xs = numpy.asarray(xs, dtype=DTYPE)
+        cdef ndarray [DTYPE_t, ndim=1] _ys = numpy.asarray(ys, dtype=DTYPE)
+        cdef int N = len(xs)
+        self._set_bounds(_xs[0], _xs[N - 1])
+        self._integration_mode = 1  # use quad
+        if _array_issorted(_xs) < 1:
+            raise ValueError(f"Points along the x coord should be sorted without duplicates. \n{xs}")
+        self._spline = SplineS_new(_xs, _ys, N)
+    
+    def __dealloc__(self):
+        SplineS_destroy(self._spline)
+    
+    @cython.boundscheck(False)
+    cdef double __ccall__(self, double x) nogil:
+        return SplineS_at(self._spline, x)
+    
+    cdef inline tuple _points(self):
+        cdef int i
+        xs = [self._spline.xs[i] for i in range(self._spline.length)]
+        ys = [self._spline.ys[i] for i in range(self._spline.length)]
+        return (xs, ys)
+    
+    def __getstate__(self):
+        return self._points()
+    
+    def points(self):
+        """
+        Returns a tuple with the points defining this bpf
+
+        Returns:
+            (tuple[ndarray, ndarray]) a tuple (xs, ys) where `xs` is an array
+            holding the values for the *x* coordinate, and `ys` holds the values for
+            the *y* coordinate
+
+        ## Example
+        
+        ```python
+
+        >>> b = Linear.fromseq(0, 0, 1, 100, 2, 50)
+        >>> b.points()
+        ([0, 1, 2], [0, 100, 50])
+        ```
+
+        """
+        return self._points()
+
+    def segments(self):
+        """
+        Returns an iterator over the segments of this bpf
+
+        Returns:
+            (Iterable[tuple[float, float, str, float]]) An iterator of segments, 
+            where each segment has the form `(x, y, interpoltype:str, exponent)`
+
+
+        Each segment is a tuple `(float x, float y, str interpolation_type, float exponent)`
+
+        !!! note
+        
+            Exponent is only relevant if the interpolation type makes use of it
+        
+        """
+        cdef size_t i
+        cdef size_t num_segments
+        exp = 0
+        num_segments = self._spline.length - 1
+        interpoltype = self.__class__.__name__.lower()
+        for i in range(num_segments):
+            yield (float(self._spline.xs[i]), float(self._spline.ys[i]), interpoltype, 0)
+        yield (float(self._spline.xs[num_segments]), float(self._spline.ys[num_segments]), '', 0)
+
+
+cdef class USpline(BpfInterface):
+    """
+    bpf with univariate spline interpolation. 
+
+    ```python
+    a = core.Spline([0, 1, 3, 10], [0.1, 0.5, -3.5,  1])
+    b = core.USpline(*a.points())
+
+    fig, axes = plt.subplots(1, 2, figsize=(12, 4), sharey=True, tight_layout=True)
+    a.plot(axes=axes[0], show=False)
+    b.plot(axes=axes[1])
+    ```
+    ![](assets/Uspline.png)
+    """
+    cdef object spline
+    cdef object spline__call__
+    cdef ndarray xs, ys
+    
+    def __init__(self, xs, ys):
+        """
+        Args:
+            xs (ndarray): the x coord data
+            ys (ndarray): the y coord data
+        """
+        
+        try:
+            from scipy.interpolate import UnivariateSpline
+        except ImportError:
+            raise ImportError("could not import scipy. USpline is a wrapper of UnivariateSpline"
+                              " and cant be used without scipy")
+        self.spline = UnivariateSpline(xs, ys)
+        self.spline__call__ = self.spline.__call__
+        self.xs = numpy.asarray(xs)
+        self.ys = numpy.asarray(ys)
+        self._set_bounds(xs[0], xs[len(xs) - 1])
+        self._integration_mode = 1  # use quad
+    
+    def __call__(self, x):
+        return self.spline(x)
+    
+    cdef double __ccall__(self, double x) nogil:
+        with gil:
+            return self.spline__call__(x)
+    
+    cpdef ndarray map(self, xs, ndarray out=None):
+        if out is not None:
+            out[...] = self.spline__call__(xs)
+            return out
+        else:
+            return self.spline__call__(xs)
+    
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        """
+        Return an array of `n` elements resulting of evaluating this bpf regularly
+
+        The x coordinates at which this bpf is evaluated are equivalent to `linspace(x0, x1, n)`
+
+        Args:
+            n (int): the number of elements to generate
+            x0 (float): x to start mapping
+            x1 (float): x to end mapping
+            out (ndarray): if given, result is put here
+
+        Returns:
+            (ndarray) An array of this bpf evaluated at a grid [xstart:xend:dx], where *dx*
+            is `(xend-xstart)/n`
+        """
+        
+        xs = numpy.linspace(x0, x1, n)
+        return self.map(xs, out)
+    
+    property _spline:
+        def __get__(self):
+            return self.spline
+    
+    def segments(self):
+        """
+        Returns an iterator over the segments of this bpf
+
+        Returns:
+            (Iterable[tuple[float, float, str, float]]) An iterator of segments, 
+            where each segment has the form `(x, y, interpoltype:str, exponent)`
+
+        """
+        cdef size_t i
+        cdef size_t num_segments
+        exp = 0
+        num_segments = len(self.xs) - 1
+        interpoltype = self.__class__.__name__.lower()
+        for i in range(num_segments):
+            yield (float(self.xs[i]), float(self.ys[i]), interpoltype, 0)
+        yield (float(self.xs[num_segments]), float(self.ys[num_segments]), '', 0)
+
+
+cdef class _BpfConcat2(BpfInterface):
+    cdef BpfInterface a
+    cdef BpfInterface b
+    cdef double splitpoint
+    cdef double __ccall__(self, double x) nogil:
+        if x < self.splitpoint:
+            return self.a.__ccall__(x)
+        return self.b.__ccall__(x)
+    
+    def __getstate__(self):
+        return self.a, self.b, self.splitpoint
+    
+    def __setstate__(self, state):
+        self.a, self.b, self.splitpoint = state
+        cdef double x0 = self.a._x0 if self.a._x0 < self.b._x0 else self.b._x0
+        cdef double x1 = self.b._x1 if self.b._x1 > self.a._x1 else self.a._x1
+        self._set_bounds(x0, x1)
+    
+
+cdef class Slope(BpfInterface):
+    """
+    A bpf representing a linear equation `y = slope * x + offset`
+
+    ```python
+
+    >>> from bpf4.core import *
+    >>> a = Slope(0.5, 1)
+    >>> a
+    Slope[-inf:inf]
+    >>> a[0:10].plot()
+    ```
+    ![](assets/slope-plot.png)
+    """
+    cdef public double slope
+    cdef public double offset
+    
+    def __init__(self, double slope, double offset=0, tuple bounds=None):
+        """
+        A bpf representing a linear equation `y = slope * x + offset`
+
+        Args:
+            slope (float): the slope of the line
+            offset (float): an offset added 
+            bounds (tuple): if given, the line is clipped on the x axis to the
+                given bounds
+        """
+        
+        self.slope = slope
+        self.offset = offset
+        if bounds is not None:
+            self._set_bounds(bounds[0], bounds[1])
+        else:
+            self._set_bounds(INFNEG, INF)
+        
+    cdef double __ccall__(self, double x) nogil:
+        return self.offset + x*self.slope
+
+    cpdef Slope _slice(self, double x0, double x1):
+        return Slope(self.slope, self.offset, bounds=(x0, x1))
+
+    def __add__(a, b):
+        if isnumber(a):
+            # we are b
+            return Slope(b.slope, b.offset + a, b.bounds())
+        elif isnumber(b):
+            return Slope(a.slope, a.offset + b, a.bounds())
+        else:
+            return _create_lambda(a, b, _BpfLambdaAdd, _BpfLambdaAddConst)
+
+    def __sub__(a, b):
+        if isnumber(a):
+            return b + (-a)
+        elif isnumber(b):
+            return a + (-b)
+        else:
+            return _create_rlambda(a, b, _BpfLambdaSub, _BpfLambdaSubConst, _BpfLambdaRSub, _BpfLambdaRSubConst)
+
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        """
+        Return an array of `n` elements resulting of evaluating this bpf regularly
+
+        The x coordinates at which this bpf is evaluated are equivalent to `linspace(x0, 1, n)`
+
+        Args:
+            n (int): the number of elements to generate
+            x0 (float): x to start mapping
+            x1 (float): x to end mapping
+            out (ndarray): if given, result is put here
+
+        Returns:
+            (ndarray) An array of this bpf evaluated at a grid [x0:x1:dx], where *dx*
+            is `(xend-xstart)/n`
+
+        """
+        cdef double[::1] result = out if out is not None else EMPTY1D(n)
+        cdef double offset = self.offset
+        cdef double slope = self.slope
+        cdef int i
+        cdef double x
+        cdef double dx = _ntodx(n, x0, x1)
+        cdef double slopex0 = slope * x0
+        cdef double slopedx = slope * dx
+        cdef double offset2 = offset + slopex0
+        with nogil:
+            for i in range(n):
+                # x = x0 + i * dx
+                # y = offset + (x0 + i*dx)*slope
+                # y = offset + slope*x0 + i*(dx*slope)
+                result[i] = offset2 + i * slopedx
+        return numpy.asarray(result)
+
+
+    def __mul__(a, b):
+        if isnumber(a):
+            return Slope(b.slope*a, b.offset*a, b.bounds())
+        elif isnumber(b):
+            return Slope(a.slope*b, a.offset*b, a.bounds())
+        return BpfInterface.__mul__(a, b)
+
+    def __getstate__(self):
+        return self.slope, self.offset, self.bounds()
+
+    
+cdef class _BpfCompose(BpfInterface):
+    """
+    A bpf representing function composition `f(x) = b(a(x))`
+    """
+    cdef BpfInterface a
+    cdef BpfInterface b
+
+    cdef double __ccall__(self, double x) nogil:
+        x = self.a.__ccall__(x)
+        return self.b.__ccall__(x)
+
+    def __getstate__(self):
+        return self.a, self.b
+
+    def __setstate__(self, state):
+        self.a, self.b = state
+        self._set_bounds(self.a._x0, self.a._x1)
+
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        """
+        Return an array of `n` elements resulting of evaluating this bpf regularly
+
+        The x coordinates at which this bpf is evaluated are equivalent to `linspace(x0, 1, n)`
+
+        Args:
+            n (int): the number of elements to generate
+            x0 (float): x to start mapping
+            x1 (float): x to end mapping
+            out (ndarray): if given, result is put here
+
+        Returns:
+            (ndarray) An array of this bpf evaluated at a grid [x0:x1:dx], where *dx*
+            is `(xend-xstart)/n`
+        """
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A
+        if out is not None:
+            self.a.mapn_between(n, x0, x1, out)
+            self.b.map(out, out)
+            return out
+        else:
+            A = self.a.mapn_between(n, x0, x1)
+            self.b.map(A, A)
+            return A
+ 
+
+cdef _BpfCompose _BpfCompose_new(BpfInterface a, BpfInterface b):
+    cdef _BpfCompose self = _BpfCompose()
+    self.a = a
+    self.b = b
+    self._set_bounds(a._x0, a._x1)
+    return self
+
+
+cdef _BpfConcat2 _BpfConcat2_new(BpfInterface bpf_a, BpfInterface bpf_b, double splitpoint):
+    cdef _BpfConcat2 self = _BpfConcat2()
+    cdef double x0 = bpf_a._x0 if bpf_a._x0 < bpf_b._x0 else bpf_b._x0
+    cdef double x1 = bpf_b._x1 if bpf_b._x1 > bpf_a._x1 else bpf_a._x1
+    self._set_bounds(x0, x1)
+    self.a = bpf_a
+    self.b = bpf_b
+    self.splitpoint = splitpoint
+    return self
+
+
+cdef class _BpfConcat(BpfInterface):
+    """
+    A bpf representing the concatenation of multiple bpfs
+    """
+    cdef list bpfs
+    cdef double *xs
+    cdef Py_ssize_t size
+    cdef double last_x0, last_x1
+    cdef BpfInterface last_bpf, bpf0, bpf1
+
+    def __cinit__(self, xs, bpfs):
+        self.size = len(xs)
+        self.xs = <double *>malloc(sizeof(double) * self.size)
+
+    def __init__(self, xs, bpfs):
+        """
+        Args:
+            xs (list|ndarray):  the offset of each bpf
+            bpfs (list[BpfInterface]): a list of bpfs to concatenate
+        """
+        cdef int i
+        cdef BpfInterface bpf
+        self.bpfs = list(bpfs)
+        i = 0
+        for x in xs:
+            self.xs[i] = x
+            i += 1
+        cdef double x0 = INF
+        cdef double x1 = INFNEG
+        for i in range(self.size):
+            bpf = self.bpfs[i]
+            if bpf._x0 < x0:
+                x0 = bpf._x0
+            if bpf._x1 > x1:
+                x1 = bpf._x1
+        self._set_bounds(x0, x1)
+        self.bpf0 = self.bpfs[0]
+        self.bpf1 = self.bpfs[self.size - 1]
+        self.last_bpf = self.bpf0
+        self.last_x0 = self.xs[0]
+        self.last_x1 = self.xs[1]
+
+    def __dealloc__(self):
+        free(self.xs)
+
+    cdef double __ccall__(self, double x) nogil:
+        cdef int index
+        if x <= self._x0:
+            return self.bpf0.__ccall__(x)
+        elif x >= self._x1:
+            return self.bpf1.__ccall__(x)
+        elif x >= self.last_x0 and x < self.last_x1:
+            return self.last_bpf.__ccall__(x)
+        else:
+            index = _csearchsorted_left(self.xs, self.size, x) - 1
+            with gil:
+                self.last_bpf = self.bpfs[index]
+            self.last_x0 = self.xs[index]
+            self.last_x1 = self.xs[index+1]
+            return self.last_bpf.__ccall__(x)
+
+    cpdef BpfInterface concat(self, BpfInterface other, double fadetime=0, fadeshape='expon(3)'):
+        cdef BpfInterface other2 = other.fit_between(self._x1, self._x1 + (other._x1 - other._x0))
+        cdef int i
+        cdef list xs
+        cdef list bpfs
+        if fadetime == 0:
+            xs = [self.xs[i] for i in range(self.size)]
+            bpfs = self.bpfs[:]
+            bpfs.append(other2)
+            return _BpfConcat(xs, bpfs)
+        raise NotImplementedError("fade is not implemented")
+
+    def __getstate__(self):
+        cdef list xs
+        cdef int i
+        xs = [self.xs[i] for i in range(self.size)]
+        return xs, self.bpfs
+
+
+cdef class _BpfBlend(BpfInterface):
+    cdef BpfInterface a, b
+    cdef BpfInterface which
+
+    def __init__(self, a: BpfInterface, b: BpfInterface, which: BpfInterface):
+        """
+        Args:
+            a: the first bpf
+            b: the second bpf
+            which: a bpf returning a value between 0-1; indicates the mix factor
+                at any x-point
+        """
+        self.a = a
+        self.b = b
+        self.which = which
+        cdef double x0 = min(a.x0, b.x0)
+        cdef double x1 = max(a.x1, b.x1)
+        self._set_bounds(x0, x1)
+
+    cdef double __ccall__(self, double x) nogil:
+        cdef double ya, yb, mix
+        mix = self.which.__ccall__(x)
+        ya = self.a.__ccall__(x) * (1 - mix)
+        yb = self.b.__ccall__(x) * mix
+        return ya + yb
+
+    def __getstate__(self):
+        return self.a, self.b, self.which
+
+        
+cdef class _BpfBlendConst(BpfInterface):
+    cdef BpfInterface a, b
+    cdef double which
+
+    def __init__(_BpfBlendConst self, BpfInterface a, BpfInterface b, double which):
+        """
+        Args:
+            a (BpfInterface): the first bpf
+            b (BpfInterface): the second bpf
+            which (float): a constant mix factor between 0-1
+        """
+        self.a = a
+        self.b = b
+        self.which = which
+        cdef double x0 = min(a._x0, b._x0)
+        cdef double x1 = max(a._x1, b._x1)
+        self._set_bounds(x0, x1)
+
+    cdef double __ccall__(self, double x) nogil:
+        return self.a.__ccall__(x) * (1 - self.which) + self.b.__ccall__(x) * self.which
+
+    def __getstate__(self): return self.a, self.b, self.which
+
+        
+cdef class Multi(BpfInterface):
+    """
+    A bpf where each segment can have its own interpolation kind
+    """
+    cdef DTYPE_t* xs
+    cdef DTYPE_t* ys
+    cdef InterpolFunc** interpolations
+    cdef int size
+    cdef DTYPE_t y0, y1, last_x0, last_x1, last_y0, last_y1
+    cdef InterpolFunc* last_interpol
+
+    def __cinit__(self, xs, ys, interpolations):
+        self.size = len(xs)
+        self.interpolations = <InterpolFunc **>malloc(sizeof(InterpolFunc*) * (self.size - 1))
+
+    def __init__(self, xs, ys, interpolations):
+        """
+        Args:
+            xs (ndarray): the sequence of x points
+            ys (ndarray): the sequence of y points
+            interpolations (list[str]): the interpolation used between these points
+
+        !!! note
+
+            ```python
+            
+            len(interpolations) == len(xs) - 1
+
+            ```
+
+        The interpelation is indicated via a descriptor: `'linear'` (linear), `'expon(x)'` 
+        (exponential with exp=x), `'halfcos'`, `'halfcos(x)'` (cosine interpol with exp=x),
+        `'nointerpol'`, ``'smooth'` (smoothstep)
+        """
+        cdef int i
+        cdef list interpolations_list
+        self.xs = _seq_to_doubles(xs)
+        self.ys = _seq_to_doubles(ys)
+        assert len(interpolations) == self.size - 1
+        i = 0
+        for interpolation in interpolations:
+            self.interpolations[i] = InterpolFunc_new_from_descriptor(interpolation)
+            i += 1
+        self._set_bounds(self.xs[0], self.xs[self.size - 1])
+        self.y0 = self.ys[0]
+        self.y1 = self.ys[self.size - 1]
+        self.last_x0 = self.xs[0]
+        self.last_x1 = self.xs[1]
+        self.last_y0 = self.ys[0]
+        self.last_y1 = self.ys[1]
+        self.last_interpol = self.interpolations[0]
+
+    def __dealloc__(self):
+        free(self.xs)
+        free(self.ys)
+        cdef int i
+        for i in range(self.size - 1):
+            InterpolFunc_free(self.interpolations[i])
+        free(self.interpolations)
+
+    def __getstate__(self):
+        cdef int i
+        xs = [self.xs[i] for i in range(self.size)]
+        ys = [self.ys[i] for i in range(self.size)]
+        interpolations = [InterpolFunc_get_descriptor(self.interpolations[i]) for i in range(self.size - 1)]
+        return xs, ys, interpolations
+
+    cdef double __ccall__(self, double x) nogil:
+        cdef double res, x0, x1, y0, y1
+        cdef int index1, index0
+        if x <= self._x0:
+            res = self.y0
+        elif x >= self._x1:
+            res = self.y1
+        else:
+            if self.last_x0 <= x < self.last_x1:
+                # res = self.last_interpol.func(x, self.last_x0, self.last_y0, self.last_x1, self.last_y1, self.last_interpol.exp)
+                res = InterpolFunc_call(self.last_interpol, x, self.last_x0, self.last_y0, self.last_x1, self.last_y1)
+            else:
+                index1 = _csearchsorted(self.xs, self.size, x)
+                index0 = index1 - 1
+                self.last_x0 = x0 = self.xs[index0]
+                self.last_x1 = x1 = self.xs[index1]
+                self.last_y0 = y0 = self.ys[index0]
+                self.last_y1 = y1 = self.ys[index1]
+                self.last_interpol = self.interpolations[index0]
+                # res = self.last_interpol.func(x, x0, y0, x1, y1, self.last_interpol.exp)
+                res = InterpolFunc_call(self.last_interpol, x, x0, y0, x1, y1)
+        return res
+
+    def segments(self):
+        """
+        Returns an iterator over the segments of this bpf
+
+        Returns:
+            (Iterator[tuple[float, float, str, float]]) An iterator of segments, 
+            where each segment has the form `(x, y, interpoltype:str, exponent)`
+
+        """
+        cdef int i
+        cdef InterpolFunc* func
+        for i in range(self.size - 1):
+            func = self.interpolations[i]
+            yield self.xs[i], self.ys[i], func.name, func.exp
+        yield (self.xs[self.size-1], self.ys[self.size-1], '', 0)
+
+
+ctypedef double(*dfunc)(double) nogil
+
+
+def _FunctionWrap(f, bounds=(INFNEG, INF)):
+    return _FunctionWrap_Object(f, bounds)
+
+
+cdef class _FunctionWrap_Object(BpfInterface):
+    cdef object f
+
+    def __init__(self, f, bounds=(INFNEG, INF)):
+        """
+        Args:
+            f (callable): a function to wrap as a bpf
+            bounds (tuple[float, float]): the bounds of this bpf
+        """
+        self._set_bounds(bounds[0], bounds[1])
+        self.f = f.__call__
+
+    cdef double __ccall__(self, double x) nogil:
+        with gil:
+            return self.f(x)
+
+    def __getstate__(self):
+        return (self.f, (self._x0, self._x1))
+
+    cpdef BpfInterface _slice(self, double x0, double x1):
+        return _FunctionWrap_Object_OutboundConst_new(self, x0, x1)
+
+    cpdef ndarray map(self, xs, ndarray out=None):
+        """
+        the same as map(self, xs) but somewhat faster
+
+        xs can also be a number, in which case it is interpreted as
+        the number of elements to calculate in an evenly spaced
+        grid between the bounds of this bpf.
+        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
+
+        if out is given, the result if put into it. it must have the 
+        same shape as xs
+        """
+        cdef ndarray [DTYPE_t, ndim=1] _xs
+        cdef ndarray [DTYPE_t, ndim=1] result
+        cdef DTYPE_t *data1
+        cdef DTYPE_t *data0
+        cdef list xs_as_list
+        cdef tuple xs_as_tuple
+        cdef int i, nx
+        cdef double x0,x1, dx
+        cdef object f = self.f
+        if isinstance(xs, (int, long)):
+            return self.mapn_between(xs, self._x0, self._x1, out)
+        else:
+            if out is None:
+                nx = len(xs)
+                result = EMPTY1D(nx)
+            else:
+                result = <ndarray>out
+                nx = PyArray_DIM(<ndarray>result, 0)
+            if isinstance(xs, ndarray):
+                if PyArray_ISCONTIGUOUS(<ndarray>xs):
+                    data1 = <DTYPE_t *>((<ndarray>xs).data)
+                    if PyArray_ISCONTIGUOUS(result):
+                        data0 = <DTYPE_t *>result.data
+                        for i in range(nx):
+                            data0[i] = f(data1[i])
+                    else:
+                        nx = PyArray_DIM(<ndarray>xs, 0)
+                        for i in range(nx):
+                            result[i] = f(data1[i])
+                else:
+                    _xs = <ndarray>xs
+                    for i in range(PyArray_DIM(xs, 0)):
+                        result[i] = f(_xs[i])
+            else:
+                if isinstance(xs, list):
+                    for i in range(nx):
+                        result[i] = f((<list>xs)[i])
+                elif isinstance(xs, tuple):
+                    xs_as_tuple = xs
+                    for i in range(len(xs_as_tuple)):
+                        result[i] = f(xs_as_tuple[i])
+                else:
+                    for i in range(nx):
+                        result[i] = f(xs[i])
+        return result
+        
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        xs = numpy.linspace(x0, x1, n)
+        return self.map(xs, out=out)
+
+
+cdef class _FunctionWrap_Object_OutboundConst(_FunctionWrap_Object):
+    cdef double y0, y1
+    cdef double __ccall__(self, double x) nogil:
+        if x < self._x0:
+            return self.y0
+        elif x > self._x1:
+            return self.y1
+        else:
+            with gil:
+                return self.f(x)
+
+
+cdef _FunctionWrap_Object_OutboundConst _FunctionWrap_Object_OutboundConst_new(_FunctionWrap_Object bpf, double x0, double x1):
+    cdef _FunctionWrap_Object_OutboundConst out = _FunctionWrap_Object_OutboundConst(bpf.f, (x0, x1))
+    out.y0 = out.f(x0)
+    out.y1 = out.f(x1)
+    return out
+
+
+cdef class Const(BpfInterface):
+    """
+    A bpf representing a constant value
+    """
+
+    cdef double value
+    
+    def __init__(self, double value, bounds: tuple[float, float]=None):
+        """
+        Args:
+            value (float): the constant value of this bpf
+        """
+        if bounds:
+            self._set_bounds(bounds[0], bounds[1])
+        else:
+            self._set_bounds(INFNEG, INF)
+        self.value = value
+    
+    def __call__(self, x): return self.value
+    
+    cdef double __ccall__(self, double x) nogil:
+        return self.value
+    
+    def __getstate__(self):
+        return (self.value,)
+    
+    def _get_points_for_rendering(self, int n):
+        x0 = self._x0 if self._x0 > INFNEG else 0.
+        x1 = self._x1 if self._x1 < INF else 1.
+        return numpy.array([x0, x1]), numpy.array([self.value, self.value])
+    
+    def __getitem__(self, slice):
+        if not hasattr(slice, 'start'):
+            raise ValueError("BPFs accept only slices, not single items.")    
+        cdef double x0 = slice.start if slice.start is not None else self._x0
+        cdef double x1 = slice.stop if slice.stop is not None else self._x1
+        cdef BpfInterface out = Const(self.value)
+        out._set_bounds(x0, x1)
+        return out
+            
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        if out is not None:
+            out[...] = self.value
+            return out
+        cdef double[::1] out2 = EMPTY1D(n)
+        cdef int i
+        for i in range(n):
+            out2[i] = self.value
+        return numpy.asarray(out2)
+        
+cdef _create_lambda_unordered(a, b, class_bin, class_const):
+    if isinstance(a, BpfInterface):        
+        if isinstance(b, BpfInterface):
+            out = class_bin(a, b, _get_bounds(a, b))
+        elif callable(b):
+            out = class_bin(a, _FunctionWrap(b), a.bounds())
+        else:
+            out = class_const(a, b, a.bounds())
+        return out
+    elif isinstance(b, BpfInterface):
+        if callable(a):
+            out = class_bin(b, _FunctionWrap(a), a.bounds())
+        else:
+            out = class_const(b, a, b.bounds())
+        return out
+
+cdef _create_lambda(BpfInterface a, object b, class_bin, class_const):
+    if isinstance(b, BpfInterface):
+        out = class_bin(a, b, _get_bounds(a, b))
+    elif callable(b):
+        out = class_bin(a, _FunctionWrap(b), a.bounds())
+    else:
+        out = class_const(a, b, a.bounds())
+    return out
+
+cdef _create_rlambda(object a, object b, class_bin, class_const, class_rbin=None, class_rconst=None):
+    if isinstance(a, BpfInterface):
+        if isinstance(b, BpfInterface):
+            out = class_bin(a, b, _get_bounds(a, b))
+        elif callable(b):
+            out = class_bin(a, _FunctionWrap(b), a.bounds())
+        else:
+            out = class_const(a, b, a.bounds())
+        return out
+    else:
+        if callable(a):
+            out = class_rbin(_FunctionWrap(a), b, b.bounds())
+        else:
+            out = class_rconst(b, a, b.bounds())
+    return out
+
+cdef class _BpfBinOp(BpfInterface):
+    """
+    A bpf representing a binary operation between two bpfs
+    """
+    cdef BpfInterface a, b
+
+    def __init__(self, BpfInterface a, BpfInterface b, tuple bounds):
+        self.a = a
+        self.b = b
+        self._x0, self._x1 = bounds
+    
+    def __getstate__(self):
+        return self.a, self.b, (self._x0, self._x1)
+    
+    def _get_xs_for_rendering(self, int n):
+        return numpy.unique(numpy.append(self.a._get_xs_for_rendering(n), self.b._get_xs_for_rendering(n)))
+
+    cdef double __ccall__(self, double x) nogil:
+        cdef double A = self.a.__ccall__(x)
+        cdef double B = self.b.__ccall__(x)
+        self._apply(&A, &B, 1)
+        return A
+
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        # the result should be put in A
+        pass
+    
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = <ndarray>out if out is not None else EMPTY1D(n)
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] B = EMPTY1D(n)
+        self.a.mapn_between(n, x0, x1, A)
+        self.b.mapn_between(n, x0, x1, B)
+        #cdef c_numpy.ndarray[DTYPE_t, ndim=1] ys_a = self.a.mapn_between(n, x0, x1, out)
+        #cdef c_numpy.ndarray[DTYPE_t, ndim=1] ys_b = self.b.mapn_between(n, x0, x1)
+        with nogil:
+            self._apply(<DTYPE_t*>A.data, <DTYPE_t*>B.data, n)
+            # self._apply(&A[0], &B[0], n)
+        return A
+        
+    cpdef ndarray map(self, xs, ndarray out=None):
+        """
+        the same as map(self, xs) but somewhat faster
+
+        xs can also be a number, in which case it is interpreted as
+        the number of elements to calculate in an evenly spaced
+        grid between the bounds of this bpf.
+        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
+        ( this is the same as bpf.mapn_between(10, bpf.x0, bpf.x1) )
+        """
+        cdef int len_xs
+        if isinstance(xs, (int, long)):
+            return self.mapn_between(xs, self._x0, self._x1, out)
+        len_xs = len(xs)
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = out if out is not None else EMPTY1D(len_xs)
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] B = EMPTY1D(len_xs)
+        self.a.map(xs, A)
+        self.b.map(xs, B)
+        with nogil:
+            self._apply(<DTYPE_t *>(A.data), <DTYPE_t *>(B.data), len_xs)
+        return numpy.asarray(A)
+
+
+cdef class _BpfUnaryFunc(BpfInterface):
+    cdef BpfInterface a
+    cdef t_unfunc func
+    cdef int funcindex
+    
+    def __reduce__(self):
+        return type(self), (), self.a, self.funcindex 
+    
+    def __setstate__(self, state):
+        bpf, funcindex = state
+        return _BpfUnaryFunc_new_from_index(bpf, funcindex)
+    
+    cdef void _apply(self, DTYPE_t *A, int n) nogil:
+        cdef t_unfunc func = self.func
+        for i in range(n):
+            A[i] = func(A[i])
+    
+    cdef double __ccall__(self, double x) nogil:
+        return self.func(self.a.__ccall__(x))
+    
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = self.a.mapn_between(n, x0, x1, out)
+        cdef t_unfunc func = self.func
+        with nogil:
+            self._apply(<DTYPE_t *>(A.data), n)
+        return A
+    
+    cpdef ndarray map(self, xs, ndarray out=None):
+        """
+        the same as map(self, xs) but somewhat faster
+
+        xs can also be a number, in which case it is interpreted as
+        the number of elements to calculate in an evenly spaced
+        grid between the bounds of this bpf.
+        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
+        ( this is the same as bpf.mapn_between(10, bpf.x0, bpf.x1) )
+        """
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A
+        if isinstance(xs, (int, long)):
+            return self.mapn_between(xs, self._x0, self._x1, out)
+        A = self.a.map(xs, out)
+        self._apply(<DTYPE_t *>(A.data), len(xs))
+        return A
+     
+
+cdef _BpfUnaryFunc _BpfUnaryFunc_new(BpfInterface a, t_unfunc func, int funcindex):
+    cdef _BpfUnaryFunc self = _BpfUnaryFunc()
+    self.a = a
+    self.func = func
+    self.funcindex = funcindex
+    cdef double x0, x1
+    x0, x1 = a.bounds()
+    self._set_bounds(x0, x1)
+    return self
+    
+
+cdef _BpfUnaryFunc _BpfUnaryFunc_new_from_index (BpfInterface a, int funcindex):
+    cdef t_unfunc func = _unfunc_from_index(funcindex)
+    return _BpfUnaryFunc_new(a, func, funcindex)
+    
+
+cdef t_unfunc _unfunc_from_index(int funcindex):
+    return UNFUNCS [funcindex]
+
+
+cdef class _BpfUnaryOp(BpfInterface):
+    """
+    A bpf representing a unary operation on a bpf
+    """
+    cdef BpfInterface a
+
+    def __init__(self, BpfInterface a):
+        self.a = a
+        cdef double x0, x1
+        x0, x1 = a.bounds()
+        self._set_bounds(x0, x1)
+    
+    cdef double __ccall__(self, double x) nogil:
+        cdef double X = self.a.__ccall__(x)
+        self._apply(&X, 1)
+        return X
+    
+    def __getstate__(self):
+        return (self.a,)
+    
+    def _get_xs_for_rendering(self, int n):
+        return self.a._get_xs_for_rendering(n)
+    
+    cdef void _apply(self, DTYPE_t *A, int n) nogil:
+        pass
+    
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = self.a.mapn_between(n, x0, x1, out)
+        with nogil:
+            self._apply(<DTYPE_t *>(A.data), n)
+        return A
+    
+    cpdef ndarray map(self, xs, ndarray out=None):
+        """
+        the same as map(self, xs) but somewhat faster
+
+        xs can also be a number, in which case it is interpreted as
+        the number of elements to calculate in an evenly spaced
+        grid between the bounds of this bpf.
+        bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))
+        ( this is the same as bpf.mapn_between(10, bpf.x0, bpf.x1) )
+        """
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A
+        if isinstance(xs, (int, long)):
+            return self.mapn_between(xs, self._x0, self._x1, out)
+        A = self.a.map(xs, out)
+        self._apply(<DTYPE_t *>(A.data), len(xs))
+        return A
+
+
+cdef class _BpfBinOpConst(BpfInterface):
+    """
+    A bpf representing a binary operation between a bpf and a constant value
+    """
+    cdef double b_const
+    cdef BpfInterface a
+    
+    def __init__(_BpfBinOpConst self, BpfInterface a, double b, tuple bounds, str op=''):
+        self.a = a
+        self.b_const = b
+        self._x0, self._x1 = bounds
+    
+    def __getstate__(self):
+        return self.a, self.b_const, (self._x0, self._x1)
+    
+    def _get_xs_for_rendering(self, int n):
+        return self.a._get_xs_for_rendering(n)
+    
+    cdef void _apply(self, DTYPE_t *A, int n, double x) nogil:
+        pass
+    
+    cpdef ndarray map(self, xs, ndarray out=None):
+        """
+        the same as map(self, xs) but somewhat faster
+
+        Args:
+            xs (ndarray | int): the points to evaluate this bpf at, or an
+                int indicating the number of points to sample this bpf
+                at within its bounds
+            out (ndarray): if given, the results of the evaluation
+                are placed here. It must be the same size as `xs`
+
+        Returns:
+            (ndarray) The resulting array
+
+        **NB**: `xs`` can be a number, in which case it is interpreted as
+        the number of elements to calculate in an evenly spaced
+        grid between the bounds of this bpf.
+        
+        `bpf.map(10) == bpf.map(numpy.linspace(x0, x1, 10))`
+
+        This is the same as `bpf.mapn_between(10, bpf.x0, bpf.x1)`
+        """
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A
+        cdef int len_xs
+        if isinstance(xs, (int, long)):
+            return self.mapn_between(xs, self._x0, self._x1, out)
+        A = self.a.map(xs, out)
+        len_xs = len(xs)
+        with nogil:
+            self._apply(<DTYPE_t *>(A.data), len_xs, self.b_const)
+        return A
+    
+    cdef double __ccall__(self, double x) nogil:
+        cdef double A = self.a.__ccall__(x)
+        self._apply(&A, 1, self.b_const)
+        return A
+
+
+cdef class _BpfLambdaAdd(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] += B[i]
+
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        return self.a.integrate_between(x0, x1, N) + self.b.integrate_between(x0, x1, N)
+
+    
+cdef class _BpfLambdaAddConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] += b
+
+    def __add__(a, b):
+        cdef double c
+        if isinstance(a, BpfInterface):
+            try:
+                c = float(b)
+                return _BpfLambdaAddConst(a.a, a.b + c)
+            except:
+                return _BpfBinOpConst.__add__(a, b)
+        else:
+            try:
+                c = float(a)
+                return _BpfLambdaAddConst(b.a, b.b + a)
+            except:
+                return _BpfBinOpConst.__add__(b, a)
+
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        return self.a.integrate_between(x0, x1, N) + (x1 - x0) * self.b_const
+
+
+cdef class _BpfLambdaSub(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] -= B[i]
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        return self.a.integrate_between(x0, x1, N) - self.b.integrate_between(x0, x1, N) 
+
+
+cdef class _BpfLambdaRSub(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            B[i] -= A[i]
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        return self.b.integrate_between(x0, x1, N) - self.a.integrate_between(x0, x1, N)
+
+
+cdef class _BpfLambdaSubConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] -= b
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        return self.a.integrate_between(x0, x1, N) - (x1-x0)*self.b_const
+
+
+cdef class _BpfLambdaRSubConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = b - A[i]
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        return self.b_const*(x1-x0) - self.a.integrate_between(x0, x1, N)
+
+
+cdef class _BpfLambdaMul(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] *= B[i]
+
+            
+cdef class _BpfLambdaMulConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] *= b
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        return self.a.integrate_between(x0, x1, N) * self.b_const
+
+
+cdef class _BpfLambdaPow(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = A[i] ** B[i]
+
+
+cdef class _BpfLambdaPowConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = A[i] ** b
+
+
+cdef class _BpfLambdaRPowConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = b ** A[i]
+
+
+cdef class _BpfLambdaDiv(_BpfBinOp):
+    @cython.cdivision(True)
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] /= B[i]
+
+
+cdef class _BpfLambdaDivConst(_BpfBinOpConst):
+    @cython.cdivision(True)
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] /= b
+
+
+cdef class _BpfLambdaMod(_BpfBinOp):
+    @cython.cdivision(True)
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = fmod(A[i], B[i])
+
+
+cdef class _BpfLambdaModConst(_BpfBinOpConst):
+    @cython.cdivision(True)
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = fmod(A[i], b)
+
+
+cdef class _BpfLambdaRDiv(_BpfBinOp):
+    @cython.cdivision(True)
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = B[i] / A[i]
+
+
+cdef class _BpfLambdaRDivConst(_BpfBinOpConst):
+    @cython.cdivision(True)
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = b / A[i]
+
+
+cdef class _BpfLambdaGreaterThan(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = A[i] > B[i]
+
+    
+cdef class _BpfLambdaGreaterOrEqualThan(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = A[i] >= B[i]
+
+
+cdef class _BpfLambdaGreaterThanConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = A[i] > b
+
+
+cdef class _BpfLambdaGreaterOrEqualThanConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = A[i] >= b
+
+
+cdef class _BpfLambdaLowerThan(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = A[i] < B[i]
+
+
+cdef class _BpfLambdaLowerThanConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = A[i] < b
+
+
+cdef class _BpfLambdaLowerOrEqualThan(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = A[i] <= B[i]
+
+
+cdef class _BpfLambdaLowerOrEqualThanConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = A[i] <= b
+
+
+cdef class _BpfLambdaEqual(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = A[i] == B[i]
+
+
+cdef class _BpfLambdaEqualConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = A[i] == b
+
+
+cdef class _BpfLambdaUnequal(_BpfBinOp):
+    cdef void _apply(self, DTYPE_t *A, DTYPE_t *B, int n) nogil:
+        for i in range(n):
+            A[i] = A[i] != B[i]
+
+
+cdef class _BpfLambdaUnequalConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = A[i] != b
+
+            
+cdef class _BpfMaxConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        cdef double y
+        for i in range(n):
+            y = A[i]
+            A[i] = y if y > b else b
+
+        
+cdef class _BpfMinConst(_BpfBinOpConst):
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        cdef double y
+        for i in range(n):
+            y = A[i]
+            A[i] = y if y < b else b
+
+
+cdef class _BpfLambdaLog(_BpfBinOpConst):
+    def __init__(_BpfBinOpConst self, BpfInterface a, double b, tuple bounds, str op=''):
+        _BpfBinOpConst.__init__(self, a, b, bounds, op)
+        self.b_const = m_log(b)
+    
+    @cython.cdivision(True)
+    cdef void _apply(self, DTYPE_t *A, int n, double b) nogil:
+        for i in range(n):
+            A[i] = m_log(A[i]) / b
+
+
+cdef class _BpfLambdaRound(_BpfUnaryOp):
+    cdef void _apply(self, DTYPE_t *A, int n) nogil:
+        for i in range(n):
+            A[i] = floor(A[i] + 0.5)
+
+
+cdef class _BpfRand(_BpfUnaryOp):
+    @cython.cdivision(True)
+    cdef void _apply(self, DTYPE_t *A, int n) nogil:
+        for i in range(n):
+            A[i] = (rand()/<double>RAND_MAX) * A[i]
+
+
+cdef class _BpfM2F(_BpfUnaryOp):
+    cdef void _apply(self, DTYPE_t *A, int n) nogil:
+        for i in range(n):
+            A[i] = m2f(A[i])
+
+
+cdef class _BpfF2M(_BpfUnaryOp):
+    cdef void _apply(self, DTYPE_t *A, int n) nogil:
+        for i in range(n):
+            A[i] = f2m(A[i])
+
+
+cdef class _Bpf_db2amp(_BpfUnaryOp):
+    cdef void _apply(self, DTYPE_t *A, int n) nogil:
+        for i in range(n):
+            A[i] = 10.0 ** (0.05*A[i])
+
+
+cdef class _Bpf_amp2db(_BpfUnaryOp):
+    cdef void _apply(self, DTYPE_t *A, int n) nogil:
+        cdef double x
+        for i in range(n):
+            x = max(A[i], 1e-14)
+            A[i] = log10(x) * 20.0
+            
+
+cdef class _BpfLambdaClip(BpfInterface):
+    cdef BpfInterface bpf
+    cdef double y0, y1
+    cdef double __ccall__(self, double x) nogil:
+        cdef double y = self.bpf.__ccall__(x)
+        if y > self.y1:
+            return self.y1
+        elif y < self.y0:
+            return self.y0
+        return y
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        cdef:
+            ndarray [DTYPE_t, ndim=1] result
+            DTYPE_t *data
+            int i
+            # we account for the edge (x1 IS INCLUDED)
+            double dx = (x1 - x0) / (n - 1) 
+            double y1 = self.y1
+            double y0 = self.y0
+            double y
+            BpfInterface bpf = self.bpf
+        if out is None:
+            result = EMPTY1D(n)
+            data = <DTYPE_t *>result.data
+            with nogil:
+                for i in range(n):
+                    y = bpf.__ccall__(x0 + dx * i)
+                    y = _clip(y, y0, y1)
+                    data[i] = y
+            return result
+        else:
+            if PyArray_ISCONTIGUOUS(out):
+                data = <DTYPE_t *>out.data
+                with nogil:
+                    for i in range(n):
+                        y = bpf.__ccall__(x0 + dx * i)
+                        y = _clip(y, y0, y1)
+                        data[i] = y
+            else:
+                for i in range(n):
+                    for i in range(n):
+                        y = bpf.__ccall__(x0 + dx * i)
+                        y = _clip(y, y0, y1)
+                        out[i] = y
+            return out
+
+    def __reduce__(self):
+        return type(self), (), (self.bpf, self.y0, self.y1)
+    
+    def __setstate__(self, state):
+        self.bpf, self.y0, self.y1 = state
+        self._set_bounds_like(self.bpf)
+
+
+cdef _BpfLambdaClip _BpfLambdaClip_new(BpfInterface bpf, double y0, double y1):
+    cdef _BpfLambdaClip self = _BpfLambdaClip()
+    self._set_bounds_like(bpf)
+    self.bpf = bpf
+    self.y0 = y0
+    self.y1 = y1
+    return self
+
+
+cdef class _BpfDeriv(BpfInterface):
+    """
+    A bpf representing the derivative of another bpf
+
+    The derivative at a point x is the forward derivative: `d = (f(x) + f(x+h)) / 2`
+    """
+    cdef BpfInterface bpf
+    cdef double h
+
+    def __init__(self, BpfInterface bpf, double h=0):
+        """
+        Args:
+            bpf (BpfInterface): the bpf to take the derivative
+            h (float): the delta x used to calculate the derivative
+        """
+        self.h = h
+        self.bpf = bpf
+        self._x0, self._x1 = bpf.bounds()
+
+
+    @cython.cdivision(True)
+    cdef double __ccall__(self, double x) nogil:
+        cdef double h = self.h if self.h > 0 else (SQRT_EPS if x == 0 else SQRT_EPS*x)
+        cdef double xh = x+h
+        cdef double f0, f1
+        cdef double x1 = self._x1
+        if x <= x1 and xh > x1:
+            # Prevent discontinuities at the boundaries
+            f1 = self.bpf.__ccall__(x1)
+            f0 = self.bpf.__ccall__(x1-h)
+        else:
+            f1 = self.bpf.__ccall__(x+h)
+            f0 = self.bpf.__ccall__(x)
+        return (f1 - f0) / h   
+       
+    def __getstate__(self):
+        return (self.bpf,)
+
+
+cdef class _BpfInverted(BpfInterface):
+    cdef BpfInterface bpf
+    cdef double bpf_x0, bpf_x1
+    
+    def __init__(self, BpfInterface bpf):
+        cdef double x0, x1
+        self.bpf = bpf
+        self.bpf_x0, self.bpf_x1 = bpf.bounds()
+        x0 = bpf(self.bpf_x0)
+        x1 = bpf(self.bpf_x1)
+        if x0 >= x1:
+            raise BpfInversionError("could not invert bpf")
+        self._set_bounds(x0, x1)
+
+    cdef double __ccall__(self, double x) nogil:
+        cdef double out
+        cdef int outerror, funcalls
+        if x < self._x0:
+            return self.bpf_x0
+        elif x > self._x1:
+            return self.bpf_x1
+        out = _bpf_brentq(self.bpf, -x, self.bpf_x0, self.bpf_x1, &outerror, BRENTQ_XTOL, BRENTQ_RTOL, BRENTQ_MAXITER, &funcalls)
+        if outerror == 1:   # error
+            return NAN
+        return out
+    
+    def __getstate__(self): return (self.bpf,)
+
+
+cdef class _BpfIntegrate(BpfInterface):
+    """
+    A bpf representing the integration of another bpf
+    """
+    cdef BpfInterface bpf
+    cdef double bpf_at_x0, width, min_N_ratio, Nexp
+    cdef int N, N0, Nwidth
+    cdef public int debug
+    cdef public size_t oversample
+    
+    def __init__(self, BpfInterface bpf, N=None, bounds=None, double min_N_ratio=0.3, 
+                 double Nexp=0.8, int oversample=0):
+        """
+        Args:
+            bpf: the bpf to integrate
+            N (int): the number of intervals to integrate
+            bounds (tuple(float, float)): the bounds of this bpf
+            min_N_ratio (float): ??
+            Nexp (float): ??
+            oversample (int): oversampling index
+        """
+        cdef double x0, x1, dx
+        cdef int i
+        cdef BpfInterface tmpbpf
+        cdef int _N
+        if bounds is None:
+            bounds = bpf.bounds()
+        _N = N if N is not None else CONFIG['integrate.trapz_intervals']
+        x0, x1 = bounds
+        self._set_bounds(x0, x1)
+        self.bpf = bpf
+        self.N = _N
+        self.bpf_at_x0 = bpf.__ccall__(x0)
+        self.min_N_ratio = min_N_ratio
+        self.N0 = <int>(_N * min_N_ratio)
+        self.Nexp = Nexp
+        self.width = x1 - x0
+        self.Nwidth = _N - self.N0
+        self.oversample = oversample if oversample > 0 else CONFIG['integrate.oversample']
+        if x0 == INFNEG or x0 == INF:
+            raise ValueError("cannot integrate a function with an infinite lower bound")
+        self.debug = 0
+    
+    @cython.cdivision(True)
+    cdef int get_integration_steps(self, double x) nogil:
+        return <int>(self.N0 + pow((x - self._x0) / self.width, self.Nexp) * self.Nwidth)
+    
+    @cython.cdivision(True)
+    cdef double __ccall__(self, double x) nogil:
+        with gil:
+            return self.bpf.integrate_between(self._x0, x)
+        
+    @cython.cdivision(True)
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        cdef double [::1] accums
+        cdef double dx0, dx1, dy
+        cdef double dx = (x1 - x0) / (n-1)
+        cdef int i, return_out
+        cdef double accum = self.bpf.integrate_between(self._x0, x0) if x0 > self._x0 else self.__ccall__(self._x0)
+        cdef size_t subn = self.oversample
+        if out is not None and out.shape[0] == n and PyArray_ISCONTIGUOUS(out):
+            accums = out
+            return_out = 1
+        else:
+            accums = EMPTY1D(n)
+            return_out = 0
+        accums[0] = accum
+        for i in range(1, n):
+            dx1 = x0 + i*dx
+            dx0 = dx1 - dx            
+            dy = self.bpf.integrate_between(dx0, dx1, subn)
+            accum += dy
+            accums[i] = accum
+        if return_out:
+            return out
+        else:
+            return numpy.asarray(accums)
+
+    cpdef BpfInterface derivative(self):
+        return self.bpf
+
+    def __getstate__(self):
+        return (self.bpf, self.N, self.bounds(), self.min_N_ratio, self.Nexp)
+
+
+cdef class _BpfPeriodic(BpfInterface):
+    cdef BpfInterface bpf
+    cdef double x0
+    cdef double period
+
+    def __init__(self, BpfInterface bpf):
+        self._set_bounds(INFNEG, INF)
+        self.bpf = bpf
+        cdef double x0, x1
+        x0, x1 = bpf.bounds()
+        self.x0 = x0
+        self.period = x1 - x0
+    
+    @cython.cdivision(True)
+    cdef double __ccall__(self, double x) nogil:
+        # the C equivalent of self.x0 + ((x - self.x0) % self.period)
+        # python n % M | c ((n % M) + M) % M
+        cdef double n = x - self.x0
+        cdef double p = self.x0 + ( (n % self.period + self.period) % self.period )
+        return self.bpf.__ccall__( p )
+
+    def __getstate__(self): return (self.bpf,)
+
+
+cdef class _BpfProjection(BpfInterface):
+    cdef BpfInterface bpf
+    cdef double bpf_x0
+    cdef readonly double dx, rx, offset
+
+    def __init__(self, BpfInterface bpf, double rx, double dx=0, double offset=0, bounds=None):
+        """
+        equation:
+
+        x2 = (x - offset) * rx + dx
+        self(x) = bpf(x2)
+
+        stretched 3: rx=3, offset=0, dx=0
+        shifted 2: rx=1, offset=0, dx=1
+        """
+        self.bpf = bpf
+        self.rx = rx
+        self.dx = dx
+        self.offset = offset
+        cdef double x0, x1
+        if bounds:
+            self._set_bounds(bounds[0], bounds[1])
+        else:
+            x0 = (bpf._x0 - dx)/rx + offset
+            x1 = (bpf._x1 - dx)/rx + offset
+            if x0 < x1:
+                self._set_bounds(x0, x1)
+            else:
+                self._set_bounds(x1, x0)
+
+    @cython.cdivision(True)
+    cdef double __ccall__(self, double x) nogil:
+        x = (x - self.offset) * self.rx + self.dx
+        return self.bpf.__ccall__(x)
+
+    def fixpoint(self):
+        return 1 - (self.fx - self.offset*self.rx)/self.rx
+
+    def __getstate__(self): return (self.bpf, self.rx, self.dx, self.bounds())
+
+
+cdef double m_log(double x) nogil:
+    # taken from python implementation (in C)
+    if isfinite(x):  # INFNEG > x < INF:
+        if x > 0:
+            return log(x)
+        if x == 0:
+            return INFNEG
+        else:
+            return NAN
+    elif isnan(x):
+        return x
+    elif x > 0:
+        return x
+    else:
+        return NAN
+
+
+cdef class _BpfKeepSlope(BpfInterface):
+    cdef BpfInterface bpf
+    cdef double EPSILON
+
+    def __init__(self, BpfInterface bpf, double EPSILON=DEFAULT_EPSILON):
+        #BpfInterface.__init__(self, INFNEG, INF)
+        self._set_bounds(INFNEG, INF)
+        self.bpf = bpf
+        self.EPSILON = EPSILON
+
+    @cython.cdivision(True)
+    cdef double __ccall__(self, double x) nogil:
+        cdef double slope
+        cdef double x0 = self.bpf._x0
+        cdef double x1 = self.bpf._x1
+        if x0 <= x <= x1:
+            return self.bpf.__ccall__(x)
+        elif x > x1:
+            slope = (self.bpf.__ccall__(x1) - self.bpf.__ccall__(x1 - self.EPSILON)) / self.EPSILON
+            return self.bpf.__ccall__(x1) + slope * (x - x1)
+        else:
+            slope = (self.bpf.__ccall__(x0 + self.EPSILON) - self.bpf.__ccall__(x0)) / self.EPSILON
+            return self.bpf.__ccall__(x0) + slope * (x - x0)
+
+    def __getstate__(self): return self.bpf, self.EPSILON
+
+
+cdef class _BpfCrop(BpfInterface):
+    cdef BpfInterface bpf
+    cdef readonly double _y0, _y1
+    cdef readonly int outbound_mode
+
+    cdef double __ccall__(self, double x) nogil:
+        if self.outbound_mode == 0:
+            return self.bpf.__ccall__(x)
+        else:
+            if x < self._x0:
+                return self._y0
+            elif x > self._x1:
+                return self._y1
+            return self.bpf.__ccall__(x)
+
+    def __reduce__(self):
+        return type(self), (), (self.bpf, self._x0, self._x1, self.outbound_mode, self._y0, self._y1)
+
+    def __setstate__(self, state):
+        self.bpf, x0, x1, self.outbound_mode, self._y0, self._y1 = state
+        self._set_bounds(x0, x1)
+
+    cpdef _BpfCrop outbound_set(self, double y0, double y1):
+        """
+        set the value returned by this BPF outside its defined bounds (inplace)
+        """
+        self.outbound_mode = OUTBOUND_SET
+        self._y0 = y0
+        self._y1 = y1
+        return self
+
+    def outbound(self, double y0, y1=None):
+        """
+        return a new Bpf with the given values outside the bounds
+
+        !!! note
+    
+            One can specify one value for lower and one for upper bounds, 
+            or just one value for both
+        """
+        if y1 is None:
+            y1 = y0
+        return _BpfCrop_new(self.bpf, self._x0, self._x1, OUTBOUND_SET, y0, y1)
+
+    cpdef double integrate_between(self, double x0, double x1, size_t N=0):
+        if x0 >= self.bpf._x0 and x1 <= self.bpf._x1:
+            return self.bpf.integrate_between(x0, x1)
+        cdef double integr0=0., integr1=0., integr2=0., _x0, _x1
+        if x0 < self.bpf._x0:
+            integr0 = self.__ccall__(x0) * (self.bpf._x0 - x0)
+            _x0 = self.bpf._x0
+        else:
+            _x0 = x0
+        if self._x1 > self.bpf._x1:
+            integr2 = self.__ccall__(x1) * (x1 - self.bpf._x1)
+            _x1 = self.bpf._x1
+        else:
+            _x1 = x1
+        integr1 = self.bpf.integrate_between(_x0, _x1)
+        return integr0 + integr1 + integr2
+
+    cpdef ndarray mapn_between(self, int n, double x0, double x1, ndarray out=None):
+        if self.outbound_mode == OUTBOUND_DONOTHING:
+            return self.bpf.mapn_between(n, x0, x1, out)
+        if x0 >= self._x1:
+            return numpy.ones((n,), dtype=float) * self.__ccall__(x0)
+        if x1 <= self._x0:
+            return numpy.ones((n,), dtype=float) * self.__ccall__(x1)
+
+        cdef double x, y0, y1, intersect_x0, intersect_x1, dx
+        cdef int i = 0
+        cdef int intersect_n, intersect_i0, intersect_i
+         
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] A = out if out is not None else EMPTY1D(n)
+        cdef c_numpy.ndarray[DTYPE_t, ndim=1] intersection
+        
+        cdef DTYPE_t *data = <DTYPE_t*>(A.data)
+        
+        dx = (x1 - x0) / (n - 1)
+        
+        if x0 < self._x0:
+            i = <int>((self._x0 - x0) / dx)
+            for j in range(i):
+                data[j] = self._y0
+            intersect_x0_quant = x0 + dx*i
+        else:
+            intersect_x0_quant = x0
+
+        intersect_x1 = min(x1, self._x1)
+        cdef double diff = ((intersect_x1 - x0) % dx)
+        if diff < 1e-15 or (dx - diff) < 1e-15:
+            diff = 0
+        intersect_x1_quant = intersect_x1 - diff
+        intersect_n = _dxton(dx, intersect_x0_quant, intersect_x1_quant)
+        intersection = self.bpf.mapn_between(intersect_n, intersect_x0_quant, intersect_x1_quant)
+        cdef DTYPE_t *intersection_data = <DTYPE_t*>(intersection.data)
+        cdef double intersect_dx = _ntodx(intersect_n, intersect_x0_quant, intersect_x1_quant)
+        # print("dx: %f, intersect_dx: %f, intersect_x1: %f, intersect_x1_quant: %f, x1: %f, diff:%f" % (dx, intersect_dx, intersect_x1, intersect_x1_quant, x1, diff))
+        for j in range(intersect_n):
+            A[i+j] = intersection_data[j]
+
+        y1 = self._y1
+        for j in range(i+intersect_n, n):
+            data[j] = y1
+
+        return A
+        
+
+cpdef _BpfCrop _BpfCrop_new(BpfInterface bpf, double x0, double x1, int outbound_mode, 
+                            double outbound0=0, double outbound1=0):
+    """
+    Create a cropped bpf. 
+    
+    Args:
+        bpf: the bpf to crop
+        x0: the lower bound
+        x1: the upper bound
+        outbound_mode: -1=use the default; 0=do nothing (the bpf is evaluated at the cropping 
+            point each time it is called outside the bounds); 1=cache the values; 2=set (in  
+            this case the last parameters outbount0 and outbound1 are used when called outside 
+            the bounds) 
+        outbound0: lower outbound value, returned when called with `x < x0` and *outbound_mode* is 2
+        outbound1: upper outbound value, returned when called with `x > x1` and *outbound_mode* is 2
+    
+    Returns:
+        (_BpfCrop) a cropped bpf
+    """
+    self = _BpfCrop()
+    self._set_bounds(x0, x1)
+    self.bpf = bpf
+    # -1: use the default, 0: do nothing, call __ccall__ each time, 
+    # 1: cache y0 and y1 for values outside the bounds, 
+    # 2: set y0 and y1 for values outside the bounds
+    if outbound_mode == OUTBOUND_DEFAULT:
+        outbound_mode = CONFIG['crop.outbound_mode']
+    self.outbound_mode = outbound_mode
+    if outbound_mode == OUTBOUND_CACHE:
+        self._y0 = self.bpf.__ccall__(x0)
+        self._y1 = self.bpf.__ccall__(x1)
+    elif outbound_mode == OUTBOUND_SET:
+        self._y0 = outbound0
+        self._y1 = outbound1
+    return self
+    
+
+cdef class _MultipleBpfs(BpfInterface):
+    cdef tuple _bpfs
+    cdef void** bpfpointers
+    cdef BpfInterface tmp
+    cdef int _numbpfs
+    
+    def __init__(self, bpfs):
+        self._numbpfs = len(bpfs)
+        self._bpfs = tuple(bpfs)
+        self._calculate_bounds()
+        self.bpfpointers = <void**>malloc(sizeof(void*) * self._numbpfs)
+        cdef int i
+        for i in range(self._numbpfs):
+            self.bpfpointers[i] = <void*>bpfs[i]
+    
+    def __dealloc__(self):
+        free(self.bpfpointers)
+    
+    def _calculate_bounds(self):
+        cdef double bounds0, bounds1
+        cdef double x0=INF, x1=INFNEG
+        for bpf in self._bpfs:
+            bound0, bound1 = bpf.bounds()
+            if bound0 < x0:
+                x0 = bound0
+            if bound1 > x1:
+                x1 = bound1
+        self._set_bounds(x0, x1)
+    
+    def __getstate__(self): return (self._bpfs,)
+    
+    cdef double __ccall__(self, double x) nogil:
+        with gil:
+            raise NotImplementedError
+
+
+cdef class Max(_MultipleBpfs):
+    """
+    A bpf which returns the max of multiple bpfs at a given point
+
+    ```python
+    a = linear(0, 0, 1, 0.5, 2, 0)
+    b = expon(0, 0, 2, 1, exp=3)
+    a.plot(show=False, color="red", linewidth=4, alpha=0.3)
+    b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
+    core.Max((a, b)).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
+    ```
+    ![](assets/Max.png)
+    """
+    def __init__(self, *bpfs):
+        if len(bpfs) == 1 and isinstance(bpfs[0], (list, tuple)):
+            bpfs = bpfs[0]
+        _MultipleBpfs.__init__(self, bpfs)
+
+    cdef double __ccall__(self, double x) nogil:
+        cdef double y = INFNEG
+        cdef double res
+        cdef int i
+        for i in range(self._numbpfs):
+            with gil:
+                self.tmp = <BpfInterface>(self.bpfpointers[i])
+            res = self.tmp.__ccall__(x)
+            if res > y:
+                y = res
+        return y
+
+
+cdef class Min(_MultipleBpfs):
+    """
+    A bpf which returns the min of multiple bpfs at a given point
+
+    ```python
+    a = linear(0, 0, 1, 0.5, 2, 0)
+    b = expon(0, 0, 2, 1, exp=3)
+    a.plot(show=False, color="red", linewidth=4, alpha=0.3)
+    b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
+    core.Min((a, b)).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
+    ```
+    ![](assets/Min.png)
+    
+    """
+    def __init__(self, *bpfs):
+        if len(bpfs) == 1 and isinstance(bpfs[0], (list, tuple)):
+            bpfs = bpfs[0]
+        _MultipleBpfs.__init__(self, bpfs)
+    
+    cdef double __ccall__(self, double x) nogil:
+        cdef double y = INF
+        cdef double res
+        cdef int i
+        for i in range(self._numbpfs):
+            with gil:
+                tmp = <BpfInterface>(self.bpfpointers[i])
+            res = tmp.__ccall__(x)
+            if res < y:
+                y = res
+        return y
+
+
+cdef class Stack(_MultipleBpfs):
+    """
+    A bpf representing a stack of bpf
+
+    Within a Stack, a bpf does not have outbound values. When evaluated
+    outside its bounds the bpf below is used, iteratively until the
+    lowest bpf is reached. Only the lowest bpf is evaluated outside its
+    bounds
+
+    Example
+    -------
+
+    ```python
+    # Interval    bpf
+    # [0, 3]      a
+    # (3, 4]      b
+    # (4, 10]     c
+
+    from bpf4 import *
+    import matplotlib.pyplot as plt
+    
+    a = linear(0, 0, 3, 1)
+    b = linear(2, 9, 4, 10)
+    c = halfcos(0, 0, 10, 10)
+    s = core.Stack((a, b, c))
+
+    ax = plt.subplot(111)
+    a.plot(color="#f00", alpha=0.4, axes=ax, linewidth=4, show=False)
+    b.plot(color="#00f", alpha=0.4, axes=ax, linewidth=4, show=False)
+    c.plot(color="#f0f", alpha=0.4, axes=ax, linewidth=4, show=False)
+    s.plot(axes=ax, linewidth=2, color="#000", linestyle='dotted')
+    ```
+    ![](assets/stack2.png)
+
+    """
+    cdef double[::1] flatbounds
+
+    def __init__(self, bpfs):
+        """
+        Args:
+            bpfs (list|tuple): A sequence of bpfs. The order defined the evaluation
+                order. The first bpf is on top, the last bpf is on bottom. Only
+                the last bpf is evaluated outside its bounds
+
+        """
+        self.flatbounds = EMPTY1D(len(bpfs)*2)
+        _MultipleBpfs.__init__(self, bpfs)
+
+    def _calculate_bounds(self):
+        cdef double x0 = INF, x1 = INFNEG
+        cdef BpfInterface b
+        cdef int i = 0
+        for b in self._bpfs:
+            if b.x0 < x0:
+                x0 = b.x0
+            if b.x1 > x1:
+                x1 = b.x1
+            self.flatbounds[i] = b.x0
+            self.flatbounds[i+1] = b.x1
+            i += 2
+        self._set_bounds(x0, x1)
+
+    cdef double __ccall__(self, double x) nogil:
+        cdef double out = 0.
+        for i in range(self._numbpfs):
+            if self.flatbounds[i*2] <= x <= self.flatbounds[i*2+1] or i == self._numbpfs - 1:
+                with gil:
+                    self.tmp = <BpfInterface>(self.bpfpointers[i])
+                out = self.tmp.__ccall__(x)
+                break
+        return out
+
+
+cdef class _BpfSelect(_MultipleBpfs):
+    cdef BpfInterface which
+    cdef InterpolFunc* func
+    cdef int numbpfs
+    
+    def __init__(self, which, bpfs, shape='linear'):
+        """
+        Interpolate between adjacent bpfs
+
+        Args:
+            which: a bpf mapping x->bpf index, where the index can
+                be fractionl and will interpolate between adjacent
+                bpfs
+            bpfs: the bpfs to select from
+            shape: the interpolation shape when dealing with fractional indexes
+        """
+        self.which = which
+        self.numbpfs = len(bpfs)
+        self.func = InterpolFunc_new_from_descriptor(shape)
+        _MultipleBpfs.__init__(self, bpfs)
+    
+    cdef double __ccall__(self, double x) nogil:
+        cdef double index = self.which.__ccall__(x)
+        cdef double y0, y1, x0
+        if index <= 0:
+            with gil:
+                b0 = <BpfInterface>(self.bpfpointers[0])
+            return b0.__ccall__(x)
+        elif index >= self.numbpfs - 1:
+            with gil:
+                b0 = <BpfInterface>(self.bpfpointers[self.numbpfs-1])
+            return b0.__ccall__(x)
+        else:
+            x0 = floor(index)
+            if x0 == index:
+                with gil:
+                    b0 = <BpfInterface>(self.bpfpointers[<int>x0])
+                    return b0.__ccall__(x)
+
+            with gil:
+                b0 = <BpfInterface>(self.bpfpointers[<int>x0])
+                b1 = <BpfInterface>(self.bpfpointers[<int>x0 + 1])
+
+            y0 = b0.__ccall__(x)
+            y1 = b1.__ccall__(x)
+            return InterpolFunc_call(self.func, index, x0, y0, x0+1, y1)
+
+def brentq(bpf, double x0, double xa, double xb, double xtol=9.9999999999999998e-13, 
+           double rtol=4.4408920985006262e-16, max_iter=100):
+    """
+    Calculate the zero of `bpf + x0` in the interval `(xa, xb)` using brentq algorithm
+
+    !!! note 
+
+        To calculate all the zeros of a bpf, use [.zeros()](#zeros)
+
+    Args:
+        bpf (BpfInterface): the bpf to evaluate
+        x0 (float): an offset so that bpf(x) + x0 = 0
+        xa (float): the starting point to look for a zero
+        xb (float): the end point
+        xtol (float): The computed root x0 will satisfy np.allclose(x, x0, atol=xtol, rtol=rtol)
+        rtol (float): The computed root x0 will satisfy np.allclose(x, x0, atol=xtol, rtol=rtol)
+        max_iter (int): the max. number of iterations
+
+    Returns:
+        (tuple[float, int]) A tuple (zero of the bpf, number of function calls)
+
+
+    ## Example
+    
+    ```python
+
+    # calculate the x where a == 0.5
+    >>> from bpf4 import *
+    >>> a = linear(0, 0, 10, 1)
+    >>> xzero, numcalls = brentq(a, -0.5, 0, 1)
+    >>> xzero
+    5
+    ```
+    """
+    cdef int outerror, funcalls
+    cdef double result
+    result = _bpf_brentq(bpf, x0, xa, xb, &outerror, xtol, rtol, max_iter, &funcalls)
+    if outerror:
+        raise ValueError("zero of function cannot be found within the interval given")
+    return result, funcalls
+
+
+cpdef BpfInterface blend(a, b, mix=0.5):
+    """
+    Blend these BPFs
+
+    Args:
+        a (BpfInterface): first bpf
+        b (BpfInterface): second bpf
+        mix (float | BpfInterface): how to mix the bpfs. Can be fixed or
+            itself a bpf (or any function) returning a value between 0-1 
+
+    Returns:
+        (BpfInterface) The blended bpf
+    
+    
+    !!! note
+
+        if mix == 0: the result is *a*
+        if mix == 1: the result is *b*
+    
+    
+    ## Example
+    
+    Create a curve which is in between a halfcos and a linear interpolation
+    
+    ```python
+    from bpf4 import *
+    a = halfcos(0, 0, 1, 1, exp=2)
+    b = linear(0, 0, 1, 1)
+    c = blend(a, b, 0.5)
+
+    a.plot(show=False, color="red")
+    b.plot(show=False, color="blue")
+    c.plot(color="green")
+
+    ```
+    ![](assets/blend1.png)
+
+    Closer to halfcos
+
+    ```python
+    c = blend(a, b, 0.2)
+    a.plot(show=False, color="red")
+    b.plot(show=False, color="blue")
+    c.plot(color="green")
+    ```
+    ![](assets/blend2.png)
+    """
+    if isinstance(mix, (int, float)):
+        return _BpfBlendConst(_asbpf(a), _asbpf(b), mix)
+    return _BpfBlend(_asbpf(a), _asbpf(b), _asbpf(mix))
+        
+
+
+cdef inline int isnumber(obj):
+    return isinstance(obj, (int, float))
+
+
+@cython.cdivision(True)
+cdef inline double _bpf_brentq(BpfInterface bpf, double x0, double xa, double xb, int* outerror, 
+                               double xtol, double rtol, int max_iter, int *outfuncalls) nogil:
+    # original values: xtol=9.9999999999999998e-13, rtol=4.4408920985006262e-16, max_iter=100
+    # calculate the 0 of the function bpf + x0 in the interval (xa, xb)
+    # if it is not possible, outerror is set to 1, otherwise it is 0
+    cdef:
+        double xpre = xa
+        double xcur = xb
+        double xblk = 0
+        double fpre, fcur, stry, dpre, dblk, sbis, tol
+        double fblk = 0
+        double spre = 0
+        double scur = 0
+        double a, b
+        int funcalls = 2
+        int i
+    outerror[0] = 0
+    fpre = bpf.__ccall__(xpre) + x0
+    fcur = bpf.__ccall__(xcur) + x0
+    outfuncalls[0] = 2
+    if fpre * fcur > 0:
+        outerror[0] = 1
+        return 0
+    if fpre == 0:
+        return xpre
+    if fcur == 0:
+        return xcur
+    for i in range(max_iter):
+        if fpre * fcur < 0:
+            xblk = xpre
+            fblk = fpre
+            spre = scur = xcur - xpre
+        if fabs(fblk) < fabs(fcur):
+            xpre = xcur
+            xcur = xblk
+            xblk = xpre
+            fpre = fcur
+            fcur = fblk
+            fblk = fpre
+        tol = xtol + rtol * fabs(xcur)
+        sbis = (xblk - xcur) / 2
+        if fabs(fcur) == 0 or fabs(sbis) < tol:
+            return xcur
+        if fabs(spre) > tol and fabs(fcur) < fabs(fpre):
+            if xpre == xblk:    # interpolate
+                stry = -fcur * (xcur - xpre) / (fcur - fpre)
+            else:               # extrapolate
+                dpre = (fpre - fcur)/(xpre - xcur)
+                dblk = (fblk - fcur)/(xblk - xcur)
+                stry = -fcur*(fblk*dblk - fpre*dpre) / (dblk*dpre*(fblk - fpre))     
+            # if (2*fabs(stry) < DMIN(fabs(spre), 3*fabs(sbis) - tol)):
+            a = fabs(spre)
+            b = 3*fabs(sbis) - tol
+            if (2*fabs(stry) < (a if a < b else b)):
+            #if (2*fabs(stry) < DMIN(fabs(spre), 3*fabs(sbis) - tol)):   
+                spre = scur
+                scur = stry  # good short step
+            else:
+                spre = sbis
+                scur = sbis  # bisect 
+        else:
+            spre = sbis
+            scur = sbis
+        xpre = xcur
+        fpre = fcur
+        if fabs(scur) > tol:
+            xcur += scur
+        else:
+            xcur += tol if sbis > 0 else -tol
+        fcur = bpf.__ccall__(xcur) + x0
+        funcalls += 1
+    outfuncalls[0] = funcalls
+    return xcur
+
+
+@cython.boundscheck(False)
+@cython.cdivision(True)
+cpdef list bpf_zero_crossings(BpfInterface b, double h=0.01, int N=0, 
+                              double x0=NAN, double x1=NAN, int maxzeros=0):
+    """
+    Return the zeros if b in the interval defined
+
+    Args:
+        b (BpfInterface): a bpf
+        h (float): the interval to scan for zeros. for each interval only one zero will be found
+        N (int): alternatively you can give the number of intervals to scan. *h* will be calculated 
+            from *N* (the *h* parameter is not used)
+        x0 (float): If given, the bounds to search within 
+        x1 (float): If given, the bounds to search within
+        maxzeros (int): if given, search will stop if this number of zeros is found
+
+    Returns:
+        (List[float]) A list of zeros (x coord points where the bpf is 0)
+    """
+    if isnan(x0):
+        x0 = b._x0
+    if isnan(x1):
+        x1 = b._x1
+    if h > (x1 - x0) * 0.5:
+        h = (x1 - x0) * 0.25
+    if N == 0:
+        N = <int>((x1 - x0) / h) + 1
+    else:
+        h = (x1 - x0) / (N - 1)
+    cdef list out = []
+    cdef double y0, y1, xa, xb, zero
+    cdef int outerror, funcalls
+    y1 = b.__ccall__(x0)
+    cdef double last_zero = 0
+    cdef int numzeros = 0
+    cdef int add_it
+    for i in range(N - 1):
+        xa = x0 + i * h
+        xb = xa + h - EPS
+        y0 = b.__ccall__(xa)
+        y1 = b.__ccall__(xb)
+        add_it = 0
+        if y0 * y1 < 0:
+            outerror = -1
+            zero = _bpf_brentq(b, 0, xa, xb, &outerror, 9.9999999999999998e-13, 4.4408920985006262e-16, 100, &funcalls)
+            if outerror == 0:
+                add_it = 1
+        elif y1 == 0 and y0 != 0:
+            zero = xb
+            add_it = 1
+        elif y0 == 0 and y1 != 0 and xa > last_zero:
+            zero = xa
+            add_it = 1
+        if add_it:
+            last_zero = zero
+            out.append(zero)
+            numzeros += 1
+            if maxzeros > 0 and numzeros >= maxzeros:
+                break
+    return out
+
+
+cdef inline double _integrate_adaptive_simpsons_inner(BpfInterface f, double a, double b, double epsilon, 
+                                                      double S, double fa, double fb, double fc, int bottom):
+    cdef: 
+        double c = (a + b) / 2
+        double h = b - a
+        double d = (a + c) / 2
+        double g = (c + b) / 2
+        double fd = f.__ccall__(d)
+        double fe = f.__ccall__(g)
+        double Sleft = (h / 12) * (fa + 4 * fd + fc)
+        double Sright = (h / 12) * (fc + 4 * fe + fb)
+    S2 = Sleft + Sright
+    if bottom <= 0 or abs(S2 - S) <= 15 * epsilon:
+        return S2 + (S2 - S) / 15.
+    return _integrate_adaptive_simpsons_inner(f, a, c, epsilon / 2, Sleft, fa, fc, fd, bottom - 1) + \
+           _integrate_adaptive_simpsons_inner(f, c, b, epsilon / 2, Sright, fc, fb, fe, bottom - 1)
+
+
+cdef double integrate_simpsons(BpfInterface f, double a, double b, double accuracy=10e-10, int max_iterations=50):
+    cdef:
+        double c = (a + b) / 2
+        double h = b - a
+        double fa = f.__ccall__(a)
+        double fb = f.__ccall__(b)
+        double fc = f.__ccall__(c)
+        double S = (h / 6) * (fa + 4 * fc + fb)
+    return _integrate_adaptive_simpsons_inner(f, a, b, accuracy, S, fa, fb, fc, max_iterations)
```

## bpf4/csvtools.py

 * *Ordering differences only*

```diff
@@ -1,221 +1,221 @@
-from __future__ import absolute_import as _absimport, division as _division
-import csv as _csv
-import os as _os
-from fractions import Fraction as _Fraction
-from collections import namedtuple as _namedtuple
-
-
-def _could_be_number(s, accept_fractions=False):
-    try:
-        n = eval(s)
-        return isinstance(n, _Number)
-    except:
-        return False
-
-def _as_number_if_possible(s, accept_fractions=True):
-    """try to convert 's' to a number if it is possible"""
-    if accept_fractions:
-        if "/" in s:
-            try:
-                n = _Fraction("/".join(n.strip() for n in s.split("/")))
-                return n
-            except:
-                return s
-    try:
-        n = int(s)
-        return n
-    except ValueError:
-        try:
-            n = float(s)
-            return n
-        except ValueError:
-            s
-    return s
-
-def replace_non_alfa(s):
-    TRANSLATION_STRING = '\x00\x01\x02\x03\x04\x05\x06\x07\x08\t\n\x0b\x0c\r\x0e\x0f\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f !"#$%&\'__x+,__/0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\\]^_`abcdefghijklmnopqrstuvwxyz{|}~\x7f\x80\x81\x82\x83\x84\x85\x86\x87\x88\x89\x8a\x8b\x8c\x8d\x8e\x8f\x90\x91\x92\x93\x94\x95\x96\x97\x98\x99\x9a\x9b\x9c\x9d\x9e\x9f\xa0\xa1\xa2\xa3\xa4\xa5\xa6\xa7\xa8\xa9\xaa\xab\xac\xad\xae\xaf\xb0\xb1\xb2\xb3\xb4\xb5\xb6\xb7\xb8\xb9\xba\xbb\xbc\xbd\xbe\xbf\xc0\xc1\xc2\xc3\xc4\xc5\xc6\xc7\xc8\xc9\xca\xcb\xcc\xcd\xce\xcf\xd0\xd1\xd2\xd3\xd4\xd5\xd6\xd7\xd8\xd9\xda\xdb\xdc\xdd\xde\xdf\xe0\xe1\xe2\xe3\xe4\xe5\xe6\xe7\xe8\xe9\xea\xeb\xec\xed\xee\xef\xf0\xf1\xf2\xf3\xf4\xf5\xf6\xf7\xf8\xf9\xfa\xfb\xfc\xfd\xfe\xff'
-    return s.translate(TRANSLATION_STRING, '[]#:')
-
-def _normalize_column_name(name):
-    name = replace_non_alfa(name)
-    if name and name[0] in '0123456789':
-        name = 'n' + name
-    name = name.strip().rstrip('_')
-    return name if name else 'untitled'
-
-def _treat_duplicates(columns):
-    names = {}
-    new_names = []
-    for column in columns:
-        if not column in names:
-            names[column] = 1
-            new_name = column
-        else:
-            n = names[column]
-            n += 1
-            names[column] = n
-            new_name = "%s_%d" % (column, n)
-        new_names.append(new_name)
-    return new_names
-
-def readcsv_numpy(csvfile):
-    """
-    Read CSV into a numpy array
-    """
-    import numpy
-    return numpy.genfromtxt(csvfile, names=True, delimiter=',')
-
-def readcsv(csvfile, rowname=None, transform_numbers=True, astuple=False, prefer_fractions=True, dialect='excel'):
-    """
-    read a CSV file into a namedtuple
-    
-    if the first collumn is all text: assume these are the column names
-    mode: in some cases you might need to set mode='U' when reading
-    files generated by excel in windows
-
-    rowname: override the row name specified in the CSV file (if any)
-    transform_numbers: convert strings to numbers if they can be converted
-    prefer_fractions: the normal behaviour to treat strings like 3/4 is to treat
-                      them as dates. If this is True, fractions will be prefered
-    astuple: do not use namedtuples, use normal tuples instead
-    """
-    assert dialect in _csv.list_dialects()
-    mode = "U"
-    f = open(csvfile, mode)
-    r = _csv.reader(f, dialect=dialect)
-    try:
-        firstrow = next(r)
-    except:
-        mode = mode + 'U'
-        f = open(csvfile, mode + 'U')
-        r = _csv.reader(f, dialect=dialect)
-        first_row = next(r)
-    attributes = {}
-    if firstrow[0].startswith('#'):
-        # the first row contains attributes
-        f.close()
-        f = open(csvfile, mode)
-        attribute_line = f.readline()
-        attrs = attribute_line[1:].split()
-        for attr in attrs:
-            key, value = attr.split(':')
-            attributes[key] = value
-        r = _csv.reader(f, dialect=dialect)
-        firstrow = next(r)
-    else:
-        attrs = None
-    if all(not _could_be_number(x) for x in firstrow) or first_row[0].startswith('#'):
-        columns = firstrow
-    else:
-        raise TypeError("""
-            Number-like cells found in the first-row. cannot assume column names
-            To load simple data you dont need this utility so use normal csv module
-            """)
-    normalized_columns = [_normalize_column_name(col) for col in columns]
-    columns = _treat_duplicates(normalized_columns)
-    if attributes:
-        a_rowname = attributes.get('rowname')
-        rowname = rowname if rowname is not None else a_rowname
-    rowname = rowname if rowname is not None else 'Row'
-    Row = _namedtuple(rowname, ' '.join(columns))
-    numcolumns = len(columns)
-    rows = []
-    for row in r:
-        if transform_numbers:
-            row = [_as_number_if_possible(cell, accept_fractions=prefer_fractions) for cell in row]
-        if not astuple:
-            if len(row) == numcolumns:
-                rows.append(Row(*row))
-            else:
-                row.extend([''] * (numcolumns - len(row)))
-                row = row[:numcolumns]
-                rows.append(Row(*row))
-        else:
-            rows.append(row)
-    return rows
-
-def read(*args, **kws):
-    import warnings
-    warnings.warn("This function has been renamed to readcsv")
-    return readcsv(*args, **kws)
-
-def readcsv_tabs(csvfile, transform_numbers=True, as_tuple=False):
-    """
-    read a csv file which uses tabs instead of commas as column-divider
-    """
-    return read(csvfile, transform_numbers=transform_numbers, as_tuple=as_tuple, dialect='excel-tab')
-
-def writecsv(namedtuples, outfile, column_names=None, write_row_name=False):
-    """
-    write a sequence of named tuples to outfile as CSV
-
-    alternatively, you can also specify the column_names. in this case it
-    is not necessary for the tuples to be be namedtuples
-    """
-    firstrow = namedtuples[0]
-    isnamedtuple = hasattr(firstrow, '_fields')
-    if isnamedtuple:
-        column_names = firstrow._fields
-    outfile = _os.path.splitext(outfile)[0] + '.csv'
-    def parse_fractions(row):
-        def parse_fraction(cell):
-            if isinstance(cell, Fraction):
-                return "0 %s" % str(cell)
-            elif isinstance(cell, str) and "/" in cell:
-                return '"%s"' % str(cell)
-            return cell
-        row = list(map(parse_fraction, row))
-        return row
-    f = open(outfile, 'wb')
-    f_write = f.write
-    w = _csv.writer(f)
-    if isnamedtuple and write_row_name:
-        try:
-            rowname = firstrow.__doc__.split('(')[0] # <-- this is a hack! where is the name of a namedtuple??
-        except AttributeError:  # maybe not a namedtuple in the end
-            rowname = firstrow.__class__.__name__
-        line = "# rowname:%s\n" % rowname
-        f_write(line)
-    if column_names:
-        w.writerow(column_names)
-    for row in namedtuples:
-        try:
-            w.writerow(row)
-        except:
-            w.writerow(tuple(row))
-    f.close()
-
-def _to_number(x, accept_fractions=True):
-    if _could_be_number(x, accept_fractions=accept_fractions):
-        if '.' in x or x in ('nan', 'inf', '-inf'):
-            return float(x)
-        else:
-            try:
-                return int(x)
-            except:
-                try:
-                    return _Fraction(x)
-                except:
-                    return x
-    else:
-        return x
-
-# class NamedTuples(list):
-#     def __init__(self, column_names, row_name='_'):
-#         self.factory = _namedtuple(row_name, column_names)
-#         if isinstance(column_names, basestring):
-#             column_names = [name.strip() for name in (column_names.split(',') if ',' in column_names else column_names.split())]
-#         self.column_names = column_names
-#     def append(self, *args, **keys):
-#         list.append(self, self.factory(*args, **keys))
-#     def writecsv(self, outfile):
-#         writecsv(self, outfile, self.column_names)
-#     @classmethod
-#     def readcsv(self, csvfile):
-#         rows = read(csvfile)
-#         row_name = '_'
-#         column_names = ' '.join(rows[0]._fields)
-#         out = NamedTuples(row_name, column_names)
-#         out.extend(rows)
-#         return out
-
+from __future__ import absolute_import as _absimport, division as _division
+import csv as _csv
+import os as _os
+from fractions import Fraction as _Fraction
+from collections import namedtuple as _namedtuple
+
+
+def _could_be_number(s, accept_fractions=False):
+    try:
+        n = eval(s)
+        return isinstance(n, _Number)
+    except:
+        return False
+
+def _as_number_if_possible(s, accept_fractions=True):
+    """try to convert 's' to a number if it is possible"""
+    if accept_fractions:
+        if "/" in s:
+            try:
+                n = _Fraction("/".join(n.strip() for n in s.split("/")))
+                return n
+            except:
+                return s
+    try:
+        n = int(s)
+        return n
+    except ValueError:
+        try:
+            n = float(s)
+            return n
+        except ValueError:
+            s
+    return s
+
+def replace_non_alfa(s):
+    TRANSLATION_STRING = '\x00\x01\x02\x03\x04\x05\x06\x07\x08\t\n\x0b\x0c\r\x0e\x0f\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f !"#$%&\'__x+,__/0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\\]^_`abcdefghijklmnopqrstuvwxyz{|}~\x7f\x80\x81\x82\x83\x84\x85\x86\x87\x88\x89\x8a\x8b\x8c\x8d\x8e\x8f\x90\x91\x92\x93\x94\x95\x96\x97\x98\x99\x9a\x9b\x9c\x9d\x9e\x9f\xa0\xa1\xa2\xa3\xa4\xa5\xa6\xa7\xa8\xa9\xaa\xab\xac\xad\xae\xaf\xb0\xb1\xb2\xb3\xb4\xb5\xb6\xb7\xb8\xb9\xba\xbb\xbc\xbd\xbe\xbf\xc0\xc1\xc2\xc3\xc4\xc5\xc6\xc7\xc8\xc9\xca\xcb\xcc\xcd\xce\xcf\xd0\xd1\xd2\xd3\xd4\xd5\xd6\xd7\xd8\xd9\xda\xdb\xdc\xdd\xde\xdf\xe0\xe1\xe2\xe3\xe4\xe5\xe6\xe7\xe8\xe9\xea\xeb\xec\xed\xee\xef\xf0\xf1\xf2\xf3\xf4\xf5\xf6\xf7\xf8\xf9\xfa\xfb\xfc\xfd\xfe\xff'
+    return s.translate(TRANSLATION_STRING, '[]#:')
+
+def _normalize_column_name(name):
+    name = replace_non_alfa(name)
+    if name and name[0] in '0123456789':
+        name = 'n' + name
+    name = name.strip().rstrip('_')
+    return name if name else 'untitled'
+
+def _treat_duplicates(columns):
+    names = {}
+    new_names = []
+    for column in columns:
+        if not column in names:
+            names[column] = 1
+            new_name = column
+        else:
+            n = names[column]
+            n += 1
+            names[column] = n
+            new_name = "%s_%d" % (column, n)
+        new_names.append(new_name)
+    return new_names
+
+def readcsv_numpy(csvfile):
+    """
+    Read CSV into a numpy array
+    """
+    import numpy
+    return numpy.genfromtxt(csvfile, names=True, delimiter=',')
+
+def readcsv(csvfile, rowname=None, transform_numbers=True, astuple=False, prefer_fractions=True, dialect='excel'):
+    """
+    read a CSV file into a namedtuple
+    
+    if the first collumn is all text: assume these are the column names
+    mode: in some cases you might need to set mode='U' when reading
+    files generated by excel in windows
+
+    rowname: override the row name specified in the CSV file (if any)
+    transform_numbers: convert strings to numbers if they can be converted
+    prefer_fractions: the normal behaviour to treat strings like 3/4 is to treat
+                      them as dates. If this is True, fractions will be prefered
+    astuple: do not use namedtuples, use normal tuples instead
+    """
+    assert dialect in _csv.list_dialects()
+    mode = "U"
+    f = open(csvfile, mode)
+    r = _csv.reader(f, dialect=dialect)
+    try:
+        firstrow = next(r)
+    except:
+        mode = mode + 'U'
+        f = open(csvfile, mode + 'U')
+        r = _csv.reader(f, dialect=dialect)
+        first_row = next(r)
+    attributes = {}
+    if firstrow[0].startswith('#'):
+        # the first row contains attributes
+        f.close()
+        f = open(csvfile, mode)
+        attribute_line = f.readline()
+        attrs = attribute_line[1:].split()
+        for attr in attrs:
+            key, value = attr.split(':')
+            attributes[key] = value
+        r = _csv.reader(f, dialect=dialect)
+        firstrow = next(r)
+    else:
+        attrs = None
+    if all(not _could_be_number(x) for x in firstrow) or first_row[0].startswith('#'):
+        columns = firstrow
+    else:
+        raise TypeError("""
+            Number-like cells found in the first-row. cannot assume column names
+            To load simple data you dont need this utility so use normal csv module
+            """)
+    normalized_columns = [_normalize_column_name(col) for col in columns]
+    columns = _treat_duplicates(normalized_columns)
+    if attributes:
+        a_rowname = attributes.get('rowname')
+        rowname = rowname if rowname is not None else a_rowname
+    rowname = rowname if rowname is not None else 'Row'
+    Row = _namedtuple(rowname, ' '.join(columns))
+    numcolumns = len(columns)
+    rows = []
+    for row in r:
+        if transform_numbers:
+            row = [_as_number_if_possible(cell, accept_fractions=prefer_fractions) for cell in row]
+        if not astuple:
+            if len(row) == numcolumns:
+                rows.append(Row(*row))
+            else:
+                row.extend([''] * (numcolumns - len(row)))
+                row = row[:numcolumns]
+                rows.append(Row(*row))
+        else:
+            rows.append(row)
+    return rows
+
+def read(*args, **kws):
+    import warnings
+    warnings.warn("This function has been renamed to readcsv")
+    return readcsv(*args, **kws)
+
+def readcsv_tabs(csvfile, transform_numbers=True, as_tuple=False):
+    """
+    read a csv file which uses tabs instead of commas as column-divider
+    """
+    return read(csvfile, transform_numbers=transform_numbers, as_tuple=as_tuple, dialect='excel-tab')
+
+def writecsv(namedtuples, outfile, column_names=None, write_row_name=False):
+    """
+    write a sequence of named tuples to outfile as CSV
+
+    alternatively, you can also specify the column_names. in this case it
+    is not necessary for the tuples to be be namedtuples
+    """
+    firstrow = namedtuples[0]
+    isnamedtuple = hasattr(firstrow, '_fields')
+    if isnamedtuple:
+        column_names = firstrow._fields
+    outfile = _os.path.splitext(outfile)[0] + '.csv'
+    def parse_fractions(row):
+        def parse_fraction(cell):
+            if isinstance(cell, Fraction):
+                return "0 %s" % str(cell)
+            elif isinstance(cell, str) and "/" in cell:
+                return '"%s"' % str(cell)
+            return cell
+        row = list(map(parse_fraction, row))
+        return row
+    f = open(outfile, 'wb')
+    f_write = f.write
+    w = _csv.writer(f)
+    if isnamedtuple and write_row_name:
+        try:
+            rowname = firstrow.__doc__.split('(')[0] # <-- this is a hack! where is the name of a namedtuple??
+        except AttributeError:  # maybe not a namedtuple in the end
+            rowname = firstrow.__class__.__name__
+        line = "# rowname:%s\n" % rowname
+        f_write(line)
+    if column_names:
+        w.writerow(column_names)
+    for row in namedtuples:
+        try:
+            w.writerow(row)
+        except:
+            w.writerow(tuple(row))
+    f.close()
+
+def _to_number(x, accept_fractions=True):
+    if _could_be_number(x, accept_fractions=accept_fractions):
+        if '.' in x or x in ('nan', 'inf', '-inf'):
+            return float(x)
+        else:
+            try:
+                return int(x)
+            except:
+                try:
+                    return _Fraction(x)
+                except:
+                    return x
+    else:
+        return x
+
+# class NamedTuples(list):
+#     def __init__(self, column_names, row_name='_'):
+#         self.factory = _namedtuple(row_name, column_names)
+#         if isinstance(column_names, basestring):
+#             column_names = [name.strip() for name in (column_names.split(',') if ',' in column_names else column_names.split())]
+#         self.column_names = column_names
+#     def append(self, *args, **keys):
+#         list.append(self, self.factory(*args, **keys))
+#     def writecsv(self, outfile):
+#         writecsv(self, outfile, self.column_names)
+#     @classmethod
+#     def readcsv(self, csvfile):
+#         rows = read(csvfile)
+#         row_name = '_'
+#         column_names = ' '.join(rows[0]._fields)
+#         out = NamedTuples(row_name, column_names)
+#         out.extend(rows)
+#         return out
+
```

## bpf4/plot.py

 * *Ordering differences only*

```diff
@@ -1,143 +1,143 @@
-from __future__ import annotations
-from .config import CONFIG
-import matplotlib.pyplot as plt
-import numpy as np
-
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from typing import Sequence, Union
-    from bpf4 import core
-
-
-def plot_coords(xs: Union[list[float], np.ndarray],
-                ys: Union[list[float], np.ndarray],
-                show:bool=None, 
-                kind='line', 
-                axes: plt.Axes = None,
-                figsize:tuple(float, float)=None,
-                **keys
-                ) -> plt.Axes:
-    """
-    Plot the points defined by xs and ys
-
-    Args:
-        xs: a seq. of x coords
-        ys: a seq. of y coords
-        kind: one of line or bar
-        axes: if given, this axes is used
-        figsize: as passed to pyplot.figure(...), a tuple (width, height). This setting
-            only has effect if axes is not given
-        keys: any keywords will be bassed to `axes.plot` (or `axes.bar` depending
-            on `kind`)
-
-    Returns:
-        the matplotlib's Axes object used. If it was passed as the axes
-        arg, then the returned axes will be this same Axes object
-
-    """
-    if not axes:
-        if figsize:
-            fig, axes = plt.subplots(figsize=figsize)
-        else:
-            fig, axes = plt.subplots()
-    if kind == 'line':
-        axes.plot(xs, ys, **keys)
-    elif kind == 'bar':
-        axes.bar(xs, ys, **keys)
-    elif kind == 'stem':
-        axes.stem(xs, ys, **keys) 
-    plot_always_show = CONFIG['plot.always_show']
-    if plot_always_show and (show is None or show is True):
-        if axes:
-            axes.show()
-        else:
-            plt.show()
-    elif not plot_always_show and show is True:
-        plt.show()
-    return axes
-
-        
-def bpfplot(*bpfs: core.BpfInterface, npoints=400, show=True, **kws) -> None:
-    """
-    Plot one/multiple bpfs
-
-    Args:
-        bpfs: one or more bpfs to be plotted
-        npoints: number of points to be used for the plot
-        show: should the plot be plot immediately. else you can call show yourself
-        kws: any keywords are passed to `plt.plot`
-    """
-    x0 = min(bpf.bounds()[0] for bpf in bpfs)
-    x1 = max(bpf.bounds()[1] for bpf in bpfs)
-    xs = np.linspace(x0, x1, npoints)
-    yss = [bpf.map(xs) for bpf in bpfs]
-    args = []
-    for ys in yss:
-        args.extend((xs, ys))
-    plt.plot(*args, **kws)
-    if show:
-        plt.show()
-
-        
-def plot_stacked(*bpfs: core.BpfInterface, **kws) -> None:
-    """
-    Example
-    -------
-
-    ```python
-    
-    a = bpf.linear(0,0, 1,1)
-    b = bpf.halfcos(0, 0, 0.5, 1, 1, 0)
-    
-    plot_stacked(a, (b, 'b'))
-    ```
-
-    """
-    min_x = float('inf')
-    max_x = -float('inf')
-    bpfs2, labels = [], []
-    for i, bpf in enumerate(bpfs):
-        if isinstance(bpf, (tuple, list)):
-            bpf, label = bpf
-        else:
-            label = str(i + 1)
-        bpfs2.append(bpf)
-        labels.append(label)
-        x0, x1 = bpf.bounds()
-        if x0 < min_x:
-            min_x = x0
-        if x1 > max_x:
-            max_x = x1
-    N = 2000
-    xs = np.linspace(min_x, max_x, N)
-    yss = [bpf[min_x:max_x].map(N) for bpf in bpfs2]
-    y_data = np.row_stack(yss)
-    y_data_stacked = np.cumsum(y_data, axis=0)
-    fig = plt.figure()
-    ax1 = fig.add_subplot(111)
-    split_lines = [(0, y_data_stacked[0,:])]
-    COLORTHEME = (
-        '#CC6666',
-        '#1DACD6',
-        '#6E5160',
-        '#FF22FF',
-        '#66FF88',
-        '#FF2266',
-        '#444444'
-    )
-    for i in range(len(bpfs) - 1):
-        split_lines.append((y_data_stacked[i,:], y_data_stacked[i+1,:]))
-    facecolors = COLORTHEME[:len(bpfs)]
-    for i in range(len(bpfs)):
-        y0, y1 = split_lines[i]
-        color = facecolors[i]
-        ax1.fill_between(xs, y0, y1, facecolor=color, alpha=0.9, label=labels[i])
-        ax1.plot(xs, y1, lw=3, label=labels[i],color=color)
-    ax1.legend(loc='upper left')
-    if kws.get('show'):
-        plt.show()
-
-        
-def show() -> None:
-    """Show the plotted bpfs"""
-    plt.show()
+from __future__ import annotations
+from .config import CONFIG
+import matplotlib.pyplot as plt
+import numpy as np
+
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from typing import Sequence, Union
+    from bpf4 import core
+
+
+def plot_coords(xs: Union[list[float], np.ndarray],
+                ys: Union[list[float], np.ndarray],
+                show:bool=None, 
+                kind='line', 
+                axes: plt.Axes = None,
+                figsize:tuple(float, float)=None,
+                **keys
+                ) -> plt.Axes:
+    """
+    Plot the points defined by xs and ys
+
+    Args:
+        xs: a seq. of x coords
+        ys: a seq. of y coords
+        kind: one of line or bar
+        axes: if given, this axes is used
+        figsize: as passed to pyplot.figure(...), a tuple (width, height). This setting
+            only has effect if axes is not given
+        keys: any keywords will be bassed to `axes.plot` (or `axes.bar` depending
+            on `kind`)
+
+    Returns:
+        the matplotlib's Axes object used. If it was passed as the axes
+        arg, then the returned axes will be this same Axes object
+
+    """
+    if not axes:
+        if figsize:
+            fig, axes = plt.subplots(figsize=figsize)
+        else:
+            fig, axes = plt.subplots()
+    if kind == 'line':
+        axes.plot(xs, ys, **keys)
+    elif kind == 'bar':
+        axes.bar(xs, ys, **keys)
+    elif kind == 'stem':
+        axes.stem(xs, ys, **keys) 
+    plot_always_show = CONFIG['plot.always_show']
+    if plot_always_show and (show is None or show is True):
+        if axes:
+            axes.show()
+        else:
+            plt.show()
+    elif not plot_always_show and show is True:
+        plt.show()
+    return axes
+
+        
+def bpfplot(*bpfs: core.BpfInterface, npoints=400, show=True, **kws) -> None:
+    """
+    Plot one/multiple bpfs
+
+    Args:
+        bpfs: one or more bpfs to be plotted
+        npoints: number of points to be used for the plot
+        show: should the plot be plot immediately. else you can call show yourself
+        kws: any keywords are passed to `plt.plot`
+    """
+    x0 = min(bpf.bounds()[0] for bpf in bpfs)
+    x1 = max(bpf.bounds()[1] for bpf in bpfs)
+    xs = np.linspace(x0, x1, npoints)
+    yss = [bpf.map(xs) for bpf in bpfs]
+    args = []
+    for ys in yss:
+        args.extend((xs, ys))
+    plt.plot(*args, **kws)
+    if show:
+        plt.show()
+
+        
+def plot_stacked(*bpfs: core.BpfInterface, **kws) -> None:
+    """
+    Example
+    -------
+
+    ```python
+    
+    a = bpf.linear(0,0, 1,1)
+    b = bpf.halfcos(0, 0, 0.5, 1, 1, 0)
+    
+    plot_stacked(a, (b, 'b'))
+    ```
+
+    """
+    min_x = float('inf')
+    max_x = -float('inf')
+    bpfs2, labels = [], []
+    for i, bpf in enumerate(bpfs):
+        if isinstance(bpf, (tuple, list)):
+            bpf, label = bpf
+        else:
+            label = str(i + 1)
+        bpfs2.append(bpf)
+        labels.append(label)
+        x0, x1 = bpf.bounds()
+        if x0 < min_x:
+            min_x = x0
+        if x1 > max_x:
+            max_x = x1
+    N = 2000
+    xs = np.linspace(min_x, max_x, N)
+    yss = [bpf[min_x:max_x].map(N) for bpf in bpfs2]
+    y_data = np.row_stack(yss)
+    y_data_stacked = np.cumsum(y_data, axis=0)
+    fig = plt.figure()
+    ax1 = fig.add_subplot(111)
+    split_lines = [(0, y_data_stacked[0,:])]
+    COLORTHEME = (
+        '#CC6666',
+        '#1DACD6',
+        '#6E5160',
+        '#FF22FF',
+        '#66FF88',
+        '#FF2266',
+        '#444444'
+    )
+    for i in range(len(bpfs) - 1):
+        split_lines.append((y_data_stacked[i,:], y_data_stacked[i+1,:]))
+    facecolors = COLORTHEME[:len(bpfs)]
+    for i in range(len(bpfs)):
+        y0, y1 = split_lines[i]
+        color = facecolors[i]
+        ax1.fill_between(xs, y0, y1, facecolor=color, alpha=0.9, label=labels[i])
+        ax1.plot(xs, y1, lw=3, label=labels[i],color=color)
+    ax1.legend(loc='upper left')
+    if kws.get('show'):
+        plt.show()
+
+        
+def show() -> None:
+    """Show the plotted bpfs"""
+    plt.show()
```

## bpf4/pyinterp.py

 * *Ordering differences only*

```diff
@@ -1,45 +1,45 @@
-from __future__ import annotations
-from . import core
-import numpy as np
-OUTBOUND_CACHE = 1
-
-
-class _NumpyInterp(core._FunctionWrap_Object):
-    
-    def __init__(self, interpolator, xs, ys):
-        self._interpolator = interpolator
-        super(_NumpyInterp, self).__init__(interpolator, (xs[0], xs[-1]))
-        self.xs, self.ys = xs, ys
-
-    def mapn_between(self, n, x0, x1, out=None):
-        xs = np.linspace(x0, x1, n)
-        out0 = self._interpolator(xs)
-        if out is not None:
-            out[...] = out0
-            return out
-        return out0
-    
-    def map(self, xs, out=None):
-        if isinstance(xs, int):
-            return self.mapn_between(xs, self.x0, self.x1)
-        return self._interpolator(xs)
-    
-    def points(self):
-        return [self.xs, self.ys]
-    
-    def __getstate__(self):
-        return self.xs, self.ys
-    
-    def _slice(self, x0, x1):
-        return core._BpfCrop_new(self, x0, x1, OUTBOUND_CACHE)
-
-
-class Pchip(_NumpyInterp):
-    """
-    Monotonic Piecewise Cubit Hermite interpolation, similar to matlab's pchip
-    """
-    def __init__(self, xs: np.ndarray, ys: np.ndarray):
-        from scipy.interpolate import PchipInterpolator
-        interpolator = PchipInterpolator(xs, ys)
-        super().__init__(interpolator, xs, ys)
-
+from __future__ import annotations
+from . import core
+import numpy as np
+OUTBOUND_CACHE = 1
+
+
+class _NumpyInterp(core._FunctionWrap_Object):
+    
+    def __init__(self, interpolator, xs, ys):
+        self._interpolator = interpolator
+        super(_NumpyInterp, self).__init__(interpolator, (xs[0], xs[-1]))
+        self.xs, self.ys = xs, ys
+
+    def mapn_between(self, n, x0, x1, out=None):
+        xs = np.linspace(x0, x1, n)
+        out0 = self._interpolator(xs)
+        if out is not None:
+            out[...] = out0
+            return out
+        return out0
+    
+    def map(self, xs, out=None):
+        if isinstance(xs, int):
+            return self.mapn_between(xs, self.x0, self.x1)
+        return self._interpolator(xs)
+    
+    def points(self):
+        return [self.xs, self.ys]
+    
+    def __getstate__(self):
+        return self.xs, self.ys
+    
+    def _slice(self, x0, x1):
+        return core._BpfCrop_new(self, x0, x1, OUTBOUND_CACHE)
+
+
+class Pchip(_NumpyInterp):
+    """
+    Monotonic Piecewise Cubit Hermite interpolation, similar to matlab's pchip
+    """
+    def __init__(self, xs: np.ndarray, ys: np.ndarray):
+        from scipy.interpolate import PchipInterpolator
+        interpolator = PchipInterpolator(xs, ys)
+        super().__init__(interpolator, xs, ys)
+
```

## bpf4/tests.py

 * *Ordering differences only*

```diff
@@ -1,47 +1,47 @@
-#!/usr/bin/env python
-# encoding: utf-8
-"""
-tests.py
-
-"""
-
-import bpf4 as bpf
-import random
-
-N = 1000
-EPSILON = 0.000001
-
-def random_floats(n, rnge):
-    x0, x1 = rnge
-    return [random.random() * (x1 - x0) + x0 for n in range(n)]
-    
-def assert_almost_equal(a, b):
-    assert abs(a - b) < EPSILON
-
-def test_aritm():
-    a = bpf.Linear((0, 10), (0, 100))
-    cases = random_floats(n=N, rnge=(-10, 20))
-    for x in cases:
-        try:
-            print(x)
-            assert a(x) + 10 == (a + 10)(x)
-            assert a(x) - 13.5 == (a - 13.5)(x)
-            assert a(x) * 0.5 == (a * 0.5)(x)
-            assert a(x) / 8.3 == (a / 8.3)(x)
-            assert a(x) * a(x) == (a * a)(x)
-            assert a(x) + a(x) == (a + a)(x)
-            assert a(x) - a(x) * 2 == (a - a(x) * 2)(x) == (a - a * 2)(x)
-            assert a(x) / (a(x) - 1) == (a / (a - 1))(x)
-            assert a(x) ** x == (a ** x)(x)
-            assert float(a(x) > 5) == float((a > 5)(x))
-            assert float(a(x) >= 5) == float((a >= 5)(x))
-            assert float(a(x) < 1.3) == float((a < 1.3)(x))
-            assert float(a(x) <= 1.3) == float((a <= 1.3)(x))
-            assert abs(a(x) * -1) == abs(a * -1)(x)
-            assert_almost_equal(  a(x) * 10, (a + a + a + a + a + a + a + a + a + a)(x)  )    
-        except ZeroDivisionError:
-            pass
-    #assert all(a(x) == x ** 2
-    
-if __name__ == '__main__':
+#!/usr/bin/env python
+# encoding: utf-8
+"""
+tests.py
+
+"""
+
+import bpf4 as bpf
+import random
+
+N = 1000
+EPSILON = 0.000001
+
+def random_floats(n, rnge):
+    x0, x1 = rnge
+    return [random.random() * (x1 - x0) + x0 for n in range(n)]
+    
+def assert_almost_equal(a, b):
+    assert abs(a - b) < EPSILON
+
+def test_aritm():
+    a = bpf.Linear((0, 10), (0, 100))
+    cases = random_floats(n=N, rnge=(-10, 20))
+    for x in cases:
+        try:
+            print(x)
+            assert a(x) + 10 == (a + 10)(x)
+            assert a(x) - 13.5 == (a - 13.5)(x)
+            assert a(x) * 0.5 == (a * 0.5)(x)
+            assert a(x) / 8.3 == (a / 8.3)(x)
+            assert a(x) * a(x) == (a * a)(x)
+            assert a(x) + a(x) == (a + a)(x)
+            assert a(x) - a(x) * 2 == (a - a(x) * 2)(x) == (a - a * 2)(x)
+            assert a(x) / (a(x) - 1) == (a / (a - 1))(x)
+            assert a(x) ** x == (a ** x)(x)
+            assert float(a(x) > 5) == float((a > 5)(x))
+            assert float(a(x) >= 5) == float((a >= 5)(x))
+            assert float(a(x) < 1.3) == float((a < 1.3)(x))
+            assert float(a(x) <= 1.3) == float((a <= 1.3)(x))
+            assert abs(a(x) * -1) == abs(a * -1)(x)
+            assert_almost_equal(  a(x) * 10, (a + a + a + a + a + a + a + a + a + a)(x)  )    
+        except ZeroDivisionError:
+            pass
+    #assert all(a(x) == x ** 2
+    
+if __name__ == '__main__':
     test_aritm()
```

## bpf4/util.py

 * *Ordering differences only*

```diff
@@ -1,1109 +1,1109 @@
-"""
-Utilities for bpf4
-"""
-from __future__ import annotations
-import operator as _operator
-import os as _os
-import itertools as _itertools
-from functools import reduce
-from typing import Sequence
-
-import numpy as np
-from scipy.integrate import quad as _quad
-from scipy.optimize import brentq as _brentq
-from . import core
-
-
-_CSV_COLUMN_NAMES = ('x', 'y', 'interpolation', 'exponent')
-
-
-_CONSTRUCTORS = {
-    'linear': core.Linear,
-    'expon': core.Expon,
-    'halfcos': core.Halfcos,
-    'nointerpol': core.NoInterpol,
-    'spline': core.Spline,
-    'uspline': core.USpline,
-    'slope': core.Slope,
-    'nearest': core.Nearest,
-    'halfcosm': core.Halfcosm,
-    'smooth': core.Smooth,
-    'smoother': core.Smoother
-}
-
-
-def _isiterable(obj) -> bool:
-    try:
-        iter(obj)
-        return not isinstance(obj, str)
-    except TypeError:
-        return False
-
-
-def _iflatten(seq):
-    """
-    Return an iterator to the flattened items of sequence s
-    
-    Strings are not flattened
-    """
-    try:
-        iter(seq)
-    except TypeError:
-        yield seq
-    else:
-        for elem in seq:
-            if isinstance(elem, str):
-                yield elem
-            else:
-                for subelem in _iflatten(elem):
-                    yield subelem
-
-def csv_to_bpf(csvfile: str) -> core.BpfInterface:
-    """
-    Read a bpf from a csv file
-    """
-    from emlib import csvtools
-    rows = csvtools.readcsv(csvfile)
-    interpolation = rows[0].interpolation
-    if all(row.interpolation == interpolation for row in rows[:-1]):
-        # all of the same type
-        if interpolation in ('expon', 'halfcosexp', 'halfcos2'):
-            exp = rows[0].exponent
-            constructor = get_bpf_constructor("%s(%.3f)" % (interpolation, exp))
-        else:
-            constructor = get_bpf_constructor(interpolation)
-        numrows = len(rows)
-        xs = np.empty((numrows,), dtype=float)
-        ys = np.empty((numrows,), dtype=float)
-        for i in range(numrows):
-            r = rows[i]
-            xs[i] = r.x
-            ys[i] = r.y
-        return constructor(xs, ys)
-    else:
-        # multitype
-        raise NotImplementedError("BPFs with multiple types not implemented YET")
-
-
-def bpf_to_csv(bpf: core.BpfInterface, csvfile: str) -> None:
-    """
-    Write this bpf as a csv representation
-
-    Args:
-        bpf: the bpf to write as csv
-        csvfile: the output filename
-    """
-    import csv
-    csvfile = _os.path.splitext(csvfile)[0] + '.csv'
-    try:
-        # it follows the 'segments' protocol, returning a seq of (x, y, interpoltype, exp)
-        segments = bpf.segments()
-        with open(csvfile, 'w') as f:
-            writer = csv.writer(f)
-            writer.writerow(_CSV_COLUMN_NAMES)
-            writer.writerows(segments)
-    except AttributeError:
-        raise TypeError("BPF must be rendered in order to be written as CSV")
-
-
-def bpf_to_dict(bpf: core.BpfInterface) -> dict:
-    """
-    convert a bpf to a dict with the following format
-
-    Args:
-        bpf: the bpf to convert to a dict
-
-    Returns:
-        (dict) The bpf as a dictionary
-
-    ```python
-
-    >>> b = bpf.expon(3.0, 0, 0, 1, 10, 2, 20)
-    >>> bpf_to_dict(b)
-    {
-        'interpolation': 'expon(3.0)',
-        'points': [0, 0, 1, 10, 20, 20]  # [x0, y0, x1, y1, ...]
-    }
-
-    >>> b = bpf.multi(0, 0, 'linear',
-                      1, 10, 'expon(2)',
-                      3, 25)
-    >>> bpf_to_dict(b)
-    {
-        'interpolation': 'multi',
-        'segments': [
-            [0, 0, 'linear'],
-            [1, 10, 'expon(2)',
-            [3, 25, '']]
-    }
-    ```
-    """
-    try:
-        segments = list(bpf.segments())
-    except:
-        raise TypeError("this kind of BPF cannot be translated. It must be rendered first.")
-    d = {}
-    interpolation = segments[0][2]
-    # x y interpolation exp
-
-    def normalize_segment(segment):
-        """
-        a segment as returned by .segments() is [x, y, interpl, exp]
-        we want [x, y, interpol(exp)]
-        """
-        if len(segment) == 4:
-            x, y, interpol, exp = segment
-            if not interpol and exp == 0:
-                # the last segment of a multi bpf
-                segment = [x, y]
-            else:
-                interpol = "{interpol}({exp})".format(interpol=interpol, exp=exp)
-                segment = [x, y, interpol]
-        return segment
-
-    if not all(segment[2] == interpolation for segment in segments[:-1]):
-        # multi
-        d['interpolation'] = 'multi'
-        segments = [normalize_segment(seg) for seg in segments]
-        d['segments'] = segments
-    else:
-        try:
-            exp = bpf.exp
-            if exp != 1:
-                assert "(" not in interpolation
-                interpolation = "{interp}({exp})".format(interp=interpolation, exp=exp)
-        except AttributeError:
-            pass
-        d['interpolation'] = interpolation
-        points = []
-        for segment in segments:
-            points.append(segment[0])
-            points.append(segment[1])
-        d['points'] = points
-    return d
-
-
-def bpf_to_json(bpf: core.BpfInterface, outfile: str = None) -> str:
-    """
-    convert this bpf to json format.
-
-    If outfile is not given, it returns a string, as in dumps
-
-    Args:
-        bpf: the bpf to dump as json
-        outfile: the output filename. If given, output is saved here
-
-    Returns:
-        (str) The json text
-    """
-    import json
-    asdict = bpf_to_dict(bpf)
-    jsontxt = json.dumps(asdict)
-    if outfile:
-        open(outfile, 'w').write(jsontxt)
-    return jsontxt
-        
-
-def bpf_to_yaml(bpf: core.BpfInterface, outfile: str = None) -> str:
-    """
-    Convert this bpf to json format. 
-
-    Args:
-        bpf: the bpf to convert
-        outfile: if given, the yaml text is saved to this file
-
-    Returns:
-        (str) The yaml text
-    """
-    from io import StringIO
-    import yaml
-    d = bpf_to_dict(bpf)
-    if outfile is None:
-        stream = StringIO()
-    else:
-        outfile = _os.path.splitext(outfile)[0] + '.yaml'
-        stream = open(outfile, 'w')
-    dumper = yaml.Dumper(stream)
-    dumper.add_representer(tuple, lambda du, instance: du.represent_list(instance))
-    dumper.add_representer(np.float64, lambda du, instance: du.represent_float(instance))
-    dumper.open()
-    dumper.represent(d)
-    dumper.close()
-    return stream.getvalue()
-
-
-def dict_to_bpf(d: dict) -> bpf.BpfInterface:
-    """
-    Convert a dict to a bpf
-
-    Args:
-        d: the dictionary to convert to a bpf
-
-    Returns:
-        the converted bpf
-
-
-    **Format 1** 
-
-    ```python
-
-    bpf = {
-        'interpolation': 'expon(2)',
-        10: 0.1,
-        15: 1,
-        25: -1
-    }
-    ```
-
-    **Format 2**
-
-    ```python
-    bpf = {
-        'interpolation': 'linear',
-        'points': [x0, y0, x1, y1, ...]
-    }
-    ```
-
-    **Format 2b**
-
-    ```python
-    bpf = {
-        'interpolation': 'linear',
-        'points': [(x0, y0), (x1, y1), ...]
-    }
-    ```
-
-    **Format 3 (multi)**
-
-    ```python
-
-    bpf = {
-        'interpolation': 'multi',
-        'segments': [
-            [x0, y0, 'descr0'],
-            [x1, y1, 'descr1'],
-            ...
-            [xn, yn, '']
-        ]
-    }
-    ```
-    """
-
-    # check format
-    if 'points' in d:
-        # format 2
-        interpolation = d.get('interpolation', 'linear')
-        constructor = get_bpf_constructor(interpolation)
-        points = d['points']
-        if isinstance(points[0], (int, float)):
-            # format 2a
-            X = points[::2]
-            Y = points[1::2]
-        elif isinstance(points[0], (list, tuple)):
-            X = [point[0] for point in points]
-            Y = [point[1] for point in points]
-        return constructor.fromxy(X, Y)
-    elif 'segments' in d and d['interpolation'] == 'multi':
-        segments = d['segments']
-        X = [s[0] for s in segments]
-        Y = [s[1] for s in segments]
-        interpolations = [s[2] for s in segments[:-1]]
-        return core.Multi(X, Y, interpolations)
-    else:
-        # format 1
-        interpolation = d.get('interpolation', 'linear')
-        constructor = get_bpf_constructor(interpolation)
-        points = [(k, v) for k, v in d.items() if isinstance(k, (int, float))]
-        points.sort()
-        X, Y = list(zip(*points))
-        return constructor.fromxy(X, Y)
-
-
-def loadbpf(path: str, fmt='auto') -> core.BpfInterface:
-    """
-    Load a bpf saved with dumpbpf
-
-    Possible formats: auto, csv, yaml, json
-
-    Args:
-        path: the path of the saved bpf
-        fmt: the format used to save the bpf ('auto' to detect the format)
-
-    Returns:
-        a bpf
-    """
-    if fmt == 'auto':
-        fmt = _os.path.splitext(path)[-1].lower()[1:]
-    assert fmt in ('csv', 'yaml', 'json')
-    if fmt == 'yaml':
-        import yaml
-        d = yaml.load(open(path))
-    elif fmt == 'json':
-        import json
-        d = json.load(path)
-    elif fmt == 'csv':
-        return csv_to_bpf(path)
-    return dict_to_bpf(d)  
-
-
-def asbpf(obj, bounds=(-np.inf, np.inf)) -> core.BpfInterface:
-    """
-    Convert obj to a bpf
-
-    obj can be a function, a dict, a constant, or a bpf (in which case it
-    is returned as is)
-    """
-    if isinstance(obj, core.BpfInterface):
-        return obj
-    elif callable(obj):
-        return core._FunctionWrap(obj, bounds)
-    elif hasattr(obj, '__float__'):
-        return core.Const(float(obj))
-    else:
-        raise TypeError("can't wrap %s" % str(obj))
- 
-
-def parseargs(*args, **kws) -> tuple[list[float], list[float], dict]:
-    """
-    Convert the args and kws to the canonical form (xs, ys, kws)
-    
-    Returns:
-        (tuple[list[float], list[float], dict]) A tuple `(xs, ys, kws)`
-    
-    Raises ValueError if failed
-
-    All the following variants result in the same result:
-
-    ```python
-
-    x0, y0, x1, y1, …, exp=0.5
-    (x0, y0), (x1, y1), …, exp=0.5           
-    {x0:y0, x1:y1, …}, exp=0.5               
-    [x0, x1, …], [y0, y1, …], exp=0.5        
-    
-    Result: [x0, x1, …], [y0, y1, …], {exp:0.5}
-    ```
-    """
-    L = len(args)
-    if L == 0:
-        raise ValueError("no arguments given")
-    elif L == 1:
-        d = args[0]
-        assert isinstance(d, dict)
-        items = list(d.items())
-        items.sort()
-        xs, ys = list(zip(*items))
-    elif L == 2:
-        if not all(map(_isiterable, args)):
-            raise ValueError(f"parsing error: 2 args, expected a seq. "
-                             f"[(x0, y1), (x1, y1)] or (xs, ys) but got {args}")
-        if len(args[0]) > 2:   # <--  (xs, ys)
-            xs, ys = args
-        else:                  # <--  ((x0, y0), (x1, y1), ...)
-            xs, ys = list(zip(*args))    
-    elif not any(map(_isiterable, args)):
-        # (x0, y0, x1, y1, ...)
-        if L % 2 == 0:  # even
-            xs = args[::2]
-            ys = args[1::2]
-        else:
-            if kws:
-                raise ValueError(f"Uneven number of args. No keywords allowed in "
-                                 f"this case, but got {kws}")
-            kws = {'exp': args[0]}
-            xs = args[1::2]
-            ys = args[2::2]
-    elif all(map(_isiterable, args)):   # <-- ((x0, y0), (x1, y1), ...)
-        xs, ys = list(zip(*args))
-    else:
-        raise ValueError("could not parse arguments")
-    return xs, ys, kws
-        
-
-
-def parsedescr(descr: str, validate=True) -> tuple[str, dict]:
-    """
-    Parse interpolation description
-
-
-    | descr                   | output                             |
-    |-------------------------|------------------------------------|
-    | linear                  | linear, {}                         |
-    | expon(0.4)              | expon, {'exp': 0.4}                |
-    | halfcos(2.5, numiter=1) | halfcos, {'exp':2.5, 'numiter': 1} |
-
-    """
-    if "(" not in descr:
-        classname = descr
-        kws = {}
-    else:
-        classname, rest = descr.split("(")
-        assert rest[-1] == ")"
-        rest = rest[:-1]
-        parts = rest.split(",")
-        kws = {}
-        for part in parts:
-            if "=" in part:
-                key, value = part.split("=")
-                kws[key] = float(value)
-            else:
-                assert 'exp' not in kws
-                kws['exp'] = float(part)
-    if validate:
-        assert classname in _CONSTRUCTORS
-    return classname, kws
-
-
-def makebpf(descr: str, X: Sequence[float], Y: Sequence[float]) -> core.BpfInterface:
-    """
-    Create a bpf from the given descriptor and points
-
-    Args:
-        descr: a string descriptor of the interpolation ("linear", "expon(xx)", ...)
-        X: the array of xs
-        Y: the array of ys
-
-    Returns:
-        the created bpf
-    """
-    interpolkind, kws = parsedescr(descr)
-    bpfclass = _CONSTRUCTORS.get(interpolkind)
-    if bpfclass is None:
-        raise ValueError(f"descr {descr} is not valid")
-    return bpfclass(X, Y, **kws)
-    
-
-def multi_parseargs(args) -> tuple[list[float], list[float], list[str]]:
-    """
-    Parse args of a multi bpf
-
-    Given a list of args of the form (x0, y0, interpol) or (x0, y0) (or a flat
-    version thereof), fills the possibly missing interpolation descriptions
-    and returns a tuple `(xs, ys, interpolations)`
-
-    Returns:
-        a tuple (xs, ys, interpolations), where len(interpolations) == len(xs) - 1
-    """
-    xs = []
-    ys = []
-    interpolations = []
-    last_interpolation = 'linear'
-    if all(isinstance(arg, (int, float, str)) for arg in args):
-        # a flat list
-        accum = 0
-        for arg in args:
-            if accum == 0:
-                xs.append(arg)
-                accum += 1
-            elif accum == 1:
-                ys.append(arg)
-                accum += 1
-            else:
-                if isinstance(arg, str):
-                    interpolations.append(arg)
-                    last_interpolation = arg
-                    accum = 0
-                else:
-                    interpolations.append(last_interpolation)
-                    xs.append(arg)
-                    accum = 1
-    else:
-        # it is of the type (x0, y0, interpolation), (x1, y1), ...
-        assert all(isinstance(arg, tuple) and 2 <= len(arg) <= 3 for arg in args)
-        
-        for arg in args[:-1]:
-            if len(arg) == 2:
-                x, y = arg
-                interp = last_interpolation
-            elif len(arg) == 3:
-                x, y, interp = arg
-            xs.append(x)
-            ys.append(y)
-            interpolations.append(interp)
-        x, y = args[-1]
-        xs.append(x)
-        ys.append(y)
-    assert all(isinstance(x, (int, float)) for x in xs)
-    assert all(isinstance(y, (int, float)) for x in ys) 
-    assert all(isinstance(i, str) for i in interpolations)
-    assert len(xs) == len(ys) == len(interpolations)+1
-    return xs, ys, interpolations    
-    
-    
-def max_(*elements) -> core.Max:
-    """
-    Return a bpf representing the max over the given elements
-
-    Args:
-        elements: each element can be a bpf or a scalar
-
-    Returns:
-        a Max bpf
-    """
-    bpfs = list(map(asbpf, elements))
-    return core.Max(*bpfs)
-
-    
-def min_(*elements) -> core.Min:
-    """
-    Return a bpf representing the min over elements
-
-    Args:
-        elements: each can be a bpf or a scalar
-
-    Returns:
-        a Min bpf
-    """
-    bpfs = list(map(asbpf, elements))
-    return core.Min(*bpfs)
-
-    
-def sum_(*elements):
-    """
-    Return a bpf representing the sum of elements
-
-    Args:
-        elements: each can be a bpf or a scalar
-
-    Returns:
-        a bpf representing the sum of all elements
-    
-    """
-    bpfs = list(map(asbpf, elements))
-    return reduce(_operator.add, bpfs)
-
-
-def select(which: core.BpfInterface, bpfs: Sequence[core.BpfInterface], shape='linear') -> core._BpfSelect:
-    """
-    Create a new bpf which interpolates between adjacent bpfs given
-    
-    Args:
-        which: returns at any x, which bpf from bpfs should return the result
-        bpfs: a list of bpfs
-        shape: interpolation shape between consecutive bpfs
-
-    Returns:
-        a BpfSelect
-
-    **Example**
-
-    ```python   
-
-    >>> which = nointerpol(0, 0, 5, 1)
-    >>> bpfs = [linear(0, 0, 10, 10), linear(0, 10, 10, 0)]
-    >>> s = select(which, bpfs)
-    >>> s(1)     # at time=1, the first bpf will be selected
-    0
-    ```
-    """
-    return core._BpfSelect(asbpf(which), list(map(asbpf, bpfs)), shape)
-
-    
-def dumpbpf(bpf: core.BpfInterface, fmt='yaml') -> str:
-    """
-    Dump the data of this bpf as human readable text 
-
-    
-    Args:
-        bpf: the bpf to dump
-        fmt: the format, one of 'csv', 'yaml', 'json'
-        
-    Returns:
-        the text representation according to the format 
-    
-    The bpf can then be reconstructed via `loadbpf`
-
-    """
-    if fmt == 'csv':
-        if outfile is None:
-            raise ValueError("need an outfile to dump to CSV")
-        return bpf_to_csv(bpf, outfile)
-    elif fmt == 'json':
-        return bpf_to_json(bpf, outfile)
-    elif fmt == 'yaml':
-        return bpf_to_yaml(bpf, outfile)
-    else:
-        raise ValueError(f"Format {fmt} not supported")
-        
-            
-def concat_bpfs(bpfs: list[core.BpfInterface]) -> core._BpfConcat:
-    """
-    Concatenate these bpfs together, one after the other
-    """
-    bpfs2 = [bpfs[0]]
-    x0, x1 = bpfs[0].bounds()
-    xs = [x0]
-    for bpf in bpfs[1:]:
-        bpf2 = bpf.fit_between(x1, x1 + (bpf._x1 - bpf._x0))
-        bpfs2.append(bpf2)
-        xs.append(bpf2._x0)
-        x0, x1 = bpf2.bounds()
-    return core._BpfConcat(xs, bpfs2)
-
-
-def warped(bpf: core.BpfInterface, dx:float=None, numpoints=1000) -> core.Sampled:
-    """
-    Represents the curvature of a linear space. 
-
-    The result is a warped bpf so that:
-    
-    ```
-    position_bpf | warped_bpf = corresponding position after warping
-    ```
-
-    Args:
-        dx: the accuracy of the measurement
-        numpoints: if dx is not given, the bpf is sampled `numpoints` times
-            across its bounds
-
-    Returns:
-        (core.Sampled) The warped bpf
-    
-
-    Example
-    -------
-
-    Find the theoretical position of a given point according to a 
-    probability distribution
-    
-    ```python
-    >>> from bpf4 import *
-    >>> import matplotlib.pyplot as plt
-    >>> distribution = halfcos(0,0, 0.5,1, 1, 0)
-    >>> w = util.warped(distribution)
-    >>> distribution.plot()
-    >>> w.plot()
-
-    ```
-    ![](assets/warped.png)
-    
-    Now plot the histrogram of the warped bpf. It should resemble the
-    original distribution
-    ```python
-    plt.hist(w.map(10000), bins=200, density=True)
-    ```
-    ![](assets/warped-hist.png)
-
-    Using another distribution, notice that the histogram follows the
-    distribution again:
-
-    ```python
-    distribution = halfcos(0,0, 0.8,1, 1, 0, exp=3.)
-    w = util.warped(distribution)
-    distribution.plot()
-    w.plot()
-    _ = plt.hist(w.map(10000), bins=200, density=True)[2]
-    ```
-    ![](assets/warped-hist2.png)
-    """
-
-    x0, x1 = bpf.bounds()
-    if dx is None:
-        dx = (x1 - x0) / numpoints
-    integrated = bpf.integrated()[::dx]
-    integrated_at_x1 = integrated(bpf.x1)
-    # N = int((x1 + dx - x0) / dx + 0.5)
-    xs = np.arange(x0, x1+dx, dx)    
-    ys = np.ones_like(xs) * np.nan
-    for i in range(len(xs)):
-        try:
-            ys[i] = _brentq(integrated - xs[i]*integrated_at_x1, x0, x1)
-        except:
-            pass
-    return core.Sampled(ys, dx=dx, x0=x0)
-
-        
-def _minimize(bpf, N: int, func=min, debug=False) -> float | None:
-    x0, x1 = bpf.bounds()
-    xs = np.linspace(x0, x1, N)
-    from scipy.optimize import brent
-    mins = [brent(bpf, brack=(xs[i], xs[-i])) for i in range(int(len(xs) * 0.5 + 0.5))]
-    mins2 = [(bpf(m), m) for m in mins]  # if x0 <= m <= x1]
-    if debug:
-        print(mins2)
-    if mins2:
-        return float(func(mins2)[1])
-    return None
-
-    
-def minimum(bpf: core.BpfInterface, N=10) -> float | None:
-    """
-    Find the x where bpf(x) is minimized
-    
-    Args:
-        bpf: the bpf to analyze
-        N: the number of estimates
-
-    Returns:
-        the *x* value where bpf(x) is minimized. Returns `None` if
-        no minimum found
-
-    """
-    return _minimize(bpf, N, min)
-
-
-def maximum(bpf: core.BpfInterface, N=10) -> float | None:
-    """
-    return the x where bpf(x) is the maximum of bpf
-
-    Args:
-        bpf: the bpf to analyze
-    
-    Returns:
-        the *x* value where bpf(x) is the maximum. Returns `None` if
-        no maximum found
-
-    """
-    return _minimize(-bpf, N, min)
-    
-
-def rms(bpf: core.BpfInterface, rmstime=0.1) -> core.BpfInterface:
-    """
-    The rms of this bpf
-
-    Args:
-        bpf: the bpf 
-        rmstime: the time to calculate the rms over
-
-    Returns:
-        a bpf representing the rms of this bpf at any x coord
-    """
-    bpf2 = bpf**2
-    from math import sqrt
-
-    def func(x):
-        return sqrt(bpf2.integrate_between(x, x+rmstime) / rmstime)
-    return asbpf(func, bounds=(bpf.x0, bpf.x1))
-
-
-def rmsbpf(samples: np.ndarray, sr:int, dt=0.01, overlap=1) -> core.Sampled:
-    """
-    Return a bpf representing the rms of the given samples as a function of time
-
-    Args:
-        samples: the audio samples
-        sr: the sample rate
-        dt: analysis time period
-        overlap: overlap of analysis frames
-
-    Returns:
-        a samples bpf
-    """
-    s = samples
-    period = int(sr * dt + 0.5)
-    hopsamps = period // overlap
-    dt2 = hopsamps / sr
-    numperiods = len(s) // hopsamps
-    data = np.empty((numperiods,), dtype=float)
-    for i in range(numperiods):
-        idx0 = i * hopsamps
-        chunk = s[idx0:idx0+period]
-        data[i] = rms(chunk)
-    return bpf4.core.Sampled(data, x0=0, dx=dt2)
-
-
-def calculate_projection(x0, x1, p0, p1):
-    """
-    Calculate a projection needed to map the interval x0:x1 to p0:p1
-
-    Returns:
-        (tuple[float, float, float]) A tuple (rx, dx, offset)
-    """
-    rx = (x1-x0) / (p1-p0)
-    dx = x0
-    offset = p0
-    return rx, dx, offset
-    
-
-def projection_fixedpoint(rx, dx, offset):
-    """
-    Returns the fixed point given the projection parameters
-
-    x2 = (x-offset)*rx + dx
-
-    For a fixed point, x2 == x
-    """
-    return (-offset*rx + dx)/(1-rx)
-    
-    
-
-def binarymask(mask: str | list[int],
-               durs: Sequence[float]=None,
-               offset=0.,
-               cycledurs=True
-               ) -> core.NoInterpol:
-    """
-    Creates a binary mask
-
-    Args:
-        mask: a mask string ('x'=1, '-'=0) or a sequence of states (a state is either 0 or 1)
-        durs: a sequence of durations (default=[1])
-
-    Returns:
-        (core.NoInterpol) A NoInterpol bpf representing the binary mask
-
-    **Example**
-
-    ```python
-        
-    >>> mask = binarymask("x--x-x---")
-    ```
-
-    """
-    if durs is None:
-        durs = [1]
-    if cycledurs:
-        durs = _itertools.cycle(durs)
-    else:
-        assert len(durs) == len(mask)
-
-    def binvalue(x):
-        d = {'x':1, 'o':0, '-':0, 1:1, 0:0, '1':1, '0':0}
-        return d.get(x)
-
-    mask = [binvalue(x) for x in mask]
-    mask.append(mask[-1])
-    assert all(x is not None for x in mask)
-    t = offset
-    times = []
-    for i, dur in zip(range(len(mask)), durs):
-        times.append(t)
-        t += dur
-    return core.NoInterpol(times, mask)
-
-
-def _pairwise(iterable):
-    "s -> (s0,s1), (s1,s2), (s2, s3), ..."
-    a, b = _itertools.tee(iterable)
-    try:
-        next(b)
-    except StopIteration:
-        pass
-    return zip(a, b)
-
-    
-def jagged_band(xs: list[float], upperbpf: core.BpfInterface, lowerbpf=0, curve='linear'
-                ) -> core.BpfInterface:
-    """
-    Create a jagged bpf between lowerbpf and upperbpf at the x values given
-    
-    At each x in xs the, the value is equal to lowerbpf, sweeping
-    with curvature 'curve' to upperbpf just before the next x
-
-    Example
-    -------
-
-    ```python
-    
-    from bpf4 import *
-    import numpy as np
-    a = expon(0, 0, 1, 10, exp=2)
-    b = expon(0, 0, 1, 5, exp=4)
-    j = util.jagged_band(list(np.arange(0, 1, 0.1)), a, b, curve='expon(1.5)')
-    j.plot()
-    ```
-    ![](assets/jagged.png)
-    """
-    upperbpf = asbpf(upperbpf)
-    lowerbpf = asbpf(lowerbpf)
-    if not isinstance(xs, list): 
-        xs = list(xs)
-    EPSILON = 1e-12
-    fragments = []
-    if xs[0] > upperbpf.x0 > float('-inf'):
-        xs = [upperbpf.x0] + xs
-    if xs[-1] < upperbpf.x1 < float('inf'):
-        xs.append(upperbpf.x1)
-    for x0, x1 in _pairwise(xs[:-1]):
-        x1 = x1 - EPSILON
-        fragment = makebpf(curve, [x0, x1], [lowerbpf(x0), upperbpf(x1)])[x0:x1].outbound(0, 0)
-        fragments.append(fragment)
-    x0 = xs[-2]
-    x1 = xs[-1]
-    fragments.append(makebpf(curve, [x0, x1], [lowerbpf(x0), upperbpf(x1)])[x0:x1].outbound(0, 0))
-    return max_(*fragments)
-    
-
-def randombw(bw: float | core.BpfInterface,
-             center: float | core.BpfInterface
-             ) -> core.BpfInterface:
-    """
-    Create a random bpf
-    
-    Args:
-        bw: a (time-varying) bandwidth
-        center: the center of the random distribution
-
-    Returns:
-        a bpf
-        
-    if randombw is 0.1 and center is 1, the bpf will render values 
-    between 0.95 and 1.05
-
-    **NB**: this bpf will always be different, since the random numbers
-    are calculated as needed. Sample it to freeze it to a known state.
-
-    **Example**
-    
-    ```python
-
-    >>> l = bpf.linear(0, 0, 1, 1)
-    >>> r = bpf.util.randombw(0.1)
-    >>> l2 = (l*r)[::0.01]
-    ```
-    """
-    bw = asbpf(bw)
-    return (bw.rand() + (center - bw*0.5))[bw.x0:bw.x1]
-    
-
-def blendwithfloor(b: core.BpfInterface, mix=0.5) -> core._BpfBlend:
-    return core.blend(b, asbpf(b(maximum(b))), mix)[b.x0:b.x1]
-    
-    
-def blendwithceil(b, mix=0.5) -> core._BpfBlend:
-    return core.blend(b, asbpf(b(maximum(b))), mix)[b.x0:b.x1]
-    
-
-def smoothen(b: core.BpfInterface, window:int, N=1000, interpol='linear') -> core.BpfInterface:
-    """
-    Return a linear bpf representing a smooth version of b
-
-    Args:
-        b: a bpf
-        window: the width (in x coords) of the smoothing window
-        N: number of points to resample the bpf
-        interpol: the interpolation to use. One of 'linear', 'smooth', 'halfcos'
-
-    Returns:
-        a bpf representing a smoother version of b
-    """
-    dx = min((b.x1 - b.x0) / N, window/7)
-    nwin = int(window / dx)
-    box = np.ones(nwin)/nwin
-    Y = b[::dx].ys
-    Y2 = np.convolve(Y, box, mode="same")
-    X = np.linspace(b.x0, b.x1, len(Y2))
-    if interpol == 'linear':
-        return core.Linear(X, Y2)
-    elif interpol == 'smooth':
-        return core.Smooth(X, Y2)
-    elif interpol == 'halfcos':
-        return core.Halfcos(X, Y2)
-    else:
-        raise ValueError(f"Interpolation {interpol} not supported here. "
-                          "Possible values: linear, smooth, halfcos")
-
-
-def zigzag(b0: core.BpfInterface,
-           b1: core.BpfInterface,
-           xs: Sequence[float],
-           shape='linear'
-           ) -> core.BpfInterface:
-    """
-    Creates a curve formed of lines from b0(x) to b1(x) for each x in xs
-
-    Args:
-        b0: a bpf
-        b1: a bpf
-        xs: a seq. of x values to evaluate b0 and b1
-        shape: the shape of each segment
-
-    Returns:
-        The resulting bpf
-
-    ::
-
-       *.
-        *...  b0
-         *  ...
-         *     ...
-          *       ....
-           *          ...
-            *         :  ...
-             *        :*    ...
-             *        : *      ...
-              *       :  **       ...
-               *      :    *         :*.
-                *     :     *        : **...
-                 *    :      *       :   *  ...
-                 *    :       *      :    *    ...
-                  *   :        *     :     **     .:.
-                   *  :         *    :       *     :**..
-                    * :          **  :        **   :  ****.
-                     *:            * :          *  :      ****
-        -----------  *:             *:           * :          ****
-          b1       ---*--------------*---         **:             ****
-                                         -----------*----------      .**
-                                                               -----------
-        x0            x1              x2                       x3
-
-    """
-    curves = []
-    for x0, x1 in pairwise(xs):
-        X = [x0, x1]
-        Y = [b0(x0), b1(x1)]
-        curve = bpf.util.makebpf(shape, X, Y)
-        curves.append(curve)
-    jointcurve = bpf.max_(*[c.outbound(0, 0) for c in curves])
-    return jointcurve
-
-
-def bpfavg(b: core.BpfInterface,
-           dx: float
-           ) -> core.BpfInterface:
-    """
-    Return a Bpf which is the average of b over the range `dx`
-
-    Args:
-        b: the bpf
-        dx: the period to average *b* over
-
-    Returns:
-        a bpf representing the average of *b* along the bounds of
-        *b* over a sliding period of *dx*
-    """
-    dx2 = dx/2
-    avg = ((b<<dx2)+b+(b>>dx2))/3.0
-    return avg[b.x0:b.x1]
-
-
-def histbpf(b: core.BpfInterface, numbins=10, numsamples=200, interpolation='linear'
-            ) -> core.BpfInterface:
-    """
-    Create a historgram of *b*
-
-    Args:
-        b: the bpf
-        numbins: the number of bins
-        numsamples: how many samples to take to determine the histogram
-        interpolation: the kind of interpolation of the returned bpf
-
-    Returns:
-        a bpf representing the percentile associated with a given value of *b*
-        Percentiles are given between 0 and 1
-
-    Example
-    ~~~~~~~
-
-    >>> from sndfileio import *
-    >>> samples, sr = sndread("path/to/soundfile.wav")
-    >>> dbcurve = rmsbpf(samples, sr=sr).amp2db()
-    >>> dbhist = histbpf(dbcurve)
-    # Find the db percentile at a given time, this gives a measurement of the
-    # relative strength of the sound at a given moment
-    >>> dur = len(samples)/sr
-    >>> percentile = dbhist(dur*0.5)
-    0.312
-
-    This indicates that at the middle of the sound the amplitude is at percentile ~30
-
-    """
-    samples = b.map(numsamples)
-    edges, hist = np.histogram(b, bins=numbins)
-    percentile = np.linspace(0, 1, len(hist))
-    if interpolation == 'linear':
-        return core.Linear(hist, percentile)
-    elif interpolation == 'nointerpol':
-        return core.NoInterpol(hist, percentile)
-    else:
-        raise ValueError("Only 'linear' or 'nointerpol' are supported")
+"""
+Utilities for bpf4
+"""
+from __future__ import annotations
+import operator as _operator
+import os as _os
+import itertools as _itertools
+from functools import reduce
+from typing import Sequence
+
+import numpy as np
+from scipy.integrate import quad as _quad
+from scipy.optimize import brentq as _brentq
+from . import core
+
+
+_CSV_COLUMN_NAMES = ('x', 'y', 'interpolation', 'exponent')
+
+
+_CONSTRUCTORS = {
+    'linear': core.Linear,
+    'expon': core.Expon,
+    'halfcos': core.Halfcos,
+    'nointerpol': core.NoInterpol,
+    'spline': core.Spline,
+    'uspline': core.USpline,
+    'slope': core.Slope,
+    'nearest': core.Nearest,
+    'halfcosm': core.Halfcosm,
+    'smooth': core.Smooth,
+    'smoother': core.Smoother
+}
+
+
+def _isiterable(obj) -> bool:
+    try:
+        iter(obj)
+        return not isinstance(obj, str)
+    except TypeError:
+        return False
+
+
+def _iflatten(seq):
+    """
+    Return an iterator to the flattened items of sequence s
+    
+    Strings are not flattened
+    """
+    try:
+        iter(seq)
+    except TypeError:
+        yield seq
+    else:
+        for elem in seq:
+            if isinstance(elem, str):
+                yield elem
+            else:
+                for subelem in _iflatten(elem):
+                    yield subelem
+
+def csv_to_bpf(csvfile: str) -> core.BpfInterface:
+    """
+    Read a bpf from a csv file
+    """
+    from emlib import csvtools
+    rows = csvtools.readcsv(csvfile)
+    interpolation = rows[0].interpolation
+    if all(row.interpolation == interpolation for row in rows[:-1]):
+        # all of the same type
+        if interpolation in ('expon', 'halfcosexp', 'halfcos2'):
+            exp = rows[0].exponent
+            constructor = get_bpf_constructor("%s(%.3f)" % (interpolation, exp))
+        else:
+            constructor = get_bpf_constructor(interpolation)
+        numrows = len(rows)
+        xs = np.empty((numrows,), dtype=float)
+        ys = np.empty((numrows,), dtype=float)
+        for i in range(numrows):
+            r = rows[i]
+            xs[i] = r.x
+            ys[i] = r.y
+        return constructor(xs, ys)
+    else:
+        # multitype
+        raise NotImplementedError("BPFs with multiple types not implemented YET")
+
+
+def bpf_to_csv(bpf: core.BpfInterface, csvfile: str) -> None:
+    """
+    Write this bpf as a csv representation
+
+    Args:
+        bpf: the bpf to write as csv
+        csvfile: the output filename
+    """
+    import csv
+    csvfile = _os.path.splitext(csvfile)[0] + '.csv'
+    try:
+        # it follows the 'segments' protocol, returning a seq of (x, y, interpoltype, exp)
+        segments = bpf.segments()
+        with open(csvfile, 'w') as f:
+            writer = csv.writer(f)
+            writer.writerow(_CSV_COLUMN_NAMES)
+            writer.writerows(segments)
+    except AttributeError:
+        raise TypeError("BPF must be rendered in order to be written as CSV")
+
+
+def bpf_to_dict(bpf: core.BpfInterface) -> dict:
+    """
+    convert a bpf to a dict with the following format
+
+    Args:
+        bpf: the bpf to convert to a dict
+
+    Returns:
+        (dict) The bpf as a dictionary
+
+    ```python
+
+    >>> b = bpf.expon(3.0, 0, 0, 1, 10, 2, 20)
+    >>> bpf_to_dict(b)
+    {
+        'interpolation': 'expon(3.0)',
+        'points': [0, 0, 1, 10, 20, 20]  # [x0, y0, x1, y1, ...]
+    }
+
+    >>> b = bpf.multi(0, 0, 'linear',
+                      1, 10, 'expon(2)',
+                      3, 25)
+    >>> bpf_to_dict(b)
+    {
+        'interpolation': 'multi',
+        'segments': [
+            [0, 0, 'linear'],
+            [1, 10, 'expon(2)',
+            [3, 25, '']]
+    }
+    ```
+    """
+    try:
+        segments = list(bpf.segments())
+    except:
+        raise TypeError("this kind of BPF cannot be translated. It must be rendered first.")
+    d = {}
+    interpolation = segments[0][2]
+    # x y interpolation exp
+
+    def normalize_segment(segment):
+        """
+        a segment as returned by .segments() is [x, y, interpl, exp]
+        we want [x, y, interpol(exp)]
+        """
+        if len(segment) == 4:
+            x, y, interpol, exp = segment
+            if not interpol and exp == 0:
+                # the last segment of a multi bpf
+                segment = [x, y]
+            else:
+                interpol = "{interpol}({exp})".format(interpol=interpol, exp=exp)
+                segment = [x, y, interpol]
+        return segment
+
+    if not all(segment[2] == interpolation for segment in segments[:-1]):
+        # multi
+        d['interpolation'] = 'multi'
+        segments = [normalize_segment(seg) for seg in segments]
+        d['segments'] = segments
+    else:
+        try:
+            exp = bpf.exp
+            if exp != 1:
+                assert "(" not in interpolation
+                interpolation = "{interp}({exp})".format(interp=interpolation, exp=exp)
+        except AttributeError:
+            pass
+        d['interpolation'] = interpolation
+        points = []
+        for segment in segments:
+            points.append(segment[0])
+            points.append(segment[1])
+        d['points'] = points
+    return d
+
+
+def bpf_to_json(bpf: core.BpfInterface, outfile: str = None) -> str:
+    """
+    convert this bpf to json format.
+
+    If outfile is not given, it returns a string, as in dumps
+
+    Args:
+        bpf: the bpf to dump as json
+        outfile: the output filename. If given, output is saved here
+
+    Returns:
+        (str) The json text
+    """
+    import json
+    asdict = bpf_to_dict(bpf)
+    jsontxt = json.dumps(asdict)
+    if outfile:
+        open(outfile, 'w').write(jsontxt)
+    return jsontxt
+        
+
+def bpf_to_yaml(bpf: core.BpfInterface, outfile: str = None) -> str:
+    """
+    Convert this bpf to json format. 
+
+    Args:
+        bpf: the bpf to convert
+        outfile: if given, the yaml text is saved to this file
+
+    Returns:
+        (str) The yaml text
+    """
+    from io import StringIO
+    import yaml
+    d = bpf_to_dict(bpf)
+    if outfile is None:
+        stream = StringIO()
+    else:
+        outfile = _os.path.splitext(outfile)[0] + '.yaml'
+        stream = open(outfile, 'w')
+    dumper = yaml.Dumper(stream)
+    dumper.add_representer(tuple, lambda du, instance: du.represent_list(instance))
+    dumper.add_representer(np.float64, lambda du, instance: du.represent_float(instance))
+    dumper.open()
+    dumper.represent(d)
+    dumper.close()
+    return stream.getvalue()
+
+
+def dict_to_bpf(d: dict) -> bpf.BpfInterface:
+    """
+    Convert a dict to a bpf
+
+    Args:
+        d: the dictionary to convert to a bpf
+
+    Returns:
+        the converted bpf
+
+
+    **Format 1** 
+
+    ```python
+
+    bpf = {
+        'interpolation': 'expon(2)',
+        10: 0.1,
+        15: 1,
+        25: -1
+    }
+    ```
+
+    **Format 2**
+
+    ```python
+    bpf = {
+        'interpolation': 'linear',
+        'points': [x0, y0, x1, y1, ...]
+    }
+    ```
+
+    **Format 2b**
+
+    ```python
+    bpf = {
+        'interpolation': 'linear',
+        'points': [(x0, y0), (x1, y1), ...]
+    }
+    ```
+
+    **Format 3 (multi)**
+
+    ```python
+
+    bpf = {
+        'interpolation': 'multi',
+        'segments': [
+            [x0, y0, 'descr0'],
+            [x1, y1, 'descr1'],
+            ...
+            [xn, yn, '']
+        ]
+    }
+    ```
+    """
+
+    # check format
+    if 'points' in d:
+        # format 2
+        interpolation = d.get('interpolation', 'linear')
+        constructor = get_bpf_constructor(interpolation)
+        points = d['points']
+        if isinstance(points[0], (int, float)):
+            # format 2a
+            X = points[::2]
+            Y = points[1::2]
+        elif isinstance(points[0], (list, tuple)):
+            X = [point[0] for point in points]
+            Y = [point[1] for point in points]
+        return constructor.fromxy(X, Y)
+    elif 'segments' in d and d['interpolation'] == 'multi':
+        segments = d['segments']
+        X = [s[0] for s in segments]
+        Y = [s[1] for s in segments]
+        interpolations = [s[2] for s in segments[:-1]]
+        return core.Multi(X, Y, interpolations)
+    else:
+        # format 1
+        interpolation = d.get('interpolation', 'linear')
+        constructor = get_bpf_constructor(interpolation)
+        points = [(k, v) for k, v in d.items() if isinstance(k, (int, float))]
+        points.sort()
+        X, Y = list(zip(*points))
+        return constructor.fromxy(X, Y)
+
+
+def loadbpf(path: str, fmt='auto') -> core.BpfInterface:
+    """
+    Load a bpf saved with dumpbpf
+
+    Possible formats: auto, csv, yaml, json
+
+    Args:
+        path: the path of the saved bpf
+        fmt: the format used to save the bpf ('auto' to detect the format)
+
+    Returns:
+        a bpf
+    """
+    if fmt == 'auto':
+        fmt = _os.path.splitext(path)[-1].lower()[1:]
+    assert fmt in ('csv', 'yaml', 'json')
+    if fmt == 'yaml':
+        import yaml
+        d = yaml.load(open(path))
+    elif fmt == 'json':
+        import json
+        d = json.load(path)
+    elif fmt == 'csv':
+        return csv_to_bpf(path)
+    return dict_to_bpf(d)  
+
+
+def asbpf(obj, bounds=(-np.inf, np.inf)) -> core.BpfInterface:
+    """
+    Convert obj to a bpf
+
+    obj can be a function, a dict, a constant, or a bpf (in which case it
+    is returned as is)
+    """
+    if isinstance(obj, core.BpfInterface):
+        return obj
+    elif callable(obj):
+        return core._FunctionWrap(obj, bounds)
+    elif hasattr(obj, '__float__'):
+        return core.Const(float(obj))
+    else:
+        raise TypeError("can't wrap %s" % str(obj))
+ 
+
+def parseargs(*args, **kws) -> tuple[list[float], list[float], dict]:
+    """
+    Convert the args and kws to the canonical form (xs, ys, kws)
+    
+    Returns:
+        (tuple[list[float], list[float], dict]) A tuple `(xs, ys, kws)`
+    
+    Raises ValueError if failed
+
+    All the following variants result in the same result:
+
+    ```python
+
+    x0, y0, x1, y1, …, exp=0.5
+    (x0, y0), (x1, y1), …, exp=0.5           
+    {x0:y0, x1:y1, …}, exp=0.5               
+    [x0, x1, …], [y0, y1, …], exp=0.5        
+    
+    Result: [x0, x1, …], [y0, y1, …], {exp:0.5}
+    ```
+    """
+    L = len(args)
+    if L == 0:
+        raise ValueError("no arguments given")
+    elif L == 1:
+        d = args[0]
+        assert isinstance(d, dict)
+        items = list(d.items())
+        items.sort()
+        xs, ys = list(zip(*items))
+    elif L == 2:
+        if not all(map(_isiterable, args)):
+            raise ValueError(f"parsing error: 2 args, expected a seq. "
+                             f"[(x0, y1), (x1, y1)] or (xs, ys) but got {args}")
+        if len(args[0]) > 2:   # <--  (xs, ys)
+            xs, ys = args
+        else:                  # <--  ((x0, y0), (x1, y1), ...)
+            xs, ys = list(zip(*args))    
+    elif not any(map(_isiterable, args)):
+        # (x0, y0, x1, y1, ...)
+        if L % 2 == 0:  # even
+            xs = args[::2]
+            ys = args[1::2]
+        else:
+            if kws:
+                raise ValueError(f"Uneven number of args. No keywords allowed in "
+                                 f"this case, but got {kws}")
+            kws = {'exp': args[0]}
+            xs = args[1::2]
+            ys = args[2::2]
+    elif all(map(_isiterable, args)):   # <-- ((x0, y0), (x1, y1), ...)
+        xs, ys = list(zip(*args))
+    else:
+        raise ValueError("could not parse arguments")
+    return xs, ys, kws
+        
+
+
+def parsedescr(descr: str, validate=True) -> tuple[str, dict]:
+    """
+    Parse interpolation description
+
+
+    | descr                   | output                             |
+    |-------------------------|------------------------------------|
+    | linear                  | linear, {}                         |
+    | expon(0.4)              | expon, {'exp': 0.4}                |
+    | halfcos(2.5, numiter=1) | halfcos, {'exp':2.5, 'numiter': 1} |
+
+    """
+    if "(" not in descr:
+        classname = descr
+        kws = {}
+    else:
+        classname, rest = descr.split("(")
+        assert rest[-1] == ")"
+        rest = rest[:-1]
+        parts = rest.split(",")
+        kws = {}
+        for part in parts:
+            if "=" in part:
+                key, value = part.split("=")
+                kws[key] = float(value)
+            else:
+                assert 'exp' not in kws
+                kws['exp'] = float(part)
+    if validate:
+        assert classname in _CONSTRUCTORS
+    return classname, kws
+
+
+def makebpf(descr: str, X: Sequence[float], Y: Sequence[float]) -> core.BpfInterface:
+    """
+    Create a bpf from the given descriptor and points
+
+    Args:
+        descr: a string descriptor of the interpolation ("linear", "expon(xx)", ...)
+        X: the array of xs
+        Y: the array of ys
+
+    Returns:
+        the created bpf
+    """
+    interpolkind, kws = parsedescr(descr)
+    bpfclass = _CONSTRUCTORS.get(interpolkind)
+    if bpfclass is None:
+        raise ValueError(f"descr {descr} is not valid")
+    return bpfclass(X, Y, **kws)
+    
+
+def multi_parseargs(args) -> tuple[list[float], list[float], list[str]]:
+    """
+    Parse args of a multi bpf
+
+    Given a list of args of the form (x0, y0, interpol) or (x0, y0) (or a flat
+    version thereof), fills the possibly missing interpolation descriptions
+    and returns a tuple `(xs, ys, interpolations)`
+
+    Returns:
+        a tuple (xs, ys, interpolations), where len(interpolations) == len(xs) - 1
+    """
+    xs = []
+    ys = []
+    interpolations = []
+    last_interpolation = 'linear'
+    if all(isinstance(arg, (int, float, str)) for arg in args):
+        # a flat list
+        accum = 0
+        for arg in args:
+            if accum == 0:
+                xs.append(arg)
+                accum += 1
+            elif accum == 1:
+                ys.append(arg)
+                accum += 1
+            else:
+                if isinstance(arg, str):
+                    interpolations.append(arg)
+                    last_interpolation = arg
+                    accum = 0
+                else:
+                    interpolations.append(last_interpolation)
+                    xs.append(arg)
+                    accum = 1
+    else:
+        # it is of the type (x0, y0, interpolation), (x1, y1), ...
+        assert all(isinstance(arg, tuple) and 2 <= len(arg) <= 3 for arg in args)
+        
+        for arg in args[:-1]:
+            if len(arg) == 2:
+                x, y = arg
+                interp = last_interpolation
+            elif len(arg) == 3:
+                x, y, interp = arg
+            xs.append(x)
+            ys.append(y)
+            interpolations.append(interp)
+        x, y = args[-1]
+        xs.append(x)
+        ys.append(y)
+    assert all(isinstance(x, (int, float)) for x in xs)
+    assert all(isinstance(y, (int, float)) for x in ys) 
+    assert all(isinstance(i, str) for i in interpolations)
+    assert len(xs) == len(ys) == len(interpolations)+1
+    return xs, ys, interpolations    
+    
+    
+def max_(*elements) -> core.Max:
+    """
+    Return a bpf representing the max over the given elements
+
+    Args:
+        elements: each element can be a bpf or a scalar
+
+    Returns:
+        a Max bpf
+    """
+    bpfs = list(map(asbpf, elements))
+    return core.Max(*bpfs)
+
+    
+def min_(*elements) -> core.Min:
+    """
+    Return a bpf representing the min over elements
+
+    Args:
+        elements: each can be a bpf or a scalar
+
+    Returns:
+        a Min bpf
+    """
+    bpfs = list(map(asbpf, elements))
+    return core.Min(*bpfs)
+
+    
+def sum_(*elements):
+    """
+    Return a bpf representing the sum of elements
+
+    Args:
+        elements: each can be a bpf or a scalar
+
+    Returns:
+        a bpf representing the sum of all elements
+    
+    """
+    bpfs = list(map(asbpf, elements))
+    return reduce(_operator.add, bpfs)
+
+
+def select(which: core.BpfInterface, bpfs: Sequence[core.BpfInterface], shape='linear') -> core._BpfSelect:
+    """
+    Create a new bpf which interpolates between adjacent bpfs given
+    
+    Args:
+        which: returns at any x, which bpf from bpfs should return the result
+        bpfs: a list of bpfs
+        shape: interpolation shape between consecutive bpfs
+
+    Returns:
+        a BpfSelect
+
+    **Example**
+
+    ```python   
+
+    >>> which = nointerpol(0, 0, 5, 1)
+    >>> bpfs = [linear(0, 0, 10, 10), linear(0, 10, 10, 0)]
+    >>> s = select(which, bpfs)
+    >>> s(1)     # at time=1, the first bpf will be selected
+    0
+    ```
+    """
+    return core._BpfSelect(asbpf(which), list(map(asbpf, bpfs)), shape)
+
+    
+def dumpbpf(bpf: core.BpfInterface, fmt='yaml') -> str:
+    """
+    Dump the data of this bpf as human readable text 
+
+    
+    Args:
+        bpf: the bpf to dump
+        fmt: the format, one of 'csv', 'yaml', 'json'
+        
+    Returns:
+        the text representation according to the format 
+    
+    The bpf can then be reconstructed via `loadbpf`
+
+    """
+    if fmt == 'csv':
+        if outfile is None:
+            raise ValueError("need an outfile to dump to CSV")
+        return bpf_to_csv(bpf, outfile)
+    elif fmt == 'json':
+        return bpf_to_json(bpf, outfile)
+    elif fmt == 'yaml':
+        return bpf_to_yaml(bpf, outfile)
+    else:
+        raise ValueError(f"Format {fmt} not supported")
+        
+            
+def concat_bpfs(bpfs: list[core.BpfInterface]) -> core._BpfConcat:
+    """
+    Concatenate these bpfs together, one after the other
+    """
+    bpfs2 = [bpfs[0]]
+    x0, x1 = bpfs[0].bounds()
+    xs = [x0]
+    for bpf in bpfs[1:]:
+        bpf2 = bpf.fit_between(x1, x1 + (bpf._x1 - bpf._x0))
+        bpfs2.append(bpf2)
+        xs.append(bpf2._x0)
+        x0, x1 = bpf2.bounds()
+    return core._BpfConcat(xs, bpfs2)
+
+
+def warped(bpf: core.BpfInterface, dx:float=None, numpoints=1000) -> core.Sampled:
+    """
+    Represents the curvature of a linear space. 
+
+    The result is a warped bpf so that:
+    
+    ```
+    position_bpf | warped_bpf = corresponding position after warping
+    ```
+
+    Args:
+        dx: the accuracy of the measurement
+        numpoints: if dx is not given, the bpf is sampled `numpoints` times
+            across its bounds
+
+    Returns:
+        (core.Sampled) The warped bpf
+    
+
+    Example
+    -------
+
+    Find the theoretical position of a given point according to a 
+    probability distribution
+    
+    ```python
+    >>> from bpf4 import *
+    >>> import matplotlib.pyplot as plt
+    >>> distribution = halfcos(0,0, 0.5,1, 1, 0)
+    >>> w = util.warped(distribution)
+    >>> distribution.plot()
+    >>> w.plot()
+
+    ```
+    ![](assets/warped.png)
+    
+    Now plot the histrogram of the warped bpf. It should resemble the
+    original distribution
+    ```python
+    plt.hist(w.map(10000), bins=200, density=True)
+    ```
+    ![](assets/warped-hist.png)
+
+    Using another distribution, notice that the histogram follows the
+    distribution again:
+
+    ```python
+    distribution = halfcos(0,0, 0.8,1, 1, 0, exp=3.)
+    w = util.warped(distribution)
+    distribution.plot()
+    w.plot()
+    _ = plt.hist(w.map(10000), bins=200, density=True)[2]
+    ```
+    ![](assets/warped-hist2.png)
+    """
+
+    x0, x1 = bpf.bounds()
+    if dx is None:
+        dx = (x1 - x0) / numpoints
+    integrated = bpf.integrated()[::dx]
+    integrated_at_x1 = integrated(bpf.x1)
+    # N = int((x1 + dx - x0) / dx + 0.5)
+    xs = np.arange(x0, x1+dx, dx)    
+    ys = np.ones_like(xs) * np.nan
+    for i in range(len(xs)):
+        try:
+            ys[i] = _brentq(integrated - xs[i]*integrated_at_x1, x0, x1)
+        except:
+            pass
+    return core.Sampled(ys, dx=dx, x0=x0)
+
+        
+def _minimize(bpf, N: int, func=min, debug=False) -> float | None:
+    x0, x1 = bpf.bounds()
+    xs = np.linspace(x0, x1, N)
+    from scipy.optimize import brent
+    mins = [brent(bpf, brack=(xs[i], xs[-i])) for i in range(int(len(xs) * 0.5 + 0.5))]
+    mins2 = [(bpf(m), m) for m in mins]  # if x0 <= m <= x1]
+    if debug:
+        print(mins2)
+    if mins2:
+        return float(func(mins2)[1])
+    return None
+
+    
+def minimum(bpf: core.BpfInterface, N=10) -> float | None:
+    """
+    Find the x where bpf(x) is minimized
+    
+    Args:
+        bpf: the bpf to analyze
+        N: the number of estimates
+
+    Returns:
+        the *x* value where bpf(x) is minimized. Returns `None` if
+        no minimum found
+
+    """
+    return _minimize(bpf, N, min)
+
+
+def maximum(bpf: core.BpfInterface, N=10) -> float | None:
+    """
+    return the x where bpf(x) is the maximum of bpf
+
+    Args:
+        bpf: the bpf to analyze
+    
+    Returns:
+        the *x* value where bpf(x) is the maximum. Returns `None` if
+        no maximum found
+
+    """
+    return _minimize(-bpf, N, min)
+    
+
+def rms(bpf: core.BpfInterface, rmstime=0.1) -> core.BpfInterface:
+    """
+    The rms of this bpf
+
+    Args:
+        bpf: the bpf 
+        rmstime: the time to calculate the rms over
+
+    Returns:
+        a bpf representing the rms of this bpf at any x coord
+    """
+    bpf2 = bpf**2
+    from math import sqrt
+
+    def func(x):
+        return sqrt(bpf2.integrate_between(x, x+rmstime) / rmstime)
+    return asbpf(func, bounds=(bpf.x0, bpf.x1))
+
+
+def rmsbpf(samples: np.ndarray, sr:int, dt=0.01, overlap=1) -> core.Sampled:
+    """
+    Return a bpf representing the rms of the given samples as a function of time
+
+    Args:
+        samples: the audio samples
+        sr: the sample rate
+        dt: analysis time period
+        overlap: overlap of analysis frames
+
+    Returns:
+        a samples bpf
+    """
+    s = samples
+    period = int(sr * dt + 0.5)
+    hopsamps = period // overlap
+    dt2 = hopsamps / sr
+    numperiods = len(s) // hopsamps
+    data = np.empty((numperiods,), dtype=float)
+    for i in range(numperiods):
+        idx0 = i * hopsamps
+        chunk = s[idx0:idx0+period]
+        data[i] = rms(chunk)
+    return bpf4.core.Sampled(data, x0=0, dx=dt2)
+
+
+def calculate_projection(x0, x1, p0, p1):
+    """
+    Calculate a projection needed to map the interval x0:x1 to p0:p1
+
+    Returns:
+        (tuple[float, float, float]) A tuple (rx, dx, offset)
+    """
+    rx = (x1-x0) / (p1-p0)
+    dx = x0
+    offset = p0
+    return rx, dx, offset
+    
+
+def projection_fixedpoint(rx, dx, offset):
+    """
+    Returns the fixed point given the projection parameters
+
+    x2 = (x-offset)*rx + dx
+
+    For a fixed point, x2 == x
+    """
+    return (-offset*rx + dx)/(1-rx)
+    
+    
+
+def binarymask(mask: str | list[int],
+               durs: Sequence[float]=None,
+               offset=0.,
+               cycledurs=True
+               ) -> core.NoInterpol:
+    """
+    Creates a binary mask
+
+    Args:
+        mask: a mask string ('x'=1, '-'=0) or a sequence of states (a state is either 0 or 1)
+        durs: a sequence of durations (default=[1])
+
+    Returns:
+        (core.NoInterpol) A NoInterpol bpf representing the binary mask
+
+    **Example**
+
+    ```python
+        
+    >>> mask = binarymask("x--x-x---")
+    ```
+
+    """
+    if durs is None:
+        durs = [1]
+    if cycledurs:
+        durs = _itertools.cycle(durs)
+    else:
+        assert len(durs) == len(mask)
+
+    def binvalue(x):
+        d = {'x':1, 'o':0, '-':0, 1:1, 0:0, '1':1, '0':0}
+        return d.get(x)
+
+    mask = [binvalue(x) for x in mask]
+    mask.append(mask[-1])
+    assert all(x is not None for x in mask)
+    t = offset
+    times = []
+    for i, dur in zip(range(len(mask)), durs):
+        times.append(t)
+        t += dur
+    return core.NoInterpol(times, mask)
+
+
+def _pairwise(iterable):
+    "s -> (s0,s1), (s1,s2), (s2, s3), ..."
+    a, b = _itertools.tee(iterable)
+    try:
+        next(b)
+    except StopIteration:
+        pass
+    return zip(a, b)
+
+    
+def jagged_band(xs: list[float], upperbpf: core.BpfInterface, lowerbpf=0, curve='linear'
+                ) -> core.BpfInterface:
+    """
+    Create a jagged bpf between lowerbpf and upperbpf at the x values given
+    
+    At each x in xs the, the value is equal to lowerbpf, sweeping
+    with curvature 'curve' to upperbpf just before the next x
+
+    Example
+    -------
+
+    ```python
+    
+    from bpf4 import *
+    import numpy as np
+    a = expon(0, 0, 1, 10, exp=2)
+    b = expon(0, 0, 1, 5, exp=4)
+    j = util.jagged_band(list(np.arange(0, 1, 0.1)), a, b, curve='expon(1.5)')
+    j.plot()
+    ```
+    ![](assets/jagged.png)
+    """
+    upperbpf = asbpf(upperbpf)
+    lowerbpf = asbpf(lowerbpf)
+    if not isinstance(xs, list): 
+        xs = list(xs)
+    EPSILON = 1e-12
+    fragments = []
+    if xs[0] > upperbpf.x0 > float('-inf'):
+        xs = [upperbpf.x0] + xs
+    if xs[-1] < upperbpf.x1 < float('inf'):
+        xs.append(upperbpf.x1)
+    for x0, x1 in _pairwise(xs[:-1]):
+        x1 = x1 - EPSILON
+        fragment = makebpf(curve, [x0, x1], [lowerbpf(x0), upperbpf(x1)])[x0:x1].outbound(0, 0)
+        fragments.append(fragment)
+    x0 = xs[-2]
+    x1 = xs[-1]
+    fragments.append(makebpf(curve, [x0, x1], [lowerbpf(x0), upperbpf(x1)])[x0:x1].outbound(0, 0))
+    return max_(*fragments)
+    
+
+def randombw(bw: float | core.BpfInterface,
+             center: float | core.BpfInterface
+             ) -> core.BpfInterface:
+    """
+    Create a random bpf
+    
+    Args:
+        bw: a (time-varying) bandwidth
+        center: the center of the random distribution
+
+    Returns:
+        a bpf
+        
+    if randombw is 0.1 and center is 1, the bpf will render values 
+    between 0.95 and 1.05
+
+    **NB**: this bpf will always be different, since the random numbers
+    are calculated as needed. Sample it to freeze it to a known state.
+
+    **Example**
+    
+    ```python
+
+    >>> l = bpf.linear(0, 0, 1, 1)
+    >>> r = bpf.util.randombw(0.1)
+    >>> l2 = (l*r)[::0.01]
+    ```
+    """
+    bw = asbpf(bw)
+    return (bw.rand() + (center - bw*0.5))[bw.x0:bw.x1]
+    
+
+def blendwithfloor(b: core.BpfInterface, mix=0.5) -> core._BpfBlend:
+    return core.blend(b, asbpf(b(maximum(b))), mix)[b.x0:b.x1]
+    
+    
+def blendwithceil(b, mix=0.5) -> core._BpfBlend:
+    return core.blend(b, asbpf(b(maximum(b))), mix)[b.x0:b.x1]
+    
+
+def smoothen(b: core.BpfInterface, window:int, N=1000, interpol='linear') -> core.BpfInterface:
+    """
+    Return a linear bpf representing a smooth version of b
+
+    Args:
+        b: a bpf
+        window: the width (in x coords) of the smoothing window
+        N: number of points to resample the bpf
+        interpol: the interpolation to use. One of 'linear', 'smooth', 'halfcos'
+
+    Returns:
+        a bpf representing a smoother version of b
+    """
+    dx = min((b.x1 - b.x0) / N, window/7)
+    nwin = int(window / dx)
+    box = np.ones(nwin)/nwin
+    Y = b[::dx].ys
+    Y2 = np.convolve(Y, box, mode="same")
+    X = np.linspace(b.x0, b.x1, len(Y2))
+    if interpol == 'linear':
+        return core.Linear(X, Y2)
+    elif interpol == 'smooth':
+        return core.Smooth(X, Y2)
+    elif interpol == 'halfcos':
+        return core.Halfcos(X, Y2)
+    else:
+        raise ValueError(f"Interpolation {interpol} not supported here. "
+                          "Possible values: linear, smooth, halfcos")
+
+
+def zigzag(b0: core.BpfInterface,
+           b1: core.BpfInterface,
+           xs: Sequence[float],
+           shape='linear'
+           ) -> core.BpfInterface:
+    """
+    Creates a curve formed of lines from b0(x) to b1(x) for each x in xs
+
+    Args:
+        b0: a bpf
+        b1: a bpf
+        xs: a seq. of x values to evaluate b0 and b1
+        shape: the shape of each segment
+
+    Returns:
+        The resulting bpf
+
+    ::
+
+       *.
+        *...  b0
+         *  ...
+         *     ...
+          *       ....
+           *          ...
+            *         :  ...
+             *        :*    ...
+             *        : *      ...
+              *       :  **       ...
+               *      :    *         :*.
+                *     :     *        : **...
+                 *    :      *       :   *  ...
+                 *    :       *      :    *    ...
+                  *   :        *     :     **     .:.
+                   *  :         *    :       *     :**..
+                    * :          **  :        **   :  ****.
+                     *:            * :          *  :      ****
+        -----------  *:             *:           * :          ****
+          b1       ---*--------------*---         **:             ****
+                                         -----------*----------      .**
+                                                               -----------
+        x0            x1              x2                       x3
+
+    """
+    curves = []
+    for x0, x1 in pairwise(xs):
+        X = [x0, x1]
+        Y = [b0(x0), b1(x1)]
+        curve = bpf.util.makebpf(shape, X, Y)
+        curves.append(curve)
+    jointcurve = bpf.max_(*[c.outbound(0, 0) for c in curves])
+    return jointcurve
+
+
+def bpfavg(b: core.BpfInterface,
+           dx: float
+           ) -> core.BpfInterface:
+    """
+    Return a Bpf which is the average of b over the range `dx`
+
+    Args:
+        b: the bpf
+        dx: the period to average *b* over
+
+    Returns:
+        a bpf representing the average of *b* along the bounds of
+        *b* over a sliding period of *dx*
+    """
+    dx2 = dx/2
+    avg = ((b<<dx2)+b+(b>>dx2))/3.0
+    return avg[b.x0:b.x1]
+
+
+def histbpf(b: core.BpfInterface, numbins=10, numsamples=200, interpolation='linear'
+            ) -> core.BpfInterface:
+    """
+    Create a historgram of *b*
+
+    Args:
+        b: the bpf
+        numbins: the number of bins
+        numsamples: how many samples to take to determine the histogram
+        interpolation: the kind of interpolation of the returned bpf
+
+    Returns:
+        a bpf representing the percentile associated with a given value of *b*
+        Percentiles are given between 0 and 1
+
+    Example
+    ~~~~~~~
+
+    >>> from sndfileio import *
+    >>> samples, sr = sndread("path/to/soundfile.wav")
+    >>> dbcurve = rmsbpf(samples, sr=sr).amp2db()
+    >>> dbhist = histbpf(dbcurve)
+    # Find the db percentile at a given time, this gives a measurement of the
+    # relative strength of the sound at a given moment
+    >>> dur = len(samples)/sr
+    >>> percentile = dbhist(dur*0.5)
+    0.312
+
+    This indicates that at the middle of the sound the amplitude is at percentile ~30
+
+    """
+    samples = b.map(numsamples)
+    edges, hist = np.histogram(b, bins=numbins)
+    percentile = np.linspace(0, 1, len(hist))
+    if interpolation == 'linear':
+        return core.Linear(hist, percentile)
+    elif interpolation == 'nointerpol':
+        return core.NoInterpol(hist, percentile)
+    else:
+        raise ValueError("Only 'linear' or 'nointerpol' are supported")
```

## bpf4/version.py

```diff
@@ -1,4 +1,4 @@
-__version__ = (1, 8, 8)
-    
-def versionstr():
-    return ("%d.%d.%d" % __version__)
+__version__ = (1, 9, 0)
+    
+def versionstr():
+    return ("%d.%d.%d" % __version__)
```

## Comparing `bpf4-1.8.8.dist-info/METADATA` & `bpf4-1.9.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-Metadata-Version: 2.1
-Name: bpf4
-Version: 1.8.8
-Summary: Piece-wise interpolation and lazy evaluation in cython
-Home-page: https://github.com/gesellkammer/bpf4
-Download-URL: https://github.com/gesellkammer/bpf4
-Author: eduardo moguillansky
-Author-email: eduardo.moguillansky@gmail.com
-Maintainer: 
-Maintainer-email: 
-License: BSD 3-Clause License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: numpy >=1.8
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-
-BPF4
-====
-
-![wheels](https://github.com/gesellkammer/bpf4/actions/workflows/wheels.yml/badge.svg)
-
-
-About
------
-
-**bpf4** is a python library to operate with curves in 2D space. 
-
-Curves can be defined via breakpoints (break-point functions, hence the name) or using functions.
-Moreover, curves can be used to build other curves. **bpf4** can be used to perform
-curve fitting, data analysis, plotting, etc. Its core is programmed
-in cython for efficiency.
-
-
-Installation
-------------
-
-
-```bash
-pip install --upgrade bpf4
-
-```
-
-Documentation
--------------
-
-The documentation is hosted at https://bpf4.readthedocs.io
-
-
------------------
-
-Example
--------
-
-Find the intersection between two curves
-
-```python
-
-from bpf4 import bpf  # this imports the api
-a = bpf.spline((0, 0), (1, 5), (2, 3), (5, 10))  # each point (x, y)
-b = bpf.expon((0, -10), (2,15), (5, 3), exp=3)
-a.plot() # uses matplotlib
-b.plot() 
-zeros = (a - b).zeros()
-import pylab
-pylab.plot(zeros, a.map(zeros), 'o')
-```
-   
-![1](https://github.com/gesellkammer/bpf4/raw/master/pics/zeros.png)
-
-Features
---------
-
-Many interpolation types besides linear:
-
-* spline
-* univariate splie
-* pchip (hermite)
-* cosine
-* exponential
-* logarithmic
-* etc. 
-
-
-With the exception of curve-fitting bpfs (splines), interpolation types can be mixed, so that each segment 
-has a different interpolation. Following from the example above:  
-
-
-```pyton
-
-c = (a + b).sin().abs()
-# plot only the range (1.5, 4)
-c[1.5:4].plot()  
-
-```
-
-![2](https://github.com/gesellkammer/bpf4/raw/master/pics/sinabs.png)
-
-Syntax support for shifting, scaling and slicing a bpf
-
-```python
-
-a >> 2        # a shifted to the right
-(a * 5) ^ 2   # scale the x coord by 2, scale the y coord by 5
-a[2:2.5]      # slice only a portion of the bpf
-a[::0.01]     # sample the bpf with an interval of 0.01
-
-```
-
-### Derivation / Integration
-
-```python
-from bpf4 import *
-a = spline((0, 0), (1, 5), (2, 3), (5, 10))
-deriv = a.derivative()
-integr = a.integrated()
-
-import matplotlib.pyplot as plt 
-fig, axs = plt.subplots(3, 1, sharex=True, figsize=(16, 8), tight_layout=True)
-a.plot(axes=axs[0], show=False)
-deriv.plot(axes=axs[1], show=False)
-integr.plot(axes=axs[2])
-```
-
-![](docs/assets/deriv3.png)
-
-
-----------------
-
-## Mathematical operations
-
-### Max / Min
-
-```python
-a = linear(0, 0, 1, 0.5, 2, 0)
-b = expon(0, 0, 2, 1, exp=3)
-a.plot(show=False, color="red", linewidth=4, alpha=0.3)
-b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
-core.Max((a, b)).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
-```
-![](docs/assets/Max.png)
-
-```python
-a = linear(0, 0, 1, 0.5, 2, 0)
-b = expon(0, 0, 2, 1, exp=3)
-a.plot(show=False, color="red", linewidth=4, alpha=0.3)
-b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
-core.Min((a, b)).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
-```
-![](docs/assets/Min.png)
-
-
-### `+, -, *, /`
-
-```
-a = linear(0, 0, 1, 0.5, 2, 0)
-b = expon(0, 0, 2, 1, exp=3)
-a.plot(show=False, color="red", linewidth=4, alpha=0.3)
-b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
-(a*b).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
-```
-![](docs/assets/math-mul.png)
-
-```python
-a = linear(0, 0, 1, 0.5, 2, 0)
-b = expon(0, 0, 2, 1, exp=3)
-a.plot(show=False, color="red", linewidth=4, alpha=0.3)
-b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
-(a**b).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
-```
-![](docs/assets/math-pow.png)
-
-```python
-a = linear(0, 0, 1, 0.5, 2, 0)
-b = expon(0, 0, 2, 1, exp=3)
-a.plot(show=False, color="red", linewidth=4, alpha=0.3)
-b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
-((a+b)/2).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
-```
-![](docs/assets/math-avg.png)
-
-### Building functions
-
-A bpf can be used to build complex formulas
-
-**Fresnel's Integral**: \( S(x) = \int_0^x {sin(t^2)} dt \)
-
-```python
-t = slope(1)
-f = (t**2).sin()[0:10:0.001].integrated()
-f.plot()
-```
-
-![](docs/assets/fresnel.png)
-
-
-#### Polar plots
-
-Any kind of matplotlib plot can be used. For example, polar plots are possible
-by creating an axes with *polar*=`True`
-
-**Cardiod**: \(\rho = 1 + sin(-\theta) \)
-
-```python
-
-from math import *
-theta = slope(1, bounds=(0, 2*pi))
-r = 1 + (-theta).sin()
-
-ax = plt.axes(polar=True)
-ax.set_rticks([0.5, 1, 1.5, 2]); ax.set_rlabel_position(38)
-r.plot(axes=ax)
-```
-![](docs/assets/cardioid.png)
-
-
-**Flower 5**: \(\rho = 3 + cos(5 * \theta) \)
-
-```python
-theta = core.Slope(1, bounds=(0, 2*pi))
-r = 3 + (5*theta).cos()
-
-ax = plt.axes(polar=True)
-r.plot(axes=ax)
-
-```
-![](docs/assets/polar1.png)
+Metadata-Version: 2.1
+Name: bpf4
+Version: 1.9.0
+Summary: Piece-wise interpolation and lazy evaluation in cython
+Home-page: https://github.com/gesellkammer/bpf4
+Download-URL: https://github.com/gesellkammer/bpf4
+Author: eduardo moguillansky
+Author-email: eduardo.moguillansky@gmail.com
+Maintainer: 
+Maintainer-email: 
+License: BSD 3-Clause License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: numpy >=1.8
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+
+BPF4
+====
+
+![wheels](https://github.com/gesellkammer/bpf4/actions/workflows/wheels.yml/badge.svg)
+
+
+About
+-----
+
+**bpf4** is a python library to operate with curves in 2D space. 
+
+Curves can be defined via breakpoints (break-point functions, hence the name) or using functions.
+Moreover, curves can be used to build other curves. **bpf4** can be used to perform
+curve fitting, data analysis, plotting, etc. Its core is programmed
+in cython for efficiency.
+
+
+Installation
+------------
+
+
+```bash
+pip install --upgrade bpf4
+
+```
+
+Documentation
+-------------
+
+The documentation is hosted at https://bpf4.readthedocs.io
+
+
+-----------------
+
+Example
+-------
+
+Find the intersection between two curves
+
+```python
+
+from bpf4 import bpf  # this imports the api
+a = bpf.spline((0, 0), (1, 5), (2, 3), (5, 10))  # each point (x, y)
+b = bpf.expon((0, -10), (2,15), (5, 3), exp=3)
+a.plot() # uses matplotlib
+b.plot() 
+zeros = (a - b).zeros()
+import pylab
+pylab.plot(zeros, a.map(zeros), 'o')
+```
+   
+![1](https://github.com/gesellkammer/bpf4/raw/master/pics/zeros.png)
+
+Features
+--------
+
+Many interpolation types besides linear:
+
+* spline
+* univariate splie
+* pchip (hermite)
+* cosine
+* exponential
+* logarithmic
+* etc. 
+
+
+With the exception of curve-fitting bpfs (splines), interpolation types can be mixed, so that each segment 
+has a different interpolation. Following from the example above:  
+
+
+```pyton
+
+c = (a + b).sin().abs()
+# plot only the range (1.5, 4)
+c[1.5:4].plot()  
+
+```
+
+![2](https://github.com/gesellkammer/bpf4/raw/master/pics/sinabs.png)
+
+Syntax support for shifting, scaling and slicing a bpf
+
+```python
+
+a >> 2        # a shifted to the right
+(a * 5) ^ 2   # scale the x coord by 2, scale the y coord by 5
+a[2:2.5]      # slice only a portion of the bpf
+a[::0.01]     # sample the bpf with an interval of 0.01
+
+```
+
+### Derivation / Integration
+
+```python
+from bpf4 import *
+a = spline((0, 0), (1, 5), (2, 3), (5, 10))
+deriv = a.derivative()
+integr = a.integrated()
+
+import matplotlib.pyplot as plt 
+fig, axs = plt.subplots(3, 1, sharex=True, figsize=(16, 8), tight_layout=True)
+a.plot(axes=axs[0], show=False)
+deriv.plot(axes=axs[1], show=False)
+integr.plot(axes=axs[2])
+```
+
+![](docs/assets/deriv3.png)
+
+
+----------------
+
+## Mathematical operations
+
+### Max / Min
+
+```python
+a = linear(0, 0, 1, 0.5, 2, 0)
+b = expon(0, 0, 2, 1, exp=3)
+a.plot(show=False, color="red", linewidth=4, alpha=0.3)
+b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
+core.Max((a, b)).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
+```
+![](docs/assets/Max.png)
+
+```python
+a = linear(0, 0, 1, 0.5, 2, 0)
+b = expon(0, 0, 2, 1, exp=3)
+a.plot(show=False, color="red", linewidth=4, alpha=0.3)
+b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
+core.Min((a, b)).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
+```
+![](docs/assets/Min.png)
+
+
+### `+, -, *, /`
+
+```
+a = linear(0, 0, 1, 0.5, 2, 0)
+b = expon(0, 0, 2, 1, exp=3)
+a.plot(show=False, color="red", linewidth=4, alpha=0.3)
+b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
+(a*b).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
+```
+![](docs/assets/math-mul.png)
+
+```python
+a = linear(0, 0, 1, 0.5, 2, 0)
+b = expon(0, 0, 2, 1, exp=3)
+a.plot(show=False, color="red", linewidth=4, alpha=0.3)
+b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
+(a**b).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
+```
+![](docs/assets/math-pow.png)
+
+```python
+a = linear(0, 0, 1, 0.5, 2, 0)
+b = expon(0, 0, 2, 1, exp=3)
+a.plot(show=False, color="red", linewidth=4, alpha=0.3)
+b.plot(show=False, color="blue", linewidth=4, alpha=0.3)
+((a+b)/2).plot(color="black", linewidth=4, alpha=0.8, linestyle='dotted')
+```
+![](docs/assets/math-avg.png)
+
+### Building functions
+
+A bpf can be used to build complex formulas
+
+**Fresnel's Integral**: \( S(x) = \int_0^x {sin(t^2)} dt \)
+
+```python
+t = slope(1)
+f = (t**2).sin()[0:10:0.001].integrated()
+f.plot()
+```
+
+![](docs/assets/fresnel.png)
+
+
+#### Polar plots
+
+Any kind of matplotlib plot can be used. For example, polar plots are possible
+by creating an axes with *polar*=`True`
+
+**Cardiod**: \(\rho = 1 + sin(-\theta) \)
+
+```python
+
+from math import *
+theta = slope(1, bounds=(0, 2*pi))
+r = 1 + (-theta).sin()
+
+ax = plt.axes(polar=True)
+ax.set_rticks([0.5, 1, 1.5, 2]); ax.set_rlabel_position(38)
+r.plot(axes=ax)
+```
+![](docs/assets/cardioid.png)
+
+
+**Flower 5**: \(\rho = 3 + cos(5 * \theta) \)
+
+```python
+theta = core.Slope(1, bounds=(0, 2*pi))
+r = 3 + (5*theta).cos()
+
+ax = plt.axes(polar=True)
+r.plot(axes=ax)
+
+```
+![](docs/assets/polar1.png)
```

