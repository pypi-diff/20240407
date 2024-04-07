# Comparing `tmp/velbus-aio-2024.4.0.tar.gz` & `tmp/velbus-aio-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velbus-aio-2024.4.0.tar", last modified: Mon Apr  1 10:44:45 2024, max compression
+gzip compressed data, was "velbus-aio-2024.4.1.tar", last modified: Sun Apr  7 12:20:10 2024, max compression
```

## Comparing `velbus-aio-2024.4.0.tar` & `velbus-aio-2024.4.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/velbus_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:45.607878 velbus-aio-2024.4.0/velbusaio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22998 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/command_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/velbusaio/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/blind_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/bus_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/bus_error_counter_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/bus_error_counter_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/bus_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/channel_name_part1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/channel_name_part2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/channel_name_part3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/channel_name_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/clear_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/counter_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/counter_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/cover_down.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/cover_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/cover_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/cover_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dali_device_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dali_device_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dali_dim_value_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dimmer_channel_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dimmer_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/edge_set_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/edge_set_custom_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/fast_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/forced_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/forced_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/interface_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/ir_receiver_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/kwh_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/light_value_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/memo_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/memory_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/memory_data_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/memory_dump_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_subtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_type_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/push_button_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/read_data_block_from_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/read_data_from_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/realtime_clock_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/receive_buffer_full.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/receive_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/relay_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/restore_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/select_program.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/sensor_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/sensor_temp_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/sensor_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_daylight_saving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_realtime_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/slider_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/slow_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/start_relay_blinking_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/start_relay_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_relay_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_relay_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_to_comfort.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_to_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_to_night.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_to_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part1.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part2.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part3.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part4.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_set_cooling.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_set_heating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/update_led_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/very_fast_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/write_data_to_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/write_memory_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/write_module_address_and_serial_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    34978 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/module.py
--rw-r--r--   0 runner    (1001) docker     (127)   250285 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/protocol.json
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/raw_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/velbus_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:10.689069 velbus-aio-2024.4.1/velbusaio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22799 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/command_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/velbusaio/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/blind_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/bus_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/bus_error_counter_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/bus_error_counter_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/bus_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/channel_name_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/channel_name_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/channel_name_part3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/channel_name_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/clear_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/counter_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/counter_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/cover_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/cover_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/cover_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/cover_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dali_device_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dali_device_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dali_dim_value_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dimmer_channel_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dimmer_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/edge_set_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/edge_set_custom_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/fast_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/forced_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/forced_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/interface_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/ir_receiver_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/kwh_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/light_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/memo_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/memory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/memory_data_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/memory_dump_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_type_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/push_button_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/read_data_block_from_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/read_data_from_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/realtime_clock_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/receive_buffer_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/receive_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/relay_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/restore_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/select_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/sensor_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/sensor_temp_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/sensor_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_daylight_saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_realtime_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/slider_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/slow_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/start_relay_blinking_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/start_relay_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_relay_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_relay_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_to_comfort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_to_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_to_night.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_to_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_set_cooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_set_heating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/update_led_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/very_fast_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/write_data_to_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/write_memory_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/write_module_address_and_serial_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35467 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250396 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/protocol.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/raw_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/util.py
```

### Comparing `velbus-aio-2024.4.0/LICENSE` & `velbus-aio-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/PKG-INFO` & `velbus-aio-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velbus-aio
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/Cereal2nd/velbus-aio
 Project-URL: Bug Reports, https://github.com/Cereal2nd/velbus-aio/issues
 Keywords: home,velbus,automation
 Platform: any
```

### Comparing `velbus-aio-2024.4.0/README.md` & `velbus-aio-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbus_aio.egg-info/PKG-INFO` & `velbus-aio-2024.4.1/velbus_aio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velbus-aio
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/Cereal2nd/velbus-aio
 Project-URL: Bug Reports, https://github.com/Cereal2nd/velbus-aio/issues
 Keywords: home,velbus,automation
 Platform: any
```

### Comparing `velbus-aio-2024.4.0/velbus_aio.egg-info/SOURCES.txt` & `velbus-aio-2024.4.1/velbus_aio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/channels.py` & `velbus-aio-2024.4.1/velbusaio/channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,25 +132,16 @@
         d = self.__dict__
         return {
             k: d[k]
             for k in d
             if k != "_writer" and k != "_on_status_update" and k != "_name_parts"
         }
 
-    def to_json(self) -> dict:
-        d = self.__dict__
-        return {
-            k: d[k]
-            for k in d
-            if k != "_writer"
-            and k != "_on_status_update"
-            and k != "_name_parts"
-            and k != "_module"
-            and k != "__name__"
-        }
+    def to_cache(self) -> dict:
+        return {"name": self._name, "type": type(self).__name__}
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self._on_status_update = []
         self._name_parts = {}
 
     def __repr__(self) -> str:
```

### Comparing `velbus-aio-2024.4.0/velbusaio/command_registry.py` & `velbus-aio-2024.4.1/velbusaio/command_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+"""Command registry.
+
 :author: Maikel Punie <maikel.punie@gmail.com> and Thomas Delaet <thomas@delaet.org>
 """
 
 from __future__ import annotations
 
 MODULE_DIRECTORY = {
     0x01: "VMB8PB",
@@ -83,22 +84,26 @@
     0x5A: "VMBDALI-20",
     0x5C: "VMBEL4PIR-20",
     0x5F: "VMBGP4PIR-20",
 }
 
 
 class CommandRegistry:
+    """Command registry class."""
+
     def __init__(self, module_directory: dict) -> None:
+        """Init method."""
         self._module_directory = module_directory
         self._default_commands = {}
         self._overrides = {}
 
     def register_command(
         self, command_value: int, command_class: type, module_name: str | None = None
     ) -> None:
+        """Register a command."""
         if command_value < 0 or command_value > 255:
             raise ValueError("Command_value should be >=0 and <=255")
         if module_name and module_name not in self._module_directory.values():
             raise Exception(f"Module name {module_name} not known")
         if module_name:
             module_type = next(
                 (
@@ -111,50 +116,56 @@
             self._register_override(command_value, command_class, module_type)
         else:
             self._register_default(command_value, command_class)
 
     def _register_override(
         self, command_value: int, command_class: type, module_type: str
     ) -> None:
+        """Register and override."""
         if module_type not in self._overrides:
             self._overrides[module_type] = {}
         if command_value not in self._overrides[module_type]:
             self._overrides[module_type][command_value] = command_class
         else:
             raise Exception(
                 f"double registration in command registry {command_value} {command_class}"
             )
 
     def _register_default(self, command_value: int, command_class: type) -> None:
+        """Register a default command."""
         if command_value not in self._default_commands:
             self._default_commands[command_value] = command_class
         else:
             raise Exception("double registration in command registry")
 
     def has_command(self, command_value: int, module_type: int = 0) -> bool:
+        """Find a command."""
         if module_type in self._overrides:
             if command_value in self._overrides[module_type]:
                 return True
         if command_value in self._default_commands:
             return True
         return False
 
     def get_command(self, command_value: int, module_type: int = 0) -> None | type:
+        """Search a command in the registry."""
         if module_type in self._overrides:
             if command_value in self._overrides[module_type]:
                 return self._overrides[module_type][command_value]
         if command_value in self._default_commands:
             return self._default_commands[command_value]
         return None
 
 
 commandRegistry = CommandRegistry(MODULE_DIRECTORY)
 
 
 def register(command_value: int, module_types: list[str] | None = None):
+    """Register decorator."""
+
     def inner_register(command_class):
         if module_types:
             for module_type in module_types:
                 commandRegistry.register_command(
                     command_value, command_class, module_type
                 )
         else:
```

### Comparing `velbus-aio-2024.4.0/velbusaio/const.py` & `velbus-aio-2024.4.1/velbusaio/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+"""Constant for velbusaio.
+
 Author: Maikel Punie <maikel.punie@gmail.com>
 """
 
 from __future__ import annotations
 
 from typing import Final
```

### Comparing `velbus-aio-2024.4.0/velbusaio/controller.py` & `velbus-aio-2024.4.1/velbusaio/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-"""
-Main interface for the velbusaio lib
-"""
+"""Main interface for the velbusaio lib."""
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import pathlib
-import pickle
 import re
 import ssl
+import time
 from urllib.parse import urlparse
 
 import serial
 import serial_asyncio
 
 from velbusaio.channels import Channel
 from velbusaio.const import LOAD_TIMEOUT
@@ -27,23 +25,22 @@
 from velbusaio.messages.set_realtime_clock import SetRealtimeClock
 from velbusaio.module import Module
 from velbusaio.protocol import VelbusProtocol
 from velbusaio.raw_message import RawMessage
 
 
 class Velbus:
-    """
-    A velbus controller
-    """
+    """A velbus controller."""
 
     def __init__(
         self,
         dsn: str,
         cache_dir: str = get_cache_dir(),
     ) -> None:
+        """Init the Velbus controller."""
         self._log = logging.getLogger("velbus")
 
         self._protocol = VelbusProtocol(
             message_received_callback=self._on_message_received,
             connection_lost_callback=self._on_connection_lost,
             end_of_scan_callback=self._on_end_of_scan,
         )
@@ -56,110 +53,86 @@
         self._submodules: list[int] = []
         self._send_queue = asyncio.Queue()
         self._cache_dir = cache_dir
         # make sure the cachedir exists
         pathlib.Path(self._cache_dir).mkdir(parents=True, exist_ok=True)
 
     async def _on_message_received(self, msg: RawMessage) -> None:
+        """On message received function."""
         await self._handler.handle(msg)
 
     def _on_connection_lost(self, exc: Exception) -> None:
         """Respond to Protocol connection lost."""
         if self._auto_reconnect and not self._closing:
             self._log.debug("Reconnecting to transport")
             asyncio.ensure_future(self.connect())
 
     def _on_end_of_scan(self) -> None:
+        """Notify the scan failure."""
         self._handler.scan_finished()
 
     async def add_module(
         self,
         addr: int,
         typ: int,
         data: dict,
         serial: int | None = None,
         memorymap: int | None = None,
         build_year: int | None = None,
         build_week: int | None = None,
     ) -> None:
-        """
-        Add a found module to the module cache
-        """
-        mod = self._load_module_from_cache(self._cache_dir, addr)
-        if mod is not None:
-            self._log.info(f"Load module from CACHE: {addr}")
-            self._modules[addr] = mod
-            self._modules[addr].initialize(self.send)
-            await self._modules[addr].load(True)
-        else:
-            self._log.info(f"Load NEW module: {typ} @ {addr}")
-            self._modules[addr] = Module.factory(
-                addr,
-                typ,
-                data,
-                serial=serial,
-                build_year=build_year,
-                build_week=build_week,
-                memorymap=memorymap,
-                cache_dir=self._cache_dir,
-            )
-            self._modules[addr].initialize(self.send)
-            await self._modules[addr].load()
+        """Add a found module to the module cache."""
+        self._log.info(f"Found module: type:{typ} address:{addr}")
+        self._modules[addr] = Module.factory(
+            addr,
+            typ,
+            data,
+            serial=serial,
+            build_year=build_year,
+            build_week=build_week,
+            memorymap=memorymap,
+            cache_dir=self._cache_dir,
+        )
+        self._modules[addr].initialize(self.send)
+        await self._modules[addr].load()
 
     async def add_submodules(self, addr: int, subList: dict[int, int]) -> None:
+        """Add submodules address to module."""
         for sub_num, sub_addr in subList.items():
             if sub_addr == 0xFF:
                 continue
             self._submodules.append(sub_addr)
             self._modules[addr]._sub_address[sub_num] = sub_addr
             self._modules[sub_addr] = self._modules[addr]
         self._modules[addr].cleanupSubChannels()
 
-    def _load_module_from_cache(self, cache_dir: str, address: int) -> None | Module:
-        try:
-            cfile = pathlib.Path(f"{cache_dir}/{address}.p")
-            with cfile.open("rb") as fl:
-                o = pickle.load(fl)
-                if isinstance(o, Module):
-                    return o
-        except OSError:
-            pass
-        return None
-
     def get_modules(self) -> dict:
-        """
-        Return the module cache
-        """
+        """Return the module cache."""
         return self._modules
 
     def get_module(self, addr: str) -> None | Module:
-        """
-        Get a module on an address
-        """
-        if addr in self._modules.keys():
+        """Get a module on an address."""
+        if addr in self._modules:
             return self._modules[addr]
         return None
 
     def get_channels(self, addr: str) -> None | dict:
-        """
-        Get the channels for an address
-        """
+        """Get the channels for an address."""
         if addr in self._modules:
             return (self._modules[addr]).get_channels()
         return None
 
     async def stop(self) -> None:
+        """Stop the controller."""
         self._closing = True
         self._auto_reconnect = False
         self._protocol.close()
 
     async def connect(self, test_connect: bool = False) -> None:
-        """
-        Connect to the bus and load all the data
-        """
+        """Connect to the bus and load all the data."""
         auth = None
         # connect to the bus
         if ":" in self._dsn:
             # tcp/ip combination
             if not re.search(r"^[A-Za-z0-9+.\-]+://", self._dsn):
                 # if no scheme, then add the tcp://
                 self._dsn = f"tcp://{self._dsn}"
@@ -178,15 +151,15 @@
                     lambda: self._protocol,
                     host=parts.hostname,
                     port=parts.port,
                     ssl=ctx,
                 )
 
             except (ConnectionRefusedError, OSError) as err:
-                raise VelbusConnectionFailed() from err
+                raise VelbusConnectionFailed from err
         else:
             # serial port
             try:
                 _transport, _protocol = await serial_asyncio.create_serial_connection(
                     asyncio.get_event_loop(),
                     lambda: self._protocol,
                     url=self._dsn,
@@ -194,25 +167,26 @@
                     bytesize=serial.EIGHTBITS,
                     parity=serial.PARITY_NONE,
                     stopbits=serial.STOPBITS_ONE,
                     xonxoff=0,
                     rtscts=1,
                 )
             except (FileNotFoundError, serial.SerialException) as err:
-                raise VelbusConnectionFailed() from err
+                raise VelbusConnectionFailed from err
         if test_connect:
             return
         # if auth is required send the auth key
         if auth:
             await self._protocol.write_auth_key(auth)
 
         # scan the bus
         await self.scan()
 
     async def scan(self) -> None:
+        """Scan the bus."""
         self._handler.scan_started()
         for addr in range(1, 256):
             msg = ModuleTypeRequestMessage(addr)
             await self.send(msg)
         await self._handler._scan_complete_event.wait()
         # calculate how long to wait
         calc_timeout = len(self._modules) * 30
@@ -226,53 +200,49 @@
             await asyncio.wait_for(tsk, timeout=timeout)
         except asyncio.TimeoutError:
             self._log.error(
                 f"Not all modules are loaded within a timeout of {LOAD_TIMEOUT} seconds, continuing with the loaded modules"
             )
 
     async def _check_if_modules_are_loaded(self) -> None:
-        """
-        Task to wait until modules are loaded
-        """
+        """Task to wait until modules are loaded."""
         while True:
             mods_loaded = 0
             for mod in (self.get_modules()).values():
                 if mod.is_loaded():
                     mods_loaded += 1
                 else:
                     self._log.warning(f"Waiting for module {mod._address}")
             if mods_loaded == len(self.get_modules()):
                 self._log.info("All modules loaded")
                 return
             self._log.info("Not all modules loaded yet, waiting 15 seconds")
             await asyncio.sleep(15)
 
     async def send(self, msg: Message) -> None:
-        """
-        Send a packet
-        """
+        """Send a packet."""
         await self._protocol.send_message(
             RawMessage(
                 priority=msg.priority,
                 address=msg.address,
                 rtr=msg.rtr,
                 data=msg.data_to_binary(),
             )
         )
 
     def get_all(self, class_name: str) -> list[Channel]:
+        """Get all channels."""
         lst = []
         for addr, mod in (self.get_modules()).items():
             if addr in self._submodules:
                 continue
             for chan in (mod.get_channels()).values():
                 if class_name in chan.get_categories():
                     lst.append(chan)
         return lst
 
     async def sync_clock(self) -> None:
-        """
-        This will send all the needed messages to sync the clock
-        """
-        await self.send(SetRealtimeClock())
-        await self.send(SetDate())
-        await self.send(SetDaylightSaving())
+        """Will send all the needed messages to sync the clock."""
+        lclt = time.localtime()
+        await self.send(SetRealtimeClock(wday=lclt[6], hour=lclt[3], min=lclt[4]))
+        await self.send(SetDate(day=lclt[2], mon=lclt[1], year=lclt[0]))
+        await self.send(SetDaylightSaving(ds=not lclt[8]))
```

### Comparing `velbus-aio-2024.4.0/velbusaio/discovery.py` & `velbus-aio-2024.4.1/velbusaio/discovery.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/exceptions.py` & `velbus-aio-2024.4.1/velbusaio/exceptions.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/handler.py` & `velbus-aio-2024.4.1/velbusaio/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
-import re
 from typing import TYPE_CHECKING, Awaitable, Callable
 import pkg_resources
 
 from velbusaio.command_registry import commandRegistry
 from velbusaio.helpers import h2, keys_exists
 from velbusaio.message import Message
 from velbusaio.messages.module_subtype import ModuleSubTypeMessage
@@ -101,15 +100,17 @@
                 msg.populate(priority, address, rtr, data)
                 self._log.debug(f"Received {msg}")
                 # send the message to the modules
                 await self._velbus.get_module(msg.address).on_message(msg)
             else:
                 self._log.warning(
                     "NOT FOUND IN command_registry: addr={} cmd={} packet={}".format(
-                        address, command_value, ":".join(format(x, "02x") for x in data)
+                        address,
+                        command_value,
+                        ":".join(format(x, "02x") for x in data),
                     )
                 )
         elif self._scan_complete:
             # this should only happen once the scan is complete, of its not complete suspended the error message
             self._log.warning(
                 "UNKNOWN module, you should initialize a full new velbus scan: packet={}, address={}, modules={}".format(
                     ":".join(format(x, "02x") for x in data),
```

### Comparing `velbus-aio-2024.4.0/velbusaio/helpers.py` & `velbus-aio-2024.4.1/velbusaio/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Helper functions
 """
 
 from __future__ import annotations
 
 import os
 import re
-from typing import Any, Dict
+from typing import Any
 
 from velbusaio.const import CACHEDIR
 
 
 def keys_exists(element: dict[str, Any], *keys) -> dict:
     """
     Check if *keys (nested) exists in `element` (dict).
```

### Comparing `velbus-aio-2024.4.0/velbusaio/message.py` & `velbus-aio-2024.4.1/velbusaio/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 The velbus abstract message class
 """
 
 from __future__ import annotations
 
 import json
-from typing import Optional
 
 from velbusaio.const import PRIORITY_FIRMWARE, PRIORITY_HIGH, PRIORITY_LOW
 
 
 class ParserError(Exception):
     """
     Error when invalid message is received
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/__init__.py` & `velbus-aio-2024.4.1/velbusaio/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/blind_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/blind_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/bus_active.py` & `velbus-aio-2024.4.1/velbusaio/messages/bus_active.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/bus_error_counter_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/bus_error_counter_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/bus_error_counter_status_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/bus_error_counter_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/bus_off.py` & `velbus-aio-2024.4.1/velbusaio/messages/bus_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/channel_name_part1.py` & `velbus-aio-2024.4.1/velbusaio/messages/channel_name_part1.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/channel_name_part2.py` & `velbus-aio-2024.4.1/velbusaio/messages/channel_name_part2.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/channel_name_part3.py` & `velbus-aio-2024.4.1/velbusaio/messages/channel_name_part3.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/channel_name_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/channel_name_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/clear_led.py` & `velbus-aio-2024.4.1/velbusaio/messages/clear_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/counter_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/counter_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/counter_status_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/counter_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/cover_down.py` & `velbus-aio-2024.4.1/velbusaio/messages/cover_down.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/cover_off.py` & `velbus-aio-2024.4.1/velbusaio/messages/cover_off.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 :author: Tom Dupré <gitd8400@gmail.com>
 """
 
 from __future__ import annotations
 
-import struct
-
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x04
 
 
 @register(COMMAND_CODE, ["VMB1BLE", "VMB2BLE", "VMB1BLS"])
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/cover_position.py` & `velbus-aio-2024.4.1/velbusaio/messages/cover_position.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
 
 from __future__ import annotations
 
-import struct
-
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x1C
 
 
 @register(COMMAND_CODE, ["VMB1BLE", "VMB2BLE", "VMB1BLS"])
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/cover_up.py` & `velbus-aio-2024.4.1/velbusaio/messages/cover_up.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/dali_device_settings.py` & `velbus-aio-2024.4.1/velbusaio/messages/dali_device_settings.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/dali_device_settings_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/dali_device_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/dali_dim_value_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/dali_dim_value_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/dimmer_channel_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/dimmer_channel_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/dimmer_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/dimmer_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/edge_set_color.py` & `velbus-aio-2024.4.1/velbusaio/messages/edge_set_color.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/edge_set_custom_color.py` & `velbus-aio-2024.4.1/velbusaio/messages/edge_set_custom_color.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/fast_blinking_led.py` & `velbus-aio-2024.4.1/velbusaio/messages/fast_blinking_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/forced_off.py` & `velbus-aio-2024.4.1/velbusaio/messages/forced_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/forced_on.py` & `velbus-aio-2024.4.1/velbusaio/messages/forced_on.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/interface_status_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/interface_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/kwh_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/kwh_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/light_value_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/light_value_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/memo_text.py` & `velbus-aio-2024.4.1/velbusaio/messages/memo_text.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/memory_data.py` & `velbus-aio-2024.4.1/velbusaio/messages/memory_data.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/memory_data_block.py` & `velbus-aio-2024.4.1/velbusaio/messages/memory_data_block.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/memory_dump_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/memory_dump_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/module_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/module_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/module_status_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/module_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/module_subtype.py` & `velbus-aio-2024.4.1/velbusaio/messages/module_subtype.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/module_type.py` & `velbus-aio-2024.4.1/velbusaio/messages/module_type.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/module_type_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/module_type_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/push_button_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/push_button_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/raw.py` & `velbus-aio-2024.4.1/velbusaio/messages/raw.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/read_data_block_from_memory.py` & `velbus-aio-2024.4.1/velbusaio/messages/read_data_block_from_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/read_data_from_memory.py` & `velbus-aio-2024.4.1/velbusaio/messages/read_data_from_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/realtime_clock_status_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/realtime_clock_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/receive_buffer_full.py` & `velbus-aio-2024.4.1/velbusaio/messages/receive_buffer_full.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/receive_ready.py` & `velbus-aio-2024.4.1/velbusaio/messages/receive_ready.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/relay_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/relay_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/restore_dimmer.py` & `velbus-aio-2024.4.1/velbusaio/messages/restore_dimmer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/select_program.py` & `velbus-aio-2024.4.1/velbusaio/messages/select_program.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/sensor_settings_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/sensor_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/sensor_temp_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/sensor_temp_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/sensor_temperature.py` & `velbus-aio-2024.4.1/velbusaio/messages/sensor_temperature.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/set_date.py` & `velbus-aio-2024.4.1/velbusaio/messages/set_date.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
 
 from __future__ import annotations
 
-import time
-
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xB7
 
 
 @register(COMMAND_CODE)
 class SetDate(Message):
     """
     received by all modules
     """
 
-    def __init__(self, address=0x00) -> None:
+    def __init__(self, address=0x00, day=None, mon=None, year=None) -> None:
         Message.__init__(self)
-        self._day = None
-        self._mon = None
-        self._year = None
+        self._day = day
+        self._mon = mon
+        self._year = year
         self.set_defaults(address)
 
     def set_defaults(self, address) -> None:
         if address is not None:
             self.set_address(address)
         self.set_low_priority()
         self.set_no_rtr()
-        lclt = time.localtime()
-        self._day = lclt[2]
-        self._mon = lclt[1]
-        self._year = lclt[0]
 
     def populate(self, priority, address, rtr, data) -> None:
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/set_daylight_saving.py` & `velbus-aio-2024.4.1/velbusaio/messages/set_daylight_saving.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
 
 from __future__ import annotations
 
-import time
-
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xAF
 
 
 @register(COMMAND_CODE)
 class SetDaylightSaving(Message):
     """
     received by all modules
     """
 
-    def __init__(self, address=0x00) -> None:
+    def __init__(self, address=0x00, ds=None) -> None:
         Message.__init__(self)
-        self._ds = None
+        self._ds = ds
         self.set_defaults(address)
 
     def set_defaults(self, address) -> None:
         if address is not None:
             self.set_address(address)
         self.set_low_priority()
         self.set_no_rtr()
-        lclt = time.localtime()
-        self._ds = not lclt[8]
 
     def populate(self, priority, address, rtr, data) -> None:
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/set_dimmer.py` & `velbus-aio-2024.4.1/velbusaio/messages/set_dimmer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/set_led.py` & `velbus-aio-2024.4.1/velbusaio/messages/set_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/set_realtime_clock.py` & `velbus-aio-2024.4.1/velbusaio/messages/switch_relay_off.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,45 @@
 """
-:author: Maikel Punie <maikel.punie@gmail.com>
+:author: Thomas Delaet <thomas@delaet.org>
 """
 
 from __future__ import annotations
 
-import time
-
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xD8
+COMMAND_CODE = 0x01
 
 
 @register(COMMAND_CODE)
-class SetRealtimeClock(Message):
+class SwitchRelayOffMessage(Message):
     """
-    received by all modules
+    send by:
+    received by: VMB4RYLD
     """
 
-    def __init__(self, address=0x00) -> None:
+    def __init__(self, address=None):
         Message.__init__(self)
-        self._wday = None
-        self._hour = None
-        self._min = None
+        self.relay_channels = []
         self.set_defaults(address)
 
-    def set_defaults(self, address) -> None:
-        if address is not None:
-            self.set_address(address)
-        self.set_low_priority()
-        self.set_no_rtr()
-        lclt = time.localtime()
-        self._wday = lclt[6]
-        self._hour = lclt[3]
-        self._min = lclt[4]
-
-    def populate(self, priority, address, rtr, data) -> None:
+    def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
-        self.needs_low_priority(priority)
+        self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 3)
+        self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
-        self._wday = data[0]
-        self._hour = data[1]
-        self._min = data[2]
+        self.relay_channels = self.byte_to_channels(data[0])
+
+    def set_defaults(self, address):
+        if address is not None:
+            self.set_address(address)
+        self.set_high_priority()
+        self.set_no_rtr()
 
-    def data_to_binary(self) -> bytes:
+    def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self._wday, self._hour, self._min])
+        return bytes([COMMAND_CODE, self.channels_to_byte(self.relay_channels)])
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/set_temperature.py` & `velbus-aio-2024.4.1/velbusaio/messages/set_temperature.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/slider_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/slider_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/slow_blinking_led.py` & `velbus-aio-2024.4.1/velbusaio/messages/slow_blinking_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/start_relay_blinking_timer.py` & `velbus-aio-2024.4.1/velbusaio/messages/start_relay_blinking_timer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/start_relay_timer.py` & `velbus-aio-2024.4.1/velbusaio/messages/start_relay_timer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/switch_relay_off.py` & `velbus-aio-2024.4.1/velbusaio/messages/switch_relay_on.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 """
 
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0x01
+COMMAND_CODE = 0x02
 
 
 @register(COMMAND_CODE)
-class SwitchRelayOffMessage(Message):
+class SwitchRelayOnMessage(Message):
     """
     send by:
     received by: VMB4RYLD
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
         self.relay_channels = []
         self.set_defaults(address)
 
+    def set_defaults(self, address):
+        if address is not None:
+            self.set_address(address)
+        self.set_high_priority()
+        self.set_no_rtr()
+
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
         self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
         self.relay_channels = self.byte_to_channels(data[0])
 
-    def set_defaults(self, address):
-        if address is not None:
-            self.set_address(address)
-        self.set_high_priority()
-        self.set_no_rtr()
-
     def data_to_binary(self):
         """
         :return: bytes
         """
         return bytes([COMMAND_CODE, self.channels_to_byte(self.relay_channels)])
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/switch_relay_on.py` & `velbus-aio-2024.4.1/velbusaio/messages/very_fast_blinking_led.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,43 +3,37 @@
 """
 
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0x02
+COMMAND_CODE = 0xF9
 
 
 @register(COMMAND_CODE)
-class SwitchRelayOnMessage(Message):
+class VeryFastBlinkingLedMessage(Message):
     """
-    send by:
-    received by: VMB4RYLD
+    send by: VMB4RYLD
+    received by: VMB6IN
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
-        self.relay_channels = []
+        self.leds = []
         self.set_defaults(address)
 
-    def set_defaults(self, address):
-        if address is not None:
-            self.set_address(address)
-        self.set_high_priority()
-        self.set_no_rtr()
-
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
-        self.needs_high_priority(priority)
+        self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
-        self.relay_channels = self.byte_to_channels(data[0])
+        self.leds = self.byte_to_channels(data[0])
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self.channels_to_byte(self.relay_channels)])
+        return bytes([COMMAND_CODE, self.channels_to_byte(self.leds)])
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/switch_to_comfort.py` & `velbus-aio-2024.4.1/velbusaio/messages/switch_to_comfort.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/switch_to_day.py` & `velbus-aio-2024.4.1/velbusaio/messages/switch_to_day.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/switch_to_night.py` & `velbus-aio-2024.4.1/velbusaio/messages/switch_to_night.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/switch_to_safe.py` & `velbus-aio-2024.4.1/velbusaio/messages/switch_to_safe.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part1.py` & `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part1.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part2.py` & `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part2.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part3.py` & `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part3.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part4.py` & `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part4.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_request.py` & `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/temp_set_cooling.py` & `velbus-aio-2024.4.1/velbusaio/messages/temp_set_cooling.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/temp_set_heating.py` & `velbus-aio-2024.4.1/velbusaio/messages/temp_set_heating.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/update_led_status.py` & `velbus-aio-2024.4.1/velbusaio/messages/update_led_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/very_fast_blinking_led.py` & `velbus-aio-2024.4.1/velbusaio/messages/write_memory_block.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,37 +3,41 @@
 """
 
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xF9
+COMMAND_CODE = 0xCA
 
 
 @register(COMMAND_CODE)
-class VeryFastBlinkingLedMessage(Message):
+class WriteMemoryBlockMessage(Message):
     """
-    send by: VMB4RYLD
-    received by: VMB6IN
+    send by:
+    received by: VMB4RYLD
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
-        self.leds = []
+        self.high_address = 0x00
+        self.low_address = 0x00
+        self.data = ""
         self.set_defaults(address)
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 1)
+        self.needs_data(data, 6)
         self.set_attributes(priority, address, rtr)
-        self.leds = self.byte_to_channels(data[0])
+        self.high_address = data[0]
+        self.low_address = data[1]
+        self.data = data[2:]
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self.channels_to_byte(self.leds)])
+        return bytes([COMMAND_CODE, self.high_address, self.low_address] + self.data)
```

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/write_data_to_memory.py` & `velbus-aio-2024.4.1/velbusaio/messages/write_data_to_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/messages/write_module_address_and_serial_number.py` & `velbus-aio-2024.4.1/velbusaio/messages/write_module_address_and_serial_number.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/module.py` & `velbus-aio-2024.4.1/velbusaio/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 This represents a velbus module
 """
 
 from __future__ import annotations
 
 import logging
-import os
 import pathlib
-import pickle
 import struct
 import sys
+import json
 from typing import Awaitable, Callable
 
 from velbusaio.channels import (
     Blind,
     Button,
     ButtonCounter,
     Channel,
@@ -33,15 +32,15 @@
     CHANNEL_LIGHT_VALUE,
     CHANNEL_MEMO_TEXT,
     CHANNEL_SELECTED_PROGRAM,
     PRIORITY_LOW,
 )
 from velbusaio.helpers import handle_match, keys_exists
 from velbusaio.message import Message
-from velbusaio.messages import DaliDeviceSettingMsg
+from velbusaio.messages.dali_device_settings import DaliDeviceSettingMsg
 from velbusaio.messages.blind_status import BlindStatusMessage, BlindStatusNgMessage
 from velbusaio.messages.channel_name_part1 import (
     ChannelNamePart1Message,
     ChannelNamePart1Message2,
     ChannelNamePart1Message3,
 )
 from velbusaio.messages.channel_name_part2 import (
@@ -77,16 +76,14 @@
 from velbusaio.messages.module_status import (
     ModuleStatusGP4PirMessage,
     ModuleStatusMessage,
     ModuleStatusMessage2,
     ModuleStatusPirMessage,
 )
 from velbusaio.messages.module_status_request import ModuleStatusRequestMessage
-from velbusaio.messages.module_subtype import ModuleSubTypeMessage
-from velbusaio.messages.module_type import ModuleTypeMessage, ModuleType2Message
 from velbusaio.messages.push_button_status import PushButtonStatusMessage
 from velbusaio.messages.read_data_from_memory import ReadDataFromMemoryMessage
 from velbusaio.messages.relay_status import RelayStatusMessage, RelayStatusMessage2
 from velbusaio.messages.sensor_temperature import SensorTemperatureMessage
 from velbusaio.messages.set_led import SetLedMessage
 from velbusaio.messages.slider_status import SliderStatusMessage
 from velbusaio.messages.slow_blinking_led import SlowBlinkingLedMessage
@@ -184,41 +181,38 @@
                 for i in range(((sub * 8) + 1), (((sub + 1) * 8) + 1)):
                     if i in self._channels and not isinstance(
                         self._channels[i], TemperatureChannelType
                     ):
                         del self._channels[i]
 
     def _cache(self) -> None:
-        cfile = pathlib.Path(f"{self._cache_dir}/{self._address}.p")
-        with cfile.open("wb") as fl:
-            pickle.dump(self, fl)
+        cfile = pathlib.Path(f"{self._cache_dir}/{self._address}.json")
+        with cfile.open("w") as fl:
+            json.dump(self.to_cache(), fl, indent=4)
 
     def __getstate__(self) -> dict:
         d = self.__dict__
         self_dict = {k: d[k] for k in d if k != "_writer" and k != "_log"}
         return self_dict
 
     def __setstate__(self, state: dict) -> None:
         self.__dict__ = state
 
     def __repr__(self) -> str:
-        return (
-            "<{}: {{{}}} @ {{{}}} loaded:{{{}}} loading:{{{}}} channels{{:{}}}>".format(
-                self._name,
-                self._type,
-                self._address,
-                self.loaded,
-                self._is_loading,
-                self._channels,
-            )
-        )
+        return f"<{self._name} type:{self._type} address:{self._address} loaded:{self.loaded} loading:{self._is_loading} channels: {self._channels}>"
 
     def __str__(self) -> str:
         return self.__repr__()
 
+    def to_cache(self) -> dict:
+        d = {"name": self._name, "channels": {}}
+        for num, chan in self._channels.items():
+            d["channels"][num] = chan.to_cache()
+        return d
+
     def get_addresses(self) -> list:
         """
         Get all addresses for this module
         """
         res = []
         res.append(self._address)
         for addr in self._sub_address.values():
@@ -228,29 +222,26 @@
     def get_type(self) -> int:
         """
         Get the module type
         """
         return self._type
 
     def get_type_name(self) -> str:
-        return self._data["Type"]
+        if "Type" in self._data:
+            return self._data["Type"]
+        return "UNKNOWN"
 
     def get_serial(self) -> str | None:
         return self.serial
 
     def get_name(self) -> str:
         return self._name
 
     def get_sw_version(self) -> str:
-        return "{}-{}.{}.{}".format(
-            self.serial,
-            self.memory_map_version,
-            self.build_year,
-            self.build_week,
-        )
+        return f"{self.serial}-{self.memory_map_version}.{self.build_year}.{self.build_week}"
 
     def calc_channel_offset(self, address: int) -> int:
         _channel_offset = 0
         if self._address != address:
             for _sub_addr_key, _sub_addr_val in self._sub_address.items():
                 if _sub_addr_val == address:
                     _channel_offset = 8 * _sub_addr_key
@@ -545,22 +536,37 @@
         if self._is_loading or self.loaded:
             if from_cache:
                 await self._request_module_status()
             return
         self._log.info("Load Module")
         # start the loading
         self._is_loading = True
+        # see if we have a cache
+        try:
+            cfile = pathlib.Path(f"{self._cache_dir}/{self._address}.json")
+            with cfile.open("r") as fl:
+                cache = json.load(fl)
+        except OSError:
+            cache = {}
         # load default channels
         await self.__load_default_channels()
         # load the data from memory ( the stuff that we need)
-        await self.__load_memory()
+        if "name" in cache and cache["name"] != "":
+            self._name = cache["name"]
+        else:
+            await self.__load_memory()
         # load the module status
         await self._request_module_status()
         # load the channel names
-        await self._request_channel_name()
+        if "channels" in cache:
+            for num, chan in cache["channels"].items():
+                self._channels[int(num)]._name = chan["name"]
+                self._channels[int(num)]._is_loaded = True
+        else:
+            await self._request_channel_name()
         # load the module specific stuff
         self._load()
         # stop the loading
         self._is_loading = False
 
     def _load(self) -> None:
         """
```

### Comparing `velbus-aio-2024.4.0/velbusaio/protocol.json` & `velbus-aio-2024.4.1/velbusaio/protocol.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985495780590719%*

 * *Differences: {"'ModuleTypes'": "{'45': {'Type': 'VMBDALI-20'}, '4F': {'Type': 'VMBEL1-20'}, '50': {'Type': "*

 * *                  "'VMBEL2-20'}, '51': {'Type': 'VMBEL4-20'}, '52': {'Type': 'VMBELO-20'}}"}*

```diff
@@ -10808,15 +10808,15 @@
                 }
             },
             "Info": "4 button interface module",
             "Type": "VMB4PB"
         },
         "45": {
             "Info": "VMBDALI-20 DALI gateway module",
-            "Type": "VMBDALI"
+            "Type": "VMBDALI-20"
         },
         "48": {
             "Channels": {
                 "01": {
                     "Editable": "yes",
                     "Name": "Relay 1",
                     "Type": "Relay"
@@ -11889,15 +11889,16 @@
                 },
                 "97": {
                     "Name": "Edge Lit",
                     "Type": "EdgeLit"
                 }
             },
             "TemperatureChannel": "09",
-            "ThermostatAddr": "0"
+            "ThermostatAddr": "0",
+            "Type": "VMBEL1-20"
         },
         "50": {
             "AllChannelStatus": "FF",
             "ChannelNumbers": {
                 "Name": {
                     "Convert": "hex"
                 }
@@ -11977,15 +11978,16 @@
                 },
                 "97": {
                     "Name": "Edge Lit",
                     "Type": "EdgeLit"
                 }
             },
             "TemperatureChannel": "09",
-            "ThermostatAddr": "0"
+            "ThermostatAddr": "0",
+            "Type": "VMBEL2-20"
         },
         "51": {
             "AllChannelStatus": "FF",
             "ChannelNumbers": {
                 "Name": {
                     "Convert": "hex"
                 }
@@ -12065,15 +12067,16 @@
                 },
                 "97": {
                     "Name": "Edge Lit",
                     "Type": "EdgeLit"
                 }
             },
             "TemperatureChannel": "09",
-            "ThermostatAddr": "0"
+            "ThermostatAddr": "0",
+            "Type": "VMBEL4-20"
         },
         "52": {
             "AllChannelStatus": "FF",
             "ChannelNumbers": {
                 "Name": {
                     "Convert": "hex"
                 }
@@ -12253,15 +12256,16 @@
                 },
                 "98": {
                     "Name": "Memo Text",
                     "Type": "Memo"
                 }
             },
             "TemperatureChannel": "33",
-            "ThermostatAddr": "3"
+            "ThermostatAddr": "3",
+            "Type": "VMBELO-20"
         },
         "54": {
             "Info": "1 Button Touch panel",
             "Type": "VMBGP1-20"
         },
         "55": {
             "Info": "2 Button Touch panel",
```

### Comparing `velbus-aio-2024.4.0/velbusaio/protocol.py` & `velbus-aio-2024.4.1/velbusaio/protocol.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/raw_message.py` & `velbus-aio-2024.4.1/velbusaio/raw_message.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.0/velbusaio/util.py` & `velbus-aio-2024.4.1/velbusaio/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Some common utils.
+"""
+
 from typing import Union
 
 from velbusaio.const import MAXIMUM_MESSAGE_SIZE, MINIMUM_MESSAGE_SIZE
 
 
 # Copyright (c) 2017 Thomas Delaet
 # Copied from python-velbus (https://github.com/thomasdelaet/python-velbus)
```

