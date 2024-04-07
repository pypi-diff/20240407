# Comparing `tmp/gns3-gui-3.0.0b1.tar.gz` & `tmp/gns3-gui-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gns3-gui-3.0.0b1.tar", last modified: Mon Nov 27 01:28:23 2023, max compression
+gzip compressed data, was "gns3-gui-3.0.0b2.tar", last modified: Sun Apr  7 12:41:31 2024, max compression
```

## Comparing `gns3-gui-3.0.0b1.tar` & `gns3-gui-3.0.0b2.tar`

### file list

```diff
@@ -1,887 +1,887 @@
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.383905 gns3-gui-3.0.0b1/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   118497 2023-11-27 01:13:32.000000 gns3-gui-3.0.0b1/CHANGELOG
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35147 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/LICENSE
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      138 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/MANIFEST.in
--rw-r--r--   0 grossmj   (1000) grossmj   (1000)    44080 2023-11-27 01:28:23.383905 gns3-gui-3.0.0b1/PKG-INFO
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1714 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/README.md
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       94 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/dev-requirements.txt
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.083979 gns3-gui-3.0.0b1/gns3/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       33 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      736 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/__main__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3456 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/appliance_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3017 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/application.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8604 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/base_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5711 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/compute.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9953 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/compute_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7972 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/compute_summary_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9461 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/console_cmd.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9947 2023-07-31 08:35:08.000000 gns3-gui-3.0.0b1/gns3/console_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16667 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/controller.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6348 2023-11-27 01:12:04.000000 gns3-gui-3.0.0b1/gns3/crash_report.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.095976 gns3-gui-3.0.0b1/gns3/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1197 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/about_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32085 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/appliance_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/capture_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2339 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/configuration_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/console_command_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8429 2022-11-02 16:17:56.000000 gns3-gui-3.0.0b1/gns3/dialogs/custom_adapters_configuration_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7834 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/doctor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3310 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/edit_compute_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6711 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/edit_project_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1993 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/exec_command_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4830 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/export_debug_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/file_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7036 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/filter_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3579 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/idlepc_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6486 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/image_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/login_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11851 2023-07-03 09:11:41.000000 gns3-gui-3.0.0b1/gns3/dialogs/new_template_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1879 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/node_info_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11399 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/node_properties_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/notif_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9036 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/preferences_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3788 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/profile_select.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14147 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/project_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9689 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/project_export_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3411 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/project_welcome_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11056 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/setup_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2457 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/show_readme_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5704 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/snapshots_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7860 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/style_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4838 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b1/gns3/dialogs/style_editor_dialog_link.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7859 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/symbol_selection_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4714 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/dialogs/text_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7243 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/vm_with_images_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6675 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/dialogs/vm_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    70371 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/graphics_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32258 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/http_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1690 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/http_client_error.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8433 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/image_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2347 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/image_upload_manager.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.103974 gns3-gui-3.0.0b1/gns3/items/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/items/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9696 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/items/drawing_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/items/ellipse_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10344 2023-05-14 07:10:13.000000 gns3-gui-3.0.0b1/gns3/items/ethernet_link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2428 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/items/image_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8318 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/items/label_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7141 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/items/line_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21450 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/items/link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4404 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/items/logo_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18633 2023-11-09 03:05:18.000000 gns3-gui-3.0.0b1/gns3/items/node_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3125 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b1/gns3/items/rectangle_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7942 2023-05-14 07:10:13.000000 gns3-gui-3.0.0b1/gns3/items/serial_link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7539 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b1/gns3/items/shape_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6164 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/items/text_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1058 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/items/utils.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18698 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/link.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.103974 gns3-gui-3.0.0b1/gns3/linux/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.103974 gns3-gui-3.0.0b1/gns3/linux/applications/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      282 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/applications/gns3.desktop
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1152 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/gns3-gui.xml
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.059985 gns3-gui-3.0.0b1/gns3/linux/icons/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.059985 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.059985 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/16x16/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.103974 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/16x16/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      832 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/16x16/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.059985 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/32x32/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.103974 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/32x32/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1905 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/32x32/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.059985 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.103974 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.107973 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/mimetypes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6075 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4500 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.059985 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.107973 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/apps/gns3.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.107973 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/mimetypes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22534 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11492 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19682 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/local_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21444 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/local_server.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/logger.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12226 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/main.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    55556 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/main_window.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.107973 gns3-gui-3.0.0b1/gns3/modules/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1095 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.107973 gns3-gui-3.0.0b1/gns3/modules/builtin/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4854 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5614 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/atm_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5123 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/cloud.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.107973 gns3-gui-3.0.0b1/gns3/modules/builtin/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/dialogs/cloud_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1930 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2891 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ethernet_hub.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4557 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ethernet_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4085 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/frame_relay_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2437 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/nat.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.115971 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7683 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/atm_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2595 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/builtin_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22227 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/cloud_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9871 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/cloud_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5598 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9707 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10385 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6627 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1750 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.119970 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9107 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/atm_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13163 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2666 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/builtin_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3269 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/builtin_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    19129 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24391 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4401 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5315 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3433 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5232 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3876 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5670 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4431 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5536 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4186 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6247 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9148 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13299 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4397 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5674 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4222 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6343 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7303 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11148 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.119970 gns3-gui-3.0.0b1/gns3/modules/builtin/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1212 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/builtin/utils/tree_widget_item.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.119970 gns3-gui-3.0.0b1/gns3/modules/docker/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4407 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.119970 gns3-gui-3.0.0b1/gns3/modules/docker/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5356 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/dialogs/docker_vm_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5188 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/docker_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.119970 gns3-gui-3.0.0b1/gns3/modules/docker/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1968 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/pages/docker_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9347 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/pages/docker_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12426 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/pages/docker_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1385 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.123969 gns3-gui-3.0.0b1/gns3/modules/docker/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2400 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2852 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12930 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17480 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4709 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11020 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16543 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.127968 gns3-gui-3.0.0b1/gns3/modules/dynamips/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7828 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2360 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/adapters.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.127968 gns3-gui-3.0.0b1/gns3/modules/dynamips/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17596 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/dialogs/ios_router_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.131967 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1759 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c1700.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2320 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c2600.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c2691.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2022-12-24 09:42:12.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c3600.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c3725.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c3745.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1885 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c7200.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2218 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/etherswitch_router.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12170 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/router.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.135966 gns3-gui-3.0.0b1/gns3/modules/dynamips/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/pages/dynamips_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27874 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/pages/ios_router_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22638 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/pages/ios_router_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7767 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.135966 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     6439 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/dynamips_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8491 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    35772 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    45950 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4850 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5957 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15247 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23315 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.139965 gns3-gui-3.0.0b1/gns3/modules/dynamips/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/utils/decompress_ios.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2179 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/utils/decompress_ios_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/dynamips/wics.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.139965 gns3-gui-3.0.0b1/gns3/modules/iou/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3974 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.139965 gns3-gui-3.0.0b1/gns3/modules/iou/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5044 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/iou/dialogs/iou_device_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4930 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/iou/iou_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.139965 gns3-gui-3.0.0b1/gns3/modules/iou/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13549 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/iou/pages/iou_device_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15262 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/iou/pages/iou_device_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5027 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/pages/iou_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1305 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/iou/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.147963 gns3-gui-3.0.0b1/gns3/modules/iou/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    13890 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17361 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4638 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5659 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6717 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9276 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2927 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3557 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4403 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/module.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1066 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/module_error.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.147963 gns3-gui-3.0.0b1/gns3/modules/qemu/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5394 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.147963 gns3-gui-3.0.0b1/gns3/modules/qemu/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8102 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/dialogs/qemu_image_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4777 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/dialogs/qemu_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.151962 gns3-gui-3.0.0b1/gns3/modules/qemu/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2896 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/pages/qemu_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30663 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/pages/qemu_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15236 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/pages/qemu_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7606 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/qemu_vm.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2054 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.155961 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23636 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_image_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29391 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_image_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2888 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3655 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    32701 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    43581 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4602 2021-10-08 05:49:21.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5444 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12608 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18678 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.155961 gns3-gui-3.0.0b1/gns3/modules/virtualbox/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5807 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.155961 gns3-gui-3.0.0b1/gns3/modules/virtualbox/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.155961 gns3-gui-3.0.0b1/gns3/modules/virtualbox/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4001 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11547 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10054 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1438 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.159960 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3684 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4480 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    10804 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4373 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3801 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5833 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4953 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/virtualbox/virtualbox_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.159960 gns3-gui-3.0.0b1/gns3/modules/vmware/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10348 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.159960 gns3-gui-3.0.0b1/gns3/modules/vmware/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3586 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/dialogs/vmware_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.163959 gns3-gui-3.0.0b1/gns3/modules/vmware/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5647 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/pages/vmware_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11191 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/pages/vmware_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10397 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/pages/vmware_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1731 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.167958 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7503 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8865 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9806 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13005 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4329 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5270 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3802 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5702 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6181 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vmware/vmware_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.171957 gns3-gui-3.0.0b1/gns3/modules/vpcs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4669 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.171957 gns3-gui-3.0.0b1/gns3/modules/vpcs/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.171957 gns3-gui-3.0.0b1/gns3/modules/vpcs/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7092 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9365 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/pages/vpcs_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1064 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.175956 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4135 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6719 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4278 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4868 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3424 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5202 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3653 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4263 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3367 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/modules/vpcs/vpcs_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1630 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/network_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29284 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1513 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/nodes_dock_widget.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9340 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/nodes_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11255 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/packet_capture.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.179955 gns3-gui-3.0.0b1/gns3/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14398 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/pages/controller_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21008 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/pages/general_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/pages/gns3_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/pages/packet_capture_preferences_page.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.179955 gns3-gui-3.0.0b1/gns3/ports/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ports/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      857 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ports/ethernet_port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8108 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ports/port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2335 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ports/port_name_factory.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      887 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ports/serial_port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10489 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/progress.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25110 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/project.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/pycutext.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.179955 gns3-gui-3.0.0b1/gns3/qt/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6678 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/qt/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5143 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/qt/qimage_svg_renderer.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.183954 gns3-gui-3.0.0b1/gns3/registry/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/registry/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9946 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/registry/appliance.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12895 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/registry/appliance_to_template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2646 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/registry/config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4251 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/registry/image.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4698 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/registry/registry.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.183954 gns3-gui-3.0.0b1/gns3/schemas/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15780 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/schemas/appliance.json
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23589 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/schemas/appliance_v8.json
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19624 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/settings.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2766 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/spice_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.183954 gns3-gui-3.0.0b1/gns3/static/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/static/.keep
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2732 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/status_bar.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/style.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/symbol.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6213 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/telnet_console.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8535 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/template_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20587 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/topology.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15220 2023-07-31 08:35:08.000000 gns3-gui-3.0.0b1/gns3/topology_summary_view.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.243939 gns3-gui-3.0.0b1/gns3/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    96556 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/about_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   112145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/about_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10358 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/appliance_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12795 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/appliance_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3516 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/capture_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4471 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/capture_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3197 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/configuration_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/configuration_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5108 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/ui/console_command_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/ui/console_command_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    19259 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/controller_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24059 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/controller_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2012 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/custom_adapters_configuration_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2258 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/custom_adapters_configuration_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3252 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/doctor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3521 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/doctor_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5487 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/edit_compute_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6478 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/edit_compute_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9096 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/edit_project_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11089 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/edit_project_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     1694 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/exec_command_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1648 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/exec_command_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3559 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/export_debug_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3716 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/export_debug_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5607 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/export_project_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8170 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/export_project_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3422 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/file_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/file_editor_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3881 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/filter_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3708 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/filter_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    43663 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/general_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54735 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/general_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7845 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/gns3_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10781 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/gns3_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1824 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/idlepc_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1919 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/idlepc_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3693 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/image_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3823 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/image_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2758 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/login_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2734 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/login_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    41586 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/main_window.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    50821 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/main_window_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3059 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/new_template_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4766 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/new_template_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2636 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/node_info_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/node_info_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/node_properties_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5071 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/node_properties_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     4492 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/ui/packet_capture_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7011 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/ui/packet_capture_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4704 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/preferences_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4996 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/preferences_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4950 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/profile_select_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5375 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/profile_select_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/project_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11436 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/project_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2754 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/project_welcome_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3385 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/project_welcome_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)  9439247 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/resources_rc.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7770 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/setup_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11373 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/setup_wizard_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     2778 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/show_readme_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2882 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/ui/show_readme_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2357 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/snapshots_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2588 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/snapshots_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     6586 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b1/gns3/ui/style_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8330 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b1/gns3/ui/style_editor_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/symbol_selection_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5838 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/symbol_selection_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4884 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b1/gns3/ui/text_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/ui/text_editor_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11356 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b1/gns3/update_manager.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.247939 gns3-gui-3.0.0b1/gns3/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3691 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1294 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b1/gns3/utils/authorize_ubridge.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2799 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/bring_to_front.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/file_copy_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1326 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/get_icon.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1528 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/utils/get_resource.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/utils/import_project_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3816 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/gns3/utils/install_mime_types.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/interfaces.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2295 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b1/gns3/utils/macos_ubridge_setuid.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1256 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/normalize_filename.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5435 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/process_files_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6405 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/progress_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/run_in_terminal.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2524 2023-06-21 10:04:51.000000 gns3-gui-3.0.0b1/gns3/utils/server_select.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4424 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b1/gns3/utils/sudo.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2420 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/wait_for_command_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2713 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/wait_for_connection_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2288 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/wait_for_lambda_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2850 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/gns3/utils/wait_for_runas_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1490 2023-11-27 01:13:32.000000 gns3-gui-3.0.0b1/gns3/version.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2771 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/gns3/vnc_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.383905 gns3-gui-3.0.0b1/gns3_gui.egg-info/
--rw-r--r--   0 grossmj   (1000) grossmj   (1000)    44080 2023-11-27 01:28:23.000000 gns3-gui-3.0.0b1/gns3_gui.egg-info/PKG-INFO
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    30105 2023-11-27 01:28:23.000000 gns3-gui-3.0.0b1/gns3_gui.egg-info/SOURCES.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        1 2023-11-27 01:28:23.000000 gns3-gui-3.0.0b1/gns3_gui.egg-info/dependency_links.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)       36 2023-11-27 01:28:23.000000 gns3-gui-3.0.0b1/gns3_gui.egg-info/entry_points.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)      235 2023-11-27 01:28:23.000000 gns3-gui-3.0.0b1/gns3_gui.egg-info/requires.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        5 2023-11-27 01:28:23.000000 gns3-gui-3.0.0b1/gns3_gui.egg-info/top_level.txt
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1830 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/pyproject.toml
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      217 2023-11-27 01:05:12.000000 gns3-gui-3.0.0b1/requirements.txt
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.247939 gns3-gui-3.0.0b1/resources/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.263935 gns3-gui-3.0.0b1/resources/charcoal_icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6231 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/add-link-1-cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/add-link-1-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/add-link-1.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/add-note-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2879 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/aux-console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/browse-all-icons-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/browse-all-icons.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13891 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/calculate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2220 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2127 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/capture-start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3369 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/capture-stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3362 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/command_line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6261 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/configuration-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8406 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/console_edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4172 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/delete-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4156 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2881 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/duplicate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3852 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3846 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/export-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2822 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24996 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/filter-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/filter-reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25640 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24989 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/firewall-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2141 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/front-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12619 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/help-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12581 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/image-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/import-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/import_export_configs-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2409 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/inspect-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2403 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3738 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/lock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3730 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3546 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/lower_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/minus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/new-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4223 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/node_conception-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/open-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/pc-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/pc.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2680 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/plus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2673 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6090 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/preferences-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6084 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/preferences.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5543 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/quit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5870 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/raise_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3542 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/reload-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2181 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2175 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/router-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5279 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/save-as-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5281 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/save-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/save-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/show-hostname-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/show-interface-names-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/snapshot-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2684 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/switch-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2648 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/unlock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/zoom-in-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/zoom-in.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2808 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/zoom-out-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1746 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/charcoal_icons/zoom-out.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.287929 gns3-gui-3.0.0b1/resources/classic_icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5935 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/add-link-cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2971 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/add-link-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3086 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/add-link.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4148 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/add-note-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4315 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2593 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/aux-console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2589 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/browse-all-icons-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/browse-all-icons.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13890 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/calculate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2992 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2914 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/capture-start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3368 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/capture-stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3363 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/command_line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6254 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/configuration-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8405 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2046 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2070 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/console_edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4162 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/delete-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4143 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2885 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/duplicate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3856 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3857 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4312 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4321 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/export-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24995 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/filter-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/filter-reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25639 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24990 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2047 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/firewall-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2056 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/front-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9629 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/help-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9625 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2011 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/image-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2020 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/import-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2351 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/import_export_configs-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2375 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2373 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/inspect-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2382 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/lock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3731 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3545 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/lower_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/minus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4249 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/new-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4245 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/node_conception-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2243 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/open-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2261 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2166 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3496 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/pc-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3493 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/pc.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2679 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/plus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2674 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5725 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/preferences-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/preferences.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5032 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/quit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5026 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/raise_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3541 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2530 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2266 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/reload-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2275 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2180 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2174 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2313 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/router-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2322 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4710 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/save-as-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4748 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/save-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3417 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/save-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/show-hostname-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3636 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/show-interface-names-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3686 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2876 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/snapshot-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2901 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1742 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2495 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/switch-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/unlock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2761 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/zoom-in-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2785 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/zoom-in.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/zoom-out-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2727 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/classic_icons/zoom-out.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.315922 gns3-gui-3.0.0b1/resources/icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    63187 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/PC-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    60045 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/PC.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    28134 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16099 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/applications.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21937 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   291074 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/browse-all-icons-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   297712 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/browse-all-icons.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32570 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39042 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    37642 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25560 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/cancel-connection.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12039 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31090 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26448 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19139 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23701 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/connection-new-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23702 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/connection-new.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21216 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30385 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13772 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/dialog-warning.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26729 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/drawing.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23490 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16831 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24733 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21372 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10572 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21681 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/filter-capture.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27285 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23917 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    57273 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/firewall-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    53702 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/firewall.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13259 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7175 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/horizontally.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19675 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10549 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39319 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15756 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10184 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/led_gray.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/led_green.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6952 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/led_red.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9965 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/led_yellow.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32132 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6518 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4612 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24126 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16626 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/new.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27187 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30745 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23462 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21534 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19130 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7903 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35282 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31055 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16810 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8571 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    58719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/router-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54133 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/router.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3184 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/rtv.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    40599 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31854 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/save-as.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29835 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/save.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15166 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26306 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18013 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17454 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    67991 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/switch-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    64865 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/switch.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    34969 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5816 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/vertically.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/virtualbox.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/warning.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1906 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/wireshark.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5939 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/zoom-in-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6276 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/zoom-in.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/zoom-out-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6157 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/icons/zoom-out.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.315922 gns3-gui-3.0.0b1/resources/images/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   370070 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/images/gns3.ico
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7892 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/images/gns3_icon_128x128.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16745 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/images/gns3_icon_256x256.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7921 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/images/gns3_logo.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16025 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/resources.qrc
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.315922 gns3-gui-3.0.0b1/resources/styles/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1231 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b1/resources/styles/charcoal.css
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.315922 gns3-gui-3.0.0b1/resources/symbols/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16298 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/atm_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    78565 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/cloud.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/computer.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19782 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/docker_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18650 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/ethernet_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18401 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18343 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/frame_relay_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18128 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/hub.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19150 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/multilayer_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18421 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/qemu_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18494 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16401 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/vbox_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16843 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/vmware_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/resources/symbols/vpcs_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       38 2023-11-27 01:28:23.383905 gns3-gui-3.0.0b1/setup.cfg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.339916 gns3-gui-3.0.0b1/tests/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6326 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/conftest.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.339916 gns3-gui-3.0.0b1/tests/items/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1997 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/items/test_ellipse_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1509 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/items/test_image_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2106 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/items/test_label_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4449 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/items/test_line_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3046 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/items/test_rectangle_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2039 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/items/test_text_item.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.063984 gns3-gui-3.0.0b1/tests/modules/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.339916 gns3-gui-3.0.0b1/tests/modules/docker/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1478 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/modules/docker/test_docker_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.339916 gns3-gui-3.0.0b1/tests/modules/dynamips/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1486 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/modules/dynamips/test_dynamips_init.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.343915 gns3-gui-3.0.0b1/tests/modules/iou/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1841 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/modules/iou/test_iou_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.343915 gns3-gui-3.0.0b1/tests/modules/qemu/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1526 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/modules/qemu/test_qemu_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.343915 gns3-gui-3.0.0b1/tests/modules/virtualbox/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1574 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/modules/virtualbox/test_virtualbox_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.343915 gns3-gui-3.0.0b1/tests/modules/vpcs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/modules/vpcs/test_vpcs_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.343915 gns3-gui-3.0.0b1/tests/qt/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1285 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/qt/test_qimage_svg_renderer.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.347914 gns3-gui-3.0.0b1/tests/registry/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.359911 gns3-gui-3.0.0b1/tests/registry/appliances/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2607 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/arista-veos-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2451 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/arista-veos.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1353 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/broken-microcore-linux.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/cisco-3745-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1356 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/cisco-3745.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1171 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/cisco-iou-l3-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1019 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/cisco-iou-l3.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4047 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/empty-vm-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1612 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/juniper-vsrx.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2022 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/microcore-linux.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1216 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/openvswitch-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1096 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/appliances/openvswitch.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9492 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/registry/test_appliance.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13248 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/registry/test_appliance_to_template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2895 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/registry/test_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2304 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/registry/test_image.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2185 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/registry/test_registry.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1376 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/test_compute.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5810 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_compute_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1717 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_controller.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/test_graphics_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8696 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_http_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3087 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_image_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1596 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_image_upload_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4739 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_link.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13656 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_local_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2980 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_local_server.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1760 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_main_window.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/test_network_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5698 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/test_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1496 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/test_progress.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5498 2023-11-23 03:49:49.000000 gns3-gui-3.0.0b1/tests/test_project.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2574 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/tests/test_spice_console.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/test_topology.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3575 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b1/tests/test_update_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/test_utils.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b1/tests/test_vnc_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2023-11-27 01:28:23.379906 gns3-gui-3.0.0b1/tests/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1394 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/utils/test_file_copy_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3705 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b1/tests/utils/test_server_select.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.608210 gns3-gui-3.0.0b2/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   119702 2024-04-07 11:51:59.000000 gns3-gui-3.0.0b2/CHANGELOG
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35147 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/LICENSE
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      138 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/MANIFEST.in
+-rw-r--r--   0 grossmj   (1000) grossmj   (1000)    43930 2024-04-07 12:41:31.608210 gns3-gui-3.0.0b2/PKG-INFO
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1714 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/README.md
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       94 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/dev-requirements.txt
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.056205 gns3-gui-3.0.0b2/gns3/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       33 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      736 2024-02-12 05:00:39.000000 gns3-gui-3.0.0b2/gns3/__main__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3456 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/appliance_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3017 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/application.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8604 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/base_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5711 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/compute.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9953 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/compute_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7972 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/compute_summary_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9666 2024-03-04 16:17:41.000000 gns3-gui-3.0.0b2/gns3/console_cmd.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9947 2023-07-31 08:35:08.000000 gns3-gui-3.0.0b2/gns3/console_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17467 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/controller.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6351 2024-04-07 11:41:17.000000 gns3-gui-3.0.0b2/gns3/crash_report.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.080205 gns3-gui-3.0.0b2/gns3/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1197 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/about_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32085 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/appliance_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/capture_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2339 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/configuration_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/console_command_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8429 2022-11-02 16:17:56.000000 gns3-gui-3.0.0b2/gns3/dialogs/custom_adapters_configuration_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7834 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/doctor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3310 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/edit_compute_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6711 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/edit_project_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1993 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/exec_command_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4830 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/export_debug_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/file_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7036 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/filter_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3579 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/idlepc_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6486 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/image_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/login_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11851 2023-07-03 09:11:41.000000 gns3-gui-3.0.0b2/gns3/dialogs/new_template_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1879 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/node_info_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11399 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/node_properties_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/notif_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9036 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/preferences_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3788 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/profile_select.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14147 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/project_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9689 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/project_export_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3411 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/project_welcome_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11056 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/setup_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2457 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/show_readme_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5704 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/snapshots_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7860 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/style_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4838 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/dialogs/style_editor_dialog_link.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7859 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/symbol_selection_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4714 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/text_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7243 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/vm_with_images_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6675 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/vm_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    70504 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/graphics_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32258 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/http_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1690 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/http_client_error.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8433 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/image_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2347 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/image_upload_manager.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.088205 gns3-gui-3.0.0b2/gns3/items/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10076 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/items/drawing_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/ellipse_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10344 2023-05-14 07:10:13.000000 gns3-gui-3.0.0b2/gns3/items/ethernet_link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2428 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/image_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8318 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/label_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7141 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/line_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21450 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/items/link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4404 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/logo_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19182 2024-03-04 16:17:41.000000 gns3-gui-3.0.0b2/gns3/items/node_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3125 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/items/rectangle_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7942 2023-05-14 07:10:13.000000 gns3-gui-3.0.0b2/gns3/items/serial_link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7539 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b2/gns3/items/shape_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6164 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/text_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1058 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/utils.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18698 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/link.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/applications/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      282 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/applications/gns3.desktop
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1152 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/gns3-gui.xml
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/16x16/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/16x16/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      832 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/16x16/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/32x32/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/32x32/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1905 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/32x32/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6075 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4500 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/apps/gns3.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22534 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11492 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19682 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/local_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21632 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/local_server.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/logger.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12548 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/main.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    56561 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/main_window.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.096205 gns3-gui-3.0.0b2/gns3/modules/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1095 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.096205 gns3-gui-3.0.0b2/gns3/modules/builtin/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4854 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5614 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/atm_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5123 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/cloud.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.100206 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/cloud_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1930 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2891 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ethernet_hub.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4557 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ethernet_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4085 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/frame_relay_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2437 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/nat.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.104205 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7683 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/atm_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2595 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/builtin_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22227 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/cloud_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9871 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/cloud_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5598 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9707 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10385 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6627 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1750 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.116206 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9107 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/atm_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13163 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2666 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/builtin_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3269 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/builtin_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    19129 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24391 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4401 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5315 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3433 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5232 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3876 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5670 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4431 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5536 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4186 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6247 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9148 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13299 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4397 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5674 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4222 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6343 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7303 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11148 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.120206 gns3-gui-3.0.0b2/gns3/modules/builtin/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1212 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/utils/tree_widget_item.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.120206 gns3-gui-3.0.0b2/gns3/modules/docker/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4407 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.120206 gns3-gui-3.0.0b2/gns3/modules/docker/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5356 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/dialogs/docker_vm_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5188 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/docker_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.120206 gns3-gui-3.0.0b2/gns3/modules/docker/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1968 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9394 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12700 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1385 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.128206 gns3-gui-3.0.0b2/gns3/modules/docker/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2400 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2852 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12930 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17480 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4709 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11020 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16543 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.132206 gns3-gui-3.0.0b2/gns3/modules/dynamips/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7828 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2360 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/adapters.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.132206 gns3-gui-3.0.0b2/gns3/modules/dynamips/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17596 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/dialogs/ios_router_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.136206 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1759 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c1700.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2320 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c2600.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c2691.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2022-12-24 09:42:12.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3600.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3725.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3745.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1885 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c7200.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2218 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/etherswitch_router.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12170 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/router.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.136206 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/dynamips_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27874 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/ios_router_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22638 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/ios_router_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7767 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.152206 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     6439 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/dynamips_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8491 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    35772 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    45950 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4850 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5957 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15247 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23315 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.160206 gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/decompress_ios.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2179 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/decompress_ios_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/wics.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.160206 gns3-gui-3.0.0b2/gns3/modules/iou/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3974 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.160206 gns3-gui-3.0.0b2/gns3/modules/iou/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5044 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/dialogs/iou_device_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4930 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/iou_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.160206 gns3-gui-3.0.0b2/gns3/modules/iou/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13549 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_device_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15262 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_device_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5027 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1305 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.168206 gns3-gui-3.0.0b2/gns3/modules/iou/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    13890 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17361 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4638 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5659 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6717 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9276 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2927 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3557 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4403 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/module.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1066 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/module_error.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.168206 gns3-gui-3.0.0b2/gns3/modules/qemu/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5394 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.168206 gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8102 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/qemu_image_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4777 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/qemu_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.172206 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2896 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30797 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15366 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7651 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/qemu_vm.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2075 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.176206 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23636 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_image_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29391 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_image_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2888 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3655 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    33160 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    44174 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4602 2021-10-08 05:49:21.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5444 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12608 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18678 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.176206 gns3-gui-3.0.0b2/gns3/modules/virtualbox/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5807 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.176206 gns3-gui-3.0.0b2/gns3/modules/virtualbox/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.180206 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4001 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11547 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10054 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1438 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.184206 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3684 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4480 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    10804 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4373 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3801 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5833 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4953 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/virtualbox_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.188206 gns3-gui-3.0.0b2/gns3/modules/vmware/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10348 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.188206 gns3-gui-3.0.0b2/gns3/modules/vmware/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3586 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/dialogs/vmware_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.192206 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5647 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11191 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10397 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1731 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.200206 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7503 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8865 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9806 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13005 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4329 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5270 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3802 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5702 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6181 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/vmware_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.200206 gns3-gui-3.0.0b2/gns3/modules/vpcs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4669 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.200206 gns3-gui-3.0.0b2/gns3/modules/vpcs/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.204207 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7092 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9365 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1064 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.208207 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4135 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6719 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4278 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4868 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3424 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5202 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3653 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4263 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3367 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/vpcs_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1630 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/network_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29284 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1513 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/nodes_dock_widget.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9340 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/nodes_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11255 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/packet_capture.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.208207 gns3-gui-3.0.0b2/gns3/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15586 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/pages/controller_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21008 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/pages/general_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/pages/gns3_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/pages/packet_capture_preferences_page.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.212206 gns3-gui-3.0.0b2/gns3/ports/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      857 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/ethernet_port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8108 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2335 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/port_name_factory.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      887 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/serial_port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10489 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/progress.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25349 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/project.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/pycutext.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.212206 gns3-gui-3.0.0b2/gns3/qt/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6678 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/qt/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5143 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/qt/qimage_svg_renderer.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.216207 gns3-gui-3.0.0b2/gns3/registry/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/registry/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9946 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/appliance.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12895 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/appliance_to_template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2646 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4251 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/image.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4698 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/registry.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.216207 gns3-gui-3.0.0b2/gns3/schemas/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15780 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/schemas/appliance.json
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23629 2024-01-27 06:07:27.000000 gns3-gui-3.0.0b2/gns3/schemas/appliance_v8.json
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19651 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/settings.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2766 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/spice_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.220207 gns3-gui-3.0.0b2/gns3/static/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/static/.keep
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2732 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/status_bar.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/style.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/symbol.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6213 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/telnet_console.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8535 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/template_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20587 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/topology.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15220 2023-07-31 08:35:08.000000 gns3-gui-3.0.0b2/gns3/topology_summary_view.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.276207 gns3-gui-3.0.0b2/gns3/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    96556 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/about_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   112145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/about_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10358 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/appliance_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12795 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/appliance_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3516 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/capture_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4471 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/capture_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3197 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/configuration_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/configuration_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5108 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/ui/console_command_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/ui/console_command_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    20055 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24755 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2012 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/custom_adapters_configuration_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2258 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/custom_adapters_configuration_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3252 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/doctor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3521 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/doctor_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5487 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/edit_compute_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6478 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/edit_compute_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9096 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/edit_project_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11089 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/edit_project_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     1694 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/exec_command_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1648 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/exec_command_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3559 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/export_debug_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3716 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/export_debug_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5607 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/export_project_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8170 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/export_project_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3422 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/file_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/file_editor_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3881 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/filter_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3708 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/filter_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    43663 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/general_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54735 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/general_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7845 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/gns3_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10781 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/gns3_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1824 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/idlepc_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1919 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/idlepc_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3693 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/image_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3823 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/image_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2758 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/login_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2734 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/login_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    41762 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/main_window.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    50875 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/main_window_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3059 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/new_template_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4766 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/new_template_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2636 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/node_info_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/node_info_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/node_properties_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5071 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/node_properties_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     4492 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/ui/packet_capture_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7011 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/ui/packet_capture_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4704 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/preferences_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4996 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/preferences_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4950 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/profile_select_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5375 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/profile_select_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/project_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11436 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/project_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2754 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/project_welcome_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3385 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/project_welcome_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)  9439247 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/resources_rc.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7770 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/setup_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11373 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/setup_wizard_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     2778 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/show_readme_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2882 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/show_readme_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2357 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/snapshots_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2588 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/snapshots_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     6586 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b2/gns3/ui/style_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8330 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b2/gns3/ui/style_editor_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/symbol_selection_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5838 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/symbol_selection_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4884 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/text_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/text_editor_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11356 2024-01-11 02:03:24.000000 gns3-gui-3.0.0b2/gns3/update_manager.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.284207 gns3-gui-3.0.0b2/gns3/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3691 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1294 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/utils/authorize_ubridge.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2799 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/bring_to_front.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/file_copy_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1326 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/get_icon.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1528 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/utils/get_resource.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/utils/import_project_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3816 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/utils/install_mime_types.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/interfaces.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2295 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/utils/macos_ubridge_setuid.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1256 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/normalize_filename.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5435 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/process_files_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6405 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/progress_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/run_in_terminal.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2524 2023-06-21 10:04:51.000000 gns3-gui-3.0.0b2/gns3/utils/server_select.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4424 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/utils/sudo.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2420 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/wait_for_command_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2713 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/wait_for_connection_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2288 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/wait_for_lambda_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2850 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/wait_for_runas_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1490 2024-04-07 11:42:46.000000 gns3-gui-3.0.0b2/gns3/version.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2771 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/vnc_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.604210 gns3-gui-3.0.0b2/gns3_gui.egg-info/
+-rw-r--r--   0 grossmj   (1000) grossmj   (1000)    43930 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/PKG-INFO
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    30105 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        1 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)       36 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/entry_points.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)      235 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/requires.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        5 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/top_level.txt
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1683 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/pyproject.toml
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      217 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/requirements.txt
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.288207 gns3-gui-3.0.0b2/resources/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.328208 gns3-gui-3.0.0b2/resources/charcoal_icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6231 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1-cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-note-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2879 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/aux-console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/browse-all-icons-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/browse-all-icons.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13891 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/calculate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2220 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2127 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/capture-start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3369 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/capture-stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3362 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/command_line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6261 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/configuration-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8406 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/console_edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4172 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/delete-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4156 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2881 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/duplicate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3852 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3846 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/export-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2822 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24996 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/filter-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/filter-reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25640 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24989 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/firewall-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2141 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/front-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12619 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/help-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12581 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/image-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/import-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/import_export_configs-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2409 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/inspect-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2403 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3738 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/lock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3730 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3546 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/lower_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/minus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/new-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4223 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/node_conception-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/open-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/pc-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/pc.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2680 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/plus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2673 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6090 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/preferences-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6084 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/preferences.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5543 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/quit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5870 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/raise_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3542 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/reload-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2181 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2175 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/router-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5279 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/save-as-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5281 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/save-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/save-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/show-hostname-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/show-interface-names-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/snapshot-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2684 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/switch-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2648 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/unlock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-in-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-in.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2808 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-out-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1746 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-out.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.364208 gns3-gui-3.0.0b2/resources/classic_icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5935 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-link-cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2971 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-link-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3086 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-link.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4148 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-note-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4315 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2593 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/aux-console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2589 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/browse-all-icons-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/browse-all-icons.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13890 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/calculate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2992 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2914 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/capture-start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3368 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/capture-stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3363 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/command_line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6254 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/configuration-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8405 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2046 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2070 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/console_edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4162 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/delete-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4143 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2885 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/duplicate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3856 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3857 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4312 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4321 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/export-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24995 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/filter-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/filter-reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25639 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24990 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2047 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/firewall-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2056 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/front-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9629 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/help-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9625 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2011 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/image-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2020 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/import-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2351 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/import_export_configs-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2375 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2373 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/inspect-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2382 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/lock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3731 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3545 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/lower_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/minus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4249 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/new-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4245 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/node_conception-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2243 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/open-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2261 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2166 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3496 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/pc-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3493 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/pc.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2679 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/plus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2674 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5725 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/preferences-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/preferences.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5032 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/quit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5026 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/raise_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3541 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2530 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2266 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/reload-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2275 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2180 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2174 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2313 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/router-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2322 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4710 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/save-as-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4748 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/save-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3417 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/save-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/show-hostname-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3636 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/show-interface-names-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3686 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2876 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/snapshot-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2901 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1742 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2495 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/switch-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/unlock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2761 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/zoom-in-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2785 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/zoom-in.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/zoom-out-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2727 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/zoom-out.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.472209 gns3-gui-3.0.0b2/resources/icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    63187 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/PC-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    60045 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/PC.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    28134 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16099 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/applications.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21937 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   291074 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/browse-all-icons-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   297712 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/browse-all-icons.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32570 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39042 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    37642 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25560 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/cancel-connection.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12039 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31090 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26448 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19139 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23701 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/connection-new-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23702 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/connection-new.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21216 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30385 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13772 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/dialog-warning.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26729 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/drawing.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23490 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16831 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24733 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21372 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10572 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21681 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/filter-capture.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27285 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23917 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    57273 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/firewall-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    53702 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/firewall.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13259 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7175 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/horizontally.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19675 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10549 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39319 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15756 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10184 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/led_gray.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/led_green.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6952 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/led_red.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9965 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/led_yellow.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32132 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6518 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4612 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24126 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16626 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/new.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27187 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30745 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23462 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21534 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19130 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7903 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35282 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31055 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16810 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8571 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    58719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/router-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54133 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/router.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3184 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/rtv.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    40599 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31854 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/save-as.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29835 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/save.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15166 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26306 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18013 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17454 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    67991 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/switch-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    64865 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/switch.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    34969 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5816 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/vertically.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/virtualbox.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/warning.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1906 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/wireshark.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5939 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/zoom-in-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6276 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/zoom-in.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/zoom-out-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6157 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/zoom-out.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.476209 gns3-gui-3.0.0b2/resources/images/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   370070 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/images/gns3.ico
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7892 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/images/gns3_icon_128x128.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16745 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/images/gns3_icon_256x256.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7921 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/images/gns3_logo.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16025 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/resources.qrc
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.476209 gns3-gui-3.0.0b2/resources/styles/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1231 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/styles/charcoal.css
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.476209 gns3-gui-3.0.0b2/resources/symbols/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16298 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/atm_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    78565 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/cloud.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/computer.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19782 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/docker_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18650 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/ethernet_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18401 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18343 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/frame_relay_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18128 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/hub.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19150 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/multilayer_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18421 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/qemu_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18494 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16401 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/vbox_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16843 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/vmware_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/vpcs_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       38 2024-04-07 12:41:31.608210 gns3-gui-3.0.0b2/setup.cfg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.492209 gns3-gui-3.0.0b2/tests/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6326 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/conftest.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.492209 gns3-gui-3.0.0b2/tests/items/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1997 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/items/test_ellipse_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1509 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/items/test_image_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2106 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/items/test_label_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4449 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/items/test_line_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3046 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/items/test_rectangle_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2039 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/items/test_text_item.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.036205 gns3-gui-3.0.0b2/tests/modules/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.492209 gns3-gui-3.0.0b2/tests/modules/docker/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1478 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/docker/test_docker_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.496209 gns3-gui-3.0.0b2/tests/modules/dynamips/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1486 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/dynamips/test_dynamips_init.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.496209 gns3-gui-3.0.0b2/tests/modules/iou/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1841 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/iou/test_iou_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.496209 gns3-gui-3.0.0b2/tests/modules/qemu/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1526 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/qemu/test_qemu_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.500209 gns3-gui-3.0.0b2/tests/modules/virtualbox/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1574 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/virtualbox/test_virtualbox_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.500209 gns3-gui-3.0.0b2/tests/modules/vpcs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/vpcs/test_vpcs_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.500209 gns3-gui-3.0.0b2/tests/qt/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1285 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/qt/test_qimage_svg_renderer.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.504209 gns3-gui-3.0.0b2/tests/registry/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.532210 gns3-gui-3.0.0b2/tests/registry/appliances/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2607 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/arista-veos-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2451 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/arista-veos.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1353 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/broken-microcore-linux.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/cisco-3745-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1356 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/cisco-3745.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1171 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/cisco-iou-l3-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1019 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/cisco-iou-l3.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4047 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/empty-vm-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1612 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/juniper-vsrx.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2022 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/microcore-linux.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1216 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/openvswitch-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1096 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/openvswitch.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9480 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/registry/test_appliance.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13248 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/registry/test_appliance_to_template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2895 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/registry/test_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2304 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/registry/test_image.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2185 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/registry/test_registry.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1376 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_compute.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5810 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_compute_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1717 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_controller.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_graphics_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8696 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_http_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3087 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_image_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1596 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_image_upload_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4739 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_link.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13656 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_local_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2980 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_local_server.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1760 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_main_window.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_network_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5698 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1496 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_progress.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5498 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_project.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2574 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/tests/test_spice_console.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_topology.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3575 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/test_update_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_utils.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/tests/test_vnc_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.588210 gns3-gui-3.0.0b2/tests/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1394 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/utils/test_file_copy_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3705 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/utils/test_server_select.py
```

### Comparing `gns3-gui-3.0.0b1/CHANGELOG` & `gns3-gui-3.0.0b2/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 # Change Log
 
+## 3.0.0b2 07/04/2024
+
+* Enable local controller support on Linux
+* Support for custom Qemu path in templates and nodes
+* Round CPUs value in Docker templates and VMs. Ref https://github.com/GNS3/gns3-gui/issues/3572
+
+## 2.2.46 26/02/2024
+
+* Add GNS3 console command "env" to show what environment variables are used. Ref https://github.com/GNS3/gns3-server/issues/2306
+* Add CTRL+C shortcut to copy status bar message. Ref #3561
+* Key modifier (ALT) to ignore snap to grid. Fixes #3538
+* Increase timeout to 5s for status bar messages. The coordinates message has no timeout and can be reset when clicking on the scene. Ref #3561
+* Add reset GUI state feature. Ref #3549
+* Fix for hiding Windows terminal. Ref #3290
+* Drop support for Python 3.6
+* Upgrade sentry-sdk, psutil and distro dependencies
+
+## 2.2.45 12/01/2024
+
+* Add missing console_type values in appliance_v8.json. Ref https://github.com/GNS3/gns3-registry/issues/849
+* Handle moved project notifications on controller stream
+* Add debug for PATH env variable
+* Add custom executable paths on Windows
+* Add --suppressApplicationTitle for Windows terminal. Fixes https://github.com/GNS3/gns3-gui/issues/3544
+* Upgrade sentry-sdk and aiohttp
+
 ## 3.0.0b1 27/11/2023
 
 * Upgrade sentry-sdk to v1.37.1
 * Deactivate showing a percentage in progress bar. Ref #3543
 
 ## 3.0.0a6 15/11/2023
```

### Comparing `gns3-gui-3.0.0b1/LICENSE` & `gns3-gui-3.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/PKG-INFO` & `gns3-gui-3.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gns3-gui
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: GNS3 graphical interface for the GNS3 server.
 Author-email: Jeremy Grossmann <developers@gns3.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,36 +687,33 @@
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.4
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsonschema<4.18,>=4.17.3
-Requires-Dist: sentry-sdk<1.38,==1.37.1
-Requires-Dist: psutil==5.9.6
-Requires-Dist: distro>=1.8.0
+Requires-Dist: sentry-sdk<1.41,==1.40.6
+Requires-Dist: psutil==5.9.8
+Requires-Dist: distro>=1.9.0
 Requires-Dist: truststore>=0.8.0; python_version >= "3.10"
 Requires-Dist: importlib-resources>=1.3; python_version <= "3.9"
 Provides-Extra: dev
-Requires-Dist: pytest==7.4.0; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: flake8==5.0.4; extra == "dev"
-Requires-Dist: pytest-timeout==2.1.0; extra == "dev"
+Requires-Dist: pytest-timeout==2.3.1; extra == "dev"
 
 GNS3-gui
 ========
 
 [![GitHub Actions tests](https://github.com/GNS3/gns3-gui/workflows/testing/badge.svg)](https://github.com/GNS3/gns3-gui/actions?query=workflow%3Atesting)
 [![Latest PyPi version](https://img.shields.io/pypi/v/gns3-gui.svg)](https://pypi.python.org/pypi/gns3-gui)
 [![Snyk scanning](https://snyk.io/test/github/GNS3/gns3-gui/badge.svg)](https://snyk.io/test/github/GNS3/gns3-gui)
```

### Comparing `gns3-gui-3.0.0b1/README.md` & `gns3-gui-3.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/__main__.py` & `gns3-gui-3.0.0b2/gns3/__main__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/appliance_manager.py` & `gns3-gui-3.0.0b2/gns3/appliance_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/application.py` & `gns3-gui-3.0.0b2/gns3/application.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/base_node.py` & `gns3-gui-3.0.0b2/gns3/base_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/compute.py` & `gns3-gui-3.0.0b2/gns3/compute.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/compute_manager.py` & `gns3-gui-3.0.0b2/gns3/compute_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/compute_summary_view.py` & `gns3-gui-3.0.0b2/gns3/compute_summary_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/console_cmd.py` & `gns3-gui-3.0.0b2/gns3/console_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 Handles commands typed in the GNS3 console.
 """
 
+import os
 import sys
 import cmd
 import struct
 from .qt import sip
 
 from .node import Node
 from .qt import QtCore
@@ -30,14 +31,22 @@
 
 import logging
 log = logging.getLogger(__name__)
 
 
 class ConsoleCmd(cmd.Cmd):
 
+    def do_env(self, args):
+        """
+        Show the environment variables used by GNS3.
+        """
+
+        for key, val in os.environ.items():
+            print("{}={}".format(key, val))
+
     def do_version(self, args):
         """
         Show the version of GNS3 and its dependencies.
         """
 
         compiled = ""
         if hasattr(sys, "frozen"):
```

### Comparing `gns3-gui-3.0.0b1/gns3/console_view.py` & `gns3-gui-3.0.0b2/gns3/console_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/controller.py` & `gns3-gui-3.0.0b2/gns3/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -443,14 +443,21 @@
                 show_progress=False
             )
         else:
             self._notification_stream = self._http_client.connectWebSocket(self._websocket, "/notifications/ws")
             self._notification_stream.textMessageReceived.connect(self._websocket_event_received)
             self._notification_stream.error.connect(self._websocket_error)
             self._notification_stream.sslErrors.connect(self._sslErrorsSlot)
+            self._notification_stream.disconnected.connect(self._websocket_disconnected)
+
+    def _websocket_disconnected(self):
+
+        self._connected = False
+        self.disconnected_signal.emit()
+        self.stopListenNotifications()
 
     def stopListenNotifications(self):
         if self._notification_stream:
             log.debug("Stop listening for notifications from controller")
             stream = self._notification_stream
             self._notification_stream = None
             stream.abort()
@@ -461,14 +468,15 @@
         """
         if self._notification_stream:
             self._notification_stream = None
             self._startListenNotifications()
 
     @qslot
     def _websocket_error(self, error):
+
         if self._notification_stream:
             log.error("Websocket controller notification stream error: {}".format(self._notification_stream.errorString()))
             self.stopListenNotifications()
 
     @qslot
     def _sslErrorsSlot(self, ssl_errors):
 
@@ -491,14 +499,24 @@
             TemplateManager.instance().templateDataReceivedCallback(result["event"])
         elif result["action"] == "template.deleted":
             from gns3.template_manager import TemplateManager
             TemplateManager.instance().deleteTemplateCallback(result["event"])
         elif result["action"] == "compute.created" or result["action"] == "compute.updated":
             from .compute_manager import ComputeManager
             ComputeManager.instance().computeDataReceivedCallback(result["event"])
+        elif result["action"] == "project.closed":
+            from .topology import Topology
+            project = Topology.instance().project()
+            if project and project.id() == result["event"]["project_id"]:
+                Topology.instance().setProject(None)
+        elif result["action"] == "project.updated":
+            from .topology import Topology
+            project = Topology.instance().project()
+            if project and project.id() == result["event"]["project_id"]:
+                project.projectUpdatedCallback(result["event"])
         elif result["action"] == "log.error":
             log.error(result["event"]["message"])
         elif result["action"] == "log.warning":
             log.warning(result["event"]["message"])
         elif result["action"] == "log.info":
             log.info(result["event"]["message"], extra={"show": True})
         elif result["action"] == "ping":
```

### Comparing `gns3-gui-3.0.0b1/gns3/crash_report.py` & `gns3-gui-3.0.0b2/gns3/crash_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 class CrashReport:
 
     """
     Report crash to a third party service
     """
 
-    DSN = "https://e8a092c2b34cea59be10b291d760ce65@o19455.ingest.sentry.io/38506"
+    DSN = "https://5450a634dcf74dacf3f24800e31c4cf8@o19455.ingest.us.sentry.io/38506"
     _instance = None
 
     def __init__(self):
         # We don't want sentry making noise if an error is caught when we don't have internet
         sentry_errors = logging.getLogger('sentry.errors')
         sentry_errors.disabled = True
```

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/about_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/about_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/appliance_wizard.py` & `gns3-gui-3.0.0b2/gns3/dialogs/appliance_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/capture_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/capture_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/configuration_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/configuration_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/console_command_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/console_command_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/custom_adapters_configuration_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/custom_adapters_configuration_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/doctor_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/doctor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/edit_compute_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/edit_compute_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/edit_project_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/edit_project_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/exec_command_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/exec_command_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/export_debug_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/export_debug_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/file_editor_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/file_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/filter_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/filter_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/idlepc_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/idlepc_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/image_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/image_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/login_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/login_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/new_template_wizard.py` & `gns3-gui-3.0.0b2/gns3/dialogs/new_template_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/node_info_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/node_info_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/node_properties_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/node_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/notif_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/notif_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/preferences_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/preferences_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/profile_select.py` & `gns3-gui-3.0.0b2/gns3/dialogs/profile_select.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/project_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/project_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/project_export_wizard.py` & `gns3-gui-3.0.0b2/gns3/dialogs/project_export_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/project_welcome_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/project_welcome_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/setup_wizard.py` & `gns3-gui-3.0.0b2/gns3/dialogs/setup_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/show_readme_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/show_readme_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/snapshots_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/snapshots_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/style_editor_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/style_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/style_editor_dialog_link.py` & `gns3-gui-3.0.0b2/gns3/dialogs/style_editor_dialog_link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/symbol_selection_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/symbol_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/text_editor_dialog.py` & `gns3-gui-3.0.0b2/gns3/dialogs/text_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/vm_with_images_wizard.py` & `gns3-gui-3.0.0b2/gns3/dialogs/vm_with_images_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/dialogs/vm_wizard.py` & `gns3-gui-3.0.0b2/gns3/dialogs/vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/graphics_view.py` & `gns3-gui-3.0.0b2/gns3/graphics_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,16 @@
 
         is_not_link = True
         is_not_logo = True
 
         item = self.itemAt(event.pos())
         if item and sip.isdeleted(item):
             return
+        elif not item:
+            self._main_window.uiStatusBar.clearMessage()  # reset the status bar message when clicking on the scene
 
         if item and (isinstance(item, LinkItem) or isinstance(item.parentItem(), LinkItem)):
             is_not_link = False
         if item and (isinstance(item, LogoItem) or isinstance(item.parentItem(), LogoItem)):
             is_not_logo = False
         else:
             for it in self.scene().items():
@@ -589,15 +591,15 @@
         Scales the view (zoom in and out).
         """
 
         factor = self.transform().scale(scale_factor, scale_factor).mapRect(QtCore.QRectF(0, 0, 1, 1)).width()
         if factor < 0.10 or factor > 10:
             return
         self.scale(scale_factor, scale_factor)
-        self._main_window.uiStatusBar.showMessage("Zoom: {}%".format(round(self.transform().m11() * 100)), 2000)
+        self._main_window.uiStatusBar.showMessage("Zoom: {}%".format(round(self.transform().m11() * 100)), 5000)
 
     def keyPressEvent(self, event):
         """
         Handles all key press events for this view.
 
         :param event: QKeyEvent
         """
@@ -634,15 +636,15 @@
             self._newlink.setMousePoint(self.mapToScene(event.pos()))
             event.ignore()
         else:
             item = self.itemAt(event.pos())
             if item:
                 # show item coords in the status bar
                 coords = "X: {} Y: {} Z: {}".format(item.x(), item.y(), item.zValue())
-                self._main_window.uiStatusBar.showMessage(coords, 2000)
+                self._main_window.uiStatusBar.showMessage(coords)
 
             # force the children to redraw because of a problem with QGraphicsEffect
             for item in self.scene().selectedItems():
                 for child in item.childItems():
                     child.update()
             super().mouseMoveEvent(event)
```

### Comparing `gns3-gui-3.0.0b1/gns3/http_client.py` & `gns3-gui-3.0.0b2/gns3/http_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/http_client_error.py` & `gns3-gui-3.0.0b2/gns3/http_client_error.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/image_manager.py` & `gns3-gui-3.0.0b2/gns3/image_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/image_upload_manager.py` & `gns3-gui-3.0.0b2/gns3/image_upload_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/drawing_item.py` & `gns3-gui-3.0.0b2/gns3/items/drawing_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     """
     Base class for non emulation item
     """
 
     def __init__(self, project=None, pos=None, drawing_id=None, svg=None, z=0, locked=False, rotation=0, **kws):
         self._id = drawing_id
         self._deleting = False
+        self._allow_snap_to_grid = True
         self._locked = locked
         if self._id is None:
             self._id = str(uuid.uuid4())
         self.setFlags(QtWidgets.QGraphicsItem.ItemIsMovable | QtWidgets.QGraphicsItem.ItemIsFocusable | QtWidgets.QGraphicsItem.ItemIsSelectable | QtWidgets.QGraphicsItem.ItemSendsGeometryChanges)
 
         from ..main_window import MainWindow
         self._graphics_view = MainWindow.instance().uiGraphicsView
@@ -131,26 +132,38 @@
                 self.setRotation(self.rotation() - 1)
             return True
         elif key in (QtCore.Qt.Key_M, QtCore.Qt.Key_Minus) and modifiers & QtCore.Qt.AltModifier \
                 or key == QtCore.Qt.Key_Minus and modifiers & QtCore.Qt.AltModifier and modifiers & QtCore.Qt.KeypadModifier:
             if self.rotation() < 360.0:
                 self.setRotation(self.rotation() + 1)
                 return True
+        elif modifiers & QtCore.Qt.AltModifier:
+            self._allow_snap_to_grid = False
+            return True
         return False
 
     def keyPressEvent(self, event):
         """
         Handles all key press events
 
         :param event: QKeyEvent
         """
 
         if not self.handleKeyPressEvent(event):
             QtWidgets.QGraphicsItem.keyPressEvent(self, event)
 
+    def keyReleaseEvent(self, event):
+        """
+        Handles all key release events
+
+        :param event: QKeyEvent
+        """
+
+        self._allow_snap_to_grid = True
+
     def __json__(self):
         data = {
             "drawing_id": self._id,
             "x": int(self.pos().x()),
             "y": int(self.pos().y()),
             "z": int(self.zValue()),
             "locked": self._locked,
@@ -209,15 +222,16 @@
         from ..topology import Topology
         Topology.instance().removeDrawing(self)
         if self._id and not skip_controller:
             self._project.delete("/drawings/" + self._id, None, body=self.__json__())
 
     def itemChange(self, change, value):
 
-        if change == QtWidgets.QGraphicsItem.ItemPositionChange and self._main_window.uiSnapToGridAction.isChecked():
+        if change == QtWidgets.QGraphicsItem.ItemPositionChange and self._main_window.uiSnapToGridAction.isChecked() \
+                and self._allow_snap_to_grid:
             grid_size = self._graphics_view.drawingGridSize()
             value.setX(grid_size * round(value.x() / grid_size))
             value.setY(grid_size * round(value.y() / grid_size))
 
         if change == QtWidgets.QGraphicsItem.ItemSelectedChange:
             if not value:
                 self.updateDrawing()
```

### Comparing `gns3-gui-3.0.0b1/gns3/items/ellipse_item.py` & `gns3-gui-3.0.0b2/gns3/items/ellipse_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/ethernet_link_item.py` & `gns3-gui-3.0.0b2/gns3/items/ethernet_link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/image_item.py` & `gns3-gui-3.0.0b2/gns3/items/image_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/label_item.py` & `gns3-gui-3.0.0b2/gns3/items/label_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/line_item.py` & `gns3-gui-3.0.0b2/gns3/items/line_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/link_item.py` & `gns3-gui-3.0.0b2/gns3/items/link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/logo_item.py` & `gns3-gui-3.0.0b2/gns3/items/logo_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/node_item.py` & `gns3-gui-3.0.0b2/gns3/items/node_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
         # attached node
         self._node = node
         # link items connected to this node item.
         self._links = []
         self._symbol = None
         self._locked = False
+        self._allow_snap_to_grid = True
 
         # says if the attached node has been initialized
         # by the server.
         self._initialized = False
 
         # node label
         self._node_label = None
@@ -465,15 +466,16 @@
         """
         Notifies this node item that some part of the item's state changes.
 
         :param change: GraphicsItemChange type
         :param value: value of the change
         """
 
-        if change == QtWidgets.QGraphicsItem.ItemPositionChange and self._main_window.uiSnapToGridAction.isChecked():
+        if change == QtWidgets.QGraphicsItem.ItemPositionChange and self._main_window.uiSnapToGridAction.isChecked() \
+                and self._allow_snap_to_grid:
             grid_size = self._main_window.uiGraphicsView.nodeGridSize()
             mid_x = self.boundingRect().width() / 2
             value.setX((grid_size * round((value.x() + mid_x) / grid_size)) - mid_x)
             mid_y = self.boundingRect().height() / 2
             value.setY((grid_size * round((value.y() + mid_y) / grid_size)) - mid_y)
 
         # dynamically change the renderer when this node item is selected/unselected.
@@ -527,14 +529,35 @@
         :param value: Z value
         """
 
         super().setZValue(value)
         for link in self._links:
             link.adjust()
 
+    def keyPressEvent(self, event):
+        """
+        Handles all key press events
+
+        :param event: QKeyEvent
+        """
+
+        if event.modifiers() & QtCore.Qt.AltModifier:
+            self._allow_snap_to_grid = False
+        else:
+            super().keyPressEvent(event)
+
+    def keyReleaseEvent(self, event):
+        """
+        Handles all key release events
+
+        :param event: QKeyEvent
+        """
+
+        self._allow_snap_to_grid = True
+
     def locked(self):
 
         return self._locked
 
     def setLocked(self, locked):
         """
         Sets the locked value.
```

### Comparing `gns3-gui-3.0.0b1/gns3/items/rectangle_item.py` & `gns3-gui-3.0.0b2/gns3/items/rectangle_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/serial_link_item.py` & `gns3-gui-3.0.0b2/gns3/items/serial_link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/shape_item.py` & `gns3-gui-3.0.0b2/gns3/items/shape_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/text_item.py` & `gns3-gui-3.0.0b2/gns3/items/text_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/items/utils.py` & `gns3-gui-3.0.0b2/gns3/items/utils.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/link.py` & `gns3-gui-3.0.0b2/gns3/link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/gns3-gui.xml` & `gns3-gui-3.0.0b2/gns3/linux/gns3-gui.xml`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/16x16/apps/gns3.png` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/16x16/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/32x32/apps/gns3.png` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/32x32/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/apps/gns3.png` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/apps/gns3.svg` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/apps/gns3.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg` & `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/local_config.py` & `gns3-gui-3.0.0b2/gns3/local_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/local_server.py` & `gns3-gui-3.0.0b2/gns3/local_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             self._settings = new_settings
         else:
             self._settings.update(new_settings)
         self._port = self._settings["port"]
         Controller.instance().setSettings(self._settings)
 
         # Settings have changed we need to restart the server
-        if old_settings != self._settings:
+        if not Controller.instance().connected() or old_settings != self._settings:
             if self._settings["auto_start"]:
                 # We restart the local server only if we really need. Auth can be hot change
                 settings_require_restart = ('host', 'port', 'path')
                 need_restart = False
                 for s in settings_require_restart:
                     if old_settings.get(s) != self._settings.get(s):
                         need_restart = True
@@ -232,14 +232,16 @@
                 if need_restart:
                     self.stopLocalServer(wait=True)
 
                 self.localServerAutoStartIfRequired()
             # If the controller is remote:
             else:
                 self.stopLocalServer(wait=True)
+                if Controller.instance().isRemote() and not Controller.instance().connected():
+                    Controller.instance().connect()
 
     def shouldLocalServerAutoStart(self):
         """
         Returns either the local server
         is automatically started on startup.
 
         :returns: boolean
```

### Comparing `gns3-gui-3.0.0b1/gns3/logger.py` & `gns3-gui-3.0.0b2/gns3/logger.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/main.py` & `gns3-gui-3.0.0b2/gns3/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,22 +144,24 @@
         frozen_dir = os.path.dirname(os.path.abspath(sys.executable))
         if sys.platform.startswith("darwin"):
             frozen_dirs = [frozen_dir]
         elif sys.platform.startswith("win"):
             frozen_dirs = [
                 frozen_dir,
                 os.path.normpath(os.path.join(frozen_dir, 'dynamips')),
+                os.path.normpath(os.path.join(frozen_dir, 'ubridge')),
                 os.path.normpath(os.path.join(frozen_dir, 'vpcs')),
             ]
 
         os.environ["PATH"] = os.pathsep.join(frozen_dirs) + os.pathsep + os.environ.get("PATH", "")
 
         if options.project:
             os.chdir(frozen_dir)
 
+
     def exceptionHook(exception, value, tb):
 
         if exception == KeyboardInterrupt:
             sys.exit(0)
 
         lines = traceback.format_exception(exception, value, tb)
         print("****** Exception detected, traceback information saved in {} ******".format(exception_file_path))
@@ -220,16 +222,19 @@
             raise SystemExit("Python for Windows extensions must be installed.")
 
         if not options.debug:
             try:
                 # hide the console
                 # win32console.AllocConsole()
                 console_window = win32console.GetConsoleWindow()
-                if console_window:
+                parent_window = win32gui.GetParent(console_window)
+                if not parent_window and console_window:
                     win32gui.ShowWindow(console_window, win32con.SW_HIDE)
+                elif parent_window:
+                    win32gui.ShowWindow(parent_window, win32con.SW_HIDE)
                 else:
                     log.warning("Could not get the console window")
             except win32console.error as e:
                 log.warning("Could not allocate console: {}".format(e))
 
     local_config = LocalConfig.instance()
 
@@ -261,14 +266,15 @@
     else:
         init_logger(logging.INFO, logfile)
 
     current_year = datetime.date.today().year
     log.info("GNS3 GUI version {}".format(__version__))
     log.info("Copyright (c) 2007-{} GNS3 Technologies Inc.".format(current_year))
     log.info("Application started with {}".format(" ".join(sys.argv)))
+    log.debug("PATH={}".format(os.environ["PATH"]))
 
     # update the exception file path to have it in the same directory as the settings file.
     exception_file_path = os.path.join(LocalConfig.instance().configDirectory(), exception_file_path)
 
     # We disallow to run GNS3 from outside the /Applications folder to avoid
     # issue when people run GNS3 from the .dmg
     if sys.platform.startswith("darwin") and hasattr(sys, "frozen"):
```

### Comparing `gns3-gui-3.0.0b1/gns3/main_window.py` & `gns3-gui-3.0.0b2/gns3/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         self._local_config_timer = QtCore.QTimer(self)
         self._local_config_timer.timeout.connect(local_config.checkConfigChanged)
         self._local_config_timer.start(1000)  # milliseconds
         self._template_manager = TemplateManager().instance()
         self._appliance_manager = ApplianceManager().instance()
 
         # restore the geometry and state of the main window.
+        self._save_gui_state_geometry = True
         self.restoreGeometry(QtCore.QByteArray().fromBase64(self._settings["geometry"].encode()))
         self.restoreState(QtCore.QByteArray().fromBase64(self._settings["state"].encode()))
 
         # populate the view -> docks menu
         self.uiDocksMenu.addAction(self.uiTopologySummaryDockWidget.toggleViewAction())
         self.uiDocksMenu.addAction(self.uiComputeSummaryDockWidget.toggleViewAction())
         self.uiDocksMenu.addAction(self.uiConsoleDockWidget.toggleViewAction())
@@ -247,14 +248,15 @@
         self.uiShowLayersAction.triggered.connect(self._showLayersActionSlot)
         self.uiResetPortLabelsAction.triggered.connect(self._resetPortLabelsActionSlot)
         self.uiShowPortNamesAction.triggered.connect(self._showPortNamesActionSlot)
         self.uiShowGridAction.triggered.connect(self._showGridActionSlot)
         self.uiShowReadmeAction.triggered.connect(self._showReadmeActionSlot)
         self.uiSnapToGridAction.triggered.connect(self._snapToGridActionSlot)
         self.uiLockAllAction.triggered.connect(self._lockActionSlot)
+        self.uiResetGUIStateAction.triggered.connect(self._resetGUIState)
         self.uiResetDocksAction.triggered.connect(self._resetDocksSlot)
 
         # tool menu connections
         self.uiWebUIAction.triggered.connect(self._openWebInterfaceActionSlot)
 
         # control menu connections
         self.uiStartAllAction.triggered.connect(self._startAllActionSlot)
@@ -381,14 +383,26 @@
                         item.setLocked(True)
                     elif not self.uiLockAllAction.isChecked() and item.locked():
                         item.setLocked(False)
                     if item.parentItem() is None:
                         item.updateNode()
                     item.update()
 
+    def _resetGUIState(self):
+        """
+        Reset the GUI state.
+        """
+
+        self._save_gui_state_geometry = False
+        self.close()
+        if hasattr(sys, "frozen"):
+            QtCore.QProcess.startDetached(os.path.abspath(sys.executable), sys.argv)
+        else:
+            QtWidgets.QMessageBox.information(self, "GUI state","The GUI state has been reset, please restart the application")
+
     def _resetDocksSlot(self):
         """
         Reset the dock widgets.
         """
 
         self.uiTopologySummaryDockWidget.setFloating(False)
         self.uiComputeSummaryDockWidget.setFloating(False)
@@ -1143,14 +1157,18 @@
         """
 
         key = event.key()
         # if the user is adding a link and press Escape, then cancel the link addition.
         if self.uiAddLinkAction.isChecked() and key == QtCore.Qt.Key_Escape:
             self.uiAddLinkAction.setChecked(False)
             self._addLinkActionSlot()
+        elif key == QtCore.Qt.Key_C and event.modifiers() & QtCore.Qt.ControlModifier:
+            status_bar_message = self.uiStatusBar.currentMessage()
+            if status_bar_message:
+                QtWidgets.QApplication.clipboard().setText(status_bar_message)
         else:
             super().keyPressEvent(event)
 
     def closeEvent(self, event):
         """
         Handles the event when the main window is closed.
 
@@ -1179,16 +1197,20 @@
         And project closed.
 
         :params closing: True the windows is currently closing do not try to reclose it
         """
 
         log.debug("_finish_application_closing")
 
-        self._settings["geometry"] = bytes(self.saveGeometry().toBase64()).decode()
-        self._settings["state"] = bytes(self.saveState().toBase64()).decode()
+        if self._save_gui_state_geometry:
+            self._settings["geometry"] = bytes(self.saveGeometry().toBase64()).decode()
+            self._settings["state"] = bytes(self.saveState().toBase64()).decode()
+        else:
+            self._settings["geometry"] = ""
+            self._settings["state"] = ""
         self.setSettings(self._settings)
 
         Controller.instance().stopListenNotifications()
         server = LocalServer.instance()
         server.stopLocalServer(wait=True)
 
         time_spent = "{:.0f}".format(time.time() - self._start_time)
@@ -1424,15 +1446,15 @@
         self.updateRecentFileActions()
         self._refreshVisibleWidgets()
 
         if self._settings["hide_setup_wizard"]:
             if self._open_file_at_startup:
                 self.loadPath(self._open_file_at_startup)
                 self._open_file_at_startup = None
-            elif Topology.instance().project() is None:
+            elif Topology.instance().project() is None and QtWidgets.QApplication.activeModalWidget() is None:
                 self._newProjectActionSlot()
 
     def run_later(self, counter, callback):
         """
         Run a function after X milliseconds
 
         :params counter: Time to wait before fire the callback (in milliseconds)
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/atm_switch.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/atm_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/cloud.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/cloud.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/dialogs/cloud_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/cloud_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ethernet_hub.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ethernet_hub.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ethernet_switch.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ethernet_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/frame_relay_switch.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/frame_relay_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/nat.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/nat.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/atm_switch_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/atm_switch_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/builtin_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/builtin_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/cloud_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/cloud_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/cloud_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/cloud_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/settings.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/atm_switch_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/atm_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/builtin_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/builtin_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/builtin_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/builtin_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/cloud_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/builtin/utils/tree_widget_item.py` & `gns3-gui-3.0.0b2/gns3/modules/builtin/utils/tree_widget_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/dialogs/docker_vm_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/dialogs/docker_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/docker_vm.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/docker_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/pages/docker_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/pages/docker_vm_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_vm_configuration_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         settings["console_resolution"] = self.uiConsoleResolutionComboBox.currentText()
         settings["console_http_port"] = self.uiConsoleHttpPortSpinBox.value()
         settings["console_http_path"] = self.uiHttpConsolePathLineEdit.text()
         settings["extra_hosts"] = self.uiExtraHostsTextEdit.toPlainText()
         # only tidy input here, validation is performed server side
         settings["extra_volumes"] = [ y for x in self.uiExtraVolumeTextEdit.toPlainText().split("\n") for y in [ x.strip() ] if y ]
         settings["memory"] = self.uiMaxMemorySpinBox.value()
-        settings["cpus"] = self.uiMaxCPUsDoubleSpinBox.value()
+        settings["cpus"] = round(self.uiMaxCPUsDoubleSpinBox.value(), self.uiMaxCPUsDoubleSpinBox.decimals())
 
         if not group:
             adapters = self.uiAdapterSpinBox.value()
             if node:
                 if settings["adapters"] != adapters:
                     # check if the adapters settings have changed
                     node_ports = node.ports()
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/pages/docker_vm_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_vm_preferences_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,22 +93,24 @@
         except KeyError:
             pass
         QtWidgets.QTreeWidgetItem(section_item, ["Console type:", str(docker_container["console_type"])])
         QtWidgets.QTreeWidgetItem(section_item, ["Auto start console:", "{}".format(docker_container["console_auto_start"])])
         QtWidgets.QTreeWidgetItem(section_item, ["Auxiliary console type:", str(docker_container["aux_type"])])
         QtWidgets.QTreeWidgetItem(section_item, ["Default name format:", docker_container["default_name_format"]])
         QtWidgets.QTreeWidgetItem(section_item, ["Adapters:", str(docker_container["adapters"])])
+        if docker_container["cpus"]:
+            QtWidgets.QTreeWidgetItem(section_item, ["CPUs:", str(docker_container["cpus"])])
+        if docker_container["memory"]:
+            QtWidgets.QTreeWidgetItem(section_item, ["Memory:", str(docker_container["memory"]) + " MB"])
         if docker_container["start_command"]:
             QtWidgets.QTreeWidgetItem(section_item, ["Start command:", str(docker_container["start_command"])])
         if docker_container["environment"]:
             QtWidgets.QTreeWidgetItem(section_item, ["Environment:", str(docker_container["environment"])])
-
         if docker_container["extra_hosts"]:
             QtWidgets.QTreeWidgetItem(section_item, ["Extra hosts:", str(docker_container["extra_hosts"])])
-
         if docker_container["extra_volumes"]:
             QtWidgets.QTreeWidgetItem(section_item, ["Extra volumes:", "\n".join(docker_container["extra_volumes"])])
 
         self.uiDockerVMInfoTreeWidget.expandAll()
         self.uiDockerVMInfoTreeWidget.resizeColumnToContents(0)
         self.uiDockerVMInfoTreeWidget.resizeColumnToContents(1)
         self.uiDockerVMsTreeWidget.setMaximumWidth(self.uiDockerVMsTreeWidget.sizeHintForColumn(0) + 10)
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/settings.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/docker/ui/docker_vm_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/adapters.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/adapters.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/dialogs/ios_router_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/dialogs/ios_router_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c1700.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c1700.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c2600.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c2600.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c2691.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c2691.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c3600.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3600.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c3725.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3725.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c3745.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3745.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/c7200.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c7200.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/etherswitch_router.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/etherswitch_router.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/nodes/router.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/router.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/pages/dynamips_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/dynamips_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/pages/ios_router_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/ios_router_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/pages/ios_router_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/ios_router_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/settings.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/dynamips_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/dynamips_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/ui/ios_router_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/utils/decompress_ios.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/decompress_ios.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/utils/decompress_ios_worker.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/decompress_ios_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/dynamips/wics.py` & `gns3-gui-3.0.0b2/gns3/modules/dynamips/wics.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/dialogs/iou_device_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/dialogs/iou_device_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/iou_device.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/iou_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/pages/iou_device_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_device_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/pages/iou_device_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_device_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/pages/iou_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/settings.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_device_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/iou/ui/iou_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/module.py` & `gns3-gui-3.0.0b2/gns3/modules/module.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/module_error.py` & `gns3-gui-3.0.0b2/gns3/modules/module_error.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/dialogs/qemu_image_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/qemu_image_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/dialogs/qemu_vm_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/qemu_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/pages/qemu_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/pages/qemu_vm_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_vm_configuration_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,14 +539,15 @@
             self.uiCPUThrottlingSpinBox.setValue(settings["cpu_throttling"])
         else:
             self.uiActivateCPUThrottlingCheckBox.setChecked(False)
 
         index = self.uiProcessPriorityComboBox.findText(settings["process_priority"], QtCore.Qt.MatchFixedString)
         if index != -1:
             self.uiProcessPriorityComboBox.setCurrentIndex(index)
+        self.uiQemuPathLineEdit.setText(settings["qemu_path"])
         self.uiQemuOptionsLineEdit.setText(settings["options"])
         self.uiUsageTextEdit.setPlainText(settings["usage"])
         self.uiTPMCheckBox.setChecked(settings["tpm"])
         self.uiUEFICheckBox.setChecked(settings["uefi"])
 
     def saveSettings(self, settings, node=None, group=False):
         """
@@ -648,12 +649,13 @@
         settings["cpus"] = self.uiCPUSpinBox.value()
         settings["ram"] = self.uiRamSpinBox.value()
         if self.uiActivateCPUThrottlingCheckBox.isChecked():
             settings["cpu_throttling"] = self.uiCPUThrottlingSpinBox.value()
         else:
             settings["cpu_throttling"] = 0
         settings["process_priority"] = self.uiProcessPriorityComboBox.currentText().lower()
+        settings["qemu_path"] = self.uiQemuPathLineEdit.text().strip()
         settings["options"] = self.uiQemuOptionsLineEdit.text()
         settings["usage"] = self.uiUsageTextEdit.toPlainText()
         settings["tpm"] = self.uiTPMCheckBox.isChecked()
         settings["uefi"] = self.uiUEFICheckBox.isChecked()
         return settings
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/pages/qemu_vm_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_vm_preferences_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,16 @@
                     msg = "Dynamically allocated by the controller"
                 else:
                     msg = "Manually chosen"
                 QtWidgets.QTreeWidgetItem(section_item, ["Compute:", msg])
         except KeyError:
             pass
         QtWidgets.QTreeWidgetItem(section_item, ["QEMU platform:", os.path.basename(qemu_vm["platform"])])
+        if qemu_vm["qemu_path"]:
+            QtWidgets.QTreeWidgetItem(section_item, ["Custom QEMU path:", qemu_vm["qemu_path"]])
         QtWidgets.QTreeWidgetItem(section_item, ["Console type:", qemu_vm["console_type"]])
         QtWidgets.QTreeWidgetItem(section_item, ["Auto start console:", "{}".format(qemu_vm["console_auto_start"])])
         QtWidgets.QTreeWidgetItem(section_item, ["Auxiliary console type:", qemu_vm["aux_type"]])
         QtWidgets.QTreeWidgetItem(section_item, ["CPUs:", str(qemu_vm["cpus"])])
         QtWidgets.QTreeWidgetItem(section_item, ["Memory:", "{} MB".format(qemu_vm["ram"])])
         QtWidgets.QTreeWidgetItem(section_item, ["Linked base VM:", "{}".format(qemu_vm["linked_clone"])])
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/qemu_vm.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/qemu_vm.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
                             "adapter_type": QEMU_VM_SETTINGS["adapter_type"],
                             "mac_address": QEMU_VM_SETTINGS["mac_address"],
                             "replicate_network_connection_state": QEMU_VM_SETTINGS["replicate_network_connection_state"],
                             "tpm": QEMU_VM_SETTINGS["tpm"],
                             "uefi": QEMU_VM_SETTINGS["uefi"],
                             "create_config_disk": QEMU_VM_SETTINGS["create_config_disk"],
                             "platform": QEMU_VM_SETTINGS["platform"],
+                            "qemu_path": "",
                             "on_close": QEMU_VM_SETTINGS["on_close"],
                             "cpu_throttling": QEMU_VM_SETTINGS["cpu_throttling"],
                             "process_priority": QEMU_VM_SETTINGS["process_priority"],
                             "initrd": "",
                             "kernel_image": "",
                             "initrd_md5sum": "",
                             "kernel_image_md5sum": "",
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/settings.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "mac_address": "",
     "replicate_network_connection_state": True,
     "tpm": False,
     "uefi": False,
     "create_config_disk": False,
     "on_close": "power_off",
     "platform": "x86_64",
+    "qemu_path": "",
     "cpu_throttling": 0,
     "process_priority": "normal",
     "options": "",
     "kernel_image": "",
     "initrd": "",
     "kernel_command_line": "",
     "linked_clone": True,
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_image_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_image_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_image_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_image_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui`

 * *Files 1% similar despite different names*

#### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>QemuVMConfigPageWidget</class>
   <widget class="QWidget" name="QemuVMConfigPageWidget">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>478</width>
-        <height>579</height>
+        <width>518</width>
+        <height>618</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>QEMU VM template configuration</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
@@ -892,29 +892,15 @@
               </item>
               <item>
                 <widget class="QGroupBox" name="groupBox">
                   <property name="title">
                     <string>Additional settings</string>
                   </property>
                   <layout class="QGridLayout" name="gridLayout_3">
-                    <item row="1" column="0" colspan="2">
-                      <widget class="QCheckBox" name="uiTPMCheckBox">
-                        <property name="text">
-                          <string>Enable Trusted Platform Module (TPM)</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="uiQemuOptionsLabel">
-                        <property name="text">
-                          <string>Options:</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
+                    <item row="1" column="1">
                       <widget class="QLineEdit" name="uiQemuOptionsLineEdit">
                         <property name="toolTip">
                           <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Variable replacements:&lt;/p&gt;
 &lt;ul&gt;
 &lt;li&gt;%vm-name% =VM name&lt;/li&gt;
 &lt;li&gt;%vm-id% =VM ID&lt;/li&gt;
 &lt;li&gt;%project-id% = project ID&lt;/li&gt;
@@ -922,37 +908,63 @@
 &lt;li&gt;%console-port% = console port number&lt;/li&gt;
 &lt;li&gt;%guest-cid% = unique ID from 3 to 65535&lt;/li&gt;
 &lt;/ul&gt;
 &lt;/body&gt;&lt;/html&gt;</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="3" column="0" colspan="2">
+                    <item row="4" column="0" colspan="2">
+                      <widget class="QCheckBox" name="uiUEFICheckBox">
+                        <property name="text">
+                          <string>Enable UEFI boot mode</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="5" column="0" colspan="2">
                       <widget class="QCheckBox" name="uiBaseVMCheckBox">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="text">
                           <string>Use as a linked base VM</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="2" column="0" colspan="2">
-                      <widget class="QCheckBox" name="uiUEFICheckBox">
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="uiQemuPathLabel">
                         <property name="text">
-                          <string>Enable UEFI boot mode</string>
+                          <string>Qemu binary path:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
+                      <widget class="QLabel" name="uiQemuOptionsLabel">
+                        <property name="text">
+                          <string>Command line options:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="3" column="0" colspan="2">
+                      <widget class="QCheckBox" name="uiTPMCheckBox">
+                        <property name="text">
+                          <string>Enable Trusted Platform Module (TPM)</string>
                         </property>
                       </widget>
                     </item>
+                    <item row="0" column="1">
+                      <widget class="QLineEdit" name="uiQemuPathLineEdit"/>
+                    </item>
                   </layout>
                   <zorder>uiQemuOptionsLineEdit</zorder>
                   <zorder>uiQemuOptionsLabel</zorder>
                   <zorder>uiBaseVMCheckBox</zorder>
                   <zorder>uiTPMCheckBox</zorder>
                   <zorder>uiUEFICheckBox</zorder>
+                  <zorder>uiQemuPathLabel</zorder>
+                  <zorder>uiQemuPathLineEdit</zorder>
                 </widget>
               </item>
               <item>
                 <spacer name="verticalSpacer">
                   <property name="orientation">
                     <enum>Qt::Vertical</enum>
                   </property>
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file '/home/grossmj/PycharmProjects/gns3-gui/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.9
+# Created by: PyQt5 UI code generator 5.15.6
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_QemuVMConfigPageWidget(object):
     def setupUi(self, QemuVMConfigPageWidget):
         QemuVMConfigPageWidget.setObjectName("QemuVMConfigPageWidget")
-        QemuVMConfigPageWidget.resize(478, 579)
+        QemuVMConfigPageWidget.resize(518, 618)
         self.verticalLayout = QtWidgets.QVBoxLayout(QemuVMConfigPageWidget)
         self.verticalLayout.setObjectName("verticalLayout")
         self.uiQemutabWidget = QtWidgets.QTabWidget(QemuVMConfigPageWidget)
         self.uiQemutabWidget.setObjectName("uiQemutabWidget")
         self.uiGeneralSettingsTab = QtWidgets.QWidget()
         self.uiGeneralSettingsTab.setObjectName("uiGeneralSettingsTab")
         self.gridLayout_4 = QtWidgets.QGridLayout(self.uiGeneralSettingsTab)
@@ -432,35 +432,43 @@
         self.uiProcessPriorityComboBox.addItem("")
         self.gridLayout.addWidget(self.uiProcessPriorityComboBox, 2, 1, 1, 1)
         self.verticalLayout_2.addWidget(self.uiOptimizationGroupBox)
         self.groupBox = QtWidgets.QGroupBox(self.uiAdvancedSettingsTab)
         self.groupBox.setObjectName("groupBox")
         self.gridLayout_3 = QtWidgets.QGridLayout(self.groupBox)
         self.gridLayout_3.setObjectName("gridLayout_3")
-        self.uiTPMCheckBox = QtWidgets.QCheckBox(self.groupBox)
-        self.uiTPMCheckBox.setObjectName("uiTPMCheckBox")
-        self.gridLayout_3.addWidget(self.uiTPMCheckBox, 1, 0, 1, 2)
-        self.uiQemuOptionsLabel = QtWidgets.QLabel(self.groupBox)
-        self.uiQemuOptionsLabel.setObjectName("uiQemuOptionsLabel")
-        self.gridLayout_3.addWidget(self.uiQemuOptionsLabel, 0, 0, 1, 1)
         self.uiQemuOptionsLineEdit = QtWidgets.QLineEdit(self.groupBox)
         self.uiQemuOptionsLineEdit.setObjectName("uiQemuOptionsLineEdit")
-        self.gridLayout_3.addWidget(self.uiQemuOptionsLineEdit, 0, 1, 1, 1)
+        self.gridLayout_3.addWidget(self.uiQemuOptionsLineEdit, 1, 1, 1, 1)
+        self.uiUEFICheckBox = QtWidgets.QCheckBox(self.groupBox)
+        self.uiUEFICheckBox.setObjectName("uiUEFICheckBox")
+        self.gridLayout_3.addWidget(self.uiUEFICheckBox, 4, 0, 1, 2)
         self.uiBaseVMCheckBox = QtWidgets.QCheckBox(self.groupBox)
         self.uiBaseVMCheckBox.setEnabled(True)
         self.uiBaseVMCheckBox.setObjectName("uiBaseVMCheckBox")
-        self.gridLayout_3.addWidget(self.uiBaseVMCheckBox, 3, 0, 1, 2)
-        self.uiUEFICheckBox = QtWidgets.QCheckBox(self.groupBox)
-        self.uiUEFICheckBox.setObjectName("uiUEFICheckBox")
-        self.gridLayout_3.addWidget(self.uiUEFICheckBox, 2, 0, 1, 2)
+        self.gridLayout_3.addWidget(self.uiBaseVMCheckBox, 5, 0, 1, 2)
+        self.uiQemuPathLabel = QtWidgets.QLabel(self.groupBox)
+        self.uiQemuPathLabel.setObjectName("uiQemuPathLabel")
+        self.gridLayout_3.addWidget(self.uiQemuPathLabel, 0, 0, 1, 1)
+        self.uiQemuOptionsLabel = QtWidgets.QLabel(self.groupBox)
+        self.uiQemuOptionsLabel.setObjectName("uiQemuOptionsLabel")
+        self.gridLayout_3.addWidget(self.uiQemuOptionsLabel, 1, 0, 1, 1)
+        self.uiTPMCheckBox = QtWidgets.QCheckBox(self.groupBox)
+        self.uiTPMCheckBox.setObjectName("uiTPMCheckBox")
+        self.gridLayout_3.addWidget(self.uiTPMCheckBox, 3, 0, 1, 2)
+        self.uiQemuPathLineEdit = QtWidgets.QLineEdit(self.groupBox)
+        self.uiQemuPathLineEdit.setObjectName("uiQemuPathLineEdit")
+        self.gridLayout_3.addWidget(self.uiQemuPathLineEdit, 0, 1, 1, 1)
         self.uiQemuOptionsLineEdit.raise_()
         self.uiQemuOptionsLabel.raise_()
         self.uiBaseVMCheckBox.raise_()
         self.uiTPMCheckBox.raise_()
         self.uiUEFICheckBox.raise_()
+        self.uiQemuPathLabel.raise_()
+        self.uiQemuPathLineEdit.raise_()
         self.verticalLayout_2.addWidget(self.groupBox)
         spacerItem4 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_2.addItem(spacerItem4)
         self.uiQemutabWidget.addTab(self.uiAdvancedSettingsTab, "")
         self.uiUsageTab = QtWidgets.QWidget()
         self.uiUsageTab.setObjectName("uiUsageTab")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.uiUsageTab)
@@ -562,23 +570,24 @@
         self.uiProcessPriorityComboBox.setItemText(0, _translate("QemuVMConfigPageWidget", "Realtime"))
         self.uiProcessPriorityComboBox.setItemText(1, _translate("QemuVMConfigPageWidget", "Very high"))
         self.uiProcessPriorityComboBox.setItemText(2, _translate("QemuVMConfigPageWidget", "High"))
         self.uiProcessPriorityComboBox.setItemText(3, _translate("QemuVMConfigPageWidget", "Normal"))
         self.uiProcessPriorityComboBox.setItemText(4, _translate("QemuVMConfigPageWidget", "Low"))
         self.uiProcessPriorityComboBox.setItemText(5, _translate("QemuVMConfigPageWidget", "Very low"))
         self.groupBox.setTitle(_translate("QemuVMConfigPageWidget", "Additional settings"))
-        self.uiTPMCheckBox.setText(_translate("QemuVMConfigPageWidget", "Enable Trusted Platform Module (TPM)"))
-        self.uiQemuOptionsLabel.setText(_translate("QemuVMConfigPageWidget", "Options:"))
         self.uiQemuOptionsLineEdit.setToolTip(_translate("QemuVMConfigPageWidget", "<html><head/><body><p>Variable replacements:</p>\n"
 "<ul>\n"
 "<li>%vm-name% =VM name</li>\n"
 "<li>%vm-id% =VM ID</li>\n"
 "<li>%project-id% = project ID</li>\n"
 "<li>%project-path% = project path</li>\n"
 "<li>%console-port% = console port number</li>\n"
 "<li>%guest-cid% = unique ID from 3 to 65535</li>\n"
 "</ul>\n"
 "</body></html>"))
-        self.uiBaseVMCheckBox.setText(_translate("QemuVMConfigPageWidget", "Use as a linked base VM"))
         self.uiUEFICheckBox.setText(_translate("QemuVMConfigPageWidget", "Enable UEFI boot mode"))
+        self.uiBaseVMCheckBox.setText(_translate("QemuVMConfigPageWidget", "Use as a linked base VM"))
+        self.uiQemuPathLabel.setText(_translate("QemuVMConfigPageWidget", "Qemu binary path:"))
+        self.uiQemuOptionsLabel.setText(_translate("QemuVMConfigPageWidget", "Command line options:"))
+        self.uiTPMCheckBox.setText(_translate("QemuVMConfigPageWidget", "Enable Trusted Platform Module (TPM)"))
         self.uiQemutabWidget.setTabText(self.uiQemutabWidget.indexOf(self.uiAdvancedSettingsTab), _translate("QemuVMConfigPageWidget", "Advanced"))
         self.uiQemutabWidget.setTabText(self.uiQemutabWidget.indexOf(self.uiUsageTab), _translate("QemuVMConfigPageWidget", "Usage"))
```

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/settings.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/virtualbox/virtualbox_vm.py` & `gns3-gui-3.0.0b2/gns3/modules/virtualbox/virtualbox_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/dialogs/vmware_vm_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/dialogs/vmware_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/pages/vmware_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/pages/vmware_vm_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/pages/vmware_vm_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/settings.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vmware/vmware_vm.py` & `gns3-gui-3.0.0b2/gns3/modules/vmware/vmware_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/__init__.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/pages/vpcs_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/settings.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_wizard.ui` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/modules/vpcs/vpcs_node.py` & `gns3-gui-3.0.0b2/gns3/modules/vpcs/vpcs_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/network_client.py` & `gns3-gui-3.0.0b2/gns3/network_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/node.py` & `gns3-gui-3.0.0b2/gns3/node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/nodes_dock_widget.py` & `gns3-gui-3.0.0b2/gns3/nodes_dock_widget.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/nodes_view.py` & `gns3-gui-3.0.0b2/gns3/nodes_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/packet_capture.py` & `gns3-gui-3.0.0b2/gns3/packet_capture.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/pages/controller_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/pages/controller_preferences_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from gns3.qt import QtNetwork, QtWidgets
 from ..ui.controller_preferences_page_ui import Ui_ControllerPreferencesPageWidget
 from ..topology import Topology
 from ..settings import CONTROLLER_SETTINGS, DEFAULT_CONTROLLER_HOST
 from ..dialogs.edit_compute_dialog import EditComputeDialog
 from ..local_server import LocalServer
 from ..compute_manager import ComputeManager
+from gns3.http_client import HTTPClient
+from gns3.controller import Controller
 
 
 class ControllerPreferencesPage(QtWidgets.QWidget, Ui_ControllerPreferencesPageWidget):
 
     """
     QWidget configuration page for controller preferences.
     """
@@ -50,14 +52,15 @@
 
         # connect the slots
         self.uiLocalServerToolButton.clicked.connect(self._localServerBrowserSlot)
         self.uiUbridgeToolButton.clicked.connect(self._ubridgeBrowserSlot)
         self.uiAddRemoteServerPushButton.clicked.connect(self._remoteServerAddSlot)
         self.uiDeleteRemoteServerPushButton.clicked.connect(self._remoteServerDeleteSlot)
         self.uiUpdateRemoteServerPushButton.clicked.connect(self._remoteServerUpdateSlot)
+        self.uiConnectPushButton.clicked.connect(self._connectSlot)
 
         self.uiRemoteServersTreeWidget.itemSelectionChanged.connect(self._remoteServerChangedSlot)
         self.uiRestoreDefaultsPushButton.clicked.connect(self._restoreDefaultsSlot)
         self.uiLocalServerAutoStartCheckBox.stateChanged.connect(self._useLocalServerAutoStartSlot)
 
         # load all available addresses
         for address in QtNetwork.QNetworkInterface.allAddresses():
@@ -171,14 +174,32 @@
 
         item = self.uiRemoteServersTreeWidget.currentItem()
         dialog = EditComputeDialog(self.parent(), item.compute)
         dialog.show()
         if dialog.exec_():
             self._populateRemoteServersTree()
 
+    def _connectSlot(self):
+        """
+        Connects to a remote controller.
+        """
+
+        controller_settings = {
+            "host": self.uiRemoteMainServerHostLineEdit.text(),
+            "port": self.uiRemoteMainServerPortSpinBox.value(),
+            "protocol": self.uiRemoteMainServerProtocolComboBox.currentText().lower(),
+            "username": self.uiRemoteMainServerUserLineEdit.text(),
+            "password": self.uiRemoteMainServerPasswordLineEdit.text(),
+            "remote": True
+        }
+        http_client = HTTPClient(controller_settings)
+        Controller.instance().setHttpClient(http_client)
+        if http_client.connected():
+            QtWidgets.QMessageBox.information(self, "Controller", "Successfully connected to controller {}".format(controller_settings["host"]))
+
     def _populateWidgets(self, servers_settings):
         """
         Populates the widgets with the settings.
 
         :param servers_settings: servers settings
         """
 
@@ -191,21 +212,22 @@
 
         self.uiRemoteMainServerHostLineEdit.setText(servers_settings["host"])
         self.uiRemoteMainServerPortSpinBox.setValue(servers_settings["port"])
         self.uiRemoteMainServerProtocolComboBox.setCurrentText(servers_settings["protocol"].upper())
         self.uiRemoteMainServerUserLineEdit.setText(servers_settings["username"])
         self.uiRemoteMainServerPasswordLineEdit.setText(servers_settings["password"])
 
-        #self.uiLocalServerAutoStartCheckBox.setChecked(servers_settings["auto_start"])
-        #self._useLocalServerAutoStartSlot(servers_settings["auto_start"])
-
-        # FIXME: only allow remote server (temporary)
         self.uiLocalServerAutoStartCheckBox.setChecked(False)
         self.uiLocalServerAutoStartCheckBox.setEnabled(False)
         self._useLocalServerAutoStartSlot(False)
+        if sys.platform.startswith("linux"):
+            # Local controller only supported on Linux
+            self.uiLocalServerAutoStartCheckBox.setChecked(servers_settings["auto_start"])
+            self.uiLocalServerAutoStartCheckBox.setEnabled(True)
+            self._useLocalServerAutoStartSlot(servers_settings["auto_start"])
 
         self.uiConsoleConnectionsToAnyIPCheckBox.setChecked(servers_settings["allow_console_from_anywhere"])
         self.uiDynamicComputeAllocationCheckBox.setChecked(servers_settings["dynamic_compute_allocation"])
         self.uiConsoleStartPortSpinBox.setValue(servers_settings["console_start_port_range"])
         self.uiConsoleEndPortSpinBox.setValue(servers_settings["console_end_port_range"])
         self.uiUDPStartPortSpinBox.setValue(servers_settings["udp_start_port_range"])
         self.uiUDPEndPortSpinBox.setValue(servers_settings["udp_end_port_range"])
@@ -252,14 +274,15 @@
         # save the local server preferences
         new_local_server_settings = local_server_settings.copy()
         new_local_server_settings.update({"path": self.uiLocalServerPathLineEdit.text(),
                                           "ubridge_path": self.uiUbridgePathLineEdit.text(),
                                           "host": self.uiLocalServerHostComboBox.itemData(self.uiLocalServerHostComboBox.currentIndex()),
                                           "port": self.uiLocalServerPortSpinBox.value(),
                                           "auto_start": self.uiLocalServerAutoStartCheckBox.isChecked(),
+                                          "remote": False,
                                           "allow_console_from_anywhere": self.uiConsoleConnectionsToAnyIPCheckBox.isChecked(),
                                           "dynamic_compute_allocation": self.uiDynamicComputeAllocationCheckBox.isChecked(),
                                           "console_start_port_range": self.uiConsoleStartPortSpinBox.value(),
                                           "console_end_port_range": self.uiConsoleEndPortSpinBox.value(),
                                           "udp_start_port_range": self.uiUDPStartPortSpinBox.value(),
                                           "udp_end_port_range": self.uiUDPEndPortSpinBox.value()})
 
@@ -289,14 +312,15 @@
                 LocalServer.instance().updateLocalServerSettings(new_local_server_settings)
         else:
             new_local_server_settings["host"] = self.uiRemoteMainServerHostLineEdit.text()
             new_local_server_settings["port"] = self.uiRemoteMainServerPortSpinBox.value()
             new_local_server_settings["protocol"] = self.uiRemoteMainServerProtocolComboBox.currentText().lower()
             new_local_server_settings["username"] = self.uiRemoteMainServerUserLineEdit.text()
             new_local_server_settings["password"] = self.uiRemoteMainServerPasswordLineEdit.text()
+            new_local_server_settings["remote"] = True
 
             # Some users get confused by compute and controller and
             # configure the same server twice
             for compute in self._remote_computes.values():
                 if new_local_server_settings["host"] == compute.host() and new_local_server_settings["port"] == compute.port():
                     QtWidgets.QMessageBox.critical(self, "Remote compute", "Is it not possible to use a controller as a remote compute")
                     return
```

### Comparing `gns3-gui-3.0.0b1/gns3/pages/general_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/pages/general_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/pages/gns3_vm_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/pages/gns3_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/pages/packet_capture_preferences_page.py` & `gns3-gui-3.0.0b2/gns3/pages/packet_capture_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ports/ethernet_port.py` & `gns3-gui-3.0.0b2/gns3/ports/ethernet_port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ports/port.py` & `gns3-gui-3.0.0b2/gns3/ports/port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ports/port_name_factory.py` & `gns3-gui-3.0.0b2/gns3/ports/port_name_factory.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ports/serial_port.py` & `gns3-gui-3.0.0b2/gns3/ports/serial_port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/progress.py` & `gns3-gui-3.0.0b2/gns3/progress.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/project.py` & `gns3-gui-3.0.0b2/gns3/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,17 +473,17 @@
             "show_grid": self._show_grid,
             "grid_size": self._grid_size,
             "drawing_grid_size": self._drawing_grid_size,
             "show_interface_labels": self._show_interface_labels,
             "variables": self._variables,
             "supplier": self._supplier
         }
-        self.put("", self._projectUpdatedCallback, body=body)
+        self.put("", self.projectUpdatedCallback, body=body)
 
-    def _projectUpdatedCallback(self, result, error=False, **kwargs):
+    def projectUpdatedCallback(self, result, error=False, **kwargs):
         if error:
             self.project_creation_error_signal.emit(result["message"])
             return
         self._parseResponse(result)
         self.project_updated_signal.emit()
 
     def _projectCreatedCallback(self, result, error=False, **kwargs):
@@ -723,18 +723,21 @@
             drawing = Topology.instance().getDrawingFromUuid(result["event"]["drawing_id"])
             if drawing is not None:
                 drawing.updateDrawingCallback(result["event"])
         elif result["action"] == "drawing.deleted":
             drawing = Topology.instance().getDrawingFromUuid(result["event"]["drawing_id"])
             if drawing is not None:
                 drawing.delete(skip_controller=True)
+        # project.closed and project.updated notifications have been moved to the controller
+        # because they are not project specific, keeping it there for backward compatibility
+        # when connected to an older controller version
         elif result["action"] == "project.closed":
             Topology.instance().setProject(None)
         elif result["action"] == "project.updated":
-            self._projectUpdatedCallback(result["event"])
+            self.projectUpdatedCallback(result["event"])
         elif result["action"] == "snapshot.restored":
             Topology.instance().restoreSnapshot(result["event"]["project_id"])
         elif result["action"] == "log.error":
             log.error(result["event"]["message"])
         elif result["action"] == "log.warning":
             log.warning(result["event"]["message"])
         elif result["action"] == "log.info":
```

### Comparing `gns3-gui-3.0.0b1/gns3/pycutext.py` & `gns3-gui-3.0.0b2/gns3/pycutext.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/qt/__init__.py` & `gns3-gui-3.0.0b2/gns3/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/qt/qimage_svg_renderer.py` & `gns3-gui-3.0.0b2/gns3/qt/qimage_svg_renderer.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/registry/appliance.py` & `gns3-gui-3.0.0b2/gns3/registry/appliance.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/registry/appliance_to_template.py` & `gns3-gui-3.0.0b2/gns3/registry/appliance_to_template.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/registry/config.py` & `gns3-gui-3.0.0b2/gns3/registry/config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/registry/image.py` & `gns3-gui-3.0.0b2/gns3/registry/image.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/registry/registry.py` & `gns3-gui-3.0.0b2/gns3/registry/registry.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/schemas/appliance.json` & `gns3-gui-3.0.0b2/gns3/schemas/appliance.json`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/schemas/appliance_v8.json` & `gns3-gui-3.0.0b2/gns3/schemas/appliance_v8.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999989129929315%*

 * *Differences: {"'definitions'": "{'docker_properties': {'properties': {'console_type': {'enum': {insert: [(4, "*

 * *                  "'none')]}}}}, 'qemu_properties': {'properties': {'console_type': {'enum': "*

 * *                  "{insert: [(4, 'none')]}}}}}"}*

```diff
@@ -34,15 +34,16 @@
                     "type": "string"
                 },
                 "console_type": {
                     "enum": [
                         "telnet",
                         "vnc",
                         "http",
-                        "https"
+                        "https",
+                        "none"
                     ],
                     "title": "Type of console"
                 },
                 "default_name_format": {
                     "title": "Default name format",
                     "type": "string"
                 },
@@ -365,15 +366,16 @@
                     "title": "Category of the template"
                 },
                 "console_type": {
                     "enum": [
                         "telnet",
                         "vnc",
                         "spice",
-                        "spice+agent"
+                        "spice+agent",
+                        "none"
                     ],
                     "title": "Type of console connection for the administration of the appliance"
                 },
                 "cpu_throttling": {
                     "maximum": 100,
                     "minimum": 0,
                     "title": "Throttle the CPU",
```

### Comparing `gns3-gui-3.0.0b1/gns3/settings.py` & `gns3-gui-3.0.0b2/gns3/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                                              'Royal TS V3': r'{}\code4ward.net\Royal TS V3\RTS3App.exe /connectadhoc:{{host}} /adhoctype:terminal /p:IsTelnetConnection="true" /p:ConnectionType="telnet;Telnet Connection" /p:Port="{{port}}" /p:Name="{{name}}"'.format(program_files),
                                              'Royal TS V5': r'"{}\Royal TS V5\RoyalTS.exe" /protocol:terminal /using:adhoc /uri:"{{host}}" /property:Port="{{port}}" /property:IsTelnetConnection="true" /property:Name="{{name}}"'.format(program_files_x86),
                                              'SuperPutty': r'SuperPutty.exe -telnet "{host} -P {port} -wt \"{name}\""',
                                              'SecureCRT': r'"{}\VanDyke Software\SecureCRT\SecureCRT.exe" /N "{{name}}" /T /TELNET {{host}} {{port}}'.format(program_files),
                                              'SecureCRT (personal profile)': r'"{}\AppData\Local\VanDyke Software\SecureCRT\SecureCRT.exe" /T /N "{{name}}" /TELNET {{host}} {{port}}'.format(userprofile),
                                              'TeraTerm Pro': r'"{}\teraterm\ttermpro.exe" /W="{{name}}" /M="ttstart.macro" /T=1 {{host}} {{port}}'.format(program_files_x86),
                                              'Telnet': 'telnet {host} {port}',
-                                             'Windows Terminal': 'wt.exe -w 1 new-tab --title {name} telnet {host} {port}',
+                                             'Windows Terminal': 'wt.exe -w 1 new-tab --suppressApplicationTitle --title {name} telnet {host} {port}',
                                              'Xshell 4': r'"{}\NetSarang\Xshell 4\xshell.exe" -url telnet://{{host}}:{{port}}'.format(program_files_x86),
                                              'Xshell 5': r'"{}\NetSarang\Xshell 5\xshell.exe" -url telnet://{{host}}:{{port}} -newtab {{name}}'.format(program_files_x86),
                                              'ZOC 6': r'"{}\ZOC6\zoc.exe" "/TELNET:{{host}}:{{port}}" /TABBED "/TITLE:{{name}}"'.format(program_files_x86)}
 
     # default on Windows
     if shutil.which("Solar-PuTTY.exe"):
         # Solar-Putty is the default if it is installed.
```

### Comparing `gns3-gui-3.0.0b1/gns3/spice_console.py` & `gns3-gui-3.0.0b2/gns3/spice_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/status_bar.py` & `gns3-gui-3.0.0b2/gns3/status_bar.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/style.py` & `gns3-gui-3.0.0b2/gns3/style.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/symbol.py` & `gns3-gui-3.0.0b2/gns3/symbol.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/telnet_console.py` & `gns3-gui-3.0.0b2/gns3/telnet_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/template.py` & `gns3-gui-3.0.0b2/gns3/template.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/template_manager.py` & `gns3-gui-3.0.0b2/gns3/template_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/topology.py` & `gns3-gui-3.0.0b2/gns3/topology.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,31 +221,31 @@
             project.setFilesDir(os.path.dirname(project_settings["project_path"]))
             project.setFilename(os.path.basename(project_settings["project_path"]))
 
         if "project_id" in project_settings:
             project.setId(project_settings["project_id"])
             self.setProject(project)
             project.load()
-            self._main_window.uiStatusBar.showMessage("Project loaded", 2000)
+            self._main_window.uiStatusBar.showMessage("Project loaded", 5000)
         else:
             self.setProject(project)
             project.create()
-            self._main_window.uiStatusBar.showMessage("Project created", 2000)
+            self._main_window.uiStatusBar.showMessage("Project created", 5000)
         return project
 
     def restoreSnapshot(self, project_id):
         """
         Restore a snapshot for a given project.
         """
 
         assert self._project.id() == project_id
         project = self._project
         self.setProject(project, snapshot=True)
         project.load()
-        self._main_window.uiStatusBar.showMessage("Snapshot restored", 2000)
+        self._main_window.uiStatusBar.showMessage("Snapshot restored", 5000)
 
     def loadProject(self, path):
         """
         Loads a project into GNS3.
 
         :param path: path to project file
         """
@@ -253,15 +253,15 @@
         if not Controller.instance().connected():
             self._project_to_load_path = path
             return
 
         from .project import Project
         self.setProject(Project())
         self._project.load(path)
-        self._main_window.uiStatusBar.showMessage("Project loaded {}".format(path), 2000)
+        self._main_window.uiStatusBar.showMessage("Project loaded {}".format(path), 5000)
         return True
 
     def editReadme(self):
         if self.project() is None:
             return
 
         from .dialogs.edit_project_dialog import EditProjectDialog
```

### Comparing `gns3-gui-3.0.0b1/gns3/topology_summary_view.py` & `gns3-gui-3.0.0b2/gns3/topology_summary_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/about_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/about_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/about_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/appliance_wizard.ui` & `gns3-gui-3.0.0b2/gns3/ui/appliance_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/appliance_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/appliance_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/capture_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/capture_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/capture_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/capture_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/configuration_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/configuration_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/configuration_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/console_command_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/console_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/console_command_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/console_command_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/controller_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page.ui`

 * *Files 1% similar despite different names*

#### Comparing `gns3-gui-3.0.0b1/gns3/ui/controller_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>ControllerPreferencesPageWidget</class>
   <widget class="QWidget" name="ControllerPreferencesPageWidget">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>585</width>
-        <height>791</height>
+        <width>524</width>
+        <height>824</height>
       </rect>
     </property>
     <property name="sizePolicy">
       <sizepolicy hsizetype="MinimumExpanding" vsizetype="MinimumExpanding">
         <horstretch>0</horstretch>
         <verstretch>0</verstretch>
       </sizepolicy>
@@ -284,60 +284,53 @@
               </item>
               <item>
                 <widget class="QGroupBox" name="uiRemoteMainServerGroupBox">
                   <property name="title">
                     <string>Remote controller</string>
                   </property>
                   <layout class="QGridLayout" name="gridLayout_4">
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="label_2">
-                        <property name="text">
-                          <string>Host:</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="3" column="2">
-                      <widget class="QLineEdit" name="uiRemoteMainServerUserLineEdit"/>
-                    </item>
-                    <item row="4" column="2">
-                      <widget class="QLineEdit" name="uiRemoteMainServerPasswordLineEdit">
-                        <property name="echoMode">
-                          <enum>QLineEdit::Password</enum>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="4" column="0" colspan="2">
-                      <widget class="QLabel" name="label_5">
-                        <property name="text">
-                          <string>Password:</string>
-                        </property>
-                      </widget>
-                    </item>
                     <item row="0" column="0">
                       <widget class="QLabel" name="uiRemoteMainServerProtocolLabel">
                         <property name="text">
                           <string>Protocol:</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="3" column="0">
-                      <widget class="QLabel" name="label_4">
+                    <item row="0" column="1">
+                      <widget class="QComboBox" name="uiRemoteMainServerProtocolComboBox">
+                        <item>
+                          <property name="text">
+                            <string>HTTP</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>HTTPS</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
+                      <widget class="QLabel" name="label_2">
                         <property name="text">
-                          <string>Username:</string>
+                          <string>Host:</string>
                         </property>
                       </widget>
                     </item>
+                    <item row="1" column="1">
+                      <widget class="QLineEdit" name="uiRemoteMainServerHostLineEdit"/>
+                    </item>
                     <item row="2" column="0">
                       <widget class="QLabel" name="label_3">
                         <property name="text">
                           <string>Port:</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="2" column="2">
+                    <item row="2" column="1">
                       <widget class="QSpinBox" name="uiRemoteMainServerPortSpinBox">
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Expanding" vsizetype="Preferred">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
@@ -348,30 +341,61 @@
                           <number>65535</number>
                         </property>
                         <property name="value">
                           <number>3080</number>
                         </property>
                       </widget>
                     </item>
-                    <item row="1" column="2">
-                      <widget class="QLineEdit" name="uiRemoteMainServerHostLineEdit"/>
+                    <item row="3" column="0">
+                      <widget class="QLabel" name="label_4">
+                        <property name="text">
+                          <string>Username:</string>
+                        </property>
+                      </widget>
                     </item>
-                    <item row="0" column="2">
-                      <widget class="QComboBox" name="uiRemoteMainServerProtocolComboBox">
+                    <item row="3" column="1">
+                      <widget class="QLineEdit" name="uiRemoteMainServerUserLineEdit"/>
+                    </item>
+                    <item row="4" column="0">
+                      <widget class="QLabel" name="label_5">
+                        <property name="text">
+                          <string>Password:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="4" column="1">
+                      <widget class="QLineEdit" name="uiRemoteMainServerPasswordLineEdit">
+                        <property name="echoMode">
+                          <enum>QLineEdit::Password</enum>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="5" column="0" colspan="2">
+                      <layout class="QHBoxLayout" name="horizontalLayout_7">
                         <item>
-                          <property name="text">
-                            <string>HTTP</string>
-                          </property>
+                          <spacer name="horizontalSpacer_5">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>40</width>
+                                <height>20</height>
+                              </size>
+                            </property>
+                          </spacer>
                         </item>
                         <item>
-                          <property name="text">
-                            <string>HTTPS</string>
-                          </property>
+                          <widget class="QPushButton" name="uiConnectPushButton">
+                            <property name="text">
+                              <string>&amp;Connect</string>
+                            </property>
+                          </widget>
                         </item>
-                      </widget>
+                      </layout>
                     </item>
                   </layout>
                 </widget>
               </item>
               <item>
                 <spacer name="verticalSpacer">
                   <property name="orientation">
@@ -386,16 +410,16 @@
                 </spacer>
               </item>
             </layout>
             <zorder>uiGeneralSettingsGroupBox</zorder>
             <zorder>uiConsolePortRangeGroupBox</zorder>
             <zorder>uiUDPPortRangeGroupBox</zorder>
             <zorder>uiLocalServerAutoStartCheckBox</zorder>
-            <zorder>uiRemoteMainServerGroupBox</zorder>
             <zorder>verticalSpacer</zorder>
+            <zorder>uiRemoteMainServerGroupBox</zorder>
           </widget>
           <widget class="QWidget" name="uiRemoteTabWidget">
             <property name="sizePolicy">
               <sizepolicy hsizetype="Preferred" vsizetype="MinimumExpanding">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
```

### Comparing `gns3-gui-3.0.0b1/gns3/ui/controller_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file '/home/grossmj/PycharmProjects/gns3-gui/gns3/ui/controller_preferences_page.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.9
+# Created by: PyQt5 UI code generator 5.15.6
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_ControllerPreferencesPageWidget(object):
     def setupUi(self, ControllerPreferencesPageWidget):
         ControllerPreferencesPageWidget.setObjectName("ControllerPreferencesPageWidget")
-        ControllerPreferencesPageWidget.resize(585, 791)
+        ControllerPreferencesPageWidget.resize(524, 824)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.MinimumExpanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(ControllerPreferencesPageWidget.sizePolicy().hasHeightForWidth())
         ControllerPreferencesPageWidget.setSizePolicy(sizePolicy)
         ControllerPreferencesPageWidget.setMinimumSize(QtCore.QSize(0, 0))
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(ControllerPreferencesPageWidget)
@@ -143,57 +143,65 @@
         self.horizontalLayout_4.addItem(spacerItem1)
         self.gridLayout_3.addLayout(self.horizontalLayout_4, 0, 0, 1, 1)
         self.verticalLayout.addWidget(self.uiUDPPortRangeGroupBox)
         self.uiRemoteMainServerGroupBox = QtWidgets.QGroupBox(self.uiLocalTabWidget)
         self.uiRemoteMainServerGroupBox.setObjectName("uiRemoteMainServerGroupBox")
         self.gridLayout_4 = QtWidgets.QGridLayout(self.uiRemoteMainServerGroupBox)
         self.gridLayout_4.setObjectName("gridLayout_4")
-        self.label_2 = QtWidgets.QLabel(self.uiRemoteMainServerGroupBox)
-        self.label_2.setObjectName("label_2")
-        self.gridLayout_4.addWidget(self.label_2, 1, 0, 1, 1)
-        self.uiRemoteMainServerUserLineEdit = QtWidgets.QLineEdit(self.uiRemoteMainServerGroupBox)
-        self.uiRemoteMainServerUserLineEdit.setObjectName("uiRemoteMainServerUserLineEdit")
-        self.gridLayout_4.addWidget(self.uiRemoteMainServerUserLineEdit, 3, 2, 1, 1)
-        self.uiRemoteMainServerPasswordLineEdit = QtWidgets.QLineEdit(self.uiRemoteMainServerGroupBox)
-        self.uiRemoteMainServerPasswordLineEdit.setEchoMode(QtWidgets.QLineEdit.Password)
-        self.uiRemoteMainServerPasswordLineEdit.setObjectName("uiRemoteMainServerPasswordLineEdit")
-        self.gridLayout_4.addWidget(self.uiRemoteMainServerPasswordLineEdit, 4, 2, 1, 1)
-        self.label_5 = QtWidgets.QLabel(self.uiRemoteMainServerGroupBox)
-        self.label_5.setObjectName("label_5")
-        self.gridLayout_4.addWidget(self.label_5, 4, 0, 1, 2)
         self.uiRemoteMainServerProtocolLabel = QtWidgets.QLabel(self.uiRemoteMainServerGroupBox)
         self.uiRemoteMainServerProtocolLabel.setObjectName("uiRemoteMainServerProtocolLabel")
         self.gridLayout_4.addWidget(self.uiRemoteMainServerProtocolLabel, 0, 0, 1, 1)
-        self.label_4 = QtWidgets.QLabel(self.uiRemoteMainServerGroupBox)
-        self.label_4.setObjectName("label_4")
-        self.gridLayout_4.addWidget(self.label_4, 3, 0, 1, 1)
+        self.uiRemoteMainServerProtocolComboBox = QtWidgets.QComboBox(self.uiRemoteMainServerGroupBox)
+        self.uiRemoteMainServerProtocolComboBox.setObjectName("uiRemoteMainServerProtocolComboBox")
+        self.uiRemoteMainServerProtocolComboBox.addItem("")
+        self.uiRemoteMainServerProtocolComboBox.addItem("")
+        self.gridLayout_4.addWidget(self.uiRemoteMainServerProtocolComboBox, 0, 1, 1, 1)
+        self.label_2 = QtWidgets.QLabel(self.uiRemoteMainServerGroupBox)
+        self.label_2.setObjectName("label_2")
+        self.gridLayout_4.addWidget(self.label_2, 1, 0, 1, 1)
+        self.uiRemoteMainServerHostLineEdit = QtWidgets.QLineEdit(self.uiRemoteMainServerGroupBox)
+        self.uiRemoteMainServerHostLineEdit.setObjectName("uiRemoteMainServerHostLineEdit")
+        self.gridLayout_4.addWidget(self.uiRemoteMainServerHostLineEdit, 1, 1, 1, 1)
         self.label_3 = QtWidgets.QLabel(self.uiRemoteMainServerGroupBox)
         self.label_3.setObjectName("label_3")
         self.gridLayout_4.addWidget(self.label_3, 2, 0, 1, 1)
         self.uiRemoteMainServerPortSpinBox = QtWidgets.QSpinBox(self.uiRemoteMainServerGroupBox)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.uiRemoteMainServerPortSpinBox.sizePolicy().hasHeightForWidth())
         self.uiRemoteMainServerPortSpinBox.setSizePolicy(sizePolicy)
         self.uiRemoteMainServerPortSpinBox.setMaximum(65535)
         self.uiRemoteMainServerPortSpinBox.setProperty("value", 3080)
         self.uiRemoteMainServerPortSpinBox.setObjectName("uiRemoteMainServerPortSpinBox")
-        self.gridLayout_4.addWidget(self.uiRemoteMainServerPortSpinBox, 2, 2, 1, 1)
-        self.uiRemoteMainServerHostLineEdit = QtWidgets.QLineEdit(self.uiRemoteMainServerGroupBox)
-        self.uiRemoteMainServerHostLineEdit.setObjectName("uiRemoteMainServerHostLineEdit")
-        self.gridLayout_4.addWidget(self.uiRemoteMainServerHostLineEdit, 1, 2, 1, 1)
-        self.uiRemoteMainServerProtocolComboBox = QtWidgets.QComboBox(self.uiRemoteMainServerGroupBox)
-        self.uiRemoteMainServerProtocolComboBox.setObjectName("uiRemoteMainServerProtocolComboBox")
-        self.uiRemoteMainServerProtocolComboBox.addItem("")
-        self.uiRemoteMainServerProtocolComboBox.addItem("")
-        self.gridLayout_4.addWidget(self.uiRemoteMainServerProtocolComboBox, 0, 2, 1, 1)
+        self.gridLayout_4.addWidget(self.uiRemoteMainServerPortSpinBox, 2, 1, 1, 1)
+        self.label_4 = QtWidgets.QLabel(self.uiRemoteMainServerGroupBox)
+        self.label_4.setObjectName("label_4")
+        self.gridLayout_4.addWidget(self.label_4, 3, 0, 1, 1)
+        self.uiRemoteMainServerUserLineEdit = QtWidgets.QLineEdit(self.uiRemoteMainServerGroupBox)
+        self.uiRemoteMainServerUserLineEdit.setObjectName("uiRemoteMainServerUserLineEdit")
+        self.gridLayout_4.addWidget(self.uiRemoteMainServerUserLineEdit, 3, 1, 1, 1)
+        self.label_5 = QtWidgets.QLabel(self.uiRemoteMainServerGroupBox)
+        self.label_5.setObjectName("label_5")
+        self.gridLayout_4.addWidget(self.label_5, 4, 0, 1, 1)
+        self.uiRemoteMainServerPasswordLineEdit = QtWidgets.QLineEdit(self.uiRemoteMainServerGroupBox)
+        self.uiRemoteMainServerPasswordLineEdit.setEchoMode(QtWidgets.QLineEdit.Password)
+        self.uiRemoteMainServerPasswordLineEdit.setObjectName("uiRemoteMainServerPasswordLineEdit")
+        self.gridLayout_4.addWidget(self.uiRemoteMainServerPasswordLineEdit, 4, 1, 1, 1)
+        self.horizontalLayout_7 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_7.setObjectName("horizontalLayout_7")
+        spacerItem2 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_7.addItem(spacerItem2)
+        self.uiConnectPushButton = QtWidgets.QPushButton(self.uiRemoteMainServerGroupBox)
+        self.uiConnectPushButton.setObjectName("uiConnectPushButton")
+        self.horizontalLayout_7.addWidget(self.uiConnectPushButton)
+        self.gridLayout_4.addLayout(self.horizontalLayout_7, 5, 0, 1, 2)
         self.verticalLayout.addWidget(self.uiRemoteMainServerGroupBox)
-        spacerItem2 = QtWidgets.QSpacerItem(10, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout.addItem(spacerItem2)
+        spacerItem3 = QtWidgets.QSpacerItem(10, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout.addItem(spacerItem3)
         self.uiGeneralSettingsGroupBox.raise_()
         self.uiConsolePortRangeGroupBox.raise_()
         self.uiUDPPortRangeGroupBox.raise_()
         self.uiLocalServerAutoStartCheckBox.raise_()
         self.uiRemoteMainServerGroupBox.raise_()
         self.uiServerPreferenceTabWidget.addTab(self.uiLocalTabWidget, "")
         self.uiRemoteTabWidget = QtWidgets.QWidget()
@@ -227,30 +235,30 @@
         self.uiUpdateRemoteServerPushButton.setEnabled(False)
         self.uiUpdateRemoteServerPushButton.setObjectName("uiUpdateRemoteServerPushButton")
         self.horizontalLayout_3.addWidget(self.uiUpdateRemoteServerPushButton)
         self.uiDeleteRemoteServerPushButton = QtWidgets.QPushButton(self.uiRemoteTabWidget)
         self.uiDeleteRemoteServerPushButton.setEnabled(False)
         self.uiDeleteRemoteServerPushButton.setObjectName("uiDeleteRemoteServerPushButton")
         self.horizontalLayout_3.addWidget(self.uiDeleteRemoteServerPushButton)
-        spacerItem3 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_3.addItem(spacerItem3)
+        spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_3.addItem(spacerItem4)
         self.gridLayout_5.addLayout(self.horizontalLayout_3, 1, 0, 1, 2)
-        spacerItem4 = QtWidgets.QSpacerItem(20, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.gridLayout_5.addItem(spacerItem4, 3, 0, 1, 1)
+        spacerItem5 = QtWidgets.QSpacerItem(20, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.gridLayout_5.addItem(spacerItem5, 3, 0, 1, 1)
         self.uiDynamicComputeAllocationCheckBox = QtWidgets.QCheckBox(self.uiRemoteTabWidget)
         self.uiDynamicComputeAllocationCheckBox.setObjectName("uiDynamicComputeAllocationCheckBox")
         self.gridLayout_5.addWidget(self.uiDynamicComputeAllocationCheckBox, 2, 0, 1, 1)
         self.uiRemoteServersTreeWidget.raise_()
         self.uiDynamicComputeAllocationCheckBox.raise_()
         self.uiServerPreferenceTabWidget.addTab(self.uiRemoteTabWidget, "")
         self.verticalLayout_2.addWidget(self.uiServerPreferenceTabWidget)
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        spacerItem5 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_2.addItem(spacerItem5)
+        spacerItem6 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_2.addItem(spacerItem6)
         self.uiRestoreDefaultsPushButton = QtWidgets.QPushButton(ControllerPreferencesPageWidget)
         self.uiRestoreDefaultsPushButton.setObjectName("uiRestoreDefaultsPushButton")
         self.horizontalLayout_2.addWidget(self.uiRestoreDefaultsPushButton)
         self.verticalLayout_2.addLayout(self.horizontalLayout_2)
 
         self.retranslateUi(ControllerPreferencesPageWidget)
         self.uiServerPreferenceTabWidget.setCurrentIndex(0)
@@ -284,22 +292,23 @@
         self.uiConsoleConnectionsToAnyIPCheckBox.setText(_translate("ControllerPreferencesPageWidget", "Allow console connections to any local IP address"))
         self.uiLocalServerPortLabel.setText(_translate("ControllerPreferencesPageWidget", "Port:"))
         self.uiConsolePortRangeGroupBox.setTitle(_translate("ControllerPreferencesPageWidget", "Console port range (5900 => 6000 is shared with VNC)"))
         self.uiConsolePortRangeLabel.setText(_translate("ControllerPreferencesPageWidget", "to"))
         self.uiUDPPortRangeGroupBox.setTitle(_translate("ControllerPreferencesPageWidget", "UDP tunneling port range"))
         self.uiUDPPortRangeLabel.setText(_translate("ControllerPreferencesPageWidget", "to"))
         self.uiRemoteMainServerGroupBox.setTitle(_translate("ControllerPreferencesPageWidget", "Remote controller"))
-        self.label_2.setText(_translate("ControllerPreferencesPageWidget", "Host:"))
-        self.label_5.setText(_translate("ControllerPreferencesPageWidget", "Password:"))
         self.uiRemoteMainServerProtocolLabel.setText(_translate("ControllerPreferencesPageWidget", "Protocol:"))
-        self.label_4.setText(_translate("ControllerPreferencesPageWidget", "Username:"))
-        self.label_3.setText(_translate("ControllerPreferencesPageWidget", "Port:"))
-        self.uiRemoteMainServerPortSpinBox.setSuffix(_translate("ControllerPreferencesPageWidget", " TCP"))
         self.uiRemoteMainServerProtocolComboBox.setItemText(0, _translate("ControllerPreferencesPageWidget", "HTTP"))
         self.uiRemoteMainServerProtocolComboBox.setItemText(1, _translate("ControllerPreferencesPageWidget", "HTTPS"))
+        self.label_2.setText(_translate("ControllerPreferencesPageWidget", "Host:"))
+        self.label_3.setText(_translate("ControllerPreferencesPageWidget", "Port:"))
+        self.uiRemoteMainServerPortSpinBox.setSuffix(_translate("ControllerPreferencesPageWidget", " TCP"))
+        self.label_4.setText(_translate("ControllerPreferencesPageWidget", "Username:"))
+        self.label_5.setText(_translate("ControllerPreferencesPageWidget", "Password:"))
+        self.uiConnectPushButton.setText(_translate("ControllerPreferencesPageWidget", "&Connect"))
         self.uiServerPreferenceTabWidget.setTabText(self.uiServerPreferenceTabWidget.indexOf(self.uiLocalTabWidget), _translate("ControllerPreferencesPageWidget", "Controller"))
         self.uiRemoteServersTreeWidget.headerItem().setText(0, _translate("ControllerPreferencesPageWidget", "Name"))
         self.uiRemoteServersTreeWidget.headerItem().setText(4, _translate("ControllerPreferencesPageWidget", "Username"))
         self.uiAddRemoteServerPushButton.setText(_translate("ControllerPreferencesPageWidget", "&Add"))
         self.uiUpdateRemoteServerPushButton.setText(_translate("ControllerPreferencesPageWidget", "Edit"))
         self.uiDeleteRemoteServerPushButton.setText(_translate("ControllerPreferencesPageWidget", "&Delete"))
         self.uiDynamicComputeAllocationCheckBox.setText(_translate("ControllerPreferencesPageWidget", "Allow controller to dynamically allocate computes"))
```

### Comparing `gns3-gui-3.0.0b1/gns3/ui/custom_adapters_configuration_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/custom_adapters_configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/custom_adapters_configuration_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/custom_adapters_configuration_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/doctor_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/doctor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/doctor_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/doctor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/edit_compute_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/edit_compute_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/edit_compute_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/edit_compute_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/edit_project_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/edit_project_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/edit_project_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/edit_project_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/exec_command_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/exec_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/exec_command_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/exec_command_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/export_debug_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/export_debug_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/export_debug_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/export_debug_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/export_project_wizard.ui` & `gns3-gui-3.0.0b2/gns3/ui/export_project_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/export_project_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/export_project_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/file_editor_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/file_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/file_editor_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/file_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/filter_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/filter_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/filter_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/filter_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/general_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/ui/general_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/general_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/general_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/gns3_vm_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/ui/gns3_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/gns3_vm_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/gns3_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/idlepc_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/idlepc_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/idlepc_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/idlepc_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/image_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/image_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/image_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/image_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/login_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/login_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/login_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/login_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/main_window.ui` & `gns3-gui-3.0.0b2/gns3/ui/main_window.ui`

 * *Files 0% similar despite different names*

#### Comparing `gns3-gui-3.0.0b1/gns3/ui/main_window.ui` & `gns3-gui-3.0.0b2/gns3/ui/main_window.ui`

```diff
@@ -134,14 +134,15 @@
         <addaction name="uiSnapToGridAction"/>
         <addaction name="uiShowGridAction"/>
         <addaction name="uiResetPortLabelsAction"/>
         <addaction name="uiShowPortNamesAction"/>
         <addaction name="uiShowReadmeAction"/>
         <addaction name="uiLockAllAction"/>
         <addaction name="separator"/>
+        <addaction name="uiResetGUIStateAction"/>
         <addaction name="uiResetDocksAction"/>
         <addaction name="uiDocksMenu"/>
       </widget>
       <widget class="QMenu" name="uiControlMenu">
         <property name="title">
           <string>Control</string>
         </property>
@@ -1402,14 +1403,19 @@
       </property>
     </action>
     <action name="uiResetConsoleAllAction">
       <property name="text">
         <string>Reset all console connections</string>
       </property>
     </action>
+    <action name="uiResetGUIStateAction">
+      <property name="text">
+        <string>Reset GUI state</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>GraphicsView</class>
       <extends>QGraphicsView</extends>
       <header>..graphics_view.h</header>
     </customwidget>
```

### Comparing `gns3-gui-3.0.0b1/gns3/ui/main_window_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/main_window_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file '/home/grossmj/PycharmProjects/gns3-gui/gns3/ui/main_window.ui'
 #
-# Created by: PyQt5 UI code generator 5.14.1
+# Created by: PyQt5 UI code generator 5.15.9
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
@@ -454,19 +455,18 @@
         self.uiResetConsoleAllAction = QtWidgets.QAction(MainWindow)
         self.uiResetConsoleAllAction.setObjectName("uiResetConsoleAllAction")
         self.uiImageManagementAction = QtWidgets.QAction(MainWindow)
         self.uiImageManagementAction.setIcon(icon10)
         self.uiImageManagementAction.setObjectName("uiImageManagementAction")
         self.uiResetDocksAction = QtWidgets.QAction(MainWindow)
         self.uiResetDocksAction.setObjectName("uiResetDocksAction")
-        self.uiEditReadmeAction = QtWidgets.QAction(MainWindow)
-        self.uiEditReadmeAction.setIcon(icon31)
-        self.uiEditReadmeAction.setObjectName("uiEditReadmeAction")
         self.uiResetConsoleAllAction = QtWidgets.QAction(MainWindow)
         self.uiResetConsoleAllAction.setObjectName("uiResetConsoleAllAction")
+        self.uiResetGUIStateAction = QtWidgets.QAction(MainWindow)
+        self.uiResetGUIStateAction.setObjectName("uiResetGUIStateAction")
         self.uiEditMenu.addAction(self.uiSelectAllAction)
         self.uiEditMenu.addAction(self.uiSelectNoneAction)
         self.uiEditMenu.addSeparator()
         self.uiEditMenu.addAction(self.uiSnapshotAction)
         self.uiEditMenu.addAction(self.uiPreferencesAction)
         self.uiFileMenu.addAction(self.uiNewProjectAction)
         self.uiFileMenu.addAction(self.uiOpenProjectAction)
@@ -501,14 +501,15 @@
         self.uiViewMenu.addAction(self.uiSnapToGridAction)
         self.uiViewMenu.addAction(self.uiShowGridAction)
         self.uiViewMenu.addAction(self.uiResetPortLabelsAction)
         self.uiViewMenu.addAction(self.uiShowPortNamesAction)
         self.uiViewMenu.addAction(self.uiShowReadmeAction)
         self.uiViewMenu.addAction(self.uiLockAllAction)
         self.uiViewMenu.addSeparator()
+        self.uiViewMenu.addAction(self.uiResetGUIStateAction)
         self.uiViewMenu.addAction(self.uiResetDocksAction)
         self.uiViewMenu.addAction(self.uiDocksMenu.menuAction())
         self.uiControlMenu.addAction(self.uiStartAllAction)
         self.uiControlMenu.addAction(self.uiSuspendAllAction)
         self.uiControlMenu.addAction(self.uiStopAllAction)
         self.uiControlMenu.addAction(self.uiReloadAllAction)
         self.uiControlMenu.addAction(self.uiAuxConsoleAllAction)
@@ -560,15 +561,15 @@
         self.uiAnnotationToolBar.addAction(self.uiDrawLineAction)
         self.uiAnnotationToolBar.addAction(self.uiLockAllAction)
         self.uiAnnotationToolBar.addAction(self.uiZoomInAction)
         self.uiAnnotationToolBar.addAction(self.uiZoomOutAction)
         self.uiAnnotationToolBar.addAction(self.uiScreenshotAction)
 
         self.retranslateUi(MainWindow)
-        self.uiQuitAction.triggered.connect(MainWindow.close)
+        self.uiQuitAction.triggered.connect(MainWindow.close) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
         MainWindow.setTabOrder(self.uiGraphicsView, self.uiNodesView)
         MainWindow.setTabOrder(self.uiNodesView, self.uiConsoleTextEdit)
         MainWindow.setTabOrder(self.uiConsoleTextEdit, self.uiTopologySummaryTreeWidget)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
@@ -731,17 +732,16 @@
         self.uiWebUIAction.setText(_translate("MainWindow", "Web UI - beta"))
         self.uiNewTemplateAction.setText(_translate("MainWindow", "New template"))
         self.uiEditReadmeAction.setText(_translate("MainWindow", "Edit readme"))
         self.uiEditReadmeAction.setToolTip(_translate("MainWindow", "Edit readme"))
         self.uiResetConsoleAllAction.setText(_translate("MainWindow", "Reset all console connections"))
         self.uiImageManagementAction.setText(_translate("MainWindow", "Image management"))
         self.uiResetDocksAction.setText(_translate("MainWindow", "Reset docks"))
-        self.uiEditReadmeAction.setText(_translate("MainWindow", "Edit readme"))
-        self.uiEditReadmeAction.setToolTip(_translate("MainWindow", "Edit readme"))
         self.uiResetConsoleAllAction.setText(_translate("MainWindow", "Reset all console connections"))
+        self.uiResetGUIStateAction.setText(_translate("MainWindow", "Reset GUI state"))
 from ..compute_summary_view import ComputeSummaryView
 from ..console_view import ConsoleView
 from ..graphics_view import GraphicsView
 from ..nodes_dock_widget import NodesDockWidget
 from ..nodes_view import NodesView
 from ..status_bar import StatusBar
 from ..topology_summary_view import TopologySummaryView
```

### Comparing `gns3-gui-3.0.0b1/gns3/ui/new_template_wizard.ui` & `gns3-gui-3.0.0b2/gns3/ui/new_template_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/new_template_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/new_template_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/node_info_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/node_info_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/node_info_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/node_info_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/node_properties_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/node_properties_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/node_properties_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/node_properties_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/packet_capture_preferences_page.ui` & `gns3-gui-3.0.0b2/gns3/ui/packet_capture_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/packet_capture_preferences_page_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/packet_capture_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/preferences_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/preferences_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/preferences_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/preferences_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/profile_select_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/profile_select_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/profile_select_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/profile_select_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/project_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/project_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/project_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/project_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/project_welcome_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/project_welcome_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/project_welcome_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/project_welcome_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/resources_rc.py` & `gns3-gui-3.0.0b2/gns3/ui/resources_rc.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/setup_wizard.ui` & `gns3-gui-3.0.0b2/gns3/ui/setup_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/setup_wizard_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/setup_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/show_readme_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/show_readme_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/show_readme_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/show_readme_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/snapshots_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/snapshots_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/snapshots_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/snapshots_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/style_editor_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/style_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/style_editor_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/style_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/symbol_selection_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/symbol_selection_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/symbol_selection_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/symbol_selection_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/text_editor_dialog.ui` & `gns3-gui-3.0.0b2/gns3/ui/text_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/ui/text_editor_dialog_ui.py` & `gns3-gui-3.0.0b2/gns3/ui/text_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/update_manager.py` & `gns3-gui-3.0.0b2/gns3/update_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/__init__.py` & `gns3-gui-3.0.0b2/gns3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/authorize_ubridge.py` & `gns3-gui-3.0.0b2/gns3/utils/authorize_ubridge.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/bring_to_front.py` & `gns3-gui-3.0.0b2/gns3/utils/bring_to_front.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/file_copy_worker.py` & `gns3-gui-3.0.0b2/gns3/utils/file_copy_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/get_icon.py` & `gns3-gui-3.0.0b2/gns3/utils/get_icon.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/get_resource.py` & `gns3-gui-3.0.0b2/gns3/utils/get_resource.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/import_project_worker.py` & `gns3-gui-3.0.0b2/gns3/utils/import_project_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/install_mime_types.py` & `gns3-gui-3.0.0b2/gns3/utils/install_mime_types.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/interfaces.py` & `gns3-gui-3.0.0b2/gns3/utils/interfaces.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/macos_ubridge_setuid.py` & `gns3-gui-3.0.0b2/gns3/utils/macos_ubridge_setuid.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/normalize_filename.py` & `gns3-gui-3.0.0b2/gns3/utils/normalize_filename.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/process_files_worker.py` & `gns3-gui-3.0.0b2/gns3/utils/process_files_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/progress_dialog.py` & `gns3-gui-3.0.0b2/gns3/utils/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/run_in_terminal.py` & `gns3-gui-3.0.0b2/gns3/utils/run_in_terminal.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/server_select.py` & `gns3-gui-3.0.0b2/gns3/utils/server_select.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/sudo.py` & `gns3-gui-3.0.0b2/gns3/utils/sudo.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/wait_for_command_worker.py` & `gns3-gui-3.0.0b2/gns3/utils/wait_for_command_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/wait_for_connection_worker.py` & `gns3-gui-3.0.0b2/gns3/utils/wait_for_connection_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/wait_for_lambda_worker.py` & `gns3-gui-3.0.0b2/gns3/utils/wait_for_lambda_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/utils/wait_for_runas_worker.py` & `gns3-gui-3.0.0b2/gns3/utils/wait_for_runas_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3/version.py` & `gns3-gui-3.0.0b2/gns3/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # __version_info__ is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
 
-__version__ = "3.0.0b1"
+__version__ = "3.0.0b2"
 __version_info__ = (3, 0, 0, -99)
 
 if "dev" in __version__:
     try:
         import os
         import subprocess
         if os.path.exists(os.path.join(os.path.dirname(os.path.abspath(__file__)), "..", ".git")):
```

### Comparing `gns3-gui-3.0.0b1/gns3/vnc_console.py` & `gns3-gui-3.0.0b2/gns3/vnc_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/gns3_gui.egg-info/PKG-INFO` & `gns3-gui-3.0.0b2/gns3_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gns3-gui
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: GNS3 graphical interface for the GNS3 server.
 Author-email: Jeremy Grossmann <developers@gns3.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,36 +687,33 @@
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.4
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsonschema<4.18,>=4.17.3
-Requires-Dist: sentry-sdk<1.38,==1.37.1
-Requires-Dist: psutil==5.9.6
-Requires-Dist: distro>=1.8.0
+Requires-Dist: sentry-sdk<1.41,==1.40.6
+Requires-Dist: psutil==5.9.8
+Requires-Dist: distro>=1.9.0
 Requires-Dist: truststore>=0.8.0; python_version >= "3.10"
 Requires-Dist: importlib-resources>=1.3; python_version <= "3.9"
 Provides-Extra: dev
-Requires-Dist: pytest==7.4.0; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: flake8==5.0.4; extra == "dev"
-Requires-Dist: pytest-timeout==2.1.0; extra == "dev"
+Requires-Dist: pytest-timeout==2.3.1; extra == "dev"
 
 GNS3-gui
 ========
 
 [![GitHub Actions tests](https://github.com/GNS3/gns3-gui/workflows/testing/badge.svg)](https://github.com/GNS3/gns3-gui/actions?query=workflow%3Atesting)
 [![Latest PyPi version](https://img.shields.io/pypi/v/gns3-gui.svg)](https://pypi.python.org/pypi/gns3-gui)
 [![Snyk scanning](https://snyk.io/test/github/GNS3/gns3-gui/badge.svg)](https://snyk.io/test/github/GNS3/gns3-gui)
```

### Comparing `gns3-gui-3.0.0b1/gns3_gui.egg-info/SOURCES.txt` & `gns3-gui-3.0.0b2/gns3_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/pyproject.toml` & `gns3-gui-3.0.0b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,26 @@
 name = "gns3-gui"
 description = "GNS3 graphical interface for the GNS3 server."
 license = {file = "LICENSE"}
 authors = [
   { name = "Jeremy Grossmann", email = "developers@gns3.com" }
 ]
 readme = "README.md"
-requires-python = ">=3.4"
+requires-python = ">=3.7"
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Environment :: X11 Applications :: Qt",
         "Intended Audience :: Information Technology",
         "Topic :: System :: Networking",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Operating System :: POSIX",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
 ]
```

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/add-link-1-cancel.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1-cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/add-link-1-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/add-link-1.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/add-note-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/add-note-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/add-note.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/aux-console-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/aux-console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/aux-console.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/browse-all-icons-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/browse-all-icons-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/browse-all-icons.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/browse-all-icons.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/calculate-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/calculate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/calculate.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/camera-photo-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/camera-photo.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/capture-start-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/capture-start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/capture-start.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/capture-stop-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/capture-stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/capture-stop.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/command_line-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/command_line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/command_line.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/configuration-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/configuration-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/configuration.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/console-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/console.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/console_edit-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/console_edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/console_edit.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/delete-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/delete-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/delete.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/duplicate-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/duplicate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/duplicate.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/edit-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/edit.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/ellipse-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/ellipse.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/export-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/export-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/export.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/filter-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/filter-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/filter-reset-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/filter-reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/filter-reset.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/filter.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/firewall-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/firewall-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/firewall.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/front-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/front-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/front.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/help-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/help-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/help.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/image-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/image-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/image.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/import-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/import-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/import.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/import_export_configs-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/import_export_configs-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/import_export_configs.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/inspect-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/inspect-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/inspect.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/line-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/line.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/lock-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/lock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/lock.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/lower_z_value-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/lower_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/lower_z_value.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/minus-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/minus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/minus.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/new-project-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/new-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/new-project.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/node_conception-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/node_conception-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/node_conception.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/open-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/open-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/open.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/pause-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/pause.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/pc-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/pc-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/pc.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/pc.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/plus-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/plus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/plus.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/preferences-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/preferences-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/preferences.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/quit-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/quit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/quit.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/raise_z_value-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/raise_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/raise_z_value.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/rectangle-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/rectangle.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/reload-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/reload-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/reload.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/reset-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/reset.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/router-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/router-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/router.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/save-as-project-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/save-as-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/save-as-project.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/save-project-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/save-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/save-project.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/save-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/show-hostname-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/show-hostname-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/show-hostname.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/show-interface-names-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/show-interface-names-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/show-interface-names.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/snapshot-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/snapshot-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/snapshot.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/start-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/start.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/stop-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/stop.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/switch-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/switch-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/switch.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/unlock-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/unlock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/unlock.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/zoom-in-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-in-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/zoom-in.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/zoom-out-hover.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-out-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/charcoal_icons/zoom-out.svg` & `gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/add-link-cancel.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/add-link-cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/add-link-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/add-link-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/add-link.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/add-link.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/add-note-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/add-note-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/add-note.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/aux-console-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/aux-console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/aux-console.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/browse-all-icons-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/browse-all-icons-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/browse-all-icons.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/browse-all-icons.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/calculate-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/calculate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/calculate.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/camera-photo-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/camera-photo.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/capture-start-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/capture-start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/capture-start.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/capture-stop-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/capture-stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/capture-stop.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/command_line-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/command_line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/command_line.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/configuration-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/configuration-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/configuration.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/console-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/console.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/console_edit-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/console_edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/console_edit.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/delete-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/delete-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/delete.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/duplicate-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/duplicate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/duplicate.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/edit-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/edit.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/ellipse-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/ellipse.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/export-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/export-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/export.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/filter-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/filter-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/filter-reset-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/filter-reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/filter-reset.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/filter.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/firewall-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/firewall-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/firewall.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/front-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/front-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/front.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/help-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/help-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/help.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/image-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/image-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/image.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/import-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/import-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/import.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/import_export_configs-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/import_export_configs-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/import_export_configs.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/inspect-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/inspect-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/inspect.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/line-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/line.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/lock-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/lock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/lock.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/lower_z_value-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/lower_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/lower_z_value.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/minus-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/minus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/minus.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/new-project-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/new-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/new-project.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/node_conception-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/node_conception-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/node_conception.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/open-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/open-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/open.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/pause-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/pause.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/pc-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/pc-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/pc.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/pc.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/plus-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/plus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/plus.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/preferences-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/preferences-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/preferences.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/quit-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/quit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/quit.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/raise_z_value-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/raise_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/raise_z_value.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/rectangle-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/rectangle.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/reload-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/reload-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/reload.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/reset-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/reset.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/router-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/router-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/router.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/save-as-project-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/save-as-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/save-as-project.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/save-project-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/save-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/save-project.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/save-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/show-hostname-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/show-hostname-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/show-hostname.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/show-interface-names-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/show-interface-names-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/show-interface-names.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/snapshot-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/snapshot-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/snapshot.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/start-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/start.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/stop-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/stop.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/switch-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/switch-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/switch.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/unlock-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/unlock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/unlock.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/zoom-in-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/zoom-in-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/zoom-in.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/zoom-out-hover.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/zoom-out-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/classic_icons/zoom-out.svg` & `gns3-gui-3.0.0b2/resources/classic_icons/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/PC-hover.png` & `gns3-gui-3.0.0b2/resources/icons/PC-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/PC.png` & `gns3-gui-3.0.0b2/resources/icons/PC.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/add-note.svg` & `gns3-gui-3.0.0b2/resources/icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/applications.svg` & `gns3-gui-3.0.0b2/resources/icons/applications.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/aux-console.svg` & `gns3-gui-3.0.0b2/resources/icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/browse-all-icons-hover.png` & `gns3-gui-3.0.0b2/resources/icons/browse-all-icons-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/browse-all-icons.png` & `gns3-gui-3.0.0b2/resources/icons/browse-all-icons.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/calculate.svg` & `gns3-gui-3.0.0b2/resources/icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/camera-photo-hover.svg` & `gns3-gui-3.0.0b2/resources/icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/camera-photo.svg` & `gns3-gui-3.0.0b2/resources/icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/cancel-connection.svg` & `gns3-gui-3.0.0b2/resources/icons/cancel-connection.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/cancel.svg` & `gns3-gui-3.0.0b2/resources/icons/cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/capture-start.svg` & `gns3-gui-3.0.0b2/resources/icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/capture-stop.svg` & `gns3-gui-3.0.0b2/resources/icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/command_line.svg` & `gns3-gui-3.0.0b2/resources/icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/configuration.svg` & `gns3-gui-3.0.0b2/resources/icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/connection-new-hover.svg` & `gns3-gui-3.0.0b2/resources/icons/connection-new-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/connection-new.svg` & `gns3-gui-3.0.0b2/resources/icons/connection-new.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/console.svg` & `gns3-gui-3.0.0b2/resources/icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/console_edit.svg` & `gns3-gui-3.0.0b2/resources/icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/delete.svg` & `gns3-gui-3.0.0b2/resources/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/dialog-warning.svg` & `gns3-gui-3.0.0b2/resources/icons/dialog-warning.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/drawing.svg` & `gns3-gui-3.0.0b2/resources/icons/drawing.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/duplicate.svg` & `gns3-gui-3.0.0b2/resources/icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/edit.svg` & `gns3-gui-3.0.0b2/resources/icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/ellipse-hover.svg` & `gns3-gui-3.0.0b2/resources/icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/ellipse.svg` & `gns3-gui-3.0.0b2/resources/icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/export.svg` & `gns3-gui-3.0.0b2/resources/icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/filter-capture.svg` & `gns3-gui-3.0.0b2/resources/icons/filter-capture.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/filter-reset.svg` & `gns3-gui-3.0.0b2/resources/icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/filter.svg` & `gns3-gui-3.0.0b2/resources/icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/firewall-hover.png` & `gns3-gui-3.0.0b2/resources/icons/firewall-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/firewall.png` & `gns3-gui-3.0.0b2/resources/icons/firewall.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/front.svg` & `gns3-gui-3.0.0b2/resources/icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/help.svg` & `gns3-gui-3.0.0b2/resources/icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/horizontally.svg` & `gns3-gui-3.0.0b2/resources/icons/horizontally.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/image.svg` & `gns3-gui-3.0.0b2/resources/icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/import.svg` & `gns3-gui-3.0.0b2/resources/icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/import_export_configs.svg` & `gns3-gui-3.0.0b2/resources/icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/inspect.svg` & `gns3-gui-3.0.0b2/resources/icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/led_gray.svg` & `gns3-gui-3.0.0b2/resources/icons/led_gray.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/led_green.svg` & `gns3-gui-3.0.0b2/resources/icons/led_green.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/led_red.svg` & `gns3-gui-3.0.0b2/resources/icons/led_red.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/led_yellow.svg` & `gns3-gui-3.0.0b2/resources/icons/led_yellow.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/lock.svg` & `gns3-gui-3.0.0b2/resources/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/lower_z_value.svg` & `gns3-gui-3.0.0b2/resources/icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/minus.svg` & `gns3-gui-3.0.0b2/resources/icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/new-project.svg` & `gns3-gui-3.0.0b2/resources/icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/new.svg` & `gns3-gui-3.0.0b2/resources/icons/new.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/node_conception.svg` & `gns3-gui-3.0.0b2/resources/icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/open.svg` & `gns3-gui-3.0.0b2/resources/icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/pause-hover.svg` & `gns3-gui-3.0.0b2/resources/icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/pause.svg` & `gns3-gui-3.0.0b2/resources/icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/plus.svg` & `gns3-gui-3.0.0b2/resources/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/quit.svg` & `gns3-gui-3.0.0b2/resources/icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/raise_z_value.svg` & `gns3-gui-3.0.0b2/resources/icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/rectangle-hover.svg` & `gns3-gui-3.0.0b2/resources/icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/rectangle.svg` & `gns3-gui-3.0.0b2/resources/icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/reload.svg` & `gns3-gui-3.0.0b2/resources/icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/reset.svg` & `gns3-gui-3.0.0b2/resources/icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/router-hover.png` & `gns3-gui-3.0.0b2/resources/icons/router-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/router.png` & `gns3-gui-3.0.0b2/resources/icons/router.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/rtv.png` & `gns3-gui-3.0.0b2/resources/icons/rtv.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/save-as-project.svg` & `gns3-gui-3.0.0b2/resources/icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/save-as.svg` & `gns3-gui-3.0.0b2/resources/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/save.svg` & `gns3-gui-3.0.0b2/resources/icons/save.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/show-hostname.svg` & `gns3-gui-3.0.0b2/resources/icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/show-interface-names.svg` & `gns3-gui-3.0.0b2/resources/icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/snapshot.svg` & `gns3-gui-3.0.0b2/resources/icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/start-hover.svg` & `gns3-gui-3.0.0b2/resources/icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/start.svg` & `gns3-gui-3.0.0b2/resources/icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/stop-hover.svg` & `gns3-gui-3.0.0b2/resources/icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/stop.svg` & `gns3-gui-3.0.0b2/resources/icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/switch-hover.png` & `gns3-gui-3.0.0b2/resources/icons/switch-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/switch.png` & `gns3-gui-3.0.0b2/resources/icons/switch.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/unlock.svg` & `gns3-gui-3.0.0b2/resources/icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/vertically.svg` & `gns3-gui-3.0.0b2/resources/icons/vertically.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/virtualbox.png` & `gns3-gui-3.0.0b2/resources/icons/virtualbox.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/warning.svg` & `gns3-gui-3.0.0b2/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/wireshark.png` & `gns3-gui-3.0.0b2/resources/icons/wireshark.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/zoom-in-hover.png` & `gns3-gui-3.0.0b2/resources/icons/zoom-in-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/zoom-in.png` & `gns3-gui-3.0.0b2/resources/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/zoom-out-hover.png` & `gns3-gui-3.0.0b2/resources/icons/zoom-out-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/icons/zoom-out.png` & `gns3-gui-3.0.0b2/resources/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/images/gns3.ico` & `gns3-gui-3.0.0b2/resources/images/gns3.ico`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/images/gns3_icon_128x128.png` & `gns3-gui-3.0.0b2/resources/images/gns3_icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/images/gns3_icon_256x256.png` & `gns3-gui-3.0.0b2/resources/images/gns3_icon_256x256.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/images/gns3_logo.png` & `gns3-gui-3.0.0b2/resources/images/gns3_logo.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/resources.qrc` & `gns3-gui-3.0.0b2/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/styles/charcoal.css` & `gns3-gui-3.0.0b2/resources/styles/charcoal.css`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/atm_switch.svg` & `gns3-gui-3.0.0b2/resources/symbols/atm_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/cloud.svg` & `gns3-gui-3.0.0b2/resources/symbols/cloud.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/computer.svg` & `gns3-gui-3.0.0b2/resources/symbols/computer.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/docker_guest.svg` & `gns3-gui-3.0.0b2/resources/symbols/docker_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/ethernet_switch.svg` & `gns3-gui-3.0.0b2/resources/symbols/ethernet_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/firewall.svg` & `gns3-gui-3.0.0b2/resources/symbols/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/frame_relay_switch.svg` & `gns3-gui-3.0.0b2/resources/symbols/frame_relay_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/hub.svg` & `gns3-gui-3.0.0b2/resources/symbols/hub.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/multilayer_switch.svg` & `gns3-gui-3.0.0b2/resources/symbols/multilayer_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/qemu_guest.svg` & `gns3-gui-3.0.0b2/resources/symbols/qemu_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/router.svg` & `gns3-gui-3.0.0b2/resources/symbols/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/vbox_guest.svg` & `gns3-gui-3.0.0b2/resources/symbols/vbox_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/vmware_guest.svg` & `gns3-gui-3.0.0b2/resources/symbols/vmware_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/resources/symbols/vpcs_guest.svg` & `gns3-gui-3.0.0b2/resources/symbols/vpcs_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/conftest.py` & `gns3-gui-3.0.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/items/test_ellipse_item.py` & `gns3-gui-3.0.0b2/tests/items/test_ellipse_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/items/test_image_item.py` & `gns3-gui-3.0.0b2/tests/items/test_image_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/items/test_label_item.py` & `gns3-gui-3.0.0b2/tests/items/test_label_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/items/test_line_item.py` & `gns3-gui-3.0.0b2/tests/items/test_line_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/items/test_rectangle_item.py` & `gns3-gui-3.0.0b2/tests/items/test_rectangle_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/items/test_text_item.py` & `gns3-gui-3.0.0b2/tests/items/test_text_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/modules/docker/test_docker_vm.py` & `gns3-gui-3.0.0b2/tests/modules/docker/test_docker_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/modules/dynamips/test_dynamips_init.py` & `gns3-gui-3.0.0b2/tests/modules/dynamips/test_dynamips_init.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/modules/iou/test_iou_device.py` & `gns3-gui-3.0.0b2/tests/modules/iou/test_iou_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/modules/qemu/test_qemu_vm.py` & `gns3-gui-3.0.0b2/tests/modules/qemu/test_qemu_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/modules/virtualbox/test_virtualbox_vm.py` & `gns3-gui-3.0.0b2/tests/modules/virtualbox/test_virtualbox_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/modules/vpcs/test_vpcs_device.py` & `gns3-gui-3.0.0b2/tests/modules/vpcs/test_vpcs_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/qt/test_qimage_svg_renderer.py` & `gns3-gui-3.0.0b2/tests/qt/test_qimage_svg_renderer.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/arista-veos-v8.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/arista-veos-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/arista-veos.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/arista-veos.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/broken-microcore-linux.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/broken-microcore-linux.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/cisco-3745-v8.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/cisco-3745-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/cisco-3745.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/cisco-3745.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/cisco-iou-l3-v8.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/cisco-iou-l3-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/cisco-iou-l3.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/cisco-iou-l3.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/empty-vm-v8.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/empty-vm-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/juniper-vsrx.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/juniper-vsrx.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/microcore-linux.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/microcore-linux.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/openvswitch-v8.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/openvswitch-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/appliances/openvswitch.gns3a` & `gns3-gui-3.0.0b2/tests/registry/appliances/openvswitch.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/test_appliance.py` & `gns3-gui-3.0.0b2/tests/registry/test_appliance.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,27 +125,27 @@
         "hda_disk_image": hda
     }
 
 
 def test_search_images_for_version(linux_microcore_img, microcore_appliance):
 
     detected = microcore_appliance.search_images_for_version("3.4.1")
-    assert detected["name"] == "Micro Core Linux 3.4.1"
+    assert detected["name"] == "Micro Core Linux"
     assert detected["images"][0]["type"] == "hda_disk_image"
     assert detected["images"][0]["path"] == linux_microcore_img
     assert detected["images"][0]["md5sum"] == "5d41402abc4b2a76b9719d911017c592"
     assert detected["images"][0]["filesize"] == 5
 
 
 def test_search_images_for_version_no_md5(linux_microcore_img, microcore_appliance):
 
     microcore_appliance._appliance['versions'][0]['images']['hda_disk_image'].pop('filesize')
     microcore_appliance._appliance['versions'][0]['images']['hda_disk_image'].pop('md5sum')
     detected = microcore_appliance.search_images_for_version("3.4.1")
-    assert detected["name"] == "Micro Core Linux 3.4.1"
+    assert detected["name"] == "Micro Core Linux"
     assert detected["images"][0]["type"] == "hda_disk_image"
     assert detected["images"][0]["path"] == linux_microcore_img
     assert detected["images"][0]["md5sum"] == "5d41402abc4b2a76b9719d911017c592"
     assert detected["images"][0]["filesize"] == 5
 
 
 def test_search_images_for_version_unknow_version(microcore_appliance):
```

### Comparing `gns3-gui-3.0.0b1/tests/registry/test_appliance_to_template.py` & `gns3-gui-3.0.0b2/tests/registry/test_appliance_to_template.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/test_config.py` & `gns3-gui-3.0.0b2/tests/registry/test_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/test_image.py` & `gns3-gui-3.0.0b2/tests/registry/test_image.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/registry/test_registry.py` & `gns3-gui-3.0.0b2/tests/registry/test_registry.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_compute.py` & `gns3-gui-3.0.0b2/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_compute_manager.py` & `gns3-gui-3.0.0b2/tests/test_compute_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_controller.py` & `gns3-gui-3.0.0b2/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_graphics_view.py` & `gns3-gui-3.0.0b2/tests/test_graphics_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_http_client.py` & `gns3-gui-3.0.0b2/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_image_manager.py` & `gns3-gui-3.0.0b2/tests/test_image_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_image_upload_manager.py` & `gns3-gui-3.0.0b2/tests/test_image_upload_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_link.py` & `gns3-gui-3.0.0b2/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_local_config.py` & `gns3-gui-3.0.0b2/tests/test_local_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_local_server.py` & `gns3-gui-3.0.0b2/tests/test_local_server.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_main_window.py` & `gns3-gui-3.0.0b2/tests/test_main_window.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_network_client.py` & `gns3-gui-3.0.0b2/tests/test_network_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_node.py` & `gns3-gui-3.0.0b2/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_progress.py` & `gns3-gui-3.0.0b2/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_project.py` & `gns3-gui-3.0.0b2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_spice_console.py` & `gns3-gui-3.0.0b2/tests/test_spice_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_topology.py` & `gns3-gui-3.0.0b2/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_update_manager.py` & `gns3-gui-3.0.0b2/tests/test_update_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_utils.py` & `gns3-gui-3.0.0b2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/test_vnc_console.py` & `gns3-gui-3.0.0b2/tests/test_vnc_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/utils/test_file_copy_worker.py` & `gns3-gui-3.0.0b2/tests/utils/test_file_copy_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b1/tests/utils/test_server_select.py` & `gns3-gui-3.0.0b2/tests/utils/test_server_select.py`

 * *Files identical despite different names*

