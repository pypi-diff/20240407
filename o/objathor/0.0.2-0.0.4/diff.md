# Comparing `tmp/objathor-0.0.2.tar.gz` & `tmp/objathor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objathor-0.0.2.tar", last modified: Mon Mar 11 21:42:35 2024, max compression
+gzip compressed data, was "objathor-0.0.4.tar", last modified: Sat Apr  6 22:12:25 2024, max compression
```

## Comparing `objathor-0.0.2.tar` & `objathor-0.0.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.461088 objathor-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-11 21:42:23.000000 objathor-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-11 21:42:35.461088 objathor-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-11 21:42:23.000000 objathor-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.453088 objathor-0.0.2/objathor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.457088 objathor-0.0.2/objathor/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/annotation/annotation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/annotation/embed_synset_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/annotation/gpt_from_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/annotation/objaverse_annotations_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/annotation/synset_from_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.457088 objathor-0.0.2/objathor/asset_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/asset_conversion_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.457088 objathor-0.0.2/objathor/asset_conversion/colliders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/colliders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/colliders/decompose_convex_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/colliders/generate_colliders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/convert_obj_to_glb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.457088 objathor-0.0.2/objathor/asset_conversion/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/data/empty_house.json
--rw-r--r--   0 runner    (1001) docker     (127)    64921 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/object_consolidater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/object_consolidater_blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/object_consolidater_blender_package.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31364 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/pipeline_to_thor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/asset_conversion/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.461088 objathor-0.0.2/objathor/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/aggregate_asset_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/download_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/download_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/download_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/download_holodeck_base_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/generate_holodeck_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/postprocess_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/upgrade_2023_holodeck_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/dataset/upload_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.461088 objathor-0.0.2/objathor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.461088 objathor-0.0.2/objathor/utils/blender/
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/utils/blender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/utils/blender/render_glb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/utils/gpt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/utils/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-11 21:42:23.000000 objathor-0.0.2/objathor/utils/synsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:42:35.457088 objathor-0.0.2/objathor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-11 21:42:35.000000 objathor-0.0.2/objathor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-11 21:42:35.000000 objathor-0.0.2/objathor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 21:42:35.000000 objathor-0.0.2/objathor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-11 21:42:35.000000 objathor-0.0.2/objathor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 21:42:35.000000 objathor-0.0.2/objathor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 21:42:35.461088 objathor-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-03-11 21:42:23.000000 objathor-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.706651 objathor-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 22:12:16.000000 objathor-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-06 22:12:25.706651 objathor-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-06 22:12:16.000000 objathor-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.698651 objathor-0.0.4/objathor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/annotation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/embed_synset_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/gpt_from_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/objaverse_annotations_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/synset_from_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor/asset_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/asset_conversion_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor/asset_conversion/colliders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/colliders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/colliders/decompose_convex_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/colliders/generate_colliders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/convert_obj_to_glb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor/asset_conversion/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/data/empty_house.json
+-rw-r--r--   0 runner    (1001) docker     (127)    64921 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/object_consolidater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/object_consolidater_blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/object_consolidater_blender_package.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31364 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/pipeline_to_thor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.706651 objathor-0.0.4/objathor/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/aggregate_asset_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/download_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/download_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/download_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/download_holodeck_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/generate_holodeck_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/postprocess_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/upgrade_2023_holodeck_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.706651 objathor-0.0.4/objathor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.706651 objathor-0.0.4/objathor/utils/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/blender/render_glb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/gpt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/synsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 22:12:25.706651 objathor-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-06 22:12:16.000000 objathor-0.0.4/setup.py
```

### Comparing `objathor-0.0.2/LICENSE` & `objathor-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/PKG-INFO` & `objathor-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objathor
-Version: 0.0.2
+Version: 0.0.4
 Summary: Objaverse asset importer for THOR
 Home-page: https://github.com/allenai/objathor
 Author: Allen Institute for AI
 Author-email: contact@allenai.org
 License: Apache 2.0
 Keywords: 3D assets,annotation,
 Classifier: Development Status :: 4 - Beta
@@ -44,21 +44,21 @@
 
 We recommend setting an environment variable with your OpenAI key:
 
 ```bash
 export OPENAI_API_KEY=[Your key]
 ```
 
-If we're planning to annotate objects for which we don't have pre-generated
+If you're planning to annotate objects for which we don't have pre-generated
 views in S3 (see an example under [Annotation](#annotation) below), we also need to install blender either as an extra (as shown above) or as an application:
 
 ### Blender install instructions
 Installing  the `Blender` as a module:
 ```bash
-pip install -e bpy"
+pip install bpy
 ```
 Installing  the Blender as a module, requires a python `3.10` environment.
 
 Or installing blender as an application:
 [Blender install instructions](https://docs.blender.org/manual/en/latest/getting_started/installing/index.html)
 
 If application is not in the cannonical directories you may need to pass `blender_installation_path` to scripts that use Blender.
```

### Comparing `objathor-0.0.2/README.md` & `objathor-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 
 We recommend setting an environment variable with your OpenAI key:
 
 ```bash
 export OPENAI_API_KEY=[Your key]
 ```
 
-If we're planning to annotate objects for which we don't have pre-generated
+If you're planning to annotate objects for which we don't have pre-generated
 views in S3 (see an example under [Annotation](#annotation) below), we also need to install blender either as an extra (as shown above) or as an application:
 
 ### Blender install instructions
 Installing  the `Blender` as a module:
 ```bash
-pip install -e bpy"
+pip install bpy
 ```
 Installing  the Blender as a module, requires a python `3.10` environment.
 
 Or installing blender as an application:
 [Blender install instructions](https://docs.blender.org/manual/en/latest/getting_started/installing/index.html)
 
 If application is not in the cannonical directories you may need to pass `blender_installation_path` to scripts that use Blender.
```

### Comparing `objathor-0.0.2/objathor/annotation/annotation_utils.py` & `objathor-0.0.4/objathor/annotation/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/annotation/embed_synset_definitions.py` & `objathor-0.0.4/objathor/annotation/embed_synset_definitions.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/annotation/gpt_from_views.py` & `objathor-0.0.4/objathor/annotation/gpt_from_views.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/annotation/objaverse_annotations_utils.py` & `objathor-0.0.4/objathor/annotation/objaverse_annotations_utils.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/annotation/synset_from_description.py` & `objathor-0.0.4/objathor/annotation/synset_from_description.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import traceback
 from typing import Sequence, Optional, Dict, List, Tuple
 
 import compress_pickle
 import numpy as np
 
-from objathor.utils.synsets import import_install_nltk_commit
+from objathor.utils.synsets import _ensure_nltk
 
-# import nltk
-import_install_nltk_commit()
+_ensure_nltk()  # Running this by itself will not import anything, but will raise an error if nltk is not installed
+import nltk
 from nltk.corpus import wordnet2022 as wn
 from sklearn.neighbors import NearestNeighbors
 
 from objathor.annotation.embed_synset_definitions import (
     get_embeddings_single as get_synset_embeddings,
 )
 from objathor.utils.gpt_utils import get_embedding
```

### Comparing `objathor-0.0.2/objathor/asset_conversion/colliders/decompose_convex_obj.py` & `objathor-0.0.4/objathor/asset_conversion/colliders/decompose_convex_obj.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/asset_conversion/colliders/generate_colliders.py` & `objathor-0.0.4/objathor/asset_conversion/colliders/generate_colliders.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/asset_conversion/convert_obj_to_glb.py` & `objathor-0.0.4/objathor/asset_conversion/convert_obj_to_glb.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/asset_conversion/data/empty_house.json` & `objathor-0.0.4/objathor/asset_conversion/data/empty_house.json`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/asset_conversion/object_consolidater.py` & `objathor-0.0.4/objathor/asset_conversion/object_consolidater.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/asset_conversion/object_consolidater_blender.py` & `objathor-0.0.4/objathor/asset_conversion/object_consolidater_blender.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/asset_conversion/object_consolidater_blender_package.py` & `objathor-0.0.4/objathor/asset_conversion/object_consolidater_blender_package.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/asset_conversion/pipeline_to_thor.py` & `objathor-0.0.4/objathor/asset_conversion/pipeline_to_thor.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/asset_conversion/util.py` & `objathor-0.0.4/objathor/asset_conversion/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,14 +388,15 @@
     thor_controller,
     asset_id,
     asset_directory,
     copy_to_dir=None,
     verbose=False,
     load_file_in_unity=False,
     extension=None,
+    raise_for_failure=True,
 ):
     # Verifies the file exists
     create_prefab_action = {}
 
     asset_path = get_existing_thor_asset_file_path(
         out_dir=asset_directory, asset_id=asset_id, force_extension=extension
     )
@@ -426,21 +427,26 @@
     )
 
     if not load_file_in_unity:
         asset = change_asset_paths(asset=asset, save_dir=copy_to_dir)
         asset = add_default_annotations(
             asset=asset, asset_directory=asset_directory, verbose=verbose
         )
-        create_prefab_action = {"action": "CreateRuntimeAsset", "asset": asset}
+        create_prefab_action = {
+            "action": "CreateRuntimeAsset",
+            "asset": asset,
+            "raise_for_failure": raise_for_failure,
+        }
     else:
         create_prefab_action = {
             "action": "CreateRuntimeAsset",
             "id": asset_id,
             "dir": copy_to_dir,
             "extension": file_extension,
+            "raise_for_failure": raise_for_failure,
         }
         create_prefab_action = add_default_annotations(
             asset=create_prefab_action, asset_directory=asset_directory, verbose=verbose
         )
 
     evt = thor_controller.step(**create_prefab_action)
     logger.debug(f"Last Action: {thor_controller.last_action['action']}")
```

### Comparing `objathor-0.0.2/objathor/dataset/__init__.py` & `objathor-0.0.4/objathor/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/dataset/aggregate_asset_annotations.py` & `objathor-0.0.4/objathor/dataset/aggregate_asset_annotations.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/dataset/download_annotations.py` & `objathor-0.0.4/objathor/dataset/download_annotations.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/dataset/example.py` & `objathor-0.0.4/objathor/dataset/example.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/dataset/generate_holodeck_features.py` & `objathor-0.0.4/objathor/dataset/generate_holodeck_features.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/dataset/postprocess_assets.py` & `objathor-0.0.4/objathor/dataset/postprocess_assets.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/dataset/upgrade_2023_holodeck_databases.py` & `objathor-0.0.4/objathor/dataset/upgrade_2023_holodeck_databases.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/dataset/upload_dataset.py` & `objathor-0.0.4/objathor/dataset/upload_dataset.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/main.py` & `objathor-0.0.4/objathor/main.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/utils/blender/__init__.py` & `objathor-0.0.4/objathor/utils/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/utils/blender/render_glb.py` & `objathor-0.0.4/objathor/utils/blender/render_glb.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/utils/download_utils.py` & `objathor-0.0.4/objathor/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/utils/gpt_utils.py` & `objathor-0.0.4/objathor/utils/gpt_utils.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/utils/queries.py` & `objathor-0.0.4/objathor/utils/queries.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/objathor/utils/synsets.py` & `objathor-0.0.4/objathor/utils/synsets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,31 @@
-import os
-import subprocess
 from typing import List, Optional, Sequence
 
 
-def import_install_nltk_commit(
-    commit_id="582e6e35f0e6c984b44ec49dcb8846d9c011d0a8", install_if_import_fails=True
-):
+def _ensure_nltk():
     try:
         import nltk
-    except ImportError as e:
-        # print(f"Coululd not import `nltk` please install it by running `pip install git+https://github.com/nltk/nltk@{commit_id}`.")
+    except ImportError:
         raise ValueError(
-            f"\nCoululd not import `nltk` please install it by running `pip install git+https://github.com/nltk/nltk@{commit_id}`."
+            f"\nCould not import `nltk` please install it by running `pip install git+https://github.com/nltk/nltk@582e6e35f0e6c984b44ec49dcb8846d9c011d0a8`."
         )
-        # if install_if_import_fails:
 
-        # does not work when subprocess.
-        # errors: fatal: fetch-pack: invalid index-pack output; error: subprocess-exited-with-error
-        # command = (
-        #     f"pip"
-        #     f" install"
-        #     f" git+https://github.com/nltk/nltk@{commit_id}"
-        # )
-        # try:
-        #     print(f"Installing nltk commit_id={commit_id}, running: `{command}`")
-        #     subprocess.check_call(command, shell=True)
-        # except Exception as e:
-        #     result_code = e.returncode
-        #     print(f"`pip install` process error: {e.output}")
-        #     out = e.output
-        # else:
-        # print(f"Coululd not import `nltk` please install it by running `pip install git+https://github.com/nltk/nltk@{commit_id}`.")
-
-
-try:
-    from nltk.corpus import wordnet2022 as wn
-except ImportError:
-    # import nltk
-    import_install_nltk_commit()
-
-    nltk.download("wordnet2022")
-    nltk.download("punkt")
-    nltk.download("brown")
-    nltk.download("averaged_perceptron_tagger")
+    try:
+        from nltk.corpus import wordnet2022 as wn
+    except ImportError:
+        nltk.download("wordnet2022")
+        nltk.download("punkt")
+        nltk.download("brown")
+        nltk.download("averaged_perceptron_tagger")
+
+        from nltk.corpus import wordnet2022 as wn
 
-    from nltk.corpus import wordnet2022 as wn
 
+_ensure_nltk()  # Running this by itself will not import anything, but will raise an error if nltk is not installed
+from nltk.corpus import wordnet2022 as wn
 
 DEFAULT_TOP_SYNSET_STR = "entity.n.01"
 # DEFAULT_TOP_SYNSET_STR = "physical_entity.n.01"
 # DEFAULT_TOP_SYNSET_STR = "object.n.01"
 
 
 def _gather_synsets(current_synset_str: str) -> List[str]:
```

### Comparing `objathor-0.0.2/objathor.egg-info/PKG-INFO` & `objathor-0.0.4/objathor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objathor
-Version: 0.0.2
+Version: 0.0.4
 Summary: Objaverse asset importer for THOR
 Home-page: https://github.com/allenai/objathor
 Author: Allen Institute for AI
 Author-email: contact@allenai.org
 License: Apache 2.0
 Keywords: 3D assets,annotation,
 Classifier: Development Status :: 4 - Beta
@@ -44,21 +44,21 @@
 
 We recommend setting an environment variable with your OpenAI key:
 
 ```bash
 export OPENAI_API_KEY=[Your key]
 ```
 
-If we're planning to annotate objects for which we don't have pre-generated
+If you're planning to annotate objects for which we don't have pre-generated
 views in S3 (see an example under [Annotation](#annotation) below), we also need to install blender either as an extra (as shown above) or as an application:
 
 ### Blender install instructions
 Installing  the `Blender` as a module:
 ```bash
-pip install -e bpy"
+pip install bpy
 ```
 Installing  the Blender as a module, requires a python `3.10` environment.
 
 Or installing blender as an application:
 [Blender install instructions](https://docs.blender.org/manual/en/latest/getting_started/installing/index.html)
 
 If application is not in the cannonical directories you may need to pass `blender_installation_path` to scripts that use Blender.
```

### Comparing `objathor-0.0.2/objathor.egg-info/SOURCES.txt` & `objathor-0.0.4/objathor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `objathor-0.0.2/setup.py` & `objathor-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     REQUIREMENTS = _read_reqs("requirements.txt")
     REQUIREMENTS_ANNOTATION = _read_reqs("requirements-annotation.txt")
 
     setup(
         name="objathor",
         packages=find_packages(),
         include_package_data=True,
-        version="0.0.2",
+        version="0.0.4",
         license="Apache 2.0",
         description="Objaverse asset importer for THOR",
         long_description=long_description,
         long_description_content_type="text/markdown",
         author="Allen Institute for AI",
         author_email="contact@allenai.org",
         url="https://github.com/allenai/objathor",
```

