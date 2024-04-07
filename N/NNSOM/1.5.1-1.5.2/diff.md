# Comparing `tmp/nnsom-1.5.1.tar.gz` & `tmp/nnsom-1.5.2.tar.gz`

## Comparing `nnsom-1.5.1.tar` & `nnsom-1.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    76967 2020-02-02 00:00:00.000000 nnsom-1.5.1/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 nnsom-1.5.1/src/NNSOM/som.py
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.5.1/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.1/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.1/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    77087 2020-02-02 00:00:00.000000 nnsom-1.5.2/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 nnsom-1.5.2/src/NNSOM/som.py
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.5.2/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.2/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.2/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.2/PKG-INFO
```

### Comparing `nnsom-1.5.1/src/NNSOM/plots.py` & `nnsom-1.5.2/src/NNSOM/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,23 +328,26 @@
         # divider = make_axes_locatable(ax)
         # cax = divider.append_axes("right", size="5%", pad=0.05)
         #
         # cbar = plt.colorbar(ax, cax=cax, cmap=cmap)
 
         cax = cm.ScalarMappable(cmap=cmap)
         cax.set_array(xx)
-        cbar = fig.colorbar(cax)
+        cbar = fig.colorbar(cax, ax=ax)
 
         # Adjust the tick labels to the correct scale
         ticklab = cbar.ax.get_yticks()
         numticks = len(ticklab)
         ticktext = []
         for i in range(numticks):
             ticktext.append('%.2f' % (dmax * ticklab[i]))
 
+        # Set the ticks first
+        cbar.ax.set_yticks(ticklab)
+
         cbar.ax.set_yticklabels(ticktext)
 
         # Get rid of extra white space on sides
         fig.tight_layout()
 
         return fig, ax, patches, text, cbar
 
@@ -758,15 +761,15 @@
         # # Add a color bar the the figure to indicate levels
         # # create an axes on the right side of ax. The width of cax will be 5%
         # # of ax and the padding between cax and ax will be fixed at 0.05 inch.
 
         cax = cm.ScalarMappable(cmap=cmap)
         cax.set_array(xx)
         # cbar = fig.colorbar(cax)
-        cbar = fig.colorbar(cax, fraction=0.046, pad=0.04)
+        cbar = fig.colorbar(cax, ax = ax, fraction=0.046, pad=0.04)
 
         # plt.colorbar(im, fraction=0.046, pad=0.04)
         #
         # divider = make_axes_locatable(ax)
         # cax = divider.append_axes("right", size="5%", pad=0.05)
         #
         # plt.colorbar(im, cax=cax)
@@ -774,14 +777,16 @@
         # Adjust the tick labels to the correct scale
         ticklab = cbar.ax.get_yticks()
         numticks = len(ticklab)
         ticktext = []
         for i in range(numticks):
             ticktext.append('%.2f' % (drange * ticklab[i] + dmin))
 
+        cbar.ax.set_yticks(ticklab)
+
         cbar.ax.set_yticklabels(ticktext)
 
         if mouse_click and connect_pick_event:
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
```

### Comparing `nnsom-1.5.1/src/NNSOM/som.py` & `nnsom-1.5.2/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.1/src/NNSOM/utils.py` & `nnsom-1.5.2/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.1/.gitignore` & `nnsom-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.1/pyproject.toml` & `nnsom-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.5.1"
+version = "1.5.2"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.5.1/PKG-INFO` & `nnsom-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.5.1
+Version: 1.5.2
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

