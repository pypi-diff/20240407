# Comparing `tmp/bacpypes3-0.0.86.tar.gz` & `tmp/bacpypes3-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacpypes3-0.0.86.tar", last modified: Mon Dec 11 01:32:00 2023, max compression
+gzip compressed data, was "bacpypes3-0.0.91.tar", last modified: Sat Apr  6 22:32:29 2024, max compression
```

## Comparing `bacpypes3-0.0.86.tar` & `bacpypes3-0.0.91.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.382958 bacpypes3-0.0.86/
--rw-r--r--   0 joel      (1000) joel      (1000)      666 2023-12-11 01:32:00.382958 bacpypes3-0.0.86/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.86/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.366958 bacpypes3-0.0.86/bacpypes3/
--rw-rw-r--   0 joel      (1000) joel      (1000)     1391 2023-12-11 01:30:51.000000 bacpypes3-0.0.86/bacpypes3/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    25537 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/bacpypes3/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    56670 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/bacpypes3/apdu.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    34476 2023-11-12 13:48:48.000000 bacpypes3-0.0.86/bacpypes3/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    65965 2023-10-31 15:46:12.000000 bacpypes3-0.0.86/bacpypes3/appservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    20848 2023-05-31 11:51:39.000000 bacpypes3-0.0.86/bacpypes3/argparse.py
--rw-rw-r--   0 joel      (1000) joel      (1000)   103270 2023-11-12 13:48:48.000000 bacpypes3-0.0.86/bacpypes3/basetypes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16296 2023-10-14 01:56:06.000000 bacpypes3-0.0.86/bacpypes3/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.86/bacpypes3/comm.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.86/bacpypes3/console.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    64628 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/bacpypes3/constructeddata.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.86/bacpypes3/debugging.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.86/bacpypes3/errors.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.370957 bacpypes3-0.0.86/bacpypes3/ipv4/
--rw-rw-r--   0 joel      (1000) joel      (1000)     9245 2023-06-26 19:19:16.000000 bacpypes3-0.0.86/bacpypes3/ipv4/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.86/bacpypes3/ipv4/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.86/bacpypes3/ipv4/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.86/bacpypes3/ipv4/link.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.86/bacpypes3/ipv4/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.370957 bacpypes3-0.0.86/bacpypes3/ipv6/
--rw-rw-r--   0 joel      (1000) joel      (1000)     6298 2023-01-09 14:29:42.000000 bacpypes3-0.0.86/bacpypes3/ipv6/__init__.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.86/bacpypes3/ipv6/bvll.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.86/bacpypes3/ipv6/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.370957 bacpypes3-0.0.86/bacpypes3/json/
--rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.86/bacpypes3/json/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.86/bacpypes3/json/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/bacpypes3/json/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.370957 bacpypes3-0.0.86/bacpypes3/lib/
--rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.86/bacpypes3/lib/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    15883 2023-11-13 00:20:14.000000 bacpypes3-0.0.86/bacpypes3/lib/batchread.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.374958 bacpypes3-0.0.86/bacpypes3/local/
--rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/bacpypes3/local/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5804 2023-06-21 18:50:45.000000 bacpypes3-0.0.86/bacpypes3/local/analog.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4447 2023-06-21 18:50:45.000000 bacpypes3-0.0.86/bacpypes3/local/binary.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.86/bacpypes3/local/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.86/bacpypes3/local/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.86/bacpypes3/local/device.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    87515 2023-06-26 19:19:16.000000 bacpypes3-0.0.86/bacpypes3/local/event.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.86/bacpypes3/local/fault.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.86/bacpypes3/local/networkport.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.86/bacpypes3/local/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.86/bacpypes3/local/oos.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    24849 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/bacpypes3/local/schedule.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    77562 2023-07-03 03:39:30.000000 bacpypes3-0.0.86/bacpypes3/netservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.86/bacpypes3/npdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    91107 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/bacpypes3/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    65850 2023-06-26 19:19:16.000000 bacpypes3-0.0.86/bacpypes3/pdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    93426 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/bacpypes3/primitivedata.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.374958 bacpypes3-0.0.86/bacpypes3/rdf/
--rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.86/bacpypes3/rdf/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.86/bacpypes3/rdf/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10774 2023-12-11 01:30:51.000000 bacpypes3-0.0.86/bacpypes3/rdf/core.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-12-11 01:30:51.000000 bacpypes3-0.0.86/bacpypes3/rdf/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.374958 bacpypes3-0.0.86/bacpypes3/sc/
--rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/bacpypes3/sc/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/bacpypes3/sc/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.86/bacpypes3/sc/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.374958 bacpypes3-0.0.86/bacpypes3/service/
--rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.86/bacpypes3/service/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22864 2023-10-31 15:28:33.000000 bacpypes3-0.0.86/bacpypes3/service/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23249 2023-09-15 04:35:23.000000 bacpypes3-0.0.86/bacpypes3/service/device.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    37038 2023-11-12 13:48:48.000000 bacpypes3-0.0.86/bacpypes3/service/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.86/bacpypes3/settings.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3854 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/bacpypes3/vendor.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.374958 bacpypes3-0.0.86/bacpypes3/vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.86/bacpypes3/vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.86/bacpypes3/vlan/link.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.370957 bacpypes3-0.0.86/bacpypes3.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)      666 2023-12-11 01:32:00.000000 bacpypes3-0.0.86/bacpypes3.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     3069 2023-12-11 01:32:00.000000 bacpypes3-0.0.86/bacpypes3.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-12-11 01:32:00.000000 bacpypes3-0.0.86/bacpypes3.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.86/bacpypes3.egg-info/not-zip-safe
--rw-rw-r--   0 joel      (1000) joel      (1000)       16 2023-12-11 01:32:00.000000 bacpypes3-0.0.86/bacpypes3.egg-info/top_level.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      101 2023-10-23 02:32:34.000000 bacpypes3-0.0.86/pyproject.toml
--rw-rw-r--   0 joel      (1000) joel      (1000)       38 2023-12-11 01:32:00.382958 bacpypes3-0.0.86/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.86/setup.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.374958 bacpypes3-0.0.86/tests/
--rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/clocked_test.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/conftest.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/state_machine.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_1.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test__template.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.378958 bacpypes3-0.0.86/tests/test_constructed_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_constructed_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_constructed_data/test_any.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_constructed_data/test_array.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_constructed_data/test_choice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_constructed_data/test_list.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_constructed_data/test_read_property_multiple.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_constructed_data/test_sequence.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_constructed_data/test_sequence_of.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.378958 bacpypes3-0.0.86/tests/test_pdu/
--rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_pdu/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16509 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_pdu/test_address.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_pdu/test_pci.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_pdu/test_pdu.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.378958 bacpypes3-0.0.86/tests/test_primitive_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_bit_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_boolean.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_character_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2671 2023-02-17 06:25:03.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_date.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_double.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_enumerated.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_integer.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_null.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_object_identifier.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_octet_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_real.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_tag.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_time.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.86/tests/test_primitive_data/test_unsigned.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.378958 bacpypes3-0.0.86/tests/test_utilities/
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_utilities/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_utilities/test_state_machine.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-12-11 01:32:00.382958 bacpypes3-0.0.86/tests/test_vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_vlan/test_ipv4_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_vlan/test_ipv4_router.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/test_vlan/test_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/trapped_classes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.86/tests/utilities.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.130368 bacpypes3-0.0.91/
+-rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-04-06 22:32:29.130368 bacpypes3-0.0.91/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.91/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.114368 bacpypes3-0.0.91/bacpypes3/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1391 2024-03-31 21:04:35.000000 bacpypes3-0.0.91/bacpypes3/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    25537 2023-10-23 02:32:34.000000 bacpypes3-0.0.91/bacpypes3/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    56670 2023-10-23 02:32:34.000000 bacpypes3-0.0.91/bacpypes3/apdu.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    34748 2024-03-21 12:00:37.000000 bacpypes3-0.0.91/bacpypes3/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    65965 2023-10-31 15:46:12.000000 bacpypes3-0.0.91/bacpypes3/appservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    21688 2024-03-31 21:04:35.000000 bacpypes3-0.0.91/bacpypes3/argparse.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)   103597 2024-03-31 21:04:35.000000 bacpypes3-0.0.91/bacpypes3/basetypes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16296 2023-10-14 01:56:06.000000 bacpypes3-0.0.91/bacpypes3/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.91/bacpypes3/comm.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.91/bacpypes3/console.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    64628 2023-10-23 02:32:34.000000 bacpypes3-0.0.91/bacpypes3/constructeddata.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.91/bacpypes3/debugging.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.91/bacpypes3/errors.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.118368 bacpypes3-0.0.91/bacpypes3/ipv4/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9911 2024-01-20 06:39:19.000000 bacpypes3-0.0.91/bacpypes3/ipv4/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.91/bacpypes3/ipv4/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.91/bacpypes3/ipv4/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.91/bacpypes3/ipv4/link.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.91/bacpypes3/ipv4/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.118368 bacpypes3-0.0.91/bacpypes3/ipv6/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6919 2024-01-20 06:39:19.000000 bacpypes3-0.0.91/bacpypes3/ipv6/__init__.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.91/bacpypes3/ipv6/bvll.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.91/bacpypes3/ipv6/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.118368 bacpypes3-0.0.91/bacpypes3/json/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.91/bacpypes3/json/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.91/bacpypes3/json/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/bacpypes3/json/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.118368 bacpypes3-0.0.91/bacpypes3/lib/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.91/bacpypes3/lib/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    15883 2023-11-13 00:20:14.000000 bacpypes3-0.0.91/bacpypes3/lib/batchread.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.118368 bacpypes3-0.0.91/bacpypes3/local/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-10-23 02:32:34.000000 bacpypes3-0.0.91/bacpypes3/local/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5836 2024-03-21 05:28:34.000000 bacpypes3-0.0.91/bacpypes3/local/analog.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4696 2024-03-21 05:28:34.000000 bacpypes3-0.0.91/bacpypes3/local/binary.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.91/bacpypes3/local/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.91/bacpypes3/local/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.91/bacpypes3/local/device.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    89092 2024-03-31 21:04:35.000000 bacpypes3-0.0.91/bacpypes3/local/event.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.91/bacpypes3/local/fault.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1998 2024-03-21 05:28:34.000000 bacpypes3-0.0.91/bacpypes3/local/multistate.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.91/bacpypes3/local/networkport.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.91/bacpypes3/local/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.91/bacpypes3/local/oos.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    24849 2023-10-23 02:32:34.000000 bacpypes3-0.0.91/bacpypes3/local/schedule.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    82059 2024-03-31 21:04:35.000000 bacpypes3-0.0.91/bacpypes3/netservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.91/bacpypes3/npdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    91152 2024-03-21 05:28:34.000000 bacpypes3-0.0.91/bacpypes3/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    66217 2024-03-31 21:04:35.000000 bacpypes3-0.0.91/bacpypes3/pdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    93426 2023-10-23 02:32:34.000000 bacpypes3-0.0.91/bacpypes3/primitivedata.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.122368 bacpypes3-0.0.91/bacpypes3/rdf/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.91/bacpypes3/rdf/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.91/bacpypes3/rdf/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10764 2024-04-02 15:17:43.000000 bacpypes3-0.0.91/bacpypes3/rdf/core.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-12-11 01:30:51.000000 bacpypes3-0.0.91/bacpypes3/rdf/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.122368 bacpypes3-0.0.91/bacpypes3/sc/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/bacpypes3/sc/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/bacpypes3/sc/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.91/bacpypes3/sc/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.122368 bacpypes3-0.0.91/bacpypes3/service/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.91/bacpypes3/service/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22864 2023-10-31 15:28:33.000000 bacpypes3-0.0.91/bacpypes3/service/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23249 2023-09-15 04:35:23.000000 bacpypes3-0.0.91/bacpypes3/service/device.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    40398 2024-03-21 12:00:37.000000 bacpypes3-0.0.91/bacpypes3/service/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.91/bacpypes3/settings.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3854 2023-10-23 02:32:34.000000 bacpypes3-0.0.91/bacpypes3/vendor.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.122368 bacpypes3-0.0.91/bacpypes3/vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.91/bacpypes3/vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.91/bacpypes3/vlan/link.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.126368 bacpypes3-0.0.91/bacpypes3.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-04-06 22:32:29.000000 bacpypes3-0.0.91/bacpypes3.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3099 2024-04-06 22:32:29.000000 bacpypes3-0.0.91/bacpypes3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2024-04-06 22:32:29.000000 bacpypes3-0.0.91/bacpypes3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.91/bacpypes3.egg-info/not-zip-safe
+-rw-rw-r--   0 joel      (1000) joel      (1000)       16 2024-04-06 22:32:29.000000 bacpypes3-0.0.91/bacpypes3.egg-info/top_level.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      101 2023-10-23 02:32:34.000000 bacpypes3-0.0.91/pyproject.toml
+-rw-rw-r--   0 joel      (1000) joel      (1000)       38 2024-04-06 22:32:29.130368 bacpypes3-0.0.91/setup.cfg
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.91/setup.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.122368 bacpypes3-0.0.91/tests/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/clocked_test.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/conftest.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/state_machine.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_1.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test__template.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.126368 bacpypes3-0.0.91/tests/test_constructed_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_constructed_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_constructed_data/test_any.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_constructed_data/test_array.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_constructed_data/test_choice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_constructed_data/test_list.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_constructed_data/test_read_property_multiple.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_constructed_data/test_sequence.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_constructed_data/test_sequence_of.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.126368 bacpypes3-0.0.91/tests/test_pdu/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_pdu/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16956 2024-03-31 21:04:35.000000 bacpypes3-0.0.91/tests/test_pdu/test_address.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_pdu/test_pci.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_pdu/test_pdu.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.126368 bacpypes3-0.0.91/tests/test_primitive_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_bit_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_boolean.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_character_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2671 2023-02-17 06:25:03.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_date.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_double.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_enumerated.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_integer.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_null.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_object_identifier.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_octet_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_real.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_tag.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_time.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.91/tests/test_primitive_data/test_unsigned.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.126368 bacpypes3-0.0.91/tests/test_utilities/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_utilities/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_utilities/test_state_machine.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-06 22:32:29.126368 bacpypes3-0.0.91/tests/test_vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_vlan/test_ipv4_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_vlan/test_ipv4_router.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/test_vlan/test_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/trapped_classes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.91/tests/utilities.py
```

### Comparing `bacpypes3-0.0.86/PKG-INFO` & `bacpypes3-0.0.91/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.86
+Version: 0.0.91
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.86/bacpypes3/__init__.py` & `bacpypes3-0.0.91/bacpypes3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 if _sys.platform not in _supported_platforms:
     _warnings.warn("unsupported platform", RuntimeWarning)
 
 #
 #   Project Metadata
 #
 
-__version__ = "0.0.86"
+__version__ = "0.0.91"
 __author__ = "Joel Bender"
 __email__ = "joel@carrickbender.com"
 
 #
 #   Settings and Debugging
 #
```

### Comparing `bacpypes3-0.0.86/bacpypes3/__main__.py` & `bacpypes3-0.0.91/bacpypes3/__main__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/apdu.py` & `bacpypes3-0.0.91/bacpypes3/apdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/app.py` & `bacpypes3-0.0.91/bacpypes3/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,101 +1,82 @@
 """
 Application Module
 """
 
 from __future__ import annotations
 
-import asyncio
 import argparse
+import asyncio
 import dataclasses
-
 from functools import partial
+from typing import TYPE_CHECKING
+from typing import Any as _Any
+from typing import Callable, Dict, List, Optional, Set, Tuple, Union, cast
 
-from typing import (
-    TYPE_CHECKING,
-    cast,
-    Any as _Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Set,
-    Union,
-)
-
-from .debugging import bacpypes_debugging, DebugContents, ModuleLogger
-
-from .comm import ApplicationServiceElement, bind
-from .pdu import Address
-
+# for computing protocol services supported
 from .apdu import (
     APDU,
-    UnconfirmedRequestPDU,
-    ConfirmedRequestPDU,
-    SimpleAckPDU,
+    AbortPDU,
     ComplexAckPDU,
+    ConfirmedRequestPDU,
+    ConfirmedServiceChoice,
+    Error,
     ErrorPDU,
+    IAmRequest,
     RejectPDU,
-    AbortPDU,
-    Error,
-)
-
-from .errors import ExecutionError, UnrecognizedService, AbortException, RejectException
-
-# for computing protocol services supported
-from .apdu import (
+    SimpleAckPDU,
+    UnconfirmedRequestPDU,
     confirmed_request_types,
     unconfirmed_request_types,
-    IAmRequest,
 )
-from .primitivedata import ObjectType, ObjectIdentifier
+from .appservice import ApplicationServiceAccessPoint
 from .basetypes import (
+    BDTEntry,
+    HostNPort,
+    IPMode,
+    NetworkType,
+    ProtocolLevel,
     Segmentation,
     ServicesSupported,
-    ProtocolLevel,
-    NetworkType,
-    IPMode,
-    HostNPort,
-    BDTEntry,
 )
-from .object import Object, DeviceObject
-from .vendor import get_vendor_info
+from .comm import ApplicationServiceElement, bind
+from .debugging import DebugContents, ModuleLogger, bacpypes_debugging
+from .errors import AbortException, ExecutionError, RejectException, UnrecognizedService
+from .ipv4.link import BBMDLinkLayer as BBMDLinkLayer_ipv4
+from .ipv4.link import ForeignLinkLayer as ForeignLinkLayer_ipv4
+from .ipv4.link import NormalLinkLayer as NormalLinkLayer_ipv4
 
-from .appservice import ApplicationServiceAccessPoint
+# for serialized parameter initialization
+from .json import json_to_sequence
+
+# network port interpretation
+from .local.networkport import NetworkPortObject
+
+# objects with specialized interpreters
+from .local.schedule import ScheduleObject
 from .netservice import (
     NetworkServiceAccessPoint,
     NetworkServiceElement,
     RouterInfoCache,
 )
+from .object import DeviceObject, Object
+from .pdu import Address
+from .primitivedata import ObjectIdentifier, ObjectType
+from .service.cov import ChangeOfValueServices
 
 # basic services
-from .service.device import WhoIsIAmServices, WhoHasIHaveServices
+from .service.device import WhoHasIHaveServices, WhoIsIAmServices
 from .service.object import (
     ReadRangeServices,
-    ReadWritePropertyServices,
     ReadWritePropertyMultipleServices,
+    ReadWritePropertyServices,
 )
-from .service.cov import ChangeOfValueServices
-
-# network port interpretation
-from .local.networkport import NetworkPortObject
-from .ipv4.link import (
-    NormalLinkLayer as NormalLinkLayer_ipv4,
-    ForeignLinkLayer as ForeignLinkLayer_ipv4,
-    BBMDLinkLayer as BBMDLinkLayer_ipv4,
-)
+from .vendor import get_vendor_info
 from .vlan.link import VirtualLinkLayer
 
-# objects with specialized interpreters
-from .local.schedule import ScheduleObject
-
-# for serialized parameter initialization
-from .json import json_to_sequence
-
 if TYPE_CHECKING:
     # class is declared as generic in stubs but not at runtime
     APDUFuture = asyncio.Future[Optional[APDU]]
 else:
     APDUFuture = asyncio.Future
 
 # some debugging
@@ -499,15 +480,15 @@
                 args,
                 device_info_cache,
                 aseID,
             )
 
         # get the vendor info for the provided identifier
         vendor_info = get_vendor_info(args.vendoridentifier)
-        if not vendor_info:
+        if vendor_info.vendor_identifier == 0:
             raise RuntimeError(f"missing vendor info: {args.vendoridentifier}")
 
         # get the device object class and make an instance
         device_object_class = vendor_info.get_object_class(ObjectType.device)
         if not device_object_class:
             raise RuntimeError(
                 f"vendor indentifier {args.vendoridentifier} missing device object class"
@@ -754,21 +735,25 @@
 
         services_supported = ServicesSupported([])
 
         # look through the confirmed services
         for service_choice, service_request_class in confirmed_request_types.items():
             service_helper = "do_" + service_request_class.__name__
             if hasattr(self, service_helper):
-                services_supported[service_choice] = 1
+                _key = ConfirmedServiceChoice(service_choice).attr
+                choice = getattr(services_supported, _key)
+                services_supported[choice] = 1
 
         # look through the unconfirmed services
         for service_choice, service_request_class in unconfirmed_request_types.items():
             service_helper = "do_" + service_request_class.__name__
             if hasattr(self, service_helper):
-                services_supported[service_choice] = 1
+                _key = ConfirmedServiceChoice(service_choice).attr
+                choice = getattr(services_supported, _key)
+                services_supported[choice] = 1
 
         # return the bit list
         return services_supported
 
     # -----
 
     def close(self):
```

### Comparing `bacpypes3-0.0.86/bacpypes3/appservice.py` & `bacpypes3-0.0.91/bacpypes3/appservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/argparse.py` & `bacpypes3-0.0.91/bacpypes3/argparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,39 @@
 )
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
 
+def _getenv(varname: str, default: Any = None) -> Any:
+    """
+    When passing environment variables into a docker build process the value
+    might be an empty string which should be interpreted as not provided.  In
+    the case where a default value is an integer, the string value should be
+    converted to an int.
+    """
+    value = os.getenv(varname)
+    if (value is None) or (value == ""):
+        return default
+    if isinstance(default, int):
+        return int(value)
+    return value
+
+
+# settings
+BACPYPES_DEVICE_NAME = _getenv("BACPYPES_DEVICE_NAME", "Excelsior")
+BACPYPES_DEVICE_INSTANCE = _getenv("BACPYPES_DEVICE_INSTANCE", 999)
+BACPYPES_NETWORK = _getenv("BACPYPES_NETWORK", 0)
+BACPYPES_DEVICE_ADDRESS = _getenv("BACPYPES_DEVICE_ADDRESS")
+BACPYPES_VENDOR_IDENTIFIER = _getenv("BACPYPES_VENDOR_IDENTIFIER", 999)
+BACPYPES_FOREIGN_BBMD = _getenv("BACPYPES_FOREIGN_BBMD")
+BACPYPES_FOREIGN_TTL = _getenv("BACPYPES_FOREIGN_TTL", 30)
+BACPYPES_BBMD_BDT = _getenv("BACPYPES_BBMD_BDT")
+
 # keep track of the logging handlers
 logging_handlers: Dict[logging.Logger, List[logging.StreamHandler]] = {}
 
 
 @bacpypes_debugging
 def create_log_handler(
     logger: Union[str, logging.Logger] = "",
@@ -397,57 +422,57 @@
             SimpleArgumentParser._debug("__init__")
         ArgumentParser.__init__(self, **kwargs)
 
         self.add_argument(
             "--name",
             type=str,
             help="device name",
-            default=os.getenv("BACPYPES_DEVICE_NAME") or "Excelsior",
+            default=BACPYPES_DEVICE_NAME,
         )
         self.add_argument(
             "--instance",
             type=int,
             help="device object instance number, a.k.a., device identifier",
-            default=int(os.getenv("BACPYPES_DEVICE_INSTANCE") or 999),
+            default=BACPYPES_DEVICE_INSTANCE,
         )
         self.add_argument(
             "--network",
             type=int,
             help="local network number",
-            default=int(os.getenv("BACPYPES_NETWORK") or 0),
+            default=BACPYPES_NETWORK,
         )
         self.add_argument(
             "--address",
             type=str,
             help="local network address",
-            default=os.getenv("BACPYPES_DEVICE_ADDRESS"),
+            default=BACPYPES_DEVICE_ADDRESS,
         )
         self.add_argument(
             "--vendoridentifier",
             type=int,
             help="vendor identifier",
-            default=int(os.getenv("BACPYPES_VENDOR_IDENTIFIER") or 999),
+            default=BACPYPES_VENDOR_IDENTIFIER,
         )
         self.add_argument(
             "--foreign",
             type=str,
             help="BBMD address to register as a foreign device",
-            default=os.getenv("BACPYPES_FOREIGN_BBMD"),
+            default=BACPYPES_FOREIGN_BBMD,
         )
         self.add_argument(
             "--ttl",
             type=int,
             help="foreign device subscription time-to-live",
-            default=os.getenv("BACPYPES_FOREIGN_TTL", 30),
+            default=BACPYPES_FOREIGN_TTL,
         )
         self.add_argument(
             "--bbmd",
             nargs="*",
             help="BDT addresses as a BBMD",
-            default=os.getenv("BACPYPES_BBMD_BDT"),
+            default=BACPYPES_BBMD_BDT,
         )
 
     def expand_args(self, result_args: argparse.Namespace) -> None:
         """Expand the arguments and/or update the settings."""
         if _debug:
             SimpleArgumentParser._debug("expand_args %r", result_args)
```

### Comparing `bacpypes3-0.0.86/bacpypes3/basetypes.py` & `bacpypes3-0.0.91/bacpypes3/basetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1878,14 +1878,20 @@
         **kwargs,
     ) -> None:
         if _debug:
             DeviceAddress._debug("DeviceAddress.__init__ %r %r", arg, kwargs)
 
         if arg is None:
             pass
+        elif isinstance(arg, DeviceAddress):
+            if "networkNumber" not in kwargs:
+                kwargs["networkNumber"] = arg.networkNumber
+            kwargs["macAddress"] = arg.macAddress
+        elif isinstance(arg, (bytes, bytearray)):
+            kwargs["macAddress"] = arg
         else:
             if isinstance(arg, str):
                 arg = _Address(arg)
             if not isinstance(arg, _Address):
                 raise TypeError(type(arg))
             if not any(
                 (
@@ -1902,15 +1908,17 @@
         super().__init__(**kwargs)
 
     @classmethod
     def cast(cls, arg):
         if _debug:
             HostAddress._debug("DeviceAddress.cast %r", arg)
 
-        if isinstance(arg, (bytes, bytearray, str, dict, IPv4Address, IPv6Address)):
+        if isinstance(
+            arg, (bytes, bytearray, str, dict, IPv4Address, IPv6Address, DeviceAddress)
+        ):
             return arg
         else:
             raise TypeError(type(arg))
 
 
 _sequence_number = 0
```

### Comparing `bacpypes3-0.0.86/bacpypes3/cmd.py` & `bacpypes3-0.0.91/bacpypes3/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/comm.py` & `bacpypes3-0.0.91/bacpypes3/comm.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/console.py` & `bacpypes3-0.0.91/bacpypes3/console.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/constructeddata.py` & `bacpypes3-0.0.91/bacpypes3/constructeddata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/debugging.py` & `bacpypes3-0.0.91/bacpypes3/debugging.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/errors.py` & `bacpypes3-0.0.91/bacpypes3/errors.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/ipv4/__init__.py` & `bacpypes3-0.0.91/bacpypes3/ipv4/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 from ..pdu import LocalStation, LocalBroadcast, IPv4Address, PDU
 
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
+# move this to settings sometime
+BACPYPES_ENDPOINT_RETRY_INTERVAL = 1.0
+
 
 @bacpypes_debugging
 class IPv4DatagramProtocol(asyncio.DatagramProtocol):
-
     _debug: Callable[..., None]
 
     server: "IPv4DatagramServer"
     destination: Union[IPv4Address, LocalBroadcast, None]
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         if _debug:
@@ -58,15 +60,14 @@
     def connection_lost(self, exc: Optional[Exception]) -> None:
         if _debug:
             IPv4DatagramProtocol._debug("connection_lost %r", exc)
 
 
 @bacpypes_debugging
 class IPv4DatagramServer(Server[PDU]):
-
     _debug: Callable[..., None]
     _exception: Callable[..., None]
     _transport_tasks: List[Any]
 
     local_address: Tuple[str, int]
     local_transport: asyncio.DatagramTransport
     local_protocol: IPv4DatagramProtocol
@@ -94,19 +95,15 @@
 
         # no broadcast if this is an ephemeral port
         if self.local_address[1] == 0:
             no_broadcast = True
 
         # easy call to create a local endpoint
         local_endpoint_task = loop.create_task(
-            loop.create_datagram_endpoint(
-                IPv4DatagramProtocol,
-                local_addr=address.addrTuple,
-                allow_broadcast=True,
-            )
+            self.retrying_create_datagram_endpoint(loop, address.addrTuple)
         )
         if _debug:
             IPv4DatagramServer._debug(
                 "    - local_endpoint_task: %r", local_endpoint_task
             )
         local_endpoint_task.add_done_callback(
             functools.partial(self.set_local_transport_protocol, address)
@@ -126,29 +123,46 @@
                 IPv4DatagramServer._debug(
                     "    - broadcast_address: %r", self.broadcast_address
                 )
 
             # Windows takes care of the broadcast, but Linux needs a broadcast endpoint
             if "nt" not in os.name:
                 broadcast_endpoint_task = loop.create_task(
-                    loop.create_datagram_endpoint(
-                        IPv4DatagramProtocol,
-                        local_addr=address.addrBroadcastTuple,
-                        allow_broadcast=True,
+                    self.retrying_create_datagram_endpoint(
+                        loop, address.addrBroadcastTuple
                     )
                 )
                 if _debug:
                     IPv4DatagramServer._debug(
                         "    - broadcast_endpoint_task: %r", broadcast_endpoint_task
                     )
                 broadcast_endpoint_task.add_done_callback(
                     functools.partial(self.set_broadcast_transport_protocol, address)
                 )
                 self._transport_tasks.append(broadcast_endpoint_task)
 
+    async def retrying_create_datagram_endpoint(
+        self, loop: asyncio.events.AbstractEventLoop, addrTuple: Tuple[str, int]
+    ):
+        """
+        Repeat attempts to create datagram endpoint, sometimes during boot
+        the interface isn't ready.  Contributed by PretentiousPotatoPeeler.
+        """
+        while True:
+            try:
+                return await loop.create_datagram_endpoint(
+                    IPv4DatagramProtocol, local_addr=addrTuple, allow_broadcast=True
+                )
+            except OSError:
+                if _debug:
+                    IPv4DatagramServer._debug(
+                        "    - Could not create datagram endpoint, retrying..."
+                    )
+                await asyncio.sleep(BACPYPES_ENDPOINT_RETRY_INTERVAL)
+
     def set_local_transport_protocol(self, address, task):
         if _debug:
             IPv4DatagramServer._debug(
                 "set_local_transport_protocol %r, %r", address, task
             )
 
         # get the results of creating the datagram endpoint
```

### Comparing `bacpypes3-0.0.86/bacpypes3/ipv4/app.py` & `bacpypes3-0.0.91/bacpypes3/ipv4/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/ipv4/bvll.py` & `bacpypes3-0.0.91/bacpypes3/ipv4/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/ipv4/link.py` & `bacpypes3-0.0.91/bacpypes3/ipv4/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/ipv4/service.py` & `bacpypes3-0.0.91/bacpypes3/ipv4/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/ipv6/__init__.py` & `bacpypes3-0.0.91/bacpypes3/ipv6/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 from ..comm import Server
 from ..pdu import LocalBroadcast, IPv6Address, IPv6LinkLocalMulticastAddress, PDU
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
+# move this to settings sometime
+BACPYPES_ENDPOINT_RETRY_INTERVAL = 1.0
+
 
 @bacpypes_debugging
 class IPv6DatagramProtocol(asyncio.DatagramProtocol):
-
     _debug: Callable[..., None]
 
     server: "IPv6DatagramServer"
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         if _debug:
             IPv6DatagramProtocol._debug("connection_made %r", transport)
@@ -44,15 +46,14 @@
     def connection_lost(self, exc: Optional[Exception]) -> None:
         if _debug:
             IPv6DatagramProtocol._debug("connection_lost %r", exc)
 
 
 @bacpypes_debugging
 class IPv6DatagramServer(Server[PDU]):
-
     _debug: Callable[..., None]
     _exception: Callable[..., None]
     _transport_tasks: List[Any]
 
     interface_index: int
     local_address: Tuple[str, int, int, int]
     transport: asyncio.DatagramTransport
@@ -97,30 +98,43 @@
                     self.interface_index,
                 ),
             )
         local_socket.bind(address.addrTuple)
 
         # easy call to create a local endpoint
         local_endpoint_task = loop.create_task(
-            loop.create_datagram_endpoint(
-                IPv6DatagramProtocol,
-                sock=local_socket,
-            )
+            self.retrying_create_datagram_endpoint(loop, local_socket)
         )
         if _debug:
             IPv6DatagramServer._debug(
                 "    - local_endpoint_task: %r", local_endpoint_task
             )
         local_endpoint_task.add_done_callback(
             functools.partial(self.set_local_transport_protocol, address)
         )
 
         # keep a list of things that need to complete before sending stuff
         self._transport_tasks = [local_endpoint_task]
 
+    async def retrying_create_datagram_endpoint(
+        self, loop: asyncio.events.AbstractEventLoop, local_socket: socket.socket
+    ):
+        while True:
+            try:
+                return await loop.create_datagram_endpoint(
+                    IPv6DatagramProtocol,
+                    sock=local_socket,
+                )
+            except OSError:
+                if _debug:
+                    IPv6DatagramServer._debug(
+                        "    - Could not create datagram endpoint, retrying..."
+                    )
+                await asyncio.sleep(BACPYPES_ENDPOINT_RETRY_INTERVAL)
+
     def set_local_transport_protocol(self, address, task):
         if _debug:
             IPv6DatagramServer._debug(
                 "set_local_transport_protocol %r, %r", address, task
             )
 
         # get the results of creating the datagram endpoint
```

### Comparing `bacpypes3-0.0.86/bacpypes3/ipv6/bvll.py` & `bacpypes3-0.0.91/bacpypes3/ipv6/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/ipv6/service.py` & `bacpypes3-0.0.91/bacpypes3/ipv6/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/json/util.py` & `bacpypes3-0.0.91/bacpypes3/json/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/lib/batchread.py` & `bacpypes3-0.0.91/bacpypes3/lib/batchread.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/local/analog.py` & `bacpypes3-0.0.91/bacpypes3/local/analog.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         "covIncrement",
     )
 
 
 @bacpypes_debugging
 class AnalogInputObjectIR(AnalogInputObject):
     """
-    A local analog input object with intrinsic reporting.
+    A local analog input object with intrinsic event reporting.
     """
 
     _debug: Callable[..., None]
     _event_algorithm: OutOfRangeEventAlgorithm
     _required = (  # footnote 3
         "timeDelay",
         "notificationClass",
@@ -174,15 +174,15 @@
 
 @bacpypes_debugging
 class AnalogValueObjectCmd(Commandable, AnalogValueObject):
     """
     Commandable Analog Value Object
     """
 
-    pass
+    _required = ("priorityArray",)
 
 
 @bacpypes_debugging
 class AnalogValueObjectIR(AnalogValueObjectCmd):
     """
     Commandable Analog Value Object with Intrinsic Reporting
     """
```

### Comparing `bacpypes3-0.0.86/bacpypes3/local/binary.py` & `bacpypes3-0.0.91/bacpypes3/local/binary.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,17 +34,20 @@
 class BinaryInputObject(_Object, _BinaryInputObject):
     """
     A local binary input object.
     """
 
     _debug: Callable[..., None]
     _cov_criteria = GenericCriteria
-    _required = (  # criteria Table 13-1
+    _required = (
         "presentValue",
         "statusFlags",
+        "eventState",
+        "outOfService",
+        "polarity",
     )
 
 
 @bacpypes_debugging
 class BinaryInputObjectIR(BinaryInputObject):
     """
     A local binary input object with intrinsic reporting.
@@ -83,17 +86,23 @@
 class BinaryOutputObject(Commandable, _Object, _BinaryOutputObject):
     """
     A local binary output object.
     """
 
     _debug: Callable[..., None]
     _cov_criteria = GenericCriteria
-    _required = (  # criteria Table 13-1
+    _required = (
         "presentValue",
         "statusFlags",
+        "eventState",
+        "outOfService",
+        "polarity",
+        "priorityArray",
+        "relinquishDefault",
+        "currentCommandPriority",
     )
 
 
 @bacpypes_debugging
 class BinaryOutputObjectIR(BinaryOutputObject):
     """
     A local binary output object with intrinsic reporting.
@@ -132,27 +141,30 @@
 class BinaryValueObject(_Object, _BinaryValueObject):
     """
     Vanilla Binary Value Object
     """
 
     _debug: Callable[..., None]
     _cov_criteria = GenericCriteria
-    _required = (  # criteria Table 13-1
+    _required = (
         "presentValue",
+        "priorityArray",
         "statusFlags",
+        "eventState",
+        "outOfService",
     )
 
 
 @bacpypes_debugging
-class BinaryValueObjectCmd(Commandable, BinaryValueObject):
+class BinaryValueObjectCmd(Commandable, _BinaryValueObject):
     """
     Commandable Binary Value Object
     """
 
-    pass
+    _required = ("priorityArray",)
 
 
 @bacpypes_debugging
 class BinaryValueObjectIR(BinaryValueObjectCmd):
     """
     Commandable Binary Value Object with Intrinsic Reporting
     """
```

### Comparing `bacpypes3-0.0.86/bacpypes3/local/cmd.py` & `bacpypes3-0.0.91/bacpypes3/local/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/local/cov.py` & `bacpypes3-0.0.91/bacpypes3/local/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/local/device.py` & `bacpypes3-0.0.91/bacpypes3/local/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/local/event.py` & `bacpypes3-0.0.91/bacpypes3/local/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,18 @@
     TimerObject,
 )
 from ..apdu import (
     APDU,
     ConfirmedEventNotificationRequest,
     UnconfirmedEventNotificationRequest,
 )
-from .object import Algorithm, Object
+from .object import (
+    Algorithm,
+    Object,
+)
 from .fault import FaultAlgorithm, OutOfRangeFaultAlgorithm
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
 #
@@ -549,15 +552,15 @@
             new_state_group = EventState.offnormal
 
         # turn off property change notifications
         self._execute_enabled = False
 
         # make the transition
         self.pCurrentState = new_state
-        self._current_state = new_state
+        # self._current_state = new_state
 
         # turn property change notifications back on
         self._execute_enabled = True
 
         # the event arrays are in a different order than event states
         new_state_index = {
             EventState.offnormal: 0,
@@ -692,15 +695,17 @@
             # get its address
             pdu_destination: Address
             if recipient.device:
                 device_info = await event_initiating_object._app.device_info_cache.get_device_info(
                     recipient.device[1]
                 )
                 if not device_info:
-                    raise NotImplementedError("missing device info")
+                    if _debug:
+                        EventAlgorithm._debug("    - no device info")
+                    continue
                 pdu_destination = device_info.address
             elif recipient.address:
                 network_number = recipient.address.networkNumber
                 mac_address = recipient.address.macAddress
 
                 if network_number == 0:
                     if not mac_address:
@@ -944,14 +949,15 @@
                 pTimeDelay=(monitored_object, "timeDelay"),
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             ChangeOfBitstringEventAlgorithm._debug("execute")
+        raise NotImplementedError("CHANGE_OF_BITSTRING not implemented")
 
 
 #
 #   ChangeOfStateEventAlgorithm
 #
 
 
@@ -1157,14 +1163,15 @@
             pTimeDelay=monitoring_object.eventParameters.changeOfValue.timeDelay,
             pTimeDelayNormal=None,
         )
 
     def execute(self):
         if _debug:
             ChangeOfValueEventAlgorithm._debug("execute")
+        raise NotImplementedError("CHANGE_OF_VALUE not implemented")
 
 
 #
 #   CommandFailureEventAlgorithm
 #
 
 
@@ -1226,14 +1233,15 @@
                 pTimeDelay=(monitored_object, "timeDelay"),
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             CommandFailureEventAlgorithm._debug("execute")
+        raise NotImplementedError("COMMAND_FAILURE not implemented")
 
 
 #
 #   FloatingLimitEventAlgorithm
 #
 
 
@@ -1329,14 +1337,15 @@
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             FloatingLimitEventAlgorithm._debug("execute")
             # use pHighDiffLimit for both high and low unless pLowDiffLimit has a value
+        raise NotImplementedError("FLOATING_LIMIT not implemented")
 
 
 #
 #   OutOfRangeEventAlgorithm
 #
 
 
@@ -1583,14 +1592,17 @@
         new_status_flags: StatusFlags = self.pStatusFlags
         if _debug:
             OutOfRangeEventAlgorithm._debug(
                 "    - new_status_flags: %r",
                 new_status_flags,
             )
 
+        # nothing yet
+        event_values: Optional[NotificationParameters] = None
+
         if (self._current_state == EventState.normal) and (
             new_state == EventState.highLimit
         ):
             event_values = NotificationParameters(
                 outOfRange=NotificationParametersOutOfRange(
                     exceedingValue=self.pMonitoredValue,
                     statusFlags=new_status_flags,
@@ -1679,14 +1691,21 @@
                     exceedingValue=self.pMonitoredValue,
                     statusFlags=new_status_flags,
                     deadband=self.pDeadband,
                     exceededLimit=self.pLowLimit,
                 ),
             )
 
+        if _debug:
+            OutOfRangeEventAlgorithm._debug(
+                "    - event_values: %r",
+                event_values,
+            )
+        assert event_values
+
         return event_values
 
 
 #
 #   BufferReadyEventAlgorithm
 #
 
@@ -1735,14 +1754,15 @@
                 pThreshold=monitored_object.notificationThreshold,
                 pPreviousCount=monitored_object.recordsSinceNotification,
             )
 
     def execute(self):
         if _debug:
             BufferReadyEventAlgorithm._debug("execute")
+        raise NotImplementedError("BUFFER_READY not implemented")
 
 
 #
 #   ChangeOfLifeSafetyEventAlgorithm -- 13.3.8
 #
 
 #
@@ -1804,14 +1824,15 @@
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             UnsignedRangeEventAlgorithm._debug("execute")
             # use pHighLimit for both high and low unless pLowLimit has a value
+        raise NotImplementedError("UNSIGNED_RANGE not implemented")
 
 
 #
 #   ExtendedEventAlgorithm
 #
 
 
@@ -1847,14 +1868,15 @@
             pHighLimit=monitoring_object.eventParameters.extended.extendedEventType,
             pParameters=monitoring_object.eventParameters.extended.parameters,
         )
 
     def execute(self):
         if _debug:
             ExtendedEventAlgorithm._debug("execute")
+        raise NotImplementedError("EXTENDED not implemented")
 
 
 #
 #   ChangeOfStatusFlags
 #
 
 
@@ -1911,14 +1933,15 @@
                 pTimeDelay=(monitored_object, "timeDelay"),
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             ChangeOfStatusFlags._debug("execute")
+        raise NotImplementedError("CHANGE_OF_STATUS_FLAGS not implemented")
 
 
 #
 #   AccessEventEventAlgorithm
 #
 
 
@@ -1933,15 +1956,15 @@
     def __init__(
         self,
         monitoring_object: Optional[EventEnrollmentObject],
         monitored_object: Object,
     ):
         if _debug:
             AccessEventEventAlgorithm._debug("__init__ %r", monitored_object)
-        raise NotImplementedError("AccessEventEventAlgorithm")
+        raise NotImplementedError("ACCESS_EVENT")
 
 
 #
 #   DoubleOutOfRangeEventAlgorithm
 #
 
 
@@ -2002,14 +2025,15 @@
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             DoubleOutOfRangeEventAlgorithm._debug("execute")
             # use pHighLimit for both high and low unless pLowLimit has a value
+        raise NotImplementedError("DOUBLE_OUT_OF_RANGE not implemented")
 
 
 #
 #   SignedOutOfRangeEventAlgorithm
 #
 
 
@@ -2070,14 +2094,15 @@
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             SignedOutOfRangeEventAlgorithm._debug("execute")
             # use pHighLimit for both high and low unless pLowLimit has a value
+        raise NotImplementedError("SIGNED_OUT_OF_RANGE not implemented")
 
 
 #
 #   UnsignedOutOfRangeEventAlgorithm
 #
 
 
@@ -2138,14 +2163,15 @@
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             UnsignedOutOfRangeEventAlgorithm._debug("execute")
             # use pHighLimit for both high and low unless pLowLimit has a value
+        raise NotImplementedError("UNSIGNED_OUT_OF_RANGE not implemented")
 
 
 #
 #   ChangeOfCharacterStringEventAlgorithm
 #
 
 
@@ -2200,14 +2226,15 @@
                 pTimeDelay=(monitored_object, "timeDelay"),
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             ChangeOfCharacterStringEventAlgorithm._debug("execute")
+        raise NotImplementedError("CHANGE_OF_CHARACTERSTRING not implemented")
 
 
 #
 #   NoneEventEventAlgorithm
 #
 
 
@@ -2288,14 +2315,15 @@
                 pTimeDelay=(monitored_object, "timeDelay"),
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
             ChangeOfDiscreteValueEventAlgorithm._debug("execute")
+        raise NotImplementedError("CHANGE_OF_DISCRETE_VALUE not implemented")
 
 
 #
 #   ChangeOfTimerEventAlgorithm
 #
 
 
@@ -2320,15 +2348,15 @@
 
     def __init__(
         self,
         monitoring_object: Optional[EventEnrollmentObject],
         monitored_object: Object,
     ):
         if _debug:
-            ChangeOfDiscreteValueEventAlgorithm._debug("__init__ %r", monitored_object)
+            ChangeOfTimerEventAlgorithm._debug("__init__ %r", monitored_object)
         raise NotImplementedError("special assistance needed")
 
         super().__init__(monitoring_object, monitored_object)
 
         if monitoring_object:
             # what to do with monitoring_object.eventParameters.changeOfTimer.updateTimeReference
 
@@ -2361,15 +2389,16 @@
                 pAlarmValues=(monitored_object, "alarmValues"),
                 pTimeDelay=(monitored_object, "timeDelay"),
                 pTimeDelayNormal=(monitored_object, "timeDelayNormal"),
             )
 
     def execute(self):
         if _debug:
-            ChangeOfDiscreteValueEventAlgorithm._debug("execute")
+            ChangeOfTimerEventAlgorithm._debug("execute")
+        raise NotImplementedError("CHANGE_OF_TIMER not implemented")
 
 
 #
 #   EventEnrollmentObject
 #
 
 
@@ -2389,19 +2418,21 @@
             EventEnrollmentObject._debug("__init__ ...")
         super().__init__(**kwargs)
 
     async def _post_init(self):
         """
         This function is called after all of the objects are added to the
         application so that the objectPropertyReference property can
-        find the correct object.
+        find the correct object and the algorithms can be set.
         """
         if _debug:
             EventEnrollmentObject._debug("_post_init")
-        super()._post_init()
+
+        # checks for notification class reference
+        await super()._post_init()
 
         # look up the object being monitored
         dopr: DeviceObjectPropertyReference = self.objectPropertyReference
         if dopr.propertyArrayIndex is not None:
             raise NotImplementedError()
         if dopr.deviceIdentifier is not None:
             raise NotImplementedError()
@@ -2430,14 +2461,18 @@
         event_type: EventType = self.eventType
         if event_type is None:
             self._event_algorithm = None
         elif event_type == EventType.outOfRange:
             self._event_algorithm = OutOfRangeEventAlgorithm(
                 self, self._monitored_object
             )
+        elif event_type == EventType.changeOfState:
+            self._event_algorithm = ChangeOfStateEventAlgorithm(
+                self, self._monitored_object
+            )
         else:
             raise NotImplementedError(f"event type not implemented: {event_type}")
         if _debug:
             EventEnrollmentObject._debug(
                 "    - _event_algorithm: %r",
                 self._event_algorithm,
             )
@@ -2447,15 +2482,15 @@
         """Return the reliability of the object, Clause 12.12.21."""
         if _debug:
             Object._debug("reliability(getter)")
 
         evaluated_reliability = self.__reliability
         if self.__reliability == Reliability.noFaultDetected:
             if self._monitored_object.reliability != Reliability.noFaultDetected:
-                evaluated_reliability = Reliability.monitoredObjectFault
+                evaluated_reliability = Reliability("monitored-object-fault")
             elif self._fault_algorithm:
                 evaluated_reliability = self._fault_algorithm.evaluated_reliability
 
         return evaluated_reliability
 
     @reliability.setter
     def reliability(self, value: Reliability) -> None:
```

### Comparing `bacpypes3-0.0.86/bacpypes3/local/fault.py` & `bacpypes3-0.0.91/bacpypes3/local/fault.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/local/networkport.py` & `bacpypes3-0.0.91/bacpypes3/local/networkport.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/local/object.py` & `bacpypes3-0.0.91/bacpypes3/local/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/local/oos.py` & `bacpypes3-0.0.91/bacpypes3/local/oos.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/local/schedule.py` & `bacpypes3-0.0.91/bacpypes3/local/schedule.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/netservice.py` & `bacpypes3-0.0.91/bacpypes3/netservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Network Service
 """
 
 from __future__ import annotations
 
 import asyncio
 import inspect
-from copy import deepcopy as _deepcopy
+from copy import copy as _copy, deepcopy as _deepcopy
 
 from typing import (
     TYPE_CHECKING,
     Callable,
     Dict,
     List,
     Optional,
+    Set,
     Tuple,
     Union,
     cast,
 )
 
 from .settings import settings
 from .debugging import ModuleLogger, DebugContents, bacpypes_debugging
@@ -42,15 +43,15 @@
     WhoIsRouterToNetwork,
     WhatIsNetworkNumber,
     NetworkNumberIs,
     RoutingTableEntry,
     InitializeRoutingTable,
     InitializeRoutingTableAck,
 )
-from .basetypes import NetworkNumberQuality
+from .basetypes import NetworkNumberQuality, RouterEntryStatus
 
 if TYPE_CHECKING:
     # class is declared as generic in stubs but not at runtime
     WhatIsNetworkNumberFuture = asyncio.Future[int]
 else:
     WhatIsNetworkNumberFuture = asyncio.Future
 
@@ -59,244 +60,361 @@
 _log = ModuleLogger(globals())
 
 # settings
 WHO_IS_ROUTER_TO_NETWORK_TIMEOUT = 2.0
 INITIALIZE_ROUTING_TABLE_TIMEOUT = 3.0
 
 # router status values
-ROUTER_AVAILABLE = 0  # normal
-ROUTER_BUSY = 1  # router is busy
-ROUTER_DISCONNECTED = 2  # could make a connection, but hasn't
-ROUTER_UNREACHABLE = 3  # temporarily unreachable
-
-#
-#   RouterInfo
-#
-
-
-class RouterInfo(DebugContents):
-    """
-    These objects are routing information records that map router
-    addresses with destination networks.
-    """
-
-    _debug_contents: Tuple[str, ...] = ("snet", "address", "dnets")
-
-    snet: Optional[int]
-    address: Address
-    dnets: Dict[int, int]
-
-    def __init__(self, snet: Optional[int], address: Address) -> None:
-        self.snet = snet  # source network
-        self.address = address  # address of the router
-        self.dnets = {}  # {dnet: status}
-
-    def set_status(self, dnets, status) -> None:
-        """Change the status of each of the DNETS."""
-        for dnet in dnets:
-            self.dnets[dnet] = status
-
+ROUTER_AVAILABLE = RouterEntryStatus("available")
+ROUTER_BUSY = RouterEntryStatus("busy")
+ROUTER_DISCONNECTED = RouterEntryStatus("disconnected")
 
 #
 #   RouterInfoCache
 #
 
 
 @bacpypes_debugging
 class RouterInfoCache(DebugContents):
     """
-    This class provides an in-memory implementation of a database of RouterInfo
-    objects.
+    This class provides an in-memory implementation of the network topology.
     """
 
     _debug_contents = (
-        "routers+",
         "path_info+",
+        "router_dnets+",
     )
     _debug: Callable[..., None]
 
-    routers: Dict[Optional[int], Dict[Address, RouterInfo]]
-    path_info: Dict[Tuple[Optional[int], int], RouterInfo]
+    # (snet, Address) -> [ dnet ]
+    router_dnets: Dict[Tuple[Optional[int], Address], Set[int]]
+
+    # (snet, dnet) -> (Address, status)
+    path_info: Dict[Tuple[Optional[int], int], Tuple[Address, RouterEntryStatus]]
 
     def __init__(self):
         if _debug:
             RouterInfoCache._debug("__init__")
 
-        self.routers = {}  # snet -> {Address: RouterInfo}
-        self.path_info = {}  # (snet, dnet) -> RouterInfo
+        self.path_info = {}
+        self.router_dnets = {}
 
-    def get_router_info(self, snet: Optional[int], dnet: int) -> Optional[RouterInfo]:
+    async def get_path_info(
+        self, snet: Optional[int], dnet: int
+    ) -> Optional[Tuple[Address, int]]:
+        """
+        Given a source network and a destination network, return a tuple of
+        the router address and the status of the router to the destination
+        network.
+        """
         if _debug:
-            RouterInfoCache._debug("get_router_info %r %r", snet, dnet)
+            RouterInfoCache._debug("get_path_info %r %r", snet, dnet)
 
         # return the network and address
-        router_info = self.path_info.get((snet, dnet), None)
+        path_info_key = (snet, dnet)
+        path_info = self.path_info.get(path_info_key, None)
         if _debug:
-            RouterInfoCache._debug("   - router_info: %r", router_info)
+            RouterInfoCache._debug("    - path_info: %r", path_info)
 
-        return router_info
+        return path_info
 
-    def update_router_info(
+    async def set_path_info(
         self,
         snet: Optional[int],
+        dnet: int,
         address: Address,
-        dnets: List[int],
-        status: int = ROUTER_AVAILABLE,
+        status: RouterEntryStatus,
+    ) -> bool:
+        """
+        Given a source network and a destination network, set the router
+        address and the status of the router to the destination network.
+        Return false if the cached value has not changed.
+        """
+        if _debug:
+            RouterInfoCache._debug(
+                "set_path_info %r %r %r %r", snet, dnet, address, status
+            )
+
+        path_info_key = (snet, dnet)
+        if path_info := self.path_info.get(path_info_key, None):
+            if path_info == (address, status):
+                if _debug:
+                    RouterInfoCache._debug("    - no change")
+                return False
+
+        self.path_info[path_info_key] = (address, status)
+        return True
+
+    async def delete_path_info(self, snet: Optional[int], dnet: int) -> bool:
+        """
+        Given a source network and a destination network, delete the cache
+        info.  Return false if the cache has not changed.
+        """
+        if _debug:
+            RouterInfoCache._debug("delete_path_info %r %r", snet, dnet)
+
+        # return the network and address
+        path_info_key = (snet, dnet)
+        if path_info_key not in self.path_info:
+            if _debug:
+                RouterInfoCache._debug("    - no cache entry")
+            return False
+
+        del self.path_info[path_info_key]
+        return True
+
+    async def get_router_dnets(
+        self,
+        snet: Optional[int],
+        address: Address,
+    ) -> Optional[Set[int]]:
+        """
+        Given a source network and the address of a router, return the list
+        of destination networks reachable through the router or None if
+        there is no cache entry.
+        """
+        if _debug:
+            RouterInfoCache._debug("get_router_dnets %r %r", snet, address)
+
+        router_dnets_key = (snet, address)
+        router_dnets = self.router_dnets.get(router_dnets_key, None)
+        if _debug:
+            RouterInfoCache._debug("    - router_dnets: %r", router_dnets)
+
+        return router_dnets and _copy(router_dnets)
+
+    async def set_router_dnets(
+        self,
+        snet: Optional[int],
+        address: Address,
+        dnets: Set[int],
+    ) -> bool:
+        """
+        Given a source network, router address, and list of destination
+        networks update the cache.  Return False if the cache value has not
+        changed.
+        """
+        if _debug:
+            RouterInfoCache._debug("set_router_dnets %r %r %r", snet, address, dnets)
+
+        # encode the key
+        router_dnets_key = (snet, address)
+        router_dnets = self.router_dnets.get(router_dnets_key, None)
+        if router_dnets is not None:
+            if router_dnets == dnets:
+                if _debug:
+                    RouterInfoCache._debug("    - no change")
+                return False
+
+        # update the cache
+        self.router_dnets[router_dnets_key] = dnets
+        return True
+
+    async def delete_router_dnets(
+        self,
+        snet: Optional[int],
+        address: Address,
+    ) -> bool:
+        """
+        Given a source network and router address delete the cache entry.
+        Return False if the cache value has not changed.
+        """
+        if _debug:
+            RouterInfoCache._debug("delete_router_dnets %r %r", snet, address)
+
+        # encode the key
+        router_dnets_key = (snet, address)
+        if router_dnets_key not in self.router_dnets:
+            if _debug:
+                RouterInfoCache._debug("    - no change")
+            return False
+
+        # update the cache
+        del self.router_dnets[router_dnets_key]
+        return True
+
+    async def update_path_info(
+        self,
+        snet: Optional[int],
+        address: Address,
+        dnets: Set[int],
     ) -> None:
         if _debug:
-            RouterInfoCache._debug("update_router_info %r %r %r", snet, address, dnets)
+            RouterInfoCache._debug("update_path_info %r %r %r", snet, address, dnets)
 
-        existing_router_info = self.routers.get(snet, {}).get(address, None)
+        # create/update the list of dnets for this router
+        router_dnets_key = (snet, address)
+        router_dnets = await self.get_router_dnets(*router_dnets_key)
+        new_dnets = _copy(dnets)
 
-        other_routers = set()
-        for dnet in dnets:
-            other_router = self.path_info.get((snet, dnet), None)
-            if other_router and (other_router is not existing_router_info):
-                other_routers.add(other_router)
-
-        # remove the dnets from other router(s) and paths
-        if other_routers:
-            for router_info in other_routers:
-                for dnet in dnets:
-                    if dnet in router_info.dnets:
-                        del router_info.dnets[dnet]
-                        del self.path_info[(snet, dnet)]
-                        if _debug:
-                            RouterInfoCache._debug(
-                                "    - del path: %r -> %r via %r",
-                                snet,
-                                dnet,
-                                router_info.address,
-                            )
-                if not router_info.dnets:
-                    del self.routers[snet][router_info.address]
-                    if _debug:
-                        RouterInfoCache._debug(
-                            "    - no dnets: %r via %r", snet, router_info.address
-                        )
+        if router_dnets is None:
+            if _debug:
+                RouterInfoCache._debug("    - new router: %r", address)
+            router_dnets: Set[int] = set()
+        else:
+            # just look for new dnets related to this router
+            new_dnets -= router_dnets
+            if not new_dnets:
+                # if there are no new dnets then the router_address is already
+                # correct and there are no others that need updating
+                if _debug:
+                    RouterInfoCache._debug("    - no changes")
+                return
+        if _debug:
+            RouterInfoCache._debug("    - router_dnets: %r", router_dnets)
+            RouterInfoCache._debug("    - new_dnets: %r", new_dnets)
 
-        # update current router info if there is one
-        if not existing_router_info:
-            router_info = RouterInfo(snet, address)
-            if snet not in self.routers:
-                self.routers[snet] = {address: router_info}
-            else:
-                self.routers[snet][address] = router_info
+        # get the addresses of the routers that used to be the router to
+        # any of the dnets
+        for dnet in new_dnets:
+            path_info = await self.get_path_info(snet, dnet)
+            if not path_info:
+                continue
+            if _debug:
+                RouterInfoCache._debug("    - old path: %r", path_info)
 
-            for dnet in dnets:
-                self.path_info[(snet, dnet)] = router_info
+            old_router_address = path_info[0]
+            old_router_dnets = await self.get_router_dnets(snet, old_router_address)
+            if old_router_dnets is None:
+                raise RuntimeError(f"routing cache: no router {old_router_address}")
+            if dnet not in old_router_dnets:
+                raise RuntimeError(
+                    f"routing cache: dnet {dnet} not in {old_router_dnets}"
+                )
+
+            # no longer a path through old router
+            old_router_dnets.remove(dnet)
+            await self.set_router_dnets(snet, old_router_address, old_router_dnets)
+
+            # if there are no more dnets remove the router reference
+            if not old_router_dnets:
                 if _debug:
                     RouterInfoCache._debug(
-                        "    - add path: %r -> %r via %r",
-                        snet,
-                        dnet,
-                        router_info.address,
+                        "    - router abandoned: %r", old_router_address
                     )
-                router_info.dnets[dnet] = status
-        else:
-            for dnet in dnets:
-                if dnet not in existing_router_info.dnets:
-                    self.path_info[(snet, dnet)] = existing_router_info
-                    if _debug:
-                        RouterInfoCache._debug("    - add path: %r -> %r", snet, dnet)
-                existing_router_info.dnets[dnet] = status
-
-    def update_router_status(self, snet: int, address: Address, status: int) -> None:
-        if _debug:
-            RouterInfoCache._debug(
-                "update_router_status %r %r %r", snet, address, status
-            )
+                await self.delete_router_dnets(snet, old_router_address)
 
-        existing_router_info = self.routers.get(snet, {}).get(address, None)
-        if not existing_router_info:
-            if _debug:
-                RouterInfoCache._debug("    - not a router we know about")
-            return
+        # add to the existing set with the new ones and set the path
+        router_dnets |= new_dnets
 
-        ###TODO
-        # existing_router_info.status = status
-        # if _debug:
-        #     RouterInfoCache._debug("    - status updated")
+        await self.set_router_dnets(snet, address, router_dnets)
+        for dnet in new_dnets:
+            await self.set_path_info(snet, dnet, address, ROUTER_AVAILABLE)
 
-    def delete_router_info(
+    async def remove_path_info(
         self,
         snet: int,
         address: Optional[Address] = None,
-        dnets: Optional[List[int]] = None,
+        dnets: Optional[Set[int]] = None,
     ) -> None:
+        """
+        Given a source network, optional router address and optional list of
+        destination networks, remove the path information.
+        """
         if _debug:
-            RouterInfoCache._debug("delete_router_info %r %r %r", dnets)
+            RouterInfoCache._debug("remove_path_info %r %r %r", snet, address, dnets)
 
-        if (address is None) and (dnets is None):
-            raise RuntimeError("inconsistent parameters")
-
-        # remove the dnets from a router or the whole router
         if address is not None:
-            router_info = self.routers.get(snet, {}).get(address, None)
-            if not router_info:
+            # get the list of dnets for this router
+            router_dnets = await self.get_router_dnets(snet, address)
+            if router_dnets is None:
                 if _debug:
-                    RouterInfoCache._debug("    - no route info")
+                    RouterInfoCache._debug("    - no known dnets")
+                return
+            if dnets is None:
+                if _debug:
+                    RouterInfoCache._debug("    - remove them all")
+                dnets = router_dnets
             else:
-                for dnet in dnets or router_info.dnets:
-                    del self.path_info[(snet, dnet)]
-                    if _debug:
-                        RouterInfoCache._debug(
-                            "    - del path: %r -> %r via %r",
-                            snet,
-                            dnet,
-                            router_info.address,
-                        )
-                del self.routers[snet][address]
-            return
+                if _debug:
+                    RouterInfoCache._debug("    - remove those in the router")
+                dnets &= router_dents
 
-        # look for routers to the dnets
-        other_routers = set()
-        for dnet in dnets:  # type: ignore[union-attr]
-            other_router = self.path_info.get((snet, dnet), None)
-            if other_router:  ###TODO: and (other_router is not existing_router_info):
-                other_routers.add(other_router)
-
-        # remove the dnets from other router(s) and paths
-        for router_info in other_routers:
-            for dnet in dnets:  # type: ignore[union-attr]
-                if dnet in router_info.dnets:
-                    del router_info.dnets[dnet]
-                    del self.path_info[(snet, dnet)]
-                    if _debug:
-                        RouterInfoCache._debug(
-                            "    - del path: %r -> %r via %r",
-                            snet,
-                            dnet,
-                            router_info.address,
-                        )
-            if not router_info.dnets:
-                del self.routers[snet][router_info.address]
+            # remove the path info
+            for dnet in dnets:
+                await self.delete_path_info(snet, dnet)
+
+            # remove the dnets
+            router_dnets -= dnets
+
+            # if there are no more dnets remove the router reference
+            if not router_dnets:
                 if _debug:
-                    RouterInfoCache._debug(
-                        "    - no dnets: %r via %r", snet, router_info.address
-                    )
+                    RouterInfoCache._debug("    - router abandoned: %r", address)
+                await self.delete_router_dnets(snet, address)
+            else:
+                await self.set_router_dnets(snet, address, router_dnets)
+        else:
+            if dnets is None:
+                raise RuntimeError("inconsistent parameters")
+
+            for dnet in dnets:
+                path_info = await self.get_path_info(snet, dnet)
+                if not path_info:
+                    continue
+
+                router_address, _ = path_info
+
+                # get the list of dnets for this router
+                router_dnets = await self.get_router_dnets(snet, router_address)
+                if router_dnets is None:
+                    raise RuntimeError("routing cache conflict")
+                if dnet not in router_dnets:
+                    raise RuntimeError("routing cache conflict")
+
+                router_dnets.remove(dnet)
+                await self.set_router_dnets(snet, router_address, router_dnets)
 
-    def update_source_network(self, old_snet: int, new_snet: int) -> None:
+                # delete the path info
+                await self.delete_path_info(snet, dnet)
+
+                # if there are no more dnets remove the router reference
+                if not router_dnets:
+                    if _debug:
+                        RouterInfoCache._debug("    - router abandoned: %r", address)
+                    await self.delete_router_dnets(snet, address)
+
+    async def update_router_status(
+        self, snet: int, address: Address, status: RouterEntryStatus
+    ) -> None:
         if _debug:
-            RouterInfoCache._debug("update_source_network %r %r", old_snet, new_snet)
+            RouterInfoCache._debug(
+                "update_router_status %r %r %r", snet, address, status
+            )
 
-        if old_snet not in self.routers:
+        # get the list of dnets for this router
+        router_dnets = await self.get_router_dnets(snet, address)
+        if router_dnets is None:
             if _debug:
-                RouterInfoCache._debug(
-                    "    - no router references: %r", list(self.routers.keys())
-                )
+                RouterInfoCache._debug("    - no known dnets")
             return
 
-        # move the router info records to the new net
-        snet_routers = self.routers[new_snet] = self.routers.pop(old_snet)
+        # save the status
+        for dnet in router_dnets:
+            await self.set_path_info(snet, dnet, address, status)
 
-        # update the paths
-        for address, router_info in snet_routers.items():
-            for dnet in router_info.dnets:
-                self.path_info[(new_snet, dnet)] = self.path_info.pop((old_snet, dnet))
+    async def update_source_network(self, old_snet: int, new_snet: int) -> None:
+        """
+        This method is called when the network number for an adapter becomes
+        known, the Network-Number-Is service.
+        """
+        if _debug:
+            RouterInfoCache._debug("update_source_network %r %r", old_snet, new_snet)
+
+        router_dnets_items = list(self.router_dnets.items())
+        for (snet, router_address), router_dnets in router_dnets_items:
+            if snet == old_snet:
+                # out with the old, in with the new
+                del self.router_dnets[(old_snet, router_address)]
+                self.router_dnets[(new_snet, router_address)] = router_dnets
+
+                for dnet in router_dnets:
+                    path_info = self.path_info[(old_snet, dnet)]
+                    del self.path_info[(old_snet, dnet)]
+                    self.path_info[(new_snet, dnet)] = path_info
 
 
 #
 #   NetworkAdapter
 #
 
 
@@ -487,48 +605,54 @@
                 NetworkServiceAccessPoint._debug("    - no local address")
 
         # bind to the server
         bind(adapter, server)
 
     # -----
 
-    def update_router_references(
+    async def update_router_references(
         self, snet: int, address: Address, dnets: List[int]
     ) -> None:
-        """Update references to routers."""
+        """
+        Update references to routers, called when I-Am-Router-To-Network is
+        received.  Also called to load the router info cache during application
+        startup if necessary.
+        """
         if _debug:
             NetworkServiceAccessPoint._debug(
                 "update_router_references %r %r %r", snet, address, dnets
             )
 
         # see if we have an adapter for the snet
         if snet not in self.adapters:
             raise RuntimeError("no adapter for network: %d" % (snet,))
 
         # pass this along to the cache
-        self.router_info_cache.update_router_info(snet, address, dnets)
+        await self.router_info_cache.update_path_info(snet, address, set(dnets))
 
-    def delete_router_references(
+    async def delete_router_references(
         self,
         snet: int,
         address: Optional[Address] = None,
-        dnets: Optional[List[int]] = None,
+        dnets: Optional[Set[int]] = None,
     ) -> None:
-        """Delete references to routers/networks."""
+        """
+        Delete references to routers/networks.
+        """
         if _debug:
             NetworkServiceAccessPoint._debug(
                 "delete_router_references %r %r %r", snet, address, dnets
             )
 
         # see if we have an adapter for the snet
         if snet not in self.adapters:
             raise RuntimeError("no adapter for network: %d" % (snet,))
 
         # pass this along to the cache
-        self.router_info_cache.delete_router_info(snet, address, dnets)
+        await self.router_info_cache.delete_router_info(snet, address, dnets)
 
     # -----
 
     async def indication(self, pdu: PDU) -> None:
         if _debug:
             NetworkServiceAccessPoint._debug("indication %r", pdu)
 
@@ -677,32 +801,33 @@
                 "    - look for routing information: %r", self.router_info_cache
             )
 
         # look for routing information from the network of one of our
         # adapters to the destination network
         router_info = None
         for snet, snet_adapter in self.adapters.items():
-            router_info = self.router_info_cache.get_router_info(snet, dnet)
+            router_info = await self.router_info_cache.get_path_info(snet, dnet)
             if router_info:
                 break
 
         # if there is info, we have a path
         if router_info:
             if _debug:
                 NetworkServiceAccessPoint._debug(
                     "    - router_info found: %r", router_info
                 )
 
-            # check the path status
-            dnet_status = router_info.dnets[dnet]
+            router_address, router_status = router_info
             if _debug:
-                NetworkServiceAccessPoint._debug("    - dnet_status: %r", dnet_status)
+                NetworkServiceAccessPoint._debug(
+                    "    - router_status: %r", router_status
+                )
 
             # fix the destination and send it
-            npdu.pduDestination = router_info.address
+            npdu.pduDestination = router_address
             await snet_adapter.process_npdu(npdu)
 
         else:
             if _debug:
                 NetworkServiceAccessPoint._debug("    - look for the router")
 
             result_list = await nse.who_is_router_to_network(network=dnet)
@@ -752,18 +877,18 @@
             # see if this is attempting to spoof a directly connected network
             snet = npdu.npduSADR.addrNet
             if snet in self.adapters:
                 NetworkServiceAccessPoint._warning("    - path error (1)")
                 return
 
             # pass this new path along to the cache
-            self.router_info_cache.update_router_info(
+            await self.router_info_cache.update_path_info(
                 adapter.adapterNet,
                 cast(Address, npdu.pduSource),
-                [snet],  # type: ignore[list-item]
+                set([snet]),
             )
 
         # check for destination routing
         if (not npdu.npduDADR) or (npdu.npduDADR.addrType == Address.nullAddr):
             if _debug:
                 NetworkServiceAccessPoint._debug("    - no DADR")
 
@@ -987,18 +1112,22 @@
                 await xadapter.process_npdu(_deepcopy(newpdu))
                 return
 
             # look for routing information from the network of one of our
             # adapters to the destination network
             router_info = None
             for snet, snet_adapter in self.adapters.items():
-                router_info = self.router_info_cache.get_router_info(snet, dnet)
+                router_info = await self.router_info_cache.get_path_info(snet, dnet)
                 if router_info:
+                    if _debug:
+                        NetworkServiceAccessPoint._debug(
+                            "    - router_info found: %r", router_info
+                        )
                     router_adapter = snet_adapter
-                    router_address = router_info.address
+                    router_address, router_status = router_info
                     break
 
             # no path, look for one
             if not router_info:
                 if _debug:
                     NetworkServiceAccessPoint._debug("    - look for the router")
 
@@ -1357,17 +1486,14 @@
 
             # skip for an empty list, perhaps they are not yet learned
             if not netlist:
                 if _debug:
                     NetworkServiceElement._debug("    - skipping, no netlist")
                 continue
 
-            # pass this along to the cache -- on hold #213
-            # sap.router_info_cache.update_router_info(adapter.adapterNet, adapter.adapterAddr, netlist)
-
             # send an announcement
             self.i_am_router_to_network(adapter=adapter, network=netlist)
 
     async def indication(self, adapter: NetworkAdapter, npdu: NPDU) -> None:  # type: ignore[override]
         if _debug:
             NetworkServiceElement._debug("indication %r %r", adapter, npdu)
 
@@ -1865,15 +1991,15 @@
                 await self.response(adapter, iamrtn)
                 return
 
             # look for routing information from the network of one of our
             # adapters to the destination network
             router_info = None
             for snet, snet_adapter in sap.adapters.items():
-                router_info = sap.router_info_cache.get_router_info(snet, dnet)
+                router_info = await sap.router_info_cache.get_path_info(snet, dnet)
                 if router_info:
                     break
 
             # found a path
             if router_info:
                 if _debug:
                     NetworkServiceElement._debug("    - router found: %r", router_info)
@@ -1923,15 +2049,15 @@
 
         # reference the service access point
         sap = cast(NetworkServiceAccessPoint, self.elementService)
         if _debug:
             NetworkServiceElement._debug("    - sap: %r", sap)
 
         # pass along to the service access point
-        sap.update_router_references(
+        await sap.update_router_references(
             adapter.adapterNet, npdu.pduSource, npdu.iartnNetworkList
         )
 
         # skip forwarding to other adpaters if this is not a router
         if len(sap.adapters) == 1:
             if _debug:
                 NetworkServiceElement._debug("    - not a router")
@@ -2096,15 +2222,17 @@
         if adapter.adapterNet is None:
             if _debug:
                 NetworkServiceElement._debug(
                     "   - local network not known: %r", list(sap.adapters.keys())
                 )
 
             # update the routing information
-            sap.router_info_cache.update_source_network(None, npdu.nniNet)
+            asyncio.create_task(
+                sap.router_info_cache.update_source_network(None, npdu.nniNet)
+            )
 
             # delete the reference from an unknown network
             del sap.adapters[None]
 
             adapter.adapterNet = npdu.nniNet
             adapter.adapterNetConfigured = NetworkNumberQuality.learned
```

### Comparing `bacpypes3-0.0.86/bacpypes3/npdu.py` & `bacpypes3-0.0.91/bacpypes3/npdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/object.py` & `bacpypes3-0.0.91/bacpypes3/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -2287,14 +2287,15 @@
     eventMessageTexts: ArrayOf(CharacterString, _length=3)
     eventMessageTextsConfig: ArrayOf(CharacterString, _length=3)
     eventDetectionEnable: Boolean
     eventAlgorithmInhibitRef: ObjectPropertyReference
     eventAlgorithmInhibit: Boolean
     timeDelayNormal: Unsigned
     reliabilityEvaluationInhibit: Boolean
+    currentCommandPriority: OptionalUnsigned
     valueSource: ValueSource
     valueSourceArray: ArrayOf(ValueSource, _length=16)
     lastCommandTime: TimeStamp
     commandTimeArray: ArrayOf(TimeStamp, _length=16)
     auditPriorityFilter: OptionalPriorityFilter
```

### Comparing `bacpypes3-0.0.86/bacpypes3/pdu.py` & `bacpypes3-0.0.91/bacpypes3/pdu.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     + _ipv6_address_port
     + ")"
     + _at_route
     + "$"
 )
 
 ethernet_re = re.compile(r"^([0-9A-Fa-f][0-9A-Fa-f][:]){5}([0-9A-Fa-f][0-9A-Fa-f])$")
-interface_port_re = re.compile(r"^(?:([\w.]+))(?::(\d+))?$")
+interface_port_re = re.compile(r"^(?:([A-Za-z][\w.-]+))(?::(\d+))?$")
 host_port_re = re.compile(r"^(?:([\w.]+))(?::(\d+))?$")
 
 network_types: Dict[str, type]
 
 
 @bacpypes_debugging
 class AddressMetaclass(type):
@@ -262,22 +262,26 @@
                         Address._debug("    - IPv4 address")
                     if not local_ipv4_net:
                         local_ipv4_net = "32"
                     if not local_ipv4_port:
                         local_ipv4_port = "47808"
 
                     address = super(AddressMetaclass, IPv4Address).__call__(f"{local_ipv4_addr}/{local_ipv4_net}", port=int(local_ipv4_port), **kwargs)  # type: ignore[misc]
+                    if net_addr > 0:
+                        address = super(AddressMetaclass, RemoteStation).__call__(net_addr, address.addrAddr, **kwargs)  # type: ignore[misc]
 
                 if local_ipv6_addr:
                     if _debug:
                         AddressMetaclass._debug("    - IPv6 address")
                     if not local_ipv6_port:
                         local_ipv6_port = "47808"
 
                     address = super(AddressMetaclass, IPv6Address).__call__(local_ipv6_addr, port=int(local_ipv6_port), **kwargs)  # type: ignore[misc]
+                    if net_addr > 0:
+                        address = super(AddressMetaclass, RemoteStation).__call__(net_addr, address.addrAddr, **kwargs)  # type: ignore[misc]
 
                 # if this is a remote address, add the network
                 if net and (not global_broadcast) and (not local_broadcast):
                     if _debug:
                         AddressMetaclass._debug("    - adding network")
                     address.addrNet = net_addr
```

### Comparing `bacpypes3-0.0.86/bacpypes3/primitivedata.py` & `bacpypes3-0.0.91/bacpypes3/primitivedata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/rdf/core.py` & `bacpypes3-0.0.91/bacpypes3/rdf/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,14 +347,14 @@
 
         if isinstance(value, Literal):
             o = value
         elif isinstance(value, Atomic):
             o = atomic_encode(self._graph, value)
         elif isinstance(value, Sequence):
             o = _blank_node()
-            sequence_to_graph(value, o, self._graph)
+            sequence_to_graph(value, o, g)
         else:
             o = Literal(value)
 
         # uses the convenience function which removes existing triples for
         # functional properties
         g.set((s, p, o))
```

### Comparing `bacpypes3-0.0.86/bacpypes3/rdf/util.py` & `bacpypes3-0.0.91/bacpypes3/rdf/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/sc/bvll.py` & `bacpypes3-0.0.91/bacpypes3/sc/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/sc/service.py` & `bacpypes3-0.0.91/bacpypes3/sc/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/service/cov.py` & `bacpypes3-0.0.91/bacpypes3/service/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/service/device.py` & `bacpypes3-0.0.91/bacpypes3/service/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/service/object.py` & `bacpypes3-0.0.91/bacpypes3/service/object.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ReadAccessResult,
     ReadAccessResultElement,
     ReadAccessResultElementChoice,
     ReadAccessSpecification,
 )
 from ..constructeddata import Any, Array, List, SequenceOf
 from ..debugging import ModuleLogger, bacpypes_debugging
-from ..errors import ExecutionError, ObjectError, PropertyError
+from ..errors import ExecutionError, ObjectError, PropertyError, RejectException
 from ..object import DeviceObject
 from ..pdu import Address
 from ..primitivedata import Date, Null, ObjectIdentifier, Time, Unsigned
 from ..vendor import VendorInfo, get_vendor_info
 
 # some debugging
 _debug = 0
@@ -975,8 +975,104 @@
         return property_value
 
     async def do_ReadRangeRequest(self, apdu: ReadRangeRequest) -> None:
         """Return the value of some property of one of our objects."""
         if _debug:
             ReadRangeServices._debug("do_ReadRangeRequest %r", apdu)
 
-        raise NotImplementedError
+        raise NotImplementedError()
+
+    """
+    TODO : Make that better
+        # extract the object identifier
+        objId = apdu.objectIdentifier
+
+        # get the object
+        obj = self.get_object_id(objId)
+        if not obj:
+            raise ExecutionError(errorClass="object", errorCode="unknownObject")
+
+        if _debug:
+            ReadRangeServices._debug("    - object: %r", obj)
+
+        # get the datatype
+        datatype = obj.get_property_type(apdu.propertyIdentifier)
+        if _debug:
+            ReadRangeServices._debug("    - datatype: %r", datatype)
+
+        # must be a list, or an array of lists
+        if issubclass(datatype, List):
+            pass
+        elif (
+            (apdu.propertyArrayIndex is not None)
+            and issubclass(datatype, Array)
+            and issubclass(datatype.subtype, List)
+        ):
+            pass
+        else:
+            raise ExecutionError(errorClass="property", errorCode="propertyIsNotAList")
+
+        # get the value
+        if _debug:
+            ReadRangeServices._debug(apdu.__dict__)
+        try:
+            value = await obj.read_property(
+                apdu.propertyIdentifier, apdu.propertyArrayIndex
+            )
+
+            if _debug:
+                ReadRangeServices._debug(
+                    f"    - value: {value.__repr__()} | of type {type(value)}"
+                )
+            if value is None:
+                raise PropertyError(errorCode="unknownProperty")
+            if isinstance(value, List):
+                ReadRangeServices._debug(
+                    "    - value is a list of: %r", datatype.subtype
+                )
+                # datatype = datatype.subtype
+
+            if apdu.range.byPosition:
+                range_by_position = apdu.range.byPosition
+                if _debug:
+                    ReadRangeServices._debug(
+                        "    - range_by_position: %r", range_by_position
+                    )
+
+            elif apdu.range.bySequenceNumber:
+                range_by_sequence_number = apdu.range.bySequenceNumber
+                if _debug:
+                    ReadRangeServices._debug(
+                        "    - range_by_sequence_number: %r", range_by_sequence_number
+                    )
+
+            elif apdu.range.byTime:
+                range_by_time = apdu.range.byTime
+                if _debug:
+                    ReadRangeServices._debug("    - range_by_time: %r", range_by_time)
+
+            else:
+                raise RejectException("missingRequiredParameter")
+        except AttributeError:
+            # exception if this is not a defined property
+            raise PropertyError(errorCode="unknownProperty")
+        # this is an ack
+        resp = ReadRangeACK(context=apdu)
+        resp.objectIdentifier = objId
+        resp.propertyIdentifier = apdu.propertyIdentifier
+        resp.propertyArrayIndex = apdu.propertyArrayIndex
+
+        resp.resultFlags = [1, 1, 0]
+        resp.itemCount = len(value)
+
+        # save the result in the item data
+        item_data = SequenceOf(Any)()
+        item_data.cast_in(value)
+        resp.itemData = item_data
+        if _debug:
+            ReadRangeServices._debug("    - itemData : %r", resp.itemData)
+            ReadRangeServices._debug("    - resp: %r", resp)
+        self.response(resp)
+
+        # return the result
+        await self.response(resp)
+"""
```

### Comparing `bacpypes3-0.0.86/bacpypes3/settings.py` & `bacpypes3-0.0.91/bacpypes3/settings.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/vendor.py` & `bacpypes3-0.0.91/bacpypes3/vendor.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/vlan/__init__.py` & `bacpypes3-0.0.91/bacpypes3/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3/vlan/link.py` & `bacpypes3-0.0.91/bacpypes3/vlan/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/bacpypes3.egg-info/PKG-INFO` & `bacpypes3-0.0.91/bacpypes3.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.86
+Version: 0.0.91
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.86/bacpypes3.egg-info/SOURCES.txt` & `bacpypes3-0.0.91/bacpypes3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 bacpypes3/local/analog.py
 bacpypes3/local/binary.py
 bacpypes3/local/cmd.py
 bacpypes3/local/cov.py
 bacpypes3/local/device.py
 bacpypes3/local/event.py
 bacpypes3/local/fault.py
+bacpypes3/local/multistate.py
 bacpypes3/local/networkport.py
 bacpypes3/local/object.py
 bacpypes3/local/oos.py
 bacpypes3/local/schedule.py
 bacpypes3/rdf/__init__.py
 bacpypes3/rdf/__main__.py
 bacpypes3/rdf/core.py
```

### Comparing `bacpypes3-0.0.86/setup.py` & `bacpypes3-0.0.91/setup.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/clocked_test.py` & `bacpypes3-0.0.91/tests/clocked_test.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/state_machine.py` & `bacpypes3-0.0.91/tests/state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_1.py` & `bacpypes3-0.0.91/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test__template.py` & `bacpypes3-0.0.91/tests/test__template.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_constructed_data/test_any.py` & `bacpypes3-0.0.91/tests/test_constructed_data/test_any.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_constructed_data/test_array.py` & `bacpypes3-0.0.91/tests/test_constructed_data/test_array.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_constructed_data/test_choice.py` & `bacpypes3-0.0.91/tests/test_constructed_data/test_choice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_constructed_data/test_list.py` & `bacpypes3-0.0.91/tests/test_constructed_data/test_list.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_constructed_data/test_read_property_multiple.py` & `bacpypes3-0.0.91/tests/test_constructed_data/test_read_property_multiple.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_constructed_data/test_sequence.py` & `bacpypes3-0.0.91/tests/test_constructed_data/test_sequence.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_constructed_data/test_sequence_of.py` & `bacpypes3-0.0.91/tests/test_constructed_data/test_sequence_of.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_pdu/test_address.py` & `bacpypes3-0.0.91/tests/test_pdu/test_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,15 @@
         self.match_address(test_addr, 4, 1, 1, "02")
         assert str(test_addr) == "1:2"
 
         # test bad network
         with pytest.raises(ValueError):
             Address("65536:0x02")
 
+        # test hex string
         test_addr = Address("1:0x0203")
         self.match_address(test_addr, 4, 1, 2, "0203")
         assert str(test_addr) == "1:0x0203"
 
         # test old school hex string
         if False:
             test_addr = Address("1:X'02'")
@@ -227,14 +228,24 @@
             self.match_address(test_addr, 4, 1, 2, "0203")
             assert str(test_addr) == "1:0x0203"
 
             # test bad network
             with pytest.raises(ValueError):
                 Address("65536:X'02'")
 
+        # test IPv4 remote station address
+        test_addr = Address("1:2.3.4.5")
+        self.match_address(test_addr, 4, 1, 6, "02030405BAC0")
+        assert str(test_addr) == "1:2.3.4.5"
+
+        # test IPv4 remote station address with non-standard port
+        test_addr = Address("1:2.3.4.5:47809")
+        self.match_address(test_addr, 4, 1, 6, "02030405BAC1")
+        assert str(test_addr) == "1:2.3.4.5:47809"
+
     def test_address_global_broadcast_str(self):
         if _debug:
             TestAddress._debug("test_address_global_broadcast_str")
 
         # test local broadcast
         test_addr = Address("*:*")
         self.match_address(test_addr, 5, None, None, None)
```

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_bit_string.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_bit_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_boolean.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_boolean.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_character_string.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_character_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_date.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_date.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_double.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_double.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_enumerated.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_enumerated.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_integer.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_integer.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_null.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_null.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_object_identifier.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_object_identifier.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_octet_string.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_octet_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_real.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_real.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_tag.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_tag.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_time.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_time.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_primitive_data/test_unsigned.py` & `bacpypes3-0.0.91/tests/test_primitive_data/test_unsigned.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_utilities/test_state_machine.py` & `bacpypes3-0.0.91/tests/test_utilities/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_vlan/test_ipv4_network.py` & `bacpypes3-0.0.91/tests/test_vlan/test_ipv4_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_vlan/test_ipv4_router.py` & `bacpypes3-0.0.91/tests/test_vlan/test_ipv4_router.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/test_vlan/test_network.py` & `bacpypes3-0.0.91/tests/test_vlan/test_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/trapped_classes.py` & `bacpypes3-0.0.91/tests/trapped_classes.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.86/tests/utilities.py` & `bacpypes3-0.0.91/tests/utilities.py`

 * *Files identical despite different names*

