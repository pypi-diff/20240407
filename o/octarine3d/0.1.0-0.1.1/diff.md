# Comparing `tmp/octarine3d-0.1.0.tar.gz` & `tmp/octarine3d-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octarine3d-0.1.0.tar", last modified: Sat Mar 23 20:28:06 2024, max compression
+gzip compressed data, was "octarine3d-0.1.1.tar", last modified: Sun Apr  7 11:37:27 2024, max compression
```

## Comparing `octarine3d-0.1.0.tar` & `octarine3d-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2024-03-23 20:28:06.303367 octarine3d-0.1.0/
--rw-r--r--   0 philipps   (501) staff       (20)     1305 2024-03-22 14:15:33.000000 octarine3d-0.1.0/LICENSE
--rw-r--r--   0 philipps   (501) staff       (20)     4604 2024-03-23 20:28:06.303003 octarine3d-0.1.0/PKG-INFO
--rw-r--r--   0 philipps   (501) staff       (20)     3667 2024-03-23 20:27:16.000000 octarine3d-0.1.0/README.md
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2024-03-23 20:28:06.301947 octarine3d-0.1.0/octarine/
--rw-r--r--   0 philipps   (501) staff       (20)       41 2024-03-22 17:20:45.000000 octarine3d-0.1.0/octarine/__init__.py
--rw-r--r--   0 philipps   (501) staff       (20)       21 2024-03-22 14:23:28.000000 octarine3d-0.1.0/octarine/__version__.py
--rw-r--r--   0 philipps   (501) staff       (20)     1294 2024-03-22 23:17:40.000000 octarine3d-0.1.0/octarine/config.py
--rw-r--r--   0 philipps   (501) staff       (20)    11129 2024-03-23 18:22:20.000000 octarine3d-0.1.0/octarine/controls.py
--rw-r--r--   0 philipps   (501) staff       (20)     3843 2024-03-23 18:17:44.000000 octarine3d-0.1.0/octarine/utils.py
--rw-r--r--   0 philipps   (501) staff       (20)    29156 2024-03-23 19:14:25.000000 octarine3d-0.1.0/octarine/viewer.py
--rw-r--r--   0 philipps   (501) staff       (20)     7752 2024-03-23 16:03:50.000000 octarine3d-0.1.0/octarine/visuals.py
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2024-03-23 20:28:06.302790 octarine3d-0.1.0/octarine3d.egg-info/
--rw-r--r--   0 philipps   (501) staff       (20)     4604 2024-03-23 20:28:06.000000 octarine3d-0.1.0/octarine3d.egg-info/PKG-INFO
--rw-r--r--   0 philipps   (501) staff       (20)      385 2024-03-23 20:28:06.000000 octarine3d-0.1.0/octarine3d.egg-info/SOURCES.txt
--rw-r--r--   0 philipps   (501) staff       (20)        1 2024-03-23 20:28:06.000000 octarine3d-0.1.0/octarine3d.egg-info/dependency_links.txt
--rw-r--r--   0 philipps   (501) staff       (20)        1 2024-03-23 20:28:06.000000 octarine3d-0.1.0/octarine3d.egg-info/not-zip-safe
--rw-r--r--   0 philipps   (501) staff       (20)       34 2024-03-23 20:28:06.000000 octarine3d-0.1.0/octarine3d.egg-info/requires.txt
--rw-r--r--   0 philipps   (501) staff       (20)        9 2024-03-23 20:28:06.000000 octarine3d-0.1.0/octarine3d.egg-info/top_level.txt
--rw-r--r--   0 philipps   (501) staff       (20)       80 2024-03-23 19:35:16.000000 octarine3d-0.1.0/pyproject.toml
--rw-r--r--   0 philipps   (501) staff       (20)       38 2024-03-23 20:28:06.303406 octarine3d-0.1.0/setup.cfg
--rw-r--r--   0 philipps   (501) staff       (20)     1613 2024-03-23 20:27:55.000000 octarine3d-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:27.732447 octarine3d-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-07 11:37:25.000000 octarine3d-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-07 11:37:27.732447 octarine3d-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-07 11:37:25.000000 octarine3d-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:27.732447 octarine3d-0.1.1/octarine/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:27.732447 octarine3d-0.1.1/octarine3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-07 11:37:25.000000 octarine3d-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:37:27.732447 octarine3d-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-07 11:37:25.000000 octarine3d-0.1.1/setup.py
```

### Comparing `octarine3d-0.1.0/LICENSE` & `octarine3d-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.0/PKG-INFO` & `octarine3d-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,56 @@
-Metadata-Version: 2.1
-Name: octarine3d
-Version: 0.1.0
-Summary: WGPU-based 3d viewer
-Home-page: https://github.com/schlegelp/octarine
-Author: Philipp Schlegel
-Author-email: pms70@cam.ac.uk
-License: BSD-2-Clause
-Project-URL: Source, https://github.com/schlegelp/octarine
-Project-URL: Changelog, https://github.com/schlegelp/octarine/releases
-Keywords: 3D viewer WGPU pygfx
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pygfx
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: pypng
-Requires-Dist: six
-Requires-Dist: cmap
-
-![cocoa](docs/_static/octarine_logo_banner.png)
+![octarine banner](https://schlegelp.github.io/octarine/_static/octarine_logo_banner.png)
 <p align="center">
 <i>
 Octarine is the eighth color of the Discworld's spectrum, which is described as the color of magic itself. Only wizards and cats can see it.
 </i>
 </p>
 
+[![docs](https://github.com/schlegelp/octarine/actions/workflows/docs.yml/badge.svg)](https://schlegelp.github.io/octarine/)
+
 # Octarine
-A high-performance, easy-to-use 3D viewer. `Octarine` is build on top of the excellent
+A minimalist, easy-to-use, high-performance 3D viewer. `Octarine` is build on top of the excellent
 [`pygfx`](https://github.com/pygfx/pygfx) WGPU rendering engine which does most of the heavy lifting - we're simply
 abstracting away some of the boiler plate code for you.
 
 ## Rationale :thought_balloon:
 Why another 3d viewer? There are plenty options out there:
-[`vedo`](https://github.com/marcomusy/vedo), [`ipygany`](https://github.com/jupyter-widgets-contrib/ipygany), [`polyscope`](https://github.com/nmwsharp/polyscope), [`napari`](https://github.com/napari/napari), [`fury`](https://github.com/fury-gl/fury) or [`pyvista`](https://github.com/pyvista/pyvista) to name but a few. All of these are great in their own right but I wanted something (a) without heavy dependencies (i.e. no VTK), (b) that lets me interactively explore my data in both REPL and Jupyter and (c) is very performant. None of the above ticked all those boxes for me.
+[`vedo`](https://github.com/marcomusy/vedo), [`ipygany`](https://github.com/jupyter-widgets-contrib/ipygany), [`polyscope`](https://github.com/nmwsharp/polyscope), [`napari`](https://github.com/napari/napari), [`fury`](https://github.com/fury-gl/fury), [`plotly`](https://github.com/plotly/plotly.py) or [`pyvista`](https://github.com/pyvista/pyvista) to name but a few. All of these are great in their own right but I wanted something *(a)* without heavy dependencies (i.e. no VTK), *(b)* that lets me interactively explore my data in both REPL and Jupyter and *(c)* is very performant. None of the existing solutions ticked all those boxes for me.
 
 `Octarine` tries to fill that gap:
 1. _Lightweight_ with very few direct or indirect dependencies.
 2. Works in both _Jupyter_ and _REPL_.
-3. _High performance_: a mesh with 15M faces renders with 80 fps at 1080p (2023 MacBook Pro).
+3. _High performance_: a mesh with 15M faces renders with 80 fps at 1080p on a 2023 MacBook Pro.
 
 ## ToDo :ballot_box_with_check:
 This is still a prototype but basic stuff already works (mostly because `pygfx` makes it so ridiculously easy).
 
 - [x] basic datatypes: meshes, points, scatter, volumes
 - [x] custom keyboard shortcuts
 - [x] rudamentary controls + legend
-- [ ] user-defined animations
-- [ ] proper docs
+- [x] screenshots
+- [x] support for trimesh scenes
+- [x] user-defined animations
+- [x] documentation
+- [ ] methods/controls to manipulate image volumes
 - [ ] tests
 
 ## Installation :rocket:
 
 ```bash
 pip install octarine3d
 ```
 
-In addition you will need to install at least one window manager supported by [wgpu-py](https://github.com/pygfx/wgpu-py):
+In addition you will need to install at least one window manager supported by [`wgpu-py`](https://github.com/pygfx/wgpu-py):
 - qt: PySide6, PyQt6, PySide2, PyQt5 all work but I recommend PySide6 (see below)
 - glfw: a lightweight GUI for the desktop
 - jupyter_rfb: only needed if you plan on using `Octarine` in Jupyter
 - wx
 
-Please note that at this point, `Octarine`'s controls panel requires `PySide6`. So if you need GUI controls you have to use `PySide6`.
+Please note that at this point, `Octarine`'s controls panel requires `PySide6`. So if you want GUI controls you have to use `PySide6`.
 
 ## Quickstart :fire:
 
 ```python
 # Create a Viewer instance
 from octarine import Viewer
 v = Viewer()
@@ -92,37 +69,64 @@
 m = gfx.geometries.mobius_strip_geometry()
 v.add(m, color='b')
 
 # Close the viewer
 v.close()
 ```
 
+![demo gif](docs/_static/octarine_demo_720p.gif)
+
 Other selected `Viewer` methods:
 - `add()`: generic method to add stuff to the viewer; will call respective specialised methods
 - `add_lines()`: add line plot
 - `add_mesh()`: add meshes (anything that has `.vertices` and `.faces` goes)
-- `add_scatter()`: add a scatter plot
+- `add_points()`: add a scatter plot
 - `add_volume()`: add an image volume
 - `center_camera()`: center camera on scene
 - `clear()`: clear scene
 - `close()`: close viewer
 - `colorize()`: cycle colors for all objects
 - `pop()`: remove last added object
-- `remove()`: remove a given object(s) from the scene
+- `remove_objects()`: remove a given object(s) from the scene
 - `screenshot()`: take (and save) a screenshot
 - `set_bgcolor()`: set background color
 - `set_colors()`: set object colors
 
 ### Hotkeys
 The following keyboard shortcuts are hard-coded:
 - `1`: reset view to XY (frontal)
 - `2`: reset view to XZ (dorsal)
 - `3`: reset view to YZ (lateral)
 - `f`: show FPS
-- `c`: show control panel
+- `c`: show control panel (requires `PySide6`)
 
 You can also bind custom functions to keys:
 
 ```python
 # Bind `x` key to the cycle-colors method
 v.key_events['x'] = lambda : v.colorize()
 ```
+
+## Want to contribute?
+We welcome all kinds of contributions. For example:
+
+- reports of bugs, broken examples, etc.
+- feature requests
+- pull requests with bug fixes or new features
+
+If you already know what needs doing, feel free to open a pull request
+right away. When in doubt please open an [issue](https://github.com/schlegelp/octarine/issues)
+so we can discuss the best way to address the issue.
+
+## Development :dash:
+
+### Tests
+TODO
+
+### Docs
+
+To generate the documentation:
+
+```bash
+pip install -e .[docs]
+mkdocs build
+```
```

### Comparing `octarine3d-0.1.0/octarine/config.py` & `octarine3d-0.1.1/octarine/config.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.0/octarine/controls.py` & `octarine3d-0.1.1/octarine/controls.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,68 @@
+import numpy as np
 import pygfx as gfx
 
 try:
-    from PySide6 import QtWidgets, QtGui, QtCore
+    from PySide6 import QtWidgets, QtCore
 except ImportError:
     raise ImportError("Showing controls requires PySide6. Please install it via:\n `pip install PySide6`.")
 
 # TODOs:
 # - add custom legend formatting (e.g. "{object.name}")
 # - show type of object in legend
 # - add dropdown to manipulate all selected objects
 # - add filter to legend (use item.setHidden(True/False) to show/hide items)
 # - highlight object in legend when hovered over in scene
+# - make legend tabbed (QTabWidget)
 
 class Controls(QtWidgets.QWidget):
     def __init__(self, viewer, width=200, height=400):
         super().__init__()
         self.viewer = viewer
         self.setWindowTitle("Legend")
         self.resize(width, height)
 
         self.btn_layout = QtWidgets.QVBoxLayout()
         self.setLayout(self.btn_layout)
 
+        # Build legend
         self.build_gui()
 
+        # Populate legend
+        self.update_legend()
+
+        # This determines the target for color changes
+        self.active_objects = None
+
+        self.color_picker = QtWidgets.QColorDialog(parent=self)
+        self.color_picker.currentColorChanged.connect(self.set_color)
+        self.color_picker.colorSelected.connect(self.reset_active_objects)
+
     def build_gui(self):
         """Build the GUI."""
-
-        # Add legend
+        # Add legend (i.e. a list widget)
         self.legend = self.create_legend()
 
+        # Add the dropdown to action all selected objects
+        self.sel_action = QtWidgets.QPushButton(text="Action")
+        self.sel_action_menu = QtWidgets.QMenu(self)
+        self.sel_action_menu.addAction("Hide")
+        self.sel_action_menu.actions()[-1].triggered.connect(self.hide_selected)
+        self.sel_action_menu.addAction("Show")
+        self.sel_action_menu.actions()[-1].triggered.connect(self.show_selected)
+        self.sel_action_menu.addAction("Delete")
+        self.sel_action_menu.actions()[-1].triggered.connect(self.delete_selected)
+        self.sel_action_menu.addAction("Color")
+        self.sel_action_menu.actions()[-1].triggered.connect(self.color_selected)
+        self.sel_action.setMenu(self.sel_action_menu)
+        self.btn_layout.addWidget(self.sel_action)
+
+        # Add horizontal divider
+        self.add_split()
+
         # First: add button to toggle flat shading
         self.mesh_flat_checkbox = self.create_checkbox(
             "Flat Shading", gfx.Mesh, "material.flat_shading"
         )
 
         # Second: add button to toggle wireframe
         self.mesh_wireframe_checkbox = QtWidgets.QCheckBox("Wireframe")
@@ -43,14 +72,15 @@
             for vis in self.viewer.scene.children:
                 if isinstance(vis, gfx.Mesh):
                     vis.material.wireframe = self.mesh_wireframe_checkbox.isChecked()
 
         self.mesh_wireframe_checkbox.toggled.connect(set_wireframe)
         self.btn_layout.addWidget(self.mesh_wireframe_checkbox)
 
+        # Add horizontal divider
         self.add_split()
 
         # Third: add controls to adjust ambient light
         self.ambient_light_checkbox = QtWidgets.QCheckBox("Ambient Light")
         self.ambient_light_checkbox.setChecked(True)
 
         def toggle_ambient_light(*args):
@@ -61,39 +91,43 @@
         self.ambient_light_checkbox.toggled.connect(toggle_ambient_light)
         self.btn_layout.addWidget(self.ambient_light_checkbox)
 
         self.ambient_light_slider = self.create_slider(
                     "Intensity", 0, 10, gfx.AmbientLight, "intensity", step=0.01
                 )
 
-        self.add_split()
+        # Add horizontal divider
+        # self.add_split()
 
-        self.btn_layout.addStretch(1)
+        # This would make it so the legend does not stretch when
+        # we resize the window vertically
+        # self.btn_layout.addStretch(1)
 
         return
 
     def add_split(self):
+        """Add horizontal divider."""
         # self.btn_layout.addSpacing(5)
         self.btn_layout.addWidget(QHLine())
         # self.btn_layout.addSpacing(5)
 
     def create_legend(self, spacing=0, index=None):
         """Generate the legend widget."""
         layout = QtWidgets.QHBoxLayout()
         layout.addWidget(QtWidgets.QLabel("Legend"))
         list_widget = QtWidgets.QListWidget()
         list_widget.setSelectionMode(QtWidgets.QAbstractItemView.ExtendedSelection)
         layout.addWidget(list_widget)
         list_widget.setSpacing(spacing)
 
-        # Add some example items
-        for i, c in enumerate(["red", "green", "blue"]):
-            item, item_widget = self.make_legend_entry(f"Item {i}", color=c)
-            list_widget.addItem(item)
-            list_widget.setItemWidget(item, item_widget)
+        # Add some example items (for debugging only)
+        # for i, c in enumerate(["red", "green", "blue"]):
+        #     item, item_widget = self.make_legend_entry(f"Item {i}", color=c)
+        #     list_widget.addItem(item)
+        #     list_widget.setItemWidget(item, item_widget)
 
         if index is not None:
             self.btn_layout.insertWidget(index, list_widget)
         else:
             self.btn_layout.addWidget(list_widget)
 
         return list_widget
@@ -110,39 +144,53 @@
 
         Returns
         -------
         item :      QtWidgets.QListWidgetItem
                     List item.
         item_widget : QtWidgets.QWidget
                     List item widget.
+
         """
         # Initialize widget and item
         item_widget = QtWidgets.QWidget()
+        item_widget.setObjectName(name)
         item = QtWidgets.QListWidgetItem()
         item._id = name  # this helps to identify the item
 
-        # Generate a button
+        # Generate the label
         line_text = QtWidgets.QLabel(f"{name}")
-        line_push_button = QtWidgets.QPushButton()
-        line_push_button.setMaximumWidth(20)
-        line_push_button.setMaximumHeight(20)
-        line_push_button.setObjectName(name)  # this helps to identify the button
-        line_push_button.clicked.connect(self._clicked)  # connect button to function
-
-        if color is not None:
-            color = gfx.Color(color).css
-            line_push_button.setStyleSheet(f"background-color: {color}")
+        line_text.setToolTip("Click to select")
+
+        # Generate the checkbox
+        line_checkbox = QtWidgets.QCheckBox()
+        line_checkbox.setObjectName(name)  # this helps to identify the checkbox
+        line_checkbox.setMaximumWidth(40)
+        line_checkbox.setToolTip("Toggle visibility")
+        line_checkbox.setChecked(True)
+
+        def set_property(*args):
+            for vis in self.viewer.objects.get(name, []):
+                # Navigate to the correct property
+                vis.visible = line_checkbox.isChecked()
+
+        line_checkbox.toggled.connect(set_property)
+
+        # Generate the button
+        line_push_button = self.create_color_btn(name, color=color, callback=None)
 
         # Generate item layout
         item_layout = QtWidgets.QHBoxLayout()
         item_layout.setContentsMargins(0, 0, 0, 0)  # make layout tight
         item_layout.setSpacing(0)
+
         # Add text and button to layout
         item_layout.addWidget(line_text)
+        item_layout.addWidget(line_checkbox)
         item_layout.addWidget(line_push_button)
+
         # Set layout
         item_widget.setLayout(item_layout)
         item.setSizeHint(item_widget.sizeHint())
 
         return item, item_widget
 
     def update_legend(self):
@@ -185,46 +233,96 @@
                     # Note to self: need to make sure we also cater for color arrays
                     # which are in the geometry object
                     color = 'k'
                 item, item_widget = self.make_legend_entry(obj, color=color)
                 self.legend.addItem(item)
                 self.legend.setItemWidget(item, item_widget)
 
-    def _clicked(self):
+    def color_button_clicked(self):
+        """Set the active object to be the buttons target."""
         sender = self.sender()
         push_button = self.findChild(QtWidgets.QPushButton, sender.objectName())
         # print(f'click: {push_button.objectName()}')
+        self.active_objects = push_button.objectName()
+        self.color_picker.show()
 
-    def create_color_btn(self, name, target, property, callback=None):
-        layout = QtWidgets.QHBoxLayout()
-
-        layout.addWidget(QtWidgets.QLabel(name))
-
+    def set_color(self, color):
+        """Color current active object(s). This is the callback for the color picker."""
+        if self.active_objects is None:
+            return
+        elif self.active_objects == "selected":
+            targets = self.get_selected()
+        elif not isinstance(self.active_objects, list):
+            targets = [self.active_objects]
+
+        # Convert QColor to [0-1] RGB
+        color = np.array(color.toTuple()) / 255
+
+        self.viewer.set_colors({name: color for name in targets})
+
+    def get_selected(self):
+        """Get selected items."""
+        sel = []
+        for item in self.legend.selectedItems():
+            sel.append(item._id)
+        return sel
+
+    def color_selected(self):
+        """Set the active object to be the selected objects."""
+        self.active_objects = "selected"
+        self.color_picker.show()
+
+    def hide_selected(self):
+        """Hide selected objects."""
+        sel = self.get_selected()
+        if sel:
+            self.viewer.hide_objects(self.get_selected())
+
+    def show_selected(self):
+        """Show selected objects."""
+        sel = self.get_selected()
+        if sel:
+            self.viewer.unhide_objects(self.get_selected())
+
+    def delete_selected(self):
+        """Delete selected objects."""
+        sel = self.get_selected()
+        if sel:
+            self.viewer.remove_objects(self.get_selected())
+
+    def reset_active_objects(self):
+        """Reset active objects."""
+        self.color_target = None
+
+    def create_color_btn(self, name, color=None, callback=None):
+        """Generate a colorize button ."""
+        # Generate button
         color_btn = QtWidgets.QPushButton()
-        color_btn.setStyleSheet("background-color: %s" % getattr(target, property).hex)
 
-        def set_color():
-            color = QtWidgets.QColorDialog.getColor(
-                QtGui.QColor(getattr(target, property).hex)
-            )
-            if color.isValid():
-                color_btn.setStyleSheet("background-color: %s" % color.name())
-                setattr(target, property, color.name())
-                if callback:
-                    callback(color.name())
+        # Make sure it doesn't take up too much space
+        color_btn.setMaximumWidth(20)
+        color_btn.setMaximumHeight(20)
+        color_btn.setObjectName(name)
+
+        # Set tooltip
+        color_btn.setToolTip("Click to change color")
+
+        # Set color (will be updated subsequently via controls.update_legend())
+        if color is None:
+            color = 'w'
+        color = gfx.Color(color)
+        color_btn.setStyleSheet(f"background-color: {color.css}")
 
-        color_btn.clicked.connect(set_color)
+        # Connect callback (this just sets the active object)
+        color_btn.clicked.connect(self.color_button_clicked)
 
-        layout.addWidget(color_btn)
-        self.btn_layout.addLayout(layout)
         return color_btn
 
-    def create_checkbox(
-        self, name, targets=None, property=None, callback=None, toggle=[], index=None, default_value=False
-    ):
+    def create_checkbox(self, name, targets=None, property=None, callback=None, toggle=[], index=None, default_value=False):
+        """Create a checkbox to toggle a property."""
         checkbox = QtWidgets.QCheckBox(name)
 
         checkbox.setChecked(bool(default_value))
 
         def set_property(*args):
             path = property.split(".")
             for vis in self.viewer.scene.children:
@@ -244,14 +342,15 @@
         if index is not None:
             self.btn_layout.insertWidget(index, checkbox)
         else:
             self.btn_layout.addWidget(checkbox)
         return checkbox
 
     def create_slider(self, name, min, max, targets, property, step=1, callback=None):
+        """Generate a slider to adjust a property."""
         layout = QtWidgets.QHBoxLayout()
         layout.addWidget(QtWidgets.QLabel(name))
         slide = QtWidgets.QSlider(QtCore.Qt.Horizontal)
         slide.setMinimum(min / step)
         slide.setMaximum(max / step)
         # slide.setSingleStep(step)
         val = 0
@@ -285,30 +384,19 @@
         slide.valueChanged.connect(set_value)
 
         layout.addWidget(slide)
 
         self.btn_layout.addLayout(layout)
         return slide
 
-
-    #     self.hello = ["Hallo Welt", "Hei maailma", "Hola Mundo", "Привет мир"]
-
-    #     self.button = QtWidgets.QPushButton("Click me!")
-    #     self.text = QtWidgets.QLabel("Hello World",
-    #                                  alignment=QtCore.Qt.AlignCenter)
-
-    #     self.layout = QtWidgets.QVBoxLayout(self)
-    #     self.layout.addWidget(self.text)
-    #     self.layout.addWidget(self.button)
-
-    #     self.button.clicked.connect(self.magic)
-
-    # @QtCore.Slot()
-    # def magic(self):
-    #     self.text.setText(random.choice(self.hello))
+    def close(self):
+        """Close the controls."""
+        # This makes sure to also close the color picker, not just the controls window
+        self.color_picker.close()
+        super().close()
 
 
 class QHLine(QtWidgets.QFrame):
     def __init__(self):
         super(QHLine, self).__init__()
         self.setFrameShape(QtWidgets.QFrame.HLine)
         self.setFrameShadow(QtWidgets.QFrame.Sunken)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `octarine3d-0.1.0/octarine/utils.py` & `octarine3d-0.1.1/octarine/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import six
 
+import pygfx as gfx
 import numpy as np
 import pandas as pd
 
 from collections.abc import Iterable
 
 from . import config
 
@@ -74,22 +75,14 @@
     arrays = [ob for ob in arrays if any(np.isin(ob.shape, [2, 3]))]
 
     points = dataframes + arrays
 
     return meshes, volumes, points, visuals
 
 
-def is_mesh_like(x):
-    """Check if object is mesh (i.e. contains vertices and faces)."""
-    if hasattr(x, 'vertices') and hasattr(x, 'faces'):
-        return True
-
-    return False
-
-
 def make_iterable(x, force_type = None):
     """Force input into a numpy array.
 
     For dicts, keys will be turned into array.
 
     Examples
     --------
@@ -125,7 +118,92 @@
     True
 
     """
     if isinstance(x, Iterable) and not isinstance(x, (six.string_types, pd.DataFrame)):
         return True
     else:
         return False
+
+
+def is_hashable(x) -> bool:
+    """Check if object is hashable."""
+    try:
+        hash(x)
+        return True
+    except TypeError:
+        return False
+
+
+def is_mesh_like(x):
+    """Check if object is mesh (i.e. contains vertices and faces)."""
+    if hasattr(x, 'vertices') and hasattr(x, 'faces'):
+        return True
+
+    return False
+
+
+def is_points(x):
+    """Check if object could be points (i.e. contains 3D coordinates)."""
+    if isinstance(x, np.ndarray) and x.ndim == 2 and x.shape[1] == 3:
+        return True
+
+    return False
+
+
+def is_lines(x):
+    """Check if object could be lines (i.e. contains 3D coordinates)."""
+    if isinstance(x, np.ndarray) and x.ndim == 2 and x.shape[1] == 3:
+        return True
+
+    return False
+
+
+def is_volume(x):
+    """Check if object could be a volume (i.e. 3D array)."""
+    if isinstance(x, np.ndarray) and x.ndim == 3:
+        return True
+
+    return False
+
+
+def is_pygfx_visual(x):
+    """Check if object is a pygfx visual."""
+    if isinstance(x, gfx.WorldObject):
+        return True
+    return False
+
+
+def is_pygfx_geometry(x):
+    """Check if object is a pygfx geometry."""
+    if isinstance(x, gfx.Geometry):
+        return True
+    return False
+
+
+def _type_of_script() -> str:
+    """Return context (terminal, jupyter, colab, iPython) in which navis is run."""
+    try:
+        ipy_str = str(type(get_ipython()))  # noqa: F821
+        if 'zmqshell' in ipy_str:
+            return 'jupyter'
+        elif 'colab' in ipy_str:
+            return 'colab'
+        else:  # if 'terminal' in ipy_str:
+            return 'ipython'
+    except BaseException:
+        return 'terminal'
+
+
+def is_jupyter() -> bool:
+    """Test if navis is run in a Jupyter notebook.
+
+    Also returns True if inside Google colaboratory!
+
+    Examples
+    --------
+    >>> from navis.utils import is_jupyter
+    >>> # If run outside a Jupyter environment
+    >>> is_jupyter()
+    False
+
+    """
+    return _type_of_script() in ('jupyter', 'colab')
```

### Comparing `octarine3d-0.1.0/octarine/viewer.py` & `octarine3d-0.1.1/octarine/viewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import png
 import cmap
 import uuid
+import wgpu
 import random
+import inspect
 
 import numpy as np
 import pygfx as gfx
 
+from functools import wraps
 from collections import OrderedDict
 
 from wgpu.gui.auto import WgpuCanvas
 from wgpu.gui.offscreen import WgpuCanvas as WgpuCanvasOffscreen
 
 from .visuals import mesh2gfx, volume2gfx, points2gfx, lines2gfx
+from .conversion import get_converter
 from . import utils, config
 
 
-
 __all__ = ['Viewer']
 
 logger = config.get_logger(__name__)
 
 # TODO
 # - add styles for viewer (lights, background, etc.) - e.g. .set_style(dark)
 #   - e.g. material.metalness = 2 looks good for background meshes
 #   - metalness = 1 with roughness = 0 makes for funky looking neurons
 #   - m.material.side = "FRONT" makes volumes look better
 # - make Viewer reactive (see reactive_rendering.py) to save
 #   resources when not actively using the viewer - might help in Jupyter?
 # [/] add specialised methods for adding neurons, volumes, etc. to the viewer
+# - move lights to just outside the scene's bounding box (maybe use decorator?)
+#   whenever we add/remove objects
 
 
 def update_legend(func):
     """Decorator to update legend after function call."""
+    @wraps(func)
     def wrapper(*args, **kwargs):
         func(*args, **kwargs)
         if args[0].controls:
             args[0].controls.update_legend()
     return wrapper
 
 
@@ -49,63 +55,73 @@
                 want a screenshot.
     title :     str, optional
                 Title of the viewer window.
     max_fps :   int, optional
                 Maximum frames per second to render.
     size :      tuple, optional
                 Size of the viewer window.
+    show :      bool, optional
+                Whether to immediately show the viewer.
     show_controls : bool, optional
                 If True, will show the controls widget.
                 You can always show/hide the controls with
                 ``viewer.show_controls()`` and ``viewer.hide_controls()``.
-
     **kwargs
-                Keyword arguments passed to ``WgpuCanvas``.
+                Keyword arguments are passed through to ``WgpuCanvas``.
 
     """
+    # Palette used for assigning colors to objects
     palette='seaborn:tab10'
 
     def __init__(self,
-                offscreen=False,
-                title='Octarine Viewer',
-                max_fps=30,
-                size=None,
-                show_controls=False,
-                **kwargs):
+                 offscreen=False,
+                 title='Octarine Viewer',
+                 max_fps=30,
+                 size=None,
+                 show=True,
+                 show_controls=False,
+                 **kwargs):
         # Check if we're running in an IPython environment
-        try:
-            ip = get_ipython()
+        if utils._type_of_script() == 'ipython':
+            ip = get_ipython()  # noqa: F821
             if not ip.active_eventloop:
                 # ip.enable_gui('qt6')
                 raise ValueError('IPython event loop not running. Please use e.g. "%gui qt" to hook into the event loop.')
-        except NameError:
-            ip = None
+
+        self._title = title
 
         # Update some defaults as necessary
         defaults = {'title': title, 'max_fps': max_fps, 'size': size}
         defaults.update(kwargs)
 
         # If we're running in headless mode (primarily for tests on CI) we will
         # simply not initialize the gfx objects. Not ideal but it turns
         # out to be very annoying to correctly setup on Github Actions.
         if getattr(config, 'HEADLESS', False):
             return
 
         if not offscreen:
-            self._offscreen = False
             self.canvas = WgpuCanvas(**defaults)
         else:
-            self._offscreen = True
             self.canvas = WgpuCanvasOffscreen(**defaults)
-        self.renderer = gfx.renderers.WgpuRenderer(self.canvas, show_fps=False)
+
+        # There is a bug in pygfx 0.1.18 that causes the renderer to crash
+        # when using a Jupyter canvas without explicitly setting the pixel_ratio.
+        # This is already fixed in main but for now:
+        if self._is_jupyter:
+            self.renderer = gfx.renderers.WgpuRenderer(self.canvas, show_fps=False, pixel_ratio=2)
+        else:
+            self.renderer = gfx.renderers.WgpuRenderer(self.canvas, show_fps=False)
 
         # Set up a default scene
         self.scene = gfx.Scene()
-        self.scene.add(gfx.AmbientLight())
-        self.scene.add(gfx.DirectionalLight())
+        self.scene.add(gfx.AmbientLight(intensity=0.5))
+        self.scene.add(gfx.PointLight(intensity=4))
+        # Adjust shadow bias (this helps with shadow acne)
+        self.scene.children[-1].shadow.bias = 0.0000005
 
         # Modify the light
         light = self.scene.children[-1]
         light.local.z = -10000  # move light forward
         light.local.euler_x = 2.5 # rotate light
 
         # Set up a default background
@@ -137,24 +153,37 @@
                 self.key_events[event.key]()
 
         # Register events
         self.renderer.add_event_handler(_keydown, "key_down")
 
         # Finally, setting some variables
         self._show_bounds = False
+        self._shadows = False
+        self._animations = []
 
         # This starts the animation loop
-        self.show()
+        if show:
+            self.show()
 
-        # Add controls
-        if show_controls:
-            self.show_controls()
+            # Add controls
+            if show_controls:
+                self.show_controls()
 
     def _animate(self):
         """Animate the scene."""
+        to_remove = []
+        for i, func in enumerate(self._animations):
+            try:
+                func()
+            except BaseException as e:
+                logger.error(f'Removing animation function {func} because of error: {e}')
+                to_remove.append(i)
+        for i in to_remove[::-1]:
+            self.remove_animation(i)
+
         if self._show_fps:
             with self.stats:
                 self.renderer.render(self.scene, self.camera, flush=False)
             self.stats.render()
         else:
             self.renderer.render(self.scene, self.camera)
         self.canvas.request_draw()
@@ -252,14 +281,53 @@
         # Update data text
         # Currently only the development version of vispy supports escape
         # character (e.g. \n)
         t = '| '.join([f'{objects[s][0]._name} - #{s}' for s in self.__selected])
         self._data_text.text = t
 
     @property
+    def size(self):
+        """Return size of the canvas."""
+        return self.canvas.get_logical_size()
+
+    @size.setter
+    def size(self, size):
+        """Set size of the canvas."""
+        assert len(size) == 2
+        self.canvas.set_logical_size(*size)
+
+    @property
+    def shadows(self):
+        """Return shadow state."""
+        return self._shadows
+
+    @shadows.setter
+    def shadows(self, v):
+        """Set shadow state."""
+        if not isinstance(v, bool):
+            raise TypeError(f'Expected bool, got {type(v)}')
+
+        def set_shadow(obj, state):
+            if hasattr(obj, 'cast_shadow'):
+                obj.cast_shadow = state
+            if hasattr(obj, 'receive_shadow'):
+                obj.receive_shadow = state
+
+        if v != self._shadows:
+            self._shadows = v
+            for vis in self.visuals:
+                set_shadow(vis, v)
+
+            for ch in self.scene.children:
+                if isinstance(ch, gfx.PointLight):
+                    ch.cast_shadow = v
+
+            #self.scene.traverse(lambda x: set_shadow(x, v))
+
+    @property
     def visuals(self):
         """List of all visuals on this canvas."""
         return [c for c in self.scene.children if hasattr(c, '_object_id')]
 
     @property
     def bounds(self):
         """Bounds of all currently visuals (visible and invisible)."""
@@ -281,14 +349,34 @@
 
         mn = bounds[:, 0, :].min(axis=1)
         mx = bounds[:, 1, :].max(axis=1)
 
         return np.vstack((mn, mx)).T
 
     @property
+    def max_fps(self):
+        """Maximum frames per second to render."""
+        return self.canvas._subwidget._max_fps
+
+    @max_fps.setter
+    def max_fps(self, v):
+        assert isinstance(v, int)
+        self.canvas._subwidget._max_fps = v
+
+    @property
+    def _is_jupyter(self):
+        """Check if Viewer is using Jupyter canvas."""
+        return "JupyterWgpuCanvas" in str(type(self.canvas))
+
+    @property
+    def _is_offscreen(self):
+        """Check if Viewer is using offscreen canvas."""
+        return isinstance(self.canvas, WgpuCanvasOffscreen)
+
+    @property
     def _object_ids(self):
         """All object IDs on this canvas in order of addition."""
         obj_ids = []
         for v in self.visuals:
             if hasattr(v, '_object_id'):
                 obj_ids.append(v._object_id)
         return sorted(set(obj_ids), key=lambda x: obj_ids.index(x))
@@ -298,26 +386,84 @@
         """Ordered dictionary {name->[visuals]} of all objects in order of addition."""
         objects = OrderedDict()
         for ob in self._object_ids:
             objects[ob] = [v for v in self.visuals if getattr(v, '_object_id', None) == ob]
 
         return objects
 
-    def show(self):
-        """Show viewer."""
+    def add_animation(self, x):
+        """Add animation function to the Viewer.
+
+        Parameters
+        ----------
+        x :     callable
+                Function to add to the animation loop.
+
+        """
+        if not callable(x):
+            raise TypeError(f'Expected callable, got {type(x)}')
+
+        self._animations.append(x)
+
+    def remove_animation(self, x):
+        """Remove animation function from the Viewer.
+
+        Parameters
+        ----------
+        x :     callable | int
+                Either the function itself or its index
+                in the list of animations.
+
+        """
+        if callable(x):
+            self._animations.remove(x)
+        elif isinstance(x, int):
+            self._animations.pop(x)
+        else:
+            raise TypeError(f'Expected callable or index (int), got {type(x)}')
+
+    def show(self, use_sidecar=False):
+        """Show viewer.
+
+        Parameters
+        ----------
+        use_sidecar : bool
+                      For Jupyter lab only: if True, will use the Sidecar
+                      extension to display the viewer outside the notebooks.
+                      Will throw an error if Sidecar is not installed.
+
+        """
         # This is for e.g. headless testing
         if getattr(config, 'HEADLESS', False):
             logger.info("Viewer widget not shown - running in headless mode.")
             return
 
-        self.canvas.show()
+        # Start the animation loop
         self.canvas.request_draw(self._animate)
 
+        # If this is an offscreen canvas, we don't need to show anything
+        if isinstance(self.canvas, WgpuCanvasOffscreen):
+            return
+        # In terminal we can just show the window
+        elif not self._is_jupyter:
+            self.canvas.show()
+        # For Jupyter we need to wrap the canvas in a widget
+        else:
+            if not hasattr(self, 'widget'):
+                from .jupyter import JupyterOutput
+                # Construct the widget
+                self.widget = JupyterOutput(self, use_sidecar=use_sidecar, sidecar_kwargs={'title': self._title})
+            return self.widget
+
     def show_controls(self):
         """Show controls."""
+        if self._is_jupyter:
+            logger.warning('Controls are not (yet) supported in Jupyter.')
+            return
+
         if not hasattr(self, '_controls'):
             from .controls import Controls
             self._controls = Controls(self)
         self._controls.show()
 
     def hide_controls(self):
         """Hide controls."""
@@ -341,36 +487,33 @@
         if getattr(config, 'HEADLESS', False):
             return
 
         # Remove everything but the lights and backgrounds
         self.scene.remove(*self.visuals)
 
     @update_legend
-    def remove(self, to_remove):
+    def remove_objects(self, to_remove):
         """Remove given neurons/visuals from canvas."""
         to_remove = utils.make_iterable(to_remove)
 
-        neurons = self.objects  # grab this only once to speed things up
-        for vis in to_remove:
-            if vis in self.scene.children:
+        for vis in self.scene.children:
+            if vis in to_remove:
                 self.scene.children.remove(vis)
-            else:
-                uuids = utils.eval_id(to_remove)
-                for u in uuids:
-                    for v in neurons.get(u, []):
-                        self.scene.children.remove(v)
+            elif hasattr(vis, '_object_id'):
+                if vis._object_id in to_remove:
+                    self.scene.children.remove(vis)
 
         if self.show_bounds:
             self.update_bounds()
 
     @update_legend
     def pop(self, N=1):
         """Remove the most recently added N visuals."""
         for vis in list(self.objects.values())[-N:]:
-            self.remove(vis)
+            self.remove_objects(vis)
 
     @property
     def show_bounds(self):
         """Set to ``True`` to show bounding box."""
         return self._show_bounds
 
     def toggle_bounds(self):
@@ -390,18 +533,24 @@
             self.remove_bounds()
 
     def remove_bounds(self):
         """Remove bounding box visual."""
         self._show_bounds = False
         for v in self.visuals:
             if getattr(v, '_object_type', '') == 'boundingbox':
-                self.remove(v)
+                self.remove_objects(v)
 
     def resize(self, size):
-        """Resize canvas."""
+        """Resize canvas.
+
+        Parameters
+        ----------
+        size :  (width, height) tuple
+                New size of the canvas.
+        """
         assert len(size) == 2
         self.canvas.set_logical_size(*size)
 
     def update_bounds(self, color='w', width=1):
         """Update bounding box visual."""
         # Remove any existing visual
         self.remove_bounds()
@@ -422,133 +571,161 @@
         box._object_id = uuid.uuid4()
 
         self.scene.add(box)
 
     def center_camera(self):
         """Center camera on visuals."""
         if len(self):
-            self.camera.show_object(self.scene, scale=1.1, view_dir=(0., 0., 1.), up=(0., -1., 0.))
+            self.camera.show_object(
+                self.scene,
+                scale=1,
+                view_dir=(0., 0., 1.),
+                up=(0., -1., 0.)
+                )
 
     @update_legend
-    def add(self, x, center=True, clear=False, **kwargs):
-        """Add objects to canvas.
+    def add(self, x, name=None, center=True, clear=False, **kwargs):
+        """Add object to canvas.
+
+        This function is a general entry point for adding objects to the canvas.
+        It will look at the type of the input and try to find an appropriate
+        function to convert the input to visuals.
 
-        This is just a shorthand for the respective methods (e.g. `Viewer.add_mesh`).
+        Use `octarine.register_converter` to add custom converters.
 
         Parameters
         ----------
-        x :         Mesh-like | Volume | Points | gfx Visuals
+        x
                     Object(s) to add to the canvas.
+        name :      str, optional
+                    Name for the visual(s).
         center :    bool, optional
                     If True, re-center camera to all objects on canvas.
         clear :     bool, optional
                     If True, clear canvas before adding new objects.
         **kwargs
-                    Keyword arguments passed when generating visuals. See
-                    the respective methods (e.g. `Viewer.add_mesh`) for details.
+                    Keyword arguments passed to the conversion functions when
+                    generating visuals.
 
         Returns
         -------
         None
 
         """
-        (meshes, volumes, points, visuals) = utils.parse_objects(x)
-
-        if len(set(kwargs) & set(['c', 'color', 'colors'])) > 1:
-            raise ValueError('Must not provide colors via multiple arguments')
+        if clear:
+            self.clear()
 
-        # If we're runningg in headless mode (primarily for tests on CI) we will
-        # simply not add the objects. Not ideal but it turns out to be very
-        # annoying to correctly setup on Github Actions.
-        if getattr(config, 'HEADLESS', False):
+        if utils.is_iterable(x) and not isinstance(x, np.ndarray):
+            for xx in x:
+                self.add(xx, center=False, clear=False, name=name, **kwargs)
+            if center:
+                self.center_camera()
             return
 
-        if clear:
-            self.clear()
+        converter = get_converter(x, raise_missing=False)
+        if converter is None:
+            raise NotImplementedError(f'No converter found for {x} ({type(x)})')
+
+        # Check if we have to provide a color
+        if 'color' not in kwargs and 'color' in inspect.signature(converter).parameters:
+            kwargs['color'] = tuple(self._next_color().rgba)
+
+        visuals = utils.make_iterable(converter(x, **kwargs))
 
-        for m in meshes:
-            self.add_mesh(m, **kwargs)
-        for v in volumes:
-            self.add_volume(v, **kwargs)
-        for p in points:
-            self.add_scatter(p, **kwargs)
         for v in visuals:
-            # Check if the visual is actually just the geometry
-            if isinstance(v, gfx.Geometry):
-                v = gfx.Mesh(
-                    v,
-                    gfx.MeshPhongMaterial()
-                )
+            # If we have a name, assign it to the visual
+            if name is not None:
+                v._object_id = name
+            # If not we either use existing ID or generate a new one
+            else:
+                # Give visuals an _object_id if they don't already have one
+                if not hasattr(v, '_object_id'):
+                    new_id = self._next_label('Object')
+                    for v2 in visuals:
+                        v._object_id = new_id
+                elif not isinstance(v._object_id, str):
+                    v._object_id = str(v._object_id)
 
-            # Give visuals an _object_id if they don't already have one
-            if not hasattr(v, '_object_id'):
-                v._object_id = self._next_label('Mesh')
             self.scene.add(v)
 
         if center:
             self.center_camera()
 
     @update_legend
-    def add_mesh(self, mesh, name=None, color=None):
+    def add_mesh(self, mesh, name=None, color=None, center=True):
         """Add mesh to canvas.
 
         Parameters
         ----------
-        mesh :          Mesh-like
-                        Mesh to plot.
-        name :          str, optional
-                        Name for the visual.
-        color :         str | tuple, optional
-                        Color to use for plotting. Can be the name of
-                        a colormap or a single color.
+        mesh :      Mesh-like
+                    Mesh to plot.
+        name :      str, optional
+                    Name for the visual.
+        color :     str | tuple, optional
+                    Color to use for plotting. Can be the name of
+                    a colormap or a single color.
+        center :    bool, optional
+                    If True, re-center camera to all objects on canvas.
 
         """
         if not utils.is_mesh_like(mesh):
             raise TypeError(f'Expected mesh-like object, got {type(mesh)}')
         if color is None:
             color = self._next_color()
         if name is None:
             name = self._next_label('Mesh')
+        elif not isinstance(name, str):
+            name = str(name)
 
         visual = mesh2gfx(mesh, color=color)
         visual._object_id = name if name else uuid.uuid4()
         self.scene.add(visual)
 
+        if center:
+            self.center_camera()
+
     @update_legend
-    def add_scatter(self, points, name=None, color=None, size=2):
-        """Add scatter plot to canvas.
+    def add_points(self, points, name=None, color=None, size=2, center=True):
+        """Add points plot to canvas.
 
         Parameters
         ----------
-        points :        (N, 3) array
-                        Points to plot.
-        name :          str, optional
-                        Name for the visual.
-        color :         str | tuple, optional
-                        Color to use for plotting. Can be the name of
-                        a colormap or a single color.
-        size :          int | float
-                        Marker size.
+        points :    (N, 3) array
+                    Points to plot.
+        name :      str, optional
+                    Name for the visual.
+        color :     str | tuple, optional
+                    Color to use for plotting. Can be the name of
+                    a colormap or a single color.
+        size :      int | float
+                    Marker size.
+        center :    bool, optional
+                    If True, re-center camera to all objects on canvas.
 
         """
         if not isinstance(points, np.ndarray):
             raise TypeError(f'Expected numpy array, got {type(points)}')
         if points.ndim != 2 or points.shape[1] != 3:
             raise ValueError(f'Expected (N, 3) array, got {points.shape}')
         if color is None:
             color = self._next_color()
         if name is None:
             name = self._next_label('Scatter')
+        elif not isinstance(name, str):
+            name = str(name)
 
         visual = points2gfx(points, color=color, size=size)
         visual._object_id = name if name else uuid.uuid4()
         self.scene.add(visual)
 
+        if center:
+            self.center_camera()
+
     @update_legend
-    def add_lines(self, lines, name=None, color=None, linewidth=1):
+    def add_lines(self, lines, name=None, color=None, linewidth=1, center=True):
         """Add lines to canvas.
 
         Parameters
         ----------
         lines :     list of (N, 3) arrays | (N, 3) array
                     Lines to plot. If a list of arrays, each array
                     represents a separate line. If a single array,
@@ -557,66 +734,87 @@
         name :      str, optional
                     Name for the visual.
         color :     str | tuple, optional
                     Color to use for plotting. Can be a single color
                     or one for every point in the line(s).
         linewidth : float, optional
                     Line width.
+        center :    bool, optional
+                    If True, re-center camera to all objects on canvas.
 
         """
+        # TODO:
+        # - allow providing a tuple of (positions, edges) for lines
+
         if isinstance(lines, np.ndarray):
             if lines.ndim != 2 or lines.shape[1] != 3:
                 raise ValueError(f'Expected (N, 3) array, got {lines.shape}')
         elif isinstance(lines, list):
             if not all([l.ndim == 2 and l.shape[1] == 3 for l in lines]):
                 raise ValueError('Expected list of (N, 3) arrays.')
         else:
             raise TypeError(f'Expected numpy array or list, got {type(lines)}')
 
         if color is None:
             color = self._next_color()
         if name is None:
             name = self._next_label('Lines')
+        elif not isinstance(name, str):
+            name = str(name)
 
         visual = lines2gfx(lines, linewidth=linewidth, color=color)
         visual._object_id = name if name else uuid.uuid4()
         self.scene.add(visual)
 
+        if center:
+            self.center_camera()
+
     @update_legend
-    def add_volume(self, volume, dims, name=None, color=None, offset=(0, 0, 0)):
+    def add_volume(self, volume, dims, name=None, color=None, offset=(0, 0, 0), cmin=None, cmax='auto', center=True):
         """Add image volume to canvas.
 
         Parameters
         ----------
-        volume :        (N, M, K) array
-                        Volume to plot.
-        dims :          tuple
-                        Scale factors for the volume.
-        name :          str, optional
-                        Name for the visual.
-        color :         tuple, optional
-                        Color to use for plotting. Can be the name of
-                        a colormap or a single color.
-        offset :        tuple, optional
-                        Offset for the volume.
+        volume :    (N, M, K) array
+                    Volume to plot.
+        dims :      tuple
+                    Scale factors for the volume.
+        name :      str, optional
+                    Name for the visual.
+        color :     tuple, optional
+                    Color to use for plotting. Can be the name of
+                    a colormap or a single color.
+        offset :    tuple, optional
+                    Offset for the volume.
+        cmin/cmax : float | "auto", optional
+                    Min/max values for the colormap. If "auto", will
+                    use the min/max of the volume. If `None` will determine
+                    the min/max based on the data type of `volume`.
+        center :    bool, optional
+                    If True, re-center camera to all objects on canvas.
 
         """
         if not isinstance(volume, np.ndarray):
             raise TypeError(f'Expected numpy array, got {type(volume)}')
         if volume.ndim != 3:
             raise ValueError(f'Expected 3D array, got {volume.ndim}')
         if color is None:
             color = self._next_color()
         if name is None:
             name = self._next_label('Volume')
+        elif not isinstance(name, str):
+            name = str(name)
 
-        visual = volume2gfx(volume, dims=dims, offset=offset, color=color)
+        visual = volume2gfx(volume, dims=dims, offset=offset, color=color, cmin=cmin, cmax=cmax)
         visual._object_id = name if name else uuid.uuid4()
         self.scene.add(visual)
 
+        if center:
+            self.center_camera()
+
     def close(self):
         """Close the viewer."""
         # Skip if this is headless mode
         if getattr(config, 'HEADLESS', False):
             return
 
         # Clear first to free all visuals
@@ -629,27 +827,31 @@
         # Close if not already closed
         if not self.canvas.is_closed():
             self.canvas.close()
 
         if hasattr(self, '_controls'):
             self._controls.close()
 
-    def hide_object(self, obj):
+        # Close the Jupyter widget
+        if hasattr(self, 'widget') and not getattr(self.widget, '_is_closed', False):
+            self.widget.close(close_viewer=False)
+
+    def hide_objects(self, obj):
         """Hide given object(s).
 
         Parameters
         ----------
         obj :   str | list
                 Object(s) to hide.
 
         """
         objects = self.objects   # grab once to speed things up
         for ob in utils.make_iterable(obj):
             if ob not in objects:
-                logger.warning(f'Object {ob} not found on canvas.')
+                logger.warning(f'Object "{ob}" not found on canvas.')
                 continue
             for v in objects[ob]:
                 if getattr(v, '_pinned', False):
                     continue
                 if v.visible:
                     v.visible = False
 
@@ -664,15 +866,15 @@
         ----------
         obj :   str | list | None
                 Object(s) to unhide. If None, will unhide all objects.
 
         """
         objects = self.objects  # grab once to speed things up
         if obj is not None:
-            obj = utils.make_iterable(obj)
+            ids = utils.make_iterable(obj)
         else:
             ids = list(objects.keys())
 
         for ob in ids:
             if ob not in objects:
                 logger.warning(f'Object {ob} not found on canvas.')
                 continue
@@ -784,72 +986,88 @@
             colors = list(palette.iter_colors(len(objects)))
 
         colormap = {s: tuple(colors[i].rgba) for i, s in enumerate(objects)}
 
         self.set_colors(colormap)
 
     def set_bgcolor(self, c):
-        """Set background color."""
-        if getattr(config, 'HEADLESS', False):
-            return
+        """Set background color.
+
+        Parameters
+        ----------
+        c :     tuple | str
+                RGB(A) color to use for the background.
+
+        """
         self._background.set_colors(gfx.Color(c).rgba)
 
     def _toggle_fps(self):
         """Switch FPS measurement on and off."""
         self._show_fps = not self._show_fps
 
     def screenshot(self,
                    filename='screenshot.png',
-                   pixel_scale=2,
                    size=None,
+                   pixel_ratio=None,
                    alpha=True):
         """Save a screenshot of the canvas.
 
         Parameters
         ----------
         filename :      str, optional
                         Filename to save to. If ``None``, will return image array.
                         Note that this will always save a PNG file, no matter
                         the extension.
-        pixel_scale :   int, optional
-                        Factor by which to scale canvas. Determines image
-                        dimensions.
         size :          tuple, optional
                         Size of the screenshot. If provided, will temporarily
                         change the canvas size.
+        pixel_ratio :   int, optional
+                        Factor by which to scale canvas. Determines image
+                        dimensions. Note that this seems to have no effect
+                        on offscreen canvases.
         alpha :         bool, optional
                         If True, will export transparent background.
 
         """
-        im = self._screenshot(alpha=alpha, size=size)
+        im = self._screenshot(alpha=alpha, size=size, pixel_ratio=pixel_ratio)
         if filename:
             if not filename.endswith('.png'):
                 filename += '.png'
             png.from_array(im.reshape(im.shape[0], im.shape[1] * im.shape[2]), mode='RGBA').save(filename)
         else:
             return im
 
-    def _screenshot(self, alpha=True, size=None):
+    def _screenshot(self, alpha=True, size=None, pixel_ratio=None):
         """Return image array for screenshot."""
         if alpha:
             op = self._background.opacity
             self._background.opacity = 0
         if size:
-            os = (self.canvas.width(), self.canvas.height())
-            self.canvas.set_logical_size(*size)
+            os = self.size
+            self.size = size
+        if pixel_ratio:
+            opr = self.renderer.pixel_ratio
+            self.renderer.pixel_ratio = pixel_ratio
+
+        # If this is an offscreen canvas, we need to manually trigger a draw first
+        # Note: this has to happen _after_ adjust parameters!
+        if isinstance(self.canvas, WgpuCanvasOffscreen):
+            self.canvas.draw()
 
         try:
             im = self.renderer.snapshot()
         except BaseException:
             raise
         finally:
             if alpha:
                 self._background.opacity = op
             if size:
-                self.canvas.set_logical_size(*os)
+                self.size = os
+            if pixel_ratio:
+                self.renderer.pixel_ratio = opr
 
         return im
 
     def set_view(self, view):
         """(Re-)set camera position.
 
         Parameters
```

### Comparing `octarine3d-0.1.0/octarine3d.egg-info/PKG-INFO` & `octarine3d-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,98 @@
 Metadata-Version: 2.1
 Name: octarine3d
-Version: 0.1.0
+Version: 0.1.1
 Summary: WGPU-based 3d viewer
 Home-page: https://github.com/schlegelp/octarine
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: BSD-2-Clause
+Project-URL: Documentation, https://schlegelp.github.io/octarine/
 Project-URL: Source, https://github.com/schlegelp/octarine
 Project-URL: Changelog, https://github.com/schlegelp/octarine/releases
 Keywords: 3D viewer WGPU pygfx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygfx
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pypng
 Requires-Dist: six
 Requires-Dist: cmap
+Provides-Extra: all
+Requires-Dist: jupyter_rfb; extra == "all"
+Requires-Dist: PySide6; extra == "all"
+Requires-Dist: ipywidgets; extra == "all"
+Requires-Dist: sidecar; extra == "all"
+Provides-Extra: docs
+Requires-Dist: mkdocs; extra == "docs"
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: mkdocstrings-python; extra == "docs"
+Requires-Dist: mkdocs-minify-plugin; extra == "docs"
+Requires-Dist: mkdocs-literate-nav; extra == "docs"
+Requires-Dist: mkdocs-gen-files; extra == "docs"
 
-![cocoa](docs/_static/octarine_logo_banner.png)
+![octarine banner](https://schlegelp.github.io/octarine/_static/octarine_logo_banner.png)
 <p align="center">
 <i>
 Octarine is the eighth color of the Discworld's spectrum, which is described as the color of magic itself. Only wizards and cats can see it.
 </i>
 </p>
 
+[![docs](https://github.com/schlegelp/octarine/actions/workflows/docs.yml/badge.svg)](https://schlegelp.github.io/octarine/)
+
 # Octarine
-A high-performance, easy-to-use 3D viewer. `Octarine` is build on top of the excellent
+A minimalist, easy-to-use, high-performance 3D viewer. `Octarine` is build on top of the excellent
 [`pygfx`](https://github.com/pygfx/pygfx) WGPU rendering engine which does most of the heavy lifting - we're simply
 abstracting away some of the boiler plate code for you.
 
 ## Rationale :thought_balloon:
 Why another 3d viewer? There are plenty options out there:
-[`vedo`](https://github.com/marcomusy/vedo), [`ipygany`](https://github.com/jupyter-widgets-contrib/ipygany), [`polyscope`](https://github.com/nmwsharp/polyscope), [`napari`](https://github.com/napari/napari), [`fury`](https://github.com/fury-gl/fury) or [`pyvista`](https://github.com/pyvista/pyvista) to name but a few. All of these are great in their own right but I wanted something (a) without heavy dependencies (i.e. no VTK), (b) that lets me interactively explore my data in both REPL and Jupyter and (c) is very performant. None of the above ticked all those boxes for me.
+[`vedo`](https://github.com/marcomusy/vedo), [`ipygany`](https://github.com/jupyter-widgets-contrib/ipygany), [`polyscope`](https://github.com/nmwsharp/polyscope), [`napari`](https://github.com/napari/napari), [`fury`](https://github.com/fury-gl/fury), [`plotly`](https://github.com/plotly/plotly.py) or [`pyvista`](https://github.com/pyvista/pyvista) to name but a few. All of these are great in their own right but I wanted something *(a)* without heavy dependencies (i.e. no VTK), *(b)* that lets me interactively explore my data in both REPL and Jupyter and *(c)* is very performant. None of the existing solutions ticked all those boxes for me.
 
 `Octarine` tries to fill that gap:
 1. _Lightweight_ with very few direct or indirect dependencies.
 2. Works in both _Jupyter_ and _REPL_.
-3. _High performance_: a mesh with 15M faces renders with 80 fps at 1080p (2023 MacBook Pro).
+3. _High performance_: a mesh with 15M faces renders with 80 fps at 1080p on a 2023 MacBook Pro.
 
 ## ToDo :ballot_box_with_check:
 This is still a prototype but basic stuff already works (mostly because `pygfx` makes it so ridiculously easy).
 
 - [x] basic datatypes: meshes, points, scatter, volumes
 - [x] custom keyboard shortcuts
 - [x] rudamentary controls + legend
-- [ ] user-defined animations
-- [ ] proper docs
+- [x] screenshots
+- [x] support for trimesh scenes
+- [x] user-defined animations
+- [x] documentation
+- [ ] methods/controls to manipulate image volumes
 - [ ] tests
 
 ## Installation :rocket:
 
 ```bash
 pip install octarine3d
 ```
 
-In addition you will need to install at least one window manager supported by [wgpu-py](https://github.com/pygfx/wgpu-py):
+In addition you will need to install at least one window manager supported by [`wgpu-py`](https://github.com/pygfx/wgpu-py):
 - qt: PySide6, PyQt6, PySide2, PyQt5 all work but I recommend PySide6 (see below)
 - glfw: a lightweight GUI for the desktop
 - jupyter_rfb: only needed if you plan on using `Octarine` in Jupyter
 - wx
 
-Please note that at this point, `Octarine`'s controls panel requires `PySide6`. So if you need GUI controls you have to use `PySide6`.
+Please note that at this point, `Octarine`'s controls panel requires `PySide6`. So if you want GUI controls you have to use `PySide6`.
 
 ## Quickstart :fire:
 
 ```python
 # Create a Viewer instance
 from octarine import Viewer
 v = Viewer()
@@ -92,37 +111,64 @@
 m = gfx.geometries.mobius_strip_geometry()
 v.add(m, color='b')
 
 # Close the viewer
 v.close()
 ```
 
+![demo gif](docs/_static/octarine_demo_720p.gif)
+
 Other selected `Viewer` methods:
 - `add()`: generic method to add stuff to the viewer; will call respective specialised methods
 - `add_lines()`: add line plot
 - `add_mesh()`: add meshes (anything that has `.vertices` and `.faces` goes)
-- `add_scatter()`: add a scatter plot
+- `add_points()`: add a scatter plot
 - `add_volume()`: add an image volume
 - `center_camera()`: center camera on scene
 - `clear()`: clear scene
 - `close()`: close viewer
 - `colorize()`: cycle colors for all objects
 - `pop()`: remove last added object
-- `remove()`: remove a given object(s) from the scene
+- `remove_objects()`: remove a given object(s) from the scene
 - `screenshot()`: take (and save) a screenshot
 - `set_bgcolor()`: set background color
 - `set_colors()`: set object colors
 
 ### Hotkeys
 The following keyboard shortcuts are hard-coded:
 - `1`: reset view to XY (frontal)
 - `2`: reset view to XZ (dorsal)
 - `3`: reset view to YZ (lateral)
 - `f`: show FPS
-- `c`: show control panel
+- `c`: show control panel (requires `PySide6`)
 
 You can also bind custom functions to keys:
 
 ```python
 # Bind `x` key to the cycle-colors method
 v.key_events['x'] = lambda : v.colorize()
 ```
+
+## Want to contribute?
+We welcome all kinds of contributions. For example:
+
+- reports of bugs, broken examples, etc.
+- feature requests
+- pull requests with bug fixes or new features
+
+If you already know what needs doing, feel free to open a pull request
+right away. When in doubt please open an [issue](https://github.com/schlegelp/octarine/issues)
+so we can discuss the best way to address the issue.
+
+## Development :dash:
+
+### Tests
+TODO
+
+### Docs
+
+To generate the documentation:
+
+```bash
+pip install -e .[docs]
+mkdocs build
+```
```

### Comparing `octarine3d-0.1.0/setup.py` & `octarine3d-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-from setuptools import setup, find_packages
 import re
 
+from setuptools import setup, find_packages
+from extreqs import parse_requirement_files
+from pathlib import Path
 
 VERSIONFILE = "octarine/__version__.py"
 verstrline = open(VERSIONFILE, "rt").read()
 VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     verstr = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
-    requirements = [l for l in requirements if not l.startswith('#')]
+HERE = Path(__file__).resolve().parent
+install_requires, extras_require = parse_requirement_files(
+    HERE / "requirements.txt",
+)
+
 
 setup(
     name='octarine3d',
     version=verstr,
     packages=find_packages(),
     license='BSD-2-Clause',
     description='WGPU-based 3d viewer',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/schlegelp/octarine',
     project_urls={
-     #"Documentation": "https://octarine.readthedocs.io",
+     "Documentation": "https://schlegelp.github.io/octarine/",
      "Source": "https://github.com/schlegelp/octarine",
      "Changelog": "https://github.com/schlegelp/octarine/releases",
     },
     author='Philipp Schlegel',
     author_email='pms70@cam.ac.uk',
     keywords='3D viewer WGPU pygfx',
     classifiers=[
@@ -38,14 +42,15 @@
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
 
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
-    install_requires=requirements,
-    extras_require={},
+    install_requires=install_requires,
+    extras_require=dict(extras_require),
     python_requires='>=3.8',
     zip_safe=False,
     include_package_data=True
 )
```

