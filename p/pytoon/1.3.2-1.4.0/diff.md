# Comparing `tmp/pytoon-1.3.2.tar.gz` & `tmp/pytoon-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoon-1.3.2.tar", last modified: Fri Apr  5 22:10:45 2024, max compression
+gzip compressed data, was "pytoon-1.4.0.tar", last modified: Sun Apr  7 05:04:12 2024, max compression
```

## Comparing `pytoon-1.3.2.tar` & `pytoon-1.4.0.tar`

### file list

```diff
@@ -1,143 +1,17 @@
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.610962 pytoon-1.3.2/
--rw-r--r--   0 luke       (501) staff       (20)     2286 2024-04-05 22:10:45.609748 pytoon-1.3.2/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)     1668 2024-04-05 17:19:51.000000 pytoon-1.3.2/README.md
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.379446 pytoon-1.3.2/pytoon/
--rw-r--r--   0 luke       (501) staff       (20)        0 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/__init__.py
--rw-r--r--   0 luke       (501) staff       (20)     9963 2024-04-05 21:49:05.000000 pytoon-1.3.2/pytoon/animator.py
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.387359 pytoon-1.3.2/pytoon/assets/
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.374819 pytoon-1.3.2/pytoon/assets/junk/
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.389504 pytoon-1.3.2/pytoon/assets/junk/json_files/
--rw-r--r--   0 luke       (501) staff       (20)      541 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/junk/json_files/data_templates.json
--rw-r--r--   0 luke       (501) staff       (20)     3328 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/junk/json_files/og_coordinates_system.json
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.390506 pytoon-1.3.2/pytoon/assets/junk/scripts/
--rw-r--r--   0 luke       (501) staff       (20)     2421 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/junk/scripts/img_database_schema_migration.py
--rw-r--r--   0 luke       (501) staff       (20)      577 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/phonemes.json
--rw-r--r--   0 luke       (501) staff       (20)    14332 2024-03-30 23:15:20.000000 pytoon-1.3.2/pytoon/assets/pose_data.json
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.580553 pytoon-1.3.2/pytoon/assets/poses/
--rw-r--r--   0 luke       (501) staff       (20)    46192 2024-03-30 23:08:14.000000 pytoon-1.3.2/pytoon/assets/poses/1.png
--rw-r--r--   0 luke       (501) staff       (20)    43456 2024-03-30 22:56:31.000000 pytoon-1.3.2/pytoon/assets/poses/10.png
--rw-r--r--   0 luke       (501) staff       (20)    43264 2024-03-30 22:56:18.000000 pytoon-1.3.2/pytoon/assets/poses/11.png
--rw-r--r--   0 luke       (501) staff       (20)    44687 2024-03-30 22:55:36.000000 pytoon-1.3.2/pytoon/assets/poses/12.png
--rw-r--r--   0 luke       (501) staff       (20)    43849 2024-03-30 22:55:51.000000 pytoon-1.3.2/pytoon/assets/poses/13.png
--rw-r--r--   0 luke       (501) staff       (20)    45330 2024-03-30 22:54:11.000000 pytoon-1.3.2/pytoon/assets/poses/14.png
--rw-r--r--   0 luke       (501) staff       (20)    46021 2024-03-30 22:54:55.000000 pytoon-1.3.2/pytoon/assets/poses/15.png
--rw-r--r--   0 luke       (501) staff       (20)    51922 2024-03-30 22:55:23.000000 pytoon-1.3.2/pytoon/assets/poses/16.png
--rw-r--r--   0 luke       (501) staff       (20)    51922 2024-03-30 22:55:10.000000 pytoon-1.3.2/pytoon/assets/poses/17.png
--rw-r--r--   0 luke       (501) staff       (20)    51922 2024-03-30 22:59:40.000000 pytoon-1.3.2/pytoon/assets/poses/18.png
--rw-r--r--   0 luke       (501) staff       (20)    49015 2024-03-30 23:00:48.000000 pytoon-1.3.2/pytoon/assets/poses/19.png
--rw-r--r--   0 luke       (501) staff       (20)    46496 2024-03-30 23:05:50.000000 pytoon-1.3.2/pytoon/assets/poses/2.png
--rw-r--r--   0 luke       (501) staff       (20)    48003 2024-03-30 22:57:26.000000 pytoon-1.3.2/pytoon/assets/poses/20.png
--rw-r--r--   0 luke       (501) staff       (20)    49291 2024-03-30 22:57:12.000000 pytoon-1.3.2/pytoon/assets/poses/21.png
--rw-r--r--   0 luke       (501) staff       (20)    45419 2024-03-30 22:57:54.000000 pytoon-1.3.2/pytoon/assets/poses/22.png
--rw-r--r--   0 luke       (501) staff       (20)    46784 2024-03-30 22:58:36.000000 pytoon-1.3.2/pytoon/assets/poses/23.png
--rw-r--r--   0 luke       (501) staff       (20)    47652 2024-03-30 23:00:09.000000 pytoon-1.3.2/pytoon/assets/poses/24.png
--rw-r--r--   0 luke       (501) staff       (20)    47894 2024-03-30 23:00:23.000000 pytoon-1.3.2/pytoon/assets/poses/25.png
--rw-r--r--   0 luke       (501) staff       (20)    47185 2024-03-30 22:59:27.000000 pytoon-1.3.2/pytoon/assets/poses/26.png
--rw-r--r--   0 luke       (501) staff       (20)    46988 2024-03-30 22:58:49.000000 pytoon-1.3.2/pytoon/assets/poses/27.png
--rw-r--r--   0 luke       (501) staff       (20)    49812 2024-03-30 22:54:25.000000 pytoon-1.3.2/pytoon/assets/poses/28.png
--rw-r--r--   0 luke       (501) staff       (20)    51493 2024-03-30 22:54:40.000000 pytoon-1.3.2/pytoon/assets/poses/29.png
--rw-r--r--   0 luke       (501) staff       (20)    47463 2024-03-30 23:06:18.000000 pytoon-1.3.2/pytoon/assets/poses/3.png
--rw-r--r--   0 luke       (501) staff       (20)    52033 2024-03-30 22:59:55.000000 pytoon-1.3.2/pytoon/assets/poses/30.png
--rw-r--r--   0 luke       (501) staff       (20)    38790 2024-03-30 23:00:35.000000 pytoon-1.3.2/pytoon/assets/poses/31.png
--rw-r--r--   0 luke       (501) staff       (20)    38731 2024-03-30 22:59:13.000000 pytoon-1.3.2/pytoon/assets/poses/32.png
--rw-r--r--   0 luke       (501) staff       (20)    39014 2024-03-30 22:59:01.000000 pytoon-1.3.2/pytoon/assets/poses/33.png
--rw-r--r--   0 luke       (501) staff       (20)    50560 2024-03-30 22:57:40.000000 pytoon-1.3.2/pytoon/assets/poses/34.png
--rw-r--r--   0 luke       (501) staff       (20)    50560 2024-03-30 22:56:59.000000 pytoon-1.3.2/pytoon/assets/poses/35.png
--rw-r--r--   0 luke       (501) staff       (20)    50560 2024-03-30 22:58:08.000000 pytoon-1.3.2/pytoon/assets/poses/36.png
--rw-r--r--   0 luke       (501) staff       (20)    43632 2024-03-30 22:58:22.000000 pytoon-1.3.2/pytoon/assets/poses/37.png
--rw-r--r--   0 luke       (501) staff       (20)    44288 2024-03-30 22:56:45.000000 pytoon-1.3.2/pytoon/assets/poses/38.png
--rw-r--r--   0 luke       (501) staff       (20)    45412 2024-03-30 22:56:04.000000 pytoon-1.3.2/pytoon/assets/poses/39.png
--rw-r--r--   0 luke       (501) staff       (20)    45114 2024-03-30 23:01:15.000000 pytoon-1.3.2/pytoon/assets/poses/4.png
--rw-r--r--   0 luke       (501) staff       (20)    46449 2024-03-30 23:04:40.000000 pytoon-1.3.2/pytoon/assets/poses/40.png
--rw-r--r--   0 luke       (501) staff       (20)    47674 2024-03-30 23:03:05.000000 pytoon-1.3.2/pytoon/assets/poses/41.png
--rw-r--r--   0 luke       (501) staff       (20)    48572 2024-03-30 23:01:42.000000 pytoon-1.3.2/pytoon/assets/poses/42.png
--rw-r--r--   0 luke       (501) staff       (20)    47371 2024-03-30 23:01:57.000000 pytoon-1.3.2/pytoon/assets/poses/43.png
--rw-r--r--   0 luke       (501) staff       (20)    48218 2024-03-30 23:05:36.000000 pytoon-1.3.2/pytoon/assets/poses/44.png
--rw-r--r--   0 luke       (501) staff       (20)    48633 2024-03-30 23:06:46.000000 pytoon-1.3.2/pytoon/assets/poses/45.png
--rw-r--r--   0 luke       (501) staff       (20)    49932 2024-03-30 23:08:45.000000 pytoon-1.3.2/pytoon/assets/poses/46.png
--rw-r--r--   0 luke       (501) staff       (20)    50472 2024-03-30 23:08:30.000000 pytoon-1.3.2/pytoon/assets/poses/47.png
--rw-r--r--   0 luke       (501) staff       (20)    50756 2024-03-30 22:50:29.000000 pytoon-1.3.2/pytoon/assets/poses/48.png
--rw-r--r--   0 luke       (501) staff       (20)    57488 2024-03-30 22:50:42.000000 pytoon-1.3.2/pytoon/assets/poses/49.png
--rw-r--r--   0 luke       (501) staff       (20)    47053 2024-03-30 23:02:10.000000 pytoon-1.3.2/pytoon/assets/poses/5.png
--rw-r--r--   0 luke       (501) staff       (20)    56151 2024-03-30 23:06:04.000000 pytoon-1.3.2/pytoon/assets/poses/50.png
--rw-r--r--   0 luke       (501) staff       (20)    54855 2024-03-30 23:06:31.000000 pytoon-1.3.2/pytoon/assets/poses/51.png
--rw-r--r--   0 luke       (501) staff       (20)    48315 2024-03-30 23:09:00.000000 pytoon-1.3.2/pytoon/assets/poses/52.png
--rw-r--r--   0 luke       (501) staff       (20)    49280 2024-03-30 23:07:58.000000 pytoon-1.3.2/pytoon/assets/poses/53.png
--rw-r--r--   0 luke       (501) staff       (20)    49614 2024-03-30 23:04:13.000000 pytoon-1.3.2/pytoon/assets/poses/54.png
--rw-r--r--   0 luke       (501) staff       (20)    43890 2024-03-30 23:03:19.000000 pytoon-1.3.2/pytoon/assets/poses/55.png
--rw-r--r--   0 luke       (501) staff       (20)    44964 2024-03-30 23:01:29.000000 pytoon-1.3.2/pytoon/assets/poses/56.png
--rw-r--r--   0 luke       (501) staff       (20)    45589 2024-03-30 23:02:24.000000 pytoon-1.3.2/pytoon/assets/poses/57.png
--rw-r--r--   0 luke       (501) staff       (20)    42488 2024-03-30 22:52:35.000000 pytoon-1.3.2/pytoon/assets/poses/58.png
--rw-r--r--   0 luke       (501) staff       (20)    44566 2024-03-30 22:51:22.000000 pytoon-1.3.2/pytoon/assets/poses/59.png
--rw-r--r--   0 luke       (501) staff       (20)    47205 2024-03-30 23:04:26.000000 pytoon-1.3.2/pytoon/assets/poses/6.png
--rw-r--r--   0 luke       (501) staff       (20)    45129 2024-03-30 22:50:04.000000 pytoon-1.3.2/pytoon/assets/poses/60.png
--rw-r--r--   0 luke       (501) staff       (20)    42927 2024-03-30 22:51:08.000000 pytoon-1.3.2/pytoon/assets/poses/61.png
--rw-r--r--   0 luke       (501) staff       (20)    43773 2024-03-30 22:49:21.000000 pytoon-1.3.2/pytoon/assets/poses/62.png
--rw-r--r--   0 luke       (501) staff       (20)    44371 2024-03-30 22:49:07.000000 pytoon-1.3.2/pytoon/assets/poses/63.png
--rw-r--r--   0 luke       (501) staff       (20)    47121 2024-03-30 22:52:19.000000 pytoon-1.3.2/pytoon/assets/poses/64.png
--rw-r--r--   0 luke       (501) staff       (20)    48485 2024-03-30 22:51:35.000000 pytoon-1.3.2/pytoon/assets/poses/65.png
--rw-r--r--   0 luke       (501) staff       (20)    49252 2024-03-30 22:53:17.000000 pytoon-1.3.2/pytoon/assets/poses/66.png
--rw-r--r--   0 luke       (501) staff       (20)    48647 2024-03-30 22:53:30.000000 pytoon-1.3.2/pytoon/assets/poses/67.png
--rw-r--r--   0 luke       (501) staff       (20)    49427 2024-03-30 23:03:59.000000 pytoon-1.3.2/pytoon/assets/poses/68.png
--rw-r--r--   0 luke       (501) staff       (20)    50204 2024-03-30 23:03:46.000000 pytoon-1.3.2/pytoon/assets/poses/69.png
--rw-r--r--   0 luke       (501) staff       (20)    44642 2024-03-30 23:03:33.000000 pytoon-1.3.2/pytoon/assets/poses/7.png
--rw-r--r--   0 luke       (501) staff       (20)    48358 2024-03-30 22:52:04.000000 pytoon-1.3.2/pytoon/assets/poses/70.png
--rw-r--r--   0 luke       (501) staff       (20)    48950 2024-03-30 22:51:49.000000 pytoon-1.3.2/pytoon/assets/poses/71.png
--rw-r--r--   0 luke       (501) staff       (20)    49548 2024-03-30 22:53:04.000000 pytoon-1.3.2/pytoon/assets/poses/72.png
--rw-r--r--   0 luke       (501) staff       (20)    44777 2024-03-30 22:53:43.000000 pytoon-1.3.2/pytoon/assets/poses/73.png
--rw-r--r--   0 luke       (501) staff       (20)    46246 2024-03-30 22:50:16.000000 pytoon-1.3.2/pytoon/assets/poses/74.png
--rw-r--r--   0 luke       (501) staff       (20)    46489 2024-03-30 22:50:55.000000 pytoon-1.3.2/pytoon/assets/poses/75.png
--rw-r--r--   0 luke       (501) staff       (20)    46676 2024-03-30 22:49:35.000000 pytoon-1.3.2/pytoon/assets/poses/76.png
--rw-r--r--   0 luke       (501) staff       (20)    46972 2024-03-30 22:48:53.000000 pytoon-1.3.2/pytoon/assets/poses/77.png
--rw-r--r--   0 luke       (501) staff       (20)    47909 2024-03-30 23:05:21.000000 pytoon-1.3.2/pytoon/assets/poses/78.png
--rw-r--r--   0 luke       (501) staff       (20)    40214 2024-03-30 23:07:00.000000 pytoon-1.3.2/pytoon/assets/poses/79.png
--rw-r--r--   0 luke       (501) staff       (20)    45246 2024-03-30 22:52:50.000000 pytoon-1.3.2/pytoon/assets/poses/8.png
--rw-r--r--   0 luke       (501) staff       (20)    40152 2024-03-30 23:02:37.000000 pytoon-1.3.2/pytoon/assets/poses/80.png
--rw-r--r--   0 luke       (501) staff       (20)    41435 2024-03-30 23:01:02.000000 pytoon-1.3.2/pytoon/assets/poses/81.png
--rw-r--r--   0 luke       (501) staff       (20)    44506 2024-03-30 23:02:52.000000 pytoon-1.3.2/pytoon/assets/poses/82.png
--rw-r--r--   0 luke       (501) staff       (20)    45645 2024-03-30 23:04:54.000000 pytoon-1.3.2/pytoon/assets/poses/83.png
--rw-r--r--   0 luke       (501) staff       (20)    46365 2024-03-30 23:07:41.000000 pytoon-1.3.2/pytoon/assets/poses/84.png
--rw-r--r--   0 luke       (501) staff       (20)    44614 2024-03-30 23:09:15.000000 pytoon-1.3.2/pytoon/assets/poses/85.png
--rw-r--r--   0 luke       (501) staff       (20)    45314 2024-03-30 23:07:13.000000 pytoon-1.3.2/pytoon/assets/poses/86.png
--rw-r--r--   0 luke       (501) staff       (20)    45799 2024-03-30 23:05:08.000000 pytoon-1.3.2/pytoon/assets/poses/87.png
--rw-r--r--   0 luke       (501) staff       (20)    45290 2024-03-30 22:48:40.000000 pytoon-1.3.2/pytoon/assets/poses/88.png
--rw-r--r--   0 luke       (501) staff       (20)    46154 2024-03-30 22:49:49.000000 pytoon-1.3.2/pytoon/assets/poses/89.png
--rw-r--r--   0 luke       (501) staff       (20)    46357 2024-03-30 22:53:56.000000 pytoon-1.3.2/pytoon/assets/poses/9.png
--rw-r--r--   0 luke       (501) staff       (20)    46370 2024-03-30 23:07:27.000000 pytoon-1.3.2/pytoon/assets/poses/90.png
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.375693 pytoon-1.3.2/pytoon/assets/visemes/
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.592425 pytoon-1.3.2/pytoon/assets/visemes/negative/
--rw-r--r--   0 luke       (501) staff       (20)     2829 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/1.png
--rw-r--r--   0 luke       (501) staff       (20)     1341 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/10.png
--rw-r--r--   0 luke       (501) staff       (20)     1146 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/11.png
--rw-r--r--   0 luke       (501) staff       (20)     2511 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/2.png
--rw-r--r--   0 luke       (501) staff       (20)     2949 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/3.png
--rw-r--r--   0 luke       (501) staff       (20)     2562 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/4.png
--rw-r--r--   0 luke       (501) staff       (20)     3136 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/5.png
--rw-r--r--   0 luke       (501) staff       (20)     2962 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/6.png
--rw-r--r--   0 luke       (501) staff       (20)     2966 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/7.png
--rw-r--r--   0 luke       (501) staff       (20)     2216 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/8.png
--rw-r--r--   0 luke       (501) staff       (20)     1786 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/negative/9.png
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.607320 pytoon-1.3.2/pytoon/assets/visemes/positive/
--rw-r--r--   0 luke       (501) staff       (20)     3542 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/1.png
--rw-r--r--   0 luke       (501) staff       (20)     1341 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/10.png
--rw-r--r--   0 luke       (501) staff       (20)     1146 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/11.png
--rw-r--r--   0 luke       (501) staff       (20)     3049 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/2.png
--rw-r--r--   0 luke       (501) staff       (20)     3549 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/3.png
--rw-r--r--   0 luke       (501) staff       (20)     3194 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/4.png
--rw-r--r--   0 luke       (501) staff       (20)     3635 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/5.png
--rw-r--r--   0 luke       (501) staff       (20)     3488 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/6.png
--rw-r--r--   0 luke       (501) staff       (20)     3516 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/7.png
--rw-r--r--   0 luke       (501) staff       (20)     2928 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/8.png
--rw-r--r--   0 luke       (501) staff       (20)     1901 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes/positive/9.png
--rw-r--r--   0 luke       (501) staff       (20)      523 2024-03-25 18:18:13.000000 pytoon-1.3.2/pytoon/assets/visemes.json
--rw-r--r--   0 luke       (501) staff       (20)     2314 2024-03-30 20:38:55.000000 pytoon-1.3.2/pytoon/dataloader.py
--rw-r--r--   0 luke       (501) staff       (20)     7639 2024-04-05 22:09:51.000000 pytoon-1.3.2/pytoon/lipsync.py
--rw-r--r--   0 luke       (501) staff       (20)     3457 2024-04-05 17:03:17.000000 pytoon-1.3.2/pytoon/util.py
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-05 22:10:45.608677 pytoon-1.3.2/pytoon.egg-info/
--rw-r--r--   0 luke       (501) staff       (20)     2286 2024-04-05 22:10:45.000000 pytoon-1.3.2/pytoon.egg-info/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)     3749 2024-04-05 22:10:45.000000 pytoon-1.3.2/pytoon.egg-info/SOURCES.txt
--rw-r--r--   0 luke       (501) staff       (20)        1 2024-04-05 22:10:45.000000 pytoon-1.3.2/pytoon.egg-info/dependency_links.txt
--rw-r--r--   0 luke       (501) staff       (20)       59 2024-04-05 22:10:45.000000 pytoon-1.3.2/pytoon.egg-info/requires.txt
--rw-r--r--   0 luke       (501) staff       (20)        7 2024-04-05 22:10:45.000000 pytoon-1.3.2/pytoon.egg-info/top_level.txt
--rw-r--r--   0 luke       (501) staff       (20)       38 2024-04-05 22:10:45.611225 pytoon-1.3.2/setup.cfg
--rw-r--r--   0 luke       (501) staff       (20)     1137 2024-04-05 22:10:07.000000 pytoon-1.3.2/setup.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-07 05:04:12.169539 pytoon-1.4.0/
+-rw-r--r--   0 luke       (501) staff       (20)     2173 2024-04-07 05:04:12.169028 pytoon-1.4.0/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)     1668 2024-04-05 17:19:51.000000 pytoon-1.4.0/README.md
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-07 05:04:12.165487 pytoon-1.4.0/pytoon/
+-rw-r--r--   0 luke       (501) staff       (20)        0 2024-03-25 18:18:13.000000 pytoon-1.4.0/pytoon/__init__.py
+-rw-r--r--   0 luke       (501) staff       (20)     8780 2024-04-07 04:56:06.000000 pytoon-1.4.0/pytoon/animator.py
+-rw-r--r--   0 luke       (501) staff       (20)     2314 2024-03-30 20:38:55.000000 pytoon-1.4.0/pytoon/dataloader.py
+-rw-r--r--   0 luke       (501) staff       (20)     7742 2024-04-06 23:48:56.000000 pytoon-1.4.0/pytoon/lipsync.py
+-rw-r--r--   0 luke       (501) staff       (20)     3457 2024-04-05 17:03:17.000000 pytoon-1.4.0/pytoon/util.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-07 05:04:12.168293 pytoon-1.4.0/pytoon.egg-info/
+-rw-r--r--   0 luke       (501) staff       (20)     2173 2024-04-07 05:04:12.000000 pytoon-1.4.0/pytoon.egg-info/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)      259 2024-04-07 05:04:12.000000 pytoon-1.4.0/pytoon.egg-info/SOURCES.txt
+-rw-r--r--   0 luke       (501) staff       (20)        1 2024-04-07 05:04:12.000000 pytoon-1.4.0/pytoon.egg-info/dependency_links.txt
+-rw-r--r--   0 luke       (501) staff       (20)       59 2024-04-07 05:04:12.000000 pytoon-1.4.0/pytoon.egg-info/requires.txt
+-rw-r--r--   0 luke       (501) staff       (20)        7 2024-04-07 05:04:12.000000 pytoon-1.4.0/pytoon.egg-info/top_level.txt
+-rw-r--r--   0 luke       (501) staff       (20)       38 2024-04-07 05:04:12.169746 pytoon-1.4.0/setup.cfg
+-rw-r--r--   0 luke       (501) staff       (20)     1137 2024-04-07 05:02:33.000000 pytoon-1.4.0/setup.py
```

### Comparing `pytoon-1.3.2/PKG-INFO` & `pytoon-1.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: pytoon
-Version: 1.3.2
-Summary: A Python library for lip-syncing cartoons to voice recordings.
-Home-page: https://github.com/lukerbs/apple
-Author: Luke Kerbs
-Keywords: animation,forced alignment,lip-sync,audio forced alignment,phoneme,generate subtitles
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: forcealign==1.1.1
-Requires-Dist: moviepy
-Requires-Dist: opencv-python
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: pillow
-
 # PyToon
 ## Overview 
 PyToon is a Python based animation library for animating characters and their mouth movements. This tools uses machine learning based audio analysis techiques to automatically lip-sync animated character mouth mouth movements to a given audio recording of someone talking.
 
 [Example Output Video](https://youtu.be/fX2loRnr7II)
 
 ## Features
@@ -55,8 +37,8 @@
 
 # Overlay the animation on top of another video and save as an .mp4 file.
 background_video = VideoFileClip("./path/to/background_video.mp4")
 animation.export(path='video.mp4', background=background_video, scale=0.7)
 ```
 
 ## Acknowledgements
-This project uses character images created by [lazykh](https://github.com/carykh/lazykh).
+This project uses character images created by [lazykh](https://github.com/carykh/lazykh).
```

### Comparing `pytoon-1.3.2/README.md` & `pytoon-1.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: pytoon
+Version: 1.4.0
+Summary: A Python library for lip-syncing cartoons to voice recordings.
+Home-page: https://github.com/lukerbs/apple
+Author: Luke Kerbs
+License: UNKNOWN
+Keywords: animation,forced alignment,lip-sync,audio forced alignment,phoneme,generate subtitles
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # PyToon
 ## Overview 
 PyToon is a Python based animation library for animating characters and their mouth movements. This tools uses machine learning based audio analysis techiques to automatically lip-sync animated character mouth mouth movements to a given audio recording of someone talking.
 
 [Example Output Video](https://youtu.be/fX2loRnr7II)
 
 ## Features
@@ -37,8 +51,9 @@
 
 # Overlay the animation on top of another video and save as an .mp4 file.
 background_video = VideoFileClip("./path/to/background_video.mp4")
 animation.export(path='video.mp4', background=background_video, scale=0.7)
 ```
 
 ## Acknowledgements
-This project uses character images created by [lazykh](https://github.com/carykh/lazykh).
+This project uses character images created by [lazykh](https://github.com/carykh/lazykh).
+
```

### Comparing `pytoon-1.3.2/pytoon/dataloader.py` & `pytoon-1.4.0/pytoon/dataloader.py`

 * *Files identical despite different names*

### Comparing `pytoon-1.3.2/pytoon/lipsync.py` & `pytoon-1.4.0/pytoon/lipsync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from forcealign import ForceAlign
 from .util import read_json
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Union
 import random
+import re
 
 # Viseme image for silence (i.e. closed mouth, not speaking)
 SILENT_VISEME = "9.png"
 SILENT_PHONEME = "PAUSE"
 # ARPAbet phonemes to simplified phonemes mapping
 PHONEMES = read_json("phonemes.json")
 # Simplified phonemes to viseme-sequence mapping
@@ -19,14 +20,15 @@
     word: Union[str, None]  # Word associated with viseme
     visemes: list[str]  # List of mouth shape images for viseme
     phonemes: list[str]  # The phoneme associated with the viseme
     time_start: datetime  # The time the word starts (seconds)
     time_end: datetime  # The time the word ends (seconds)
     duration: float  # total word duration from start to end (seconds)
     total_frames: int  # total number of frames in video for word
+    breath: bool
 
 
 def viseme_sequencer(audio_file: str, transcript: str, fps:int=48) -> list[WordViseme]:
     """Converts and audio / txt file to force aligned viseme sequence
 
     Args:
         audio_file (str): Path to audio file of a person speaking english (.wav or .mp3)
@@ -70,14 +72,15 @@
                 word=word.word,
                 visemes=visemes,
                 phonemes=phonemes,
                 time_start=word.time_start,
                 time_end=word.time_end,
                 duration=duration,
                 total_frames=total_frames,
+                breath=word.breath
             )
         )
 
     # Add silence viseme (closed mouth) between speaking visemes
     finished_sequence = []
     for i, _ in enumerate(viseme_sequence):
         finished_sequence.append(viseme_sequence[i])
@@ -198,14 +201,15 @@
         word=None,
         visemes=silent_visemes,
         phonemes=phonemes,
         time_start=silence_start,
         time_end=silence_end,
         duration=duration,
         total_frames=total_frames,
+        breath=False
     )
 
 def ending_silence(duration:float, fps:int, start_t:int):
     total_frames = int(duration * fps)
 
     # Create frames for silence
     silent_visemes = [SILENT_VISEME for _ in range(total_frames)]
@@ -214,8 +218,9 @@
         word=None,
         visemes=silent_visemes,
         phonemes=phonemes,
         time_start=start_t,
         time_end=start_t+duration,
         duration=duration,
         total_frames=total_frames,
-    )
+        breath=False
+    )
```

### Comparing `pytoon-1.3.2/pytoon/util.py` & `pytoon-1.4.0/pytoon/util.py`

 * *Files identical despite different names*

### Comparing `pytoon-1.3.2/pytoon.egg-info/PKG-INFO` & `pytoon-1.4.0/pytoon.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: pytoon
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Python library for lip-syncing cartoons to voice recordings.
 Home-page: https://github.com/lukerbs/apple
 Author: Luke Kerbs
+License: UNKNOWN
 Keywords: animation,forced alignment,lip-sync,audio forced alignment,phoneme,generate subtitles
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: forcealign==1.1.1
-Requires-Dist: moviepy
-Requires-Dist: opencv-python
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: pillow
 
 # PyToon
 ## Overview 
 PyToon is a Python based animation library for animating characters and their mouth movements. This tools uses machine learning based audio analysis techiques to automatically lip-sync animated character mouth mouth movements to a given audio recording of someone talking.
 
 [Example Output Video](https://youtu.be/fX2loRnr7II)
 
@@ -56,7 +52,8 @@
 # Overlay the animation on top of another video and save as an .mp4 file.
 background_video = VideoFileClip("./path/to/background_video.mp4")
 animation.export(path='video.mp4', background=background_video, scale=0.7)
 ```
 
 ## Acknowledgements
 This project uses character images created by [lazykh](https://github.com/carykh/lazykh).
+
```

### Comparing `pytoon-1.3.2/setup.py` & `pytoon-1.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pytoon",
-    version="1.3.2",
+    version="1.4.0",
     packages=find_packages(),
     install_requires=[
-        "forcealign==1.1.1",
+        "forcealign==1.1.5",
         "moviepy",
         "opencv-python",
         "scipy",
         "numpy",
         "pillow",
     ],
     author="Luke Kerbs",
```

