# Comparing `tmp/openlane-2.0.0b9.tar.gz` & `tmp/openlane-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlane-2.0.0b9.tar", last modified: Wed Aug 23 09:52:43 2023, max compression
+gzip compressed data, was "openlane-2.0.0rc2.tar", last modified: Sun Apr  7 19:01:48 2024, max compression
```

## Comparing `openlane-2.0.0b9.tar` & `openlane-2.0.0rc2.tar`

### file list

```diff
@@ -1,161 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.860095 openlane-2.0.0b9/
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-23 09:52:43.860095 openlane-2.0.0b9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.844095 openlane-2.0.0b9/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/design_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/drc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/generic_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/tcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/common/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21190 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/pdk_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/removals.py
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/config/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/env_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/optimizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/flows/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/open_pdks_rev
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/base.sdc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane/scripts/klayout/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/Readme.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/open_design.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4712 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/render.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6639 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/stream_out.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/klayout/xor.drc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/magic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/magic/def/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/def/antenna_check.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/def/mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2740 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/def/mag_gds.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/def/read.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/drc.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/extract_spice.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/magic/gds/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/drc_batch.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/erase_box.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/extras_mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/mag_with_pointers.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/gds/read.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/magic/lef/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/lef/extras_maglef.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/lef/maglef.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/lef.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/magic/wrapper.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.852095 openlane-2.0.0b9/openlane/scripts/odbpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/apply_def_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/contextualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/defutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/diodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/disconnected_pins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/io_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/label_macro_pins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/lefutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/manual_macro_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/padringer.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/power_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/random_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/remove_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/set_power_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/snap_to_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/odbpy/wire_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/openroad/
--rwxr-xr-x   0 runner    (1001) docker     (123)      759 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/basic_mp.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/check_antennas.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/openroad/common/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/dpl.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/dpl_cell_pad.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/io.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/pdn_cfg.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/resizer.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_global_connections.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_layer_adjustments.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_power_nets.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_rc.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/common/set_routing_layers.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/cts.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/dpl.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/drt.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/fill.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3636 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/floorplan.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/gpl.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/gui.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/insert_buffer.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/ioplacer.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/irdrop.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/pdn.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/rcx.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/repair_design.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/rsz_timing_postcts.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/rsz_timing_postgrt.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/openroad/sta/
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/sta/corner.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/sta/multi_corner.tcl.bk
--rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/tapcell.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/openroad/write_views.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/tclsh/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/tclsh/hello.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/scripts/yosys/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/yosys/common.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/yosys/json_header.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/scripts/yosys/synthesize.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/smoke_test_design/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/smoke_test_design/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/smoke_test_design/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/smoke_test_design/src/spm.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.856095 openlane-2.0.0b9/openlane/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.860095 openlane-2.0.0b9/openlane/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/common_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/klayout.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/netgen.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/odb.py
--rw-r--r--   0 runner    (1001) docker     (123)    55107 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/openroad.py
--rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/tclstep.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-08-23 09:49:46.000000 openlane-2.0.0b9/openlane/steps/yosys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.848095 openlane-2.0.0b9/openlane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-23 09:52:43.000000 openlane-2.0.0b9/openlane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-23 09:52:43.860095 openlane-2.0.0b9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1560 2023-08-23 09:49:46.000000 openlane-2.0.0b9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 09:52:43.860095 openlane-2.0.0b9/test/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-23 09:49:46.000000 openlane-2.0.0b9/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-08-23 09:49:46.000000 openlane-2.0.0b9/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.501187 openlane-2.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-07 19:01:48.501187 openlane-2.0.0rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.449187 openlane-2.0.0rc2/openlane/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.453187 openlane-2.0.0rc2/openlane/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/drc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/generic_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.453187 openlane-2.0.0rc2/openlane/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/tcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20900 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/tpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.457187 openlane-2.0.0rc2/openlane/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32144 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/pdk_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/removals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25394 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/env_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.445187 openlane-2.0.0rc2/openlane/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.457187 openlane-2.0.0rc2/openlane/examples/spm/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm/pin_order.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.461187 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/SPM_example.v
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/config-tut.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/defines.v
+-rw-r--r--   0 runner    (1001) docker     (127)   438993 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/template.def
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.465187 openlane-2.0.0rc2/openlane/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15375 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33165 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/optimizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/synth_explore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.465187 openlane-2.0.0rc2/openlane/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/open_pdks_rev
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.465187 openlane-2.0.0rc2/openlane/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/base.sdc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.469187 openlane-2.0.0rc2/openlane/scripts/klayout/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/Readme.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2151 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/open_design.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3833 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/render.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5867 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/stream_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/xml_drc_report_to_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3131 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/xor.drc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.469187 openlane-2.0.0rc2/openlane/scripts/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.469187 openlane-2.0.0rc2/openlane/scripts/magic/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/common/read.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.469187 openlane-2.0.0rc2/openlane/scripts/magic/def/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/def/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/def/mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2137 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/def/mag_gds.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2402 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/drc.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/extract_spice.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.473187 openlane-2.0.0rc2/openlane/scripts/magic/gds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2198 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/gds/drc_batch.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/gds/erase_box.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/gds/extras_mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/gds/mag_with_pointers.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/get_bbox.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.473187 openlane-2.0.0rc2/openlane/scripts/magic/lef/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/lef/extras_maglef.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/lef/maglef.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/lef.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/wrapper.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.473187 openlane-2.0.0rc2/openlane/scripts/netgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/netgen/setup.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.477187 openlane-2.0.0rc2/openlane/scripts/odbpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/apply_def_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/check_antenna_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/contextualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/defutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/diodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/disconnected_pins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/exception_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/filter_unannotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/io_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/label_macro_pins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/lefutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/manual_macro_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/power_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/random_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/remove_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/snap_to_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/wire_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.485187 openlane-2.0.0rc2/openlane/scripts/openroad/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/antenna_repair.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      788 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/basic_mp.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.489187 openlane-2.0.0rc2/openlane/scripts/openroad/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/dpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/dpl_cell_pad.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/io.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/pdn_cfg.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/resizer.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_global_connections.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_layer_adjustments.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_power_nets.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_rc.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_routing_layers.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2658 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/cts.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/cut_rows.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/dpl.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1175 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/drt.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/fill.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4849 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/floorplan.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2413 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/gpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/gui.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/insert_buffer.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1893 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/ioplacer.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/irdrop.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/pdn.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/rcx.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/repair_design.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/repair_design_postgrt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/rsz_timing_postcts.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/rsz_timing_postgrt.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.489187 openlane-2.0.0rc2/openlane/scripts/openroad/sta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/sta/check_macro_instances.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/sta/corner.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      935 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/tapcell.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      663 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/write_views.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.489187 openlane-2.0.0rc2/openlane/scripts/tclsh/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/tclsh/hello.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.489187 openlane-2.0.0rc2/openlane/scripts/yosys/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/yosys/common.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/yosys/json_header.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    14953 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/yosys/synthesize.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.493187 openlane-2.0.0rc2/openlane/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/state/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/state/design_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.497187 openlane-2.0.0rc2/openlane/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/common_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/cvc_rv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/klayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/netgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29790 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/odb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78837 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/openroad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/openroad_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/tclstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/verilator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/yosys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.449187 openlane-2.0.0rc2/openlane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:01:48.501187 openlane-2.0.0rc2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1744 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.501187 openlane-2.0.0rc2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/test/conftest.py
```

### Comparing `openlane-2.0.0b9/PKG-INFO` & `openlane-2.0.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0b9
+Version: 2.0.0rc2
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized, but some oddities are still to be expected. Proceed with caution.
         >
@@ -17,15 +17,15 @@
             <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style: black"/></a>
             <a href="https://mypy-lang.org/"><img src="https://www.mypy-lang.org/static/mypy_badge.svg" alt="Checked with mypy"/></a>
             <a href="https://nixos.org/"><img src="https://img.shields.io/static/v1?logo=nixos&logoColor=white&label=&message=Built%20with%20Nix&color=41439a" alt="Built with Nix"/></a>
         </p>
         <p align="center">
             <a href="https://colab.research.google.com/github/efabless/openlane2/blob/main/notebook.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"></a>
             <a href="https://openlane2.readthedocs.io/"><img src="https://readthedocs.org/projects/openlane2/badge/?version=latest" alt="Documentation Build Status Badge"/></a>
-            <a href="https://invite.skywater.tools"><img src="https://img.shields.io/badge/Community-Open%20Source%20Silicon%20Slack-ff69b4?logo=slack" alt="Invite to the Open Source Silicon Slack"/></a>
+            <a href="https://open-source-silicon.dev"><img src="https://img.shields.io/badge/Community-Open%20Source%20Silicon%20Slack-ff69b4?logo=slack" alt="Invite to the Open Source Silicon Slack"/></a>
         </p>
         
         OpenLane is a RTL to GDSII infrastructure library based on several components including OpenROAD, Yosys, Magic, Netgen, CVC, KLayout and a number of custom scripts for design exploration and optimization. A reference flow performs all ASIC implementation steps from RTL all the way down to GDSII.
         
         You can find the documentation [here](https://openlane2.readthedocs.io/en/latest/getting_started/) to get started. You can discuss OpenLane 2 in the [#openlane-2](https://open-source-silicon.slack.com/archives/C05M85Q5GCF) channel of the [Efabless Open Source Silicon Slack](https://invite.skywater.tools).
         
         ```python
@@ -52,22 +52,22 @@
         by following [**this link**](https://colab.research.google.com/github/efabless/openlane2/blob/main/notebook.ipynb).
         
         ## Installation
         You'll need the following:
         * Python **3.8** or higher with PIP, Venv and Tkinter
         
         ### Nix (Recommended)
-        Works for macOS and Linux (x86-64). Recommended, as it is more integrated with your filesystem and overall has less upload and download deltas.
+        Works for macOS and Linux (x86-64 and aarch64). Recommended, as it is more integrated with your filesystem and overall has less upload and download deltas.
         
-        See [Nix-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/nix_installation/index.html) in the docs.
+        See [Nix-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/common/nix_installation/index.html) in the docs for more info.
         
         ### Docker
-        Works for Windows, macOS and Linux (x86-64, aarch64 with emulation).
+        Works for Windows, macOS and Linux (x86-64 and aarch64).
         
-        See [Docker-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/docker_installation/index.html) in the docs.
+        See [Docker-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/common/docker_installation/index.html) in the docs for more info.
         
         Do note you'll need to add `--dockerized` right after `openlane` in most CLI invocations.
         
         ### Python-only Installation (Advanced)
         You'll need to bring your own compiled utilities, but otherwise, simply install OpenLane as follows:
         
         ```sh
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0b9 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0rc2 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized,
 but some oddities are still to be expected. Proceed with caution. > > If you
 *don't* know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ************ OOppeennLLaannee ************
@@ -21,27 +21,27 @@
 from openlane.flows import Flow Classic = Flow.factory.get("Classic") flow =
 Classic( { "PDK": "sky130A", "DESIGN_NAME": "spm", "VERILOG_FILES": ["./src/
 spm.v"], "CLOCK_PORT": "clk", "CLOCK_PERIOD": 10, }, design_dir=".", )
 flow.start() ``` ## Try it out You can try OpenLane right in your browser,
 free-of-charge, using Google Colaboratory by following [**this link**](https://
 colab.research.google.com/github/efabless/openlane2/blob/main/notebook.ipynb).
 ## Installation You'll need the following: * Python **3.8** or higher with PIP,
-Venv and Tkinter ### Nix (Recommended) Works for macOS and Linux (x86-64).
-Recommended, as it is more integrated with your filesystem and overall has less
-upload and download deltas. See [Nix-based installation](https://
-openlane2.readthedocs.io/en/latest/getting_started/nix_installation/index.html)
-in the docs. ### Docker Works for Windows, macOS and Linux (x86-64, aarch64
-with emulation). See [Docker-based installation](https://
-openlane2.readthedocs.io/en/latest/getting_started/docker_installation/
-index.html) in the docs. Do note you'll need to add `--dockerized` right after
-`openlane` in most CLI invocations. ### Python-only Installation (Advanced)
-You'll need to bring your own compiled utilities, but otherwise, simply install
-OpenLane as follows: ```sh python3 -m pip install --upgrade openlane ``` ##
-Usage In the root folder of the repository, you may invoke: ```sh python3 -
-m openlane --pdk-root
+Venv and Tkinter ### Nix (Recommended) Works for macOS and Linux (x86-64 and
+aarch64). Recommended, as it is more integrated with your filesystem and
+overall has less upload and download deltas. See [Nix-based installation]
+(https://openlane2.readthedocs.io/en/latest/getting_started/common/
+nix_installation/index.html) in the docs for more info. ### Docker Works for
+Windows, macOS and Linux (x86-64 and aarch64). See [Docker-based installation]
+(https://openlane2.readthedocs.io/en/latest/getting_started/common/
+docker_installation/index.html) in the docs for more info. Do note you'll need
+to add `--dockerized` right after `openlane` in most CLI invocations. ###
+Python-only Installation (Advanced) You'll need to bring your own compiled
+utilities, but otherwise, simply install OpenLane as follows: ```sh python3 -
+m pip install --upgrade openlane ``` ## Usage In the root folder of the
+repository, you may invoke: ```sh python3 -m openlane --pdk-root
 o/pdk>
 o/config.json> ``` To start with, you can try: ```sh python3 -m openlane --pdk-
 root $HOME/.volare ./designs/spm/config.json ``` ## Publication If you use
 OpenLane in your research, please cite the following paper. * M. Shalan and T.
 Edwards, âBuilding OpenLANE: A 130nm OpenROAD-based Tapeout-Proven Flow:
 Invited Paper,â *2020 IEEE/ACM International Conference On Computer Aided
 Design (ICCAD)*, San Diego, CA, USA, 2020, pp. 1-6. [Paper](https://
```

### Comparing `openlane-2.0.0b9/openlane/__init__.py` & `openlane-2.0.0rc2/openlane/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,7 +31,8 @@
     .. data:: discovered_plugins
 
         A dictionary of detected OpenLane plugins, with the module name as a key and
         the module version as a version.
 """
 from .plugins import discovered_plugins
 from .__version__ import __version__
+from .env_info import env_info_cli
```

### Comparing `openlane-2.0.0b9/openlane/__main__.py` & `openlane-2.0.0rc2/openlane/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,27 +16,24 @@
 import shutil
 import marshal
 import tempfile
 import traceback
 import subprocess
 from textwrap import dedent
 from functools import partial
-from typing import Tuple, Type, Optional, List, Union
+from typing import Sequence, Tuple, Type, Optional, List, Union
 
-from click import Parameter, pass_context
+from click import Parameter, pass_context, Path
 from cloup import (
     option,
     option_group,
     command,
     Context,
 )
 from cloup.constraints import (
-    If,
-    IsSet,
-    accept_none,
     mutually_exclusive,
 )
 
 
 from .__version__ import __version__
 from .state import State
 from .logging import (
@@ -44,106 +41,126 @@
     err,
     warn,
     info,
 )
 from . import common
 from .container import run_in_container
 from .plugins import discovered_plugins
-from .config import Config, InvalidConfig
+from .config import Config, InvalidConfig, PassedDirectoryError
 from .common.cli import formatter_settings
 from .flows import Flow, SequentialFlow, FlowException, FlowError, cloup_flow_opts
 
 
 def run(
     ctx: Context,
     flow_name: Optional[str],
     pdk_root: Optional[str],
     pdk: str,
     scl: Optional[str],
-    config_files: List[str],
+    config_files: Sequence[str],
     tag: Optional[str],
     last_run: bool,
     frm: Optional[str],
     to: Optional[str],
     skip: Tuple[str, ...],
     reproducible: Optional[str],
     with_initial_state: Optional[State],
     config_override_strings: List[str],
-) -> int:
+    _force_run_dir: Optional[str],
+    design_dir: Optional[str],
+    view_save_path: Optional[str] = None,
+    ef_view_save_path: Optional[str] = None,
+):
+    try:
+        if len(config_files) == 0:
+            err("No config file(s) have been provided.")
+            ctx.exit(1)
 
-    config_file = config_files[0]
+        flow_description: Optional[Union[str, List[str]]] = None
 
-    # Enforce Mutual Exclusion
+        for config_file in config_files:
+            if meta := Config.get_meta(config_file, flow_override=flow_name):
+                if flow_ids := meta.flow:
+                    if flow_description is None:
+                        flow_description = flow_ids
 
-    flow_description: Union[str, List[str]] = flow_name or "Classic"
+        if flow_name is not None:
+            flow_description = flow_name
 
-    if meta := Config.get_meta(config_file, flow_override=flow_name):
-        if flow_ids := meta.flow:
-            flow_description = flow_ids
+        if flow_description is None:
+            flow_description = "Classic"
 
-    TargetFlow: Type[Flow]
+        TargetFlow: Type[Flow]
 
-    if not isinstance(flow_description, str):
-        TargetFlow = SequentialFlow.make(flow_description)
-    else:
-        if FlowClass := Flow.factory.get(flow_description):
-            TargetFlow = FlowClass
+        if not isinstance(flow_description, str):
+            TargetFlow = SequentialFlow.make(flow_description)
         else:
-            err(
-                f"Unknown flow '{flow_description}' specified in configuration file's 'meta' object."
-            )
-            return -1
+            if FlowClass := Flow.factory.get(flow_description):
+                TargetFlow = FlowClass
+            else:
+                err(
+                    f"Unknown flow '{flow_description}' specified in configuration file's 'meta' object."
+                )
+                ctx.exit(1)
 
-    try:
         flow = TargetFlow(
-            config_file,
+            config_files,
             pdk_root=pdk_root,
             pdk=pdk,
             scl=scl,
             config_override_strings=config_override_strings,
+            design_dir=design_dir,
+        )
+    except PassedDirectoryError as e:
+        err(e)
+        info(
+            f"If you meant to pass this as a design directory alongside valid configuration files, pass it as '--design-dir {e.config}'."
         )
+        ctx.exit(1)
     except InvalidConfig as e:
-        info(f"[green]Errors have occurred while loading the {e.config}.")
-        for error in e.errors:
-            err(error)
-
         if len(e.warnings) > 0:
-            info("The following warnings have also been generated:")
+            warn("The following warnings have been generated:")
             for warning in e.warnings:
                 warn(warning)
-        info("OpenLane will now quit. Please check your configuration.")
-        return 1
+        err(f"Errors have occurred while loading the {e.config}.")
+        for error in e.errors:
+            err(error)
+
+        err("OpenLane will now quit. Please check your configuration.")
+        ctx.exit(1)
     except ValueError as e:
         err(e)
         debug(traceback.format_exc())
-        info("OpenLane will now quit.")
-        return 1
+        err("OpenLane will now quit.")
+        ctx.exit(1)
 
     try:
-        flow.start(
+        state_out = flow.start(
             tag=tag,
             last_run=last_run,
             frm=frm,
             to=to,
             skip=skip,
             with_initial_state=with_initial_state,
             reproducible=reproducible,
+            _force_run_dir=_force_run_dir,
         )
     except FlowException as e:
-        err(f"The flow has encountered an unexpected error: {e}")
-        traceback.print_exc()
+        err(f"The flow has encountered an unexpected error:\n{e}")
         err("OpenLane will now quit.")
-        return 1
+        ctx.exit(1)
     except FlowError as e:
-        if "deferred" not in str(e):
-            err(f"The following error was encountered while running the flow: {e}")
+        err(f"The following error was encountered while running the flow:\n{e}")
         err("OpenLane will now quit.")
-        return 2
+        ctx.exit(2)
 
-    return 0
+    if vsp := view_save_path:
+        state_out.save_snapshot(vsp)
+    if evsp := ef_view_save_path:
+        flow._save_snapshot_ef(evsp)
 
 
 def print_version(ctx: Context, param: Parameter, value: bool):
     if not value:
         return
 
     message = dedent(
@@ -176,74 +193,89 @@
 ):
     if not value:
         return
     print(__version__, end="")
     ctx.exit(0)
 
 
-def run_smoke_test(
+def run_example(
     ctx: Context,
     param: Parameter,
-    value: bool,
+    value: Union[str, bool],
 ):
     if not value:
         return
 
+    if isinstance(value, bool):
+        value = "spm"
+
+    example_path = os.path.join(common.get_openlane_root(), "examples", value)
+    if not os.path.isdir(example_path):
+        print(f"Unknown example '{value}'.", file=sys.stderr)
+        ctx.exit(1)
+
     status = 0
-    d = tempfile.mkdtemp("openlane2")
-    final_path = os.path.join(d, "smoke_test_design")
+    final_path = os.path.join(os.getcwd(), value)
+    cleanup = False
+    if param.name == "smoke_test":
+        d = tempfile.mkdtemp("openlane2")
+        final_path = os.path.join(d, "smoke_test_design")
+        cleanup = True
     try:
+        if os.path.isdir(final_path):
+            print(f"A directory named {value} already exists.", file=sys.stderr)
+            ctx.exit(1)
         # 1. Copy the files
         shutil.copytree(
-            os.path.join(common.get_openlane_root(), "smoke_test_design"),
+            example_path,
             final_path,
             symlinks=False,
         )
 
         # 2. Make files writable
         if os.name == "posix":
-            subprocess.check_call(["chmod", "-R", "777", final_path])
+            subprocess.check_call(["chmod", "-R", "755", final_path])
 
         pdk_root = ctx.params.get("pdk_root")
         if ctx.obj["use_volare"]:
             import volare
 
-            pdk_root = volare.get_volare_home(ctx.params.get("pdk_root"))
-            common.mkdirp(pdk_root)
-            volare.enable(pdk_root, "sky130", common.get_opdks_rev())
+            volare_home = volare.get_volare_home(ctx.params.get("pdk_root"))
+            fetched = volare.fetch(volare_home, "sky130", common.get_opdks_rev())
+            pdk_root = fetched.get_dir(volare_home)
 
         config_file = os.path.join(final_path, "config.json")
 
         # 3. Run
-        status = run(
+        run(
             ctx,
             flow_name=None,
             pdk_root=pdk_root,
             pdk="sky130A",
             scl=None,
             config_files=[config_file],
             tag=None,
             last_run=False,
             frm=None,
             to=None,
             reproducible=None,
             skip=(),
             with_initial_state=None,
             config_override_strings=[],
+            _force_run_dir=None,
+            design_dir=None,
         )
-        if status == 0:
-            info("Smoke test passed.")
-        else:
-            err("Smoke test failed.")
+        info("Smoke test passed.")
     except KeyboardInterrupt:
         info("Smoke test aborted.")
         status = -1
     finally:
         try:
-            shutil.rmtree(final_path)
+            if cleanup:
+                shutil.rmtree(final_path)
         except FileNotFoundError:
             pass
 
     ctx.exit(status)
 
 
 def cli_in_container(
@@ -252,30 +284,36 @@
     value: bool,
 ):
     if not value:
         return
 
     status = 0
     docker_mounts = list(ctx.params.get("docker_mounts") or ())
+    docker_tty: bool = ctx.params.get("docker_tty", True)
     pdk_root = ctx.params.get("pdk_root")
     argv = sys.argv[sys.argv.index("--dockerized") + 1 :]
 
     interactive = True
     final_argv = ["zsh"]
     if len(argv) != 0:
         final_argv = ["openlane"] + argv
         interactive = False
 
+    docker_image = os.getenv(
+        "OPENLANE_IMAGE_OVERRIDE", f"ghcr.io/efabless/openlane2:{__version__}"
+    )
+
     try:
         status = run_in_container(
-            f"ghcr.io/efabless/openlane2:{__version__}",
+            docker_image,
             final_argv,
             pdk_root=pdk_root,
             other_mounts=docker_mounts,
             interactive=interactive,
+            tty=docker_tty,
         )
     except ValueError as e:
         print(e)
         status = -1
     except Exception:
         traceback.print_exc()
         status = -1
@@ -287,33 +325,55 @@
 
 
 @command(
     no_args_is_help=True,
     formatter_settings=formatter_settings,
 )
 @option_group(
+    "Copy final views",
+    o(
+        "--save-views-to",
+        "view_save_path",
+        type=Path(file_okay=False, dir_okay=True),
+        default=None,
+        help="A directory to copy the final views to, where each format is saved under a directory named after the corner ID (much like the 'final' directory after running a flow.)",
+    ),
+    o(
+        "--ef-save-views-to",
+        "ef_view_save_path",
+        type=Path(file_okay=False, dir_okay=True),
+        default=None,
+        help="A directory to copy the final views to in the Efabless format, compatible with Caravel User Project.",
+    ),
+)
+@option_group(
     "Containerization options",
     o(
         "--docker-mount",
         "-m",
         "docker_mounts",
         multiple=True,
-        is_eager=True,  # docker mount, dockerized should be processed before anything else
-        default=[],
-        help="Additionally mount this directory in dockerized mode. Can be supplied multiple times to mount multiple directories. Must be passed before --dockerized.",
+        is_eager=True,  # docker options should be processed before anything else
+        default=(),
+        help="Used to mount more directories in dockerized mode. If a valid directory is specified, it will be mounted in the same path in the container. Otherwise, the value of the option will be passed to the Docker-compatible container engine verbatim. Must be passed before --dockerized, has no effect if --dockerized is not set.",
+    ),
+    o(
+        "--docker-tty/--docker-no-tty",
+        is_eager=True,  # docker options should be processed before anything else
+        default=True,
+        help="Controls the allocation of a virtual terminal by passing -t to the Docker-compatible container engine invocation. Must be passed before --dockerized, has no effect if --dockerized is not set.",
     ),
     o(
         "--dockerized",
         default=False,
         is_flag=True,
-        is_eager=True,  # docker mount, dockerized should be processed before anything else
-        help="Re-invoke using a Docker container. Some caveats apply. Must precede all options except --docker-mount.",
+        is_eager=True,  # ddocker options should be processed before anything else
+        help="Run the remaining flags using a Docker container. Some caveats apply. Must precede all options except --docker-mount, --docker-tty/--docker-no-tty.",
         callback=cli_in_container,
     ),
-    constraint=If(~IsSet("dockerized"), accept_none),
 )
 @option_group(
     "Subcommands",
     o(
         "--version",
         is_flag=True,
         is_eager=True,
@@ -326,20 +386,26 @@
         is_eager=True,
         callback=print_bare_version,
         hidden=True,
     ),
     o(
         "--smoke-test",
         is_flag=True,  # Cannot be eager- PDK options need to be processed
-        help="Runs a basic OpenLane smoke test.",
-        callback=run_smoke_test,
+        help="Runs a basic OpenLane smoke test, the results of which are temporary and discarded.",
+        callback=run_example,
+    ),
+    o(
+        "--run-example",
+        default=None,  # Cannot be eager- PDK options need to be processed
+        help="Copies one of the OpenLane examples to the current working directory and runs it.",
+        callback=run_example,
     ),
     constraint=mutually_exclusive,
 )
-@cloup_flow_opts(sequential_flow_reproducible=True)
+@cloup_flow_opts(_enable_debug_flags=True, sequential_flow_reproducible=True)
 @pass_context
 def cli(ctx, /, **kwargs):
     """
     Runs an OpenLane flow via the commandline using a design configuration
     object.
 
     Try 'python3 -m openlane.steps --help' for step-specific options, including
@@ -349,21 +415,23 @@
     run_kwargs = kwargs.copy()
 
     if len(args) == 1 and args[0].endswith(".marshalled"):
         run_kwargs = marshal.load(open(args[0], "rb"))
         run_kwargs.update(**{k: kwargs[k] for k in ["pdk_root", "pdk", "scl"]})
 
     for subcommand_flag in [
+        "docker_tty",
         "docker_mounts",
         "dockerized",
         "version",
         "bare_version",
         "smoke_test",
+        "run_example",
     ]:
         if subcommand_flag in run_kwargs:
             del run_kwargs[subcommand_flag]
-
-    ctx.exit(run(ctx, **run_kwargs))
+    run(ctx, **run_kwargs)
+    ctx.exit(0)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `openlane-2.0.0b9/openlane/__version__.py` & `openlane-2.0.0rc2/openlane/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "2.0.0b9"
+__version__ = "2.0.0rc2"
 
 if __name__ == "__main__":
     print(__version__, end="")
```

### Comparing `openlane-2.0.0b9/openlane/common/__init__.py` & `openlane-2.0.0rc2/openlane/common/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,58 +14,46 @@
 """
 Common Utilities Module
 -----------------------
 
 A number of common utility functions and classes used throughout the codebase.
 """
 import os
-from concurrent.futures import ThreadPoolExecutor
 
 from .tcl import TclUtils
 from .metrics import parse_metric_modifiers, aggregate_metrics
-from .design_format import DesignFormat, DesignFormatObject
+from . import metrics
 from .generic_dict import (
     GenericDictEncoder,
     GenericDict,
     GenericImmutableDict,
     copy_recursive,
-    is_string,
 )
 from .misc import (
     idem,
     get_openlane_root,
     get_script_dir,
     get_opdks_rev,
     slugify,
     protected,
     final,
     mkdirp,
-    StringEnum,
-    Path,
     zip_first,
+    format_size,
+    format_elapsed_time,
+    Filter,
+    get_latest_file,
+    process_list_file,
+)
+from .types import (
+    is_number,
+    is_string,
+    Number,
+    Path,
+    AnyPath,
+    ScopedFile,
 )
 from .toolbox import Toolbox
 from .drc import DRC, Violation
-
-
-## TPE
-
-TPE = ThreadPoolExecutor(max_workers=os.cpu_count())
-
-
-def set_tpe(tpe: ThreadPoolExecutor):
-    """
-    Allows replacing OpenLane's global ``ThreadPoolExecutor`` with a customized
-    one.
-
-    :param tpe: The replacemend ThreadPoolExecutor
-    """
-    global TPE
-    TPE = tpe
-
-
-def get_tpe() -> ThreadPoolExecutor:
-    """
-    :returns: OpenLane's global ``ThreadPoolExecutor``
-    """
-    global TPE
-    return TPE
+from . import cli
+from .tpe import get_tpe, set_tpe
+from .ring_buffer import RingBuffer
```

### Comparing `openlane-2.0.0b9/openlane/common/cli.py` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/dpl.tcl`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-# Copyright 2023 Efabless Corporation
+# Copyright 2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from cloup import (
-    HelpFormatter,
-    HelpTheme,
-    Style,
-)
+source $::env(SCRIPTS_DIR)/openroad/common/dpl_cell_pad.tcl
 
-formatter_settings = HelpFormatter.settings(
-    theme=HelpTheme(
-        invoked_command=Style(fg="bright_yellow"),
-        heading=Style(fg="cyan", bold=True),
-        constraint=Style(fg="magenta"),
-        col1=Style(fg="bright_yellow"),
-    )
-)
+remove_fillers
+
+detailed_placement\
+    -max_displacement [subst { $::env(PL_MAX_DISPLACEMENT_X) $::env(PL_MAX_DISPLACEMENT_Y) }]
+
+if { [info exists ::env(PL_OPTIMIZE_MIRRORING)] && $::env(PL_OPTIMIZE_MIRRORING) } {
+    optimize_mirroring
+}
+check_placement -verbose
```

### Comparing `openlane-2.0.0b9/openlane/common/design_format.py` & `openlane-2.0.0rc2/openlane/state/design_format.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,25 +40,43 @@
         "Verilog Netlist",
     )
     POWERED_NETLIST: DesignFormatObject = DesignFormatObject(
         "pnl",
         "pnl.v",
         "Powered Verilog Netlist",
     )
+    POWERED_NETLIST_SDF_FRIENDLY: DesignFormatObject = DesignFormatObject(
+        "pnl-sdf-friendly",
+        "pnl-sdf.v",
+        "Powered Verilog Netlist For SDF Simulation (Without Fill Cells)",
+        folder_override="pnl",
+    )
+    POWERED_NETLIST_NO_PHYSICAL_CELLS: DesignFormatObject = DesignFormatObject(
+        "pnl-npc",
+        "pnl-npc.v",
+        "Powered Verilog Netlist Without Physical Cells (Fill Cells and Diode Cells)",
+        folder_override="pnl",
+    )
 
     DEF: DesignFormatObject = DesignFormatObject(
         "def",
         "def",
         "Design Exchange Format",
     )
     LEF: DesignFormatObject = DesignFormatObject(
         "lef",
         "lef",
         "Library Exchange Format",
     )
+    OPENROAD_LEF: DesignFormatObject = DesignFormatObject(
+        "openroad-lef",
+        "openroad.lef",
+        "Library Exchange Format Generated by OpenROAD",
+        folder_override="lef",
+    )
     ODB: DesignFormatObject = DesignFormatObject(
         "odb",
         "odb",
         "OpenDB Database",
     )
 
     SDC: DesignFormatObject = DesignFormatObject(
@@ -86,14 +104,20 @@
     )
     SPICE: DesignFormatObject = DesignFormatObject(
         "spice",
         "spice",
         "Simulation Program with Integrated Circuit Emphasis",
     )
 
+    MAG: DesignFormatObject = DesignFormatObject(
+        "mag",
+        "mag",
+        "Magic VLSI View",
+    )
+
     GDS: DesignFormatObject = DesignFormatObject(
         "gds",
         "gds",
         "GDSII Stream",
     )
     MAG_GDS: DesignFormatObject = DesignFormatObject(
         "mag_gds",
@@ -107,14 +131,19 @@
     )
 
     JSON_HEADER: DesignFormatObject = DesignFormatObject(
         "json_h",
         "h.json",
         "Design JSON Header File",
     )
+    VERILOG_HEADER: DesignFormatObject = DesignFormatObject(
+        "vh",
+        "vh",
+        "Verilog Header",
+    )
 
     def __str__(self) -> str:
         return self.value.id
 
     @staticmethod
     def by_id(id: str) -> Optional["DesignFormat"]:
         return _designformat_by_id.get(id)
```

### Comparing `openlane-2.0.0b9/openlane/common/drc.py` & `openlane-2.0.0rc2/openlane/common/drc.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                 with xf.element("items"):
                     for _, violation in self.violations.items():
                         for bounding_box in violation.bounding_boxes:
                             with xf.element("item"):
                                 cell = ET.Element("cell")
                                 cell.text = self.module
                                 category = ET.Element("category")
-                                category.text = violation.category_name
+                                category.text = f"'{violation.category_name}'"
                                 visited = ET.Element("visited")
                                 visited.text = "false"
                                 multiplicity = ET.Element("multiplicity")
                                 multiplicity.text = "1"
                                 xf.write(cell, category, visited, multiplicity)
                                 with xf.element("values"):
                                     llx, lly, urx, ury = bounding_box
```

### Comparing `openlane-2.0.0b9/openlane/common/generic_dict.py` & `openlane-2.0.0rc2/openlane/common/generic_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,33 +9,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import json
+import dataclasses
 from enum import Enum
 from decimal import Decimal
 from collections import UserString
-from dataclasses import asdict, is_dataclass
 from typing import (
     Any,
     Callable,
     Dict,
     Hashable,
+    ItemsView,
     Iterator,
     Mapping,
     Sequence,
     Type,
     TypeVar,
     Tuple,
     Optional,
 )
 
 from .misc import idem
+from .types import is_string
 
 
 class GenericDictEncoder(json.JSONEncoder):
     """
     A JSON encoder for :class:`GenericDict` objects. Also handles some types not
     necessarily handled by the default JSON encoder, i.e., UserString, os.PathLike,
     Decimals, etcetera.
@@ -45,16 +47,16 @@
     """
 
     def default(self, o):
         if isinstance(o, GenericDict):
             return o.to_raw_dict()
         elif isinstance(o, os.PathLike) or isinstance(o, UserString):
             return str(o)
-        elif is_dataclass(o):
-            return asdict(o)
+        elif dataclasses.is_dataclass(o):
+            return dataclasses.asdict(o)
         elif isinstance(o, Enum):
             return o.name
         elif isinstance(o, Decimal):
             if o.as_integer_ratio()[1] == 1:
                 return int(o)
             else:
                 return float(o)
@@ -171,15 +173,15 @@
 
     def values(self):
         """
         :returns: A set-like object providing a view of the values of the GenericDict object.
         """
         return self.__data.values()
 
-    def items(self):
+    def items(self) -> ItemsView[KT, VT]:
         """
         :returns: A set-like object providing a view of the GenericDict object as (key, value) tuples.
         """
         return self.__data.items()
 
     def dumps(self, **kwargs) -> str:
         """
@@ -206,19 +208,32 @@
         """
         return (key if key in self.__data else None, self.get(key))
 
     def update(self, incoming: "Mapping[KT, VT]"):
         """
         A convenience function to update multiple values in the GenericDict object
         at the same time.
-        :param
+        :param incoming: The values to update
         """
         for key, value in incoming.items():
             self[key] = value
 
+    def update_reorder(self, incoming: "Mapping[KT, VT]"):
+        """
+        A convenience function to update multiple values in the GenericDict object
+        at the same time. Pre-existing keys are deleted first so the values in
+        incoming are emplaced at the end of the dictionary.
+
+        :param incoming: The values to update
+        """
+        for key, value in incoming.items():
+            if key in self:
+                del self[key]
+            self[key] = value
+
 
 class GenericImmutableDict(GenericDict[KT, VT]):
     __lock: bool
 
     def __init__(
         self,
         copying: Optional[Mapping[KT, VT]] = None,
@@ -252,47 +267,49 @@
             pass
         return super().__setattr__(attr, value)
 
     def copy_mut(self) -> GenericDict[KT, VT]:
         return GenericDict(self)
 
 
-def is_string(obj: Any) -> bool:
-    return isinstance(obj, str) or isinstance(obj, UserString)
-
-
 # Screw this, if you can figure out how to type hint mapping in dictionary out
 # and non-mapping in sequence out in Python, be my guest
 def copy_recursive(input, translator: Callable = idem):
     """
     Copies any arbitrarily-deep nested structure of Mappings and/or Sequences.
 
     :param input: The input nested structure
     :param translator: Before an object is appended, this function will be
         called to process the value.
 
         By default, :func:`idem` is called.
     :returns: The copy.
 
-        All sequences will become built-in ``list``s and all mappings will
-        become built-in ``dict``s.
+        All sequences will become built-in ``list``\\(s) and all mappings will
+        become built-in ``dict``\\(s).
     """
 
     def recursive(input, visit_stack: list, *, sequence_cls=list, mapping_cls=dict):
         if id(input) in visit_stack:
             raise ValueError("Circular reference found in target object")
 
         visit_stack.append(id(input))
 
         result: Any = input
 
         if isinstance(input, Mapping):  # Mappings are Sequences, but not vice versa
             result = mapping_cls()
             for key, value in input.items():
                 result[key] = recursive(value, visit_stack)
+        elif dataclasses.is_dataclass(input):
+            replace = {}
+            as_dict = dataclasses.asdict(input)
+            for key, value in as_dict.items():
+                replace[key] = recursive(value, visit_stack)
+            result = dataclasses.replace(input, **replace)
         elif not is_string(input) and isinstance(input, Sequence):
             result = sequence_cls()
             for value in input:
                 result.append(recursive(value, visit_stack))
 
         visit_stack.pop()
```

### Comparing `openlane-2.0.0b9/openlane/common/tcl.py` & `openlane-2.0.0rc2/openlane/common/tcl.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         """
         :returns: If the string can be parsed by Tcl as a single token, the string
             is returned verbatim.
 
             Otherwise, the string is returned in double quotes, with any unsafe
             characters escaped with a backslash.
         """
+        if s == "":
+            return '""'
         if not _find_unsafe(s):
             return s
         return '"' + _escapes_in_quotes.sub(r"\\\1", s).replace("\n", r"\n") + '"'
 
     @staticmethod
     def join(ss: Iterable[str]) -> str:
         """
@@ -57,15 +59,15 @@
         interpreter = tkinter.Tcl()
         keys_modified = _setter_rx.findall(tcl_in)
 
         env_out = dict(env_in)
         rollback = {}
         for key, value in env_in.items():
             rollback[key] = os.getenv(key)
-            os.environ[key] = value
+            os.environ[key] = str(value)
 
         tcl_script = f"""
         {tcl_in}
         set counter 0
         foreach key [array names ::env] {{
             set "key$counter" $key
             set "value$counter" $::env($key)
```

### Comparing `openlane-2.0.0b9/openlane/config/__init__.py` & `openlane-2.0.0rc2/openlane/flows/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-The Configuration Module
-------------------------
+The Flow Module
+---------------
 
-This modules includes various functions for importing and/or generating OpenLane
-configuration objects. Configuration objects are the primary input to a flow.
+An API for implementing new flows using the OpenLane infrastructure, as well
+as a number of built-in flows.
 """
-from .preprocessor import Keys
-from .variable import Instance, Macro, Variable
-from .config import Meta, Config, InvalidConfig
-from .flow import flow_common_variables as universal_flow_config_variables
+from .flow import FlowError, FlowException, FlowProgressBar, Flow
+from .sequential import SequentialFlow
+from . import builtins
+from .cli import cloup_flow_opts
```

### Comparing `openlane-2.0.0b9/openlane/config/config.py` & `openlane-2.0.0rc2/openlane/config/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,29 +26,75 @@
     Literal,
     Mapping,
     Tuple,
     Union,
     List,
     Optional,
     Sequence,
-    Callable,
     Dict,
     Set,
 )
 
 from immutabledict import immutabledict
 
 from .variable import Variable
 from .removals import removed_variables
 from .flow import pdk_variables, scl_variables, flow_common_variables
 from .pdk_compat import migrate_old_config
 from .preprocessor import preprocess_dict, Keys as SpecialKeys
 from ..logging import info, warn
 from ..__version__ import __version__
-from ..common import GenericDict, GenericImmutableDict, TclUtils, Path
+from ..common import (
+    GenericDict,
+    GenericImmutableDict,
+    TclUtils,
+    AnyPath,
+    is_string,
+)
+
+AnyConfig = Union[AnyPath, Mapping[str, Any]]
+AnyConfigs = Union[AnyConfig, Sequence[AnyConfig]]
+
+
+class UnknownExtensionError(ValueError):
+    """
+    When a passed configuration file has an unrecognized extension, i.e.,
+    not .json or .tcl.
+    """
+
+    def __init__(self, config: AnyPath) -> None:
+        self.config = str(config)
+        _, ext = os.path.splitext(config)
+        super().__init__(
+            f"Unsupported configuration file extension '{ext}' for '{config}'."
+        )
+
+
+class PassedDirectoryError(ValueError):
+    """
+    When a passed configuration file is in fact a directory.
+    """
+
+    def __init__(self, config: AnyPath) -> None:
+        self.config = str(config)
+        super().__init__(
+            "Passing design directories as arguments is unsupported in OpenLane 2 or higher: please pass the configuration file(s) directly."
+        )
+
+
+def _validate_config_file(config: AnyPath) -> Literal["json", "tcl"]:
+    config = str(config)
+    if config.endswith(".tcl"):
+        return "tcl"
+    elif config.endswith(".json"):
+        return "json"
+    elif os.path.isdir(config):
+        raise PassedDirectoryError(config)
+    else:
+        raise UnknownExtensionError(config)
 
 
 class InvalidConfig(ValueError):
     """
     An error raised when a configuration under resolution is invalid.
 
     :param config: A human-readable name for the particular configuration file
@@ -76,15 +122,16 @@
     ) -> None:
         self.config = config
         self.warnings = warnings
         self.errors = errors
         if message is None:
             message = "The following errors were encountered: \n"
             for error in self.errors:
-                message += f"\t* {error}"
+                message += f"\t* {error}\n"
+            message = message.strip()
         super().__init__(message, *args, **kwargs)
 
 
 @dataclass
 class Meta:
     """
     Constitutes metadata for a configuration object.
@@ -253,30 +300,38 @@
             processed,
             meta=self.meta.copy(),
         )
 
     @classmethod
     def get_meta(
         Self,
-        json_config_in: Union[str, os.PathLike],
+        config_in: AnyConfig,
         flow_override: Optional[str] = None,
-    ) -> Optional[Meta]:
+    ) -> Meta:
         """
-        Returns the Meta object of a JSON configuration file
+        Returns the Meta object of a configuration dictionary or file.
 
-        :param config_in: A configuration file.
-        :returns: Either a Meta object, or if the file is not a JSON file, None.
+        :param config_in: A configuration object or file.
+        :returns: Either a Meta object, or if the file is invalid, None.
         """
-        try:
-            obj = json.load(open(json_config_in, encoding="utf8"))
-        except (json.JSONDecodeError, IsADirectoryError):
-            return None
+        default_meta_version = 2 if isinstance(config_in, Mapping) else 1
+
+        if is_string(config_in):
+            config_in = str(config_in)
+            validated_type = _validate_config_file(config_in)
+            if validated_type == "tcl":
+                return Meta(version=1)
+            elif validated_type == "json":
+                config_in = json.load(open(config_in, encoding="utf8"))
 
-        meta = Meta()
-        if meta_raw := obj.get("meta"):
+        assert not isinstance(config_in, str)
+        assert not isinstance(config_in, os.PathLike)
+
+        meta = Meta(version=default_meta_version)
+        if meta_raw := config_in.get("meta"):
             meta = Meta(**meta_raw)
 
         if flow_override is not None:
             meta.flow = flow_override
 
         return meta
 
@@ -349,15 +404,15 @@
         Config.current_interactive = Config(processed)
 
         return Config.current_interactive
 
     @classmethod
     def load(
         Self,
-        config_in: Union[str, os.PathLike, Mapping[str, Any]],
+        config_in: AnyConfigs,
         flow_config_vars: Sequence[Variable],
         *,
         config_override_strings: Optional[Sequence[str]] = None,
         pdk: Optional[str] = None,
         pdk_root: Optional[str] = None,
         scl: Optional[str] = None,
         design_dir: Optional[str] = None,
@@ -376,78 +431,109 @@
             Tcl files are also supported, but are deprecated and will be removed
             in the future.
 
         :param config_override_strings: A list of "overrides" in the form of
             NAME=VALUE strings. These are primarily for running OpenLane from
             the command-line and strictly speaking should not be used in the API.
 
-        :param design_dir: The design directory for said configuration.
-            Supported and required *if and only if* config_in is a dictionary.
+        :param design_dir: The design directory for said configuration(s).
+
+            If not explicitly provided, the design directory will be the
+            directory holding the last file in the list.
+
+            If no files are provided, this argument is required.
 
         :param pdk: A process design kit to use. Required unless specified via the
             "PDK" key in a configuration object.
 
         :param pdk_root: Required if Volare is not installed.
 
             If Volare is installed, this value can be used to optionally override
             Volare's default.
 
         :param scl: A standard cell library to use. If not specified, the PDK's
             default standard cell library will be used instead.
 
         :returns: A tuple containing a Config object and the design directory.
         """
-        loader: Callable = Self.__loads
-        raw: Union[str, Mapping] = ""
-        default_meta_version = 1
-        if not isinstance(config_in, Mapping):
-            if design_dir is not None:
-                raise TypeError(
-                    "The argument design_dir is not supported when config_in is not a dictionary."
-                )
-            config_in = os.path.abspath(config_in)
-
-            design_dir = str(os.path.dirname(config_in))
-            config_in = str(config_in)
-            if config_in.endswith(".json"):
-                raw = open(config_in, encoding="utf8").read()
-            elif config_in.endswith(".tcl"):
-                raw = open(config_in, encoding="utf8").read()
-                loader = Self.__loads_tcl
+        if isinstance(config_in, Mapping):
+            config_in = [config_in]
+        elif is_string(config_in):
+            config_in = [str(config_in)]
+
+        assert not isinstance(config_in, str)
+        assert not isinstance(config_in, os.PathLike)
+
+        if len(config_in) == 0:
+            raise ValueError("The value for config_in must not be empty.")
+
+        file_design_dir = None
+        configs_validated: List[AnyConfig] = []
+        for config in config_in:
+            if isinstance(config, Mapping):
+                configs_validated.append(config)
+            # Path
             else:
-                if os.path.isdir(config_in):
-                    raise ValueError(
-                        "Passing design folders as arguments is unsupported in OpenLane 2 or higher: please pass the JSON configuration file directly."
+                config = str(config)
+                _validate_config_file(config)
+                config_abspath = os.path.abspath(config)
+                file_design_dir = os.path.dirname(config_abspath)
+                configs_validated.append(config_abspath)
+
+        design_dir = design_dir or file_design_dir
+        if design_dir is None:
+            raise ValueError(
+                "The design_dir argument is required when configuration dictionaries are used."
+            )
+
+        config_obj = Config()
+        for config_validated in configs_validated:
+            try:
+                meta = Self.get_meta(config_validated)
+            except TypeError as e:
+                identifier = "configuration dict"
+                if is_string(config_validated):
+                    identifier = os.path.relpath(str(config_validated))
+                raise InvalidConfig(identifier, [], [f"'meta' object is invalid: {e}"])
+
+            assert meta is not None
+
+            mapping = None
+            if isinstance(config_validated, Mapping):
+                mapping = config_validated
+            elif isinstance(config_validated, str):
+                if config_validated.endswith(".tcl"):
+                    mapping = Self.__mapping_from_tcl(
+                        config_validated,
+                        design_dir,
+                        pdk_root=pdk_root,
+                        pdk=pdk,
+                        scl=scl,
+                    )
+                else:
+                    mapping = json.load(
+                        open(config_validated, encoding="utf8"), parse_float=Decimal
                     )
-                _, ext = os.path.splitext(config_in)
-                raise ValueError(
-                    f"Unsupported configuration file extension '{ext}' for '{config_in}'."
-                )
-        else:
-            default_meta_version = 2
-            if design_dir is None:
-                raise TypeError(
-                    "The argument design_dir is required when using attempting to load a Config with a dictionary."
-                )
-            raw = config_in
-            loader = Self.__load_dict
 
-        loaded = loader(
-            raw,
-            design_dir,
-            flow_config_vars=flow_config_vars,
-            pdk_root=pdk_root,
-            pdk=pdk,
-            scl=scl,
-            config_override_strings=(config_override_strings or []),
-            default_meta_version=default_meta_version,
-            _load_pdk_configs=_load_pdk_configs,
-        )
+            assert mapping is not None, "Invalid validated config"
+            mutable = config_obj.copy_mut()
+            mutable.update_reorder(mapping)
+            config_obj = Self.__load_dict(
+                mutable,
+                design_dir,
+                flow_config_vars=flow_config_vars,
+                pdk_root=pdk_root,
+                pdk=pdk,
+                scl=scl,
+                config_override_strings=(config_override_strings or []),
+                meta=meta,
+                _load_pdk_configs=_load_pdk_configs,
+            )
 
-        return (loaded, design_dir)
+        return (config_obj, design_dir)
 
     ## For Jupyter
     def _repr_markdown_(self) -> str:  # pragma: no cover
         title = (
             "Interactive Configuration"
             if self == Config.current_interactive
             else "Configuration"
@@ -459,79 +545,56 @@
             dedent(
                 f"""
                 ### {title}
                 #### {values_title}
 
                 <br />
 
-                ```yml
+                ```yaml
                 %s
                 ```
                 """
             )
             % yaml.safe_dump(json.loads(self.dumps()))
         )
 
     ## Private Methods
     @classmethod
-    def __loads(
-        Self,
-        json_str: str,
-        *args,
-        **kwargs,
-    ):
-        raw = json.loads(json_str, parse_float=Decimal)
-        return Self.__load_dict(
-            raw,
-            *args,
-            **kwargs,
-        )
-
-    @classmethod
     def __load_dict(
         Self,
         mapping_in: Mapping[str, Any],
         design_dir: str,
         flow_config_vars: Sequence[Variable],
         *,
+        meta: Meta,
         config_override_strings: Sequence[str],  # Unused, kept for API consistency
         pdk_root: Optional[str] = None,
         pdk: Optional[str] = None,
         scl: Optional[str] = None,
         full_pdk_warnings: bool = False,
-        default_meta_version: int = 1,
         _load_pdk_configs: bool = True,
     ) -> "Config":
         raw = dict(mapping_in)
 
-        meta: Optional[Meta] = None
-        if raw.get("meta") is not None:
-            meta_raw = raw["meta"]
+        if "meta" in raw:
             del raw["meta"]
-            try:
-                meta = Meta(**meta_raw)
-            except TypeError as e:
-                raise InvalidConfig(
-                    "design configuration file", [], [f"'meta' object is invalid: {e}"]
-                )
 
         flow_option_vars = []
         flow_pdk_vars = []
         for variable in flow_config_vars:
             if variable.pdk:
                 flow_pdk_vars.append(variable)
             else:
                 flow_option_vars.append(variable)
 
-        if meta is None:
-            meta = Meta(version=default_meta_version)
-
+        override_keys = set()
         for string in config_override_strings:
             key, value = string.split("=", 1)
             raw[key] = value
+            override_keys.add(key)
 
         mutable = GenericDict(
             preprocess_dict(
                 raw,
                 only_extract_process_info=True,
                 design_dir=design_dir,
             )
@@ -553,14 +616,17 @@
             mutable, pdkpath, scl = Self.__get_pdk_config(
                 pdk=pdk,
                 scl=scl,
                 pdk_root=pdk_root,
                 full_pdk_warnings=full_pdk_warnings,
                 flow_pdk_vars=flow_pdk_vars,
             )
+        else:
+            if pdk_root is not None:
+                pdkpath = os.path.join(pdk_root, mutable["PDK"])
 
         readable_paths = [
             os.path.abspath(design_dir),
         ]
         if pdkpath != "":
             readable_paths.append(os.path.abspath(pdkpath))
 
@@ -571,21 +637,25 @@
                 pdkpath=pdkpath,
                 scl=mutable[SpecialKeys.scl],
                 design_dir=design_dir,
                 readable_paths=readable_paths,
             )
         )
 
-        permissive_variables = []
-        strict_variables = list(flow_config_vars)
-        on_unknown_key: Union[Literal["error", "warn"], None] = "error"
-        if meta.version < 2:
-            permissive_variables = strict_variables
-            strict_variables = []
-            on_unknown_key = "warn"
+        permissive_variables = list(flow_config_vars)
+        strict_variables = []
+        on_unknown_key: Union[Literal["error", "warn"], None] = "warn"
+        if meta.version >= 2:
+            permissive_variables = []
+            for variable in flow_config_vars:
+                if variable.name in override_keys:
+                    permissive_variables.append(variable)
+                    continue
+                strict_variables.append(variable)
+            on_unknown_key = "error"
 
         processed, design_warnings, design_errors = Config.__process_variable_list(
             mutable,
             permissive_variables,
             strict_variables,
             removed_variables,
             on_unknown_key=on_unknown_key,
@@ -602,115 +672,84 @@
             )
         for warning in design_warnings:
             warn(warning)
 
         return Config(processed, meta=meta)
 
     @classmethod
-    def __loads_tcl(
+    def __mapping_from_tcl(
         Self,
-        config: str,
+        config: AnyPath,
         design_dir: str,
-        flow_config_vars: Sequence[Variable],
         *,
-        config_override_strings: Sequence[str],  # Unused, kept for API consistency
         pdk_root: Optional[str] = None,
         pdk: Optional[str] = None,
         scl: Optional[str] = None,
-        full_pdk_warnings: bool = False,
-        default_meta_version: int = 1,  # Unused, kept for API consistency
-        _load_pdk_configs: bool = True,  # Unused, kept for API consistency
-    ) -> "Config":
+    ) -> Mapping[str, Any]:
+        config_str = open(config, encoding="utf8").read()
+
         warn(
             "Support for .tcl configuration files is deprecated. Please migrate to a .json file at your earliest convenience."
         )
 
-        flow_option_vars = []
-        flow_pdk_vars = []
-        for variable in flow_config_vars:
-            if variable.pdk:
-                flow_pdk_vars.append(variable)
-            else:
-                flow_option_vars.append(variable)
-
         pdk_root = Self.__resolve_pdk_root(pdk_root)
 
         tcl_vars_in = GenericDict(
             {
                 SpecialKeys.pdk_root: pdk_root,
                 SpecialKeys.pdk: pdk,
             }
         )
         tcl_vars_in[SpecialKeys.scl] = ""
         tcl_vars_in[SpecialKeys.design_dir] = design_dir
-        tcl_config = GenericDict(TclUtils._eval_env(tcl_vars_in, config))
+        tcl_config = GenericDict(TclUtils._eval_env(tcl_vars_in, config_str))
 
         process_info = preprocess_dict(
             tcl_config,
             only_extract_process_info=True,
             design_dir=design_dir,
         )
 
         pdk = process_info.get(SpecialKeys.pdk) or pdk
 
         if pdk is None:
             raise ValueError(
                 "The pdk argument is required as the configuration object lacks a 'PDK' key."
             )
 
-        mutable, _, scl = Self.__get_pdk_config(
+        _, _, scl = Self.__get_pdk_config(
             pdk=pdk,
             scl=scl,
             pdk_root=pdk_root,
-            full_pdk_warnings=full_pdk_warnings,
-            flow_pdk_vars=flow_pdk_vars,
+            full_pdk_warnings=False,
         )
 
         tcl_vars_in[SpecialKeys.pdk] = pdk
         tcl_vars_in[SpecialKeys.scl] = scl
         tcl_vars_in[SpecialKeys.design_dir] = design_dir
 
-        mutable.update(GenericDict(TclUtils._eval_env(tcl_vars_in, config)))
-        for string in config_override_strings:
-            key, value = string.split("=", 1)
-            mutable[key] = value
+        tcl_mapping = GenericDict(TclUtils._eval_env(tcl_vars_in, config_str))
 
-        processed, design_warnings, design_errors = Config.__process_variable_list(
-            mutable,
-            list(flow_config_vars),
-            [],
-            removed_variables,
-            on_unknown_key="warn",
-        )
-
-        if len(design_errors) != 0:
-            raise InvalidConfig(
-                "design configuration file", design_warnings, design_errors
-            )
-
-        if len(design_warnings) > 0:
-            info(
-                "Loading the design configuration file has generated the following warnings:"
-            )
-        for warning in design_warnings:
-            warn(warning)
-
-        return Config(processed)
+        return tcl_mapping
 
     @classmethod
-    def __resolve_pdk_root(Self, pdk_root: Optional[str]) -> str:
-        try:
-            import volare
-
-            pdk_root = volare.get_volare_home(pdk_root)
-        except ImportError:
-            if pdk_root is None:
+    def __resolve_pdk_root(
+        Self,
+        pdk_root: Optional[str],
+    ) -> str:
+        if pdk_root is None:
+            try:
+                import volare
+
+                pdk_root = volare.get_volare_home(pdk_root)
+            except ImportError:
                 raise ValueError(
                     "The pdk_root argument is required as Volare is not installed."
                 )
+
         return os.path.abspath(pdk_root)
 
     @staticmethod
     @lru_cache(1, True)
     def __get_pdk_raw(
         pdk_root: str, pdk: str, scl: Optional[str]
     ) -> Tuple[immutabledict[str, Any], str, str]:
@@ -722,15 +761,15 @@
         )
 
         if scl is not None:
             pdk_config[SpecialKeys.scl] = scl
 
         pdkpath = os.path.join(pdk_root, pdk)
         if not os.path.exists(pdkpath):
-            matches = glob(f"{pdkpath}*")
+            matches = sorted(glob(f"{pdkpath}*"))
             errors = [f"The PDK {pdk} was not found."]
             warnings = []
             for match in matches:
                 basename = os.path.basename(match)
                 warnings.append(f"A similarly-named PDK was found: {basename}")
             raise InvalidConfig("PDK configuration", warnings, errors)
 
@@ -852,61 +891,14 @@
                 mutable["DIODE_ON_PORTS"] = "none"
                 if dis in [3, 6]:
                     mutable["GRT_REPAIR_ANTENNAS"] = True
                 if dis in [4, 6]:
                     mutable["RUN_HEURISTIC_DIODE_INSERTION"] = True
                     mutable["DIODE_ON_PORTS"] = "in"
 
-        # Macros
-        if mutable.get("EXTRA_SPEFS") is not None and mutable.get("MACROS") is None:
-            mutable["MACROS"] = {}
-
-            extra_spef_list = mutable["EXTRA_SPEFS"]
-            del mutable["EXTRA_SPEFS"]
-            if isinstance(extra_spef_list, str):
-                extra_spef_list = extra_spef_list.split(" ")
-
-            if not isinstance(extra_spef_list, list):
-                errors.append(
-                    f"Invalid type for 'EXTRA_SPEFS': {type(extra_spef_list)}. It is recommended that you update your configuration to use the Macro object."
-                )
-            elif len(extra_spef_list) % 4 != 0:
-                errors.append(
-                    "Invalid value for 'EXTRA_SPEFS': Element count not divisible by four. It is recommended that you update your configuration to use the Macro object."
-                )
-            else:
-                warnings.append(
-                    "The configuration variable 'EXTRA_SPEFS' is deprecated. Check the docs on how to use the new 'MACROS' configuration variable."
-                )
-                for i in range(len(extra_spef_list) // 4):
-                    start = i * 4
-                    module, min, nom, max = (
-                        extra_spef_list[start],
-                        extra_spef_list[start + 1],
-                        extra_spef_list[start + 2],
-                        extra_spef_list[start + 3],
-                    )
-                    macro_dict = {
-                        "module": module,
-                        "gds": [Path._dummy_path],
-                        "lef": [Path._dummy_path],
-                    }
-                    macro_dict["spef"] = {
-                        "min_*": [min],
-                        "nom_*": [nom],
-                        "max_*": [max],
-                    }
-                    mutable["MACROS"][module] = macro_dict
-        elif (
-            mutable.get("EXTRA_SPEFS") is not None and mutable.get("MACROS") is not None
-        ):
-            errors.append(
-                "EXTRA_SPEFS cannot be defined simultaneously with its successor variable, MACROS"
-            )
-
         for variable in variables:
             try:
                 key, value_processed = variable.compile(
                     mutable_config=mutable,
                     warning_list_ref=warnings,
                     values_so_far=final,
                     permissive_typing=True,
@@ -938,15 +930,19 @@
         for key in sorted(mutable.keys()):
             assert isinstance(key, str)
 
             if key in vars(SpecialKeys).values():
                 continue
             if key in removed:
                 warnings.append(f"'{key}' has been removed: {removed[key]}")
-            elif "_OPT" not in key and key != "//":
+            elif (
+                "_OPT" not in key
+                and not key.startswith("//")
+                and not key.startswith("#")
+            ):
                 if on_unknown_key == "error":
                     if key in Variable.known_variable_names:
                         warnings.append(
                             f"Key '{key}' provided is unused by the current flow."
                         )
                     else:
                         errors.append(f"Unknown key '{key}' provided.")
```

### Comparing `openlane-2.0.0b9/openlane/config/flow.py` & `openlane-2.0.0rc2/openlane/config/flow.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,36 +7,51 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import os
+
 from decimal import Decimal
-from typing import List, Optional, Dict, Union
+from typing import List, Optional, Dict, Sequence, Union, Tuple
 
 from .variable import Variable, Macro
-from ..common import Path
+from ..common import Path, get_script_dir
+
+
+def _prefix_to_wildcard(prefixes_raw: Union[str, Sequence[str]]):
+    prefixes = prefixes_raw
+    if isinstance(prefixes, str):
+        prefixes = prefixes.split()
+    return [f"{prefix}*" for prefix in prefixes]
 
 
 pdk_variables = [
     # Core/Common
     Variable(
         "STD_CELL_LIBRARY",
         str,
-        "Specifies the default standard cell library to be used under the specified PDK.",
+        "Specifies the default standard cell library to be used under the specified PDK. Must be a valid C identifier, i.e., matches the regular expression `[_a-zA-Z][_a-zA-Z0-9]+`.",
         pdk=True,
     ),
     Variable(
         "VDD_PIN",
         str,
         "The power pin for the cells.",
         pdk=True,
     ),
     Variable(
+        "VDD_PIN_VOLTAGE",
+        Decimal,
+        "The voltage of the VDD pin.",
+        pdk=True,
+    ),
+    Variable(
         "GND_PIN",
         str,
         "The ground pin for the cells.",
         pdk=True,
     ),
     Variable(
         "WIRE_LENGTH_THRESHOLD",
@@ -66,24 +81,26 @@
     Variable(
         "GPIO_PADS_VERILOG",
         Optional[List[Path]],
         "Path(s) to GPIO pad Verilog models.",
         pdk=True,
     ),
     Variable(
-        "GPIO_PADS_PREFIX",
+        "GPIO_PAD_CELLS",
         Optional[List[str]],
         "A list of pad cell name prefixes.",
+        deprecated_names=[("GPIO_PADS_PREFIX", _prefix_to_wildcard)],
         pdk=True,
     ),
     Variable(
-        "PRIMARY_SIGNOFF_TOOL",
+        "PRIMARY_GDSII_STREAMOUT_TOOL",
         str,
-        "Specify the primary signoff tool for taping out with this PDK. For most open-source PDKs, that would be 'magic'.",
+        "Specify the primary GDSII streamout tool for this PDK. For most open-source PDKs, that would be 'magic'.",
         pdk=True,
+        deprecated_names=["PRIMARY_SIGNOFF_TOOL"],
     ),
     # Timing and Power
     Variable(
         "DEFAULT_MAX_TRAN",
         Optional[Decimal],
         "Defines the default maximum transition value used in Synthesis and CTS.\nA minimum of 0.1 * CLOCK_PERIOD and this variable, if defined, is used.",
         units="ns",
@@ -126,100 +143,23 @@
         "FP_TAPCELL_DIST",
         Decimal,
         "The distance between tap cell columns.",
         units="µm",
         pdk=True,
     ),
     Variable(
-        "FP_PDN_RAIL_OFFSET",
-        Decimal,
-        "The offset for the power distribution network rails for first metal layer.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_VWIDTH",
-        Decimal,
-        "The strap width for the vertical layer in generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_VSPACING",
-        Decimal,
-        "The spacing between vertical straps in generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_HSPACING",
-        Decimal,
-        "The spacing between horizontal straps in generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_HWIDTH",
-        Decimal,
-        "The strap width for the horizontal layer in generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_CORE_RING_VWIDTH",
-        Decimal,
-        "The width for the vertical layer in the core ring of generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_CORE_RING_HWIDTH",
-        Decimal,
-        "The width for the horizontal layer in the core ring of generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_CORE_RING_VSPACING",
-        Decimal,
-        "The spacing for the vertical layer in the core ring of generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_CORE_RING_HSPACING",
-        Decimal,
-        "The spacing for the horizontal layer in the core ring of generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_CORE_RING_VOFFSET",
-        Decimal,
-        "The offset for the vertical layer in the core ring of generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_CORE_RING_HOFFSET",
-        Decimal,
-        "The offset for the horizontal layer in the core ring of generated power distribution networks.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
         "FP_IO_HLAYER",
         str,
         "The metal layer on which to place horizontal IO pins, i.e., the top and bottom of the die.",
         pdk=True,
     ),
     Variable(
         "FP_IO_VLAYER",
         str,
-        "The metal layer on which to place vertial IO pins, i.e., the top and bottom of the die.",
+        "The metal layer on which to place vertical IO pins, i.e., the top and bottom of the die.",
         pdk=True,
     ),
     Variable("RT_MIN_LAYER", str, "The lowest metal layer to route on.", pdk=True),
     Variable("RT_MAX_LAYER", str, "The highest metal layer to route on.", pdk=True),
 ]
 
 scl_variables = [
@@ -235,14 +175,21 @@
         "SCL_POWER_PINS",
         List[str],
         "SCL-specific power pins",
         deprecated_names=["STD_CELL_POWER_PINS"],
         pdk=True,
     ),
     Variable(
+        "TRISTATE_CELLS",
+        Optional[List[str]],
+        "A list of cell names or wildcards of tri-state buffers.",
+        deprecated_names=[("TRISTATE_CELL_PREFIX", _prefix_to_wildcard)],
+        pdk=True,
+    ),
+    Variable(
         "FILL_CELL",
         List[str],
         "A list of cell names or wildcards of fill cells to be used in fill insertion.",
         pdk=True,
     ),
     Variable(
         "DECAP_CELL",
@@ -267,31 +214,43 @@
         "CELL_GDS",
         List[Path],
         "Path(s) to the cells' GDSII file(s).",
         deprecated_names=["GDS_FILES", "CELLS_GDS"],
         pdk=True,
     ),
     Variable(
+        "CELL_VERILOG_MODELS",
+        Optional[List[Path]],
+        "Path(s) to cells' Verilog model(s)",
+        pdk=True,
+    ),
+    Variable(
+        "CELL_BB_VERILOG_MODELS",
+        Optional[List[Path]],
+        "Path(s) to cells' black-box Verilog model(s)",
+        pdk=True,
+    ),
+    Variable(
         "CELL_SPICE_MODELS",
         Optional[List[Path]],
         "Path(s) to cells' SPICE model(s)",
         pdk=True,
     ),
     Variable(
-        "SYNTH_EXCLUSION_CELL_LIST",
+        "SYNTH_EXCLUDED_CELL_FILE",
         Path,
-        "Path to a text file containing a list of cells to be excluded from the lib file in synthesis alone. If not defined, the original lib file will be used as-is.",
-        deprecated_names=["NO_SYNTH_CELL_LIST"],
+        "Path to a text file containing a list of (wildcards matching) cells to be excluded from the lib file in synthesis alone.",
+        deprecated_names=["NO_SYNTH_CELL_LIST", "SYNTH_EXCLUSION_CELL_LIST"],
         pdk=True,
     ),
     Variable(
-        "PNR_EXCLUSION_CELL_LIST",
+        "PNR_EXCLUDED_CELL_FILE",
         Path,
-        "Path to a text file containing a list of undesirable or bad (DRC-failed or complex pinout) cells to be excluded from synthesis AND PnR. If not defined, all cells will be used.",
-        deprecated_names=["DRC_EXCLUDE_CELL_LIST"],
+        "Path to a text file containing a list of undesirable or bad (DRC-failed or complex pinout) cells or wildcards matching cells to be excluded from synthesis AND PnR.",
+        deprecated_names=["DRC_EXCLUDE_CELL_LIST", "PNR_EXCLUSION_CELL_LIST"],
         pdk=True,
     ),
     # Constraints
     Variable(
         "OUTPUT_CAP_LOAD",
         Decimal,
         "Defines the capacitive load on the output ports.",
@@ -312,14 +271,21 @@
         Optional[Decimal],
         "The max transition time (slew) from high to low or low to high on cell inputs in ns to be used as a constraint on Synthesis and CTS. If not provided, it is calculated at runtime as `10%` of the provided clock period, unless that exceeds the PDK's `DEFAULT_MAX_TRAN` value.",
         units="ns",
         deprecated_names=["SYNTH_MAX_TRAN"],
         pdk=True,
     ),
     Variable(
+        "MAX_CAPACITANCE_CONSTRAINT",
+        Optional[Decimal],
+        "The maximum capacitance constraint. If not provided, the constraint is not set in the SDC file which will fall back to the value set by the liberty file",
+        units="pF",
+        pdk=True,
+    ),
+    Variable(
         "CLOCK_UNCERTAINTY_CONSTRAINT",
         Decimal,
         "Specifies a value for the clock uncertainty/jitter for timing analysis.",
         units="ns",
         deprecated_names=["SYNTH_CLOCK_UNCERTAINTY"],
         pdk=True,
     ),
@@ -374,115 +340,33 @@
     ),
     Variable(
         "SYNTH_BUFFER_CELL",
         str,
         "Defines a buffer port to be used by yosys during synthesis: in the format `{cell}/{input_port}/{output_port}`",
         pdk=True,
     ),
-    # Clock Tree Synthesis
     Variable(
-        "CTS_ROOT_BUFFER",
-        str,
-        "Defines the cell inserted at the root of the clock tree. Used in CTS.",
-        pdk=True,
-    ),
-    Variable(
-        "CTS_CLK_BUFFERS",
-        List[str],
-        "Defines the list of clock buffers to be used in CTS.",
-        deprecated_names=["CTS_CLK_BUFFER_LIST"],
-        pdk=True,
-    ),
-    Variable(
-        "CTS_MAX_CAP",
-        Decimal,
-        "Defines the maximum capacitance, used in CTS.",
-        units="pF",
-        pdk=True,
-    ),
-    # Floorplanning
-    Variable(
-        "FP_WELLTAP_CELL",
+        "WELLTAP_CELL",
         str,
         "Defines the cell used for tap insertion.",
         pdk=True,
+        deprecated_names=["FP_WELLTAP_CELL"],
     ),
     Variable(
-        "FP_ENDCAP_CELL",
+        "ENDCAP_CELL",
         str,
         "Defines so-called 'end-cap' cells- decap cells placed at either sides of a design.",
         pdk=True,
-    ),
-    Variable(
-        "FP_PDN_RAIL_LAYER",
-        str,
-        "Defines the metal layer used for PDN rails.",
-        deprecated_names=["FP_PDN_RAILS_LAYER"],
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_RAIL_WIDTH",
-        Decimal,
-        "Defines the width of PDN rails on the `FP_PDN_RAILS_LAYER` layer.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_HORIZONTAL_LAYER",
-        str,
-        "Defines the horizontal PDN layer.",
-        deprecated_names=["FP_PDN_UPPER_LAYER"],
-        pdk=True,
-    ),
-    Variable(
-        "FP_PDN_VERTICAL_LAYER",
-        str,
-        "Defines the vertical PDN layer.",
-        deprecated_names=["FP_PDN_LOWER_LAYER"],
-        pdk=True,
-    ),
-    Variable(
-        "IGNORE_DISCONNECTED_MODULES",
-        Optional[List[str]],
-        "Modules (or cells) to ignore when checking for disconnected pins.",
-        pdk=True,
+        deprecated_names=["FP_ENDCAP_CELL"],
     ),
     # Placement
     Variable(
         "PLACE_SITE",
         str,
-        "Defines the main placement site in placement as specified in the technology LEF files, to generate the placement grid.",
-        pdk=True,
-    ),
-    Variable(
-        "PLACE_SITE_WIDTH",
-        Decimal,
-        "The site width for the previously designated place site.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "PLACE_SITE_HEIGHT",
-        Decimal,
-        "The site height for the previously designated place site.",
-        units="µm",
-        pdk=True,
-    ),
-    Variable(
-        "GPL_CELL_PADDING",
-        Decimal,
-        "Cell padding value (in sites) for global placement. The number will be integer divided by 2 and placed on both sides.",
-        units="sites",
-        pdk=True,
-    ),
-    Variable(
-        "DPL_CELL_PADDING",
-        Decimal,
-        "Cell padding value (in sites) for detailed placement. The number will be integer divided by 2 and placed on both sides. Should be <= global placement.",
-        units="sites",
+        "Defines the primary placement site in placement as specified in the technology LEF files, to generate the placement grid.",
         pdk=True,
     ),
     Variable(
         "CELL_PAD_EXCLUDE",
         List[str],
         "Defines a list of cells to be excluded from cell padding.",
         pdk=True,
@@ -490,50 +374,36 @@
     # Antenna
     Variable(
         "DIODE_CELL",
         Optional[str],
         "Defines a diode cell used to fix antenna violations, in the format {name}/{port}.",
         pdk=True,
     ),
-    # Routing
-    Variable(
-        "GRT_LAYER_ADJUSTMENTS",
-        List[Decimal],
-        "Layer-specific reductions in the routing capacity of the edges between the cells in the global routing graph, delimited by commas. Values range from 0 through 1.",
-        pdk=True,
-    ),
-    # CVC
-    Variable(
-        "CVC_SCRIPTS_DIR",
-        Optional[Path],
-        "Path to a directory of Circuit Validity Checker (CVC) scripts for the relevant PDK. Must contain the following set of files: `cvcrc`, an initialization file, `cdl.awk`, an awk script to remove black box definitions from SPICE files, `models`, cell models, and finally `power.awk`, an awk script that adds power information to the verilog netlists.\nIf this path is not defined, this PDK will be marked incompatible with CVC.",
-        pdk=True,
-    ),
 ]
 option_variables = [
     # Common
     Variable(
         "DESIGN_DIR",
         Path,
-        "The directory of the design. Does not need to be provided explicitly.",
+        "The directory of the design. Should be set via command-line arguments or :meth:`Config.load` flags and not actual configuration files. If using a configuration file, ``DESIGN_DIR`` will be the directory where that file exists.",
     ),
     Variable(
-        "DESIGN_NAME",
-        str,
-        "The name of the top level module of the design. This is the only required variable for all steps and all flows.",
+        "PDK_ROOT",
+        Path,
+        "The home path of all PDKs. Should be set via command-line arguments or :meth:`Config.load` flags and not actual configuration files.",
     ),
     Variable(
-        "PDK_ROOT",
+        "DESIGN_NAME",
         str,
-        "The path to all PDKs. This variable is special and tools should typically handle them.",
+        "The name of the top level module of the design. Must be a valid C identifier, i.e., matches the regular expression `[_a-zA-Z][_a-zA-Z0-9]+`.",
     ),
     Variable(
         "PDK",
         str,
-        "Specifies the process design kit (PDK).",
+        "Specifies the process design kit (PDK). Must be a valid C identifier, i.e., matches the regular expression `[_a-zA-Z][_a-zA-Z0-9]+`.",
         default="sky130A",
     ),
     Variable(
         "CLOCK_PERIOD",
         Decimal,
         "The clock period for the design.",
         units="ns",
@@ -557,18 +427,25 @@
     Variable(
         "GND_NETS",
         Optional[List[str]],
         "Specifies the ground nets/pins to be used when creating the power grid for the design.",
     ),
     Variable(
         "DIE_AREA",
-        Optional[str],
-        'Specific die area to be used in floorplanning when `FP_SIZING` is set to `absolute`. Specified as a 4-corner rectangle "x0 y0 x1 y1".',
+        Optional[Tuple[Decimal, Decimal, Decimal, Decimal]],
+        'Specific die area to be used in floorplanning. Specified as a 4-corner rectangle "x0 y0 x1 y1".',
         units="µm",
     ),
+    # Exclusion Options
+    Variable(
+        "EXTRA_EXCLUDED_CELLS",
+        Optional[List[str]],
+        "Wildcards matching additional cells to exclude from both synthesis and PnR.",
+        deprecated_names=["RSZ_DONT_USE_CELLS", "DONT_USE_CELLS"],
+    ),
     # Macros
     Variable(
         "MACROS",
         Optional[Dict[str, Macro]],
         "A dictionary of Macro definition objects. See {py:class}`openlane.config.Macro` for more info.",
     ),
     Variable(
@@ -593,55 +470,17 @@
         "Specifies LIB files of pre-hardened macros used in the current design, used during timing analyses (and during parasitics-based STA as a fallback). These are loaded indiscriminately for all timing corners.",
     ),
     Variable(
         "EXTRA_GDS_FILES",
         Optional[List[Path]],
         "Specifies GDS files of pre-hardened macros used in the current design, used during tape-out.",
     ),
-    # Unimplemented - To be moved to steps
-    Variable(
-        "FP_CONTEXT_DEF",
-        Optional[Path],
-        "Points to the parent DEF file that includes this macro/design and uses this DEF file to determine the best locations for the pins. It must be used with `FP_CONTEXT_LEF`, otherwise it's considered non-existing. If not set, then the IO pins will be placed based on one of the other methods depending on the rest of the configurations.",
-    ),
-    Variable(
-        "FP_CONTEXT_LEF",
-        Optional[Path],
-        "Points to the parent LEF file that includes this macro/design and uses this LEF file to determine the best locations for the pins. It must be used with `FP_CONTEXT_DEF`, otherwise it's considered non-existing. If not set, then the IO pins will be placed based on one of the other methods depending on the rest of the configurations.",
-    ),
-    Variable(
-        "FP_PADFRAME_CFG",
-        Optional[str],
-        "A configuration file passed to `padringer`, a padframe generator.",
-    ),
     Variable(
-        "GRT_OBS",
-        Optional[List[str]],
-        'Specifies custom obstruction to be added prior to global routing. List of layer and coordinates: `layer llx lly urx ury`, where `ll` and `ur` stand for "lower left" and "upper right" respectively. (Example: `li1 0 100 1000 300, met5 0 0 1000 500`).',
-    ),
-    Variable(
-        "LVS_INSERT_POWER_PINS",
-        bool,
-        "Enables power pin insertion before running LVS.",
-        default=True,
-    ),
-    Variable(
-        "RUN_CVC",
-        bool,
-        "Runs the Circuit Validity Checker on the output spice, which is a voltage-aware ERC checker for CDL netlists. Will not run unless supported by the current PDK.",
-        default=True,
-    ),
-    Variable(
-        "LEC_ENABLE",
-        bool,
-        "Enables logic verification using yosys, for comparing each netlist at each stage of the flow with the previous netlist and verifying that they are logically equivalent. Warning: this will increase the runtime significantly.",
-        default=False,
-    ),
-    Variable(
-        "CHECK_ASSIGN_STATEMENTS",
-        bool,
-        "Checks for assign statement in the generated gate level netlist and aborts if any were found.",
-        default=False,
+        "FALLBACK_SDC_FILE",
+        Path,
+        "A fallback SDC file for when a step-specific SDC file is not defined.",
+        deprecated_names=["BASE_SDC_FILE", "SDC_FILE"],
+        default=Path(os.path.join(get_script_dir(), "base.sdc")),
     ),
 ]
 
 flow_common_variables = pdk_variables + scl_variables + option_variables
```

### Comparing `openlane-2.0.0b9/openlane/config/pdk_compat.py` & `openlane-2.0.0rc2/openlane/config/pdk_compat.py`

 * *Files 18% similar despite different names*

```diff
@@ -90,72 +90,140 @@
         first_lib = os.path.basename(lib_list[0])[:-4]
         pvt = first_lib.split("__")[1]
         if default_pvt == "":
             default_pvt = pvt
         corner = f"*_{pvt}"
         lib_sta[corner] = lib_list
 
-    process_sta("LIB_SYNTH")
-    process_sta("LIB_SLOWEST")
-    process_sta("LIB_FASTEST")
+    if "LIB" not in config:
+        process_sta("LIB_SYNTH")
+        process_sta("LIB_SLOWEST")
+        process_sta("LIB_FASTEST")
+
+        if new["PDK"].startswith("sky130"):
+            new["STA_CORNERS"] = [
+                "nom_tt_025C_1v80",
+                "nom_ss_100C_1v60",
+                "nom_ff_n40C_1v95",
+                "min_tt_025C_1v80",
+                "min_ss_100C_1v60",
+                "min_ff_n40C_1v95",
+                "max_tt_025C_1v80",
+                "max_ss_100C_1v60",
+                "max_ff_n40C_1v95",
+            ]
+        elif new["PDK"].startswith("gf180mcu"):
+            new["STA_CORNERS"] = [
+                "nom_tt_025C_5v00",
+                "nom_ss_125C_4v50",
+                "nom_ff_n40C_5v50",
+                "min_tt_025C_5v00",
+                "min_ss_125C_4v50",
+                "min_ff_n40C_5v50",
+                "max_tt_025C_5v00",
+                "max_ss_125C_4v50",
+                "max_ff_n40C_5v50",
+            ]
 
-    if new["PDK"].startswith("sky130"):
-        new["STA_CORNERS"] = [
-            "nom_tt_025C_1v80",
-            "nom_ss_100C_1v60",
-            "nom_ff_n40C_1v95",
-            "min_tt_025C_1v80",
-            "min_ss_100C_1v60",
-            "min_ff_n40C_1v95",
-            "max_tt_025C_1v80",
-            "max_ss_100C_1v60",
-            "max_ff_n40C_1v95",
-        ]
-    elif new["PDK"].startswith("gf180mcu"):
-        new["STA_CORNERS"] = [
-            "nom_tt_025C_5v00",
-            "nom_ss_125C_4v50",
-            "nom_ff_n40C_5v50",
-            "min_tt_025C_5v00",
-            "min_ss_125C_4v50",
-            "min_ff_n40C_5v50",
-            "max_tt_025C_5v00",
-            "max_ss_125C_4v50",
-            "max_ff_n40C_5v50",
-        ]
-
-    new["DEFAULT_CORNER"] = f"nom_{default_pvt}"
-    new["LIB"] = lib_sta
+        new["DEFAULT_CORNER"] = f"nom_{default_pvt}"
+        new["LIB"] = lib_sta
 
     # 7. capacitance and such
     if "SYNTH_CAP_LOAD" in config:
         new["OUTPUT_CAP_LOAD"] = config["SYNTH_CAP_LOAD"]
         del new["SYNTH_CAP_LOAD"]
 
-    new["MAX_FANOUT_CONSTRAINT"] = 10
-    new["CLOCK_UNCERTAINTY_CONSTRAINT"] = 0.25
-    new["CLOCK_TRANSITION_CONSTRAINT"] = 0.15
-    new["TIME_DERATING_CONSTRAINT"] = 5
-    new["IO_DELAY_CONSTRAINT"] = 20
+    if new["PDK"].startswith("sky130") or new["PDK"].startswith("gf180mcu"):
+        new["MAX_FANOUT_CONSTRAINT"] = 10
+        new["CLOCK_UNCERTAINTY_CONSTRAINT"] = 0.25
+        new["CLOCK_TRANSITION_CONSTRAINT"] = 0.15
+        new["TIME_DERATING_CONSTRAINT"] = 5
+        new["IO_DELAY_CONSTRAINT"] = 20
+        new["FP_IO_MIN_DISTANCE"] = 3
+        new["FP_IO_HLENGTH"] = 4
+        new["FP_IO_VLENGTH"] = 4
 
-    # 8. SPICE models
+    # 8. "Implicit" Paths
     if new["PDK"].startswith("sky130") or new["PDK"].startswith("gf180mcu"):
+        model_glob = os.path.join(
+            config["PDK_ROOT"],
+            config["PDK"],
+            "libs.ref",
+            config["STD_CELL_LIBRARY"],
+            "verilog",
+            "*.v",
+        )
+        new["CELL_VERILOG_MODELS"] = sorted(
+            [path for path in glob(model_glob) if "_blackbox" not in path]
+        )
+
+        bb_glob = os.path.join(
+            config["PDK_ROOT"],
+            config["PDK"],
+            "libs.ref",
+            config["STD_CELL_LIBRARY"],
+            "verilog",
+            "*__blackbox*.v",
+        )
+
+        if blackbox_models := glob(bb_glob):
+            new["CELL_BB_VERILOG_MODELS"] = sorted(blackbox_models)
+
         spice_glob = os.path.join(
             config["PDK_ROOT"],
             config["PDK"],
             "libs.ref",
             config["STD_CELL_LIBRARY"],
             "spice",
             "*.spice",
         )
-        new["CELL_SPICE_MODELS"] = glob(spice_glob)
+        new["CELL_SPICE_MODELS"] = sorted(glob(spice_glob))
+
+        mag_glob = os.path.join(
+            config["PDK_ROOT"],
+            config["PDK"],
+            "libs.ref",
+            config["STD_CELL_LIBRARY"],
+            "mag",
+            "*.mag",
+        )
+        new["CELL_MAGS"] = sorted(glob(mag_glob))
+
+        maglef_glob = os.path.join(
+            config["PDK_ROOT"],
+            config["PDK"],
+            "libs.ref",
+            config["STD_CELL_LIBRARY"],
+            "maglef",
+            "*.mag",
+        )
+        new["CELL_MAGLEFS"] = sorted(glob(maglef_glob))
+
+        new["MAGIC_PDK_SETUP"] = os.path.join(
+            config["PDK_ROOT"],
+            config["PDK"],
+            "libs.tech",
+            "magic",
+            f"{config['PDK']}.tcl",
+        )
 
     # 9. Primary Signoff Tool
     if new["PDK"].startswith("sky130") or new["PDK"].startswith("gf180mcu"):
-        new["PRIMARY_SIGNOFF_TOOL"] = "magic"
+        new["PRIMARY_GDSII_STREAMOUT_TOOL"] = "magic"
+
+    # 10. CVC
+    if "CVC_SCRIPTS_DIR" in config:
+        new["CVCRC"] = os.path.join(config["CVC_SCRIPTS_DIR"], "cvcrc")
+        new["CVC_MODELS"] = os.path.join(config["CVC_SCRIPTS_DIR"], "models")
+
+    # 11. Heuristic Antenna Threshold
+    if new["PDK"].startswith("sky130"):
+        new["HEURISTIC_ANTENNA_THRESHOLD"] = 90
+    elif new["PDK"].startswith("gf180mcu"):
+        new["HEURISTIC_ANTENNA_THRESHOLD"] = 130
 
     # x1. Disconnected Modules (sky130)
     if new["PDK"].startswith("sky130"):
         new["IGNORE_DISCONNECTED_MODULES"] = "sky130_fd_sc_hd__conb_1"
 
     # x2. Invalid Variables (gf180mcu)
     if new["PDK"].startswith("gf180mcu"):
@@ -169,8 +237,9 @@
         del new["TRISTATE_BUFFER_MAP"]
 
         del new["KLAYOUT_DRC_TECH_SCRIPT"]
 
         new[
             "SYNTH_CLK_DRIVING_CELL"
         ] = f"{config['SYNTH_CLK_DRIVING_CELL']}/{config['SYNTH_DRIVING_CELL_PIN']}"
+
     return new
```

### Comparing `openlane-2.0.0b9/openlane/config/preprocessor.py` & `openlane-2.0.0rc2/openlane/config/preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,17 +281,21 @@
             return [final_abspath]
 
         in_exposed = [final_abspath.startswith(p) for p in readable_paths]
         if True not in in_exposed:
             raise PermissionError(
                 f"'{concatenated}' is not located any path readable to OpenLane"
             )
-        files = glob.glob(final_abspath)
+        files = sorted(glob.glob(final_abspath))
         files_escaped = [file.replace("$", r"\$") for file in files]
         files_escaped.sort()
+
+        if len(files_escaped) == 0:
+            files_escaped = [concatenated]
+
         return files_escaped
     else:
         return mutable
 
 
 PDK_PREFIX = "pdk::"
 SCL_PREFIX = "scl::"
```

### Comparing `openlane-2.0.0b9/openlane/config/removals.py` & `openlane-2.0.0rc2/openlane/config/removals.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,17 +17,29 @@
     "PL_RANDOM_GLB_PLACEMENT": "The random global placer no longer yields a tangible benefit with newer versions of OpenROAD.",
     "PL_RANDOM_INITIAL_PLACEMENT": "A random initial placer no longer yields a tangible benefit with newer versions of OpenROAD.",
     "KLAYOUT_XOR_GDS": "The GDS output is of limited utility compared to the XML database.",
     "KLAYOUT_XOR_XML": "The XML database is always generated.",
     "MAGIC_GENERATE_GDS": "The GDS view is always generated when MAGIC_RUN_STREAMOUT is set.",
     "CLOCK_BUFFER_FANOUT": "The simple CTS script that used this variable no longer exists.",
     "FP_IO_HMETAL": "Replaced by FP_IO_HLAYER in the PDK configuration variables, which uses a more specific layer name.",
-    "FP_IO_VMETAL": "Replaced by FP_IO_VLAYER in the PDK  configuration variables, which uses a more specific layer name.",
+    "FP_IO_VMETAL": "Replaced by FP_IO_VLAYER in the PDK configuration variables, which uses a more specific layer name.",
     "GLB_OPTIMIZE_MIRRORING": "Shares DPL_OPTIMIZE_MIRRORING.",
     "GRT_MAX_DIODE_INS_ITERS": "Relevant diode insertion strategies removed.",
     "TAKE_LAYOUT_SCROT": "Buggy/dubious utility.",
     "MAGIC_PAD": "Hacky/dubious utility.",
     "GENERATE_FINAL_SUMMARY_REPORT": "To be specified via API/CLI- not much of a configuration variable.",
     "USE_GPIO_PADS": "Add the pad's files to EXTRA_LEFS and EXTRA_VERILOG_MODELS as apprioriate.",
     "PL_ESTIMATE_PARASITICS": "Parasitics are always estimated whenever possible.",
     "GRT_ESTIMATE_PARASITICS": "Parasitics are always estimated whenever possible.",
+    "FP_PDN_AUTO_ADJUST": "Too situational. It's always best to be more explicit.",
+    "SYNTH_READ_BLACKBOX_LIB": "Changed to always be on.",
+    "CTS_TOLERANCE": "No longer supported by OpenROAD.",
+    "MAGIC_GDS_ALLOW_ABSTRACT": "Bad practice. If an abstract view is needed, a GDS file can be generated from the abstract LEF file.",
+    "PLACE_SITE_HEIGHT": "Now automatically extracted from PLACE_SITE.",
+    "PLACE_SITE_WIDTH": "Now automatically extracted from PLACE_SITE.",
+    "LEC_ENABLE": "Buggy/doesn't scale properly.",
+    "LVS_INSERT_POWER_PINS": "No longer necessary.",
+    "RUN_CVC": "Upstream no longer supports CVC for use within OpenLane.",
+    "FP_PADFRAME_CFG": "To be implemented.",
+    "FP_CONTEXT_DEF": "To be implemented.",
+    "FP_CONTEXT_LEF": "To be implemented.",
 }
```

### Comparing `openlane-2.0.0b9/openlane/config/variable.py` & `openlane-2.0.0rc2/openlane/config/variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import shlex
 import inspect
 from enum import Enum
 from decimal import Decimal, InvalidOperation
-from dataclasses import _MISSING_TYPE, MISSING, dataclass, field, fields, is_dataclass
+from dataclasses import (
+    _MISSING_TYPE,
+    MISSING,
+    asdict,
+    dataclass,
+    field,
+    fields,
+    is_dataclass,
+)
 from typing import (
     ClassVar,
     Dict,
     List,
     Literal,
     Optional,
     Set,
@@ -28,32 +36,56 @@
     Mapping,
     Callable,
     Type,
     Any,
     get_origin,
     get_args,
 )
-from ..state import DesignFormat
-from ..common import GenericDict, Path, is_string, zip_first
+from ..state import DesignFormat, State
+from ..common import GenericDict, Path, is_string, zip_first, Number, slugify
 
 # Scalar = Union[Type[str], Type[Decimal], Type[Path], Type[bool]]
 # VType = Union[Scalar, List[Scalar]]
 
 
+class Orientation(str, Enum):
+    N = "N"
+    FN = "FN"
+    W = "W"
+    FW = "FW"
+    S = "S"
+    FS = "FS"
+    E = "E"
+    FE = "FE"
+    # OpenAccess
+    R0 = "N"
+    MY = "FN"
+    R90 = "W"
+    MXR90 = "FW"
+    R180 = "S"
+    MX = "FS"
+    R270 = "E"
+    MYR90 = "FE"
+
+    def __str__(self) -> str:
+        return self.value
+
+
 @dataclass
 class Instance:
     """
     Location information for an instance of a Macro.
 
-    :param location: The physical co-ordinates of the Macro's origin.
-    :param orientation: Whether the Macro is facing North or South.
+    :param location: The physical co-ordinates of the Macro's origin. Leave
+        empty for automatic placement.
+    :param orientation: The orientation of the macro's placement. 'N'/'R0' by default.
     """
 
-    location: Tuple[Decimal, Decimal]
-    orientation: Union[Literal["N"], Literal["S"], Literal["FN"], Literal["FS"]]
+    location: Optional[Tuple[Decimal, Decimal]]
+    orientation: Optional[Orientation]
 
 
 @dataclass
 class Macro:
     """
     A data structure for storing definitions of Macros.
 
@@ -97,15 +129,17 @@
     :param json_h: A JSON file as generated by Yosys. Helpful in some flows.
     """
 
     gds: List[Path]
     lef: List[Path]
     instances: Dict[str, Instance] = field(default_factory=lambda: {})
 
+    vh: List[Path] = field(default_factory=lambda: [])
     nl: List[Path] = field(default_factory=lambda: [])
+    pnl: List[Path] = field(default_factory=lambda: [])
     spef: Dict[str, List[Path]] = field(default_factory=lambda: {})
     lib: Dict[str, List[Path]] = field(default_factory=lambda: {})
     spice: List[Path] = field(default_factory=lambda: [])
     sdf: Dict[str, List[Path]] = field(default_factory=lambda: {})
 
     json_h: Optional[Path] = None
 
@@ -123,14 +157,56 @@
                 "Macro definition invalid- at least one GDSII file must be specified."
             )
         if len(self.lef) < 1:
             raise ValueError(
                 "Macro definition invalid- at least one LEF file must be specified."
             )
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__qualname__}(%s)" % ", ".join(
+            [f"{k}={repr(v)}" for k, v in asdict(self).items()]
+        )
+
+    def __str__(self) -> str:
+        return self.__repr__()
+
+    @classmethod
+    def from_state(Self, state: State) -> "Macro":
+        kwargs = {}
+        for macro_field in fields(Self):
+            views = state.get(macro_field.name)
+            if views is None:
+                if macro_field.default_factory is not MISSING:
+                    kwargs[macro_field.name] = macro_field.default_factory()
+                elif macro_field.default is not MISSING:
+                    kwargs[macro_field.name] = macro_field.default
+                else:  # gds or lef
+                    raise ValueError(
+                        f"Macro cannot be made out of input state: View {macro_field.name} is missing"
+                    )
+                continue
+            var_name = f"{Self.__name__}.{macro_field.name}"
+            _, final = Variable(var_name, macro_field.type, "").compile(
+                GenericDict({var_name: views}),
+                warning_list_ref=[],
+                permissive_typing=True,
+            )
+            kwargs[macro_field.name] = final
+
+        return Self(**kwargs)  # type: ignore
+
+    def instantiate(
+        self,
+        instance_name: str,
+        location: Tuple[Number, Number],
+        orientation: Orientation = Orientation.N,
+    ):
+        location = (Decimal(location[0]), Decimal(location[1]))
+        self.instances[instance_name] = Instance(location, Orientation[orientation])
+
 
 def is_optional(t: Type[Any]) -> bool:
     type_args = get_args(t)
     return get_origin(t) is Union and type(None) in type_args
 
 
 def some_of(t: Type[Any]) -> Type[Any]:
@@ -165,28 +241,33 @@
         origin, args = get_origin(some), get_args(some)
         if origin is not None:
             if origin == Union:
                 arg_strings = [repr_type(arg) for arg in args]
                 type_string = "｜".join(arg_strings)
                 type_string = f"({type_string})"
             elif origin == Literal:
-                return str(args[0])
+                return "｜".join([repr(arg) for arg in args])
             else:
                 arg_strings = [repr_type(arg) for arg in args]
-                type_string = f"{type_string}[{','.join(arg_strings)}]"
+                type_string = f"{type_string}[{', '.join(arg_strings)}]"
 
     return type_string + ("?" if optional else "")
 
 
 @dataclass
 class Variable:
     """
-    An object representing a configuration variable for a PDK, a Flow or a Step.
+    An object encapsulating metadata on an OpenLane configuration variable, which
+    is used to name, document and validate values supplied to
+    :class:`openlane.steps.Step`\\s or :class:`openlane.flows.Flow`\\s.
+
+    Values supplied for configuration variables are the primary interface by
+    which users configure OpenLane flows.
 
-    :param name: A string name for the Variable. Because of backwards compatility
+    :param name: A string name for the Variable. Because of backwards compatibility
         with OpenLane 1, the convention is ``UPPER_SNAKE_CASE``.
 
     :param type: A Python type object representing the variable.
 
         Supported scalars:
 
         - ``int``
@@ -219,14 +300,29 @@
         An element of the list can alternative be a tuple of a name and a Callable
         used to perform a translation for when a renamed variable is also slightly
         modified.
 
     :param units: Used only in documentation: the unit corresponding to this
         object, i.e., µm, pF, etc. Can be any string, but for consistency, SI units
         must be represented in terms of their official symbols.
+
+    :param pdk: Whether this variable is expected to be given a default value
+        by a PDK or not.
+
+        If this is true, and the variable is not of an option type, a PDK *must*
+        give this variable a default value in order to be marked compatible
+        with a step.
+
+        If this is true and the variable is of an option type, a PDK may
+        optionally provide a default value for this variable, however steps
+        must presume it is ``null``.
+
+        If this is false, a PDK is not allowed to set a default value for
+        this variable. In current versions of OpenLane, the value will be
+        silently ignored, but warnings or errors may occur in future versions.
     """
 
     known_variable_names: ClassVar[Set[str]] = set()
 
     name: str
     type: Any
     description: str
@@ -244,37 +340,41 @@
             if isinstance(name, tuple):
                 name, _ = name
             Variable.known_variable_names.add(name)
 
     @property
     def optional(self) -> bool:
         """
-        Returns whether a variable's type is an `Option type <https://en.wikipedia.org/wiki/Option_type>`_.
+        :returns: Whether a variable's type is an `Option type <https://en.wikipedia.org/wiki/Option_type>`_.
         """
         return is_optional(self.type)
 
     @property
     def some(self) -> Any:
         """
-        Returns the type of a variable presuming it is not None.
+        :returns: The type of a variable presuming it is not None.
 
-        If a variable is not Optional, that is simply the type specified in the
-        :ivar:`type` field.
+            If a variable is not Optional, that is simply the type specified in the
+            ``type`` attribute.
         """
         return some_of(self.type)
 
-    def type_repr_md(self) -> str:  # pragma: no cover
+    def type_repr_md(self, for_document: bool = False) -> str:  # pragma: no cover
         """
-        Prints a pretty Markdown string representation of the Variable's type.
+        :param for_document: Adds HTML line breaks between sum type separators
+            for easier wrapping by web browsers/PDF renderers/what have you
+        :returns: A pretty Markdown string representation of the Variable's type.
         """
+        if for_document:
+            return repr_type(self.type).replace("｜", "｜<br />")
         return repr_type(self.type)
 
     def desc_repr_md(self) -> str:  # pragma: no cover
         """
-        Prints the description, but with newlines escaped for Markdown.
+        :returns: The description, but with newlines escaped for Markdown.
         """
         return self.description.replace("\n", "<br />")
 
     def __process(
         self,
         key_path: str,
         value: Any,
@@ -319,17 +419,17 @@
 
         type_origin = get_origin(validating_type)
         type_args = get_args(validating_type)
 
         if type_origin in [list, tuple]:
             return_value = list()
             raw = value
-            if isinstance(raw, list):
+            if isinstance(raw, list) or isinstance(raw, tuple):
                 pass
-            elif isinstance(raw, str):
+            elif is_string(raw):
                 if not permissive_typing:
                     raise ValueError(
                         f"Refusing to automatically convert string at '{key_path}' to list"
                     )
                 if "," in raw:
                     raw = raw.split(",")
                 elif ";" in raw:
@@ -356,29 +456,32 @@
                         value=item,
                         validating_type=value_type,
                         permissive_typing=permissive_typing,
                     )
                 )
 
             if type_origin == tuple:
-                return tuple(raw)
+                return tuple(return_value)
 
             return return_value
         elif type_origin == dict:
             raw = value
             key_type, value_type = type_args
             if isinstance(raw, dict):
                 pass
-            elif isinstance(raw, str):
+            elif isinstance(raw, list) or is_string(raw):
                 if not permissive_typing:
                     raise ValueError(
                         f"Refusing to automatically convert string at '{key_path}' to dict"
                     )
+                components = raw
+                if is_string(raw):
+                    components = shlex.split(raw)
+                assert isinstance(components, list)
                 # Assuming Tcl format:
-                components = shlex.split(value)
                 if len(components) % 2 != 0:
                     raise ValueError(
                         f"Tcl-style flat dictionary provided for variable '{key_path}' is invalid: uneven number of components ({len(components)})"
                     )
                 raw = {}
                 for i in range(0, len(components) // 2):
                     key = components[2 * i]
@@ -426,29 +529,31 @@
                     [
                         f"Value for '{key_path}' is invalid for union {repr_type(validating_type)}:"
                     ]
                     + errors
                 )
             )
         elif type_origin == Literal:
-            arg = type_args[0]
-            if value == arg:
+            if value in type_args:
                 return value
             else:
-                raise ValueError(f"Value for '{key_path}' is not '{arg}': '{value}'")
+                raise ValueError(
+                    f"Value for '{key_path}' is invalid for {repr_type(validating_type)}: '{value}'"
+                )
         elif is_dataclass(validating_type):
             if isinstance(value, validating_type):
                 # Do not validate further
                 return value
 
             raw = value
             if not isinstance(raw, dict):
                 raise ValueError(
                     f"Value provided for deserializable path {validating_type} at '{key_path}' is not a dictionary."
                 )
+            raw = value.copy()
             kwargs_dict = {}
             for current_field in fields(validating_type):
                 key = current_field.name
                 subtype = current_field.type
                 explicitly_specified = False
                 if key in raw:
                     explicitly_specified = True
@@ -466,35 +571,36 @@
                     value=field_value,
                     explicitly_specified=explicitly_specified,
                     default=field_default,
                     validating_type=subtype,
                     permissive_typing=permissive_typing,
                 )
                 kwargs_dict[key] = value__processed
+                if explicitly_specified:
+                    del raw[key]
+            if len(raw):
+                raise ValueError(
+                    f"One or more keys unrecognized for dataclass {validating_type.__qualname__}: {' '.join(raw.keys())}"
+                )
             return validating_type(**kwargs_dict)
         elif validating_type == Path:
             # Handle one-file globs
             if isinstance(value, list) and len(value) == 1:
                 value = value[0]
             result = Path(value)
-            try:
-                result.validate()
-            except ValueError as e:
-                raise ValueError(
-                    f"Path provided for variable '{key_path}' is invalid: '{e}'"
-                )
+            result.validate(f"Path provided for variable '{key_path}' is invalid")
             return result
         elif validating_type == bool:
             if not permissive_typing and not isinstance(value, bool):
                 raise ValueError(
-                    f"Refusing to automatically convert '{value}' at '{key_path}' to a boolean"
+                    f"Refusing to automatically convert '{value}' at '{key_path}' to a Boolean"
                 )
-            if value in ["1", "true", 1, True]:
+            if value in ["1", "true", "True", 1, True]:
                 return True
-            elif value in ["0", "false", 0, False]:
+            elif value in ["0", "false", "False", 0, False]:
                 return False
             else:
                 raise ValueError(
                     f"Value provided for variable '{key_path}' of type {validating_type.__name__} is invalid: '{value}'"
                 )
         elif issubclass(validating_type, Enum):
             if type(value) == validating_type:
@@ -575,14 +681,20 @@
             validating_type=self.type,
             explicitly_specified=exists is not None,
             permissive_typing=permissive_typing,
         )
 
         return (exists, processed)
 
+    def _get_docs_identifier(self, parent: Optional[str] = None) -> str:
+        identifier = f"var-{self.name.lower()}"
+        if parent is not None:
+            identifier = f"var-{slugify(parent)}-{self.name.lower()}"
+        return identifier
+
     def __hash__(self) -> int:
         return hash((self.name, self.type, self.default))
 
     def __eq__(self, rhs: object) -> bool:
         if not isinstance(rhs, Variable):
             raise NotImplementedError()
         return (
```

### Comparing `openlane-2.0.0b9/openlane/container.py` & `openlane-2.0.0rc2/openlane/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 ## This file is internal to OpenLane 2 and is not part of the API.
-
 import os
 import re
+import httpx
 import shlex
 import pathlib
 import getpass
 import tempfile
-import requests
 import subprocess
 from typing import List, Sequence, Optional, Union, Tuple
 
 from .logging import err, info, warn
 from .env_info import OSInfo
 
 CONTAINER_ENGINE = os.getenv("OPENLANE_CONTAINER_ENGINE", "docker")
@@ -104,22 +103,23 @@
     elif registry == "ghcr.io":
         url = f"https://ghcr.io/v2/{repo}/manifests/{tag}"
     else:
         err(f"Unknown registry '{registry}'.")
         return False
 
     try:
-        request = requests.get(url, headers={"Accept": "application/json"})
-        request.raise_for_status()
-    except requests.exceptions.ConnectionError:
+        httpx.Client(follow_redirects=True).get(
+            url, headers={"Accept": "application/json"}
+        )
+    except httpx.NetworkError:
         err("Couldn't connect to the internet to pull container images.")
         return False
-    except requests.exceptions.HTTPError:
+    except httpx.HTTPStatusError as e:
         err(
-            f"The image {image} was not found. This may be because the CI for this image is running- in which case, please try again later."
+            f"The image {image} was not found. This may be because the CI for this image is running- in which case, please try again later. (error: {e})"
         )
         return False
     return True
 
 
 def ensure_image(image: str) -> bool:
     if image_exists(image):
@@ -130,34 +130,44 @@
     except subprocess.CalledProcessError:
         err(f"Failed to pull image {image} from the container registries.")
         return False
 
     return True
 
 
-win_path_sep = re.compile(r"\\")
+dos_path_sep = re.compile(r"\\")
 
 
 def sanitize_path(path: Union[str, os.PathLike]) -> Tuple[str, str]:
+    """
+    :returns: A tuple of:
+        - The host path, processed ``abspath``
+        - The target path, on UNIX-like operating systems it's identical to the
+          host path, but on Windows, the path is translated to a valid UNIX path
+          as follows:
+          - Backslashes are converted into forward slashes
+          - The drive letter (e.g. C:) is converted to a root directory (e.g. /c)
+    """
     path_str = str(path)
     abspath = os.path.abspath(path_str)
     mountable_path = abspath
     if os.path.sep == "\\":
-        mountable_path = win_path_sep.sub("/", abspath)[2:]
+        mountable_path = f"/{abspath[0]}" + dos_path_sep.sub("/", abspath)[2:]
     return (abspath, mountable_path)
 
 
 def run_in_container(
     image: str,
     args: Sequence[str],
     pdk_root: Optional[str] = None,
     pdk: Optional[str] = None,
     scl: Optional[str] = None,
     other_mounts: Optional[Sequence[str]] = None,
     interactive: bool = False,
+    tty: bool = False,
 ) -> int:
     # If imported at the top level, would interfere with Conda where Volare
     # would not be installed.
     import volare
 
     osinfo = OSInfo.get()
     if not osinfo.supported:
@@ -167,14 +177,20 @@
 
     if osinfo.container_info is None:
         raise FileNotFoundError("No compatible container engine found.")
 
     if not ensure_image(image):
         raise ValueError(f"Failed to use image '{image}'.")
 
+    terminal_args = []
+    if interactive:
+        terminal_args.append("-i")
+    if tty:
+        terminal_args.append("-t")
+
     mount_args = []
     from_home, to_home = sanitize_path(pathlib.Path.home())
 
     mount_args += ["-v", f"{from_home}:{to_home}"]
 
     from_pdk, to_pdk = sanitize_path(volare.get_volare_home(pdk_root))
     mount_args += [
@@ -205,24 +221,27 @@
         f"{tempdir}:/tmp",
         "-e",
         "TMPDIR=/tmp",
     ]
 
     if other_mounts is not None:
         for mount in other_mounts:
-            mount_from, mount_to = sanitize_path(mount)
-            mount_args += ["-v", f"{mount_from}:{mount_to}"]
+            if os.path.isdir(mount):
+                mount_from, mount_to = sanitize_path(mount)
+                mount_args += ["-v", f"{mount_from}:{mount_to}"]
+            else:
+                mount_args += ["-v", f"{mount}"]
 
     cmd = (
         [
             CONTAINER_ENGINE,
             "run",
             "--rm",
-            "-ti" if interactive else "-t",
         ]
+        + terminal_args
         + permission_args(osinfo)
         + mount_args
         + gui_args(osinfo)
         + [image]
         + list(args)
     )
```

### Comparing `openlane-2.0.0b9/openlane/env_info.py` & `openlane-2.0.0rc2/openlane/env_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import re
 import sys
 import json
 import platform
 import subprocess
 
 try:
-    from typing import Optional  # noqa: F401
+    from typing import Optional, Dict, List, Any  # noqa: F401
 except ImportError:
     pass
 
 CONTAINER_ENGINE = os.getenv("OPENLANE_CONTAINER_ENGINE", "docker")
 
 
 class StringRepresentable(object):
@@ -60,21 +60,23 @@
         try:
             cinfo = ContainerInfo()
 
             try:
                 info_str = subprocess.check_output(
                     [CONTAINER_ENGINE, "info", "--format", "{{json .}}"]
                 ).decode("utf8")
-            except Exception:
-                return None
+            except Exception as e:
+                raise Exception("Failed to get Docker info: %s" % str(e)) from None
 
             try:
                 info = json.loads(info_str)
-            except Exception:
-                raise Exception("Result from 'docker info' was not valid JSON.")
+            except Exception as e:
+                raise Exception(
+                    "Result from 'docker info' was not valid JSON: %s" % str(e)
+                ) from None
 
             if info.get("host") is not None:
                 if info["host"].get("conmon") is not None:
                     cinfo.conmon = True
                     if (
                         info["host"].get("remoteSocket") is not None
                         and "podman" in info["host"]["remoteSocket"]["path"]
@@ -106,33 +108,99 @@
 
             return cinfo
         except Exception as e:
             print(e, file=sys.stderr)
             return None
 
 
+class NixInfo(StringRepresentable):
+    version = ""  # type: str
+    multi_user = False  # type: bool
+    sandbox = False  # type: bool
+    channels = None  # type: Optional[Dict[str, List[str]]]
+    nixpkgs = ""  # type: str
+
+    def __init__(self) -> None:
+        self.version = ""  # type: str
+        self.multi_user = False  # type: bool
+        self.sandbox = False  # type: bool
+        self.channels = None  # type: Optional[Dict[str, List[str]]]
+        self.nixpkgs = ""  # type: str
+
+    @staticmethod
+    def get():
+        # type: () -> Optional['NixInfo']
+        ninfo = NixInfo()
+
+        try:
+            try:
+                info_str = subprocess.check_output(
+                    ["nix-shell", "-p", "nix-info", "--run", "nix-info -m"]
+                ).decode("utf8")
+            except Exception as e:
+                raise Exception("Failed to get Docker info: %s" % str(e)) from None
+
+            for line in info_str.splitlines():
+                if line.strip() == "":
+                    continue
+                line = line[3:]
+                key, value_raw = line.split(": ", maxsplit=1)
+                key = key.strip(" -")
+                value = value_raw.strip(' `"')  # type: Any
+                if value == "yes":
+                    value = True
+                elif value == "no":
+                    value = False
+                if key in ninfo.__dict__:
+                    setattr(ninfo, key, value)
+                elif key.startswith("channels"):
+                    user = key[len("channels") + 1 : -1]
+                    ninfo.channels = ninfo.channels or {}
+                    ninfo.channels[user] = [
+                        el.strip() for el in value.split(",") if el.strip() != ""
+                    ]
+                elif key.startswith("multi-user"):
+                    ninfo.multi_user = value
+
+            return ninfo
+        except Exception as e:
+            print(e, file=sys.stderr)
+            return None
+
+
 class OSInfo(StringRepresentable):
     kernel = ""  # type: str
-    python_version = ""  # type: str
     kernel_version = ""  # type: str
+    supported = False  # type: bool
     distro = None  # type: Optional[str]
     distro_version = None  # type: Optional[str]
+    python_version = ""  # type: str
+    python_path = []  # type: List[str]
     container_info = None  # type: Optional[ContainerInfo]
-    supported = False  # type: bool
+    nix_info = None  # type: Optional[NixInfo]
 
     def __init__(self):
         self.kernel = platform.system()
-        self.python_version = platform.python_version()
         self.kernel_version = (
             platform.release()
         )  # Unintuitively enough, it's the kernel's release
+        self.supported = self.kernel in ["Darwin", "Linux", "Windows"]
         self.distro = None
         self.distro_version = None
+        self.python_version = platform.python_version()
+        self.python_path = sys.path.copy()
+        self.tkinter = False
+        try:
+            import tkinter  # noqa: F401
+
+            self.tkinter = True
+        except ImportError:
+            pass
         self.container_info = None
-        self.supported = self.kernel in ["Darwin", "Linux", "Windows"]
+        self.nix_info = None
 
     @staticmethod
     def get():
         # type: () -> 'OSInfo'
         osinfo = OSInfo()
 
         if osinfo.kernel == "Windows":
@@ -171,13 +239,49 @@
                     "DISTRIB_RELEASE"
                 )
 
             else:
                 print("Failed to get distribution info.", file=sys.stderr)
 
         osinfo.container_info = ContainerInfo.get()
-
+        osinfo.nix_info = NixInfo.get()
         return osinfo
 
 
+def env_info_cli():
+    def print_params(obj, indent=0):
+        if isinstance(obj, list):
+            for value in obj:
+                if isinstance(value, StringRepresentable) or isinstance(value, dict):
+                    print("%s- " % (" " * indent), end="")
+                    print_params(value, indent=indent + 2)
+                elif isinstance(value, list):
+                    if len(value) == 0:
+                        print("%s- []" % (" " * indent))
+                    else:
+                        print("%s- " % (" " * indent), end="")
+                        print_params(value, indent=indent + 2)
+                else:
+                    print("%s- %s" % (" " * indent, value))
+
+        else:
+            current = obj if isinstance(obj, dict) else obj.__dict__
+            for key in current:
+                value = current[key]
+                if isinstance(value, StringRepresentable) or isinstance(value, dict):
+                    print("%s%s:" % (" " * indent, key))
+                    print_params(value, indent=indent + 2)
+                elif isinstance(value, list):
+                    if len(value) == 0:
+                        print("%s%s: []" % (" " * indent, key))
+                    else:
+                        print("%s%s:" % (" " * indent, key))
+                        print_params(value, indent=indent + 2)
+                else:
+                    print("%s%s: %s" % (" " * indent, key, value))
+
+    info = OSInfo.get()
+    print_params(info)
+
+
 if __name__ == "__main__":
-    print(OSInfo.get())
+    env_info_cli()
```

### Comparing `openlane-2.0.0b9/openlane/flows/__init__.py` & `openlane-2.0.0rc2/openlane/flows/builtins.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,18 +7,12 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-The Flow Module
----------------
-
-An API for implementing new flows using the OpenLane infrastructure, as well
-as a number of built-in flows.
-"""
-from .flow import FlowError, FlowException, FlowProgressBar, Flow
-from .sequential import SequentialFlow
-from . import builtins
-from .cli import cloup_flow_opts
+# flake8: noqa
+from .optimizing import Optimizing
+from .classic import Classic, VHDLClassic
+from .misc import OpenInKLayout, OpenInOpenROAD
+from .synth_explore import SynthesisExploration
```

### Comparing `openlane-2.0.0b9/openlane/flows/builtins.py` & `openlane-2.0.0rc2/openlane/scripts/magic/wrapper.tcl`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-# Copyright 2023 Efabless Corporation
+# Copyright 2020-2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# flake8: noqa
-from .optimizing import Optimizing
-from .classic import Classic
-from .misc import OpenInKLayout, OpenInOpenROAD
+source $::env(_TCL_ENV_IN)
+
+if {[catch {source $::env(MAGIC_SCRIPT)} err]} {
+    puts "Error: $err"
+    exit 1
+}
```

### Comparing `openlane-2.0.0b9/openlane/flows/cli.py` & `openlane-2.0.0rc2/openlane/flows/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-from textwrap import dedent
 from functools import partial
 from concurrent.futures import ThreadPoolExecutor
 from typing import Optional, Union
 
 
 from click import Parameter, echo
 from cloup import (
@@ -28,28 +27,28 @@
     Path,
 )
 from cloup.constraints import (
     mutually_exclusive,
 )
 from cloup.typing import Decorator
 
-from openlane.state.state import InvalidState
-
-
 from .flow import Flow
-from ..common import set_tpe, get_opdks_rev
-from ..logging import set_log_level, err, LogLevelsDict
-from ..state import State
+from ..common import set_tpe, get_opdks_rev, cli
+from ..logging import set_log_level, verbose, err, options, LogLevels
+from ..state import State, InvalidState
 
 
 def set_log_level_cb(
     ctx: Context,
     param: Parameter,
-    value: str,
+    value: Optional[str],
 ):
+    if value is None:
+        return
+
     level: Union[str, int] = value
     try:
         try:
             level = int(value)
         except ValueError:
             pass
         set_log_level(level)
@@ -130,35 +129,71 @@
     if param.name is None:
         return
 
     values = ctx.params.copy()
     values[param.name] = value
     if "pdk" in values and "scl" in values:
         pdk = values["pdk"]
-        pdk_family = pdk[:-1]
         if ctx.obj and ctx.obj.get("use_volare"):
             import volare
 
-            pdk_root = volare.get_volare_home(values["pdk_root"])
+            volare_home = volare.get_volare_home(values["pdk_root"])
 
-            volare.enable(pdk_root, pdk_family, get_opdks_rev())
+            include_libraries = ["default"]
+            if scl := values["scl"]:
+                include_libraries.append(scl)
+
+            pdk_family = None
+            if family := volare.Family.by_name.get(pdk):
+                ctx.params["pdk"] = family.default_variant
+                pdk_family = family.name
+                verbose(f"Resolved PDK variant {family.default_variant}.")
+            else:
+                for family in volare.Family.by_name.values():
+                    if pdk in family.variants:
+                        pdk_family = family.name
+                        break
+
+            if pdk_family is None:
+                err(f"Could not resolve the PDK '{ctx.params['pdk']}'.")
+                ctx.exit(1)
+
+            version = volare.fetch(
+                volare_home,
+                pdk_family,
+                get_opdks_rev(),
+                include_libraries=include_libraries,
+            )
+            ctx.params["pdk_root"] = version.get_dir(volare_home)
     return value
 
 
+def condensed_cb(ctx: Context, param: Parameter, value: bool):
+    if value:
+        options.set_condensed_mode(True)
+        options.set_show_progress_bar(False)
+
+
+def progressbar_cb(ctx: Context, param: Parameter, value: Optional[bool]):
+    if value is not None:
+        options.set_show_progress_bar(value)
+
+
 def cloup_flow_opts(
     *,
     config_options: bool = True,
     run_options: bool = True,
     sequential_flow_controls: bool = True,
     sequential_flow_reproducible: bool = False,
     pdk_options: bool = True,
     log_level: bool = True,
     jobs: bool = True,
     accept_config_files: bool = True,
     volare_by_default: bool = True,
+    _enable_debug_flags: bool = False,
 ) -> Decorator:
     """
     Creates a wrapper that appends a number of OpenLane flow-related flags to a
     function decorated with @cloup.command (https://cloup.readthedocs.io/en/stable/autoapi/cloup/index.html#cloup.command).
 
     The following keyword arguments will be passed to the decorated function.
     * Those postfixed ‡ are compatible with the constructor for :class:`Flow`.
@@ -212,40 +247,66 @@
                 ),
                 o(
                     "-c",
                     "--override-config",
                     "config_override_strings",
                     type=str,
                     multiple=True,
-                    help="For this run only- override a configuration variable with a certain value. In the format KEY=VALUE. Can be specified multiple times. Values must be valid JSON values.",
+                    help="For this run only- override a configuration variable with a certain value. In the format KEY=VALUE. Can be specified multiple times. Values must be valid JSON values, and keys must not use their deprecated names.",
                 ),
             )(f)
         if run_options:
+            f = o(
+                "-i",
+                "--with-initial-state",
+                type=Path(
+                    exists=True,
+                    file_okay=True,
+                    dir_okay=False,
+                ),
+                default=None,
+                callback=initial_state_cb,
+                help="Use this JSON file as an initial state. If this is not specified, the latest `state_out.json` of the run directory will be used if available.",
+            )(f)
+            f = o(
+                "--design-dir",
+                "design_dir",
+                type=Path(
+                    exists=True,
+                    file_okay=False,
+                    dir_okay=True,
+                ),
+                default=None,
+                help="The top-level directory for your design that configuration objects may resolve paths relative to.",
+            )(f)
+            if _enable_debug_flags:
+                f = option_group(
+                    "Debug flags",
+                    o(
+                        "--force-run-dir",
+                        "_force_run_dir",
+                        type=Path(
+                            exists=True,
+                            file_okay=False,
+                            dir_okay=True,
+                        ),
+                        hidden=True,
+                        default=None,
+                    ),
+                )(f)
             f = option_group(
                 "Run options",
                 o(
                     "--run-tag",
                     "tag",
                     default=None,
                     type=str,
                     help="An optional name to use for this particular run of an OpenLane-based flow. Used to create the run directory.",
                 ),
                 o(
-                    "-i",
-                    "--with-initial-state",
-                    type=Path(
-                        exists=True,
-                        file_okay=True,
-                        dir_okay=False,
-                    ),
-                    default=None,
-                    callback=initial_state_cb,
-                    help="Use this JSON file as an initial state. If this is not specified, the latest `state_out.json` of the run directory will be used if available.",
-                ),
-                o(
                     "--last-run",
                     is_flag=True,
                     default=False,
                     help="Use the last run as the run tag.",
                 ),
                 constraint=mutually_exclusive,
             )(f)
@@ -291,28 +352,37 @@
                 "--reproducible",
                 type=str,
                 help="Create a reproducible for the step matching this ID, then abort the flow. Supported by sequential flows.",
             )(f)
         if log_level:
             f = o(
                 "--log-level",
-                type=str,
-                default="VERBOSE",
-                help=dedent(
-                    """
-                    A logging level. Set to INFO or higher to silence subprocess logs.
-
-                    You can provide either a number or a string out of the following (higher is more silent):
-                    """
-                )
-                + ",".join(
-                    [f"{name}={value}" for name, value in LogLevelsDict.items()]
-                ),
+                type=cli.IntEnumChoice(LogLevels),
+                default=None,
+                help="A logging level. Set to VERBOSE or higher to silence subprocess logs. [default: unchanged from SUBPROCESS]",
                 callback=set_log_level_cb,
                 expose_value=False,
+                show_default=False,
+            )(f)
+            f = o(
+                "--show-progress-bar/--hide-progress-bar",
+                type=bool,
+                help="Whether to show the progress bar when running Flows. [default: show]",
+                default=None,
+                callback=progressbar_cb,
+                expose_value=False,
+            )(f)
+            f = o(
+                "--condensed/--full",
+                type=bool,
+                help="In condensed mode, subprocess logs are suppressed regardless of step, --hide-progress-bar is the default, and the log messages themselves are a bit more terse. Useful for debugging.",
+                default=False,
+                is_eager=True,
+                callback=condensed_cb,
+                expose_value=False,
             )(f)
         if pdk_options:
             f = option_group(
                 "PDK options",
                 o(
                     "--volare-pdk/--manual-pdk",
                     "use_volare",
@@ -321,15 +391,14 @@
                     help="Automatically use Volare for PDK version installation and enablement. Set --manual if you want to use a custom PDK version.",
                     expose_value=False,
                     callback=use_volare_cb,
                 ),
                 o(
                     "--pdk-root",
                     type=Path(
-                        exists=True,
                         file_okay=False,
                         dir_okay=True,
                     ),
                     is_eager=True,
                     default=os.environ.pop("PDK_ROOT", None),
                     help="Override volare PDK root folder. Required if Volare is not installed.",
                 ),
```

### Comparing `openlane-2.0.0b9/openlane/flows/flow.py` & `openlane-2.0.0rc2/openlane/flows/flow.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
-
 import os
 import glob
+import shutil
+import fnmatch
 import logging
 import datetime
 import textwrap
-import contextlib
+from io import StringIO
 from abc import abstractmethod, ABC
 from concurrent.futures import Future
 from functools import wraps
 from typing import (
     List,
     Sequence,
     Tuple,
@@ -40,30 +41,38 @@
     TextColumn,
     BarColumn,
     MofNCompleteColumn,
     TimeElapsedColumn,
     TaskID,
 )
 from deprecated.sphinx import deprecated
+from openlane.common.types import Path
 
-from ..config import (
-    Config,
-    Variable,
-    universal_flow_config_variables,
-)
-from ..state import State
-from ..steps import Step
+from ..config import Config, Variable, universal_flow_config_variables, AnyConfigs
+from ..state import State, DesignFormat, DesignFormatObject
+from ..steps import Step, StepNotFound
 from ..logging import (
+    LevelFilter,
     console,
     info,
+    warn,
     verbose,
     register_additional_handler,
     deregister_additional_handler,
+    options,
+)
+from ..common import (
+    get_tpe,
+    mkdirp,
+    protected,
+    final,
+    slugify,
+    Toolbox,
+    get_latest_file,
 )
-from ..common import get_tpe, mkdirp, protected, final, slugify, Toolbox
 
 
 class FlowError(RuntimeError):
     """
     A ``RuntimeError`` that occurs when a Flow, or one of its underlying Steps,
     fails to finish execution properly.
     """
@@ -132,14 +141,15 @@
         self.__ordinal: int = starting_ordinal
         self.__progress = Progress(
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             MofNCompleteColumn(),
             TimeElapsedColumn(),
             console=console,
+            disable=not options.get_show_progress_bar(),
         )
 
     def start(self):
         """
         Starts rendering the progress bar.
         """
         self.__progress.start()
@@ -201,51 +211,75 @@
             self.__ordinal += 1
         self.__progress.update(self.__task_id, completed=float(self.__stages_completed))
 
     @ensure_progress_started
     def get_ordinal_prefix(self) -> str:
         """
         :returns: A string with the current step ordinal, which can be
-        used to create a step directory.
+            used to create a step directory.
         """
         max_stage_digits = len(str(self.__max_stage))
-        return f"%0{max_stage_digits}d-" % self.__ordinal
+        return f"{str(self.__ordinal).zfill(max_stage_digits)}-"
+
+
+class _StepWarningFilter(LevelFilter):
+    def __init__(self) -> None:
+        super().__init__(["WARNING"])
+
+    def filter(self, record: logging.LogRecord) -> bool:
+        if hasattr(record, "step"):
+            record.step = f"[{record.step}] "
+        else:
+            record.step = ""
+        return super().filter(record)
 
 
 class Flow(ABC):
     """
     An abstract base class for a flow.
 
-    Flows encapsulates a subroutine that runs multiple steps: either synchronously,
-    asynchronously, serially or in any manner.
+    Flows encapsulate a the running of multiple :class:`Step`\\s in any order.
+    The sequence (or lack thereof) of running the steps is left to the Flow
+    itself.
 
     The Flow ABC offers a number of convenience functions, including handling the
     progress bar at the bottom of the terminal, which shows what stage the flow
     is currently in and the remaining stages.
 
-    :param config: Either a resolved :class:`Config` object, or an input to
-        :meth:`Config.load`.
+    :param config: Either a resolved :class:`openlane.config.Config` object, or an
+        input to :meth:`openlane.config.Config.load`.
 
     :param name: An optional string name for the Flow itself, and not a run of it.
 
-        If not set, the Python class name will be used instead.
+        If not provided, there are two fallbacks:
+
+        * The value of the ``name`` property (``NotImplemented`` by default)
+        * The name of the concrete ``Flow`` class
 
-    :param config_override_strings: See :meth:`Config.load`
-    :param pdk: See :meth:`Config.load`
-    :param pdk_root: See :meth:`Config.load`
-    :param scl: See :meth:`Config.load`
-    :param design_dir: See :meth:`Config.load`
+    :param config_override_strings: See :meth:`openlane.config.Config.load`
+    :param pdk: See :meth:`openlane.config.Config.load`
+    :param pdk_root: See :meth:`openlane.config.Config.load`
+    :param scl: See :meth:`openlane.config.Config.load`
+    :param design_dir: See :meth:`openlane.config.Config.load`
 
-    :ivar Steps:
+    :cvar Steps:
         A list of :class:`Step` **types** used by the Flow (not Step objects.)
 
-        Subclasses of :class:`Step` are expected to override the default value
+        Subclasses of :class:`Flow` are expected to override the default value
         as a class member- but subclasses may allow this value to be further
         overridden during construction (and only then.)
 
+        :class:`Flow` subclasses without the ``Steps`` class property declared
+        are considered abstract and cannot be initialized.
+
+    :cvar config_vars:
+        A list of **flow-specific** configuration variables. These configuration
+        variables are used entirely within the logic of the flow itself and
+        are not exposed to ``Step``\\(s).
+
     :ivar step_objects:
         A list of :class:`Step` **objects** from the last run of the flow,
         if it exists.
 
         If :meth:`start` is called again, the reference is destroyed.
 
     :ivar run_dir:
@@ -253,34 +287,53 @@
 
         If :meth:`start` is called again, the reference is destroyed.
 
     :ivar toolbox:
         The :class:`Toolbox` of the last run of the flow, if it exists.
 
         If :meth:`start` is called again, the reference is destroyed.
+
+    :ivar config_resolved_path:
+        The path to the serialization of the resolved configuration for the
+        last run of the flow.
+
+        If :meth:`start` is called again, the reference is destroyed.
     """
 
-    name: str
-    Steps: List[Type[Step]] = []  # Override
+    name: str = NotImplemented
+    Steps: List[Type[Step]] = NotImplemented  # Override
+    config_vars: List[Variable] = []
     step_objects: Optional[List[Step]] = None
     run_dir: Optional[str] = None
     toolbox: Optional[Toolbox] = None
+    config_resolved_path: Optional[str] = None
 
     def __init__(
         self,
-        config: Union[Config, str, os.PathLike, Dict],
+        config: AnyConfigs,
         *,
         name: Optional[str] = None,
         pdk: Optional[str] = None,
         pdk_root: Optional[str] = None,
         scl: Optional[str] = None,
         design_dir: Optional[str] = None,
         config_override_strings: Optional[Sequence[str]] = None,
     ):
-        self.name = name or self.__class__.__name__
+        if self.__class__.Steps == NotImplemented:
+            raise NotImplementedError(
+                f"Abstract flow {self.__class__.__qualname__} does not implement the .Steps property and cannot be initialized."
+            )
+        for step in self.Steps:
+            step.assert_concrete("used in a Flow")
+
+        self.name = (
+            self.__class__.__name__ if self.name == NotImplemented else self.name
+        )
+        if name is not None:
+            self.name = name
 
         self.Steps = self.Steps.copy()  # Break global reference
 
         if not isinstance(config, Config):
             config, design_dir = Config.load(
                 config_in=config,
                 flow_config_vars=self.get_all_config_variables(),
@@ -292,25 +345,26 @@
             )
 
         self.config: Config = config
         self.design_dir: str = str(self.config["DESIGN_DIR"])
         self.progress_bar = FlowProgressBar(self.name)
 
     @classmethod
-    def get_help_md(Self):  # pragma: no cover
+    def get_help_md(Self) -> str:  # pragma: no cover
         """
-        Renders Markdown help for this flow to a string.
+        :returns: rendered Markdown help for this Flow
         """
         doc_string = ""
         if Self.__doc__:
             doc_string = textwrap.dedent(Self.__doc__)
 
         result = (
             textwrap.dedent(
                 f"""\
+                (flow-{slugify(Self.__name__, lower=True)})=
                 ### {Self.__name__}
 
                 ```{{eval-rst}}
                 %s
                 ```
 
                 #### Using from the CLI
@@ -326,26 +380,69 @@
 
                 {Self.__name__} = Flow.factory.get("{Self.__name__}")
                 ```
                 """
             )
             % doc_string
         )
+        flow_config_vars = Self.config_vars
+
+        if len(flow_config_vars):
+            result += textwrap.dedent(
+                f"""
+                ({slugify(Self.__name__, lower=True)}-config-vars)=
+
+                #### Flow-specific Configuration Variables
+
+                | Variable Name | Type | Description | Default | Units |
+                | - | - | - | - | - |
+                """
+            )
+            for var in flow_config_vars:
+                units = var.units or ""
+                pdk_superscript = "<sup>PDK</sup>" if var.pdk else ""
+                result += f"| `{var.name}`{{#{var._get_docs_identifier(Self.__name__)}}}{pdk_superscript} | {var.type_repr_md()} | {var.desc_repr_md()} | `{var.default}` | {units} |\n"
+            result += "\n"
+
         if len(Self.Steps):
             result += "#### Included Steps\n"
             for step in Self.Steps:
-                result += f"* [`{step.id}`](./step_config_vars.md#{step.id})\n"
+                if hasattr(step, "long_name"):
+                    name = step.long_name
+                elif hasattr(step, "name"):
+                    name = step.name
+                else:
+                    name = step.id
+                result += f"* [`{step.id}`](./step_config_vars.md#{slugify(name)})\n"
 
         return result
 
     def get_all_config_variables(self) -> List[Variable]:
+        """
+        :returns: All configuration variables for this Flow, including
+            universal configuration variables, flow-specific configuration
+            variables and step-specific configuration variables.
+        """
         flow_variables_by_name: Dict[str, Tuple[Variable, str]] = {
-            variable.name: (variable, "Universal")
+            variable.name: (variable, "universal flow variables")
             for variable in universal_flow_config_variables
         }
+
+        for variable in self.config_vars:
+            if flow_variables_by_name.get(variable.name) is not None:
+                existing_variable, source = flow_variables_by_name[variable.name]
+                if variable != existing_variable:
+                    raise FlowException(
+                        f"Misconfigured flow: Unrelated variables in {source} and flow-specific variables share a name: {variable.name}"
+                    )
+            flow_variables_by_name[variable.name] = (
+                variable,
+                "flow-specific variables",
+            )
+
         for step_cls in self.Steps:
             for variable in step_cls.config_vars:
                 if flow_variables_by_name.get(variable.name) is not None:
                     existing_variable, existing_step = flow_variables_by_name[
                         variable.name
                     ]
                     if variable != existing_variable:
@@ -372,14 +469,18 @@
 
     @final
     def start(
         self,
         with_initial_state: Optional[State] = None,
         tag: Optional[str] = None,
         last_run: bool = False,
+        _force_run_dir: Optional[str] = None,
+        _no_load_previous_steps: bool = False,
+        *,
+        overwrite: bool = False,
         **kwargs,
     ) -> State:
         """
         The entry point for a flow.
 
         :param with_initial_state: An optional initial state object to use.
             If not provided:
@@ -392,125 +493,166 @@
             under the directory ``runs/`` in the design directory.
         :param last_run: Use the latest run (by modification time) as the tag.
 
             If no runs exist, a :class:`FlowException` will be raised.
 
             If ``last_run`` and ``tag`` are both set, a :class:`FlowException` will
             also be raised.
+        :param overwrite: If true and a run with the desired tag was found, the
+            contents will be deleted instead of appended.
 
         :returns: ``(success, state_list)``
         """
-        if last_run:
-            if tag is not None:
-                raise FlowException("tag and last_run cannot be used simultaneously.")
 
-            runs = glob.glob(os.path.join(self.design_dir, "runs", "*"))
+        handlers: List[logging.Handler] = []
+
+        warning_stream = StringIO()
+        warning_stream_handler = logging.StreamHandler(warning_stream)
+        warning_stream_handler.setLevel("WARNING")
+        warning_stream_handler.addFilter(_StepWarningFilter())
+        formatter = logging.Formatter("%(step)s%(message)s")
+        warning_stream_handler.setFormatter(formatter)
+        handlers.append(warning_stream_handler)
+        register_additional_handler(warning_stream_handler)
+
+        if last_run and tag is not None:
+            raise FlowException("tag and last_run cannot be used simultaneously.")
+
+        tag = tag or datetime.datetime.now().astimezone().strftime(
+            "RUN_%Y-%m-%d_%H-%M-%S"
+        )
+        if last_run:
+            runs = sorted(glob.glob(os.path.join(self.design_dir, "runs", "*")))
 
             latest_time: float = 0
             latest_run: Optional[str] = None
             for run in runs:
                 time = os.path.getmtime(run)
                 if time > latest_time:
                     latest_time = time
                     latest_run = run
 
             if latest_run is not None:
                 tag = os.path.basename(latest_run)
             else:
                 raise FlowException("last_run used without any existing runs")
 
-        if tag is None:
-            tag = datetime.datetime.now().astimezone().strftime("RUN_%Y-%m-%d_%H-%M-%S")
-
-        # Stored until next start()
-        self.run_dir = os.path.join(self.design_dir, "runs", tag)
         # Stored until next start()
-        self.toolbox = Toolbox(os.path.join(self.run_dir, "tmp"))
-
+        self.run_dir = os.path.abspath(
+            _force_run_dir or os.path.join(self.design_dir, "runs", tag)
+        )
         initial_state = with_initial_state or State()
 
+        self.step_objects = []
         starting_ordinal = 1
         try:
             entries = os.listdir(self.run_dir)
             if len(entries) == 0:
                 raise FileNotFoundError(self.run_dir)  # Treat as non-existent directory
+            elif overwrite:
+                shutil.rmtree(self.run_dir)
+                raise FileNotFoundError(self.run_dir)  # Treat as non-existent directory
+
             info(f"Using existing run at '{tag}' with the '{self.name}' flow.")
 
-            # Extract maximum step ordinal
-            for entry in entries:
-                components = entry.split("-")
-                if len(components) < 2:
-                    continue
+            # Extract maximum step ordinal + load finished steps
+            entries_sorted = sorted(
+                filter(
+                    lambda x: "-" in x and x.split("-", maxsplit=1)[0].isdigit(),
+                    entries,
+                ),
+                key=lambda x: int(x.split("-", maxsplit=1)[0]),
+            )
+            for entry in entries_sorted:
+                components = entry.split("-", maxsplit=1)
+
                 try:
                     extracted_ordinal = int(components[0])
                 except ValueError:
                     continue
+
+                if not _no_load_previous_steps:
+                    try:
+                        self.step_objects.append(
+                            Step.load_finished(
+                                os.path.join(self.run_dir, entry),
+                                self.config["PDK_ROOT"],
+                                self.Steps,
+                            )
+                        )
+                    except StepNotFound as e:
+                        raise FlowException(
+                            f"Error while loading concluded step in {entry}: {e}"
+                        )
+                    except FileNotFoundError:
+                        pass
+
                 starting_ordinal = max(starting_ordinal, extracted_ordinal + 1)
 
             # Extract Maximum State
             if with_initial_state is None:
-                latest_time = 0
-                latest_json: Optional[str] = None
-                state_out_jsons = glob.glob(
-                    os.path.join(self.run_dir, "*", "state_out.json")
-                )
-                for state_out_json in state_out_jsons:
-                    time = os.path.getmtime(state_out_json)
-                    if time > latest_time:
-                        latest_time = time
-                        latest_json = state_out_json
-
-                if latest_json is not None:
+                if latest_json := get_latest_file(self.run_dir, "state_out.json"):
                     verbose(f"Using state at '{latest_json}'.")
 
                     initial_state = State.loads(
                         open(latest_json, encoding="utf8").read()
                     )
 
         except NotADirectoryError:
             raise FlowException(
                 f"Run directory for '{tag}' already exists as a file and not a directory."
             )
         except FileNotFoundError:
             info(f"Starting a new run of the '{self.name}' flow with the tag '{tag}'.")
             mkdirp(self.run_dir)
 
-        warning_log_path = os.path.join(self.run_dir, "warnings.log")
-        warning_handler = logging.FileHandler(warning_log_path, mode="a+")
-        warning_handler.setLevel("WARNING")
-        register_additional_handler(warning_handler)
-
-        error_log_path = os.path.join(self.run_dir, "errors.log")
-        error_handler = logging.FileHandler(error_log_path, mode="a+")
-        error_handler.setLevel("ERROR")
-        register_additional_handler(error_handler)
-
-        with contextlib.ExitStack() as stack:
-            stack.callback(deregister_additional_handler, warning_handler)
-            stack.callback(deregister_additional_handler, error_handler)
-
-        config_res_path = os.path.join(self.run_dir, "resolved.json")
-        with open(config_res_path, "w") as f:
-            f.write(self.config.dumps())
-
-        self.progress_bar = FlowProgressBar(
-            self.name, starting_ordinal=starting_ordinal
-        )
-        self.progress_bar.start()
-        final_state, step_objects = self.run(
-            initial_state=initial_state,
-            starting_ordinal=starting_ordinal,
-            **kwargs,
-        )
-        self.progress_bar.end()
-
         # Stored until next start()
-        self.step_objects = step_objects
+        self.toolbox = Toolbox(os.path.join(self.run_dir, "tmp"))
 
-        return final_state
+        for level in ["WARNING", "ERROR"]:
+            path = os.path.join(self.run_dir, f"{level.lower()}.log")
+            handler = logging.FileHandler(path, mode="a+")
+            handler.setLevel(level)
+            handler.addFilter(LevelFilter([level]))
+            handlers.append(handler)
+            register_additional_handler(handler)
+
+        path = os.path.join(self.run_dir, "flow.log")
+        handler = logging.FileHandler(path, mode="a+")
+        handler.setLevel("VERBOSE")
+        handlers.append(handler)
+        register_additional_handler(handler)
+
+        try:
+            self.config_resolved_path = os.path.join(self.run_dir, "resolved.json")
+            with open(self.config_resolved_path, "w") as f:
+                f.write(self.config.dumps())
+
+            self.progress_bar = FlowProgressBar(
+                self.name, starting_ordinal=starting_ordinal
+            )
+            self.progress_bar.start()
+            final_state, step_objects = self.run(
+                initial_state=initial_state,
+                starting_ordinal=starting_ordinal,
+                **kwargs,
+            )
+            self.progress_bar.end()
+
+            # Stored until next start()
+            self.step_objects += step_objects
+
+            return final_state
+        finally:
+            for registered_handlers in handlers:
+                deregister_additional_handler(registered_handlers)
+            warnings = warning_stream.getvalue().rstrip()
+            if warnings:
+                warn("The following warnings were generated by the flow:")
+                warn(warnings)
 
     @protected
     @abstractmethod
     def run(
         self,
         initial_state: State,
         **kwargs,
@@ -585,24 +727,156 @@
         An asynchronous equivalent to :meth:`start_step`.
 
         :param step: The step object to run
         :param args: Arguments to `step.start`
         :param kwargs: Keyword arguments to `step.start`
         :returns: A ``Future`` encapsulating a State object, which can be used
             as an input to the next step (where the next step will wait for the
-            ``Future`` to be realized before calling :meth:`Step.run`).
-
-
+            ``Future`` to be realized before calling :meth:`Step.run`)
         """
 
         kwargs["toolbox"] = self.toolbox
         kwargs["step_dir"] = self.dir_for_step(step)
 
         return get_tpe().submit(step.start, *args, **kwargs)
 
+    def _save_snapshot_ef(self, path: Union[str, os.PathLike]):
+        if (
+            self.step_objects is None
+            or self.toolbox is None
+            or self.config_resolved_path is None
+        ):
+            raise RuntimeError(
+                "Flow was not run before attempting to save views in the Efabless format."
+            )
+
+        if len(self.step_objects) == 0:
+            # No steps, no data
+            return
+
+        last_step = self.step_objects[-1]
+        last_state = last_step.state_out
+
+        if last_state is None:
+            raise FlowException(
+                f"Misconfigured flow: Step {last_step.id} was appended to step objects without having been run first."
+            )
+
+        # 1. Copy Files
+        last_state.validate()
+        info(
+            f"Saving views in the Efabless/Caravel User Project format to '{os.path.abspath(path)}'…"
+        )
+        mkdirp(path)
+
+        supported_formats = {
+            DesignFormat.POWERED_NETLIST: (os.path.join("verilog", "gl"), "v"),
+            DesignFormat.DEF: ("def", "def"),
+            DesignFormat.LEF: ("lef", "lef"),
+            DesignFormat.SDF: (os.path.join("sdf", "multicorner"), "sdf"),
+            DesignFormat.SPEF: (os.path.join("spef", "multicorner"), "spef"),
+            DesignFormat.LIB: (os.path.join("lib", "multicorner"), "lib"),
+            DesignFormat.GDS: ("gds", "gds"),
+            DesignFormat.MAG: ("mag", "mag"),
+        }
+
+        def visitor(key, value, top_key, _, __):
+            df = DesignFormat.by_id(top_key)
+            assert df is not None
+            if df not in supported_formats:
+                return
+
+            dfo = df.value
+            assert isinstance(dfo, DesignFormatObject)
+
+            subdirectory, extension = supported_formats[df]
+
+            target_dir = os.path.join(path, subdirectory)
+            if not isinstance(value, Path):
+                if isinstance(value, dict):
+                    assert (
+                        self.toolbox is not None
+                    ), "toolbox check was not executed properly"
+                    default_corner_view = self.toolbox.filter_views(self.config, value)
+                    default_corner_target_dir = os.path.dirname(target_dir)
+                    mkdirp(default_corner_target_dir)
+                    if len(default_corner_view) == 1:
+                        target_basename = f"{self.config['DESIGN_NAME']}.{extension}"
+                        target_path = os.path.join(
+                            default_corner_target_dir, target_basename
+                        )
+                        shutil.copyfile(
+                            default_corner_view[0], target_path, follow_symlinks=True
+                        )
+                    else:
+                        for file in default_corner_view:
+                            shutil.copyfile(file, target_dir, follow_symlinks=True)
+                return
+
+            target_basename = os.path.basename(str(value))
+            target_basename = target_basename[: -len(dfo.extension)] + extension
+            target_path = os.path.join(target_dir, target_basename)
+            mkdirp(target_dir)
+            shutil.copyfile(value, target_path, follow_symlinks=True)
+
+        last_state._walk(last_state.to_raw_dict(metrics=False), path, visit=visitor)
+
+        # 2. Copy Logs, Reports, & Signoff Information
+        def copy_dir_contents(from_dir, to_dir, filter="*"):
+            for file in os.listdir(from_dir):
+                file_path = os.path.join(from_dir, file)
+                if os.path.isdir(file_path):
+                    continue
+                if fnmatch.fnmatch(file, filter):
+                    shutil.copyfile(
+                        file_path, os.path.join(to_dir, file), follow_symlinks=True
+                    )
+
+        signoff_folder = os.path.join(
+            path, "signoff", self.config["DESIGN_NAME"], "openlane"
+        )
+        mkdirp(signoff_folder)
+
+        # resolved.json
+        shutil.copyfile(
+            self.config_resolved_path,
+            os.path.join(signoff_folder, "resolved.json"),
+            follow_symlinks=True,
+        )
+
+        # Logs
+        mkdirp(signoff_folder)
+        copy_dir_contents(self.run_dir, signoff_folder, "*.log")
+
+        # Step-specific
+        for step in self.step_objects:
+            reports_dir = os.path.join(step.step_dir, "reports")
+            step_imp_id = step.get_implementation_id()
+            if step_imp_id.endswith("DRC") or step_imp_id.endswith("LVS"):
+                if os.path.exists(reports_dir):
+                    copy_dir_contents(reports_dir, signoff_folder)
+            if step_imp_id.endswith("LVS"):
+                copy_dir_contents(step.step_dir, signoff_folder, "*.log")
+            if step_imp_id.endswith("CheckAntennas"):
+                if os.path.exists(reports_dir):
+                    copy_dir_contents(
+                        reports_dir, signoff_folder, "antenna_summary.rpt"
+                    )
+            if step_imp_id.endswith("STAPostPNR"):
+                timing_report_folder = os.path.join(signoff_folder, "timing-reports")
+                mkdirp(timing_report_folder)
+                copy_dir_contents(step.step_dir, timing_report_folder, "*summary.rpt")
+                for dir in os.listdir(step.step_dir):
+                    dir_path = os.path.join(step.step_dir, dir)
+                    if not os.path.isdir(dir_path):
+                        continue
+                    target = os.path.join(timing_report_folder, dir)
+                    mkdirp(target)
+                    copy_dir_contents(dir_path, target, "*.rpt")
+
     @deprecated(
         version="2.0.0a46",
         reason="Use .progress_bar.set_max_stage_count",
         action="once",
     )
     @protected
     def set_max_stage_count(self, count: int):  # pragma: no cover
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlane-2.0.0b9/openlane/flows/misc.py` & `openlane-2.0.0rc2/openlane/flows/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/flows/optimizing.py` & `openlane-2.0.0rc2/openlane/flows/optimizing.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 from typing import List, Tuple
 from concurrent.futures import Future
 
 from .flow import Flow
 from ..state import State
 from ..config import Config
-from ..steps import Step, Yosys, OpenROAD, Misc, StepError
+from ..steps import Step, Yosys, OpenROAD, StepError
 from ..logging import get_log_level, set_log_level, LogLevels, success, info
 
 
 #   "Optimizing" is a custom demo flow to show what's possible with non-sequential Flows in OpenLane 2+.
 #   It works across two steps:
 #   * The Synthesis Exploration - tries multiple synthesis strategies in *parallel*.
 #       The best-performing strategy in terms of minimizing the area makes it to the next stage.
 #   * Floorplanning and Placement - tries FP and placement with a high utilization.
 #       If the high utilization fails, a lower is fallen back to as a suggestion.
 @Flow.factory.register()
 class Optimizing(Flow):
     Steps = [
         Yosys.Synthesis,
-        Misc.LoadBaseSDC,
+        OpenROAD.CheckSDCFiles,
         OpenROAD.STAPrePNR,
         OpenROAD.Floorplan,
         OpenROAD.IOPlacement,
         OpenROAD.GlobalPlacement,
     ]
 
     def run(
@@ -63,15 +63,15 @@
                 id=f"synthesis-{strategy}",
                 state_in=initial_state,
                 flow=self,
             )
             synth_future = self.start_step_async(synth_step)
             step_list.append(synth_step)
 
-            sdc_step = Misc.LoadBaseSDC(
+            sdc_step = OpenROAD.CheckSDCFiles(
                 config,
                 id=f"sdc-{strategy}",
                 state_in=synth_future,
                 flow=self,
             )
             sdc_future = self.start_step_async(sdc_step)
             step_list.append(sdc_step)
```

### Comparing `openlane-2.0.0b9/openlane/flows/sequential.py` & `openlane-2.0.0rc2/openlane/flows/sequential.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 # limitations under the License.
 from __future__ import annotations
 
 import os
 from typing import Iterable, List, Set, Tuple, Optional, Type, Dict, Union
 
 from .flow import Flow, FlowException, FlowError
+from ..common import Filter
 from ..state import State
+from ..logging import info, success, debug
 from ..steps import (
     Step,
     StepError,
     StepException,
     DeferredStepError,
 )
-from ..logging import info, success, err
 
 
 class SequentialFlow(Flow):
     """
     The simplest Flow, running each Step as a stage, serially,
     with nothing happening in parallel and no significant inter-step
     processing.
@@ -46,18 +47,49 @@
 
         You may also use the string Step IDs in place of a `Step` type object.
 
         Duplicate ID normalization is re-run after substitutions.
 
     :param args: Arguments for :class:`Flow`.
     :param kwargs: Keyword arguments for :class:`Flow`.
+
+    :cvar gating_config_vars: A mapping from step ID (wildcards) to lists of
+        Boolean variable names. All Boolean variables must be True for a step with
+        a specific ID to execute.
     """
 
-    def __init_subclass__(cls, scm_type=None, name=None, **kwargs):
-        cls.__normalize_step_ids(cls)
+    gating_config_vars: Dict[str, List[str]] = {}
+
+    def __init_subclass__(Self, scm_type=None, name=None, **kwargs):
+        Self.__normalize_step_ids(Self)
+
+        # Validate Gating Config Vars
+        variables_by_name = {}
+        for variable in Self.config_vars:
+            variables_by_name[variable.name] = variable
+
+        step_id_set = set()
+        for step in Self.Steps:
+            step_id_set.add(step.id)
+
+        for id, variable_names in Self.gating_config_vars.items():
+            matching_steps = list(Filter([id]).filter(step_id_set))
+            if id not in step_id_set and len(matching_steps) < 1:
+                raise TypeError(
+                    f"Gated Step '{id}' does not match any Step in Flow '{Self.__qualname__}'"
+                )
+            for var_name in variable_names:
+                if var_name not in variables_by_name:
+                    raise TypeError(
+                        f"Gating variable '{var_name}' for Step '{id}' does not match any declared config_vars in Flow '{Self.__qualname__}'"
+                    )
+                if variables_by_name[var_name].type != bool:
+                    raise TypeError(
+                        f"Gating variable '{var_name}' in Flow '{Self.__qualname__}' is not a Boolean"
+                    )
 
     @classmethod
     def make(Self, step_ids: List[str]) -> Type[SequentialFlow]:
         Step_list = []
         for name in step_ids:
             step = Step.factory.get(name)
             if step is None:
@@ -73,30 +105,29 @@
     @staticmethod
     def __normalize_step_ids(target: Union[SequentialFlow, Type[SequentialFlow]]):
         ids_used: Set[str] = set()
 
         for i, step in enumerate(target.Steps):
             counter = 0
             id = step.id
-            name = step.__name__
+            if (
+                id == NotImplemented
+            ):  # Will be validated later by initialization: ignore for now
+                continue
             while id in ids_used:
                 counter += 1
                 id = f"{step.id}-{counter}"
-                name = f"{step.__name__}_{counter}"
             if id != step.id:
-                new_step = type(name, (step,), {"id": id})
-                target.Steps[i] = new_step
+                target.Steps[i] = step.with_id(id)
             ids_used.add(id)
 
     def __init__(
         self,
         *args,
-        Substitute: Optional[
-            Dict[str, Union[str, Type[Step]]],
-        ] = None,
+        Substitute: Optional[Dict[str, Union[str, Type[Step]]]] = None,
         **kwargs,
     ):
         self.Steps = self.Steps.copy()  # Break global reference
 
         if substitute := Substitute:
             for key, item in substitute.items():
                 self.__substitute_step(key, item)
@@ -108,15 +139,19 @@
     def __substitute_step(
         self,
         id: str,
         with_step: Union[str, Type[Step]],
     ):
         step_indices: List[int] = []
         for i, step in enumerate(self.Steps):
-            if step.id.lower() == id.lower():
+            if (
+                step.id
+                != NotImplemented  # Will be validated later by initialization: ignore for now
+                and step.id.lower() == id.lower()
+            ):
                 step_indices.append(i)
 
         if len(step_indices) == 0:
             raise FlowException(
                 f"Could not substitute '{id}' with '{with_step}': no steps with ID '{id}' found in flow."
             )
 
@@ -136,14 +171,15 @@
         initial_state: State,
         frm: Optional[str] = None,
         to: Optional[str] = None,
         skip: Optional[Iterable[str]] = None,
         reproducible: Optional[str] = None,
         **kwargs,
     ) -> Tuple[State, List[Step]]:
+        debug(f"Starting run ▶ '{self.run_dir}'")
         step_ids = {cls.id.lower(): cls.id for cls in reversed(self.Steps)}
         skipped_ids = []
 
         frm_resolved = None
         if frm is not None:
             if id := step_ids.get(frm.lower()):
                 frm_resolved = id
@@ -184,23 +220,40 @@
         step_list = []
 
         info("Starting…")
 
         executing = frm is None
         deferred_errors = []
 
+        gating_cvars_expanded: Dict[str, List[str]] = {}
+        for key, value in self.gating_config_vars.items():
+            if key in step_ids.values():
+                gating_cvars_expanded[key] = value
+                continue
+            for id in Filter([key]).filter(step_ids.values()):
+                gating_cvars_expanded[id] = value
+
         current_state = initial_state
         for cls in self.Steps:
             step = cls(config=self.config, state_in=current_state)
             if frm_resolved is not None and frm_resolved == step.id:
                 executing = True
 
+            gated = False
+            if gating_cvars := gating_cvars_expanded.get(step.id):
+                for variable in gating_cvars:
+                    if not self.config[variable]:
+                        info(
+                            f"Gating variable for step '{step.id}' set to 'False'- the step will be skipped."
+                        )
+                        gated = True
+
             self.progress_bar.start_stage(step.name)
             increment_ordinal = True
-            if not executing or cls.id in skipped_ids:
+            if not executing or cls.id in skipped_ids or gated:
                 info(f"Skipping step '{step.name}'…")
                 increment_ordinal = False
             elif cls.id == reproducible_resolved:
                 step.create_reproducible(
                     os.path.join(
                         self.dir_for_step(step),
                         "reproducible",
@@ -211,32 +264,32 @@
                 step_list.append(step)
                 try:
                     current_state = step.start(
                         toolbox=self.toolbox,
                         step_dir=self.dir_for_step(step),
                     )
                 except StepException as e:
-                    raise FlowException(str(e))
+                    raise FlowException(str(e)) from None
                 except DeferredStepError as e:
                     deferred_errors.append(str(e))
                 except StepError as e:
-                    raise FlowError(str(e))
+                    raise FlowError(str(e)) from None
 
             self.progress_bar.end_stage(increment_ordinal=increment_ordinal)
 
             if to_resolved and to_resolved == step.id:
                 executing = False
         if len(deferred_errors) != 0:
-            err("The following deferred step errors have been encountered:")
-            for error in deferred_errors:
-                err(error)
-            raise FlowError("One or more deferred errors were encountered.")
+            raise FlowError(
+                "One or more deferred errors were encountered:\n"
+                + "\n".join(deferred_errors)
+            )
 
         assert self.run_dir is not None
+        debug(f"Run concluded ▶ '{self.run_dir}'")
         final_views_path = os.path.join(self.run_dir, "final")
-        info(f"Saving final views to '{final_views_path}'…")
         try:
             current_state.save_snapshot(final_views_path)
         except Exception as e:
             raise FlowException(f"Failed to save final views: {e}")
         success("Flow complete.")
         return (current_state, step_list)
```

### Comparing `openlane-2.0.0b9/openlane/logging/__init__.py` & `openlane-2.0.0rc2/openlane/logging/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 
 As the name implies, this handles OpenLane's logging using the ``logging``
 module and the ``rich`` library.
 """
 
 from .logger import (
     LogLevels,
-    LogLevelsDict,
+    LevelFilter,
+    options,
     console,
     set_log_level,
     reset_log_level,
     get_log_level,
     register_additional_handler,
     deregister_additional_handler,
     verbose,
     debug,
     info,
     rule,
     success,
     warn,
     err,
+    subprocess,
 )
```

### Comparing `openlane-2.0.0b9/openlane/logging/logger.py` & `openlane-2.0.0rc2/openlane/logging/logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,207 +7,317 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import sys
 import click
 import atexit
 import logging
+from enum import IntEnum
+from typing import ClassVar, Iterable, Union
+
 import rich.console
-from typing import ClassVar, Union
-from rich.logging import RichHandler
+import rich.logging
+from rich.text import Text
+from rich.style import Style, StyleType
 
 
-class LogLevels:
-    ALL: ClassVar[int] = 0
-    DEBUG: ClassVar[int] = 10
-    VERBOSE: ClassVar[int] = 15
-    INFO: ClassVar[int] = 20
-    WARN: ClassVar[int] = 30
-    ERROR: ClassVar[int] = 40
-    CRITICAL: ClassVar[int] = 50
+class LogLevels(IntEnum):
+    ALL = 0
+    DEBUG = 10
+    SUBPROCESS = 12
+    VERBOSE = 15
+    INFO = 20
+    WARNING = 30
+    ERROR = 40
+    CRITICAL = 50
 
 
-def __log_levels_dict():
-    result = {k: v for k, v in LogLevels.__dict__.items() if not k.startswith("__")}
-    for name, value in result.items():
-        logging.addLevelName(value, name)
-    return result
+console = rich.console.Console()
+atexit.register(lambda: rich.console.Console().show_cursor())
+__event_logger: logging.Logger = logging.getLogger("__openlane__")
 
 
-LogLevelsDict = __log_levels_dict()
+class options:
+    _condensed_mode: ClassVar[bool] = False
+    _show_progress_bar: ClassVar[bool] = True
 
-console = rich.console.Console()
-atexit.register(lambda: rich.console.Console().show_cursor())
-__plain_output = "pytest" in sys.modules
+    @classmethod
+    def get_condensed_mode(Self) -> bool:
+        return Self._condensed_mode
+
+    @classmethod
+    def set_condensed_mode(Self, condensed: bool):
+        Self._condensed_mode = condensed
+
+    @classmethod
+    def get_show_progress_bar(Self) -> bool:
+        return Self._show_progress_bar
+
+    @classmethod
+    def set_show_progress_bar(Self, show: bool):
+        Self._show_progress_bar = show
 
 
 class NullFormatter(logging.Formatter):
     def format(self, record):
         return record.getMessage()
 
 
-def __logger():
-    handler: logging.Handler
-    if __plain_output:
-        handler = logging.StreamHandler()
-        handler.setFormatter(NullFormatter())
-    else:
-        handler = RichHandler(
-            console=console,
-            rich_tracebacks=True,
-            markup=True,
-            tracebacks_suppress=[
-                click,
-            ],
-            show_level=False,
+class LevelFormatter(logging.Formatter):
+    def format(self, record):
+        message = record.getMessage()
+        if record.levelname == "WARNING":
+            message = f"[yellow]{message}"
+        elif record.levelname == "ERROR":
+            message = f"[red]{message}"
+        elif record.levelname == "CRITICAL":
+            message = f"[red][bold]{message}"
+        else:
+            message = f"{message}"
+        return message
+
+
+class RichHandler(rich.logging.RichHandler):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(**kwargs)
+
+    def get_level_text(self, record: logging.LogRecord) -> Text:
+        if not options.get_condensed_mode():
+            return super().get_level_text(record)
+        level_name = record.levelname
+        style: StyleType
+        if level_name == "WARNING":
+            style = Style(color="yellow", bold=True)
+        else:
+            style = f"logging.level.{level_name.lower()}"
+        level_text = Text.styled(
+            f"[{level_name[0]}]",
+            style,
         )
-        handler.setFormatter(logging.Formatter("%(message)s", datefmt="[%X]"))
+        return level_text
+
+
+class KeywordFilter(logging.Filter):
+    def __init__(self, matching_values: dict) -> None:
+        super().__init__()
+        self.matching_values = matching_values.copy()
+
+    def filter(self, record: logging.LogRecord) -> bool:
+        for key, value in self.matching_values.items():
+            if value is None:
+                if hasattr(record, key) and getattr(record, key) is not None:
+                    return False
+            else:
+                if not hasattr(record, key) or getattr(record, key) != value:
+                    return False
+        return True
+
+
+class LevelFilter(logging.Filter):
+    def __init__(self, levels: Iterable[str], invert: bool = False) -> None:
+        self.levels = levels
+        self.invert = invert
+
+    def filter(self, record: logging.LogRecord) -> bool:
+        if options.get_condensed_mode():
+            if record.levelname == "SUBPROCESS":
+                return False
+        if self.invert:
+            return record.levelname not in self.levels
+        else:
+            return record.levelname in self.levels
+
+
+def initialize_logger():
+    global __event_logger, console
+
+    for level in LogLevels:
+        logging.addLevelName(level.value, level.name)
+
+    subprocess_handler = RichHandler(
+        console=console,
+        show_time=False,
+        omit_repeated_times=False,
+        show_level=False,
+        show_path=False,
+        enable_link_path=False,
+        tracebacks_word_wrap=False,
+        keywords=[],
+        markup=False,
+    )
+    subprocess_handler.addFilter(LevelFilter(["SUBPROCESS"]))
+
+    rich_handler = RichHandler(
+        console=console,
+        rich_tracebacks=True,
+        omit_repeated_times=False,
+        markup=True,
+        tracebacks_suppress=[
+            click,
+        ],
+        show_level=True,
+        keywords=[],
+    )
+    rich_handler.setFormatter(LevelFormatter("%(message)s", datefmt="[%X]"))
+    rich_handler.addFilter(LevelFilter(["SUBPROCESS"], invert=True))
+
     logger = logging.getLogger("__openlane__")
-    logger.setLevel(LogLevels.VERBOSE)
-    logger.addHandler(handler)
-    return logger
+    logger.setLevel(LogLevels.SUBPROCESS)
+
+    logger.handlers.clear()
+
+    logger.addHandler(subprocess_handler)
+    logger.addHandler(rich_handler)
 
 
-__openlane_logger = __logger()
+initialize_logger()
 
 
 def register_additional_handler(handler: logging.Handler):
     """
     Adds a new handler to the default OpenLane logger.
 
     :param handler: The new handler. Must be of type ``logging.Handler``
         or its subclasses.
     """
-    __openlane_logger.addHandler(handler)
+    __event_logger.addHandler(handler)
 
 
 def deregister_additional_handler(handler: logging.Handler):
     """
     Removes a registered handler from the default OpenLane logger.
 
     :param handler: The handler. If not registered, the behavior
         of this function is undefined.
     """
-    __openlane_logger.removeHandler(handler)
+    __event_logger.removeHandler(handler)
 
 
 def set_log_level(lv: Union[str, int]):
     """
     Sets the log level of the default OpenLane logger.
 
     :param lv: Either the name or number of the desired log level.
     """
-    __openlane_logger.setLevel(lv)
+    __event_logger.setLevel(lv)
 
 
 def reset_log_level():
     """
     Sets the log level of the default OpenLane logger back to the
     default log level.
     """
-    set_log_level("VERBOSE")
+    set_log_level("SUBPROCESS")
 
 
 def get_log_level() -> int:
     """
     Obtains the numeric log level of the OpenLane logger.
     """
-    return __openlane_logger.getEffectiveLevel()
+    return __event_logger.getEffectiveLevel()
 
 
-def debug(msg: object, /, **kwargs):
+def debug(*args, **kwargs):
     """
     Logs to the OpenLane logger with the log level DEBUG.
 
     :param msg: The message to log
     """
     if kwargs.get("stacklevel") is None:
         kwargs["stacklevel"] = 2
-    __openlane_logger.debug(msg, **kwargs)
+    __event_logger.debug(*args, **kwargs)
 
 
 def verbose(*args, **kwargs):
     """
-    Prints to the console if the log level is <= VERBOSE.
-
-    All args and kwargs are passed to https://rich.readthedocs.io/en/stable/reference/console.html#rich.console.Console.print
+    Logs to the OpenLane logger with the log level VERBOSE.
     """
-    if get_log_level() > LogLevels.VERBOSE:
-        return
-    if __plain_output:
-        print(*args, **kwargs)
-    else:
-        console.print(*args, **kwargs)
+    if kwargs.get("stacklevel") is None:
+        kwargs["stacklevel"] = 2
+    __event_logger.log(
+        LogLevels.VERBOSE,
+        *args,
+        **kwargs,
+    )
 
 
 def info(msg: object, /, **kwargs):
     """
     Logs to the OpenLane logger with the log level INFO.
 
     :param msg: The message to log
     """
     if kwargs.get("stacklevel") is None:
         kwargs["stacklevel"] = 2
-    __openlane_logger.info(msg, **kwargs)
+    __event_logger.info(msg, **kwargs)
+
+
+def subprocess(msg: object, /, **kwargs):
+    """
+    Logs to the OpenLane logger with the log level SUBPROCESS.
+
+    :param msg: The message to log
+    """
+    if kwargs.get("stacklevel") is None:
+        kwargs["stacklevel"] = 2
+    __event_logger.log(LogLevels.SUBPROCESS, msg, **kwargs)
 
 
 def rule(title: str = "", /, **kwargs):  # pragma: no cover
     """
     Prints a horizontal line on the terminal enclosing the first argument
     if the log level is <= INFO.
 
     Kwargs are passed to https://rich.readthedocs.io/en/stable/reference/console.html#rich.console.Console.rule
 
     :param title: A title string to enclose in the console rule
     """
-    if __plain_output:
-        print(("-" * 10) + str(title) + ("-" * 10))
-    else:
-        console.rule(title, **kwargs)
+    console.rule(title)
 
 
 def success(msg: object, /, **kwargs):
     """
-    Logs an item to the OpenLane logger with a success unicode character and
-    green/bold rich formatting syntax with the log level INFO.
+    Logs to the OpenLane logger with the log level INFO.
 
     :param msg: The message to log
     """
     if kwargs.get("stacklevel") is None:
         kwargs["stacklevel"] = 2
-    __openlane_logger.info(f"⭕ [green][bold] {msg}", **kwargs)
+    __event_logger.info(f"{msg}", **kwargs)
 
 
 def warn(msg: object, /, **kwargs):
     """
-    Logs an item to the OpenLane logger with a warning unicode character and
-    gold/bold rich formatting syntax with the log level WARN.
+    Logs to the OpenLane logger with the log level WARNING.
 
     :param msg: The message to log
     """
     if kwargs.get("stacklevel") is None:
         kwargs["stacklevel"] = 2
-    __openlane_logger.warning(f"⚠️  [gold][bold] {msg}", **kwargs)
+    __event_logger.warning(f"{msg}", **kwargs)
 
 
 def err(msg: object, /, **kwargs):
     """
-    Logs an item to the OpenLane logger terminal with an error unicode character and
-    red/bold rich formatting syntax with the log level ERROR.
+    Logs to the OpenLane logger with the log level ERROR.
+
+    :param msg: The message to log
     """
     if kwargs.get("stacklevel") is None:
         kwargs["stacklevel"] = 2
-    __openlane_logger.error(f"❌ [red][bold] {msg}", **kwargs)
+    __event_logger.error(f"{msg}", **kwargs)
 
 
 if __name__ == "__main__":
+    initialize_logger()
     debug("Debug")
     verbose("Verbose")
-    rule()
+    subprocess("Subprocess")
+    rule("Rule")
     info("Info")
     success("Success")
     warn("Warn")
     err("Err")
+    print("\n")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openlane-2.0.0b9/openlane/plugins.py` & `openlane-2.0.0rc2/openlane/plugins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/base.sdc` & `openlane-2.0.0rc2/openlane/scripts/base.sdc`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 set clock_port __VIRTUAL_CLK__
 if { [info exists ::env(CLOCK_PORT)] } {
     set port_count [llength $::env(CLOCK_PORT)]
 
     if { $port_count == "0" } {
-        puts "\[WARN] No CLOCK_PORT found. A dummy clock will be used."
+        puts "\[WARNING] No CLOCK_PORT found. A dummy clock will be used."
     } elseif { $port_count != "1" } {
-        puts "\[WARN] Multi-clock files are not currently supported by the base SDC file. Only the first clock will be constrained."
+        puts "\[WARNING] Multi-clock files are not currently supported by the base SDC file. Only the first clock will be constrained."
     }
 
     if { $port_count > "0" } {
         set ::clock_port [lindex $::env(CLOCK_PORT) 0]
     }
 }
 set port_args [get_ports $clock_port]
@@ -21,14 +21,17 @@
 puts "\[INFO] Setting output delay to: $output_delay_value"
 puts "\[INFO] Setting input delay to: $input_delay_value"
 
 set_max_fanout $::env(MAX_FANOUT_CONSTRAINT) [current_design]
 if { [info exists ::env(MAX_TRANSITION_CONSTRAINT)] } {
     set_max_transition $::env(MAX_TRANSITION_CONSTRAINT) [current_design]
 }
+if { [info exists ::env(MAX_CAPACITANCE_CONSTRAINT)] } {
+    set_max_capacitance $::env(MAX_CAPACITANCE_CONSTRAINT) [current_design]
+} 
 
 set clk_input [get_port $clock_port]
 set clk_indx [lsearch [all_inputs] $clk_input]
 set all_inputs_wo_clk [lreplace [all_inputs] $clk_indx $clk_indx ""]
 
 #set rst_input [get_port resetn]
 #set rst_indx [lsearch [all_inputs] $rst_input]
```

### Comparing `openlane-2.0.0b9/openlane/scripts/klayout/render.py` & `openlane-2.0.0rc2/openlane/scripts/klayout/render.py`

 * *Files 21% similar despite different names*

```diff
@@ -40,112 +40,82 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+from typing import Tuple
 
+import pya
+import click
 
-import os
-import sys
-from typing import TYPE_CHECKING
-
-if "klayout" in os.path.basename(sys.executable):
-    import pya
-else:
-    import click
-
-    @click.command()
-    @click.option("-o", "--output", required=True)
-    @click.option(
-        "-l",
-        "--input-lef",
-        "input_lefs",
-        multiple=True,
-    )
-    @click.option(
-        "-T",
-        "--lyt",
-        required=True,
-        help="KLayout .lyt file",
-    )
-    @click.option(
-        "-P",
-        "--lyp",
-        required=True,
-        help="KLayout .lyp file",
-    )
-    @click.option(
-        "-M",
-        "--lym",
-        required=True,
-        help="KLayout .map (LEF/DEF layer map) file",
-    )
-    @click.argument("input")
-    def cli(**kwargs):
-        args = [
-            "klayout",
-            "-b",
-            "-rm",
-            __file__,
-        ]
-        for key, value in kwargs.items():
-            args.append("-rd")
-            if isinstance(value, tuple) or isinstance(value, list):
-                value = ";".join([os.path.abspath(element) for element in value])
-            elif (
-                isinstance(value, str)
-                and os.path.exists(value)
-                and key != "design_name"
-            ):
-                value = os.path.abspath(value)
-
-            args.append(f"{key}={value or 'NULL'}")
-
-        os.execlp("klayout", *args)
-
-    if __name__ == "__main__":
-        cli()
-
-
-if TYPE_CHECKING:
-    # Dummy data for type-checking
-    input: str = ""
-    output: str = ""
-    input_lefs: str = ""
-    lyp: str = ""
-    lyt: str = ""
-    lym: str = ""
-
-try:
-    gds = input.endswith(".gds")
-
-    # Load technology file
-    tech = pya.Technology()
-    tech.load(lyt)
-
-    layout_options = None
-    if not gds:
-        layout_options = tech.load_layout_options
-        layout_options.lefdef_config.map_file = lym
-        layout_options.lefdef_config.macro_resolution_mode = 1
-        layout_options.lefdef_config.read_lef_with_def = False
-        layout_options.lefdef_config.lef_files = input_lefs.split(";")
-
-    view = pya.LayoutView()
-    view.load_layer_props(lyp)
-
-    if gds:
-        view.load_layout(input)
-    else:
-        view.load_layout(input, layout_options, lyt)
-    view.max_hier()
-    pixels = view.get_pixels_with_options(1000, 1000)
-
-    with open(output, "wb") as f:
-        f.write(pixels.to_png_data())
-
-    pya.Application.instance().exit(0)
-except Exception as e:
-    print(e)
-    pya.Application.instance().exit(1)
+
+@click.command()
+@click.option("-o", "--output", required=True)
+@click.option(
+    "-l",
+    "--input-lef",
+    "input_lefs",
+    multiple=True,
+)
+@click.option(
+    "-T",
+    "--lyt",
+    required=True,
+    help="KLayout .lyt file",
+)
+@click.option(
+    "-P",
+    "--lyp",
+    required=True,
+    help="KLayout .lyp file",
+)
+@click.option(
+    "-M",
+    "--lym",
+    required=True,
+    help="KLayout .map (LEF/DEF layer map) file",
+)
+@click.argument("input")
+def render(
+    input_lefs: Tuple[str, ...],
+    output: str,
+    lyt: str,
+    lyp: str,
+    lym: str,
+    input: str,
+):
+    try:
+        gds = input.endswith(".gds")
+
+        # Load technology file
+        tech = pya.Technology()
+        tech.load(lyt)
+
+        layout_options = None
+        if not gds:
+            layout_options = tech.load_layout_options
+            layout_options.lefdef_config.map_file = lym
+            layout_options.lefdef_config.macro_resolution_mode = 1
+            layout_options.lefdef_config.read_lef_with_def = False
+            layout_options.lefdef_config.lef_files = list(input_lefs)
+
+        view = pya.LayoutView()
+        view.load_layer_props(lyp)
+
+        if gds:
+            view.load_layout(input)
+        else:
+            view.load_layout(input, layout_options, lyt)
+        view.max_hier()
+        pixels = view.get_pixels_with_options(1000, 1000)
+
+        with open(output, "wb") as f:
+            f.write(pixels.to_png_data())
+    except Exception as e:
+        print(e)
+        exit(1)
+
+
+if __name__ == "__main__":
+    render()
```

### Comparing `openlane-2.0.0b9/openlane/scripts/klayout/stream_out.py` & `openlane-2.0.0rc2/openlane/scripts/klayout/stream_out.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,166 +40,137 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+import sys
+from typing import Tuple, Optional
 
+import pya
+import click
+
+
+@click.command()
+@click.option("-o", "--output", required=True)
+@click.option(
+    "-l",
+    "--input-lef",
+    "input_lefs",
+    multiple=True,
+)
+@click.option(
+    "-T",
+    "--lyt",
+    required=True,
+    help="KLayout .lyt file",
+)
+@click.option(
+    "-P",
+    "--lyp",
+    required=True,
+    help="KLayout .lyp file",
+)
+@click.option(
+    "-M",
+    "--lym",
+    required=True,
+    help="KLayout .map (LEF/DEF layer map) file",
+)
+@click.option("-w", "--with-gds-file", "input_gds_files", multiple=True, default=[])
+@click.option("-s", "--seal-gds-file", "seal_gds", default=None)
+@click.option(
+    "-t",
+    "--top",
+    "design_name",
+    required=True,
+    help="Name of the design/top module",
+)
+@click.argument(
+    "input",
+    type=click.Path(exists=True, file_okay=True, dir_okay=False),
+)
+def stream_out(
+    output: str,
+    input_lefs: Tuple[str, ...],
+    lyt: str,
+    lyp: str,
+    lym: str,
+    input_gds_files: Tuple[str, ...],
+    seal_gds: Optional[str],
+    design_name: str,
+    input: str,
+):  # Load technology file
+    try:
+        tech = pya.Technology()
+        tech.load(lyt)
+        layout_options = tech.load_layout_options
+        layout_options.lefdef_config.read_lef_with_def = False
+        layout_options.lefdef_config.lef_files = list(input_lefs)
+        layout_options.lefdef_config.map_file = lym
+
+        # Load def file
+        main_layout = pya.Layout()
+        # main_layout.load_layer_props(props_file)
+        main_layout.read(input, layout_options)
+
+        # Clear cells
+        top_cell_index = main_layout.cell(design_name).cell_index()
+
+        print("[INFO] Clearing cells…")
+        for i in main_layout.each_cell():
+            if i.cell_index() != top_cell_index:
+                if not i.name.startswith("VIA"):
+                    i.clear()
+
+        # Load in the gds to merge
+        print("[INFO] Merging GDS files…")
+        for gds in input_gds_files:
+            main_layout.read(gds)
+
+        # Copy the top level only to a new layout
+        print(f"[INFO] Copying top level cell '{design_name}'…")
+        top_only_layout = pya.Layout()
+        top_only_layout.dbu = main_layout.dbu
+        top = top_only_layout.create_cell(design_name)
+        top.copy_tree(main_layout.cell(design_name))
+
+        print("[INFO] Checking for missing GDS…")
+        missing_gds = False
+        for i in top_only_layout.each_cell():
+            if i.is_empty():
+                missing_gds = True
+                print(
+                    f"[ERROR] LEF Cell '{i.name}' has no matching GDS cell.",
+                    file=sys.stderr,
+                )
+
+        if missing_gds:
+            raise Exception("One or more cell GDS files are missing.")
+        else:
+            print("[INFO] All LEF cells have matching GDS cells.")
+
+        if seal_gds is not None:
+            top_cell = top_only_layout.top_cell()
+
+            print(f"[INFO] Reading seal GDS file '{seal_gds}'…")
+            top_only_layout.read(seal_gds)
+
+            for cell in top_only_layout.top_cells():
+                if cell != top_cell:
+                    print(
+                        f"[INFO] Merging '{cell.name}' as child of '{top_cell.name}'…"
+                    )
+                    top.insert(pya.CellInstArray(cell.cell_index(), pya.Trans()))
+
+        # Write out the GDS
+        print(f"[INFO] Writing out GDS '{output}'…")
+        top_only_layout.write(output)
+        print("[INFO] Done.")
+    except Exception as e:
+        print(e)
+        exit(1)
 
-import os
-import sys
-from typing import TYPE_CHECKING, Optional
 
-if "klayout" in os.path.basename(sys.executable):
-    import pya
-else:
-    import click
-
-    @click.command()
-    @click.option("-o", "--output", required=True)
-    @click.option(
-        "-l",
-        "--input-lef",
-        "input_lefs",
-        multiple=True,
-    )
-    @click.option(
-        "-T",
-        "--lyt",
-        required=True,
-        help="KLayout .lyt file",
-    )
-    @click.option(
-        "-P",
-        "--lyp",
-        required=True,
-        help="KLayout .lyp file",
-    )
-    @click.option(
-        "-M",
-        "--lym",
-        required=True,
-        help="KLayout .map (LEF/DEF layer map) file",
-    )
-    @click.option("-w", "--with-gds-file", "input_gds_files", multiple=True, default=[])
-    @click.option("-s", "--seal-gds-file", "seal_gds", default=None)
-    @click.option(
-        "-t",
-        "--top",
-        "design_name",
-        required=True,
-        help="Name of the design/top module",
-    )
-    @click.argument(
-        "input",
-        type=click.Path(exists=True, file_okay=True, dir_okay=False),
-    )
-    def stream_out(**kwargs):
-        args = [
-            "klayout",
-            "-b",
-            "-rm",
-            __file__,
-        ]
-        for key, value in kwargs.items():
-            args.append("-rd")
-            if isinstance(value, tuple) or isinstance(value, list):
-                value = ";".join([os.path.abspath(element) for element in value])
-            elif (
-                isinstance(value, str)
-                and os.path.exists(value)
-                and key != "design_name"
-            ):
-                value = os.path.abspath(value)
-
-            args.append(f"{key}={value or 'NULL'}")
-
-        os.execlp("klayout", *args)
-
-    if __name__ == "__main__":
-        stream_out()
-
-
-if TYPE_CHECKING:
-    # Dummy data for type-checking
-    input: str = ""
-    output: str = ""
-    input_lefs: str = ""
-    lyp: str = ""
-    lyt: str = ""
-    lym: str = ""
-    design_name: str = ""
-    input_gds_files: str = ""
-    seal_gds: Optional[str] = ""
-
-if seal_gds == "NULL":
-    seal_gds = None
-
-
-try:
-    # Load technology file
-    tech = pya.Technology()
-    tech.load(lyt)
-    layout_options = tech.load_layout_options
-    layout_options.lefdef_config.read_lef_with_def = False
-    layout_options.lefdef_config.lef_files = input_lefs.split(";")
-    layout_options.lefdef_config.map_file = lym
-
-    # Load def file
-    main_layout = pya.Layout()
-    # main_layout.load_layer_props(props_file)
-    main_layout.read(input, layout_options)
-
-    # Clear cells
-    top_cell_index = main_layout.cell(design_name).cell_index()
-
-    print("[INFO] Clearing cells…")
-    for i in main_layout.each_cell():
-        if i.cell_index() != top_cell_index:
-            if not i.name.startswith("VIA"):
-                i.clear()
-
-    # Load in the gds to merge
-    print("[INFO] Merging GDS files…")
-    for gds in input_gds_files.split(";"):
-        print(f"\t{gds}")
-        main_layout.read(gds)
-
-    # Copy the top level only to a new layout
-    print(f"[INFO] Copying top level cell '{design_name}'…")
-    top_only_layout = pya.Layout()
-    top_only_layout.dbu = main_layout.dbu
-    top = top_only_layout.create_cell(design_name)
-    top.copy_tree(main_layout.cell(design_name))
-
-    print("[INFO] Checking for missing GDS…")
-    missing_gds = False
-    for i in top_only_layout.each_cell():
-        if i.is_empty():
-            missing_gds = True
-            print(f"[ERROR] LEF Cell '{i.name}' has no matching GDS cell.")
-
-    if missing_gds:
-        raise Exception("One or more cell GDS files are missing.")
-    else:
-        print("[INFO] All LEF cells have matching GDS cells.")
-
-    if seal_gds is not None:
-        top_cell = top_only_layout.top_cell()
-
-        print(f"[INFO] Reading seal GDS file '{seal_gds}'…")
-        top_only_layout.read(seal_gds)
-
-        for cell in top_only_layout.top_cells():
-            if cell != top_cell:
-                print(f"[INFO] Merging '{cell.name}' as child of '{top_cell.name}'…")
-                top.insert(pya.CellInstArray(cell.cell_index(), pya.Trans()))
-
-    # Write out the GDS
-    print(f"[INFO] Writing out GDS '{output}'…")
-    top_only_layout.write(output)
-    print("[INFO] Done.")
-    pya.Application.instance().exit(0)
-except Exception as e:
-    print(e)
-    pya.Application.instance().exit(1)
+if __name__ == "__main__":
+    stream_out()
```

### Comparing `openlane-2.0.0b9/openlane/scripts/klayout/xor.drc` & `openlane-2.0.0rc2/openlane/scripts/klayout/xor.drc`

 * *Files 21% similar despite different names*

```diff
@@ -16,91 +16,105 @@
 
     opts.on("-o", "--output OUTPUT", "Klayout RDB (.xml) output file (required)") do |rdb_out|
       options[:rdb_out] = rdb_out
     end
     opts.on("-i", "--ignore SEMICOLON_DELIMITED_LIST", "Ignore layer(s)") do |ignore|
       options[:ignore] = ignore
     end
-    # opts.on("-O", "--gds-out OUTPUT", "GDS output file (required)") do |gds_out|
-    #   options[:gds_out] = gds_out
-    # end
     opts.on("-t", "--top TOP_CELL", "Top cell name (required)") do |top_cell|
       options[:top_cell] = top_cell
     end
+    opts.on("-t", "--tile-size TILE_SIZE", "Tile size (in µm)") do |tile_size|
+      options[:tile_size] = tile_size.to_i
+    end
+    opts.on("-n", "--threads THREAD_COUNT", "Lower bound on the thread count used by this process (+ managing threads)") do |threads|
+      options[:threads] = threads.to_i
+    end
   end
   optparse.parse!
 
   if [options[:rdb_out], options[:top_cell]].include?(nil)
     puts optparse.help
     exit 64
   end
 
   args = [
     "klayout", "-b",
     "-r", $0,
     "-rd", "top_cell=#{options[:top_cell]}",
     "-rd", "a=#{ARGV[0]}",
     "-rd", "b=#{ARGV[1]}",
-    "-rd", "jobs=1",
+    "-rd", "jobs=#{options[:threads]}",
     "-rd", "rdb_out=#{File.absolute_path(options[:rdb_out])}",
     "-rd", "ignore=#{options[:ignore]}",
-    # "-rd", "gds_out=#{options[:gds_out]}",
+    "-rd", "tilesize=#{options[:tile_size]}",
   ]
   puts "Running: '#{args.join(" ")}'…"
   exec *args
 
 end
 
 verbose
 
+# Run XOR
+if $jobs == ""
+  $jobs = "1"
+end
+$jobs = $jobs.to_i
+
+info "Using #{$jobs} threads…"
+threads($jobs)
+
+# Tiling
+if $tilesize == ""
+  $tilesize = "500"
+end
+$tilesize = $tilesize.to_i
+
+info "Using a tile size of (#{$tilesize} µm)²…"
+tiles($tilesize.um, $tilesize.um)
+
 # Set up inputs
 puts $a, $b
 a = source($a, $top_cell)
 b = source($b, $top_cell)
 
 # Set up output
 # target($gds_out, "XOR")
 report("XOR #{$a} vs. #{$b}", $rdb_out)
 
 def write_data(xor_data, layer_info)
-  # xor_data.output(layer_info.layer, layer_info.datatype, layer_info.name)
   xor_data.output(layer_info.to_s, "XOR data for layer #{layer_info.to_s}")
 end
 
-# Run XOR
-$jobs = $jobs.to_i
-threads($jobs) unless $jobs <= 1
-
 ## Collect all common layers
 layers = {}
 [ a.layout, b.layout ].each do |ly|
   ly.layer_indices.each do |li|
     i = ly.get_info(li)
     layers[i.to_s] = i
   end
 end
 
 ignore_list = $ignore.split(";")
 
 ## Perform per-layer XOR
 total_xor_differences = 0
-layers.keys.sort.each do |layer_name|
+layers.sort.uniq.each do |layer_name, layer_data|
   if ignore_list.include? layer_name
-    warn "Skipping #{layer_name}"
+    warn "--- Skipping #{layer_name}… ---"
   else
     info "--- Running XOR for layer #{layer_name} ---"
 
     layer_info = layers[layer_name]
-    xor_data = a.input(layer_name) ^ b.input(layer_name)
+    xor_data = (a.input(layer_name, layer_data) ^ b.input(layer_name, layer_data))
     total_xor_differences += xor_data.data.size
     info "XOR differences: #{xor_data.data.size}"
 
     write_data xor_data, layer_info
    end
 end
 
 info "---"
 info "Total XOR differences: #{total_xor_differences}"
 
-puts "%OL_CREATE_REPORT difference_count.rpt"
-puts total_xor_differences
-puts "%OL_END_REPORT"
+puts "%OL_METRIC_I design__xor_difference__count #{total_xor_differences}"
```

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/def/antenna_check.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/def/antenna_check.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/def/mag.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/def/mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/extract_spice.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/extract_spice.tcl`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 if { $::env(MAGIC_EXT_USE_GDS) } {
-    source $::env(SCRIPTS_DIR)/magic/gds/read.tcl
+    gds read $::env(CURRENT_GDS)
 } else {
-    source $::env(SCRIPTS_DIR)/magic/def/read.tcl
+    source $::env(SCRIPTS_DIR)/magic/common/read.tcl
+    read_tech_lef
+    read_pdk_lef
+    read_macro_lef
+    read_extra_lef
+    read_def
 }
 
 load $::env(DESIGN_NAME) -dereference
 
+set backup $::env(PWD)
 set extdir $::env(STEP_DIR)/extraction
-set feedback_file $::env(STEP_DIR)/feedback.txt
 set netlist $::env(STEP_DIR)/$::env(DESIGN_NAME).spice
 
 file mkdir $extdir
 cd $extdir
 
 extract do local
 extract no capacitance
@@ -41,9 +46,10 @@
 
 # For designs where more than one top-level pin is connected to the same net
 if { $::env(MAGIC_EXT_SHORT_RESISTOR) } {
     ext2spice short resistor
 }
 
 ext2spice -o $netlist $::env(DESIGN_NAME).ext
-feedback save $feedback_file
-# exec cp $::env(DESIGN_NAME).spice $::env(signoff_results)/$::env(DESIGN_NAME).spice
+
+cd $backup
+feedback save $::env(STEP_DIR)/feedback.txt
```

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/gds/drc_batch.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/gds/drc_batch.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/gds/erase_box.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/gds/erase_box.tcl`

 * *Files 12% similar despite different names*

```diff
@@ -24,12 +24,9 @@
 erase
 select area
 delete
 
 select top cell
 erase labels
 
-if { $::env(MAGIC_GDS_ALLOW_ABSTRACT) } {
-    gds abstract allow
-}
 
 gds write $::env(SAVE_GDS)
```

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/gds/extras_mag.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/gds/extras_mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/gds/mag_with_pointers.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/gds/mag_with_pointers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/gds/read.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/gui.tcl`

 * *Files 20% similar despite different names*

```diff
@@ -7,18 +7,9 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-gds read $::env(CURRENT_GDS)
-
-foreach file $::env(CELL_GDS) {
-    gds read $file
-}
-
-if { [info exist ::env(EXTRA_GDS_FILES)] } {
-    foreach file $::env(EXTRA_GDS_FILES) {
-        gds read $file
-    }
-}
+source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
+read_current_odb
```

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/lef/extras_maglef.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/lef/extras_maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/lef/maglef.tcl` & `openlane-2.0.0rc2/openlane/scripts/magic/lef/maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/lef.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_power_nets.tcl`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,30 @@
-# Copyright 2020-2023 Efabless Corporation
+# Copyright 2021-2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-drc off
-if { $::env(MAGIC_LEF_WRITE_USE_GDS) } {
-    gds read $::env(CURRENT_GDS)
-} else {
-    source $::env(SCRIPTS_DIR)/magic/def/read.tcl
-}
 
 if { [info exists ::env(VDD_NETS)] || [info exists ::env(GND_NETS)] } {
     # they both must exist and be equal in length
     # current assumption: they cannot have a common ground
     if { ! [info exists ::env(VDD_NETS)] || ! [info exists ::env(GND_NETS)] } {
-        puts "\[ERROR] VDD_NETS and GND_NETS must *both* either be defined or undefined"
+        puts stderr "\[ERROR] VDD_NETS and GND_NETS must *both* either be defined or undefined"
         exit -1
     }
+    set ::env(VDD_NET) [lindex $::env(VDD_NETS) 0]
+    set ::env(GND_NET) [lindex $::env(GND_NETS) 0]
+
 } else {
+    set ::env(VDD_NET) $::env(VDD_PIN)
+    set ::env(GND_NET) $::env(GND_PIN)
     set ::env(VDD_NETS) $::env(VDD_PIN)
     set ::env(GND_NETS) $::env(GND_PIN)
 }
-
-puts "\[INFO] Ignoring '$::env(VDD_NETS) $::env(GND_NETS)'"
-lef nocheck $::env(VDD_NETS) $::env(GND_NETS)
-
-# Write LEF
-if { $::env(MAGIC_WRITE_FULL_LEF) } {
-    puts "\[INFO] Writing non-abstract (full) LEF"
-    lef write $::env(STEP_DIR)/$::env(DESIGN_NAME).lef
-} else {
-    puts "\[INFO] Writing abstract LEF"
-    lef write $::env(STEP_DIR)/$::env(DESIGN_NAME).lef -hide
-}
-puts "\[INFO] LEF Write Complete"
```

### Comparing `openlane-2.0.0b9/openlane/scripts/magic/wrapper.tcl` & `openlane-2.0.0rc2/openlane/scripts/odbpy/exception_codes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# Copyright 2020-2022 Efabless Corporation
+# Copyright 2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-if {[catch {source $::env(MAGIC_SCRIPT)} err]} {
-    puts "Error: $err"
-    exit 1
-}
+METAL_LAYER_ERROR = 10
+FORMAT_ERROR = 11
+NOT_FOUND_ERROR = 12
```

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/apply_def_template.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/apply_def_template.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,30 +9,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import defutil
+import utl
 
 from reader import click_odb, click
 
 
 @click.command()
 @click.option("-t", "--def-template", required=True, help="Template DEF")
+@click.option(
+    "--copy-def-power",
+    default=False,
+    is_flag=True,
+    help="Whether to copy power pins from the DEF template",
+)
+@click.option(
+    "--permissive/--strict",
+    default=False,
+    help="Whether to treat pin matching permissively (ignoring non-matching pins) or strictly (flagging all non-matching pins as errors)",
+)
 @click_odb
-def cli(reader, input_lefs, def_template):
+def cli(reader, input_lefs, permissive, copy_def_power, def_template):
     defutil.relocate_pins(
         reader.db,
         input_lefs,
         def_template,
+        permissive,
+        copy_def_power,
     )
-
-    defutil.move_diearea(
-        reader.db,
-        input_lefs,
-        def_template,
-    )
+    area = defutil.get_die_area(def_template, input_lefs)
+    area_metric = f"{area[0]} {area[1]} {area[2]} {area[3]}"
+    utl.metric("design__die__bbox", area_metric)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/contextualize.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/contextualize.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/defutil.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/defutil.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,40 +14,24 @@
 # limitations under the License.
 import odb
 
 import os
 import re
 import sys
 
-from reader import OdbReader, click_odb, click
+from reader import click_odb, click
+from typing import Tuple, List
+from exception_codes import METAL_LAYER_ERROR, FORMAT_ERROR, NOT_FOUND_ERROR
 
 
 @click.group()
 def cli():
     pass
 
 
-@click.command("extract_core_dims")
-@click.option("-o", "--output-data", required=True, help="Output")
-@click.option("-l", "--input-lef", required=True, help="Merged LEF file")
-@click.argument("input_def")
-def extract_core_dims(output_data, input_lef, input_def):
-    reader = OdbReader(input_lef, input_def)
-    core_area = reader.block.getCoreArea()
-
-    with open(output_data, "w") as f:
-        print(
-            f"{core_area.dx() / reader.dbunits} {core_area.dy() / reader.dbunits}",
-            file=f,
-        )
-
-
-cli.add_command(extract_core_dims)
-
-
 @click.command("mark_component_fixed")
 @click.option(
     "-c", "--cell-name", required=True, help="Cell name of the components to mark fixed"
 )
 @click_odb
 def mark_component_fixed(cell_name, reader):
     instances = reader.block.getInsts()
@@ -55,45 +39,39 @@
         if instance.getMaster().getName() == cell_name:
             instance.setPlacementStatus("FIRM")
 
 
 cli.add_command(mark_component_fixed)
 
 
-@click.command("merge_components")
-@click.option(
-    "-w",
-    "--with-components-from",
-    "donor_def",
-    required=True,
-    help="A donor def file from which to extract components.",
-)
-@click_odb
-def merge_components(reader, donor_def, input_lefs):
-    """
-    Adds all components in a donor DEF file that do not exist in the (recipient) INPUT_DEF.
-
-    Existing components with the same name will *not* be overwritten.
-    """
-    donor = OdbReader(input_lefs, donor_def)
-    recipient = reader
-
-    for instance in donor.instances:
-        odb.dbInst_create(recipient.block, instance.getMaster(), instance.getName())
-
+def get_die_area(def_file, input_lefs):
+    die_area_dbu = (-1, -1, -1, -1)
+    db = odb.dbDatabase.create()
+    for lef in input_lefs:
+        odb.read_lef(db, lef)
+    odb.read_def(db.getTech(), def_file)
+    die_area = db.getChip().getBlock().getDieArea()
+    if die_area:
+        dbu = db.getChip().getBlock().getDefUnits()
+        die_area_dbu = (
+            die_area.xMin() / dbu,
+            die_area.yMin() / dbu,
+            die_area.xMax() / dbu,
+            die_area.yMax() / dbu,
+        )
 
-cli.add_command(merge_components)
+    return die_area_dbu
 
 
 def move_diearea(target_db, input_lefs, template_def):
     source_db = odb.dbDatabase.create()
 
     for lef in input_lefs:
         odb.read_lef(source_db, lef)
-    odb.read_def(source_db, template_def)
+    odb.read_def(source_db.getTech(), template_def)
 
     assert (
         source_db.getTech().getManufacturingGrid()
         == target_db.getTech().getManufacturingGrid()
     )
     assert (
         source_db.getTech().getDbUnitsPerMicron()
@@ -114,20 +92,21 @@
     """
     move_diearea(reader.db, input_lefs, template_def)
 
 
 def check_pin_grid(manufacturing_grid, dbu_per_microns, pin_name, pin_coordinate):
     if (pin_coordinate % manufacturing_grid) != 0:
         print(
-            f"[ERROR]: Pin {pin_name}'s coordinate {pin_coordinate} does not lie on the manufacturing grid."
+            f"[ERROR] Pin {pin_name}'s coordinate {pin_coordinate} does not lie on the manufacturing grid.",
+            file=sys.stderr,
         )  # IDK how to do this
         return True
 
 
-def relocate_pins(db, input_lefs, template_def):
+def relocate_pins(db, input_lefs, template_def, permissive, copy_def_power=False):
     # --------------------------------
     # 1. Find list of all bterms in existing database
     # --------------------------------
     source_db = db
     source_bterms = source_db.getChip().getBlock().getBTerms()
 
     manufacturing_grid = source_db.getTech().getManufacturingGrid()
@@ -148,42 +127,43 @@
         # --------------------------------
         # 3. Check no bterms should be marked as power, because it is assumed that caller already removed them
         # --------------------------------
         sigtype = source_bterm.getSigType()
         if sigtype in ["POWER", "GROUND"]:
             print(
                 f"[WARNING] Bterm {source_name} is declared as a '{sigtype}' pin. It will be ignored.",
+                file=sys.stderr,
             )
             continue
         all_bterm_names.add(source_name)
 
     print(
         f"Found {len(all_bterm_names)} block terminals in existing database...",
     )
 
     # --------------------------------
     # 2. Read the donor def
     # --------------------------------
     template_db = odb.dbDatabase.create()
     for lef in input_lefs:
         odb.read_lef(template_db, lef)
-    odb.read_def(template_db, template_def)
+    odb.read_def(template_db.getTech(), template_def)
     template_bterms = template_db.getChip().getBlock().getBTerms()
 
     assert (
         source_db.getTech().getManufacturingGrid()
         == template_db.getTech().getManufacturingGrid()
     )
     assert (
         source_db.getTech().getDbUnitsPerMicron()
         == template_db.getTech().getDbUnitsPerMicron()
     )
 
     # --------------------------------
-    # 3. Create a dict with net -> pin location. Check for only one pin location to exist, overwise return an error
+    # 3. Create a dict with net -> pin locations.
     # --------------------------------
     template_bterm_locations = dict()
 
     for template_bterm in template_bterms:
         template_name = template_bterm.getName()
         template_pins = template_bterm.getBPins()
 
@@ -201,100 +181,156 @@
                         box.xMin(),
                         box.yMin(),
                         box.xMax(),
                         box.yMax(),
                     )
                 )
 
-    print(f"Found {len(template_bterm_locations)} template_bterms:")
+    template_bterm_names = set(
+        [
+            bterm.getName()
+            for bterm in template_bterms
+            if bterm.getSigType() not in ["POWER", "GROUND"]
+        ]
+    )
 
-    for name in template_bterm_locations.keys():
-        print(f"  * {name}: {template_bterm_locations[name]}")
+    print(f"Found {len(template_bterm_locations)} template_bterms…")
+
+    # for name in template_bterm_locations.keys():
+    #     print(f"  * {name}: {template_bterm_locations[name]}")
 
     # --------------------------------
     # 4. Modify the pins in out def, according to dict
     # --------------------------------
     output_db = db
     output_tech = output_db.getTech()
     output_block = output_db.getChip().getBlock()
     output_bterms = output_block.getBTerms()
+
+    if copy_def_power:
+        output_bterm_names = set([bterm.getName() for bterm in output_bterms])
+    else:
+        output_bterm_names = set(
+            [
+                bterm.getName()
+                for bterm in output_bterms
+                if bterm.getNet().getSigType() not in ["POWER", "GROUND"]
+            ]
+        )
+    not_in_design = template_bterm_names - output_bterm_names
+    not_in_template = output_bterm_names - template_bterm_names
+
+    mismatches_found = False
+    for is_in, not_in, pins in [
+        ("template", "design", not_in_design),
+        ("design", "template", not_in_template),
+    ]:
+        for name in pins:
+            mismatches_found = True
+            if permissive:
+                print(
+                    f"[WARNING] {name} not found in {not_in} layout, but found in {is_in} layout.",
+                )
+            else:
+                print(
+                    f"[ERROR] {name} not found in {not_in} layout, but found in {is_in} layout.",
+                    file=sys.stderr,
+                )
+
+    if mismatches_found and not permissive:
+        exit(os.EX_DATAERR)
+
+    if copy_def_power:
+        # If asked, we copy power pins from template
+        for bterm in template_bterms:
+            if bterm.getSigType() not in ["POWER", "GROUND"]:
+                continue
+            pin_name = bterm.getName()
+            pin_net = odb.dbNet.create(output_block, pin_name, True)
+            pin_net.setSpecial()
+            pin_net.setSigType(bterm.getSigType())
+            pin_bterm = odb.dbBTerm.create(pin_net, pin_name)
+            pin_bterm.setSigType(bterm.getSigType())
+            output_bterms.append(pin_bterm)
+
     grid_errors = False
     for output_bterm in output_bterms:
         name = output_bterm.getName()
         output_bpins = output_bterm.getBPins()
 
-        if name in template_bterm_locations and name in all_bterm_names:
-            for output_bpin in output_bpins:
-                odb.dbBPin.destroy(output_bpin)
-
-            for template_bterm_location_tuple in template_bterm_locations[name]:
-                layer = output_tech.findLayer(template_bterm_location_tuple[0])
-
-                # --------------------------------
-                # 6.2 Create new pin
-                # --------------------------------
+        if name not in template_bterm_locations:
+            continue
 
-                output_new_bpin = odb.dbBPin.create(output_bterm)
+        if (name not in all_bterm_names) and not copy_def_power:
+            continue
 
-                print(
-                    f"Wrote pin {name} at layer {layer.getName()} at {template_bterm_location_tuple[1:]}..."
-                )
-                grid_errors = (
-                    check_pin_grid(
-                        manufacturing_grid,
-                        dbu_per_microns,
-                        name,
-                        template_bterm_location_tuple[1],
-                    )
-                    or grid_errors
-                )
-                grid_errors = (
-                    check_pin_grid(
-                        manufacturing_grid,
-                        dbu_per_microns,
-                        name,
-                        template_bterm_location_tuple[2],
-                    )
-                    or grid_errors
-                )
-                grid_errors = (
-                    check_pin_grid(
-                        manufacturing_grid,
-                        dbu_per_microns,
-                        name,
-                        template_bterm_location_tuple[3],
-                    )
-                    or grid_errors
-                )
-                grid_errors = (
-                    check_pin_grid(
-                        manufacturing_grid,
-                        dbu_per_microns,
-                        name,
-                        template_bterm_location_tuple[4],
-                    )
-                    or grid_errors
-                )
-                odb.dbBox.create(
-                    output_new_bpin,
-                    layer,
+        for output_bpin in output_bpins:
+            odb.dbBPin.destroy(output_bpin)
+
+        for template_bterm_location_tuple in template_bterm_locations[name]:
+            layer = output_tech.findLayer(template_bterm_location_tuple[0])
+
+            # --------------------------------
+            # 6.2 Create new pin
+            # --------------------------------
+
+            output_new_bpin = odb.dbBPin.create(output_bterm)
+
+            print(
+                f"Wrote pin {name} at layer {layer.getName()} at {template_bterm_location_tuple[1:]}..."
+            )
+            grid_errors = (
+                check_pin_grid(
+                    manufacturing_grid,
+                    dbu_per_microns,
+                    name,
                     template_bterm_location_tuple[1],
+                )
+                or grid_errors
+            )
+            grid_errors = (
+                check_pin_grid(
+                    manufacturing_grid,
+                    dbu_per_microns,
+                    name,
                     template_bterm_location_tuple[2],
+                )
+                or grid_errors
+            )
+            grid_errors = (
+                check_pin_grid(
+                    manufacturing_grid,
+                    dbu_per_microns,
+                    name,
                     template_bterm_location_tuple[3],
+                )
+                or grid_errors
+            )
+            grid_errors = (
+                check_pin_grid(
+                    manufacturing_grid,
+                    dbu_per_microns,
+                    name,
                     template_bterm_location_tuple[4],
                 )
-                output_new_bpin.setPlacementStatus("PLACED")
-        else:
-            print(
-                f"{name} not found in donor def, but found in output def. Leaving as-is.",
+                or grid_errors
+            )
+            odb.dbBox.create(
+                output_new_bpin,
+                layer,
+                template_bterm_location_tuple[1],
+                template_bterm_location_tuple[2],
+                template_bterm_location_tuple[3],
+                template_bterm_location_tuple[4],
             )
+            output_new_bpin.setPlacementStatus("PLACED")
 
     if grid_errors:
         print(
-            "[ERROR]: Some pins were grid-misaligned. Please check the log.",
+            "[ERROR] Some pins were grid-misaligned. Please check the log.",
             file=sys.stderr,
         )
         exit(os.EX_DATAERR)
 
 
 @click.command("relocate_pins")
 @click.option(
@@ -412,57 +448,126 @@
             new_name = name.replace(f"{original_prefix}_", f"{new_prefix}_")
             instance.rename(new_name)
 
 
 cli.add_command(replace_instance_prefixes)
 
 
-@click.command("add_obstructions")
-@click.option(
-    "-O",
-    "--obstructions",
-    required=True,
-    help="Format: layer llx lly urx ury, (microns)",
-)
-@click_odb
-def add_obstructions(obstructions, reader):
+def parse_obstructions(obstructions):
     RE_NUMBER = r"[\-]?[0-9]+(\.[0-9]+)?"
     RE_OBS = (
         r"(?P<layer>\S+)\s+"
         + r"(?P<bbox>"
         + RE_NUMBER
         + r"\s+"
         + RE_NUMBER
         + r"\s+"
         + RE_NUMBER
         + r"\s+"
         + RE_NUMBER
-        + r")"
+        + r") *$"
     )
 
-    obses = obstructions.split(",")
     obs_list = []
-    for obs in obses:
+    for obs in obstructions:
         obs = obs.strip()
         m = re.match(RE_OBS, obs)
-        assert (
-            m
-        ), "Incorrectly formatted input (%s).\n Format: layer llx lly urx ury, ..." % (
-            obs
-        )
-        layer = m.group("layer")
-        bbox = [float(x) for x in m.group("bbox").split()]
-        obs_list.append((layer, bbox))
+        if m is None:
+            print(
+                f"[ERROR] Incorrectly formatted input {obs}.\n Format: layer llx lly urx ury, ...",
+                file=sys.stderr,
+            )
+            sys.exit(FORMAT_ERROR)
+        else:
+            layer = m.group("layer")
+            bbox = [float(x) for x in m.group("bbox").split()]
+            obs_list.append((layer, bbox))
+
+    return obs_list
+
 
+@click.command("add_obstructions")
+@click.option(
+    "-O",
+    "--obstructions",
+    multiple=True,
+    required=True,
+    help="Format: layer llx lly urx ury, (microns)",
+)
+@click_odb
+def add_obstructions(reader, input_lefs, obstructions):
+    obs_list = parse_obstructions(obstructions)
     for obs in obs_list:
         layer = obs[0]
+        odb_layer = reader.tech.findLayer(layer)
+        if odb_layer is None:
+            print(f"[ERROR] layer {layer} doesn't exist.", file=sys.stderr)
+            sys.exit(METAL_LAYER_ERROR)
         bbox = obs[1]
         dbu = reader.tech.getDbUnitsPerMicron()
         bbox = [int(x * dbu) for x in bbox]
-        print("Creating an obstruction on", layer, "at", *bbox, "(DBU)")
+        print(f"Creating an obstruction on {layer} at {bbox} (DBU)…")
         odb.dbObstruction_create(reader.block, reader.tech.findLayer(layer), *bbox)
 
 
 cli.add_command(add_obstructions)
 
+
+@click.command("remove_obstructions")
+@click.option(
+    "-O",
+    "--obstructions",
+    multiple=True,
+    required=True,
+    help="Format: layer llx lly urx ury, (microns)",
+)
+@click_odb
+def remove_obstructions(reader, input_lefs, obstructions):
+    obs_list = parse_obstructions(obstructions)
+    existing_obstructions: List[Tuple[str, List[int], odb.dbObstruction]] = []
+    dbu = reader.tech.getDbUnitsPerMicron()
+
+    def to_microns(x):
+        return int(x / dbu)
+
+    for odb_obstruction in reader.block.getObstructions():
+        bbox = odb_obstruction.getBBox()
+        existing_obstructions.append(
+            (
+                bbox.getTechLayer().getName(),
+                [
+                    to_microns(bbox.xMin()),
+                    to_microns(bbox.yMin()),
+                    to_microns(bbox.xMax()),
+                    to_microns(bbox.yMax()),
+                ],
+                odb_obstruction,
+            )
+        )
+
+    for obs in obs_list:
+        layer = obs[0]
+        bbox = obs[1]
+        bbox = [int(x * dbu) for x in bbox]
+        found = False
+        if reader.tech.findLayer(layer) is None:
+            print(f"[ERROR] layer {layer} doesn't exist.", file=sys.stderr)
+            sys.exit(METAL_LAYER_ERROR)
+        for odb_obstruction in existing_obstructions:
+            if odb_obstruction[0:2] == obs:
+                print(f"Removing obstruction on {layer} at {bbox} (DBU)…")
+                found = True
+                odb.dbObstruction_destroy(odb_obstruction[2])
+            if found:
+                break
+        if not found:
+            print(
+                f"[ERROR] Obstruction on {layer} at {bbox} (DBU) not found.",
+                file=sys.stderr,
+            )
+            sys.exit(NOT_FOUND_ERROR)
+
+
+cli.add_command(remove_obstructions)
+
 if __name__ == "__main__":
     cli()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/diodes.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/diodes.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,47 +16,51 @@
 
 import odb
 
 import sys
 import click
 import random
 from decimal import Decimal
-
-from reader import click_odb
+from typing import Optional, List
+from reader import click_odb, OdbReader
 
 
 @click.group()
 def cli():
     pass
 
 
 class DiodeInserter:
     def __init__(
         self,
-        block,
-        diode_cell,
-        diode_pin,
-        side_strategy="source",
-        threshold_microns=0,
-        port_protect=[],
+        reader: OdbReader,
+        diode_cell: str,
+        diode_pin: str,
+        threshold_microns: Decimal,
+        side_strategy: str = "source",
+        port_protect_polarities: Optional[List[str]] = None,
         verbose=False,
     ):
-        self.block = block
+        print(f"Using threshold {threshold_microns}µm…")
+
+        self.reader = reader
+        self.block = reader.block
         self.verbose = verbose
 
         self.diode_cell = diode_cell
         self.diode_pin = diode_pin
         self.side_strategy = side_strategy
         self.threshold_microns = threshold_microns
-        self.port_protect = port_protect
+        self.port_protect = port_protect_polarities or []
 
-        self.diode_master = block.getDataBase().findMaster(diode_cell)
+        self.diode_master = self.block.getDataBase().findMaster(diode_cell)
         self.diode_site = self.diode_master.getSite().getConstName()
 
         self.inserted = {}
+        self.insts_by_name = {i.getName(): i for i in self.block.getInsts()}
 
     def debug(self, msg):
         if self.verbose:
             print(msg, file=sys.stderr)
 
     def error(self, msg):
         print(msg, file=sys.stderr)
@@ -86,22 +90,27 @@
 
     def net_from_pin(self, net, io_types=None):
         for bt in net.getBTerms():
             if (io_types is None) or (bt.getIoType() in io_types):
                 return True
         return False
 
-    def net_has_diode(self, net):
+    def net_has_diode(self, net, *, silly_verbose=False):
         for it in net.getITerms():
             cell_type = it.getInst().getMaster().getConstName()
             cell_pin = it.getMTerm().getConstName()
+            if silly_verbose:
+                print(
+                    f"Net {net.getName()} is connected to {cell_type}/{cell_pin} via {it.getInst().getName()}"
+                )
             if (cell_type == self.diode_cell) and (cell_pin == self.diode_pin):
+                if silly_verbose:
+                    print("Found diode!")
                 return True
-        else:
-            return False
+        return False
 
     def net_manhattan_distance(self, net):
         xs = []
         ys = []
 
         for bt in net.getBTerms():
             good, x, y = bt.getFirstPinLocation()
@@ -195,60 +204,66 @@
             d = abs(px - dx) + abs(py - dy)
 
             if (best is None) or (best[0] > d):
                 best = (d, dx, dy, do)
 
         return best[1:]
 
-    def insert_diode(self, it, src_pos):
+    def insert_diode(self, net, iterm, src_pos):
         # Get information about the instance
-        inst = it.getInst()
+        inst = iterm.getInst()
         inst_name = inst.getConstName()
         inst_site = (
             inst.getMaster().getSite().getConstName()
             if (inst.getMaster().getSite() is not None)
             else None
         )
 
         # Find where the pin is
-        px, py = self.pin_position(it)
+        px, py = self.pin_position(iterm)
 
         # Apply standard cell or macro placement ?
         if inst_site == self.diode_site:
-            dx, dy, do = self.place_diode_stdcell(it, px, py, src_pos)
+            dx, dy, do = self.place_diode_stdcell(iterm, px, py, src_pos)
         else:
-            dx, dy, do = self.place_diode_macro(it, px, py, src_pos)
+            dx, dy, do = self.place_diode_macro(iterm, px, py, src_pos)
 
         # Insert instance and wire it up
-        diode_inst_name = "ANTENNA_" + inst_name + "_" + it.getMTerm().getConstName()
-        diode_master = self.diode_master
+        base_diode_inst_name = f"ANTENNA_{inst_name}_{iterm.getMTerm().getConstName()}"
+        diode_inst_name = base_diode_inst_name
+        counter = 0
+        while self.insts_by_name.get(diode_inst_name) is not None:
+            self.debug(
+                f"[d] Net {net.getName()}: diode {diode_inst_name} appears to already exist."
+            )
+            counter += 1
+            diode_inst_name = f"{base_diode_inst_name}_{counter}"
 
-        diode_inst = odb.dbInst_create(self.block, diode_master, diode_inst_name)
+        diode_inst = odb.dbInst_create(self.block, self.diode_master, diode_inst_name)
 
         diode_inst.setOrient(do)
         diode_inst.setLocation(dx, dy)
         diode_inst.setPlacementStatus("PLACED")
 
         ait = diode_inst.findITerm(self.diode_pin)
-        ait.connect(it.getNet())
+        ait.connect(iterm.getNet())
 
     def execute(self):
         # Scan all nets
         for net in self.block.getNets():
             # Skip special nets
             if net.isSpecial():
                 self.debug(f"[d] Skipping special net {net.getConstName():s}")
                 continue
 
             # Check if we already have diode on the net
-            # if yes, then we assume that the user took care of that net manually
-            if self.net_has_diode(net):
-                self.debug(
-                    f"[d] Skipping manually protected net {net.getConstName():s}"
-                )
+            # if yes, then we assume that the user took care of that some
+            # other way
+            if self.net_has_diode(net, silly_verbose=False):
+                self.debug(f"[d] Skipping already-protected net {net.getConstName():s}")
                 continue
 
             # Find signal source (first one found ...)
             src_pos = self.net_source(net)
 
             # Is this an IO we need to protect
             io_protect = None
@@ -261,21 +276,28 @@
                 else:
                     self.debug(f"[d] Skipping I/O net {net.getConstName():s}")
                     continue
 
             # Determine the span of the signal and skip small internal nets
             span = self.net_manhattan_distance(net) / self.block.getDbUnitsPerMicron()
             if (span < self.threshold_microns) and not io_protect:
-                self.debug(f"[d] Skipping small net {net.getConstName():s} ({span:f})")
+                if self.threshold_microns != Decimal("Infinity"):
+                    self.debug(
+                        f"[d] Skipping small net {net.getConstName():s} ({span:f})"
+                    )
                 continue
 
+            self.debug(
+                f"[d] Inserting diode(s) for net {net.getConstName():s} ({span:f})"
+            )
+
             # Scan all internal terminals
-            for it in net.getITerms():
-                if it.isInputSignal():
-                    self.insert_diode(it, src_pos)
+            for iterm in net.getITerms():
+                if iterm.isInputSignal():
+                    self.insert_diode(net, iterm, src_pos)
 
 
 @click.command()
 @click.option(
     "-v", "--verbose", default=False, is_flag=True, help="Verbose debug output"
 )
 @click.option(
@@ -300,44 +322,43 @@
     help="Always place a true diode on nets connected to selected ports",
 )
 @click.option(
     "-t",
     "--threshold",
     "threshold_microns",
     type=Decimal,
-    default=90,
-    help="Minimum manhattan distance of a net to be considered an antenna risk requiring a diode",
+    default=None,
+    help="Minimum Manhattan distance of a net to be considered an antenna risk requiring a diode. By default, the value used is 200 * the minimum site width.",
 )
 @click_odb
 def place(
     reader,
     verbose,
     diode_cell,
     diode_pin,
     side_strategy,
     port_protect,
     threshold_microns,
 ):
-
     print(f"Design name: {reader.name}")
 
     pp_val = {
         "none": [],
         "in": ["INPUT"],
         "out": ["OUTPUT"],
         "both": ["INPUT", "OUTPUT"],
     }
 
     di = DiodeInserter(
-        reader.block,
+        reader,
         diode_cell=diode_cell,
         diode_pin=diode_pin,
         side_strategy=side_strategy,
         threshold_microns=threshold_microns,
-        port_protect=pp_val[port_protect],
+        port_protect_polarities=pp_val[port_protect],
         verbose=verbose,
     )
     di.execute()
 
     print("Inserted", len(di.inserted), "diodes.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/io_place.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/io_place.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from functools import partial
 import odb
 
 import os
 import re
 import sys
 import math
 import click
 import random
+from decimal import Decimal
 
 from reader import click_odb
+import ioplace_parser
 
 
 def grid_to_tracks(origin, count, step):
     tracks = []
     pos = origin
     for _ in range(count):
         tracks.append(pos)
@@ -49,15 +52,20 @@
             )  # Decrement actual pin count, this value was only there to indicate virtual pin count
             total_pin_count = actual_pin_count + virtual_pin_count
     result = []
     tracks = len(possible_locations)
 
     if total_pin_count > tracks:
         print(
-            f"There are more pins/virtual_pins: {total_pin_count}, than places to put them: {tracks} in the {side} side. Try making your floorplan area larger."
+            f"[ERROR] The {side} side of the floorplan doesn't have enough slots for all the pins: {total_pin_count} pins/{tracks} slots.",
+            file=sys.stderr,
+        )
+        print(
+            "[INFO] Try re-assigning pins to other sides or making the floorplan larger.",
+            file=sys.stderr,
         )
         sys.exit(1)
     elif total_pin_count == tracks:
         return possible_locations, side_pin_placement  # All positions.
     elif total_pin_count == 0:
         return result, side_pin_placement
 
@@ -94,15 +102,15 @@
     print("Total pin count: ", total_pin_count)
     print("Tracks count: ", len(possible_locations))
     print("Tracks per pin: ", tracks_per_pin)
     print("Used tracks count: ", used_tracks)
     print("Unused track count: ", unused_tracks)
     print("Starting track index: ", starting_track_index)
 
-    VISUALIZE_PLACEMENT = True
+    VISUALIZE_PLACEMENT = False
     if VISUALIZE_PLACEMENT:
         print("Placement Map:")
         print("[", end="")
         used_track_indices = []
         for i, location in enumerate(possible_locations):
             if location in result:
                 print(f"\033[91m{location}\033[0m, ", end="")
@@ -112,60 +120,80 @@
         print("]")
         print(f"Indices of used tracks: {used_track_indices}")
         print("---")
 
     return result, side_pin_placement
 
 
-# HUMAN SORTING: https://stackoverflow.com/questions/5967500/how-to-correctly-sort-a-string-with-a-number-inside
-def natural_keys(enum):
-    def atof(text):
-        try:
-            retval = float(text)
-        except ValueError:
-            retval = text
-        return retval
-
-    text = enum[0]
-    text = re.sub(r"(\[|\]|\.|\$)", "", text)
-    """
-    alist.sort(key=natural_keys) sorts in human order
-    http://nedbatchelder.com/blog/200712/human_sorting.html
-    (see toothy's implementation in the comments)
-    float regex comes from https://stackoverflow.com/a/12643073/190597
-    """
-    return [atof(c) for c in re.split(r"[+-]?([0-9]+(?:[.][0-9]*)?|[.][0-9]+)", text)]
-
-
-def bus_keys(enum):
-    text = enum[0]
-    m = re.match(r"^.*\[(\d+)\]$", text)
-    if not m:
-        return -1
-    else:
-        return int(m.group(1))
+identifiers = re.compile(r"\b[A-Za-z_][A-Za-z_0-9]*\b")
+standalone_numbers = re.compile(r"\b\d+\b")
+trash = re.compile(r"^[^\w\d]+$")
+
+
+def sorter(bterm, order: ioplace_parser.Order):
+    text: str = bterm.getName()
+    keys = []
+    priority_keys = []
+    # tokenize and add to key
+    while trash.match(text) is None:
+        if match := identifiers.search(text):
+            bus = match[0]
+            start, end = match.span(0)
+            if order == ioplace_parser.Order.busMajor:
+                priority_keys.append(bus)
+            else:
+                keys.append(bus)
+            text = text[:start] + text[end + 1 :]
+        elif match := standalone_numbers.search(text):
+            index = int(match[0])
+            if order == ioplace_parser.Order.bitMajor:
+                priority_keys.append(index)
+            else:
+                keys.append(index)
+            text = text[: match.pos] + text[match.endpos + 1 :]
+        else:
+            break
+    return [priority_keys, keys]
 
 
 @click.command()
 @click.option(
     "-u",
     "--unmatched-error",
-    is_flag=True,
-    default=False,
+    type=click.Choice(["none", "unmatched_design", "unmatched_cfg", "both"]),
+    default=True,
     help="Treat unmatched pins as error",
 )
-@click.option("-c", "--config", required=False, help="Optional configuration file.")
 @click.option(
-    "-r",
-    "--reverse",
-    default="",
-    type=str,
-    help="Reverse along comma,delimited,cardinals: e.g. N,E",
+    "-c",
+    "--config",
+    required=True,
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    help="Input configuration file",
+)
+@click.option(
+    "-v",
+    "--ver-length",
+    default=None,
+    type=float,
+    help="Length for pins with N/S orientations in microns.",
+)
+@click.option(
+    "-h",
+    "--hor-length",
+    default=None,
+    type=float,
+    help="Length for pins with E/S orientations in microns.",
 )
-@click.option("-L", "--length", default=2, type=float, help="Pin length in microns.")
 @click.option(
     "-V",
     "--ver-layer",
     required=True,
     help="Name of metal layer to place vertical pins on.",
 )
 @click.option(
@@ -188,197 +216,184 @@
 )
 @click.option(
     "--ver-width-mult", default=2, type=float, help="Multiplier for vertical pins."
 )
 @click.option(
     "--hor-width-mult", default=2, type=float, help="Multiplier for horizontal pins."
 )
-@click.option(
-    "--bus-sort/--no-bus-sort",
-    default=False,
-    help="Misnomer: pins are grouped by index instead of bus, i.e. a[0] goes with b[0] instead of a[1].",
-)
 @click_odb
 def io_place(
     reader,
     config,
     ver_layer,
     hor_layer,
     ver_width_mult,
     hor_width_mult,
-    length,
+    hor_length,
+    ver_length,
     hor_extension,
     ver_extension,
-    reverse,
-    bus_sort,
     unmatched_error,
 ):
     """
     Places the IOs in an input def with an optional config file that supports regexes.
 
     Config format:
     #N|#S|#E|#W
     pin1_regex (low co-ordinates to high co-ordinates; e.g., bottom to top and left to right)
     pin2_regex
     ...
 
     #S|#N|#E|#W
     """
     config_file_name = config
-    bus_sort_flag = bus_sort
-    unmatched_error_flag = unmatched_error
-
-    h_layer_name = hor_layer
-    v_layer_name = ver_layer
-
-    h_width_mult = float(hor_width_mult)
-    v_width_mult = float(ver_width_mult)
-
     micron_in_units = reader.dbunits
 
-    LENGTH = int(micron_in_units * length)
-
     H_EXTENSION = int(micron_in_units * hor_extension)
     V_EXTENSION = int(micron_in_units * ver_extension)
 
     if H_EXTENSION < 0:
         H_EXTENSION = 0
 
     if V_EXTENSION < 0:
         V_EXTENSION = 0
 
-    reverse_arr_raw = reverse.split(",")
-    reverse_arr = []
-    for element in reverse_arr_raw:
-        if element.strip() != "":
-            reverse_arr.append(f"#{element}")
-    # read config
-
-    pin_placement_cfg = {"#N": [], "#E": [], "#S": [], "#W": []}
-    cur_side = None
-    if config_file_name is not None and config_file_name != "":
-        with open(config_file_name, "r") as config_file:
-            for line in config_file:
-                line = line.split()
-                if len(line) == 0:
-                    continue
+    H_LAYER = reader.tech.findLayer(hor_layer)
+    V_LAYER = reader.tech.findLayer(ver_layer)
 
-                if len(line) > 1:
-                    print("Only one entry allowed per line.")
-                    sys.exit(1)
-
-                token = line[0]
-
-                if cur_side is not None and token[0] != "#":
-                    pin_placement_cfg[cur_side].append(token)
-                elif token not in [
-                    "#N",
-                    "#E",
-                    "#S",
-                    "#W",
-                    "#NR",
-                    "#ER",
-                    "#SR",
-                    "#WR",
-                    "#BUS_SORT",
-                ]:
-                    print(
-                        "Valid directives are #N, #E, #S, or #W. Append R for reversing the default order.",
-                        "Use #BUS_SORT to group 'bus bits' by index.",
-                        "Please make sure you have set a valid side first before listing pins",
-                    )
-                    sys.exit(1)
-                elif token == "#BUS_SORT":
-                    bus_sort_flag = True
-                else:
-                    if len(token) == 3:
-                        token = token[0:2]
-                        reverse_arr.append(token)
-                    cur_side = token
+    H_WIDTH = int(Decimal(hor_width_mult) * H_LAYER.getWidth())
+    V_WIDTH = int(Decimal(ver_width_mult) * V_LAYER.getWidth())
 
-    # build a list of pins
-    H_LAYER = reader.tech.findLayer(h_layer_name)
-    V_LAYER = reader.tech.findLayer(v_layer_name)
+    if hor_length is not None:
+        H_LENGTH = int(micron_in_units * hor_length)
+    else:
+        H_LENGTH = max(
+            int(
+                math.ceil(
+                    H_LAYER.getArea() * micron_in_units * micron_in_units / H_WIDTH
+                )
+            ),
+            H_WIDTH,
+        )
 
-    H_WIDTH = int(h_width_mult * H_LAYER.getWidth())
-    V_WIDTH = int(v_width_mult * V_LAYER.getWidth())
+    if ver_length is not None:
+        V_LENGTH = int(micron_in_units * ver_length)
+    else:
+        V_LENGTH = max(
+            int(
+                math.ceil(
+                    V_LAYER.getArea() * micron_in_units * micron_in_units / V_WIDTH
+                )
+            ),
+            V_WIDTH,
+        )
+
+    # read config + calculate minima
+    config_file_str = open(config_file_name, "r", encoding="utf8").read()
+
+    try:
+        info_by_side = ioplace_parser.parse(config_file_str)
+    except ValueError as e:
+        print(f"An exception occurred: {e}")
+        exit(os.EX_DATAERR)
 
     print("Top-level design name:", reader.name)
 
-    bterms = reader.block.getBTerms()
-    bterms_enum = []
-    for bterm in bterms:
-        pin_name = bterm.getName()
-        bterms_enum.append((pin_name, bterm))
-
-    # sort them "humanly"
-    bterms_enum.sort(key=natural_keys)
-    if bus_sort_flag:
-        bterms_enum.sort(key=bus_keys)
-    bterms = [bterm[1] for bterm in bterms_enum]
-
-    pin_placement = {"#N": [], "#E": [], "#S": [], "#W": []}
-    pin_distance_min = {
-        "#N": V_WIDTH + V_LAYER.getSpacing(),
-        "#S": V_WIDTH + V_LAYER.getSpacing(),
-        "#E": H_WIDTH + H_LAYER.getSpacing(),
-        "#W": H_WIDTH + H_LAYER.getSpacing(),
-    }
-    pin_distance = pin_distance_min.copy()
-    bterm_regex_map = {}
-    for side in pin_placement_cfg:
-        for regex in pin_placement_cfg[side]:  # going through them in order
-            if regex[0] == "$":  # Sign of Virtual Pins
-                try:
-                    virtual_pins_count = int(regex[1:])
-                    pin_placement[side].append(virtual_pins_count)
-                except ValueError:
-                    print("You provided invalid values for virtual pins")
-                    sys.exit(1)
-            elif regex[0] == "@":
-                variable = regex[1:].split("=")
-                if variable[0] == "min_distance":
-                    pin_distance[side] = float(variable[1]) * reader.dbunits
-                    if pin_distance[side] < pin_distance_min[side]:
-                        print(
-                            f"Warning: Using min_distance {pin_distance_min[side] / reader.dbunits} for {side} pins to avoid overlap"
-                        )
-                        pin_distance[side] = pin_distance_min[side]
+    bterms = [
+        bterm
+        for bterm in reader.block.getBTerms()
+        if bterm.getSigType() not in ["POWER", "GROUND"]
+    ]
+
+    for side, side_info in info_by_side.items():
+        min = (
+            (V_WIDTH + V_LAYER.getSpacing())
+            if side in ["N", "S"]
+            else (H_WIDTH + H_LAYER.getSpacing())
+        ) / reader.dbunits
+        if side_info.min_distance is None:
+            side_info.min_distance = min
+        if side_info.min_distance < min:
+            print(
+                f"[WARNING] Overriding minimum distance {side_info.min_distance} with {min} for pins on side {side} to avoid overlap.",
+                file=sys.stderr,
+            )
+            side_info.min_distance = min
+
+    # build a list of pins
+    pin_placement = {"N": [], "E": [], "W": [], "S": []}
+
+    regex_by_bterm = {}
+    unmatched_regexes = set()
+    for side, side_info in info_by_side.items():
+        for pin in side_info.pins:
+            if isinstance(pin, int):  # Virtual pins
+                pin_placement[side].append(pin)
+                continue
+
+            anchored_regex = f"^{pin}$"  # anchor
+            matched = False
+            collected = []
+            for bterm in bterms:
+                pin_name = bterm.getName()
+                if re.match(anchored_regex, pin_name) is None:
+                    continue
+                if bterm in regex_by_bterm:
+                    print(
+                        f"[ERROR] Multiple regexes matched {pin_name}. Those are {regex_by_bterm[bterm]} and {pin}",
+                        file=sys.stderr,
+                    )
+                    sys.exit(os.EX_DATAERR)
+                regex_by_bterm[bterm] = pin
+                collected.append(bterm)
+                matched = True
+            collected.sort(key=partial(sorter, order=side_info.sort_mode))
+            pin_placement[side] += collected
+            if not matched:
+                unmatched_regexes.add(pin)
+
+    # check for extra or missing pins
+    not_in_design = unmatched_regexes
+    not_in_config = set(
+        [bterm.getName() for bterm in bterms if bterm not in regex_by_bterm]
+    )
+    mismatches_found = False
+    for is_in, not_in, pins in [
+        ("config", "design", not_in_design),
+        ("design", "config", not_in_config),
+    ]:
+        for name in pins:
+            if (
+                is_in == "config"
+                and (unmatched_error in {"unmatched_cfg", "both"})
+                or is_in == "design"
+                and (unmatched_error in {"unmatched_design", "both"})
+            ):
+                mismatches_found = True
+                print(
+                    f"[ERROR] {name} not found in {not_in} but found in {is_in}.",
+                    file=sys.stderr,
+                )
             else:
-                regex += "$"  # anchor
-                for bterm in bterms:
-                    # if a pin name matches multiple regexes, their order will be
-                    # arbitrary. More refinement requires more strict regexes (or just
-                    # the exact pin name).
-                    pin_name = bterm.getName()
-                    if re.match(regex, pin_name) is not None:
-                        if bterm in bterm_regex_map:
-                            print(
-                                f"Error: Multiple regexes matched {pin_name}. Those are {bterm_regex_map[bterm]} and {regex}"
-                            )
-                            sys.exit(os.EX_DATAERR)
-                        bterm_regex_map[bterm] = regex
-                        pin_placement[side].append(bterm)  # to maintain the order
-
-    unmatched_bterms = [bterm for bterm in bterms if bterm not in bterm_regex_map]
-
-    if len(unmatched_bterms) > 0:
-        print("Warning: Some pins weren't matched by the config file")
-        print("Those are:", [bterm.getName() for bterm in unmatched_bterms])
-        if unmatched_error_flag:
-            print("Treating unmatched pins as errors. Exiting..")
-            sys.exit(1)
-        else:
-            print("Assigning random sides to the above pins")
-            for bterm in unmatched_bterms:
-                random_side = random.choice(list(pin_placement.keys()))
-                pin_placement[random_side].append(bterm)
+                print(
+                    f"[WARNING] {name} not found in {not_in} but found in {is_in}.",
+                    file=sys.stderr,
+                )
+
+    if mismatches_found:
+        print("Critical mismatches found.")
+        exit(os.EX_DATAERR)
+
+    if len(not_in_config) > 0:
+        print("Assigning random sides to unmatched pins…")
+        for bterm in not_in_config:
+            random_side = random.choice(list(pin_placement.keys()))
+            pin_placement[random_side].append(bterm)
 
     # generate slots
-
     DIE_AREA = reader.block.getDieArea()
     BLOCK_LL_X = DIE_AREA.xMin()
     BLOCK_LL_Y = DIE_AREA.yMin()
     BLOCK_UR_X = DIE_AREA.xMax()
     BLOCK_UR_Y = DIE_AREA.yMax()
 
     print("Block boundaries:", BLOCK_LL_X, BLOCK_LL_Y, BLOCK_UR_X, BLOCK_UR_Y)
@@ -387,68 +402,80 @@
     print(f"Horizontal Tracks Origin: {origin}, Count: {count}, Step: {h_step}")
     h_tracks = grid_to_tracks(origin, count, h_step)
 
     origin, count, v_step = reader.block.findTrackGrid(V_LAYER).getGridPatternX(0)
     print(f"Vertical Tracks Origin: {origin}, Count: {count}, Step: {v_step}")
     v_tracks = grid_to_tracks(origin, count, v_step)
 
-    for rev in reverse_arr:
-        pin_placement[rev].reverse()
-
     pin_tracks = {}
     for side in pin_placement:
-        if side in ["#N", "#S"]:
+        if side in ["N", "S"]:
+            min_distance = info_by_side[side].min_distance * micron_in_units
             pin_tracks[side] = [
                 v_tracks[i]
                 for i in range(len(v_tracks))
-                if (i % (math.ceil(pin_distance[side] / v_step))) == 0
+                if (i % (math.ceil(min_distance / v_step))) == 0
             ]
-        elif side in ["#W", "#E"]:
+        elif side in ["W", "E"]:
             pin_tracks[side] = [
                 h_tracks[i]
                 for i in range(len(h_tracks))
-                if (i % (math.ceil(pin_distance[side] / h_step))) == 0
+                if (
+                    i
+                    % (
+                        math.ceil(
+                            info_by_side[side].min_distance * micron_in_units / h_step
+                        )
+                    )
+                )
+                == 0
             ]
 
+    # reversals (including randomly-assigned pins, if needed)
+    for side, side_info in info_by_side.items():
+        if side_info.reverse_result:
+            pin_placement[side].reverse()
+
     # create the pins
     for side in pin_placement:
         slots, pin_placement[side] = equally_spaced_sequence(
             side, pin_placement[side], pin_tracks[side]
         )
 
         assert len(slots) == len(pin_placement[side])
 
         for i in range(len(pin_placement[side])):
             bterm = pin_placement[side][i]
             slot = slots[i]
-            # print(f"Pin name: {bterm.getName()}, placed at slot: {slot}")
-
             pin_name = bterm.getName()
             pins = bterm.getBPins()
             if len(pins) > 0:
-                print(f"Warning: {pin_name} already has shapes. Modifying them")
+                print(
+                    f"[WARNING] {pin_name} already has shapes. The shapes will be modified.",
+                    file=sys.stderr,
+                )
                 assert len(pins) == 1
                 pin_bpin = pins[0]
             else:
                 pin_bpin = odb.dbBPin_create(bterm)
 
             pin_bpin.setPlacementStatus("PLACED")
 
-            if side in ["#N", "#S"]:
-                rect = odb.Rect(0, 0, V_WIDTH, LENGTH + V_EXTENSION)
-                if side == "#N":
-                    y = BLOCK_UR_Y - LENGTH
+            if side in ["N", "S"]:
+                rect = odb.Rect(0, 0, V_WIDTH, V_LENGTH + V_EXTENSION)
+                if side == "N":
+                    y = BLOCK_UR_Y - V_LENGTH
                 else:
                     y = BLOCK_LL_Y - V_EXTENSION
                 rect.moveTo(slot - V_WIDTH // 2, y)
                 odb.dbBox_create(pin_bpin, V_LAYER, *rect.ll(), *rect.ur())
             else:
-                rect = odb.Rect(0, 0, LENGTH + H_EXTENSION, H_WIDTH)
-                if side == "#E":
-                    x = BLOCK_UR_X - LENGTH
+                rect = odb.Rect(0, 0, H_LENGTH + H_EXTENSION, H_WIDTH)
+                if side == "E":
+                    x = BLOCK_UR_X - H_LENGTH
                 else:
                     x = BLOCK_LL_X - H_EXTENSION
                 rect.moveTo(x, slot - H_WIDTH // 2)
                 odb.dbBox_create(pin_bpin, H_LAYER, *rect.ll(), *rect.ur())
 
 
 if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/label_macro_pins.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/label_macro_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/lefutil.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/lefutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/manual_macro_place.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/manual_macro_place.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import sys
 from reader import click_odb, click
 
 LEF2OA_MAP = {
     "N": "R0",
     "S": "R180",
     "W": "R90",
     "E": "R270",
@@ -63,19 +64,23 @@
     with open(config, "r") as config_file:
         for line in config_file:
             # Discard comments and empty lines
             line = line.split("#")[0].strip()
             if not line:
                 continue
             line = line.split()
-            macros[line[0]] = [
-                str(int(float(line[1]) * db_units_per_micron)),
-                str(int(float(line[2]) * db_units_per_micron)),
-                line[3],
+            name, x, y, orientation = line
+            macro_data = [
+                name,
+                int(float(x) * db_units_per_micron),
+                int(float(y) * db_units_per_micron),
+                orientation,
             ]
+            name_escaped = reader.escape_verilog_name(name)
+            macros[name_escaped] = macro_data
 
     print("Placing the following macros:")
     print(macros)
 
     print("Design name:", reader.name)
 
     macros_cnt = len(macros)
@@ -83,24 +88,29 @@
         inst_name = inst.getName()
         if inst.isFixed():
             assert inst_name not in macros, inst_name
             continue
         if inst_name in macros:
             print("Placing", inst_name)
             macro_data = macros[inst_name]
-            x = gridify(int(macro_data[0]), 5)
-            y = gridify(int(macro_data[1]), 5)
-            inst.setOrient(lef_rot_to_oa_rot(macro_data[2]))
+            _, x, y, orientation = macro_data
+            x = gridify(x, 5)
+            y = gridify(y, 5)
+            inst.setOrient(lef_rot_to_oa_rot(orientation))
             inst.setLocation(x, y)
             if fixed:
                 inst.setPlacementStatus("FIRM")
             else:
                 inst.setPlacementStatus("PLACED")
             del macros[inst_name]
 
-    assert not macros, ("Macros not found:", macros)
+    if len(macros):
+        print("Declared macros not instantiated in design:", file=sys.stderr)
+        for macro in macros.values():
+            print(f"* {macro[0]}", file=sys.stderr)
+        exit(1)
 
     print(f"Successfully placed {macros_cnt} instances.")
 
 
 if __name__ == "__main__":
     manual_macro_place()
```

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/random_place.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/random_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/remove_buffers.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/remove_buffers.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/snap_to_grid.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/snap_to_grid.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/odbpy/wire_lengths.py` & `openlane-2.0.0rc2/openlane/scripts/odbpy/wire_lengths.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/basic_mp.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/basic_mp.tcl`

 * *Files 14% similar despite different names*

```diff
@@ -15,7 +15,10 @@
 read_current_odb
 
 macro_placement\
     -channel $::env(PL_MACRO_CHANNEL)\
     -halo $::env(PL_MACRO_HALO)
 
 write_views
+
+report_design_area_metrics
+
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/check_antennas.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/antenna_check.tcl`

 * *Files 17% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
 read_current_odb
 
 # start checking antennas and generate a detailed report
-puts "%OL_CREATE_REPORT antenna.rpt"
+puts "%OL_CREATE_REPORT $::env(_ANTENNA_REPORT)"
 check_antennas -verbose
-puts "%OL_END_REPORT"
+puts "%OL_END_REPORT"
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/common/dpl.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/cut_rows.tcl`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# Copyright 2022 Efabless Corporation
+# Copyright 2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-source $::env(SCRIPTS_DIR)/openroad/common/dpl_cell_pad.tcl
+source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
+read_current_odb
 
-remove_fillers
+cut_rows\
+    -endcap_master $::env(ENDCAP_CELL)\
+    -halo_width_x $::env(FP_MACRO_HORIZONTAL_HALO)\
+    -halo_width_y $::env(FP_MACRO_VERTICAL_HALO)
 
-detailed_placement\
-    -max_displacement [subst { $::env(PL_MAX_DISPLACEMENT_X) $::env(PL_MAX_DISPLACEMENT_Y) }]
+write_views
 
-if { [info exists ::env(PL_OPTIMIZE_MIRRORING)] && $::env(PL_OPTIMIZE_MIRRORING) } {
-    optimize_mirroring
-}
+report_design_area_metrics
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/common/dpl_cell_pad.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/dpl_cell_pad.tcl`

 * *Files 21% similar despite different names*

```diff
@@ -13,10 +13,14 @@
 # limitations under the License.
 set cell_pad_value $::env(DPL_CELL_PADDING)
 
 set cell_pad_side [expr $cell_pad_value / 2]
 
 set_placement_padding -global -right $cell_pad_side -left $cell_pad_side
 
-if { $::env(CELL_PAD_EXCLUDE) != "" } {
-    set_placement_padding -masters $::env(CELL_PAD_EXCLUDE) -right 0 -left 0
+foreach wildcard $::env(CELL_PAD_EXCLUDE) {
+    set_placement_padding -masters $wildcard -right 0 -left 0
+}
+if { [info exists ::env(DIODE_PADDING)] && $::env(DIODE_PADDING) } {
+    set diode_split [split $::env(DIODE_CELL) "/"]
+    set_placement_padding -masters [lindex $diode_split 0] -left $::env(DIODE_PADDING)
 }
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/common/io.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/io.tcl`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+source $::env(_TCL_ENV_IN)
 source $::env(SCRIPTS_DIR)/openroad/common/set_global_connections.tcl
 
 proc string_in_file {file_path substring} {
     set f [open $file_path r]
     set data [read $f]
     close $f
 
@@ -26,92 +26,95 @@
 }
 
 proc env_var_used {file var} {
     return [string_in_file $file "\$::env($var)"]
 }
 
 proc read_current_sdc {} {
-    if { ![info exists ::env(CURRENT_SDC)]} {
-        puts "\[INFO] CURRENT_SDC not found. Not reading an SDC file."
+    if { ![info exists ::env(_SDC_IN)]} {
+        puts "\[INFO] _SDC_IN not found. Not reading an SDC file."
         return
     }
     set ::env(IO_PCT) [expr $::env(IO_DELAY_CONSTRAINT) / 100]
     set ::env(SYNTH_TIMING_DERATE) [expr $::env(TIME_DERATING_CONSTRAINT) / 100]
     set ::env(SYNTH_MAX_FANOUT) $::env(MAX_FANOUT_CONSTRAINT)
     set ::env(SYNTH_CLOCK_UNCERTAINTY) $::env(CLOCK_UNCERTAINTY_CONSTRAINT)
     set ::env(SYNTH_CLOCK_TRANSITION) $::env(CLOCK_TRANSITION_CONSTRAINT)
     set ::env(SYNTH_CAP_LOAD) $::env(OUTPUT_CAP_LOAD)
     if { [info exists ::env(MAX_TRANSITION_CONSTRAINT)] } {
         set ::env(SYNTH_MAX_TRAN) $::env(MAX_TRANSITION_CONSTRAINT)
     }
 
-    if { [env_var_used $::env(CURRENT_SDC) SYNTH_DRIVING_CELL_PIN] == 1 } {
+    if { [env_var_used $::env(_SDC_IN) SYNTH_DRIVING_CELL_PIN] == 1 } {
         set ::env(SYNTH_DRIVING_CELL_PIN) [lindex [split $::env(SYNTH_DRIVING_CELL) "/"] 1]
         set ::env(SYNTH_DRIVING_CELL) [lindex [split $::env(SYNTH_DRIVING_CELL) "/"] 0]
     }
 
-    puts "Reading design constraints file at '$::env(CURRENT_SDC)'…"
-    if {[catch {read_sdc $::env(CURRENT_SDC)} errmsg]} {
+    puts "Reading design constraints file at '$::env(_SDC_IN)'…"
+    if {[catch {read_sdc $::env(_SDC_IN)} errmsg]} {
         puts stderr $errmsg
         exit 1
     }
 }
 
 
 proc read_current_netlist {args} {
     sta::parse_key_args "read_current_netlist" args \
         keys {}\
-        flags {-powered -all}
+        flags {-powered}
 
-    puts "Reading top-level netlist at '$::env(CURRENT_NETLIST)'…"
-    if {[catch {read_verilog $::env(CURRENT_NETLIST)} errmsg]} {
-        puts stderr $errmsg
-        exit 1
+    if { [info exists flags(-powered)] } {
+        puts "Reading top-level powered netlist at '$::env(CURRENT_POWERED_NETLIST)'…"
+        if {[catch {read_verilog $::env(CURRENT_POWERED_NETLIST)} errmsg]} {
+            puts stderr $errmsg
+            exit 1
+        }
+    } else {
+        puts "Reading top-level netlist at '$::env(CURRENT_NETLIST)'…"
+        if {[catch {read_verilog $::env(CURRENT_NETLIST)} errmsg]} {
+            puts stderr $errmsg
+            exit 1
+        }
     }
 
     puts "Linking design '$::env(DESIGN_NAME)' from netlist…"
     link_design $::env(DESIGN_NAME)
 
     read_current_sdc
 
 }
 
 proc read_timing_info {args} {
-    if { ![info exists ::env(CURRENT_CORNER_NAME)] } {
+    sta::parse_key_args "read_timing_info" args \
+        keys {}\
+        flags {-powered}
+
+    if { ![info exists ::env(_CURRENT_CORNER_NAME)] } {
         return
     }
-    set corner_name $::env(CURRENT_CORNER_NAME)
+    set corner_name $::env(_CURRENT_CORNER_NAME)
     define_corners $corner_name
 
     puts "Reading timing models for corner $corner_name…"
 
-    set macro_spefs [list]
-    set macro_nls [list]
-    set corner_models $::env(CURRENT_CORNER_TIMING_VIEWS)
-    foreach model $corner_models {
-        if { [string match *.spef $model]} {
-            lappend macro_spefs $corner_name $model
-        } elseif { [string match *.v $model] } {
-            lappend macro_nls $model
-        } else {
-            puts "Reading timing library for the '$corner_name' corner at '$model'…"
-            read_liberty -corner $corner_name $model
-        }
+    foreach lib $::env(_CURRENT_CORNER_LIBS) {
+        puts "Reading cell library for the '$corner_name' corner at '$lib'…"
+        read_liberty -corner $corner_name $lib
     }
 
     if { [info exists ::env(EXTRA_LIBS) ] } {
         puts "Reading explicitly-specified extra libs for $corner_name…"
         foreach extra_lib $::env(EXTRA_LIBS) {
             puts "Reading extra timing library for the '$corner_name' corner at '$extra_lib'…"
             read_liberty -corner $corner_name $extra_lib
         }
     }
 
     set blackbox_wildcard {/// sta-blackbox}
-    foreach nl $macro_nls {
+    foreach nl $::env(_CURRENT_CORNER_NETLISTS) {
         puts "Reading macro netlist at '$nl'…"
         if { [catch {read_verilog $nl} err] } {
             puts "Error while reading macro netlist '$nl':"
             puts $err
             puts "Make sure that this a gate-level netlist and not an RTL file."
             exit 1
         }
@@ -124,53 +127,79 @@
                 puts "Error while reading $verilog_file:"
                 puts $err
                 puts "Make sure that this a gate-level netlist and not an RTL file, otherwise, you can add the following comment '$blackbox_wildcard' in the file to skip it and blackbox the modules inside if needed."
                 exit 1
             }
         }
     }
-    read_current_netlist
-    set ::macro_spefs $macro_spefs
+    if { [info exists flags(-powered)] } {
+        read_current_netlist -powered
+    } else {
+        read_current_netlist
+    }
+}
+
+proc lshift {inputlist} {
+    upvar $inputlist argv
+    set arg  [lindex $argv 0]
+    #set argv [lrange $argv 1 end] ;# below is much faster - lreplace can make use of unshared Tcl_Obj to avoid alloc'ing the result
+    set argv [lreplace $argv[set argv {}] 0 0]
+    return $arg
 }
 
 proc read_spefs {} {
-    if { [info exists ::env(CURRENT_SPEF_BY_CORNER)] } {
-        foreach {corner_name spef} $::env(CURRENT_SPEF_BY_CORNER) {
-            puts "Reading top-level design parasitics for the '$corner_name' corner at '$spef'…"
-            read_spef -corner $corner_name $spef
+    if { [info exists ::env(_CURRENT_SPEF_BY_CORNER)] } {
+        set corner_name $::env(_CURRENT_CORNER_NAME)
+        puts "Reading top-level design parasitics for the '$corner_name' corner at '$::env(_CURRENT_SPEF_BY_CORNER)'…"
+        read_spef -corner $corner_name $::env(_CURRENT_SPEF_BY_CORNER)
+    }
+    if { [info exists ::env(_CURRENT_CORNER_SPEFS)] } {
+        set corner_name $::env(_CURRENT_CORNER_NAME)
+        foreach spefs $::env(_CURRENT_CORNER_SPEFS) {
+            set instance_path [lshift spefs]
+            foreach spef $spefs {
+                puts "Reading '$instance_path' parasitics for the '$corner_name' corner at '$spef'…"
+                read_spef -corner $corner_name -path $instance_path $spef
+            }
         }
     }
-    if { [info exists ::macro_spefs] } {
-        foreach {corner_name spef_info} $::macro_spefs {
-            set fields [split $spef_info "@"]
-            lassign $fields instance_path spef
-            puts "Reading '$instance_path' parasitics for the '$corner_name' corner at '$spef'…"
-            read_spef -corner $corner_name -path $instance_path $spef
+    if { [info exists ::env(_CURRENT_CORNER_EXTRA_SPEFS_BACKCOMPAT)] } {
+        set corner_name $::env(_CURRENT_CORNER_NAME)
+        foreach pair $::env(_CURRENT_CORNER_EXTRA_SPEFS_BACKCOMPAT) {
+            set module_name [lindex $pair 0]
+            set spef [lindex $pair 1]
+            foreach cell [get_cells * -hierarchical] {
+                if { "[get_property $cell ref_name]" eq "$module_name"} {
+                    set instance_path [get_property $cell full_name]
+                    puts "Reading '$instance_path' parasitics for the '$corner_name' corner at '$spef'…"
+                    read_spef -corner $corner_name -path $instance_path $spef
+                }
+            }
         }
     }
 }
 
 proc read_pnr_libs {args} {
-    # PNR_LIBS contains all libs and extra libs but with known-bad cells
+    # _PNR_LIBS contains all libs and extra libs but with known-bad cells
     # excluded, so OpenROAD can use cells by functionality and come up
     # with a valid design.
 
     # If there are ANY libs already read- just leave
     if { [get_libs -quiet *] != {} } {
         return
     }
 
     define_corners $::env(DEFAULT_CORNER)
 
-    foreach lib $::env(PNR_LIBS) {
+    foreach lib $::env(_PNR_LIBS) {
         puts "Reading library file at '$lib'…"
         read_liberty $lib
     }
-    if { [info exists ::env(MACRO_LIBS) ] } {
-        foreach macro_lib $::env(MACRO_LIBS) {
+    if { [info exists ::env(_MACRO_LIBS) ] } {
+        foreach macro_lib $::env(_MACRO_LIBS) {
             puts "Reading macro library file at '$macro_lib'…"
             read_liberty $macro_lib
         }
     }
     if { [info exists ::env(EXTRA_LIBS) ] } {
         foreach extra_lib $::env(EXTRA_LIBS) {
             puts "Reading extra library file at '$extra_lib'…"
@@ -199,28 +228,33 @@
         foreach lef $::env(EXTRA_LEFS) {
             puts "Reading extra LEF file at '$lef'…"
             read_lef $lef
         }
     }
 }
 
+proc set_dont_use_cells {} {
+    set_dont_use $::env(_PNR_EXCLUDED_CELLS)
+}
+
 proc read_current_odb {args} {
     sta::parse_key_args "read_current_odb" args \
         keys {}\
         flags {}
 
     puts "Reading OpenROAD database at '$::env(CURRENT_ODB)'…"
     if { [ catch {read_db $::env(CURRENT_ODB)} errmsg ]} {
         puts stderr $errmsg
         exit 1
     }
 
     # Read supporting views (if applicable)
     read_pnr_libs
     read_current_sdc
+    set_dont_use_cells
 }
 
 proc write_views {args} {
     # This script will attempt to write views based on existing "SAVE_"
     # environment variables. If the SAVE_ variable exists, the script will
     # attempt to write a corresponding view to the specified location.
     sta::parse_key_args "write_views" args \
@@ -243,14 +277,37 @@
     }
 
     if { [info exists ::env(SAVE_POWERED_NETLIST)] } {
         puts "Writing powered netlist to '$::env(SAVE_POWERED_NETLIST)'…"
         write_verilog -include_pwr_gnd $::env(SAVE_POWERED_NETLIST)
     }
 
+    if { [info exists ::env(SAVE_POWERED_NETLIST_SDF_FRIENDLY)] } {
+        set exclude_cells "[join $::env(FILL_CELL)] [join $::env(DECAP_CELL)] [join $::env(WELLTAP_CELL)] [join $::env(ENDCAP_CELL)]"
+        puts "Writing nofill powered netlist to '$::env(SAVE_POWERED_NETLIST_SDF_FRIENDLY)'…"
+        puts "Excluding $exclude_cells"
+        write_verilog -include_pwr_gnd \
+            -remove_cells "$exclude_cells"\
+            $::env(SAVE_POWERED_NETLIST_SDF_FRIENDLY)
+    }
+
+    if { [info exists ::env(SAVE_POWERED_NETLIST_NO_PHYSICAL_CELLS)] } {
+        set exclude_cells "[join [lindex [split $::env(DIODE_CELL) "/"] 0]] [join $::env(FILL_CELL)] [join $::env(DECAP_CELL)] [join $::env(WELLTAP_CELL)] [join $::env(ENDCAP_CELL)]"
+        puts "Writing nofilldiode powered netlist to '$::env(SAVE_POWERED_NETLIST_NO_PHYSICAL_CELLS)'…"
+        puts "Excluding $exclude_cells"
+        write_verilog -include_pwr_gnd \
+            -remove_cells "$exclude_cells"\
+            $::env(SAVE_POWERED_NETLIST_NO_PHYSICAL_CELLS)
+    }
+
+    if { [info exists ::env(SAVE_OPENROAD_LEF)] } {
+        puts "Writing LEF to '$::env(SAVE_OPENROAD_LEF)'…"
+        write_abstract_lef $::env(SAVE_OPENROAD_LEF)
+    }
+
     if { [info exists ::env(SAVE_DEF)] } {
         puts "Writing layout to '$::env(SAVE_DEF)'…"
         write_def $::env(SAVE_DEF)
     }
 
     if { [info exists ::env(SAVE_SDC)] } {
         puts "Writing timing constraints to '$::env(SAVE_SDC)'…"
@@ -274,33 +331,37 @@
             puts "Writing SDF to '$::env(SAVE_SDF)'…"
             write_sdf -include_typ -divider . $::env(SAVE_SDF)
         }
     }
 }
 
 proc write_sdfs {} {
-    if { [info exists ::env(SDF_SAVE_DIR)] } {
+    if { [info exists ::env(_SDF_SAVE_DIR)] } {
         set corners [sta::corners]
 
         puts "Writing SDF files for all corners…"
         foreach corner $corners {
             set corner_name [$corner name]
-            set target $::env(SDF_SAVE_DIR)/$::env(DESIGN_NAME)__$corner_name.sdf
+            set target $::env(_SDF_SAVE_DIR)/$::env(DESIGN_NAME)__$corner_name.sdf
             write_sdf -include_typ -divider . -corner $corner_name $target
         }
     }
 }
 
 proc write_libs {} {
-    if { [info exists ::env(LIB_SAVE_DIR)] && (![info exists ::(STA_PRE_CTS)] || !$::env(STA_PRE_CTS))} {
+    if { [info exists ::env(_LIB_SAVE_DIR)] } {
+        puts "Removing Clock latencies before writing libs…"
+        # This is to avoid OpenSTA writing a context-dependent timing model
+        set_clock_latency -source -max 0 [all_clocks]
+        set_clock_latency -source -min 0 [all_clocks]
         set corners [sta::corners]
         puts "Writing timing models for all corners…"
         foreach corner $corners {
             set corner_name [$corner name]
-            set target $::env(LIB_SAVE_DIR)/$::env(DESIGN_NAME)__$corner_name.lib
+            set target $::env(_LIB_SAVE_DIR)/$::env(DESIGN_NAME)__$corner_name.lib
             puts "Writing timing models for the $corner_name corner to $target…"
             write_timing_model -corner $corner_name $target
         }
     }
 }
 
 proc max {a b} {
@@ -309,23 +370,22 @@
     } else {
         return $b
     }
 }
 
 set ::metric_count 0
 set ::metrics_file ""
-if { [info exists ::env(OPENSTA)] && $::env(OPENSTA) } {
+if { [info exists ::env(_OPENSTA)] && $::env(_OPENSTA) } {
     proc write_metric_num {metric value} {
         if { $value == 1e30 } {
-            write_metric_str $metric Infinity
+            set value inf
         } elseif { $value == -1e30 } {
-            write_metric_str $metric -Infinity
-        } else {
-            puts "%OL_METRIC_F $metric $value"
+            set value -inf
         }
+        puts "%OL_METRIC_F $metric $value"
     }
     proc write_metric_int {metric value} {
         puts "%OL_METRIC_I $metric $value"
     }
     proc write_metric_str {metric value} {
         puts "%OL_METRIC $metric $value"
     }
@@ -338,8 +398,8 @@
         puts "Writing metric $metric: $value"
         utl::metric_int $metric $value
     }
     proc write_metric_num {metric value} {
         puts "Writing metric $metric: $value"
         utl::metric_float $metric $value
     }
-}
+}
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/common/pdn_cfg.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/pdn_cfg.tcl`

 * *Files 17% similar despite different names*

```diff
@@ -39,18 +39,15 @@
         }
     }
 }
 
 set_voltage_domain -name CORE -power $::env(VDD_NET) -ground $::env(GND_NET) \
     -secondary_power $secondary
 
-# Assesses whether the design is the core of the chip or not based on the
-# value of $::env(DESIGN_IS_CORE) and uses the appropriate stdcell section
-if { $::env(DESIGN_IS_CORE) == 1 } {
-    # Used if the design is the core of the chip
+if { $::env(FP_PDN_MULTILAYER) == 1 } {
     define_pdn_grid \
         -name stdcell_grid \
         -starts_with POWER \
         -voltage_domain CORE \
         -pins "$::env(FP_PDN_VERTICAL_LAYER) $::env(FP_PDN_HORIZONTAL_LAYER)"
 
     add_pdn_stripe \
@@ -71,28 +68,28 @@
         -spacing $::env(FP_PDN_HSPACING) \
         -starts_with POWER -extend_to_core_ring
 
     add_pdn_connect \
         -grid stdcell_grid \
         -layers "$::env(FP_PDN_VERTICAL_LAYER) $::env(FP_PDN_HORIZONTAL_LAYER)"
 } else {
-    # Used if the design is a macro in the core
     define_pdn_grid \
         -name stdcell_grid \
         -starts_with POWER \
         -voltage_domain CORE \
         -pins $::env(FP_PDN_VERTICAL_LAYER)
 
     add_pdn_stripe \
         -grid stdcell_grid \
         -layer $::env(FP_PDN_VERTICAL_LAYER) \
         -width $::env(FP_PDN_VWIDTH) \
         -pitch $::env(FP_PDN_VPITCH) \
         -offset $::env(FP_PDN_VOFFSET) \
-        -starts_with POWER
+        -spacing $::env(FP_PDN_VSPACING) \
+        -starts_with POWER -extend_to_core_ring
 }
 
 # Adds the standard cell rails if enabled.
 if { $::env(FP_PDN_ENABLE_RAILS) == 1 } {
     add_pdn_stripe \
         -grid stdcell_grid \
         -layer $::env(FP_PDN_RAIL_LAYER) \
@@ -104,20 +101,30 @@
         -grid stdcell_grid \
         -layers "$::env(FP_PDN_RAIL_LAYER) $::env(FP_PDN_VERTICAL_LAYER)"
 }
 
 
 # Adds the core ring if enabled.
 if { $::env(FP_PDN_CORE_RING) == 1 } {
-    add_pdn_ring \
-        -grid stdcell_grid \
-        -layers "$::env(FP_PDN_VERTICAL_LAYER) $::env(FP_PDN_HORIZONTAL_LAYER)" \
-        -widths "$::env(FP_PDN_CORE_RING_VWIDTH) $::env(FP_PDN_CORE_RING_HWIDTH)" \
-        -spacings "$::env(FP_PDN_CORE_RING_VSPACING) $::env(FP_PDN_CORE_RING_HSPACING)" \
-        -core_offset "$::env(FP_PDN_CORE_RING_VOFFSET) $::env(FP_PDN_CORE_RING_HOFFSET)"
+    if { $::env(FP_PDN_MULTILAYER) == 1 } {
+        add_pdn_ring \
+            -grid stdcell_grid \
+            -layers "$::env(FP_PDN_VERTICAL_LAYER) $::env(FP_PDN_HORIZONTAL_LAYER)" \
+            -widths "$::env(FP_PDN_CORE_RING_VWIDTH) $::env(FP_PDN_CORE_RING_HWIDTH)" \
+            -spacings "$::env(FP_PDN_CORE_RING_VSPACING) $::env(FP_PDN_CORE_RING_HSPACING)" \
+            -core_offset "$::env(FP_PDN_CORE_RING_VOFFSET) $::env(FP_PDN_CORE_RING_HOFFSET)"
+    } else {
+        throw APPLICATION "FP_PDN_CORE_RING cannot be used when FP_PDN_MULTILAYER is set to false."
+        # add_pdn_ring \
+        #     -grid stdcell_grid \
+        #     -layers "$::env(FP_PDN_VERTICAL_LAYER)" \
+        #     -widths "$::env(FP_PDN_CORE_RING_VWIDTH)" \
+        #     -spacings "$::env(FP_PDN_CORE_RING_VSPACING)" \
+        #     -core_offset "$::env(FP_PDN_CORE_RING_VOFFSET)"
+    }
 }
 
 define_pdn_grid \
     -macro \
     -default \
     -name macro \
     -starts_with POWER \
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/common/resizer.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/resizer.tcl`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         set corner($corner_name) $corner_libs
 
         incr i
         set tc_key "RSZ_CORNER_$i"
     }
 
     if { $i == "0" } {
-        puts "\[WARN] No resizer-specific timing information read."
+        puts stderr "\[WARNING] No resizer-specific timing information read."
         return
     }
 
     define_corners {*}[array name corner]
 
     foreach corner_name [array name corner] {
         puts "Reading timing models for corner $corner_name…"
@@ -101,15 +101,7 @@
         }
     }
 
     if { [info exists ::env(RSZ_DONT_TOUCH_LIST)] } {
         unset_dont_touch $::env(RSZ_DONT_TOUCH_LIST)
     }
 }
-
-
-proc set_dont_use_cells {} {
-    set_dont_use $::env(PNR_EXCLUDED_CELLS)
-    if { [info exists ::env(RSZ_DONT_USE_CELLS)] } {
-        set_dont_use $::env(RSZ_DONT_USE_CELLS)
-    }
-}
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/common/set_layer_adjustments.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_layer_adjustments.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/common/set_rc.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_rc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/common/set_routing_layers.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_routing_layers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/cts.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/cts.tcl`

 * *Files 15% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 
 # Clone clock tree inverters next to register loads
 # so cts does not try to buffer the inverted clocks.
 repair_clock_inverters
 
 puts "\[INFO\] Configuring cts characterization…"
 set cts_characterization_args [list]
-lappend -max_cap [expr {$::env(CTS_MAX_CAP) * 1e-12}]; # pF -> F
-if { [info exists ::env(MAX_FANOUT_CONSTRAINT)] } {
-    lappend -max_slew [expr {$::env(MAX_FANOUT_CONSTRAINT) * 1e-9}]; # ns -> S
+if { [info exists ::env(CTS_MAX_CAP)] } {
+    lappend cts_characterization_args -max_cap [expr {$::env(CTS_MAX_CAP) * 1e-12}]; # pF -> F
+}
+if { [info exists ::env(CTS_MAX_SLEW)] } {
+    lappend cts_characterization_args -max_slew [expr {$::env(CTS_MAX_SLEW) * 1e-9}]; # ns -> S
 }
 configure_cts_characterization {*}$cts_characterization_args
 
 puts "\[INFO] Performing clock tree synthesis…"
 puts "\[INFO] Looking for the following net(s): $::env(CLOCK_NET)"
 puts "\[INFO] Running Clock Tree Synthesis…"
 
@@ -68,15 +70,13 @@
 puts "\[INFO\] Legalizing…"
 source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
 
 estimate_parasitics -placement
 
 write_views
 
-if { [catch {check_placement -verbose} errmsg] } {
-    puts stderr $errmsg
-    exit 1
-}
-
 puts "%OL_CREATE_REPORT cts.rpt"
 report_cts
 puts "%OL_END_REPORT"
+
+report_design_area_metrics
+
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/dpl.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/grt.tcl`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-# Copyright 2020-2022 Efabless Corporation
+# Copyright 2020-2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
 read_current_odb
+source $::env(SCRIPTS_DIR)/openroad/common/dpl_cell_pad.tcl
 
-source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
+set_propagated_clock [all_clocks]
 
-if { [catch {check_placement -verbose} errmsg] } {
-    puts stderr $errmsg
-    exit 1
-}
+source $::env(SCRIPTS_DIR)/openroad/common/grt.tcl
 
-write_views
+# Check Antennas (Pre-Repair)
+puts "%OL_CREATE_REPORT antenna.rpt"
+check_antennas -verbose
+puts "%OL_END_REPORT"
+
+source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
+estimate_parasitics -global_routing
+
+write_views
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/drt.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/drt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/fill.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/fill.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/floorplan.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/floorplan.tcl`

 * *Files 21% similar despite different names*

```diff
@@ -12,24 +12,55 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
 read_pnr_libs
 read_lefs
 read_current_netlist
 
+set ::db [::ord::get_db]
+set ::chip [$::db getChip]
+set ::tech [$::db getTech]
+set ::block [$::chip getBlock]
+set ::dbu [$::tech getDbUnitsPerMicron]
+set ::libs [$::db getLibs]
+
+foreach lib $::libs {
+    set current_sites [$lib getSites]
+    foreach site $current_sites {
+        set name [$site getName]
+        set ::sites($name) $site
+    }
+}
+
+set ::default_site $::sites($::env(PLACE_SITE))
+
+set ::default_site_height [expr [$::default_site getHeight] / double($::dbu)]
+set ::default_site_width [expr [$::default_site getWidth] / double($::dbu)]
+
+puts "Using site height: $::default_site_height and site width: $::default_site_width…"
+
 unset_propagated_clock [all_clocks]
 
-set bottom_margin  [expr $::env(PLACE_SITE_HEIGHT) * $::env(BOTTOM_MARGIN_MULT)]
-set top_margin  [expr $::env(PLACE_SITE_HEIGHT) * $::env(TOP_MARGIN_MULT)]
-set left_margin [expr $::env(PLACE_SITE_WIDTH) * $::env(LEFT_MARGIN_MULT)]
-set right_margin [expr $::env(PLACE_SITE_WIDTH) * $::env(RIGHT_MARGIN_MULT)]
+set bottom_margin  [expr $::default_site_height * $::env(BOTTOM_MARGIN_MULT)]
+set top_margin  [expr $::default_site_height * $::env(TOP_MARGIN_MULT)]
+set left_margin [expr $::default_site_width * $::env(LEFT_MARGIN_MULT)]
+set right_margin [expr $::default_site_width * $::env(RIGHT_MARGIN_MULT)]
 
 set arg_list [list]
+
 lappend arg_list -site $::env(PLACE_SITE)
 
+if { [info exists ::env(EXTRA_SITES)] } {
+    foreach site $::env(EXTRA_SITES) {
+        lappend arg_list -additional_sites $site
+    }
+}
+
+puts "\[INFO] Using $::env(FP_SIZING) sizing for the floorplan."
+
 if {$::env(FP_SIZING) == "absolute"} {
     if { [llength $::env(DIE_AREA)] != 4 } {
         puts stderr "Invalid die area string '$::env(DIE_AREA)'."
         exit -1
     }
     if { ! [info exists ::env(CORE_AREA)] } {
         set die_ll_x [lindex $::env(DIE_AREA) 0]
@@ -49,50 +80,54 @@
             exit -1
         }
         puts "\[INFO] Using the set CORE_AREA; ignoring core margin parameters"
     }
 
     lappend arg_list -die_area $::env(DIE_AREA)
     lappend arg_list -core_area $::env(CORE_AREA)
-    lappend arg_list -site $::env(PLACE_SITE)
-} else {
+} elseif { $::env(FP_SIZING) == "relative" } {
     lappend arg_list -utilization $::env(FP_CORE_UTIL)
     lappend arg_list -aspect_ratio $::env(FP_ASPECT_RATIO)
     lappend arg_list -core_space "$bottom_margin $top_margin $left_margin $right_margin"
 }
 
+if { [info exists ::env(FP_OBSTRUCTIONS)] } {
+    foreach obstruction $::env(FP_OBSTRUCTIONS) {
+        set llx [expr int([expr [lindex $obstruction 0] * $::dbu])]
+        set lly [expr int([expr [lindex $obstruction 1] * $::dbu])]
+        set urx [expr int([expr [lindex $obstruction 2] * $::dbu])]
+        set ury [expr int([expr [lindex $obstruction 3] * $::dbu])]
+        odb::dbBlockage_create [ord::get_db_block] $llx $lly $urx $ury
+        puts "\[INFO] Created obstruction at $::env(FP_OBSTRUCTIONS) (µm)"
+    }
+}
+
 initialize_floorplan {*}$arg_list
 
 insert_tiecells $::env(SYNTH_TIELO_CELL) -prefix "TIE_ZERO_"
 insert_tiecells $::env(SYNTH_TIEHI_CELL) -prefix "TIE_ONE_"
 
-set ::chip [[::ord::get_db] getChip]
-set ::tech [[::ord::get_db] getTech]
-set ::block [$::chip getBlock]
-
 puts "\[INFO] Extracting DIE_AREA and CORE_AREA from the floorplan"
 set ::env(DIE_AREA) [list]
 set ::env(CORE_AREA) [list]
 
 set die_area [$::block getDieArea]
 set core_area [$::block getCoreArea]
 
 set die_area [list [$die_area xMin] [$die_area yMin] [$die_area xMax] [$die_area yMax]]
 set core_area [list [$core_area xMin] [$core_area yMin] [$core_area xMax] [$core_area yMax]]
 
-set dbu [$tech getDbUnitsPerMicron]
-
 set ::env(DIE_AREA) {}
 set ::env(CORE_AREA) {}
 
 foreach coord $die_area {
-    lappend ::env(DIE_AREA) [expr {1.0 * $coord / $dbu}]
+    lappend ::env(DIE_AREA) [expr {1.0 * $coord / $::dbu}]
 }
 foreach coord $core_area {
-    lappend ::env(CORE_AREA) [expr {1.0 * $coord / $dbu}]
+    lappend ::env(CORE_AREA) [expr {1.0 * $coord / $::dbu}]
 }
 
 puts "\[INFO] Floorplanned on a die area of $::env(DIE_AREA) (µm)."
 puts "\[INFO] Floorplanned on a core area of $::env(CORE_AREA) (µm)."
 
 source $::env(TRACKS_INFO_FILE_PROCESSED)
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/gui.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/write_views.tcl`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read_current_odb
+read_current_odb
+write_views
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/insert_buffer.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/insert_buffer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/ioplacer.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/ioplacer.tcl`

 * *Files 18% similar despite different names*

```diff
@@ -14,40 +14,54 @@
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
 read_current_odb
 
 if { [info exists ::env(CONTEXTUAL_IO_FLAG)] } {
 	read_lef $::env(placement_tmpfiles)/top_level.lef
 }
 
-if {$::env(FP_IO_HLENGTH) != "" && $::env(FP_IO_HLENGTH) != ""} {
-	set_pin_length -hor_length $::env(FP_IO_HLENGTH) \
-		-ver_length $::env(FP_IO_VLENGTH)
+if { [info exists ::env(FP_IO_HLENGTH)] } {
+	set_pin_length -hor_length $::env(FP_IO_HLENGTH)
 }
 
-if {$::env(FP_IO_HEXTEND) != "0" && $::env(FP_IO_VEXTEND) != "0"} {
-	set_pin_length_extension -hor_extension $::env(FP_IO_HEXTEND) \
-		-ver_extension $::env(FP_IO_VEXTEND)
+if { [info exists ::env(FP_IO_VLENGTH)] } {
+	set_pin_length -ver_length $::env(FP_IO_VLENGTH)
+}
+
+if { $::env(FP_IO_HEXTEND) != "0"} {
+	set_pin_length_extension -hor_extension $::env(FP_IO_HEXTEND)
+}
+
+if { $::env(FP_IO_VEXTEND) != "0"} {
+	set_pin_length_extension -ver_extension $::env(FP_IO_VEXTEND)
 }
 
 if {$::env(FP_IO_VTHICKNESS_MULT) != "" && $::env(FP_IO_HTHICKNESS_MULT) != ""} {
 	set_pin_thick_multiplier -hor_multiplier $::env(FP_IO_HTHICKNESS_MULT) \
 		-ver_multiplier $::env(FP_IO_VTHICKNESS_MULT)
 }
 
 set arg_list [list]
 if { $::env(FP_IO_MODE) == "random_equidistant" } {
 	lappend arg_list -random
 }
 
-if { $::env(FP_IO_MIN_DISTANCE) != "" } {
+if { [info exists ::env(FP_IO_MIN_DISTANCE)] } {
 	lappend arg_list -min_distance $::env(FP_IO_MIN_DISTANCE)
 }
 
+if { $::env(FP_IO_MODE) == "annealing" } {
+	lappend arg_list -annealing
+}
+
 set HMETAL $::env(FP_IO_HLAYER)
 set VMETAL $::env(FP_IO_VLAYER)
 
+puts "\[INFO] place_pins args: $arg_list"
 place_pins {*}$arg_list \
 	-random_seed 42 \
 	-hor_layers $HMETAL \
 	-ver_layers $VMETAL
 
 write_views
+
+report_design_area_metrics
+
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/irdrop.tcl` & `openlane-2.0.0rc2/openlane/scripts/yosys/json_header.tcl`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# Copyright 2022 Efabless Corporation
+# Copyright 2020-2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
+yosys -import
+source $::env(SCRIPTS_DIR)/yosys/common.tcl
+set vtop $::env(DESIGN_NAME)
 
-read_current_odb
+source $::env(_DEPS_SCRIPT)
 
-source $::env(SCRIPTS_DIR)/openroad/common/set_power_nets.tcl
-source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
-
-read_spef $::env(CURRENT_SPEF_DEFAULT_CORNER)
-
-puts "%OL_CREATE_REPORT irdrop.rpt"
-analyze_power_grid -net $::env(VDD_NET) -outfile $::env(STEP_DIR)/voltages.csv
-puts "%OL_END_REPORT"
+read_verilog_files $vtop
+hierarchy -check -top $vtop
+yosys rename -top $vtop
+yosys proc
+json -o $::env(SAVE_JSON_HEADER)
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/pdn.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/pdn.tcl`

 * *Files 21% similar despite different names*

```diff
@@ -11,37 +11,44 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
 read_current_odb
 
-if {![info exists ::env(PDN_CFG)]} {
-    set ::env(PDN_CFG) $::env(SCRIPTS_DIR)/openroad/common/pdn_cfg.tcl
-}
-
 source $::env(SCRIPTS_DIR)/openroad/common/set_power_nets.tcl
 
 # load the grid definitions
-if {[catch {source $::env(PDN_CFG)} errmsg]} {
+if {[catch {source $::env(FP_PDN_CFG)} errmsg]} {
     puts stderr $errmsg
     exit 1
 }
 set arg_list [list]
 if { $::env(FP_PDN_SKIPTRIM) } {
     lappend arg_list -skip_trim
     puts "adding -skip_trim to pdngen"
 }
 # run PDNGEN
 if {[catch {pdngen {*}$arg_list} errmsg]} {
     puts stderr $errmsg
     exit 1
 }
 
-# https://github.com/The-OpenROAD-Project/OpenROAD/issues/2126
-# checks for unconnected nodes (e.g., isolated rails or stripes)
-if { $::env(FP_PDN_CHECK_NODES) } {
-    check_power_grid -net $::env(VDD_NET)
-    check_power_grid -net $::env(GND_NET)
-}
-
 write_views
+report_design_area_metrics
+
+foreach {net} "$::env(VDD_NETS) $::env(GND_NETS)" {
+    set report_file $::env(STEP_DIR)/$net-grid-errors.rpt
+
+    # For some reason, check_power_grid is… totally okay if no nodes are found
+    # at all. i.e. PDN generation has completely failed.
+    # This is a fallback file.
+    set f [open $report_file "w"]
+    puts $f "violation type: no nodes"
+    puts $f "  srcs: "
+    puts $f "  - N/A"
+    close $f
+
+    if { [catch {check_power_grid -net $net -error_file $report_file} err] } {
+        puts stderr "\[WARNING\] Grid check for $net failed: $err"
+    }
+}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/rcx.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/rcx.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/repair_design.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/repair_design.tcl`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 load_rsz_corners
 read_current_odb
 
 unset_propagated_clock [all_clocks]
 
 set_dont_touch_objects
-set_dont_use_cells
 
 # set rc values
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 
 # CTS and detailed placement move instances, so update parastic estimates.
 # estimate wire rc parasitics
 estimate_parasitics -placement
@@ -53,18 +52,16 @@
 }
 
 report_floating_nets -verbose
 
 # Legalize
 source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
 
-if { [catch {check_placement -verbose} errmsg] } {
-    puts stderr $errmsg
-    exit 1
-}
-
 unset_dont_touch_objects
 
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 estimate_parasitics -placement
 
 write_views
+
+report_design_area_metrics
+
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/rsz_timing_postcts.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/rsz_timing_postcts.tcl`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 load_rsz_corners
 read_current_odb
 
 set_propagated_clock [all_clocks]
 
 set_dont_touch_objects
-set_dont_use_cells
 
 # set rc values
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 
 # CTS and detailed placement move instances, so update parastic estimates.
 # estimate wire rc parasitics
 estimate_parasitics -placement
@@ -38,23 +37,24 @@
 lappend arg_list -hold
 lappend arg_list -setup_margin $::env(PL_RESIZER_SETUP_SLACK_MARGIN)
 lappend arg_list -hold_margin $::env(PL_RESIZER_HOLD_SLACK_MARGIN)
 lappend arg_list -max_buffer_percent $::env(PL_RESIZER_HOLD_MAX_BUFFER_PCT)
 if { $::env(PL_RESIZER_ALLOW_SETUP_VIOS) == 1 } {
     lappend arg_list -allow_setup_violations
 }
+if { $::env(PL_RESIZER_GATE_CLONING) != 1 } {
+    lappend arg_list -skip_gate_cloning
+}
 repair_timing {*}$arg_list
 
 # Legalize
 source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
 
-if { [catch {check_placement -verbose} errmsg] } {
-    puts stderr $errmsg
-    exit 1
-}
-
 unset_dont_touch_objects
 
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 estimate_parasitics -placement
 
-write_views
+write_views
+
+report_design_area_metrics
+
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/rsz_timing_postgrt.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/rsz_timing_postgrt.tcl`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 load_rsz_corners
 read_current_odb
 
 set_propagated_clock [all_clocks]
 
 set_dont_touch_objects
-set_dont_use_cells
 
 # set rc values
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 
 # (Re-)GRT and Estimate Parasitics
 source $::env(SCRIPTS_DIR)/openroad/common/grt.tcl
 estimate_parasitics -global_routing
@@ -38,19 +37,21 @@
 lappend arg_list -hold
 lappend arg_list -setup_margin $::env(GRT_RESIZER_SETUP_SLACK_MARGIN)
 lappend arg_list -hold_margin $::env(GRT_RESIZER_HOLD_SLACK_MARGIN)
 lappend arg_list -max_buffer_percent $::env(GRT_RESIZER_HOLD_MAX_BUFFER_PCT)
 if { $::env(GRT_RESIZER_ALLOW_SETUP_VIOS) == 1 } {
     lappend arg_list -allow_setup_violations
 }
+if { $::env(GRT_RESIZER_GATE_CLONING) != 1 } {
+    lappend arg_list -skip_gate_cloning
+}
 repair_timing {*}$arg_list
 
 # Re-DPL and GRT
 source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
-if { [catch {check_placement -verbose} errmsg] } {
-    puts stderr $errmsg
-    exit 1
-}
 unset_dont_touch_objects
 source $::env(SCRIPTS_DIR)/openroad/common/grt.tcl
 
-write_views
+write_views
+
+report_design_area_metrics
+
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/tapcell.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/tapcell.tcl`

 * *Files 10% similar despite different names*

```diff
@@ -12,13 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
 read_current_odb
 
 tapcell\
     -distance $::env(FP_TAPCELL_DIST)\
-    -tapcell_master "$::env(FP_WELLTAP_CELL)"\
-    -endcap_master "$::env(FP_ENDCAP_CELL)"\
-    -halo_width_x $::env(FP_TAP_HORIZONTAL_HALO)\
-    -halo_width_y $::env(FP_TAP_VERTICAL_HALO)
+    -tapcell_master "$::env(WELLTAP_CELL)"\
+    -endcap_master "$::env(ENDCAP_CELL)"\
+    -halo_width_x $::env(FP_MACRO_HORIZONTAL_HALO)\
+    -halo_width_y $::env(FP_MACRO_VERTICAL_HALO)
+
+write_views
+
+report_design_area_metrics
 
-write_views
```

### Comparing `openlane-2.0.0b9/openlane/scripts/openroad/write_views.tcl` & `openlane-2.0.0rc2/openlane/scripts/openroad/dpl.tcl`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,24 @@
-# Copyright 2022 Efabless Corporation
+# Copyright 2020-2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
 read_current_odb
-write_views
+
+source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
+
+check_placement -verbose
+
+write_views
+
+report_design_area_metrics
+
```

### Comparing `openlane-2.0.0b9/openlane/scripts/yosys/json_header.tcl` & `openlane-2.0.0rc2/openlane/scripts/yosys/common.tcl`

 * *Files 27% similar despite different names*

```diff
@@ -7,34 +7,48 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-yosys -import
-source $::env(SCRIPTS_DIR)/yosys/common.tcl
-set vtop $::env(DESIGN_NAME)
+source $::env(_TCL_ENV_IN)
 
-read_deps "on"
+proc read_verilog_files {top_module} {
+    set verilog_include_args [list]
+    if {[info exist ::env(VERILOG_INCLUDE_DIRS)]} {
+        foreach dir $::env(VERILOG_INCLUDE_DIRS) {
+            lappend verilog_include_args "-I$dir"
+        }
+    }
+
+    set synlig_params [list]
 
-set verilog_include_args [list]
-if {[info exist ::env(VERILOG_INCLUDE_DIRS)]} {
-    foreach dir $::env(VERILOG_INCLUDE_DIRS) {
-        lappend verilog_include_args "-I$dir"
+    if { [info exists ::env(SYNTH_PARAMETERS) ] } {
+        foreach define $::env(SYNTH_PARAMETERS) {
+            set param_and_value [split $define "="]
+            lassign $param_and_value param value
+            lappend synlig_params "-P$param=$value"
+        }
     }
-}
-foreach file $::env(VERILOG_FILES) {
-    read_verilog -sv {*}$verilog_include_args $file
-}
 
-if { [info exists ::env(SYNTH_PARAMETERS) ] } {
-    foreach define $::env(SYNTH_PARAMETERS) {
-        set param_and_value [split $define "="]
-        lassign $param_and_value param value
-        chparam -set $param $value $vtop
+    if { $::env(USE_SYNLIG) && $::env(SYNLIG_DEFER) } {
+        foreach file $::env(VERILOG_FILES) {
+            read_systemverilog -defer {*}$::_synlig_defines -sverilog {*}$verilog_include_args $file
+        }
+        read_systemverilog -link -top $::env(DESIGN_NAME) {*}$synlig_params
+    } elseif { $::env(USE_SYNLIG) } {
+        read_systemverilog -top $::env(DESIGN_NAME) {*}$::_synlig_defines {*}$synlig_params -sverilog {*}$verilog_include_args {*}$::env(VERILOG_FILES)
+    } else {
+        foreach file $::env(VERILOG_FILES) {
+            read_verilog -noautowire -sv {*}$verilog_include_args $file
+        }
+
+        if { [info exists ::env(SYNTH_PARAMETERS) ] } {
+            foreach define $::env(SYNTH_PARAMETERS) {
+                set param_and_value [split $define "="]
+                lassign $param_and_value param value
+                chparam -set $param $value $top_module
+            }
+        }
     }
 }
-hierarchy -check -top $vtop
-yosys rename -top $vtop
-yosys proc
-json -o $::env(SAVE_JSON_HEADER)
```

### Comparing `openlane-2.0.0b9/openlane/scripts/yosys/synthesize.tcl` & `openlane-2.0.0rc2/openlane/scripts/yosys/synthesize.tcl`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 set report_dir $::env(STEP_DIR)/reports
 file mkdir $report_dir
 
 # inputs expected as env vars
 set vtop $::env(DESIGN_NAME)
 
+source $::env(_DEPS_SCRIPT)
+
 set lib_args [list]
 foreach lib $::env(SYNTH_LIBS) {
     lappend lib_args -liberty $lib
 }
 
 if {[info exists ::env(DFF_LIB_SYNTH)]} {
     set dfflib $::env(DFF_LIB_SYNTH)
@@ -50,16 +52,14 @@
 }
 
 set dfflib_args [list]
 foreach lib $dfflib {
     lappend dfflib_args -liberty $lib
 }
 
-read_deps
-
 set max_FO $::env(MAX_FANOUT_CONSTRAINT)
 set max_TR 0
 if { [info exist ::env(MAX_TRANSITION_CONSTRAINT)]} {
     set max_TR [expr {$::env(MAX_TRANSITION_CONSTRAINT) * 1000}]; # ns -> ps
 }
 set clock_period [expr {$::env(CLOCK_PERIOD) * 1000}]; # ns -> ps
 
@@ -77,19 +77,28 @@
 close $outfile
 
 
 # Assemble Scripts (By Strategy)
 set abc_rs_K    "resub,-K,"
 set abc_rs      "resub"
 set abc_rsz     "resub,-z"
-set abc_rw_K    "rewrite,-K,"
-set abc_rw      "rewrite"
-set abc_rwz     "rewrite,-z"
-set abc_rf      "refactor"
-set abc_rfz     "refactor,-z"
+set abc_rf      "drf,-l"
+set abc_rfz     "drf,-l,-z"
+set abc_rw      "drw,-l"
+set abc_rwz     "drw,-l,-z"
+set abc_rw_K    "drw,-l,-K"
+if { $::env(SYNTH_ABC_LEGACY_REFACTOR) == "1" } {
+    set abc_rf      "refactor"
+    set abc_rfz     "refactor,-z"
+}
+if { $::env(SYNTH_ABC_LEGACY_REWRITE) == "1" } {
+    set abc_rw      "rewrite"
+    set abc_rwz     "rewrite,-z"
+    set abc_rw_K    "rewrite,-K"
+}
 set abc_b       "balance"
 
 set abc_resyn2        "${abc_b}; ${abc_rw}; ${abc_rf}; ${abc_b}; ${abc_rw}; ${abc_rwz}; ${abc_b}; ${abc_rfz}; ${abc_rwz}; ${abc_b}"
 set abc_share         "strash; multi,-m; ${abc_resyn2}"
 set abc_resyn2a       "${abc_b};${abc_rw};${abc_b};${abc_rw};${abc_rwz};${abc_b};${abc_rwz};${abc_b}"
 set abc_resyn3        "balance;resub;resub,-K,6;balance;resub,-z;resub,-z,-K,6;balance;resub,-z,-K,5;balance"
 set abc_resyn2rs      "${abc_b};${abc_rs_K},6;${abc_rw};${abc_rs_K},6,-N,2;${abc_rf};${abc_rs_K},8;${abc_rw};${abc_rs_K},10;${abc_rwz};${abc_rs_K},10,-N,2;${abc_b},${abc_rs_K},12;${abc_rfz};${abc_rs_K},12,-N,2;${abc_rwz};${abc_b}"
@@ -122,42 +131,42 @@
     set abc_fine_tune       "upsize,{D};dnsize,{D}"
 } else {
     set abc_fine_tune       ""
 }
 
 
 set delay_scripts [list \
-    "+read_constr,${sdc_file};fx;mfs;strash;refactor;${abc_resyn2};${abc_retime_dly}; scleanup;${abc_map_old_dly};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
+    "+read_constr,${sdc_file};fx;mfs;strash;${abc_rf};${abc_resyn2};${abc_retime_dly}; scleanup;${abc_map_old_dly};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
     \
-    "+read_constr,${sdc_file};fx;mfs;strash;refactor;${abc_resyn2};${abc_retime_dly}; scleanup;${abc_choice2};${abc_map_old_dly};${abc_area_recovery_2}; retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
+    "+read_constr,${sdc_file};fx;mfs;strash;${abc_rf};${abc_resyn2};${abc_retime_dly}; scleanup;${abc_choice2};${abc_map_old_dly};${abc_area_recovery_2}; retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
     \
-    "+read_constr,${sdc_file};fx;mfs;strash;refactor;${abc_resyn2};${abc_retime_dly}; scleanup;${abc_choice};${abc_map_old_dly};${abc_area_recovery_1}; retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
+    "+read_constr,${sdc_file};fx;mfs;strash;${abc_rf};${abc_resyn2};${abc_retime_dly}; scleanup;${abc_choice};${abc_map_old_dly};${abc_area_recovery_1}; retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
     \
-    "+read_constr,${sdc_file};fx;mfs;strash;refactor;${abc_resyn2};${abc_retime_area};scleanup;${abc_choice2};${abc_map_new_area};${abc_choice2};${abc_map_old_dly};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
+    "+read_constr,${sdc_file};fx;mfs;strash;${abc_rf};${abc_resyn2};${abc_retime_area};scleanup;${abc_choice2};${abc_map_new_area};${abc_choice2};${abc_map_old_dly};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
     "+read_constr,${sdc_file};&get -n;&st;&dch;&nf;&put;&get -n;&st;&syn2;&if -g -K 6;&synch2;&nf;&put;&get -n;&st;&syn2;&if -g -K 6;&synch2;&nf;&put;&get -n;&st;&syn2;&if -g -K 6;&synch2;&nf;&put;&get -n;&st;&syn2;&if -g -K 6;&synch2;&nf;&put;&get -n;&st;&syn2;&if -g -K 6;&synch2;&nf;&put;buffer -c -N ${max_FO};topo;stime -c;upsize -c;dnsize -c;;stime,-p;print_stats -m" \
 ]
 
 set area_scripts [list \
-    "+read_constr,${sdc_file};fx;mfs;strash;refactor;${abc_resyn2};${abc_retime_area};scleanup;${abc_choice2};${abc_map_new_area};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
+    "+read_constr,${sdc_file};fx;mfs;strash;${abc_rf};${abc_resyn2};${abc_retime_area};scleanup;${abc_choice2};${abc_map_new_area};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
     \
-    "+read_constr,${sdc_file};fx;mfs;strash;refactor;${abc_resyn2};${abc_retime_area};scleanup;${abc_choice2};${abc_map_new_area};${abc_choice2};${abc_map_new_area};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
+    "+read_constr,${sdc_file};fx;mfs;strash;${abc_rf};${abc_resyn2};${abc_retime_area};scleanup;${abc_choice2};${abc_map_new_area};${abc_choice2};${abc_map_new_area};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
     \
-    "+read_constr,${sdc_file};fx;mfs;strash;refactor;${abc_choice2};${abc_retime_area};scleanup;${abc_choice2};${abc_map_new_area};${abc_choice2};${abc_map_new_area};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
+    "+read_constr,${sdc_file};fx;mfs;strash;${abc_rf};${abc_choice2};${abc_retime_area};scleanup;${abc_choice2};${abc_map_new_area};${abc_choice2};${abc_map_new_area};retime,-D,{D};&get,-n;&st;&dch;&nf;&put;${abc_fine_tune};stime,-p;print_stats -m" \
     "+read_constr,${sdc_file};strash;dch;map -B 0.9;topo;stime -c;buffer -c -N ${max_FO};upsize -c;dnsize -c;stime,-p;print_stats -m" \
 ]
 
 set all_scripts [list {*}$delay_scripts {*}$area_scripts]
 
 set strategy_parts [split $::env(SYNTH_STRATEGY)]
 
 proc synth_strategy_format_err { } {
     upvar area_scripts area_scripts
     upvar delay_scripts delay_scripts
     log -stderr "\[ERROR] Misformatted SYNTH_STRATEGY (\"$::env(SYNTH_STRATEGY)\")."
-    log -stderr "\[ERROR] Correct format is \"DELAY|AREA 0-[expr [llength $delay_scripts]-1]|0-[expr [llength $area_scripts]-1]\"."
+    log -stderr "\[ERROR] Correct format is \"DELAY 0-[expr [llength $delay_scripts]-1]|AREA 0-[expr [llength $area_scripts]-1]\"."
     exit 1
 }
 
 if { [llength $strategy_parts] != 2 } {
     synth_strategy_format_err
 }
 
@@ -192,34 +201,33 @@
 if { !($adder_type in [list "YOSYS" "FA" "RCA" "CSA"]) } {
     log -stderr "\[ERROR] Misformatted SYNTH_ADDER_TYPE (\"$::env(SYNTH_ADDER_TYPE)\")."
     log -stderr "\[ERROR] Correct format is \"YOSYS|FA|RCA|CSA\"."
     exit 1
 }
 
 # Start Synthesis
-set verilog_include_args [list]
-if {[info exist ::env(VERILOG_INCLUDE_DIRS)]} {
-    foreach dir $::env(VERILOG_INCLUDE_DIRS) {
-        lappend verilog_include_args "-I$dir"
-    }
-}
-foreach file $::env(VERILOG_FILES) {
-    read_verilog -sv {*}$verilog_include_args $file
+if { [info exists ::env(VERILOG_FILES) ]} {
+    read_verilog_files $vtop
+} elseif { [info exists ::env(VHDL_FILES)] } {
+    ghdl {*}$::env(VHDL_FILES) -e $::env(DESIGN_NAME)
+} else {
+    puts "SCRIPT NOT CALLED CORRECTLY: EITHER VERILOG_FILES OR VHDL_FILES MUST BE SET"
+    exit -1
 }
 
 if { [info exists ::env(SYNTH_PARAMETERS) ] } {
     foreach define $::env(SYNTH_PARAMETERS) {
         set param_and_value [split $define "="]
         lassign $param_and_value param value
         chparam -set $param $value $vtop
     }
 }
 
 select -module $vtop
-show -format dot -prefix $::env(STEP_DIR)/hierarchy
+catch {show -format dot -prefix $::env(STEP_DIR)/hierarchy}
 select -clear
 hierarchy -check -top $vtop
 yosys rename -top $vtop
 
 if { $::env(SYNTH_ELABORATE_ONLY) } {
     yosys proc
     if { $::env(SYNTH_ELABORATE_FLATTEN) } {
@@ -228,50 +236,57 @@
 
     setattr -set keep 1
 
     splitnets
     opt_clean -purge
 
     tee -o "$report_dir/chk.rpt" check
-    tee -o "$report_dir/stat.json" stat -json
+    tee -o "$report_dir/stat.json" stat -json {*}$lib_args
+    tee -o "$report_dir/stat.log" stat {*}$lib_args
 
     write_verilog -noattr -noexpr -nohex -nodec -defparam "$::env(SAVE_NETLIST)"
+    write_json "$::env(SAVE_NETLIST).json"
     exit 0
 }
 
 # Infer tri-state buffers.
 set tbuf_map false
-if { [info exists ::env(TRISTATE_BUFFER_MAP)] } {
+if { [info exists ::env(SYNTH_TRISTATE_MAP)] } {
     set tbuf_map true
     tribuf
 }
 
 # Handle technology mapping of RCS/CSA adders
 if { $adder_type == "RCA"} {
-    if { [info exists ::env(RIPPLE_CARRY_ADDER_MAP)] } {
+    if { [info exists ::env(SYNTH_RCA_MAP)] } {
         log "\[INFO] Applying ripple carry adder mapping from '$::env(RIPPLE_CARRY_ADDER_MAP)'…"
         techmap -map $::env(RIPPLE_CARRY_ADDER_MAP)
     }
 } elseif { $adder_type == "CSA"} {
-    if { [info exists ::env(CARRY_SELECT_ADDER_MAP)] } {
-        log "\[INFO] Applying carry-select adder mapping from '$::env(CARRY_SELECT_ADDER_MAP)'…"
-        techmap -map $::env(CARRY_SELECT_ADDER_MAP)
+    if { [info exists ::env(SYNTH_CSA_MAP)] } {
+        log "\[INFO] Applying carry-select adder mapping from '$::env(SYNTH_CSA_MAP)'…"
+        techmap -map $::env(SYNTH_CSA_MAP)
     }
 }
 
-# <synth> split to run check -assert in the middle
 hierarchy -check -auto-top
+
+if { [info exists ::env(_LIGHTER_DFF_MAP)] } {
+    puts "Using Lighter with map '$::env(_LIGHTER_DFF_MAP)'…"
+    reg_clock_gating -map $::env(_LIGHTER_DFF_MAP)
+}
+
 proc_clean
 proc_rmdead
 proc_prune
 proc_init
 proc_arst
 proc_rom
 proc_mux
-proc_dlatch
+tee -o "$report_dir/latch.rpt" proc_dlatch
 proc_dff
 proc_memwr
 proc_clean
 tee -o "$report_dir/pre_synth_chk.rpt" check
 opt_expr
 if { $::env(SYNTH_NO_FLAT) != 1 } {
     flatten
@@ -295,45 +310,47 @@
 techmap
 opt -fast
 abc -fast
 opt -fast
 hierarchy -check
 stat
 check
+delete t:\$print
 
 if { [info exists ::env(SYNTH_EXTRA_MAPPING_FILE)] } {
     log "\[INFO] Applying extra mappings from '$::env(SYNTH_EXTRA_MAPPING_FILE)'…"
     techmap -map $::env(SYNTH_EXTRA_MAPPING_FILE)
 }
 
-show -format dot -prefix $::env(STEP_DIR)/post_techmap
+catch {show -format dot -prefix $::env(STEP_DIR)/post_techmap}
 
 if { $::env(SYNTH_SHARE_RESOURCES) } {
     share -aggressive
 }
 
 set fa_map false
 if { $adder_type == "FA" } {
-    if { [info exists ::env(FULL_ADDER_MAP)] } {
+    if { [info exists ::env(SYNTH_FA_MAP)] } {
         extract_fa -fa -v
         extract_fa -ha -v
         set fa_map true
     }
 }
 
 opt
 opt_clean -purge
 
-tee -o "$report_dir/pre_techmap.json" stat -json
+tee -o "$report_dir/pre_techmap.json" stat -json {*}$lib_args
+tee -o "$report_dir/pre_techmap.log" stat {*}$lib_args
 
 # Map tri-state buffers
 if { $tbuf_map } {
     log {mapping tbuf}
-    log "\[INFO] Applying tri-state buffer mapping from '$::env(TRISTATE_BUFFER_MAP)'…"
-    techmap -map $::env(TRISTATE_BUFFER_MAP)
+    log "\[INFO] Applying tri-state buffer mapping from '$::env(SYNTH_TRISTATE_MAP)'…"
+    techmap -map $::env(SYNTH_TRISTATE_MAP)
     simplemap
 }
 
 # Map full adders
 if { $fa_map } {
     log "\[INFO] Applying full-adder mapping from '$::env(FULL_ADDER_MAP)'…"
     techmap -map $::env(FULL_ADDER_MAP)
@@ -343,15 +360,16 @@
 if { [info exists ::env(SYNTH_LATCH_MAP)] } {
     log "\[INFO] Applying latch mapping from '$::env(SYNTH_LATCH_MAP)'…"
     techmap -map $::env(SYNTH_LATCH_MAP)
     simplemap
 }
 
 dfflibmap {*}$dfflib_args
-tee -o "$report_dir/post_dff.json" stat -json
+tee -o "$report_dir/post_dff.json" stat -json {*}$lib_args
+tee -o "$report_dir/post_dff.log" stat {*}$lib_args
 
 proc run_strategy {output script strategy_name {postfix_with_strategy 0}} {
     upvar clock_period clock_period
     upvar sdc_file sdc_file
     upvar report_dir report_dir
     upvar lib_args lib_args
 
@@ -376,42 +394,44 @@
     }
 
     if { $::env(SYNTH_DIRECT_WIRE_BUFFERING) } {
         insbuf -buf {*}[split $::env(SYNTH_BUFFER_CELL) "/"]
     }
 
     tee -o "$report_dir/chk.rpt" check
-    tee -o "$report_dir/stat.json" stat -json
+    tee -o "$report_dir/stat.json" stat -json {*}$lib_args
+    tee -o "$report_dir/stat.log" stat {*}$lib_args
 
     if { $::env(SYNTH_AUTONAME) } {
         # Generate public names for the various nets, resulting in very long names that include
         # the full heirarchy, which is preferable to the internal names that are simply
         # sequential numbers such as `_000019_`. Renamed net names can be very long, such as:
         #     manual_reset_gf180mcu_fd_sc_mcu7t5v0__dffq_1_Q_D_gf180mcu_ \
         #     fd_sc_mcu7t5v0__nor3_1_ZN_A1_gf180mcu_fd_sc_mcu7t5v0__aoi21_ \
         #     1_A2_A1_gf180mcu_fd_sc_mcu7t5v0__nand3_1_ZN_A3_gf180mcu_fd_ \
         #     sc_mcu7t5v0__and3_1_A3_Z_gf180mcu_fd_sc_mcu7t5v0__buf_1_I_Z
         autoname
     }
     write_verilog -noattr -noexpr -nohex -nodec -defparam $output
+    write_json "$output.json"
     design -reset
 }
 design -save checkpoint
 
 run_strategy\
     "$::env(SAVE_NETLIST)"\
     "$strategy_script"\
     "$strategy_name"
 
 if { $::env(SYNTH_NO_FLAT) } {
     design -reset
 
-    read_deps
+    source $::env(_DEPS_SCRIPT)
 
-    file copy -force $::env(SAVE_NETLIST) $::env(synthesis_results)/$::env(DESIGN_NAME).hierarchy.nl.v
+    file copy -force $::env(SAVE_NETLIST) $::env(STEP_DIR)/$::env(DESIGN_NAME).hierarchy.nl.v
     read_verilog -sv $::env(SAVE_NETLIST)
     synth -flatten
 
     design -save checkpoint
     run_strategy\
         "$::env(SAVE_NETLIST)"\
         "$strategy_script"\
```

### Comparing `openlane-2.0.0b9/openlane/state/__init__.py` & `openlane-2.0.0rc2/openlane/state/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,12 +16,9 @@
 The State Module
 ----------------
 
 This module manages the State of a Design before and after the execution of an
 OpenLane step. The State is essentially a list of views in various formats in
 addition to the cumulative set of metrics created by previous Steps.
 """
+from .design_format import DesignFormat, DesignFormatObject
 from .state import State, InvalidState, StateElement
-from ..common import DesignFormat, DesignFormatObject
-
-# For backwards compatibility
-from ..common import Path
```

### Comparing `openlane-2.0.0b9/openlane/state/state.py` & `openlane-2.0.0rc2/openlane/state/state.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,27 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import os
+import sys
 import json
 import shutil
 from decimal import Decimal
-from typing import List, Mapping, Union, Optional, Dict, Any
+from typing import Callable, List, Mapping, Tuple, Union, Optional, Dict, Any
+
+from .design_format import (
+    DesignFormat,
+    DesignFormatObject,
+)
 
 from ..common import (
     Path,
     GenericImmutableDict,
     mkdirp,
     copy_recursive,
-    DesignFormat,
-    DesignFormatObject,
 )
+from ..logging import info
 
 
 class InvalidState(RuntimeError):
     pass
 
 
 StateElement = Union[Path, List[Path], Dict[str, Union[Path, List[Path]]], None]
@@ -122,98 +127,108 @@
     def copy(self: "State") -> "State":
         metrics: GenericImmutableDict[str, Any] = GenericImmutableDict(
             copy_recursive(self.metrics)
         )
         new = State(self, metrics=metrics)
         return new
 
-    def __save_snapshot_recursive(
+    def _walk(
         self,
-        path: Union[str, os.PathLike],
         views: Union[Dict, "State"],
+        save_directory: Union[str, os.PathLike],
+        visit: Callable[[str, StateElement, str, str, int], StateElement],
         key_path: str = "",
+        depth: int = 0,
+        top_key: Optional[str] = None,
     ):
-        mkdirp(path)
         for key, value in views.items():
-            current_key_path = f"{key_path}.{key}"
-            if value is None:
-                continue
-            current_folder = key.strip("*")
+            current_top_key = top_key
+            if current_top_key is None:
+                current_top_key = key
+            current_folder = key.strip("_*")
             if df := DesignFormat.by_id(key):
                 # For type-checker: all guaranteed to be DesignFormatObjects
                 assert isinstance(df.value, DesignFormatObject)
                 current_folder = df.value.folder
 
+            target_dir = os.path.join(save_directory, current_folder)
+
+            current_key_path = f"{key_path}.{key}"
+            visit(current_key_path, value, current_top_key, target_dir, depth)
             if isinstance(value, dict):
-                subdirectory = os.path.join(path, current_folder)
-                self.__save_snapshot_recursive(
-                    subdirectory,
+                self._walk(
                     value,
-                    key_path=current_key_path,
+                    target_dir,
+                    visit,
+                    current_key_path,
+                    depth + 1,
+                    current_top_key,
                 )
-            else:
-                target_dir = os.path.join(
-                    path,
-                    current_folder,
-                )
-                mkdirp(target_dir)
-                target_path = os.path.join(target_dir, os.path.basename(value))
-                shutil.copyfile(value, target_path, follow_symlinks=True)
+            if isinstance(value, list):
+                for i, element in enumerate(value):
+                    element_key_path = f"{current_key_path}[{i}]"
+                    visit(
+                        element_key_path,
+                        element,
+                        current_top_key,
+                        target_dir,
+                        depth + 1,
+                    )
 
     def save_snapshot(self, path: Union[str, os.PathLike]):
         """
         Validates the current state then saves all views to a folder by
         design format, including the metrics.
 
         :param path: The folder that would contain other folders.
         """
+
+        def visitor(key, value, top_key, save_directory, depth):
+            if not isinstance(value, Path):
+                return
+            mkdirp(save_directory)
+            target_path = os.path.join(save_directory, os.path.basename(value))
+            shutil.copyfile(value, target_path, follow_symlinks=True)
+
         self.validate()
-        self.__save_snapshot_recursive(path, self)
+        info(f"Saving views to '{os.path.abspath(path)}'…")
+        mkdirp(path)
+        self._walk(self, path, visitor)
         metrics_csv_path = os.path.join(path, "metrics.csv")
         with open(metrics_csv_path, "w", encoding="utf8") as f:
             f.write("Metric,Value\n")
             for metric in self.metrics:
                 f.write(f"{metric},{self.metrics[metric]}\n")
 
         metrics_json_path = os.path.join(path, "metrics.json")
         with open(metrics_json_path, "w", encoding="utf8") as f:
             f.write(self.metrics.dumps())
 
-    def __validate_recursive(
-        self,
-        views: Dict,
-        key_path: str = "",
-        depth: int = 0,
-    ):
-        for key, value in views.items():
-            current_key_path = f"{key_path}.{key}"
-            if depth == 0 and DesignFormat.by_id(key) is None:
-                raise InvalidState(
-                    f"Key {current_key_path} does not match a known design format."
-                )
-            if value is not None:
-                if isinstance(value, Path):
-                    if not value.exists():
-                        raise InvalidState(
-                            f"Path for format {current_key_path} does not exist: '{value}'."
-                        )
-                elif isinstance(value, dict):
-                    self.__validate_recursive(
-                        value, key_path=current_key_path, depth=depth + 1
-                    )
-                else:
-                    raise InvalidState(
-                        f"Value for format '{current_key_path}' is not a Path nor a dictionary of strings to Paths: '{value}'."
-                    )
-
     def validate(self):
         """
         Ensures that all paths exist in a State.
         """
-        self.__validate_recursive(self.to_raw_dict(metrics=False))
+
+        def visitor(key, value, top_key, _, depth):
+            if depth == 0 and DesignFormat.by_id(top_key) is None:
+                raise InvalidState(
+                    f"Key '{top_key}' does not match a known design format."
+                )
+            if value is None:
+                return
+            if not (
+                isinstance(value, Path)
+                or isinstance(value, dict)
+                or isinstance(value, list)
+            ):
+                raise InvalidState(
+                    f"Value at '{key}' is not a Path nor a dictionary/list of Paths: '{value}'."
+                )
+
+        self._walk(self.to_raw_dict(metrics=False), "", visit=visitor)
 
     @classmethod
     def __loads_recursive(
         Self,
         views: Dict,
         validate_path: bool = True,
         key_path: str = "",
@@ -254,38 +269,64 @@
             del raw["metrics"]
 
         views = Self.__loads_recursive(raw, validate_path)
         state = Self(views, metrics=metrics)
 
         return state
 
-    def _repr_html_(self) -> str:
+    def __mapping_to_html_rec(
+        self,
+        mapping: Mapping[str, Any],
+        header_optional: Optional[Tuple[str, str]] = None,
+    ):
         result = """
-        <div style="display: grid; grid-auto-columns: minmax(0, 1fr); grid-auto-rows: minmax(0, 1fr); grid-auto-flow: column;">
-            <table style="grid-column-start: 1; grid-column-end: 2;">
+        <table style="grid-column-start: 1; grid-column-end: 2; ">
+        """
+        if header := header_optional:
+            key_h, value_h = header
+            result += f"""
                 <tr>
-                    <th>Format</th>
-                    <th>Path</th>
+                    <th style="text-align: left;">{key_h}</th>
+                    <th style="text-align: left;">{value_h}</th>
                 </tr>
-        """
-        for id, value in self.to_raw_dict(metrics=False).items():
+            """
+
+        for id, value in mapping.items():
             if value is None:
                 continue
 
-            format = DesignFormat.by_id(id)
-            assert format is not None
-
-            value_rel = os.path.relpath(value, ".")
+            key_content = id
+            if format := DesignFormat.by_id(id):
+                key_content = format.value.id
+
+            value_content = str(value)
+            if isinstance(value, Mapping):
+                value_content = self.__mapping_to_html_rec(value)
+            elif isinstance(value, Path):
+                value_rel = os.path.relpath(value, ".")
+
+                value_content = f'<a href="{value_rel}">{value_rel}</a>'
+                if "google.colab" in sys.modules:
+                    # Can't link in colab
+                    value_content = value_rel
 
             result += f"""
                 <tr>
-                    <td>{format.value.id}</td>
-                    <td><a href="{value_rel}">{value_rel}</a></td>
+                    <td style="text-align: left;">{key_content}</td>
+                    <td style="text-align: left;">{value_content}</td>
                 </tr>
             """
 
         result += """
-            </table>
-        </div>
+        </table>
         """
-
         return result
+
+    def _repr_html_(self) -> str:
+        return (
+            '<div style="display: grid; grid-auto-columns: minmax(0, 1fr); grid-auto-rows: minmax(0, 1fr); grid-auto-flow: column;">'
+            + self.__mapping_to_html_rec(
+                self.to_raw_dict(metrics=False),
+                ("Format", "Path"),
+            )
+            + "</div>"
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlane-2.0.0b9/openlane/steps/__init__.py` & `openlane-2.0.0rc2/openlane/steps/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,33 +19,43 @@
 This modules includes various functions for importing and/or generating OpenLane
 configuration objects. Configuration objects are the primary input to a flow.
 """
 from .step import (
     StepError,
     DeferredStepError,
     StepException,
+    StepNotFound,
     Step,
+    OutputProcessor,
+    DefaultOutputProcessor,
     MetricsUpdate,
     ViewsUpdate,
 )
 from .tclstep import TclStep
 from . import checker as Checker
 
 # You'll notice some TclStep subclasses are exposed separately-
 # this is for documentation.
 from . import yosys as Yosys
 from .yosys import YosysStep
 
+from .openroad_alerts import (
+    OpenROADAlert,
+    OpenROADOutputProcessor,
+    SupportsOpenROADAlerts,
+)
+
 from . import openroad as OpenROAD
 from .openroad import OpenROADStep
 
-from . import magic as Magic
-from .magic import MagicStep
-
 from . import odb as Odb
 from .odb import OdbpyStep
 
+from . import magic as Magic
+from .magic import MagicStep
+
 from . import netgen as Netgen
 from .netgen import NetgenStep
 
 from . import klayout as KLayout
 from . import misc as Misc
+from . import verilator as Verilator
```

### Comparing `openlane-2.0.0b9/openlane/steps/__main__.py` & `openlane-2.0.0rc2/openlane/steps/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,69 +8,59 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-import json
 import shlex
 import shutil
 import datetime
+import functools
+import subprocess
 from functools import partial
-from typing import Any, Dict, Optional, Sequence, Union
+from typing import IO, Any, Dict, Optional, Sequence, Union
 
-from click import pass_context, Context
+from click import pass_context, Context, argument
 from cloup import (
     group,
     option,
     command,
     Path,
 )
 
 from .step import Step, StepError, StepException
 from ..logging import info, err, warn
+from ..flows import cloup_flow_opts
 from ..__version__ import __version__
 from ..common.cli import formatter_settings
 from ..common import mkdirp, Toolbox, get_openlane_root
 
 
-def extract_step_id(ctx: Context, json_in_path: str) -> Optional[str]:
-    try:
-        cfg = json.load(open(json_in_path, encoding="utf8"))
-        meta = cfg.get("meta") or {}
-        return meta.get("step")
-    except json.JSONDecodeError:
-        err("Invalid JSON provided for configuration object.")
-        ctx.exit(-1)
-
-
 def load_step_from_inputs(
     ctx: Context,
     id: Optional[str],
     config: str,
     state_in: str,
+    pdk_root: Optional[str] = None,
 ) -> Step:
-    if id is None:
-        id = extract_step_id(ctx, config)
-        if id is None:
+    Target = Step
+    if id is not None:
+        if Found := Step.factory.get(id):
+            Target = Found
+        else:
             err(
-                "Step ID not provided either in the Configuration object's .meta.step value or over the command-line."
+                f"No step registered with id '{id}'. Ensure all relevant plugins are installed."
             )
             ctx.exit(-1)
-    Target = Step.factory.get(id)
-    if Target is None:
-        err(
-            f"No step registered with id '{id}'. Ensure all relevant plugins are installed."
-        )
-        ctx.exit(-1)
 
     return Target.load(
-        config_path=config,
-        state_in_path=state_in,
+        config=config,
+        state_in=state_in,
+        pdk_root=pdk_root,
     )
 
 
 o = partial(option, show_default=True)
 
 
 @command(formatter_settings=formatter_settings)
@@ -111,24 +101,42 @@
     type=Path(
         exists=True,
         file_okay=True,
         dir_okay=False,
     ),
     required=False,
 )
+@o(
+    "--pdk-root",
+    type=Path(
+        exists=True,
+        file_okay=False,
+        dir_okay=True,
+    ),
+    is_eager=True,
+    default=os.environ.pop("PDK_ROOT", None),
+    help="Use this folder as the PDK root, if running a reproducible that doesn't include the PDK.",
+)
+@cloup_flow_opts(
+    config_options=False,
+    run_options=False,
+    sequential_flow_controls=False,
+    jobs=False,
+    accept_config_files=False,
+)
 @pass_context
-def run(ctx, output, state_in, config, id):
+def run(ctx, output, state_in, config, id, pdk_root, pdk, scl):
     """
     Runs a step using a step-specific configuration object and an input state.
 
     Useful for re-running a step that has already run, or running
     filesystem-independent reproducibles.
     """
 
-    step = load_step_from_inputs(ctx, id, config, state_in)
+    step = load_step_from_inputs(ctx, id, config, state_in, pdk_root)
 
     if step.config.meta.openlane_version != __version__:
         warn(
             "OpenLane version being used is different from the version this step was originally run with. Procceed with caution."
         )
 
     mkdirp(output)
@@ -208,30 +216,37 @@
             "OpenLane version being used is different from the version this step was originally run with. Procceed with caution."
         )
 
     toolbox_dir = os.path.join(".", "toolbox_tmp")
 
     found_cmd: Optional[Sequence[Union[str, os.PathLike]]] = None
     found_env: Optional[Dict[str, Any]] = None
+    found_stdin_data: Optional[Union[str, bytes]] = None
 
     class Stop(Exception):
         pass
 
-    def run_subprocess_subsitute(
+    def popen_substitute(
         cmd: Sequence[Union[str, os.PathLike]],
         env: Optional[Dict[str, Any]] = None,
+        stdin: Optional[IO[Any]] = None,
         *args,
         **kwargs,
-    ):
-        nonlocal found_env, found_cmd
+    ) -> subprocess.Popen:
+        nonlocal found_env, found_cmd, found_stdin_data
         found_cmd = cmd
         found_env = env
+        if found_stdin := stdin:
+            found_stdin_data = found_stdin.read()
         raise Stop()
 
-    step.run_subprocess = run_subprocess_subsitute
+    step.run_subprocess = functools.partial(
+        step.run_subprocess,
+        _popen_callable=popen_substitute,
+    )
 
     try:
         step.start(
             toolbox=Toolbox(toolbox_dir),
             step_dir=".",
         )
     except Stop:
@@ -252,31 +267,57 @@
 
     try:
         shutil.rmtree(target_scripts_dir)
     except FileNotFoundError:
         pass
 
     shutil.copytree(canon_scripts_dir, target_scripts_dir)
+    if chmod := shutil.which("chmod"):
+        # Nix's Files aren't writeable
+        subprocess.check_call([chmod, "-R", "755", target_scripts_dir])
 
     current_env = os.environ
     filtered_env = {
         "STEP_DIR": ".",
         "SCRIPTS_DIR": target_scripts_dir,
     }
     if found_env is not None:
         for key, value in found_env.items():
-            if value != current_env.get(key) and key not in filtered_env:
-                filtered_env[key] = value
+            if (
+                value == current_env.get(key)
+                or key in filtered_env
+                or key in ["PATH", "PYTHONPATH"]
+            ):
+                continue
+            if os.path.isabs(value) and os.path.exists(value):
+                if value.startswith(canon_scripts_dir):
+                    value = value.replace(canon_scripts_dir, target_scripts_dir)
+            filtered_env[key] = value
+
+    cat_in = ""
+    if found_stdin_data:
+        mode = "wb"
+        if isinstance(found_stdin_data, str):
+            mode = "w"
+        with open("STDIN", mode) as f:
+            f.write(found_stdin_data)
+        cat_in = "cat STDIN | "
+
+    found_cmd_filtered = []
+    for cmd in found_cmd:
+        cmd = str(cmd).replace(canon_scripts_dir, target_scripts_dir)
+        found_cmd_filtered.append(cmd)
 
     with open(output, "w", encoding="utf8") as f:
         f.write("#!/bin/sh\n")
         for key, value in filtered_env.items():
             f.write(f"export {key}={shlex.quote(str(value))}\n")
         f.write("\n")
-        f.write(shlex.join([str(e) for e in found_cmd]))
+        f.write(cat_in)
+        f.write(shlex.join([str(e) for e in found_cmd_filtered]))
         f.write("\n")
 
     if hasattr(os, "chmod"):
         os.chmod(output, 0o755)
 
     info("Ejected successfully.")
 
@@ -327,33 +368,69 @@
     type=Path(
         exists=True,
         file_okay=True,
         dir_okay=False,
     ),
     required=False,
 )
+@o(
+    "--include-pdk/--no-include-pdk",
+    type=bool,
+    default=True,
+)
+@o(
+    "--flatten/--no-flatten",
+    type=bool,
+    default=False,
+)
 @pass_context
-def create_reproducible(ctx, output, step_dir, id, config, state_in):
+@argument(
+    "step_dir_arg",
+    type=Path(
+        exists=False,
+        file_okay=False,
+        dir_okay=True,
+    ),
+    default=None,
+    required=False,
+    nargs=1,
+)
+def create_reproducible(
+    ctx,
+    output,
+    step_dir,
+    step_dir_arg,
+    id,
+    config,
+    state_in,
+    include_pdk,
+    flatten,
+):
     """
     Creates a filesystem-independent step reproducible.
 
     The input can be either:
 
     * Both a configuration object (--config) and an input state (--state-in)
 
     * A step directory (--step-dir) generated from a previous run
+      * If not provided, the fallbacks are, in order of priority:
+        * The first non-flag argument
+        * The current working directory
 
     These reproducibles are filesystem-independent, i.e. they can be run
     on any computer that has the appropriate version of OpenLane 2 installed
     (as well as the underlying utility for that specific step.)
 
     The reproducible will report an error if OpenLane is not installed and will
     emit a warning if the installed version of OpenLane mismatches the one
     declared in the config file.
     """
+    step_dir = step_dir or step_dir_arg or os.getcwd()
+
     if step_dir is None:
         if config is None or state_in is None:
             err("Either --step-dir or both --config and --state-in must be provided.")
             ctx.exit(-1)
         elif None in [config, state_in]:
             err(
                 "Both --config and --state-in must be provided if the --step-dir is not provided."
@@ -362,25 +439,59 @@
     else:
         if config is None:
             config = os.path.join(step_dir, "config.json")
         if state_in is None:
             state_in = os.path.join(step_dir, "state_in.json")
 
     step = load_step_from_inputs(ctx, id, config, state_in)
-    step.create_reproducible(output)
+    step.create_reproducible(output, include_pdk, flatten=flatten)
+
+
+@command(formatter_settings=formatter_settings, hidden=True)
+@argument(
+    "step_dir",
+    type=Path(
+        exists=False,
+        file_okay=False,
+        dir_okay=True,
+    ),
+    default=None,
+)
+@o(
+    "--output",
+    type=Path(
+        exists=False,
+        file_okay=False,
+        dir_okay=True,
+    ),
+    default=None,
+)
+@pass_context
+def create_test(ctx, step_dir, output):
+    config = os.path.join(step_dir, "config.json")
+    state_in = os.path.join(step_dir, "state_in.json")
+    if output is None:
+        output = os.path.join(step_dir, "test")
+
+    step = load_step_from_inputs(ctx, None, config, state_in)
+    step.create_reproducible(output, include_pdk=False, flatten=True)
+    os.remove(os.path.join(output, "run_ol.sh"))
+    if os.path.exists(os.path.join(output, "base.sdc")):
+        os.remove(os.path.join(output, "base.sdc"))
 
 
 @group(formatter_settings=formatter_settings)
 def cli():
     """
     Try 'python3 -m openlane.steps COMMAND --help' for help with a specific
     command.
     """
     pass
 
 
 cli.add_command(run)
 cli.add_command(eject)
 cli.add_command(create_reproducible)
+cli.add_command(create_test)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `openlane-2.0.0b9/openlane/steps/common_variables.py` & `openlane-2.0.0rc2/openlane/steps/common_variables.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,123 +28,199 @@
         "FP_IO_HEXTEND",
         Decimal,
         "Extends the horizontal io pins outside of the die by the specified units.",
         default=0,
         units="µm",
     ),
     Variable(
-        "FP_IO_VLENGTH",
+        "FP_IO_VTHICKNESS_MULT",
+        Decimal,
+        "A multiplier for vertical pin thickness. Base thickness is the pins layer min width.",
+        default=2,
+    ),
+    Variable(
+        "FP_IO_HTHICKNESS_MULT",
         Decimal,
-        "The length of the vertical IOs.",
-        default=4,
+        "A multiplier for horizontal pin thickness. Base thickness is the pins layer min width.",
+        default=2,
+    ),
+]
+
+pdn_variables = [
+    Variable(
+        "FP_PDN_SKIPTRIM",
+        bool,
+        "Enables `-skip_trim` option during pdngen which skips the metal trim step, which attempts to remove metal stubs.",
+        default=False,
+    ),
+    Variable(
+        "FP_PDN_CORE_RING",
+        bool,
+        "Enables adding a core ring around the design. More details on the control variables in the PDK config documentation.",
+        default=False,
+    ),
+    Variable(
+        "FP_PDN_ENABLE_RAILS",
+        bool,
+        "Enables the creation of rails in the power grid.",
+        default=True,
+    ),
+    Variable(
+        "FP_PDN_HORIZONTAL_HALO",
+        Decimal,
+        "Sets the horizontal halo around the macros during power grid insertion.",
+        default=10,
         units="µm",
     ),
     Variable(
-        "FP_IO_HLENGTH",
+        "FP_PDN_VERTICAL_HALO",
         Decimal,
-        "The length of the horizontal IOs.",
-        default=4,
+        "Sets the vertical halo around the macros during power grid insertion.",
+        default=10,
         units="µm",
     ),
     Variable(
-        "FP_IO_VTHICKNESS_MULT",
+        "FP_PDN_MULTILAYER",
+        bool,
+        "Controls the layers used in the power grid. If set to false, only the lower layer will be used, which is useful when hardening a macro for integrating into a larger top-level design.",
+        default=True,
+        deprecated_names=["DESIGN_IS_CORE"],
+    ),
+    Variable(
+        "FP_PDN_RAIL_OFFSET",
         Decimal,
-        "A multiplier for vertical pin thickness. Base thickness is the pins layer minwidth.",
-        default=2,
+        "The offset for the power distribution network rails for first metal layer.",
+        units="µm",
+        pdk=True,
     ),
     Variable(
-        "FP_IO_HTHICKNESS_MULT",
+        "FP_PDN_VWIDTH",
         Decimal,
-        "A multiplier for horizontal pin thickness. Base thickness is the pins layer minwidth.",
-        default=2,
+        "The strap width for the vertical layer in generated power distribution networks.",
+        units="µm",
+        pdk=True,
     ),
-]
-
-pdn_variables = [
     Variable(
-        "FP_PDN_VOFFSET",
+        "FP_PDN_HWIDTH",
         Decimal,
-        "The offset of the vertical power stripes on the metal layer 4 in the power distribution network.",
-        default=16.32,
+        "The strap width for the horizontal layer in generated power distribution networks.",
         units="µm",
         pdk=True,
     ),
     Variable(
-        "FP_PDN_VPITCH",
+        "FP_PDN_VSPACING",
         Decimal,
-        "The pitch of the vertical power stripes on the metal layer 4 in the power distribution network.",
-        default=153.6,
+        "Intra-spacing (within a set) of vertical straps in generated power distribution networks.",
         units="µm",
         pdk=True,
     ),
     Variable(
-        "FP_PDN_HOFFSET",
+        "FP_PDN_HSPACING",
         Decimal,
-        "The offset of the horizontal power stripes on the metal layer 5 in the power distribution network.",
-        default=16.65,
+        "Intra-spacing (within a set) of horizontal straps in generated power distribution networks.",
+        units="µm",
+        pdk=True,
+    ),
+    Variable(
+        "FP_PDN_VPITCH",
+        Decimal,
+        "Inter-distance (between sets) of vertical power straps in generated power distribution networks.",
         units="µm",
         pdk=True,
     ),
     Variable(
         "FP_PDN_HPITCH",
         Decimal,
-        "The pitch of the horizontal power stripes on the metal layer 5 in the power distribution network.",
-        default=153.18,
+        "Inter-distance (between sets) of horizontal power straps in generated power distribution networks.",
         units="µm",
         pdk=True,
     ),
     Variable(
-        "FP_PDN_AUTO_ADJUST",
-        bool,
-        "Decides whether or not the flow should attempt to re-adjust the power grid, in order for it to fit inside the core area of the design, if needed.",
-        default=True,
+        "FP_PDN_VOFFSET",
+        Decimal,
+        "Initial offset for sets of vertical power straps.",
+        units="µm",
+        pdk=True,
     ),
     Variable(
-        "FP_PDN_SKIPTRIM",
-        bool,
-        "Enables `-skip_trim` option during pdngen which skips the metal trim step, which attempts to remove metal stubs.",
-        default=True,
+        "FP_PDN_HOFFSET",
+        Decimal,
+        "Initial offset for sets of horizontal power straps.",
+        units="µm",
+        pdk=True,
     ),
     Variable(
-        "FP_PDN_CORE_RING",
-        bool,
-        "Enables adding a core ring around the design. More details on the control variables in the PDK config documentation.",
-        default=False,
+        "FP_PDN_CORE_RING_VWIDTH",
+        Decimal,
+        "The width for the vertical layer in the core ring of generated power distribution networks.",
+        units="µm",
+        pdk=True,
     ),
     Variable(
-        "FP_PDN_ENABLE_RAILS",
-        bool,
-        "Enables the creation of rails in the power grid.",
-        default=True,
+        "FP_PDN_CORE_RING_HWIDTH",
+        Decimal,
+        "The width for the horizontal layer in the core ring of generated power distribution networks.",
+        units="µm",
+        pdk=True,
     ),
     Variable(
-        "FP_PDN_CHECK_NODES",
-        bool,
-        "Enables checking for unconnected nodes in the power grid.",
-        default=True,
+        "FP_PDN_CORE_RING_VSPACING",
+        Decimal,
+        "The spacing for the vertical layer in the core ring of generated power distribution networks.",
+        units="µm",
+        pdk=True,
     ),
     Variable(
-        "FP_PDN_HORIZONTAL_HALO",
+        "FP_PDN_CORE_RING_HSPACING",
         Decimal,
-        "Sets the horizontal halo around the macros during power grid insertion.",
-        default=10,
+        "The spacing for the horizontal layer in the core ring of generated power distribution networks.",
         units="µm",
+        pdk=True,
     ),
     Variable(
-        "FP_PDN_VERTICAL_HALO",
+        "FP_PDN_CORE_RING_VOFFSET",
         Decimal,
-        "Sets the vertical halo around the macros during power grid insertion.",
-        default=10,
+        "The offset for the vertical layer in the core ring of generated power distribution networks.",
         units="µm",
+        pdk=True,
     ),
     Variable(
-        "DESIGN_IS_CORE",
-        bool,
-        "Controls the layers used in the power grid. Depending on whether the design is the core of a chip or a macro inside the core.",
-        default=True,
+        "FP_PDN_CORE_RING_HOFFSET",
+        Decimal,
+        "The offset for the horizontal layer in the core ring of generated power distribution networks.",
+        units="µm",
+        pdk=True,
+    ),
+    Variable(
+        "FP_PDN_RAIL_LAYER",
+        str,
+        "Defines the metal layer used for PDN rails.",
+        deprecated_names=["FP_PDN_RAILS_LAYER"],
+        pdk=True,
+    ),
+    Variable(
+        "FP_PDN_RAIL_WIDTH",
+        Decimal,
+        "Defines the width of PDN rails on the `FP_PDN_RAILS_LAYER` layer.",
+        units="µm",
+        pdk=True,
+    ),
+    Variable(
+        "FP_PDN_HORIZONTAL_LAYER",
+        str,
+        "Defines the horizontal PDN layer.",
+        deprecated_names=["FP_PDN_UPPER_LAYER"],
+        pdk=True,
+    ),
+    Variable(
+        "FP_PDN_VERTICAL_LAYER",
+        str,
+        "Defines the vertical PDN layer.",
+        deprecated_names=["FP_PDN_LOWER_LAYER"],
+        pdk=True,
     ),
 ]
 
 routing_layer_variables = [
     Variable(
         "RT_CLOCK_MIN_LAYER",
         Optional[str],
@@ -163,14 +239,20 @@
     ),
     Variable(
         "GRT_MACRO_EXTENSION",
         int,
         "Sets the number of GCells added to the blockages boundaries from macros. A GCell is typically defined in terms of Mx routing tracks. The default GCell size is 15 M3 pitches.",
         default=0,
     ),
+    Variable(
+        "GRT_LAYER_ADJUSTMENTS",
+        List[Decimal],
+        "Layer-specific reductions in the routing capacity of the edges between the cells in the global routing graph, delimited by commas. Values range from 0 through 1.",
+        pdk=True,
+    ),
 ]
 
 
 dpl_variables = [
     Variable(
         "PL_OPTIMIZE_MIRRORING",
         bool,
@@ -187,49 +269,57 @@
     Variable(
         "PL_MAX_DISPLACEMENT_Y",
         Decimal,
         "Specifies how far an instance can be moved along the Y-axis when finding a site where it can be placed during detailed placement.",
         default=100,
         units="µm",
     ),
+    Variable(
+        "DPL_CELL_PADDING",
+        Decimal,
+        "Cell padding value (in sites) for detailed placement. The number will be integer divided by 2 and placed on both sides. Should be <= global placement.",
+        units="sites",
+        pdk=True,
+    ),
 ]
 
 grt_variables = routing_layer_variables + [
     Variable(
         "DIODE_PADDING",
-        int,
+        Optional[int],
         "Diode cell padding; increases the width of diode cells during placement checks..",
-        default=2,
         units="sites",
     ),
     Variable(
         "GRT_ALLOW_CONGESTION",
         bool,
         "Allow congestion during global routing",
         default=False,
     ),
     Variable(
-        "GRT_REPAIR_ANTENNAS",
-        bool,
-        "Specifies the insertion strategy of diodes to be used in the flow.",
-        default=True,
-    ),
-    Variable(
         "GRT_ANTENNA_ITERS",
         int,
         "The maximum number of iterations for global antenna repairs.",
         default=3,
         deprecated_names=["GRT_ANT_ITERS"],
     ),
     Variable(
         "GRT_OVERFLOW_ITERS",
         int,
         "The maximum number of iterations waiting for the overflow to reach the desired value.",
         default=50,
     ),
+    Variable(
+        "GRT_ANTENNA_MARGIN",
+        int,
+        "The margin to over fix antenna violations.",
+        default=10,
+        units="%",
+        deprecated_names=["GRT_ANT_MARGIN"],
+    ),
 ]
 
 rsz_variables = dpl_variables + [
     Variable(
         "RSZ_DONT_TOUCH_RX",
         str,
         'A single regular expression designating nets or instances as "don\'t touch" by design repairs or resizer optimizations.',
@@ -239,18 +329,12 @@
     Variable(
         "RSZ_DONT_TOUCH_LIST",
         Optional[List[str]],
         'A list of nets and instances as "don\'t touch" by design repairs or resizer optimizations.',
         default=None,
     ),
     Variable(
-        "RSZ_DONT_USE_CELLS",
-        Optional[List[str]],
-        "An optional list of cells to not use during design repair or resizer optimizations in addition to cells that are excluded from PNR altogether.",
-        deprecated_names=["DONT_USE_CELLS"],
-    ),
-    Variable(
         "RSZ_CORNERS",
         Optional[List[str]],
-        "A list of fully-qualifiedd IPVT corners to use during resizer optimizations. If unspecified, the value for `STA_CORNERS` from the PDK will be used.",
+        "A list of fully-qualified IPVT corners to use during resizer optimizations. If unspecified, the value for `STA_CORNERS` from the PDK will be used.",
     ),
 ]
```

### Comparing `openlane-2.0.0b9/openlane/steps/netgen.py` & `openlane-2.0.0rc2/openlane/steps/netgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 from decimal import Decimal
 from abc import abstractmethod
 from typing import List, Dict, Tuple
 
 from .step import ViewsUpdate, MetricsUpdate, Step
 from .tclstep import TclStep
 
-from ..common import Path
-from ..logging import warn
+from ..common import Path, mkdirp, get_script_dir
 from ..config import Variable
 from ..state import DesignFormat, State
 
 
 def get_metrics(stats: Dict) -> Dict:
     metrics: Dict = {}
     if not stats:
@@ -81,20 +80,20 @@
         + property_fails
         + device_fails
         + net_fails
         + pin_fails
     )
     metrics = {}
     metrics["design__lvs_device_difference__count"] = device_differences
-    metrics["design__lvs_net_differences__count"] = net_differences
-    metrics["design__lvs_property_fails__count"] = property_fails
-    metrics["design__lvs_errors__count"] = total_errors
-    metrics["design__lvs_unmatched_devices__count"] = device_fails
-    metrics["design__lvs_unmatched_nets__count"] = net_fails
-    metrics["design__lvs_unmatched_pins__count"] = pin_fails
+    metrics["design__lvs_net_difference__count"] = net_differences
+    metrics["design__lvs_property_fail__count"] = property_fails
+    metrics["design__lvs_error__count"] = total_errors
+    metrics["design__lvs_unmatched_device__count"] = device_fails
+    metrics["design__lvs_unmatched_net__count"] = net_fails
+    metrics["design__lvs_unmatched_pin__count"] = pin_fails
 
     return metrics
 
 
 class NetgenStep(TclStep):
     inputs = []
     outputs = []
@@ -117,74 +116,70 @@
         return ["netgen", "-batch", "source"]
 
 
 @Step.factory.register()
 class LVS(NetgenStep):
     """
     Performs `Layout vs. Schematic <https://en.wikipedia.org/wiki/Layout_Versus_Schematic>`_ checks on the extracted SPICE netlist versus.
-    a verilog netlist with power connections.
+    a Verilog netlist with power connections.
 
     This verifies the following:
     * There are no unexpected shorts in the final layout.
     * There are no unexpected opens in the final layout.
     * All signals are connected correctly.
     """
 
     id = "Netgen.LVS"
+    name = "Netgen LVS"
     inputs = [DesignFormat.SPICE, DesignFormat.POWERED_NETLIST]
-    flow_control_variable = "RUN_LVS"
-
-    config_vars = NetgenStep.config_vars + [
-        Variable(
-            "RUN_LVS",
-            bool,
-            "Enables running LVS.",
-            default=True,
-        ),
-    ]
 
     def get_command(self) -> List[str]:
         return super().get_command() + [self.get_script_path()]
 
     def get_script_path(self):
         return os.path.join(self.step_dir, "lvs_script.lvs")
 
     def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         spice_files = []
         if self.config["CELL_SPICE_MODELS"] is None:
-            warn(
+            self.warn(
                 "This PDK does not appear to define any SPICE models. LVS will still run, but all cells will be black-boxed and the result may be inaccurate."
             )
         else:
             spice_files = self.config["CELL_SPICE_MODELS"].copy()
 
         if pdk_spice_files := self.config.get("SPICE_MODELS"):
             spice_files = pdk_spice_files.copy()
 
         if extra_spice_files := self.config.get("EXTRA_SPICE_MODELS"):
             spice_files += extra_spice_files
 
         design_name = self.config["DESIGN_NAME"]
+        reports_dir = os.path.join(self.step_dir, "reports")
+        stats_file = os.path.join(reports_dir, "lvs.netgen.rpt")
+        stats_file_json = os.path.join(reports_dir, "lvs.netgen.json")
+        mkdirp(reports_dir)
+
+        setup_script = os.path.join(get_script_dir(), "netgen", "setup.tcl")
 
         with open(self.get_script_path(), "w") as f:
             for lib in spice_files:
                 print(
                     f"puts \"Reading SPICE netlist file '{lib}'...\"",
                     file=f,
                 )
                 print(
                     f"readnet spice {lib} 1",
                     file=f,
                 )
 
             print(
-                f"lvs {{ {state_in[DesignFormat.SPICE]} {design_name} }} {{ {state_in[DesignFormat.POWERED_NETLIST]} {design_name} }} {self.config['NETGEN_SETUP']} {self.step_dir}/lvs.rpt -json",
+                f"lvs {{ {state_in[DesignFormat.SPICE]} {design_name} }} {{ {state_in[DesignFormat.POWERED_NETLIST]} {design_name} }} {setup_script} {stats_file} -json",
                 file=f,
             )
 
         views_updates, metrics_updates = super().run(state_in, **kwargs)
-        stats_file = os.path.join(self.step_dir, "lvs.json")
-        stats_string = open(stats_file).read()
+        stats_string = open(stats_file_json).read()
         lvs_metrics = get_metrics(json.loads(stats_string, parse_float=Decimal))
         metrics_updates.update(lvs_metrics)
 
         return (views_updates, metrics_updates)
```

### Comparing `openlane-2.0.0b9/openlane/steps/odb.py` & `openlane-2.0.0rc2/openlane/steps/klayout.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,454 +8,498 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-import re
-import json
+import shlex
+import sys
+import site
 import shutil
-from math import inf
-from decimal import Decimal
-from functools import reduce
-from abc import abstractmethod
-from typing import List, Optional, Tuple
-
-from .common_variables import io_layer_variables
-from .step import ViewsUpdate, MetricsUpdate, Step, StepException
-from ..logging import warn
-from ..config import Variable, Macro
-from ..state import State, DesignFormat
-from ..common import Path, get_script_dir, StringEnum
-
-inf_rx = re.compile(r"\b(-?)inf\b")
-
-
-class OdbpyStep(Step):
-    inputs = [DesignFormat.ODB]
-    outputs = [DesignFormat.ODB, DesignFormat.DEF]
+import subprocess
+from os.path import abspath
+from base64 import b64encode
+from typing import Any, Dict, Optional, List, Sequence, Tuple, Union
 
-    def run(self, state_in, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
-        kwargs, env = self.extract_env(kwargs)
-
-        out_paths = {}
-
-        command = self.get_command()
-        for output in [DesignFormat.ODB, DesignFormat.DEF]:
-            filename = f"{self.config['DESIGN_NAME']}.{output.value.extension}"
-            file_path = os.path.join(self.step_dir, filename)
-            command.append(f"--output-{output.value.id}")
-            command.append(file_path)
-            out_paths[output] = Path(file_path)
-
-        command += [
-            str(state_in[DesignFormat.ODB]),
-        ]
-
-        generated_metrics = self.run_subprocess(
-            command,
-            env=env,
-            **kwargs,
-        )
-
-        metrics_path = os.path.join(self.step_dir, "or_metrics_out.json")
-        metrics_updates: MetricsUpdate = generated_metrics
-        if os.path.exists(metrics_path):
-            or_metrics_out = json.loads(open(metrics_path).read(), parse_float=Decimal)
-            for key, value in or_metrics_out.items():
-                if value == "Infinity":
-                    or_metrics_out[key] = inf
-                elif value == "-Infinity":
-                    or_metrics_out[key] = -inf
-            metrics_updates.update(or_metrics_out)
-
-        views_updates: ViewsUpdate = {}
-        for output in [DesignFormat.ODB, DesignFormat.DEF]:
-            views_updates[output] = out_paths[output]
+from .step import ViewsUpdate, MetricsUpdate, Step, StepError, StepException
 
-        return views_updates, metrics_updates
+from ..config import Variable
+from ..logging import info
+from ..state import DesignFormat, State
+from ..common import Path, get_script_dir, mkdirp
 
-    def get_command(self) -> List[str]:
-        metrics_path = os.path.join(self.step_dir, "or_metrics_out.json")
 
-        tech_lefs = self.toolbox.filter_views(self.config, self.config["TECH_LEFS"])
-        if len(tech_lefs) != 1:
-            raise StepException(
-                "Misconfigured SCL: 'TECH_LEFS' must return exactly one Tech LEF for its default timing corner."
-            )
+class KLayoutStep(Step):
+    config_vars = [
+        Variable(
+            "KLAYOUT_TECH",
+            Path,
+            "A path to the KLayout layer technology (.lyt) file.",
+            pdk=True,
+        ),
+        Variable(
+            "KLAYOUT_PROPERTIES",
+            Path,
+            "A path to the KLayout layer properties (.lyp) file.",
+            pdk=True,
+        ),
+        Variable(
+            "KLAYOUT_DEF_LAYER_MAP",
+            Path,
+            "A path to the KLayout LEF/DEF layer mapping (.map) file.",
+            pdk=True,
+        ),
+    ]
 
-        lefs = ["--input-lef", tech_lefs[0]]
-        for lef in self.config["CELL_LEFS"]:
-            lefs.append("--input-lef")
-            lefs.append(lef)
-        if extra_lefs := self.config["EXTRA_LEFS"]:
-            for lef in extra_lefs:
-                lefs.append("--input-lef")
-                lefs.append(lef)
-        return (
-            [
-                "openroad",
-                "-exit",
-                "-no_splash",
-                "-metrics",
-                metrics_path,
-                "-python",
-                self.get_script_path(),
+    def run_subprocess(
+        self,
+        cmd: Sequence[Union[str, os.PathLike]],
+        log_to: Optional[Union[str, os.PathLike]] = None,
+        silent: bool = False,
+        report_dir: Optional[Union[str, os.PathLike]] = None,
+        env: Optional[Dict[str, Any]] = None,
+        **kwargs,
+    ) -> Dict[str, Any]:
+        env = env or os.environ.copy()
+        # Hack for Python subprocesses to get access to installed libraries
+        python_path_elements = site.getsitepackages() + sys.path
+        if current_pythonpath := env.get("PYTHONPATH"):
+            python_path_elements.append(current_pythonpath)
+
+        env["PYTHONPATH"] = ":".join(python_path_elements)
+        return super().run_subprocess(cmd, log_to, silent, report_dir, env, **kwargs)
+
+    def get_cli_args(
+        self,
+        *,
+        layer_info: bool = True,
+        include_lefs: bool = False,
+        include_gds: bool = False,
+    ) -> List[str]:
+        result = []
+        if layer_info:
+            lyp = abspath(self.config["KLAYOUT_PROPERTIES"])
+            lyt = abspath(self.config["KLAYOUT_TECH"])
+            lym = abspath(self.config["KLAYOUT_DEF_LAYER_MAP"])
+            if None in [lyp, lyt, lym]:
+                raise StepError(
+                    "Cannot open design in KLayout as the PDK does not appear to support KLayout."
+                )
+            result += ["--lyp", lyp, "--lyt", lyt, "--lym", lym]
+
+        if include_lefs:
+            tech_lefs = self.toolbox.filter_views(self.config, self.config["TECH_LEFS"])
+            if len(tech_lefs) != 1:
+                raise StepException(
+                    "Misconfigured SCL: 'TECH_LEFS' must return exactly one Tech LEF for its default timing corner."
+                )
+
+            lef_args = [
+                "--input-lef",
+                abspath(tech_lefs[0]),
             ]
-            + self.get_subcommand()
-            + lefs
-        )
 
-    @abstractmethod
-    def get_script_path(self):
-        pass
+            for lef in self.config["CELL_LEFS"]:
+                lef_args.append("--input-lef")
+                lef_args.append(abspath(lef))
+
+            macro_lefs = self.toolbox.get_macro_views(self.config, DesignFormat.LEF)
+            for lef in macro_lefs:
+                lef_args.append("--input-lef")
+                lef_args.append(abspath(lef))
+
+            if extra_lefs := self.config["EXTRA_LEFS"]:
+                for lef in extra_lefs:
+                    lef_args.append("--input-lef")
+                    lef_args.append(abspath(lef))
+
+            result += lef_args
+
+        if include_gds:
+            gds_args = []
+            for gds in self.config["CELL_GDS"]:
+                gds_args.append("--with-gds-file")
+                gds_args.append(gds)
+            for gds in self.toolbox.get_macro_views(self.config, DesignFormat.GDS):
+                gds_args.append("--with-gds-file")
+                gds_args.append(gds)
+            if extra_gds := self.config["EXTRA_GDS_FILES"]:
+                for gds in extra_gds:
+                    gds_args.append("--with-gds-file")
+                    gds_args.append(gds)
+            result += gds_args
 
-    def get_subcommand(self) -> List[str]:
-        return []
+        return result
 
 
 @Step.factory.register()
-class ApplyDEFTemplate(OdbpyStep):
-    """
-    Copies the floorplan of a "template" DEF file for a new design, i.e.,
-    it will copy the die area, core area, and non-power pin names and locations.
+class Render(KLayoutStep):
     """
+    Renders a PNG of the layout using KLayout.
 
-    id = "Odb.ApplyDEFTemplate"
-    name = "Apply DEF Template"
+    DEF is required as an input, but if a GDS-II view
+    exists in the input state, it will be used instead.
+    """
 
-    flow_control_variable = "FP_DEF_TEMPLATE"
-    flow_control_msg = "No DEF template provided, skipping…"
+    id = "KLayout.Render"
+    name = "Render Image (w/ KLayout)"
 
-    config_vars = [
-        Variable(
-            "FP_DEF_TEMPLATE",
-            Optional[Path],
-            "Points to the DEF file to be used as a template.",
-        ),
-    ]
-
-    def get_script_path(self):
-        return os.path.join(
-            get_script_dir(),
-            "odbpy",
-            "apply_def_template.py",
-        )
+    inputs = [DesignFormat.DEF]
+    outputs = []
 
-    def get_command(self) -> List[str]:
-        return super().get_command() + [
-            "--def-template",
-            self.config["FP_DEF_TEMPLATE"],
-        ]
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        input_view = state_in[DesignFormat.DEF]
+        if gds := state_in[DesignFormat.GDS]:
+            input_view = gds
 
+        assert isinstance(input_view, Path)
 
-class SetPowerConnections(OdbpyStep):
-    """
-    Uses JSON netlist and module information in Odb to add global power connections
-    for macros in a design.
-    """
+        self.run_subprocess(
+            [
+                sys.executable,
+                os.path.join(get_script_dir(), "klayout", "render.py"),
+                abspath(input_view),
+                "--output",
+                abspath(os.path.join(self.step_dir, "out.png")),
+            ]
+            + self.get_cli_args(include_lefs=True),
+            silent=True,
+        )
 
-    id = "Odb.SetPowerConnections"
-    name = "Set Power Connections"
-    inputs = [DesignFormat.JSON_HEADER, DesignFormat.ODB]
-
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "set_power_connections.py")
-
-    def get_command(self) -> List[str]:
-        state_in = self.state_in.result()
-        return super().get_command() + [
-            "--input-json",
-            str(state_in[DesignFormat.JSON_HEADER]),
-        ]
+        return {}, {}
 
 
 @Step.factory.register()
-class ManualMacroPlacement(OdbpyStep):
-    """
-    Performs macro placement using a simple configuration file. The file is
-    defined as a line-break delimited list of instances and positions, in the
-    format ``instance_name X_pos Y_pos Orientation``.
-
-    If no macro instances are configured, this step is skipped.
+class StreamOut(KLayoutStep):
     """
+    Converts DEF views into GDSII streams using KLayout.
 
-    id = "Odb.ManualMacroPlacement"
-    name = "Manual Macro Placement"
+    The PDK must support KLayout for this step to work, otherwise
+    it will be skipped.
 
-    config_vars = [
-        Variable(
-            "MACRO_PLACEMENT_CFG",
-            Optional[Path],
-            "Path to an optional override for instance placement instead of the `MACROS` object for compatibility with OpenLane 1. If both are `None`, this step is skipped.",
-        ),
-    ]
+    If ``PRIMARY_GDSII_STREAMOUT_TOOL`` is set to ``"klayout"``, both GDS and KLAYOUT_GDS
+    will be updated, and if set to another tool, only ``KLAYOUT_GDS`` will be
+    updated.
+    """
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "manual_macro_place.py")
+    id = "KLayout.StreamOut"
+    name = "GDSII Stream Out (KLayout)"
 
-    def get_command(self) -> List[str]:
-        return super().get_command() + [
-            "--config",
-            os.path.join(self.step_dir, "placement.cfg"),
-            "--fixed",
-        ]
+    inputs = [DesignFormat.DEF]
+    outputs = [DesignFormat.GDS, DesignFormat.KLAYOUT_GDS]
 
     def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
-        cfg_file = Path(os.path.join(self.step_dir, "placement.cfg"))
-        if cfg_ref := self.config.get("MACRO_PLACEMENT_CFG"):
-            warn(
-                "Using 'MACRO_PLACEMENT_CFG' is deprecated. It is recommended to use the 'MACROS' object."
-            )
-            shutil.copyfile(cfg_ref, cfg_file)
-        elif macros := self.config.get("MACROS"):
-            instance_count = reduce(
-                lambda x, y: x + len(y.instances), macros.values(), 0
-            )
-            if instance_count >= 1:
-                with open(cfg_file, "w") as f:
-                    for module, macro in macros.items():
-                        if not isinstance(macro, Macro):
-                            raise StepException(
-                                f"Misconstructed configuration: macro definition for key {module} is not of type 'Macro'."
-                            )
-                        for name, data in macro.instances.items():
-                            f.write(
-                                f"{name} {data.location[0]} {data.location[1]} {data.orientation}\n"
-                            )
-
-        if not cfg_file.exists():
-            warn("No instances found, skipping…")
-            return {}, {}
-
-        return super().run(state_in, **kwargs)
+        views_updates: ViewsUpdate = {}
 
+        klayout_gds_out = os.path.join(
+            self.step_dir,
+            f"{self.config['DESIGN_NAME']}.{DesignFormat.KLAYOUT_GDS.value.extension}",
+        )
+        kwargs, env = self.extract_env(kwargs)
 
-@Step.factory.register()
-class ReportWireLength(OdbpyStep):
-    """
-    Outputs a CSV of long wires, printed by length. Useful as a design aid to
-    detect when one wire is connected to too many things.
-    """
+        self.run_subprocess(
+            [
+                sys.executable,
+                os.path.join(
+                    get_script_dir(),
+                    "klayout",
+                    "stream_out.py",
+                ),
+                state_in[DesignFormat.DEF.value.id],
+                "--output",
+                abspath(klayout_gds_out),
+                "--top",
+                self.config["DESIGN_NAME"],
+            ]
+            + self.get_cli_args(include_lefs=True, include_gds=True),
+            env=env,
+        )
 
-    outputs = []
+        views_updates[DesignFormat.KLAYOUT_GDS] = Path(klayout_gds_out)
 
-    id = "Odb.ReportWireLength"
-    name = "Report Wire Length"
-    outputs = []
+        if self.config["PRIMARY_GDSII_STREAMOUT_TOOL"] == "klayout":
+            gds_path = os.path.join(self.step_dir, f"{self.config['DESIGN_NAME']}.gds")
+            shutil.copy(klayout_gds_out, gds_path)
+            views_updates[DesignFormat.GDS] = Path(gds_path)
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "wire_lengths.py")
+        return views_updates, {}
 
-    def get_command(self) -> List[str]:
-        return super().get_command() + [
-            "--human-readable",
-            "--report-out",
-            os.path.join(self.step_dir, "wire_lengths.csv"),
-        ]
+    def layout_preview(self) -> Optional[str]:
+        if self.state_out is None:
+            return None
+        assert self.toolbox is not None
 
+        if image := self.toolbox.render_png(self.config, self.state_out):
+            image_encoded = b64encode(image).decode("utf8")
+            return f'<img src="data:image/png;base64,{image_encoded}" />'
 
-@Step.factory.register()
-class ReportDisconnectedPins(OdbpyStep):
-    id = "Odb.ReportDisconnectedPins"
-    name = "Report Disconnected Pins"
-
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "disconnected_pins.py")
-
-    def get_command(self) -> List[str]:
-        command = super().get_command()
-        if ignored_modules := self.config["IGNORE_DISCONNECTED_MODULES"]:
-            for module in ignored_modules:
-                command.append("--ignore-module")
-                command.append(module)
-        return command
+        return None
 
 
 @Step.factory.register()
-class CustomIOPlacement(OdbpyStep):
+class XOR(KLayoutStep):
     """
-    Places I/O pins using a custom script, which uses a "pin order configuration"
-    file.
-
-    Check the reference documentation for the structure of said file.
+    Performs an XOR operation on the Magic and KLayout GDS views. The idea is:
+    if there's any difference between the GDSII streams between the two tools,
+    one of them have it wrong and that may lead to ambiguity.
     """
 
-    id = "Odb.CustomIOPlacement"
-    name = "Custom I/O Placement"
-    long_name = "Custom I/O Pin Placement Script"
+    id = "KLayout.XOR"
+    name = "KLayout vs. Magic XOR"
 
-    flow_control_variable = "FP_PIN_ORDER_CFG"
-    flow_control_msg = "No custom floorplan file configured, skipping…"
+    inputs = [
+        DesignFormat.MAG_GDS,
+        DesignFormat.KLAYOUT_GDS,
+    ]
+    outputs = []
 
-    config_vars = io_layer_variables + [
+    config_vars = KLayoutStep.config_vars + [
         Variable(
-            "FP_PIN_ORDER_CFG",
-            Optional[Path],
-            "Path to the configuration file. If set to `None`, this step is skipped.",
+            "KLAYOUT_XOR_THREADS",
+            Optional[int],
+            "Specifies number of threads used in the KLayout XOR check. If unset, this will be equal to your machine's thread count.",
         ),
         Variable(
-            "QUIT_ON_UNMATCHED_IO",
-            bool,
-            "Exit on unmatched pins in a provided `FP_PIN_ORDER_CFG` file.",
-            default=True,
-            deprecated_names=["FP_IO_UNMATCHED_ERROR"],
+            "KLAYOUT_XOR_IGNORE_LAYERS",
+            Optional[List[str]],
+            "KLayout layers to ignore during XOR operations.",
+            pdk=True,
+        ),
+        Variable(
+            "KLAYOUT_XOR_TILE_SIZE",
+            Optional[int],
+            "A tile size for the XOR process in µm.",
+            pdk=True,
         ),
     ]
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "io_place.py")
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        ignored = ""
+        if ignore_list := self.config["KLAYOUT_XOR_IGNORE_LAYERS"]:
+            ignored = ";".join(ignore_list)
+
+        layout_a = state_in[DesignFormat.MAG_GDS]
+        if layout_a is None:
+            self.warn("No Magic stream-out has been performed. Skipping XOR process…")
+            return {}, {}
+        layout_b = state_in[DesignFormat.KLAYOUT_GDS]
+        if layout_b is None:
+            self.warn("No KLayout stream-out has been performed. Skipping XOR process…")
+            return {}, {}
+
+        assert isinstance(layout_a, Path)
+        assert isinstance(layout_b, Path)
+
+        kwargs, env = self.extract_env(kwargs)
+
+        tile_size_options = []
+        if tile_size := self.config["KLAYOUT_XOR_TILE_SIZE"]:
+            tile_size_options += ["--tile-size", str(tile_size)]
 
-    def get_command(self) -> List[str]:
-        length = max(
-            self.config["FP_IO_VLENGTH"],
-            self.config["FP_IO_HLENGTH"],
+        thread_count = self.config["KLAYOUT_XOR_THREADS"] or os.cpu_count() or 1
+        info(f"Running XOR with {thread_count} threads…")
+
+        subprocess_result = self.run_subprocess(
+            [
+                "ruby",
+                os.path.join(
+                    get_script_dir(),
+                    "klayout",
+                    "xor.drc",
+                ),
+                "--output",
+                abspath(os.path.join(self.step_dir, "xor.xml")),
+                "--top",
+                self.config["DESIGN_NAME"],
+                "--threads",
+                thread_count,
+                "--ignore",
+                ignored,
+                abspath(layout_a),
+                abspath(layout_b),
+            ]
+            + tile_size_options,
+            env=env,
         )
 
-        return super().get_command() + [
-            "--config",
-            self.config["FP_PIN_ORDER_CFG"],
-            "--hor-layer",
-            self.config["FP_IO_HLAYER"],
-            "--ver-layer",
-            self.config["FP_IO_VLAYER"],
-            "--hor-width-mult",
-            str(self.config["FP_IO_VTHICKNESS_MULT"]),
-            "--ver-width-mult",
-            str(self.config["FP_IO_HTHICKNESS_MULT"]),
-            "--hor-extension",
-            str(self.config["FP_IO_HEXTEND"]),
-            "--ver-extension",
-            str(self.config["FP_IO_VEXTEND"]),
-            "--length",
-            str(length),
-            (
-                "--unmatched-error"
-                if self.config["QUIT_ON_UNMATCHED_IO"]
-                else "--ignore-unmatched"
-            ),
-        ]
+        return {}, subprocess_result["generated_metrics"]
 
 
 @Step.factory.register()
-class DiodesOnPorts(OdbpyStep):
-    """
-    Unconditionally inserts diodes on design ports diodes on ports,
-    to mitigate the `antenna effect <https://en.wikipedia.org/wiki/Antenna_effect>`_.
-
-    Useful for hardening macros, where ports may get long wires that are
-    unaccounted for when hardening a top-level chip.
-    """
+class DRC(KLayoutStep):
+    id = "KLayout.DRC"
+    name = "Design Rule Check (KLayout)"
 
-    id = "Odb.DiodesOnPorts"
-    name = "Diodes on Ports"
-    long_name = "Diode on Port Insertion Script"
+    inputs = [
+        DesignFormat.GDS,
+    ]
+    outputs = []
 
-    config_vars = [
+    config_vars = KLayoutStep.config_vars + [
+        Variable(
+            "KLAYOUT_DRC_RUNSET",
+            Optional[Path],
+            "A path to KLayout DRC runset.",
+            pdk=True,
+            deprecated_names=["KLAYOUT_DRC_TECH_SCRIPT"],
+        ),
+        Variable(
+            "KLAYOUT_DRC_OPTIONS",
+            Optional[Dict[str, Union[bool, int]]],
+            "Options passed directly to the KLayout DRC runset. They vary from one PDK to another.",
+            pdk=True,
+        ),
         Variable(
-            "DIODE_ON_PORTS",
-            StringEnum("DIODE_ON_PORTS", ["none", "in", "out", "both"]),
-            "Always insert diodes on ports with the specified polarities.",
-            default="none",
+            "KLAYOUT_DRC_THREADS",
+            Optional[int],
+            "Specifies the number of threads to be used in KLayout DRC"
+            + "If unset, this will be equal to your machine's thread count.",
         ),
     ]
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "diodes.py")
+    def run_sky130(self, state_in: State, **kwargs) -> MetricsUpdate:
+        kwargs, env = self.extract_env(kwargs)
+        reports_dir = os.path.join(self.step_dir, "reports")
+        mkdirp(reports_dir)
+        drc_script_path = self.config["KLAYOUT_DRC_RUNSET"]
+        xml_report = os.path.join(reports_dir, "drc_violations.klayout.xml")
+        json_report = os.path.join(reports_dir, "drc_violations.klayout.json")
+        feol = str(self.config["KLAYOUT_DRC_OPTIONS"]["feol"]).lower()
+        beol = str(self.config["KLAYOUT_DRC_OPTIONS"]["beol"]).lower()
+        floating_metal = str(
+            self.config["KLAYOUT_DRC_OPTIONS"]["floating_metal"]
+        ).lower()
+        offgrid = str(self.config["KLAYOUT_DRC_OPTIONS"]["offgrid"]).lower()
+        seal = str(self.config["KLAYOUT_DRC_OPTIONS"]["seal"]).lower()
+        threads = self.config["KLAYOUT_DRC_THREADS"] or (str(os.cpu_count()) or "1")
+        info(f"Running KLayout DRC with {threads} threads…")
 
-    def get_subcommand(self) -> List[str]:
-        return ["place"]
+        input_view = state_in[DesignFormat.GDS]
+        assert isinstance(input_view, Path)
 
-    def get_command(self) -> List[str]:
-        cell, pin = self.config["DIODE_CELL"].split("/")
+        self.run_subprocess(
+            [
+                "klayout",
+                "-b",
+                "-zz",
+                "-r",
+                drc_script_path,
+                "-rd",
+                f"input={abspath(input_view)}",
+                "-rd",
+                f"topcell={self.config['DESIGN_NAME']}",
+                "-rd",
+                f"report={abspath(xml_report)}",
+                "-rd",
+                f"feol={feol}",
+                "-rd",
+                f"beol={beol}",
+                "-rd",
+                f"floating_metal={floating_metal}",
+                "-rd",
+                f"offgrid={offgrid}",
+                "-rd",
+                f"seal={seal}",
+                "-rd",
+                f"threads={threads}",
+            ],
+            env=env,
+        )
 
-        return super().get_command() + [
-            "--diode-cell",
-            cell,
-            "--diode-pin",
-            pin,
-            "--port-protect",
-            self.config["DIODE_ON_PORTS"].value,
-        ]
+        subprocess_result = self.run_subprocess(
+            [
+                "python3",
+                os.path.join(
+                    get_script_dir(),
+                    "klayout",
+                    "xml_drc_report_to_json.py",
+                ),
+                f"--xml-file={abspath(xml_report)}",
+                f"--json-file={abspath(json_report)}",
+            ],
+            env=env,
+            log_to=os.path.join(self.step_dir, "xml_drc_report_to_json.log"),
+        )
+        return subprocess_result["generated_metrics"]
 
     def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
-        if self.config["DIODE_ON_PORTS"].value == "none":
-            warn("'DIODE_ON_PORTS' is set to 'none': skipping…")
-            return {}, {}
-
-        if self.config["GPL_CELL_PADDING"] == 0:
-            warn(
-                "'GPL_CELL_PADDING' is set to 0. This step may cause overlap failures."
+        metrics_updates: MetricsUpdate = {}
+        if self.config["PDK"] in ["sky130A", "sky130B"]:
+            metrics_updates = self.run_sky130(state_in, **kwargs)
+        else:
+            self.warn(
+                f"KLayout DRC is not supported for the {self.config['PDK']} PDK. This step will be skipped."
             )
 
-        return super().run(state_in, **kwargs)
+        return {}, metrics_updates
 
 
 @Step.factory.register()
-class HeuristicDiodeInsertion(OdbpyStep):
+class OpenGUI(KLayoutStep):
     """
-    Runs a custom diode insertion script to mitigate the `antenna effect <https://en.wikipedia.org/wiki/Antenna_effect>`_.
-
-    This script uses the `Manhattan length <https://en.wikipedia.org/wiki/Manhattan_distance>`_
-    of a (non-existent) wire at the global placement stage, and places diodes
-    if they exceed a certain threshold. This, however, requires some padding:
-    `GPL_CELL_PADDING` and `DPL_CELL_PADDING` must be higher than 0 for this
-    script to work reliably.
-
-    This step is unique in that it is the only step with a ``RUN_`` variable that
-    is disabled by default. This is for compatibility with OpenLane 1 configs.
-
-    The original script was written by `Sylvain "tnt" Munaut <https://github.com/smunaut>`_.
+    Opens the DEF view in the KLayout GUI, with layers loaded and mapped
+    properly. Useful to inspect ``.klayout.xml`` database files and the like.
     """
 
-    id = "Odb.HeuristicDiodeInsertion"
-    name = "Heuristic Diode Insertion"
-    long_name = "Heuristic Diode Insertion Script"
+    id = "KLayout.OpenGUI"
+    name = "Open In GUI"
 
-    flow_control_variable = "RUN_HEURISTIC_DIODE_INSERTION"
-    config_vars = [
+    inputs = [DesignFormat.DEF]
+    outputs = []
+
+    config_vars = KLayoutStep.config_vars + [
         Variable(
-            "RUN_HEURISTIC_DIODE_INSERTION",
+            "KLAYOUT_EDITOR_MODE",
             bool,
-            "Enables/disables this step.",
-            default=False,  # For compatibility with OL1. Yep.
+            "Whether to run the KLayout GUI in editor mode or in viewer mode.",
+            default=False,
         ),
         Variable(
-            "HEURISTIC_ANTENNA_THRESHOLD",
-            Optional[Decimal],
-            "A manhattan distance above which a diode is recommended to be inserted by a heuristic inserter. If not specified, the heuristic inserter will typically use a default value.",
-            units="µm",
+            "KLAYOUT_PRIORITIZE_GDS",
+            bool,
+            "Whether to prioritize GDS (if found) when running this step.",
+            default=True,
         ),
     ]
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "diodes.py")
-
-    def get_subcommand(self) -> List[str]:
-        return ["place"]
-
-    def get_command(self) -> List[str]:
-        cell, pin = self.config["DIODE_CELL"].split("/")
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        kwargs, env = self.extract_env(kwargs)
+        mode_args = []
+        if self.config["KLAYOUT_EDITOR_MODE"]:
+            mode_args.append("--editor")
+
+        layout = state_in[DesignFormat.DEF]
+        if self.config["KLAYOUT_PRIORITIZE_GDS"]:
+            if gds := state_in[DesignFormat.GDS]:
+                layout = gds
+        assert isinstance(layout, Path)
 
-        threshold_opts = []
-        if threshold := self.config["HEURISTIC_ANTENNA_THRESHOLD"]:
-            threshold_opts = ["--threshold", threshold]
+        env["KLAYOUT_ARGV"] = shlex.join(
+            [
+                abspath(layout),
+            ]
+            + self.get_cli_args(include_lefs=True)
+        )
 
-        return (
-            super().get_command()
+        cmd = (
+            [
+                shutil.which("klayout") or "klayout",
+            ]
+            + mode_args
             + [
-                "--diode-cell",
-                cell,
-                "--diode-pin",
-                pin,
+                "-rm",
+                os.path.join(
+                    get_script_dir(),
+                    "klayout",
+                    "open_design.py",
+                ),
             ]
-            + threshold_opts
         )
 
-    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
-        if self.config["GPL_CELL_PADDING"] == 0:
-            warn(
-                "'GPL_CELL_PADDING' is set to 0. This step may cause overlap failures."
-            )
+        subprocess.check_call(
+            cmd,
+            env=env,
+            cwd=self.step_dir,
+        )
 
-        return super().run(state_in, **kwargs)
+        return {}, {}
```

### Comparing `openlane-2.0.0b9/openlane/steps/tclstep.py` & `openlane-2.0.0rc2/openlane/steps/tclstep.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,30 +10,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import os
-import json
+import threading
 from enum import Enum
 from decimal import Decimal
 from abc import abstractmethod
 from dataclasses import is_dataclass, asdict
-from typing import Any, ClassVar, List, Tuple
+from typing import (
+    Any,
+    ClassVar,
+    Iterable,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Dict,
+    Union,
+)
 
 from .step import ViewsUpdate, MetricsUpdate, Step, StepException
 
 from ..state import State, DesignFormat
 from ..common import (
     Path,
     TclUtils,
-    GenericDictEncoder,
     get_script_dir,
     protected,
+    is_string,
 )
 
 
 class TclStep(Step):
     """
     A subclass of :class:`Step` that primarily deals with running Tcl-based utilities,
     such as Yosys, OpenROAD and Magic.
@@ -52,31 +63,31 @@
         Converts an arbitrary Python value to Tcl as follows:
 
         * If the value is an instance of a dataclass, it is serialized as a JSON object.
         * If the value is a list, it is joined using :meth:`TclUtils.join`.
         * If the value is a dict, the keys and values are escaped recursively using:
             joined using :meth:`TclUtils.join`.
         * If the value is an Enum, its name is returned.
-        * If the value is boolean, "1" is returned for True and "0" for False.
+        * If the value is Boolean, "1" is returned for True and "0" for False.
         * If the value is numeric, it is converted to a string.
         * Otherwise, the value is passed to ``str()``.
         """
         if is_dataclass(value):
-            return json.dumps(asdict(value), cls=GenericDictEncoder)
-        elif isinstance(value, list):
-            result = []
-            for item in value:
-                result.append(TclStep.value_to_tcl(item))
-            return TclUtils.join(result)
-        elif isinstance(value, dict):
+            return TclStep.value_to_tcl(asdict(value))
+        elif isinstance(value, Mapping):
             result = []
             for v_key, v_value in value.items():
                 result.append(TclStep.value_to_tcl(v_key))
                 result.append(TclStep.value_to_tcl(v_value))
             return TclUtils.join(result)
+        elif isinstance(value, Iterable) and not is_string(value):
+            result = []
+            for item in value:
+                result.append(TclStep.value_to_tcl(item))
+            return TclUtils.join(result)
         elif isinstance(value, Enum):
             return value.name
         elif isinstance(value, bool):
             return "1" if value else "0"
         elif isinstance(value, Decimal) or isinstance(value, int):
             return str(value)
         else:
@@ -121,27 +132,28 @@
 
         :param env: The input environment dictionary
         :param state: The input state
         :returns: a copy of the environment dictionary where ``self.config`` variables
         """
         env = env.copy()
 
+        env["STEP_ID"] = self.get_implementation_id()
         env["SCRIPTS_DIR"] = os.path.abspath(get_script_dir())
         env["STEP_DIR"] = os.path.abspath(self.step_dir)
 
         tech_lefs = self.toolbox.filter_views(self.config, self.config["TECH_LEFS"])
         if len(tech_lefs) != 1:
             raise StepException(
                 "Misconfigured SCL: 'TECH_LEFS' must return exactly one Tech LEF for its default timing corner."
             )
 
         env["TECH_LEF"] = tech_lefs[0]
 
         macro_lefs = self.toolbox.get_macro_views(self.config, DesignFormat.LEF)
-        env["MACRO_LEFS"] = " ".join([str(lef) for lef in macro_lefs])
+        env["MACRO_LEFS"] = TclUtils.join([str(lef) for lef in macro_lefs])
 
         for element in self.config.keys():
             value = self.config[element]
             if value is None:
                 continue
             env[element] = TclStep.value_to_tcl(value)
 
@@ -157,15 +169,15 @@
             env[f"SAVE_{output.name}"] = os.path.join(self.step_dir, filename)
 
         return env
 
     @protected
     def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         """
-        This overriden :meth:`run` function prepares configuration variables and
+        This overridden :meth:`run` function prepares configuration variables and
         inputs for use with Tcl: specifically, it converts them all to
         environment variables so they may be used by the Tcl scripts being called.
         See :meth:`prepare_env` for more info.
 
         Additionally, it logs the output to a ``.log`` file named after the script.
 
         When overriding in a subclass, you may find it useful to use this pattern:
@@ -173,28 +185,28 @@
         .. code-block:: python
 
             kwargs, env = self.extract_env(kwargs)
             env["CUSTOM_ENV_VARIABLE"] = "1"
             return super().run(state_in, env=env, **kwargs)
 
         This will allow you to add further custom environment variables to a call
-        while still respecting an `env` argument further up the call-stack.
+        while still respecting an ``env`` argument further up the call-stack.
 
         :param state_in: See superclass.
-        :param **kwargs: Passed on to subprocess execution: useful if you want to
+        :param \\*\\*kwargs: Passed on to subprocess execution: useful if you want to
             redirect stdin, stdout, etc.
         :returns: see superclass
         """
         command = self.get_command()
 
         kwargs, env = self.extract_env(kwargs)
 
         env = self.prepare_env(env, state_in)
 
-        generated_metrics = self.run_subprocess(
+        subprocess_result = self.run_subprocess(
             command,
             env=env,
             **kwargs,
         )
 
         overrides: ViewsUpdate = {}
         for output in self.outputs:
@@ -202,8 +214,66 @@
                 # Too step-specific.
                 continue
             path = Path(env[f"SAVE_{output.name}"])
             if not path.exists():
                 continue
             overrides[output] = path
 
-        return overrides, generated_metrics
+        return overrides, subprocess_result["generated_metrics"]
+
+    @protected
+    def run_subprocess(
+        self,
+        cmd: Sequence[Union[str, os.PathLike]],
+        log_to: Optional[Union[str, os.PathLike]] = None,
+        silent: bool = False,
+        report_dir: Optional[Union[str, os.PathLike]] = None,
+        env: Optional[Dict[str, str]] = None,
+        **kwargs,
+    ) -> Dict[str, Any]:
+        if env is not None:
+            thread_postfix = f"_{threading.current_thread().name}"
+            if threading.current_thread() is threading.main_thread():
+                thread_postfix = ""
+
+            env_in_dir = report_dir or self.step_dir
+            env_in_file = os.path.join(env_in_dir, f"_env{thread_postfix}.tcl")
+
+            ENV_ALLOWLIST = [
+                "PATH",
+                "PYTHONPATH",
+                "SCRIPTS_DIR",
+                "DESIGN_DIR",
+                "STEP_DIR",
+                "PDK_ROOT",
+                "PDK",
+            ]
+            env_in: List[Tuple[str, str]] = list(env.items())
+
+            # Create new "blank" env dict
+            #
+            # For all values:
+            # If a value is unchanged: keep as is
+            # If a value is changed and is in ENV_ALLOWLIST: emplace in dict
+            # If a value is changed and is not in ENV_ALLOWLIST: write to file
+            #
+            # Emplace file to be sourced in dict with key ``_TCL_ENV_IN``
+            env = os.environ.copy()
+            with open(env_in_file, "w") as f:
+                for key, value in env_in:
+                    if key in env and env[key] == value:
+                        continue
+                    if key in ENV_ALLOWLIST:
+                        env[key] = value
+                    else:
+                        f.write(
+                            f"set ::env({key}) {TclUtils.escape(TclStep.value_to_tcl(value))}\n"
+                        )
+            env["_TCL_ENV_IN"] = env_in_file
+        return super().run_subprocess(
+            cmd=cmd,
+            log_to=log_to,
+            silent=silent,
+            report_dir=report_dir,
+            env=env,
+            **kwargs,
+        )
```

### Comparing `openlane-2.0.0b9/openlane.egg-info/PKG-INFO` & `openlane-2.0.0rc2/openlane.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0b9
+Version: 2.0.0rc2
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized, but some oddities are still to be expected. Proceed with caution.
         >
@@ -17,15 +17,15 @@
             <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style: black"/></a>
             <a href="https://mypy-lang.org/"><img src="https://www.mypy-lang.org/static/mypy_badge.svg" alt="Checked with mypy"/></a>
             <a href="https://nixos.org/"><img src="https://img.shields.io/static/v1?logo=nixos&logoColor=white&label=&message=Built%20with%20Nix&color=41439a" alt="Built with Nix"/></a>
         </p>
         <p align="center">
             <a href="https://colab.research.google.com/github/efabless/openlane2/blob/main/notebook.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"></a>
             <a href="https://openlane2.readthedocs.io/"><img src="https://readthedocs.org/projects/openlane2/badge/?version=latest" alt="Documentation Build Status Badge"/></a>
-            <a href="https://invite.skywater.tools"><img src="https://img.shields.io/badge/Community-Open%20Source%20Silicon%20Slack-ff69b4?logo=slack" alt="Invite to the Open Source Silicon Slack"/></a>
+            <a href="https://open-source-silicon.dev"><img src="https://img.shields.io/badge/Community-Open%20Source%20Silicon%20Slack-ff69b4?logo=slack" alt="Invite to the Open Source Silicon Slack"/></a>
         </p>
         
         OpenLane is a RTL to GDSII infrastructure library based on several components including OpenROAD, Yosys, Magic, Netgen, CVC, KLayout and a number of custom scripts for design exploration and optimization. A reference flow performs all ASIC implementation steps from RTL all the way down to GDSII.
         
         You can find the documentation [here](https://openlane2.readthedocs.io/en/latest/getting_started/) to get started. You can discuss OpenLane 2 in the [#openlane-2](https://open-source-silicon.slack.com/archives/C05M85Q5GCF) channel of the [Efabless Open Source Silicon Slack](https://invite.skywater.tools).
         
         ```python
@@ -52,22 +52,22 @@
         by following [**this link**](https://colab.research.google.com/github/efabless/openlane2/blob/main/notebook.ipynb).
         
         ## Installation
         You'll need the following:
         * Python **3.8** or higher with PIP, Venv and Tkinter
         
         ### Nix (Recommended)
-        Works for macOS and Linux (x86-64). Recommended, as it is more integrated with your filesystem and overall has less upload and download deltas.
+        Works for macOS and Linux (x86-64 and aarch64). Recommended, as it is more integrated with your filesystem and overall has less upload and download deltas.
         
-        See [Nix-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/nix_installation/index.html) in the docs.
+        See [Nix-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/common/nix_installation/index.html) in the docs for more info.
         
         ### Docker
-        Works for Windows, macOS and Linux (x86-64, aarch64 with emulation).
+        Works for Windows, macOS and Linux (x86-64 and aarch64).
         
-        See [Docker-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/docker_installation/index.html) in the docs.
+        See [Docker-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/common/docker_installation/index.html) in the docs for more info.
         
         Do note you'll need to add `--dockerized` right after `openlane` in most CLI invocations.
         
         ### Python-only Installation (Advanced)
         You'll need to bring your own compiled utilities, but otherwise, simply install OpenLane as follows:
         
         ```sh
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0b9 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0rc2 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized,
 but some oddities are still to be expected. Proceed with caution. > > If you
 *don't* know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ************ OOppeennLLaannee ************
@@ -21,27 +21,27 @@
 from openlane.flows import Flow Classic = Flow.factory.get("Classic") flow =
 Classic( { "PDK": "sky130A", "DESIGN_NAME": "spm", "VERILOG_FILES": ["./src/
 spm.v"], "CLOCK_PORT": "clk", "CLOCK_PERIOD": 10, }, design_dir=".", )
 flow.start() ``` ## Try it out You can try OpenLane right in your browser,
 free-of-charge, using Google Colaboratory by following [**this link**](https://
 colab.research.google.com/github/efabless/openlane2/blob/main/notebook.ipynb).
 ## Installation You'll need the following: * Python **3.8** or higher with PIP,
-Venv and Tkinter ### Nix (Recommended) Works for macOS and Linux (x86-64).
-Recommended, as it is more integrated with your filesystem and overall has less
-upload and download deltas. See [Nix-based installation](https://
-openlane2.readthedocs.io/en/latest/getting_started/nix_installation/index.html)
-in the docs. ### Docker Works for Windows, macOS and Linux (x86-64, aarch64
-with emulation). See [Docker-based installation](https://
-openlane2.readthedocs.io/en/latest/getting_started/docker_installation/
-index.html) in the docs. Do note you'll need to add `--dockerized` right after
-`openlane` in most CLI invocations. ### Python-only Installation (Advanced)
-You'll need to bring your own compiled utilities, but otherwise, simply install
-OpenLane as follows: ```sh python3 -m pip install --upgrade openlane ``` ##
-Usage In the root folder of the repository, you may invoke: ```sh python3 -
-m openlane --pdk-root
+Venv and Tkinter ### Nix (Recommended) Works for macOS and Linux (x86-64 and
+aarch64). Recommended, as it is more integrated with your filesystem and
+overall has less upload and download deltas. See [Nix-based installation]
+(https://openlane2.readthedocs.io/en/latest/getting_started/common/
+nix_installation/index.html) in the docs for more info. ### Docker Works for
+Windows, macOS and Linux (x86-64 and aarch64). See [Docker-based installation]
+(https://openlane2.readthedocs.io/en/latest/getting_started/common/
+docker_installation/index.html) in the docs for more info. Do note you'll need
+to add `--dockerized` right after `openlane` in most CLI invocations. ###
+Python-only Installation (Advanced) You'll need to bring your own compiled
+utilities, but otherwise, simply install OpenLane as follows: ```sh python3 -
+m pip install --upgrade openlane ``` ## Usage In the root folder of the
+repository, you may invoke: ```sh python3 -m openlane --pdk-root
 o/pdk>
 o/config.json> ``` To start with, you can try: ```sh python3 -m openlane --pdk-
 root $HOME/.volare ./designs/spm/config.json ``` ## Publication If you use
 OpenLane in your research, please cite the following paper. * M. Shalan and T.
 Edwards, âBuilding OpenLANE: A 130nm OpenROAD-based Tapeout-Proven Flow:
 Invited Paper,â *2020 IEEE/ACM International Conference On Computer Aided
 Design (ICCAD)*, San Diego, CA, USA, 2020, pp. 1-6. [Paper](https://
```

### Comparing `openlane-2.0.0b9/openlane.egg-info/SOURCES.txt` & `openlane-2.0.0rc2/openlane.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,93 +10,116 @@
 openlane.egg-info/SOURCES.txt
 openlane.egg-info/dependency_links.txt
 openlane.egg-info/entry_points.txt
 openlane.egg-info/requires.txt
 openlane.egg-info/top_level.txt
 openlane/common/__init__.py
 openlane/common/cli.py
-openlane/common/design_format.py
 openlane/common/drc.py
 openlane/common/generic_dict.py
-openlane/common/metrics.py
 openlane/common/misc.py
+openlane/common/ring_buffer.py
 openlane/common/tcl.py
 openlane/common/toolbox.py
+openlane/common/tpe.py
+openlane/common/types.py
+openlane/common/metrics/__init__.py
+openlane/common/metrics/__main__.py
+openlane/common/metrics/library.py
+openlane/common/metrics/metric.py
+openlane/common/metrics/util.py
 openlane/config/__init__.py
+openlane/config/__main__.py
 openlane/config/config.py
 openlane/config/flow.py
 openlane/config/pdk_compat.py
 openlane/config/preprocessor.py
 openlane/config/removals.py
 openlane/config/variable.py
+openlane/examples/spm/config.json
+openlane/examples/spm/pin_order.cfg
+openlane/examples/spm-user_project_wrapper/SPM_example.v
+openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc
+openlane/examples/spm-user_project_wrapper/config-tut.json
+openlane/examples/spm-user_project_wrapper/config.json
+openlane/examples/spm-user_project_wrapper/defines.v
+openlane/examples/spm-user_project_wrapper/template.def
+openlane/examples/spm-user_project_wrapper/user_project_wrapper.v
 openlane/flows/__init__.py
 openlane/flows/builtins.py
 openlane/flows/classic.py
 openlane/flows/cli.py
 openlane/flows/flow.py
 openlane/flows/misc.py
 openlane/flows/optimizing.py
 openlane/flows/sequential.py
+openlane/flows/synth_explore.py
 openlane/logging/__init__.py
 openlane/logging/logger.py
 openlane/scripts/base.sdc
 openlane/scripts/klayout/Readme.md
 openlane/scripts/klayout/open_design.py
 openlane/scripts/klayout/render.py
 openlane/scripts/klayout/stream_out.py
+openlane/scripts/klayout/xml_drc_report_to_json.py
 openlane/scripts/klayout/xor.drc
 openlane/scripts/magic/Readme.md
 openlane/scripts/magic/drc.tcl
 openlane/scripts/magic/extract_spice.tcl
+openlane/scripts/magic/get_bbox.tcl
 openlane/scripts/magic/lef.tcl
 openlane/scripts/magic/wrapper.tcl
+openlane/scripts/magic/common/read.tcl
 openlane/scripts/magic/def/antenna_check.tcl
 openlane/scripts/magic/def/mag.tcl
 openlane/scripts/magic/def/mag_gds.tcl
-openlane/scripts/magic/def/read.tcl
 openlane/scripts/magic/gds/drc_batch.tcl
 openlane/scripts/magic/gds/erase_box.tcl
 openlane/scripts/magic/gds/extras_mag.tcl
 openlane/scripts/magic/gds/mag_with_pointers.tcl
-openlane/scripts/magic/gds/read.tcl
 openlane/scripts/magic/lef/extras_maglef.tcl
 openlane/scripts/magic/lef/maglef.tcl
+openlane/scripts/netgen/setup.tcl
 openlane/scripts/odbpy/apply_def_template.py
+openlane/scripts/odbpy/check_antenna_properties.py
 openlane/scripts/odbpy/contextualize.py
 openlane/scripts/odbpy/defutil.py
 openlane/scripts/odbpy/diodes.py
 openlane/scripts/odbpy/disconnected_pins.py
+openlane/scripts/odbpy/exception_codes.py
+openlane/scripts/odbpy/filter_unannotated.py
 openlane/scripts/odbpy/io_place.py
 openlane/scripts/odbpy/label_macro_pins.py
 openlane/scripts/odbpy/lefutil.py
 openlane/scripts/odbpy/manual_macro_place.py
-openlane/scripts/odbpy/padringer.py
 openlane/scripts/odbpy/power_utils.py
 openlane/scripts/odbpy/random_place.py
 openlane/scripts/odbpy/reader.py
 openlane/scripts/odbpy/remove_buffers.py
-openlane/scripts/odbpy/set_power_connections.py
 openlane/scripts/odbpy/snap_to_grid.py
 openlane/scripts/odbpy/wire_lengths.py
+openlane/scripts/openroad/antenna_check.tcl
+openlane/scripts/openroad/antenna_repair.tcl
 openlane/scripts/openroad/basic_mp.tcl
-openlane/scripts/openroad/check_antennas.tcl
 openlane/scripts/openroad/cts.tcl
+openlane/scripts/openroad/cut_rows.tcl
 openlane/scripts/openroad/dpl.tcl
 openlane/scripts/openroad/drt.tcl
 openlane/scripts/openroad/fill.tcl
 openlane/scripts/openroad/floorplan.tcl
 openlane/scripts/openroad/gpl.tcl
 openlane/scripts/openroad/grt.tcl
 openlane/scripts/openroad/gui.tcl
 openlane/scripts/openroad/insert_buffer.tcl
 openlane/scripts/openroad/ioplacer.tcl
 openlane/scripts/openroad/irdrop.tcl
 openlane/scripts/openroad/pdn.tcl
 openlane/scripts/openroad/rcx.tcl
 openlane/scripts/openroad/repair_design.tcl
+openlane/scripts/openroad/repair_design_postgrt.tcl
 openlane/scripts/openroad/rsz_timing_postcts.tcl
 openlane/scripts/openroad/rsz_timing_postgrt.tcl
 openlane/scripts/openroad/tapcell.tcl
 openlane/scripts/openroad/write_views.tcl
 openlane/scripts/openroad/common/dpl.tcl
 openlane/scripts/openroad/common/dpl_cell_pad.tcl
 openlane/scripts/openroad/common/grt.tcl
@@ -104,32 +127,35 @@
 openlane/scripts/openroad/common/pdn_cfg.tcl
 openlane/scripts/openroad/common/resizer.tcl
 openlane/scripts/openroad/common/set_global_connections.tcl
 openlane/scripts/openroad/common/set_layer_adjustments.tcl
 openlane/scripts/openroad/common/set_power_nets.tcl
 openlane/scripts/openroad/common/set_rc.tcl
 openlane/scripts/openroad/common/set_routing_layers.tcl
+openlane/scripts/openroad/sta/check_macro_instances.tcl
 openlane/scripts/openroad/sta/corner.tcl
-openlane/scripts/openroad/sta/multi_corner.tcl.bk
 openlane/scripts/tclsh/hello.tcl
 openlane/scripts/yosys/common.tcl
 openlane/scripts/yosys/json_header.tcl
 openlane/scripts/yosys/synthesize.tcl
-openlane/smoke_test_design/config.json
-openlane/smoke_test_design/src/spm.v
 openlane/state/__init__.py
+openlane/state/__main__.py
+openlane/state/design_format.py
 openlane/state/state.py
 openlane/steps/__init__.py
 openlane/steps/__main__.py
 openlane/steps/checker.py
 openlane/steps/common_variables.py
+openlane/steps/cvc_rv.py
 openlane/steps/klayout.py
 openlane/steps/magic.py
 openlane/steps/misc.py
 openlane/steps/netgen.py
 openlane/steps/odb.py
 openlane/steps/openroad.py
+openlane/steps/openroad_alerts.py
 openlane/steps/step.py
 openlane/steps/tclstep.py
+openlane/steps/verilator.py
 openlane/steps/yosys.py
 test/__init__.py
 test/conftest.py
```

### Comparing `openlane-2.0.0b9/setup.py` & `openlane-2.0.0rc2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 import os
 import subprocess
 from setuptools import setup, find_packages
 
 module_name = "openlane"
 
-__dir__ = os.path.dirname(__file__)
+__dir__ = os.path.abspath(os.path.dirname(__file__))
 version = subprocess.check_output(
     [
         "python3",
         os.path.join(
-            os.path.abspath(__dir__),
+            __dir__,
             module_name,
             "__version__.py",
         ),
     ],
     encoding="utf8",
 )
 
@@ -25,21 +25,21 @@
     package_data={
         module_name: [
             "py.typed",
             "open_pdks_rev",
             "scripts/*",
             "scripts/**/*",
             "scripts/**/**/*",
-            "smoke_test_design/*",
-            "smoke_test_design/**/*",
+            "examples/*",
+            "examples/**/*",
         ]
     },
     version=version,
     description="An infrastructure for implementing chip design flows",
-    long_description=open("Readme.md").read(),
+    long_description=open(os.path.join(__dir__, "Readme.md")).read(),
     long_description_content_type="text/markdown",
     author="Efabless Corporation and Contributors",
     author_email="donn@efabless.com",
     install_requires=requirements,
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
@@ -47,11 +47,14 @@
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
     ],
     entry_points={
         "console_scripts": [
             "openlane = openlane.__main__:cli",
             "openlane.steps = openlane.steps.__main__:cli",
+            "openlane.config = openlane.config.__main__:cli",
+            "openlane.state = openlane.state.__main__:cli",
+            "openlane.env_info = openlane:env_info_cli",
         ]
     },
     python_requires=">3.8",
 )
```

### Comparing `openlane-2.0.0b9/test/conftest.py` & `openlane-2.0.0rc2/test/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import tempfile
 from shutil import rmtree
 from unittest import mock
 from decimal import Decimal
-from typing import Any, Optional, Iterable, Callable, List, Dict
+from typing import Any, Literal, Optional, Iterable, Callable, List, Dict
 
 import pytest
 from pyfakefs.fake_filesystem_unittest import Patcher
+from _pytest.fixtures import SubRequest
 
 from openlane.config import Variable, Macro
-from openlane.common import StringEnum, Path, GenericDict
+from openlane.common import Path, GenericDict
 
 
 def pytest_assertrepr_compare(op, left, right):
     if isinstance(left, GenericDict) and isinstance(right, GenericDict) and op == "==":
         return_value = ["comparing GenericDict-derived objects"]
         left_d = left.to_raw_dict()
         right_d = right.to_raw_dict()
@@ -35,15 +36,15 @@
             if left_d.get(key) != right_d.get(key):
                 return_value.append(
                     f"  * mismatched values for '{key}': {repr(left_d.get(key))} vs. {repr(right_d.get(key))}"
                 )
         return return_value
 
 
-@pytest.fixture()
+@pytest.fixture
 def _mock_conf_fs():
     with Patcher() as patcher:
         rmtree("/run", ignore_errors=True)
         patcher.fs.create_dir("/cwd/src")
         patcher.fs.create_file("/cwd/src/a.v")
         patcher.fs.create_file("/cwd/src/b.v")
         patcher.fs.create_dir("/cwd/spef")
@@ -60,23 +61,23 @@
         )
         patcher.fs.create_file(
             "/pdk/dummy2/libs.tech/openlane/config.tcl",
             contents="""
             if { ![info exists ::env(STD_CELL_LIBRARY)] } {
                 set ::env(STD_CELL_LIBRARY) "dummy2_scl"
             }
-            set ::env(TECH_LEF) "/pdk/dummy2/libs.ref/techlef/dummy_scl/dummy_tech_lef.tlef"
+            set ::env(TECH_LEF) "/pdk/dummy2/libs.ref/techlef/dummy2_scl/dummy_tech_lef.tlef"
             set ::env(LIB_SYNTH) "sky130_fd_sc_hd__tt_025C_1v80.lib"
             """,
         )
         patcher.fs.create_file(
             "/pdk/dummy/libs.ref/techlef/dummy_scl/dummy_tech_lef.tlef",
         )
         patcher.fs.create_file(
-            "/pdk/dummy2/libs.ref/techlef/dummy_scl/dummy_tech_lef.tlef",
+            "/pdk/dummy2/libs.ref/techlef/dummy2_scl/dummy_tech_lef.tlef",
         )
         patcher.fs.create_file(
             "/pdk/dummy/libs.tech/openlane/dummy_scl/config.tcl",
             contents="",
         )
         patcher.fs.create_file(
             "/pdk/dummy2/libs.tech/openlane/dummy2_scl/config.tcl",
@@ -120,23 +121,30 @@
     def __exit__(self, exc_type, exc_value, traceback):
         super().__exit__(exc_type, exc_value, traceback)
         self.__temp_dir.cleanup()
         self.__temp_dir = None
         self.path = None
 
 
-@pytest.fixture()
-def _chdir_tmp():
+@pytest.fixture
+def _chdir_tmp(request: SubRequest):
+    keep_tmp = request.config.getoption("--keep-tmp")
     import tempfile
 
-    with tempfile.TemporaryDirectory() as dir, chdir(dir):
-        yield
+    if not keep_tmp:
+        with tempfile.TemporaryDirectory() as dir, chdir(dir):
+            yield
+    else:
+        dir = tempfile.mkdtemp()
+        with chdir(dir):
+            print(f"TMP: {dir}")
+            yield
+            print(f"TMP: {dir}")
 
 
-DiodeOnPortsEnum = StringEnum("Ports", ["none", "in"])
 MOCK_PDK_VARS = [
     Variable(
         "STD_CELL_LIBRARY",
         str,
         description="x",
         pdk=True,
     ),
@@ -197,15 +205,15 @@
         "RUN_HEURISTIC_DIODE_INSERTION",
         bool,
         description="x",
         default=False,
     ),
     Variable(
         "DIODE_ON_PORTS",
-        DiodeOnPortsEnum,
+        Literal["none", "in"],
         description="x",
         default="none",
     ),
     Variable(
         "MACROS",
         Optional[Dict[str, Macro]],
         description="x",
@@ -250,15 +258,15 @@
                 )(f)
 
         return f
 
     return decorator
 
 
-@pytest.fixture()
+@pytest.fixture
 @mock_variables()
 def mock_config():
     from openlane.config import Config
 
     mock_config, _ = Config.load(
         {
             "DESIGN_NAME": "whatever",
@@ -318,8 +326,13 @@
     with mock.patch.object(flow, "Progress", MockProgress):
         yield
 
 
 def pytest_configure():
     pytest.COMMON_FLOW_VARS = COMMON_FLOW_VARS
     pytest.mock_variables = mock_variables
-    pytest.DiodeOnPortsEnum = DiodeOnPortsEnum
+
+
+def pytest_addoption(parser):
+    parser.addoption("--step-rx", action="store", default="^$")
+    parser.addoption("--pdk-root", action="store", default=None)
+    parser.addoption("--keep-tmp", action="store_true", default=False)
```

