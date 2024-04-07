# Comparing `tmp/nef_pipelines-0.1.58.tar.gz` & `tmp/nef_pipelines-0.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.58.tar", last modified: Thu Apr  4 07:43:34 2024, max compression
+gzip compressed data, was "nef_pipelines-0.1.59.tar", last modified: Sun Apr  7 09:37:22 2024, max compression
```

## Comparing `nef_pipelines-0.1.58.tar` & `nef_pipelines-0.1.59.tar`

### file list

```diff
@@ -1,488 +1,490 @@
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.502173 nef_pipelines-0.1.58/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.111727 nef_pipelines-0.1.58/.github/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.219055 nef_pipelines-0.1.58/.github/workflows/
--rw-r--r--   0 garyt      (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.58/.github/workflows/ci.yml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.228232 nef_pipelines-0.1.58/.idea/
--rw-r--r--   0 garyt      (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.58/.idea/.gitignore
--rw-r--r--   0 garyt      (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.58/.idea/.name
--rw-r--r--   0 garyt      (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.58/.idea/NFC.iml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.231769 nef_pipelines-0.1.58/.idea/inspectionProfiles/
--rw-r--r--   0 garyt      (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.58/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garyt      (501) staff       (20)      229 2023-10-31 09:12:23.000000 nef_pipelines-0.1.58/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garyt      (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.58/.idea/modules.xml
--rw-r--r--   0 garyt      (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.58/.idea/vcs.xml
--rw-r--r--   0 garyt      (501) staff       (20)     1330 2024-02-09 22:26:45.000000 nef_pipelines-0.1.58/.pre-commit-config.yaml
--rw-r--r--   0 garyt      (501) staff       (20)      490 2022-11-25 17:14:46.000000 nef_pipelines-0.1.58/.readthedocs.yml
--rw-r--r--   0 garyt      (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.58/AUTHORS.md
--rw-r--r--   0 garyt      (501) staff       (20)     6576 2024-04-04 07:41:41.000000 nef_pipelines-0.1.58/CHANGELOG.md
--rw-r--r--   0 garyt      (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.58/CONTRIBUTING.md
--rw-r--r--   0 garyt      (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.58/LICENSE.txt
--rw-r--r--   0 garyt      (501) staff       (20)     9577 2024-04-04 07:43:34.501713 nef_pipelines-0.1.58/PKG-INFO
--rw-r--r--   0 garyt      (501) staff       (20)     8212 2024-03-04 22:23:39.000000 nef_pipelines-0.1.58/README.md
--rw-r--r--   0 garyt      (501) staff       (20)      807 2023-05-21 15:23:42.000000 nef_pipelines-0.1.58/TODO.md
--rw-r--r--   0 garyt      (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.58/pyproject.toml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.235426 nef_pipelines-0.1.58/references/
--rw-r--r--   0 garyt      (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.58/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garyt      (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.58/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rwxr--r--   0 garyt      (501) staff       (20)     1264 2024-03-19 22:32:32.000000 nef_pipelines-0.1.58/release_to_pypi.sh
--rw-r--r--   0 garyt      (501) staff       (20)      351 2024-03-27 22:48:52.000000 nef_pipelines-0.1.58/requirements.txt
--rw-r--r--   0 garyt      (501) staff       (20)     1697 2024-04-04 07:43:34.504104 nef_pipelines-0.1.58/setup.cfg
--rw-r--r--   0 garyt      (501) staff       (20)      710 2022-11-25 17:14:46.000000 nef_pipelines-0.1.58/setup.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.112920 nef_pipelines-0.1.58/src/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.269679 nef_pipelines-0.1.58/src/nef_pipelines/
--rw-r--r--   0 garyt      (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.58/src/nef_pipelines/VERSION
--rw-r--r--   0 garyt      (501) staff       (20)      577 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.296760 nef_pipelines-0.1.58/src/nef_pipelines/data/
--rw-r--r--   0 garyt      (501) staff       (20)    16381 2024-03-04 22:17:52.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/ambiguity_translations.json
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.549085 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/
--rw-r--r--   0 garyt      (501) staff       (20)   108495 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   104358 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json
--rw-r--r--   0 garyt      (501) staff       (20)   118386 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)   102566 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json
--rw-r--r--   0 garyt      (501) staff       (20)   108304 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)    91086 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)    35009 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   109165 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   105025 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json
--rw-r--r--   0 garyt      (501) staff       (20)   119258 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   102439 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json
--rw-r--r--   0 garyt      (501) staff       (20)    96862 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json
--rw-r--r--   0 garyt      (501) staff       (20)    99315 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    35085 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    73745 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json
--rw-r--r--   0 garyt      (501) staff       (20)   151265 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json
--rw-r--r--   0 garyt      (501) staff       (20)   102950 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json
--rw-r--r--   0 garyt      (501) staff       (20)    96313 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    99814 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)   104993 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json
--rw-r--r--   0 garyt      (501) staff       (20)   110515 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json
--rw-r--r--   0 garyt      (501) staff       (20)    67204 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json
--rw-r--r--   0 garyt      (501) staff       (20)   127933 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json
--rw-r--r--   0 garyt      (501) staff       (20)   119775 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json
--rw-r--r--   0 garyt      (501) staff       (20)   113627 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json
--rw-r--r--   0 garyt      (501) staff       (20)   150013 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   103831 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   112702 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json
--rw-r--r--   0 garyt      (501) staff       (20)    89442 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)    89294 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json
--rw-r--r--   0 garyt      (501) staff       (20)   113274 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json
--rw-r--r--   0 garyt      (501) staff       (20)   133081 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)   127888 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   104088 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    39789 2023-12-21 14:29:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    18808 2024-03-04 22:17:52.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json
--rw-r--r--   0 garyt      (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.58/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.578575 nef_pipelines-0.1.58/src/nef_pipelines/lib/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garyt      (501) staff       (20)     1297 2024-02-10 20:21:35.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     1128 2024-03-05 09:00:53.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    20242 2024-03-04 21:59:44.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    15025 2024-03-05 09:04:37.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    24736 2024-03-27 21:52:56.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     6334 2024-03-19 22:25:46.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     6757 2024-03-19 22:25:48.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     9169 2024-04-04 07:42:49.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garyt      (501) staff       (20)    10315 2024-03-04 21:14:19.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.586544 nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    33455 2024-03-04 22:01:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/chem_comp.py
--rw-r--r--   0 garyt      (501) staff       (20)    20016 2024-03-04 22:01:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/io.py
--rw-r--r--   0 garyt      (501) staff       (20)     4325 2024-03-04 22:00:30.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/object_iter.py
--rw-r--r--   0 garyt      (501) staff       (20)     2494 2023-12-21 14:29:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/translator.py
--rw-r--r--   0 garyt      (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/translation_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garyt      (501) staff       (20)    27949 2024-03-19 22:43:06.000000 nef_pipelines-0.1.58/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     5431 2024-03-04 22:07:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/main.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.588127 nef_pipelines-0.1.58/src/nef_pipelines/nef_app/
--rw-r--r--   0 garyt      (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.631744 nef_pipelines-0.1.58/src/nef_pipelines/tests/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.640303 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/__init__.py
--rwxr--r--   0 garyt      (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.646179 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr--r--   0 garyt      (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garyt      (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_list.py
--rwxr--r--   0 garyt      (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garyt      (501) staff       (20)    10231 2024-03-04 21:31:42.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garyt      (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.649945 nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.655671 nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)       41 2024-02-10 20:33:34.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garyt      (501) staff       (20)      213 2024-02-10 20:33:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rwxr-xr-x   0 garyt      (501) staff       (20)      310 2024-02-10 20:33:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
--rw-r--r--   0 garyt      (501) staff       (20)     3065 2024-03-19 18:41:13.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.657846 nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.661516 nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
--rw-r--r--   0 garyt      (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/test_import_peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.663456 nef_pipelines-0.1.58/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.695503 nef_pipelines-0.1.58/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr--r--   0 garyt      (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr--r--   0 garyt      (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.707669 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.716715 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garyt      (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_delete.py
--rw-r--r--   0 garyt      (501) staff       (20)      251 2023-12-20 20:04:53.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_filter.py
--rwxr--r--   0 garyt      (501) staff       (20)     1964 2023-12-13 22:30:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garyt      (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_rename.py
--rwxr--r--   0 garyt      (501) staff       (20)     6921 2023-12-20 16:23:42.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_tabulate.py
--rwxr--r--   0 garyt      (501) staff       (20)    17146 2023-06-04 15:49:53.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_unassign.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.726339 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.760158 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
--rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
--rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/sparky_all.out
--rw-r--r--   0 garyt      (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
--rw-r--r--   0 garyt      (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     5489 2023-05-24 21:22:23.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.772403 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.798755 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garyt      (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr--r--   0 garyt      (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-r--r--   0 garyt      (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garyt      (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garyt      (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr--r--   0 garyt      (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr--r--   0 garyt      (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr-xr-x   0 garyt      (501) staff       (20)    25195 2024-02-10 20:33:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr-xr-x   0 garyt      (501) staff       (20)      233 2024-02-10 20:33:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr--r--   0 garyt      (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garyt      (501) staff       (20)      840 2024-03-04 21:16:11.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garyt      (501) staff       (20)      504 2023-09-13 11:17:50.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     4093 2024-02-10 20:35:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr--r--   0 garyt      (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.118090 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrstar/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.805573 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrstar/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)   235686 2024-03-04 22:09:35.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
--rw-r--r--   0 garyt      (501) staff       (20)   193009 2024-03-04 22:09:35.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.821973 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garyt      (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.878154 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garyt      (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr--r--   0 garyt      (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     1291 2023-08-23 12:07:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef
--rwxr--r--   0 garyt      (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garyt      (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     2172 2023-08-24 07:47:26.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garyt      (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garyt      (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garyt      (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garyt      (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garyt      (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     2742 2024-02-10 18:10:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr--r--   0 garyt      (501) staff       (20)     3881 2023-08-24 07:58:35.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     3847 2024-02-10 20:35:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr--r--   0 garyt      (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr--r--   0 garyt      (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.882861 nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.888924 nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr--r--   0 garyt      (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.893183 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.969053 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)    29541 2023-11-21 22:17:45.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
--rw-r--r--   0 garyt      (501) staff       (20)    19578 2023-11-21 22:17:45.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4195 2023-11-21 22:06:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     2395 2023-11-21 22:06:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     2254 2023-11-21 22:06:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
--rwxr--r--   0 garyt      (501) staff       (20)      800 2023-11-21 22:06:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)     7860 2023-12-20 18:35:13.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
--rwxr--r--   0 garyt      (501) staff       (20)     4316 2023-12-20 18:23:05.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.971488 nef_pipelines-0.1.58/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8438 2024-03-19 22:19:23.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.973242 nef_pipelines-0.1.58/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:33.983167 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.017813 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garyt      (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garyt      (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garyt      (501) staff       (20)      241 2023-04-26 21:06:26.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garyt      (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garyt      (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garyt      (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
--rw-r--r--   0 garyt      (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garyt      (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     4311 2023-05-21 12:09:19.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.027492 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-28 09:23:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.087736 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     2865 2024-02-10 20:30:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef
--rw-r--r--   0 garyt      (501) staff       (20)      314 2023-11-01 22:08:23.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/predS2_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/predSS_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1835 2023-09-13 21:31:11.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/pred_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1200 2023-09-15 21:17:38.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-09-13 21:31:11.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-11-01 22:00:48.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2870 2024-02-10 20:31:11.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/protonated_his.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/ubi_4.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
--rw-r--r--   0 garyt      (501) staff       (20)     5638 2023-11-05 11:38:38.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_export_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     1877 2023-11-01 22:08:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_import_order_parameters.py
--rw-r--r--   0 garyt      (501) staff       (20)     5825 2023-12-08 21:08:54.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_import_restraints.py
--rw-r--r--   0 garyt      (501) staff       (20)     3282 2023-12-07 10:10:58.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_secondary_structure.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.105481 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garyt      (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garyt      (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/header.nef
--rwxr--r--   0 garyt      (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garyt      (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2892 2024-02-10 20:30:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr--r--   0 garyt      (501) staff       (20)    64721 2024-03-19 22:16:54.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_header.py
--rwxr--r--   0 garyt      (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_nef_lib.py
--rwxr--r--   0 garyt      (501) staff       (20)     7625 2023-09-13 21:18:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_test.py
--rw-r--r--   0 garyt      (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/test_util.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.110992 nef_pipelines-0.1.58/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garyt      (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.138683 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.147317 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
--rw-r--r--   0 garyt      (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_data/basic.seq
--rw-r--r--   0 garyt      (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)      232 2024-03-27 22:29:35.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
--rw-r--r--   0 garyt      (501) staff       (20)     3392 2024-03-19 18:40:17.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_import_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     8984 2024-03-27 21:18:54.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.159078 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.203139 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garyt      (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garyt      (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garyt      (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garyt      (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garyt      (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garyt      (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garyt      (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garyt      (501) staff       (20)     8138 2023-10-30 22:33:08.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garyt      (501) staff       (20)     6577 2023-10-30 08:28:29.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garyt      (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garyt      (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    11089 2023-07-12 13:14:21.000000 nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.217588 nef_pipelines-0.1.58/src/nef_pipelines/tools/
--rw-r--r--   0 garyt      (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.225184 nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garyt      (501) staff       (20)      527 2023-01-02 20:40:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garyt      (501) staff       (20)     1466 2024-02-10 20:35:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garyt      (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garyt      (501) staff       (20)     9215 2024-03-04 21:23:23.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.249084 nef_pipelines-0.1.58/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garyt      (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.263075 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garyt      (501) staff       (20)      759 2023-12-21 14:29:05.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garyt      (501) staff       (20)     8838 2023-12-21 14:29:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/filter.py
--rw-r--r--   0 garyt      (501) staff       (20)     4100 2023-12-20 19:42:08.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garyt      (501) staff       (20)     7617 2024-02-10 20:35:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garyt      (501) staff       (20)     7774 2024-02-12 15:11:26.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garyt      (501) staff       (20)    19382 2023-12-20 16:24:01.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garyt      (501) staff       (20)    18444 2023-06-04 15:49:53.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/unassign.py
--rw-r--r--   0 garyt      (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garyt      (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.267491 nef_pipelines-0.1.58/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garyt      (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garyt      (501) staff       (20)    10539 2023-11-19 15:24:30.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.270619 nef_pipelines-0.1.58/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garyt      (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-03-19 22:27:40.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garyt      (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garyt      (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.58/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.271859 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.272232 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.277514 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    16493 2023-11-19 15:24:30.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/csv/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)    14955 2024-03-27 21:45:12.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.279792 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/echidna/
--rw-r--r--   0 garyt      (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/echidna/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.282113 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/echidna/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/echidna/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    15433 2023-05-21 12:09:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/echidna/importers/peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.284231 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garyt      (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.287827 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.291277 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     6385 2024-02-10 20:35:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.292929 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garyt      (501) staff       (20)      964 2023-05-24 21:21:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.301106 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     5933 2023-05-24 21:29:12.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garyt      (501) staff       (20)     4299 2023-02-15 22:21:28.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garyt      (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.305960 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11114 2024-03-27 21:50:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)    11619 2023-12-20 19:50:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.311874 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garyt      (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.343542 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2374 2023-12-20 20:02:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     3781 2023-09-13 21:22:39.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     2884 2023-10-30 22:24:14.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    22750 2023-11-19 15:24:30.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.347416 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/
--rw-r--r--   0 garyt      (501) staff       (20)      682 2024-03-19 07:46:08.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.352764 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-03-04 22:03:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7315 2024-03-19 22:53:21.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/importers/project.py
--rw-r--r--   0 garyt      (501) staff       (20)     5993 2024-03-19 07:42:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    24119 2024-03-15 17:31:35.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)      225 2024-03-19 07:46:07.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/nmrstar_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.375306 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garyt      (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.382398 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     7302 2024-02-10 18:10:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garyt      (501) staff       (20)     9136 2024-03-27 21:50:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.390483 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    16945 2023-11-21 22:15:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2313 2024-02-10 20:35:20.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     5749 2023-12-20 19:52:03.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.393225 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garyt      (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.396475 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)    10943 2023-11-21 22:15:33.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garyt      (501) staff       (20)     4817 2023-11-21 22:16:36.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.400580 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rcsb/
--rw-r--r--   0 garyt      (501) staff       (20)      454 2023-11-19 15:40:56.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rcsb/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.403480 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rcsb/importers/
--rw-r--r--   0 garyt      (501) staff       (20)     4829 2023-12-20 18:35:13.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rcsb/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    34787 2023-12-20 18:35:13.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.405515 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garyt      (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.408048 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11873 2024-03-27 21:50:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.416844 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garyt      (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.419175 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     9023 2024-03-27 22:18:33.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.422191 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garyt      (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.424709 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-18 23:32:17.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    15801 2024-02-10 22:15:24.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.430462 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8116 2024-03-04 21:43:45.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     9018 2024-03-27 21:44:50.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    17455 2024-03-27 21:18:54.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/sparky_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.433117 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/
--rw-r--r--   0 garyt      (501) staff       (20)      976 2023-10-31 09:11:23.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.435009 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8157 2023-12-07 22:13:01.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.442416 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     5134 2024-03-19 07:42:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/order_parameters.py
--rw-r--r--   0 garyt      (501) staff       (20)    16249 2024-03-27 21:50:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/restraints.py
--rw-r--r--   0 garyt      (501) staff       (20)     3747 2024-03-19 07:42:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py
--rw-r--r--   0 garyt      (501) staff       (20)     1834 2024-03-19 07:42:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     8576 2024-03-27 21:50:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/talos_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.443653 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garyt      (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.446336 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.468573 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/
--rw-r--r--   0 garyt      (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.482220 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/importers/
--rw-r--r--   0 garyt      (501) staff       (20)     2923 2024-03-27 21:18:54.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2852 2023-05-21 10:57:07.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     1865 2024-03-27 21:44:26.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    22539 2023-11-19 15:23:28.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.487925 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garyt      (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.490708 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7167 2023-11-21 22:15:00.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.496945 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2834 2024-03-27 21:18:54.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-03-27 21:50:51.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garyt      (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    39703 2023-10-30 22:21:37.000000 nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-04 07:43:34.499163 nef_pipelines-0.1.58/src/nef_pipelines.egg-info/
--rw-r--r--   0 garyt      (501) staff       (20)     9577 2024-04-04 07:43:32.000000 nef_pipelines-0.1.58/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garyt      (501) staff       (20)    20894 2024-04-04 07:43:33.000000 nef_pipelines-0.1.58/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garyt      (501) staff       (20)        1 2024-04-04 07:43:32.000000 nef_pipelines-0.1.58/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garyt      (501) staff       (20)       48 2024-04-04 07:43:32.000000 nef_pipelines-0.1.58/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garyt      (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.58/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garyt      (501) staff       (20)      426 2024-04-04 07:43:32.000000 nef_pipelines-0.1.58/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garyt      (501) staff       (20)       19 2024-04-04 07:43:32.000000 nef_pipelines-0.1.58/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garyt      (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.58/tox.ini
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.683214 nef_pipelines-0.1.59/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.575280 nef_pipelines-0.1.59/.github/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.653343 nef_pipelines-0.1.59/.github/workflows/
+-rw-r--r--   0 garyt      (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.59/.github/workflows/ci.yml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.663318 nef_pipelines-0.1.59/.idea/
+-rw-r--r--   0 garyt      (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.59/.idea/.gitignore
+-rw-r--r--   0 garyt      (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.59/.idea/.name
+-rw-r--r--   0 garyt      (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.59/.idea/NFC.iml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.666664 nef_pipelines-0.1.59/.idea/inspectionProfiles/
+-rw-r--r--   0 garyt      (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.59/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      229 2023-10-31 09:12:23.000000 nef_pipelines-0.1.59/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.59/.idea/modules.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.59/.idea/vcs.xml
+-rw-r--r--   0 garyt      (501) staff       (20)     1330 2024-02-09 22:26:45.000000 nef_pipelines-0.1.59/.pre-commit-config.yaml
+-rw-r--r--   0 garyt      (501) staff       (20)      490 2022-11-25 17:14:46.000000 nef_pipelines-0.1.59/.readthedocs.yml
+-rw-r--r--   0 garyt      (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.59/AUTHORS.md
+-rw-r--r--   0 garyt      (501) staff       (20)     6833 2024-04-07 09:36:37.000000 nef_pipelines-0.1.59/CHANGELOG.md
+-rw-r--r--   0 garyt      (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.59/CONTRIBUTING.md
+-rw-r--r--   0 garyt      (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.59/LICENSE.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     9577 2024-04-07 09:37:22.682904 nef_pipelines-0.1.59/PKG-INFO
+-rw-r--r--   0 garyt      (501) staff       (20)     8212 2024-03-04 22:23:39.000000 nef_pipelines-0.1.59/README.md
+-rw-r--r--   0 garyt      (501) staff       (20)      807 2023-05-21 15:23:42.000000 nef_pipelines-0.1.59/TODO.md
+-rw-r--r--   0 garyt      (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.59/pyproject.toml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.670455 nef_pipelines-0.1.59/references/
+-rw-r--r--   0 garyt      (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.59/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garyt      (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.59/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rwxr--r--   0 garyt      (501) staff       (20)     1264 2024-03-19 22:32:32.000000 nef_pipelines-0.1.59/release_to_pypi.sh
+-rw-r--r--   0 garyt      (501) staff       (20)      351 2024-03-27 22:48:52.000000 nef_pipelines-0.1.59/requirements.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     1697 2024-04-07 09:37:22.684390 nef_pipelines-0.1.59/setup.cfg
+-rw-r--r--   0 garyt      (501) staff       (20)      710 2022-11-25 17:14:46.000000 nef_pipelines-0.1.59/setup.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.576822 nef_pipelines-0.1.59/src/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.702637 nef_pipelines-0.1.59/src/nef_pipelines/
+-rw-r--r--   0 garyt      (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.59/src/nef_pipelines/VERSION
+-rw-r--r--   0 garyt      (501) staff       (20)      577 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.725389 nef_pipelines-0.1.59/src/nef_pipelines/data/
+-rw-r--r--   0 garyt      (501) staff       (20)    16381 2024-03-04 22:17:52.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/ambiguity_translations.json
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.902644 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/
+-rw-r--r--   0 garyt      (501) staff       (20)   108495 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104358 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json
+-rw-r--r--   0 garyt      (501) staff       (20)   118386 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102566 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json
+-rw-r--r--   0 garyt      (501) staff       (20)   108304 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)    91086 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)    35009 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   109165 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   105025 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json
+-rw-r--r--   0 garyt      (501) staff       (20)   119258 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102439 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json
+-rw-r--r--   0 garyt      (501) staff       (20)    96862 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json
+-rw-r--r--   0 garyt      (501) staff       (20)    99315 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    35085 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    73745 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json
+-rw-r--r--   0 garyt      (501) staff       (20)   151265 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102950 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json
+-rw-r--r--   0 garyt      (501) staff       (20)    96313 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    99814 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104993 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json
+-rw-r--r--   0 garyt      (501) staff       (20)   110515 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json
+-rw-r--r--   0 garyt      (501) staff       (20)    67204 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json
+-rw-r--r--   0 garyt      (501) staff       (20)   127933 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json
+-rw-r--r--   0 garyt      (501) staff       (20)   119775 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json
+-rw-r--r--   0 garyt      (501) staff       (20)   113627 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json
+-rw-r--r--   0 garyt      (501) staff       (20)   150013 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   103831 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   112702 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json
+-rw-r--r--   0 garyt      (501) staff       (20)    89442 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)    89294 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json
+-rw-r--r--   0 garyt      (501) staff       (20)   113274 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json
+-rw-r--r--   0 garyt      (501) staff       (20)   133081 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)   127888 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104088 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    39789 2023-12-21 14:29:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    18808 2024-03-04 22:17:52.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json
+-rw-r--r--   0 garyt      (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.59/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.936816 nef_pipelines-0.1.59/src/nef_pipelines/lib/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1297 2024-02-10 20:21:35.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1128 2024-03-05 09:00:53.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2848 2024-04-06 16:53:23.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20242 2024-03-04 21:59:44.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15479 2024-04-07 09:31:44.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    25699 2024-04-06 13:43:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6334 2024-03-19 22:25:46.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6757 2024-03-19 22:25:48.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9169 2024-04-06 16:21:33.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10315 2024-03-04 21:14:19.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.952027 nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    33455 2024-03-04 22:01:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/chem_comp.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20016 2024-03-04 22:01:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/io.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4325 2024-03-04 22:00:30.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/object_iter.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2494 2023-12-21 14:29:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/translator.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garyt      (501) staff       (20)    27949 2024-03-19 22:43:06.000000 nef_pipelines-0.1.59/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     5431 2024-03-04 22:07:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/main.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.955987 nef_pipelines-0.1.59/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garyt      (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.982706 nef_pipelines-0.1.59/src/nef_pipelines/tests/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.989435 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/__init__.py
+-rwxr--r--   0 garyt      (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.002918 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_list.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10231 2024-03-04 21:31:42.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garyt      (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.005904 nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.008100 nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)       41 2024-02-10 20:33:34.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garyt      (501) staff       (20)      213 2024-02-10 20:33:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rwxr-xr-x   0 garyt      (501) staff       (20)      310 2024-02-10 20:33:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
+-rw-r--r--   0 garyt      (501) staff       (20)     3065 2024-03-19 18:41:13.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.009292 nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.055831 nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     3621 2024-04-07 09:20:05.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.058357 nef_pipelines-0.1.59/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.061013 nef_pipelines-0.1.59/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)       13 2024-04-07 09:17:12.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)     3405 2024-04-07 09:19:50.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.069020 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.072041 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_delete.py
+-rw-r--r--   0 garyt      (501) staff       (20)      251 2023-12-20 20:04:53.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_filter.py
+-rwxr--r--   0 garyt      (501) staff       (20)     1964 2023-12-13 22:30:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr--r--   0 garyt      (501) staff       (20)     6921 2023-12-20 16:23:42.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_tabulate.py
+-rwxr--r--   0 garyt      (501) staff       (20)    17146 2023-06-04 15:49:53.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_unassign.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.076124 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.085042 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
+-rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
+-rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/sparky_all.out
+-rw-r--r--   0 garyt      (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6221 2024-04-07 09:31:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.111426 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.132510 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr--r--   0 garyt      (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-r--r--   0 garyt      (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garyt      (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garyt      (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr--r--   0 garyt      (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr--r--   0 garyt      (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr-xr-x   0 garyt      (501) staff       (20)    25195 2024-02-10 20:33:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr-xr-x   0 garyt      (501) staff       (20)      233 2024-02-10 20:33:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr--r--   0 garyt      (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garyt      (501) staff       (20)      840 2024-03-04 21:16:11.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garyt      (501) staff       (20)      504 2023-09-13 11:17:50.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4093 2024-02-10 20:35:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr--r--   0 garyt      (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:21.583731 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrstar/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.136287 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrstar/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)   235686 2024-03-04 22:09:35.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
+-rw-r--r--   0 garyt      (501) staff       (20)   193009 2024-03-04 22:09:35.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.160473 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.176813 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr--r--   0 garyt      (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     1291 2023-08-23 12:07:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garyt      (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     2172 2023-08-24 07:47:26.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garyt      (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garyt      (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garyt      (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garyt      (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr--r--   0 garyt      (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2742 2024-02-10 18:10:55.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr--r--   0 garyt      (501) staff       (20)     3881 2023-08-24 07:58:35.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     3847 2024-02-10 20:35:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr--r--   0 garyt      (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr--r--   0 garyt      (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.178111 nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.180330 nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr--r--   0 garyt      (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.182266 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.192848 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)    29541 2023-11-21 22:17:45.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
+-rw-r--r--   0 garyt      (501) staff       (20)    19578 2023-11-21 22:17:45.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4195 2023-11-21 22:06:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     2395 2023-11-21 22:06:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     2254 2023-11-21 22:06:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2023-11-21 22:06:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
+-rwxr--r--   0 garyt      (501) staff       (20)     7860 2023-12-20 18:35:13.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
+-rwxr--r--   0 garyt      (501) staff       (20)     4316 2023-12-20 18:23:05.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.195043 nef_pipelines-0.1.59/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8438 2024-04-07 09:31:44.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.199024 nef_pipelines-0.1.59/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.227376 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.309368 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garyt      (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garyt      (501) staff       (20)      241 2023-04-26 21:06:26.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garyt      (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4314 2024-04-07 09:31:37.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.316518 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-28 09:23:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.335826 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     2865 2024-02-10 20:30:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      314 2023-11-01 22:08:23.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/predS2_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/predSS_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1835 2023-09-13 21:31:11.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/pred_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1200 2023-09-15 21:17:38.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-09-13 21:31:11.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-11-01 22:00:48.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2870 2024-02-10 20:31:11.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/protonated_his.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/ubi_4.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     5638 2023-11-05 11:38:38.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_export_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1877 2023-11-01 22:08:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_import_order_parameters.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5825 2023-12-08 21:08:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_import_restraints.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3282 2023-12-07 10:10:58.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_secondary_structure.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.341916 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garyt      (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/header.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2892 2024-02-10 20:30:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr--r--   0 garyt      (501) staff       (20)    64721 2024-03-19 22:16:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_header.py
+-rwxr--r--   0 garyt      (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     7636 2024-04-06 13:42:48.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_test.py
+-rw-r--r--   0 garyt      (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/test_util.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.342830 nef_pipelines-0.1.59/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garyt      (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.348420 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.352396 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_data/basic.seq
+-rw-r--r--   0 garyt      (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      232 2024-03-27 22:29:35.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
+-rw-r--r--   0 garyt      (501) staff       (20)     3392 2024-04-07 09:31:44.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_import_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8984 2024-03-27 21:18:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.364872 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.381014 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garyt      (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garyt      (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)     8138 2023-10-30 22:33:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6577 2023-10-30 08:28:29.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11089 2023-07-12 13:14:21.000000 nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.413996 nef_pipelines-0.1.59/src/nef_pipelines/tools/
+-rw-r--r--   0 garyt      (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.421331 nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garyt      (501) staff       (20)      527 2023-01-02 20:40:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1466 2024-02-10 20:35:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9215 2024-03-04 21:23:23.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.423695 nef_pipelines-0.1.59/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garyt      (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.437125 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garyt      (501) staff       (20)      738 2024-04-06 15:19:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8838 2023-12-21 14:29:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/filter.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4100 2023-12-20 19:42:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7617 2024-02-10 20:35:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7774 2024-02-12 15:11:26.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garyt      (501) staff       (20)    19382 2023-12-20 16:24:01.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garyt      (501) staff       (20)    18444 2023-06-04 15:49:53.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/unassign.py
+-rw-r--r--   0 garyt      (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.442403 nef_pipelines-0.1.59/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garyt      (501) staff       (20)      366 2024-04-06 16:50:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/peaks/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-04-06 15:34:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10539 2023-11-19 15:24:30.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.448520 nef_pipelines-0.1.59/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garyt      (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-03-19 22:27:40.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garyt      (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.59/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.450006 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.450466 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.455103 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16493 2023-11-19 15:24:30.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/csv/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)    14955 2024-03-27 21:45:12.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.457692 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garyt      (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.460969 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15420 2024-04-07 09:21:28.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.462057 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garyt      (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.465345 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.468108 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6680 2024-04-06 13:44:59.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.468953 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garyt      (501) staff       (20)      964 2023-05-24 21:21:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.493960 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5929 2024-04-06 13:45:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4326 2024-04-06 13:45:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garyt      (501) staff       (20)      826 2024-04-06 13:45:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5998 2024-04-06 13:45:32.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.498045 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11101 2024-04-06 16:52:09.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11631 2024-04-06 16:51:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.546864 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garyt      (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.552302 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2374 2023-12-20 20:02:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3781 2023-09-13 21:22:39.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2884 2023-10-30 22:24:14.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    22750 2023-11-19 15:24:30.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.555208 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/
+-rw-r--r--   0 garyt      (501) staff       (20)      682 2024-03-19 07:46:08.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.561206 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-03-04 22:03:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7315 2024-03-19 22:53:21.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/importers/project.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5993 2024-03-19 07:42:55.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    24119 2024-03-15 17:31:35.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)      225 2024-03-19 07:46:07.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/nmrstar_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.566645 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garyt      (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.574265 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7302 2024-02-10 18:10:55.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9136 2024-03-27 21:50:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.580334 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16945 2023-11-21 22:15:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2313 2024-02-10 20:35:20.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5749 2023-12-20 19:52:03.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.582810 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garyt      (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.585065 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)    10943 2023-11-21 22:15:33.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4817 2023-11-21 22:16:36.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.588310 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rcsb/
+-rw-r--r--   0 garyt      (501) staff       (20)      454 2023-11-19 15:40:56.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rcsb/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.591022 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rcsb/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)     4829 2023-12-20 18:35:13.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rcsb/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    34787 2023-12-20 18:35:13.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.591972 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garyt      (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.593236 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11873 2024-03-27 21:50:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.595162 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garyt      (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.596438 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9023 2024-03-27 22:18:33.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.599627 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garyt      (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.634130 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-18 23:32:17.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15801 2024-02-10 22:15:24.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.639230 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8116 2024-03-04 21:43:45.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9018 2024-03-27 21:44:50.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    17455 2024-03-27 21:18:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.642229 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/
+-rw-r--r--   0 garyt      (501) staff       (20)      976 2023-10-31 09:11:23.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.645033 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8157 2023-12-07 22:13:01.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.650468 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5134 2024-03-19 07:42:55.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/order_parameters.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16249 2024-03-27 21:50:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/restraints.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3747 2024-03-19 07:42:55.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1834 2024-03-19 07:42:55.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8576 2024-03-27 21:50:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/talos_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.651884 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garyt      (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.654788 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.660272 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/
+-rw-r--r--   0 garyt      (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.667000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)     2923 2024-03-27 21:18:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2852 2023-05-21 10:57:07.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1865 2024-03-27 21:44:26.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    22539 2023-11-19 15:23:28.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.673033 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garyt      (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.674694 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7167 2023-11-21 22:15:00.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.679810 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2834 2024-03-27 21:18:54.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-03-27 21:50:51.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    39703 2023-10-30 22:21:37.000000 nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-07 09:37:22.681575 nef_pipelines-0.1.59/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garyt      (501) staff       (20)     9577 2024-04-07 09:37:21.000000 nef_pipelines-0.1.59/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garyt      (501) staff       (20)    20993 2024-04-07 09:37:21.000000 nef_pipelines-0.1.59/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        1 2024-04-07 09:37:21.000000 nef_pipelines-0.1.59/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garyt      (501) staff       (20)       48 2024-04-07 09:37:21.000000 nef_pipelines-0.1.59/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.59/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garyt      (501) staff       (20)      426 2024-04-07 09:37:21.000000 nef_pipelines-0.1.59/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garyt      (501) staff       (20)       19 2024-04-07 09:37:21.000000 nef_pipelines-0.1.59/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.59/tox.ini
```

### Comparing `nef_pipelines-0.1.58/.github/workflows/ci.yml` & `nef_pipelines-0.1.59/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.59/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/.pre-commit-config.yaml` & `nef_pipelines-0.1.59/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/CHANGELOG.md` & `nef_pipelines-0.1.59/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -244,7 +244,12 @@
 ## version 0.1.57
 - upgrade pyparsing and pynmrstar
   1. pyparsing was triggering a deprication warning
   2. pynmrstar had a bug in renaming frames
 
 ## version 0.1.58
 - corrected a bug in Linking lookup in the nmrstar project subcommand that affected some python versions
+
+## version 0.1.59
+- corrected a bug in fasta sequence importer that affected files with spaces between residues
+- improve handling of figures of merit especially for MARS peak imports
+- correct spectrum dimension transfers were not correct in peak imports
```

### Comparing `nef_pipelines-0.1.58/CONTRIBUTING.md` & `nef_pipelines-0.1.59/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/LICENSE.txt` & `nef_pipelines-0.1.59/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/PKG-INFO` & `nef_pipelines-0.1.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.58
+Version: 0.1.59
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.58/README.md` & `nef_pipelines-0.1.59/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/TODO.md` & `nef_pipelines-0.1.59/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.59/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.59/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/release_to_pypi.sh` & `nef_pipelines-0.1.59/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/setup.cfg` & `nef_pipelines-0.1.59/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/setup.py` & `nef_pipelines-0.1.59/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/ambiguity_translations.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/ambiguity_translations.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json` & `nef_pipelines-0.1.59/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.59/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 SF_CATEGORY = f"{SF}_category"
 SF_FRAMECODE = f"{SF}_framecode"
 NUM_DIMENSIONS = "num_dimensions"
 CHEMICAL_SHIFT_LIST = "chemical_shift_list"
 EXPERIMENT_TYPE = "experiment_type"
 EXPERIMENT_CLASSIFICATION = "experiment_classification"
 CCPN_COMMENT = "ccpn_comment"
+CCPN_MERIT = "ccpn_figure_of_merit"
 
 SPECTRUM_FRAME_TAGS = (
     SF_CATEGORY,
     SF_FRAMECODE,
     NUM_DIMENSIONS,
     CHEMICAL_SHIFT_LIST,
     EXPERIMENT_CLASSIFICATION,
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/peak_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from nef_pipelines.lib.nef_frames_lib import (
     ABSOLUTE_PEAK_POSITIONS,
     ATOM_NAME,
     ATOM_NAME__DIMENSION_INDEX,
     AXIS_CODE,
     AXIS_UNIT,
     CCPN_COMMENT,
+    CCPN_MERIT,
     CHAIN_CODE,
     CHAIN_CODE__DIMENSION_INDEX,
     CHEMICAL_SHIFT_LIST,
     DIMENSION__DIMENSION_INDEX,
     DIMENSION_ID,
     DIMENSION_INDEX,
     DIMENSION_LOOP_TAGS,
@@ -204,14 +205,20 @@
 
     have_comments = False
     for peak in peaks:
         if peak.comment != "":
             have_comments = True
             break
 
+    have_merits = False
+    for peak in peaks:
+        if peak.figure_of_merit != UNUSED and peak.figure_of_merit is not None:
+            have_merits = True
+            break
+
     peak_dimensions = []
     for peak in peaks:
         peak_dimensions.append(len(peak.shifts))
 
     peak_dimensions.sort()
     peak_dimensions = remove_duplicates_stable(peak_dimensions)
 
@@ -225,15 +232,15 @@
     frame.add_tag(NUM_DIMENSIONS, peak_dimensions[0])
 
     shift_list_name = (
         extra_tags[CHEMICAL_SHIFT_LIST] if CHEMICAL_SHIFT_LIST in extra_tags else UNUSED
     )
     frame.add_tag(
         CHEMICAL_SHIFT_LIST, shift_list_name
-    )  # technically not correct to use unused bye default here but this is a nef file building
+    )  # technically not correct to use unused by default here but this is a nef file building
     # tool kit so an empty shift list maybe what we need
     # we may need to add a flag to build the shift list on the fly at a later date...
 
     experiment_classification = (
         extra_tags[EXPERIMENT_CLASSIFICATION]
         if EXPERIMENT_CLASSIFICATION in extra_tags
         else UNUSED
@@ -292,16 +299,16 @@
         for dimension_index in range(1, len(dimensions) + 1)
     ]
     transfer_loop_tags = _expand_templates(TRANSFER_LOOP_TAGS, dimension_indices)
 
     transfer_loop.add_tag(transfer_loop_tags)
 
     for dim_index in range(1, len(dimensions)):
-        dim_1 = i
-        dim_2 = i + 1
+        dim_1 = dim_index
+        dim_2 = dim_index + 1
 
         transfer_data = {
             DIMENSION__DIMENSION_INDEX.format(**{DIMENSION_INDEX: dim_1}): dim_1,
             DIMENSION__DIMENSION_INDEX.format(**{DIMENSION_INDEX: dim_2}): dim_2,
             TRANSFER_TYPE: ONE_BOND,
             IS_INDIRECT: NEF_FALSE,
         }
@@ -312,55 +319,62 @@
             ]
         )
 
     peak_loop = Loop.from_scratch(SPECTRUM_PEAK_LOOP_CATEGORY)
     frame.add_loop(peak_loop)
 
     peak_loop_tags = _expand_templates(PEAK_LOOP_TAGS, dimension_indices)
+
     if have_comments:
         peak_loop_tags.append(CCPN_COMMENT)
 
+    if have_merits:
+        peak_loop_tags.append(CCPN_MERIT)
+
     peak_loop.add_tag(peak_loop_tags)
 
     for index, peak in enumerate(peaks):
         peak_data = {
             INDEX: index,
             PEAK_ID: index if peak.id is None else peak.id,
             HEIGHT: peak.height,
             HEIGHT_UNCERTAINTY: peak.height_uncertainty,
             VOLUME: peak.volume,
             VOLUME_UNCERTAINTY: peak.volume_uncertainty,
         }
 
         for dim_index, shift in enumerate(peak.shifts, start=1):
-            peak_data[
-                CHAIN_CODE__DIMENSION_INDEX.format(dimension_index=dim_index)
-            ] = shift.atom.residue.chain_code
+            peak_data[CHAIN_CODE__DIMENSION_INDEX.format(dimension_index=dim_index)] = (
+                shift.atom.residue.chain_code
+            )
             peak_data[
                 SEQUENCE_CODE__DIMENSION_INDEX.format(dimension_index=dim_index)
             ] = shift.atom.residue.sequence_code
             peak_data[
                 RESIDUE_NAME__DIMENSION_INDEX.format(dimension_index=dim_index)
             ] = shift.atom.residue.residue_name
-            peak_data[
-                ATOM_NAME__DIMENSION_INDEX.format(dimension_index=dim_index)
-            ] = shift.atom.atom_name
-
-            peak_data[
-                POSITION__DIMENSION_INDEX.format(dimension_index=dim_index)
-            ] = shift.value
+            peak_data[ATOM_NAME__DIMENSION_INDEX.format(dimension_index=dim_index)] = (
+                shift.atom.atom_name
+            )
+
+            peak_data[POSITION__DIMENSION_INDEX.format(dimension_index=dim_index)] = (
+                shift.value
+            )
             peak_data[
                 POSITION_UNCERTAINTY__DIMENSION_INDEX.format(dimension_index=dim_index)
             ] = shift.value_uncertainty
 
             if have_comments:
                 peak_data[CCPN_COMMENT] = (
                     peak.comment if peak.comment is not None else UNUSED
                 )
-
+            if have_merits:
+                peak_data[CCPN_MERIT] = (
+                    peak.figure_of_merit if peak.figure_of_merit is not None else UNUSED
+                )
         peak_loop.add_data(
             [
                 peak_data,
             ]
         )
 
     return frame
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/sequence_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import string
 from collections import Counter
 from dataclasses import replace
 from enum import auto
 from pathlib import Path
 from textwrap import dedent
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
@@ -225,15 +226,45 @@
 
 
 class BadResidue(Exception):
     """
     Bad residue found in a sequence
     """
 
-    pass
+    def __init__(self, residue_name, error_pos, sequence_string):
+
+        self.residue_name = residue_name
+        self.sequence_string = sequence_string
+        self.error_pos = error_pos
+
+    def __str__(self):
+        try:
+            terminal_width = os.get_terminal_size().columns
+        except OSError:
+            terminal_width = 80
+
+        error_pos_string = [
+            " ",
+        ] * len(self.sequence_string)
+        error_pos_string[self.error_pos] = "^"
+        error_pos_string = "".join(error_pos_string)
+
+        msg = f"""\
+        unknown residue {self.residue_name}
+        at residue {self.error_pos+1}
+        sequence:
+        """
+        msg = dedent(msg)
+        sequence_string_chunks = list(chunks(self.sequence_string, terminal_width - 10))
+        pos_string_chunks = list(chunks(error_pos_string, terminal_width - 10))
+        for sequence_chunk, pos_chunk in zip(sequence_string_chunks, pos_string_chunks):
+            msg += f"{''.join(sequence_chunk)}\n"
+            msg += f"{''.join(pos_chunk)}\n"
+
+        return msg
 
 
 def translate_1_to_3(
     sequence: str, molecule_type=MoleculeTypes.PROTEIN, unknown: Optional[str] = None
 ) -> List[str]:
     """
     Translate a 1 letter sequence to a 3 letter sequence
@@ -248,30 +279,27 @@
 
     """
 
     translations = TRANSLATIONS_1_3[molecule_type]
 
     result = []
     for i, residue_name_1let in enumerate(sequence):
+        if residue_name_1let == " ":
+            continue
+        original_residue_name_1let = residue_name_1let
         residue_name_1let = residue_name_1let.upper()
         if translations is None:
             result.append(residue_name_1let)
         elif residue_name_1let in translations:
             result.append(translations[residue_name_1let])
         else:
             if unknown:
                 result.append(unknown)
             else:
-                msg = f"""\
-                     unknown residue {residue_name_1let} at residue {i+1}
-                     sequence: {sequence}
-                               {(' ' * i) + '^'}
-                """
-                msg = dedent(msg)
-                raise BadResidue(msg)
+                raise BadResidue(original_residue_name_1let, i, sequence)
 
     return result
 
 
 def translate_3_to_1(
     sequence: List[str], molecule_type=MoleculeTypes.PROTEIN
 ) -> List[str]:
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/structures.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/chem_comp.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/chem_comp.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/io.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/io.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/object_iter.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/object_iter.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/translation/translator.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/translation/translator.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/translation_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/translation_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.59/src/nef_pipelines/lib/util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/main.py` & `nef_pipelines-0.1.59/src/nef_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/test_import_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/echidna/test_import_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/echidna/test_import_peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,17 @@
    _nef_peak.position_uncertainty_1
    _nef_peak.position_2
    _nef_peak.position_uncertainty_2
    _nef_peak.height
    _nef_peak.height_uncertainty
    _nef_peak.volume
    _nef_peak.volume_uncertainty
-   _nef_peak.ccpn_merit
+   _nef_peak.ccpn_figure_of_merit
    _nef_peak.ccpn_comment
+
   0    0    A   10   ALA   N   A   10   ALA   H   122.836   .   7.826   .   .   .   .   .   6.03818   'large violation!'
   1    1    A   11   ALA   N   A   11   ALA   H   118.678   .   8.063   .   .   .   .   .   6.36477   'large violation!'
   2    2    A   12   ALA   N   A   12   ALA   H   119.301   .   7.842   .   .   .   .   .   4.6192    'large violation!'
   3    3    A   13   ALA   N   A   13   ALA   H   122.946   .   8.232   .   .   .   .   .   3.63582   'large violation!'
   4    4    A   14   ALA   N   A   14   ALA   H   120.475   .   8.948   .   .   .   .   .   3.07293   .
   5    5    A   15   ALA   N   A   15   ALA   H   118.138   .   8.798   .   .   .   .   .   2.89933   .
   6    6    A   16   ALA   N   A   16   ALA   H   120.784   .   8.035   .   .   .   .   .   3.00885   .
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,24 +35,34 @@
 
    stop_
 
 save_"""
 
 
 # noinspection PyUnusedLocal
-def test_3aa(clear_cache):
+def test_3aa():
 
     path = path_in_test_data(__file__, "3aa.fasta")
     result = run_and_report(app, [path])
 
     mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
     assert_lines_match(EXPECTED_3AA, mol_sys_result)
 
 
+def test_3aa_spaces():
+
+    path = path_in_test_data(__file__, "3aa_spaces.fasta")
+    result = run_and_report(app, [path])
+
+    mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
+
+    assert_lines_match(EXPECTED_3AA, mol_sys_result)
+
+
 EXPECTED_3A_AB = """\
 save_nef_molecular_system
    _nef_molecular_system.sf_category   nef_molecular_system
    _nef_molecular_system.sf_framecode  nef_molecular_system
 
    loop_
       _nef_sequence.index
@@ -72,15 +82,15 @@
 
    stop_
 
 save_"""
 
 
 # noinspection PyUnusedLocal
-def test_3aa_x2(clear_cache):
+def test_3aa_x2():
 
     path = path_in_test_data(__file__, "3aa_x2.fasta")
     result = run_and_report(app, [path])
 
     assert result.exit_code == 0
 
     mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
@@ -111,15 +121,15 @@
 
    stop_
 
 save_"""
 
 
 # noinspection PyUnusedLocal
-def test_3aa_x2_off_10_b(clear_cache):
+def test_3aa_x2_off_10_b():
 
     path = path_in_test_data(__file__, "3aa_x2.fasta")
     result = run_and_report(app, ["--starts", "1,11", path])
 
     mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
     assert_lines_match(EXPECTED_3A_AB_B_start_11, mol_sys_result)
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/frames/test_unassign.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/frames/test_unassign.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_import_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_import_peaks.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,16 +7,17 @@
     run_and_report,
 )
 from nef_pipelines.transcoders.mars.importers.peaks import peaks
 
 app = typer.Typer()
 app.command()(peaks)
 
-
+NOQUA_E501 = "# noqa E501"
 EXPECTED_HNCA = """
+# noqa E501
 loop_
     _nef_peak.index
     _nef_peak.peak_id
     _nef_peak.chain_code_1
     _nef_peak.sequence_code_1
     _nef_peak.residue_name_1
     _nef_peak.atom_name_1
@@ -34,28 +35,34 @@
     _nef_peak.position_uncertainty_2
     _nef_peak.position_3
     _nef_peak.position_uncertainty_3
     _nef_peak.height
     _nef_peak.height_uncertainty
     _nef_peak.volume
     _nef_peak.volume_uncertainty
+    _nef_peak.ccpn_comment
+    _nef_peak.ccpn_figure_of_merit
+
 
-    0   0   A   1   MET   CA   A   2   GLN   N   A   2   GLN   H   54.608   .   122.899   .   8.907   .   .   .   .   .
-    1   1   A   2   GLN   CA   A   2   GLN   N   A   2   GLN   H   55.215   .   122.899   .   8.907   .   .   .   .   .
-    2   2   A   2   GLN   CA   A   3   ILE   N   A   3   ILE   H   55.057   .   115.127   .   8.318   .   .   .   .   .
-    3   3   A   3   ILE   CA   A   3   ILE   N   A   3   ILE   H   59.616   .   115.127   .   8.318   .   .   .   .   .
-    4   4   A   3   ILE   CA   A   4   PHE   N   A   4   PHE   H   59.599   .   118.73    .   8.614   .   .   .   .   .
-    5   5   A   4   PHE   CA   A   4   PHE   N   A   4   PHE   H   55.138   .   118.73    .   8.614   .   .   .   .   .
-    6   6   A   4   PHE   CA   A   5   VAL   N   A   5   VAL   H   55.142   .   121.424   .   9.307   .   .   .   .   .
-    7   7   A   5   VAL   CA   A   5   VAL   N   A   5   VAL   H   60.412   .   121.424   .   9.307   .   .   .   .   .
+    0   0   A   1   MET   CA   A   2   GLN   N   A   2   GLN   H   54.608   .   122.899   .   8.907   .   .   .   .   .      merit=M   0.75
+    1   1   A   2   GLN   CA   A   2   GLN   N   A   2   GLN   H   55.215   .   122.899   .   8.907   .   .   .   .   .      merit=M   0.75
+    2   2   A   2   GLN   CA   A   3   ILE   N   A   3   ILE   H   55.057   .   115.127   .   8.318   .   .   .   .   .      merit=M   0.75
+    3   3   A   3   ILE   CA   A   3   ILE   N   A   3   ILE   H   59.616   .   115.127   .   8.318   .   .   .   .   .      merit=M   0.75
+    4   4   A   3   ILE   CA   A   4   PHE   N   A   4   PHE   H   59.599   .   118.73    .   8.614   .   .   .   .   .      merit=H   1.0
+    5   5   A   4   PHE   CA   A   4   PHE   N   A   4   PHE   H   55.138   .   118.73    .   8.614   .   .   .   .   .      merit=H   1.0
+    6   6   A   4   PHE   CA   A   5   VAL   N   A   5   VAL   H   55.142   .   121.424   .   9.307   .   .   .   .   .      merit=H   1.0
+    7   7   A   5   VAL   CA   A   5   VAL   N   A   5   VAL   H   60.412   .   121.424   .   9.307   .   .   .   .   .      merit=H   1.0
 
 stop_
-"""
+""".replace(
+    NOQUA_E501, ""
+)
 
 EXPECTED_HNcoCA = """
+# noqa E501
 loop_
     _nef_peak.index
     _nef_peak.peak_id
     _nef_peak.chain_code_1
     _nef_peak.sequence_code_1
     _nef_peak.residue_name_1
     _nef_peak.atom_name_1
@@ -73,23 +80,30 @@
     _nef_peak.position_uncertainty_2
     _nef_peak.position_3
     _nef_peak.position_uncertainty_3
     _nef_peak.height
     _nef_peak.height_uncertainty
     _nef_peak.volume
     _nef_peak.volume_uncertainty
+    _nef_peak.ccpn_comment
+    _nef_peak.ccpn_figure_of_merit
+
 
-    0   0   A   1   MET   CA   A   2   GLN   N   A   2   GLN   H   54.608   .   122.899   .   8.907   .   .   .   .   .
-    1   1   A   2   GLN   CA   A   3   ILE   N   A   3   ILE   H   55.057   .   115.127   .   8.318   .   .   .   .   .
-    2   2   A   3   ILE   CA   A   4   PHE   N   A   4   PHE   H   59.599   .   118.73    .   8.614   .   .   .   .   .
-    3   3   A   4   PHE   CA   A   5   VAL   N   A   5   VAL   H   55.142   .   121.424   .   9.307   .   .   .   .   .
+    0   0   A   1   MET   CA   A   2   GLN   N   A   2   GLN   H   54.608   .   122.899   .   8.907   .   .   .   .   .     merit=M   0.75
+    1   1   A   2   GLN   CA   A   3   ILE   N   A   3   ILE   H   55.057   .   115.127   .   8.318   .   .   .   .   .     merit=M   0.75
+    2   2   A   3   ILE   CA   A   4   PHE   N   A   4   PHE   H   59.599   .   118.73    .   8.614   .   .   .   .   .     merit=H   1.0
+    3   3   A   4   PHE   CA   A   5   VAL   N   A   5   VAL   H   55.142   .   121.424   .   9.307   .   .   .   .   .     merit=H   1.0
 stop_
-"""
+""".replace(
+    NOQUA_E501, ""
+)
+
 
 EXPECTED_all = """
+# noqa E501
 loop_
     _nef_peak.index
     _nef_peak.peak_id
     _nef_peak.chain_code_1
     _nef_peak.sequence_code_1
     _nef_peak.residue_name_1
     _nef_peak.atom_name_1
@@ -107,25 +121,30 @@
     _nef_peak.position_uncertainty_2
     _nef_peak.position_3
     _nef_peak.position_uncertainty_3
     _nef_peak.height
     _nef_peak.height_uncertainty
     _nef_peak.volume
     _nef_peak.volume_uncertainty
+    _nef_peak.ccpn_comment
+    _nef_peak.ccpn_figure_of_merit
 
-    0   0   A   1   MET   CA   A   2   GLN   N   A   2   GLN   H   54.608   .   122.899   .   8.907   .   .   .   .   .
-    1   1   A   1   MET   CB   A   2   GLN   N   A   2   GLN   H   33.279   .   122.899   .   8.907   .   .   .   .   .
-    2   2   A   2   GLN   CA   A   2   GLN   N   A   2   GLN   H   55.215   .   122.899   .   8.907   .   .   .   .   .
-    3   3   A   2   GLN   CB   A   2   GLN   N   A   2   GLN   H   30.606   .   122.899   .   8.907   .   .   .   .   .
-    4   4   A   2   GLN   CA   A   3   ILE   N   A   3   ILE   H   55.057   .   115.127   .   8.318   .   .   .   .   .
-    5   5   A   2   GLN   CB   A   3   ILE   N   A   3   ILE   H   30.582   .   115.127   .   8.318   .   .   .   .   .
-    6   6   A   3   ILE   CA   A   3   ILE   N   A   3   ILE   H   59.616   .   115.127   .   8.318   .   .   .   .   .
-    7   7   A   3   ILE   CB   A   3   ILE   N   A   3   ILE   H   42.025   .   115.127   .   8.318   .   .   .   .   .
+
+    0   0   A   1   MET   CA   A   2   GLN   N   A   2   GLN   H   54.608   .   122.899   .   8.907   .   .   .   .   .      merit=M   0.75
+    1   1   A   1   MET   CB   A   2   GLN   N   A   2   GLN   H   33.279   .   122.899   .   8.907   .   .   .   .   .      merit=M   0.75
+    2   2   A   2   GLN   CA   A   2   GLN   N   A   2   GLN   H   55.215   .   122.899   .   8.907   .   .   .   .   .      merit=M   0.75
+    3   3   A   2   GLN   CB   A   2   GLN   N   A   2   GLN   H   30.606   .   122.899   .   8.907   .   .   .   .   .      merit=M   0.75
+    4   4   A   2   GLN   CA   A   3   ILE   N   A   3   ILE   H   55.057   .   115.127   .   8.318   .   .   .   .   .      merit=M   0.75
+    5   5   A   2   GLN   CB   A   3   ILE   N   A   3   ILE   H   30.582   .   115.127   .   8.318   .   .   .   .   .      merit=M   0.75
+    6   6   A   3   ILE   CA   A   3   ILE   N   A   3   ILE   H   59.616   .   115.127   .   8.318   .   .   .   .   .      merit=M   0.75
+    7   7   A   3   ILE   CB   A   3   ILE   N   A   3   ILE   H   42.025   .   115.127   .   8.318   .   .   .   .   .      merit=M   0.75
 stop_
-"""
+""".replace(
+    NOQUA_E501, ""
+)
 
 
 def test_import_peaks():
 
     sequence_stream = open(path_in_test_data(__file__, "ubi_seq.nef")).read()
 
     filenames = "sparky_all.out sparky_CA-1.out sparky_CA.out".split()
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/rcsb/test_sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/rcsb/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/shifts/test_make_peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
    loop_
       _nef_spectrum_dimension_transfer.dimension_1
       _nef_spectrum_dimension_transfer.dimension_2
       _nef_spectrum_dimension_transfer.dimension_3
       _nef_spectrum_dimension_transfer.transfer_type
       _nef_spectrum_dimension_transfer.is_indirect
 
-     .   2   3   onebond   false
+     1   2   .   onebond   false
      .   2   3   onebond   false
 
    stop_
 
    loop_
       _nef_peak.index
       _nef_peak.peak_id
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
   _nef_peak.position_uncertainty_1
   _nef_peak.position_2
   _nef_peak.position_uncertainty_2
   _nef_peak.height
   _nef_peak.height_uncertainty
   _nef_peak.volume
   _nef_peak.volume_uncertainty
-_nef_peak.ccpn_comment
+  _nef_peak.ccpn_comment
+
      0   0   A   16   DG   H3'   A   16   DG   H8    4.905   .   8.01    .   .   .   7150000.0    .   'this is a comment'
      1   1   A   16   DG   H4'   A   16   DG   H8    4.439   .   8.013   .   .   .   5420000.0    .   .
      2   2   A   17   DT   H6    A   16   DG   H8    7.205   .   8.004   .   .   .   1680000.0    .   'so is this as well'
      3   3   A   17   DT   H7    A   16   DG   H8    1.459   .   8.008   .   .   .   20900000.0   .   .
      4   4   A   17   DT   H2"   A   17   DT   H1'   2.509   .   5.84    .   .   .   46800000.0   .   .
 stop_
 """.replace(
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/predSS_4.tab` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/predSS_4.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/pred_4.tab` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/pred_4.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/protonated_his.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/protonated_his.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/ubi_4.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/ubi_4.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_export_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_import_order_parameters.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_import_order_parameters.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_import_restraints.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_import_restraints.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/talos/test_secondary_structure.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/talos/test_secondary_structure.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,28 +56,29 @@
     assert list(ABC_SEQUENCE_3LET) == translate_1_to_3(ABC_SEQUENCE_1LET)
 
 
 def test_bad_1let_3let():
     BAD_SEQUENCE = "acdefghiklmonpqrstvwy"
 
     msgs = """\
-              unknown residue O
+              unknown residue o
               at residue 12
-              sequence: acdefghiklmonpqrstvwy
+              sequence:
+              acdefghiklmonpqrstvwy
               ^
               """
 
     msgs = dedent(msgs)
     msgs = msgs.split("\n")
 
     with pytest.raises(BadResidue) as exc_info:
         translate_1_to_3(BAD_SEQUENCE)
 
     for msg in msgs:
-        assert msg in exc_info.value.args[0]
+        assert msg in str(exc_info.value)
 
 
 def test_3let_sequence_residue():
 
     sequence_residues = sequence_3let_to_sequence_residues(ABC_SEQUENCE_3LET)
 
     assert sequence_residues == ABC_SEQUENCE_RESIDUES
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/test_util.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_data/basic.peaks` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_data/basic.peaks`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_import_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_import_peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
    loop_
       _nef_spectrum_dimension_transfer.dimension_1
       _nef_spectrum_dimension_transfer.dimension_2
       _nef_spectrum_dimension_transfer.dimension_3
       _nef_spectrum_dimension_transfer.transfer_type
       _nef_spectrum_dimension_transfer.is_indirect
 
-     .   2   3   onebond   false
+     1   2   .   onebond   false
      .   2   3   onebond   false
 
    stop_
 
    loop_
       _nef_peak.index
       _nef_peak.peak_id
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_import_sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_import_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import typer
 
-import nef_pipelines
 from nef_pipelines import nef_app
 
 frames_app = typer.Typer()
 
 
 if nef_app.app:
     nef_app.app.add_typer(
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/filter.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/filter.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/frames/unassign.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/frames/unassign.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.59/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/csv/importers/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/csv/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/echidna/importers/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/echidna/importers/peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Iterator, List
 
 import typer
 from fyeah import f
 from pynmrstar import Saveframe
 
-from nef_pipelines.lib.nef_frames_lib import SPECTRUM_FRAME_CATEGORY
+from nef_pipelines.lib.nef_frames_lib import CCPN_MERIT, SPECTRUM_FRAME_CATEGORY
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
     extract_column,
     read_or_create_entry_exit_error_on_bad_file,
     set_column,
     set_column_to_value,
 )
@@ -27,15 +27,14 @@
 )
 
 DEFAULT_MERIT_FUNTION = "round(x**(1.0/6.0),5)"
 
 # TODO: rationalise these into lib
 CCPN_COMMENT = "ccpn_comment"
 HEIGHT = "height"
-CCPN_MERIT = "ccpn_merit"
 NEF_PEAK = "nef_peak"
 
 app = typer.Typer()
 
 DEFAULT_NUCLEI_HELP = (
     "nuclei to use for each dimension, if not defined they are guessed from the assignments"
     "or an error is reported"
@@ -406,14 +405,15 @@
         frame_code = f"{SPECTRUM_FRAME_CATEGORY}_{f(frame_name_template)}"
 
         frame = entry.get_saveframe_by_name(frame_code)
 
         frame_name = file_name
 
         loop = frame.get_loop(NEF_PEAK)
+
         loop.add_tag(CCPN_MERIT, update_data=True)
 
         comment_values = _remove_and_store_comments(loop)
 
         height_index = loop.tag_index(HEIGHT)
         merit_index = loop.tag_index(CCPN_MERIT)
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Iterable, List
 
 import typer
 from fastaparser import Reader
 from ordered_set import OrderedSet
 
 from nef_pipelines.lib.sequence_lib import (
+    BadResidue,
     MoleculeType,
     MoleculeTypes,
     chain_code_iter,
     offset_chain_residues,
     sequence_3let_to_res,
     sequence_to_nef_frame,
     translate_1_to_3,
@@ -183,15 +184,23 @@
             for sequence, chain_code, molecule_type in zip_longest(
                 sequences, chain_codes, molecule_types, fillvalue=None
             ):
                 if molecule_type is None:
                     molecule_type = MoleculeTypes.PROTEIN
 
                 sequence = [letter_code.letter_code for letter_code in sequence]
-                sequence_3_let = translate_1_to_3(sequence, molecule_type=molecule_type)
+                try:
+                    sequence_3_let = translate_1_to_3(
+                        sequence, molecule_type=molecule_type
+                    )
+                except BadResidue as e:
+                    exit_error(
+                        f"Error translating sequence {sequence} to 3 letter code {e}",
+                        e,
+                    )
                 chain_residues = sequence_3let_to_res(sequence_3_let, chain_code)
 
                 residues.update(chain_residues)
 
     except IOError as e:
         exit_error(f"couldn't open {path} because:\n{e}", e)
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     ),
     output_file: str = typer.Argument(
         None,
         help="file name to output to [default <entry_id>_fix_con.tab] for stdout use -",
         metavar="<MARS_SHIFT_FILE>",
     ),
 ):
-    """- convert nef chemical shifts to mars fragments"""
+    """- convert chemical shifts to mars fragments"""
 
     entry = read_entry_from_file_or_stdin_or_exit_error(input)
 
     output_file = (
         f"{entry.entry_id}_fix_ass.tab" if output_file is None else output_file
     )
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     ),
     output_file: str = typer.Argument(
         None,
         help="file name to output to [default <entry_id>.inp] for stdout use -",
         metavar="<MARS-INPUT-FILENAME>",
     ),
 ):
-    """- convert nef file to mars input"""
+    """- write  mars input fixed assignment and connectivity files"""
 
     entry = read_entry_from_stdin_or_exit()
 
     output_file = f"{entry.entry_id}_mars.inp" if output_file is None else output_file
     pred_file = (
         f"{entry.entry_id}_pred.tab"
         if output_file is None
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     ),
     output_file: Path = typer.Argument(
         None,
         help="file name to output to [default <ENTRY-ID.fasta>] for stdout use -",
         metavar="<FASTA-SEQUENCE-FILE>",
     ),
 ):
-
+    """- write a mars sequence file [fasta]"""
     fasta_sequence(chain_code, in_file, output_file)
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     ),
     output_file: str = typer.Argument(
         None,
         help="file name to output to [default <entry_id>_shifts.tab] for stdout use -",
         metavar="<MARS_SHIFT_FILE>",
     ),
 ):
-    """- convert nef chemical shifts to mars"""
+    """- write a mars chemical shift file"""
 
     if len(shift_frames) == 0:
         shift_frames = ["*"]
 
     entry = read_entry_from_stdin_or_exit()
 
     output_file = f"{entry.entry_id}_shifts.tab" if output_file is None else output_file
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/importers/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/importers/peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     ),
     include_unassigned: bool = typer.Option(False, help="include unassigned peaks"),
     make_spectra: bool = typer.Option(True, help=MAKE_SPECTA_HELP),
     dont_sort_peaks: bool = typer.Option(
         False, help="don't sort the peaks [by isotopes 1H and then 13C]"
     ),
 ):
-    """convert mars [sparky] peaks file <MARS-PEAKS>.txt to NEF"""
+    """- import MARS [sparkyish] peaks files sparky_<NAME>.out"""
 
     entry = read_or_create_entry_exit_error_on_bad_file(input)
 
     sequence = sequence_from_entry_or_exit(entry)
 
     file_names_and_lines = {}
     for file_name in file_names:
@@ -301,15 +301,15 @@
     peaks = modified_peaks
     modified_peaks = []
     MERITS = {"L": 0.50, "M": 0.75, "H": 1.00}
     for peak in peaks:
         if "merit" in peak.comment:
             merit_letter = peak.comment[-1]
 
-            peak = replace(peak, comment="", figure_of_merit=MERITS[merit_letter])
+            peak = replace(peak, figure_of_merit=MERITS[merit_letter])
         modified_peaks.append(peak)
     peaks = modified_peaks
     return peaks
 
 
 def _combine_filenames_into_spectra(file_names):
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         metavar="|PIPE|",
         help="input to read NEF data from [- is stdin]",
     ),
     file_names: List[Path] = typer.Argument(
         ..., help="input files of type mars shifts.tab", metavar="<MARS-shifts>.tab"
     ),
 ):
-    """convert MARS shift file <mars-shifts>.txt to NEF"""
+    """- import shifts from MARS input shift file <mars-shifts>.tab"""
 
     entry = read_or_create_entry_exit_error_on_bad_file(input, entry_name)
 
     chain_codes = parse_comma_separated_options(chain_codes)
 
     pipe(entry, chain_codes, frame_name, file_names, prefix_to_strip, parse_residues)
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/importers/project.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/importers/project.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rcsb/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rcsb/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/sparky/sparky_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/exporters/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/order_parameters.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/order_parameters.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/restraints.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/restraints.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/talos/talos_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/talos/talos_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/importers/peaks.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/importers/shifts.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.59/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.59/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.58
+Version: 0.1.59
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.58/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.59/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
 src/nef_pipelines/tests/echidna/__init__.py
 src/nef_pipelines/tests/echidna/test_import_peaks.py
 src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
 src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
 src/nef_pipelines/tests/fasta/test_sequence.py
 src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
 src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
 src/nef_pipelines/tests/frames/__init__.py
 src/nef_pipelines/tests/frames/test_delete.py
 src/nef_pipelines/tests/frames/test_filter.py
 src/nef_pipelines/tests/frames/test_list.py
 src/nef_pipelines/tests/frames/test_rename.py
 src/nef_pipelines/tests/frames/test_tabulate.py
@@ -295,14 +296,15 @@
 src/nef_pipelines/tools/frames/delete.py
 src/nef_pipelines/tools/frames/filter.py
 src/nef_pipelines/tools/frames/insert.py
 src/nef_pipelines/tools/frames/list.py
 src/nef_pipelines/tools/frames/rename.py
 src/nef_pipelines/tools/frames/tabulate.py
 src/nef_pipelines/tools/frames/unassign.py
+src/nef_pipelines/tools/peaks/__init__.py
 src/nef_pipelines/tools/peaks/match.py
 src/nef_pipelines/tools/shifts/__init__.py
 src/nef_pipelines/tools/shifts/make_peaks.py
 src/nef_pipelines/transcoders/__init__.py
 src/nef_pipelines/transcoders/csv/__init__.py
 src/nef_pipelines/transcoders/csv/importers/__init__.py
 src/nef_pipelines/transcoders/csv/importers/peaks.py
```

### Comparing `nef_pipelines-0.1.58/tox.ini` & `nef_pipelines-0.1.59/tox.ini`

 * *Files identical despite different names*

