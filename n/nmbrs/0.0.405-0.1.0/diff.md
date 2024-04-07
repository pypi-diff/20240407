# Comparing `tmp/nmbrs-0.0.405.tar.gz` & `tmp/nmbrs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmbrs-0.0.405.tar", last modified: Fri Mar 22 15:40:43 2024, max compression
+gzip compressed data, was "nmbrs-0.1.0.tar", last modified: Sun Apr  7 11:28:52 2024, max compression
```

## Comparing `nmbrs-0.0.405.tar` & `nmbrs-0.1.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.501194 nmbrs-0.0.405/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-03-22 15:40:30.000000 nmbrs-0.0.405/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 15:40:30.000000 nmbrs-0.0.405/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-03-22 15:40:43.501194 nmbrs-0.0.405/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-22 15:40:30.000000 nmbrs-0.0.405/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-22 15:40:30.000000 nmbrs-0.0.405/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:40:43.501194 nmbrs-0.0.405/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-22 15:40:30.000000 nmbrs-0.0.405/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.485194 nmbrs-0.0.405/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.489194 nmbrs-0.0.405/src/nmbrs/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-22 15:40:41.000000 nmbrs-0.0.405/src/nmbrs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.489194 nmbrs-0.0.405/src/nmbrs/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/data_classes/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/data_classes/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/data_classes/debtor.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/data_classes/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/data_classes/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.489194 nmbrs-0.0.405/src/nmbrs/data_classes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/data_classes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/data_classes/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.489194 nmbrs-0.0.405/src/nmbrs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/exceptions/nmbrs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/exceptions/sso_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.493194 nmbrs-0.0.405/src/nmbrs/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/company_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/debtor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/employee_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.493194 nmbrs-0.0.405/src/nmbrs/service/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.493194 nmbrs-0.0.405/src/nmbrs/service/microservices/company/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/cost_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/hour_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/labout_aggreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/pension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/salary_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/salary_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/wage_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/wage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/company/wage_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.497194 nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/title.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/webook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.501194 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/absence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/child.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/days.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/employment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/hour_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/labour_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/lease_car.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/levensloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/personal_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/salary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/spaarloon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/time_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/employee/wage_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/microservices/micro_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/service/sso_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.501194 nmbrs-0.0.405/src/nmbrs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/utils/find_empty_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/utils/nmbrs_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-22 15:40:30.000000 nmbrs-0.0.405/src/nmbrs/utils/return_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:40:43.501194 nmbrs-0.0.405/src/nmbrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-03-22 15:40:43.000000 nmbrs-0.0.405/src/nmbrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-22 15:40:43.000000 nmbrs-0.0.405/src/nmbrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:40:43.000000 nmbrs-0.0.405/src/nmbrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-22 15:40:43.000000 nmbrs-0.0.405/src/nmbrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 15:40:43.000000 nmbrs-0.0.405/src/nmbrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.683338 nmbrs-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-07 11:28:40.000000 nmbrs-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 11:28:40.000000 nmbrs-0.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-07 11:28:52.683338 nmbrs-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-07 11:28:40.000000 nmbrs-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-07 11:28:40.000000 nmbrs-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:28:52.683338 nmbrs-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-07 11:28:40.000000 nmbrs-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.671338 nmbrs-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.671338 nmbrs-0.1.0/src/nmbrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 11:28:50.000000 nmbrs-0.1.0/src/nmbrs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.671338 nmbrs-0.1.0/src/nmbrs/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/data_classes/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/data_classes/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/data_classes/debtor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/data_classes/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/data_classes/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.675338 nmbrs-0.1.0/src/nmbrs/data_classes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/data_classes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/data_classes/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.675338 nmbrs-0.1.0/src/nmbrs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/exceptions/nmbrs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/exceptions/sso_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.675338 nmbrs-0.1.0/src/nmbrs/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/company_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/debtor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/employee_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.675338 nmbrs-0.1.0/src/nmbrs/service/microservices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.679338 nmbrs-0.1.0/src/nmbrs/service/microservices/company/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/cost_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/hour_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/labout_aggreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/pension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/salary_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/salary_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/wage_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/wage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/company/wage_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.679338 nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/webook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.683338 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/absence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/employment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/hour_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/labour_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/lease_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/levensloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/personal_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/salary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/spaarloon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/time_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/employee/wage_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/microservices/micro_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/service/sso_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.683338 nmbrs-0.1.0/src/nmbrs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/utils/find_empty_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/utils/nmbrs_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-07 11:28:40.000000 nmbrs-0.1.0/src/nmbrs/utils/return_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:28:52.683338 nmbrs-0.1.0/src/nmbrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-07 11:28:52.000000 nmbrs-0.1.0/src/nmbrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-07 11:28:52.000000 nmbrs-0.1.0/src/nmbrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:28:52.000000 nmbrs-0.1.0/src/nmbrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 11:28:52.000000 nmbrs-0.1.0/src/nmbrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 11:28:52.000000 nmbrs-0.1.0/src/nmbrs.egg-info/top_level.txt
```

### Comparing `nmbrs-0.0.405/LICENSE` & `nmbrs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/PKG-INFO` & `nmbrs-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.0.405
+Version: 0.1.0
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/Visma-NMBRS-SOAP-API-SDK
```

### Comparing `nmbrs-0.0.405/README.md` & `nmbrs-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/setup.py` & `nmbrs-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/api.py` & `nmbrs-0.1.0/src/nmbrs/api.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/data_classes/company.py` & `nmbrs-0.1.0/src/nmbrs/data_classes/company.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,18 +18,50 @@
         self.fax_number: str = data.get("FaxNumber", None)
         self.email: str = data.get("Email", None)
         self.website: str = data.get("Website", None)
         self.loonaangifte_tijdvak: str = data.get("LoonaangifteTijdvak", None)
         self.kvk_number: str = data.get("KvkNr", None)
 
 
+class BankAccount(DataClass):
+    """A class representing a bank account."""
+
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
+        self.id: int = data.get("Id", None)
+        self.number: str = data.get("Number", None)
+        self.description: str = data.get("Description", None)
+        self.iban: str = data.get("IBAN", None)
+        self.bic: str = data.get("BIC", None)
+        self.city: str = data.get("City", None)
+        self.name: str = data.get("Name", None)
+        self.type: str = data.get("Type", None)
+
+
+class Address(DataClass):
+    """A class representing an address."""
+
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
+        self.id: int = data.get("Id", None)
+        self.default: bool = data.get("Default", None)
+        self.street: str = data.get("Street", None)
+        self.house_number: str = data.get("HouseNumber", None)
+        self.house_number_addition: str = data.get("HouseNumberAddition", None)
+        self.postal_code: str = data.get("PostalCode", None)
+        self.city: str = data.get("City", None)
+        self.state_province: str = data.get("StateProvince", None)
+        self.country_iso_code: str = data.get("CountryISOCode", None)
+
+
 class LabourAgreement(DataClass):
     """A class representing a labour agreement."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.id: int = data.get("Id")
         self.guid: str = data.get("Guid")
         self.number: int = data.get("Number")
         self.description: str = data.get("Description")
         self.default: bool = data.get("Default")
         self.schedule_model: CodeDescription = CodeDescription(data.get("ScheduleModel"))
         self.wage_model: CodeDescription = CodeDescription(data.get("WageModel"))
@@ -46,25 +78,27 @@
         self.cao: CodeDescription = CodeDescription(data.get("CAO"))
         self.bln_use_provisional: bool = data.get("BlnUseProvisional")
 
 
 class Period(DataClass):
     """A class representing a period of a company."""
 
-    def __init__(self, data: str) -> None:
+    def __init__(self, company_id: int, data: str) -> None:
         parts = data.split("-")
+        self.company_id = company_id
         self.year: int = int(parts[0])
         self.period: int = int(parts[1])
         self.type: str = parts[2]
 
 
 class WageTax(DataClass):
     """A class representing a wage tax."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.loonaangifte_id: int = data.get("LoonaangifteID", None)
         self.serial_number: int = data.get("SerialNumber", None)
         self.payment_reference: str = data.get("PaymentReference", None)
         self.total_general: int = data.get("TotalGeneral", None)
         self.period: int = data.get("Period", None)
         self.year: int = data.get("Year", None)
         self.status: str = data.get("Status", None)
@@ -85,30 +119,32 @@
         """Convert the instance to a dictionary."""
         return parse_xml_to_dict(self.xml)
 
 
 class ContactPerson(DataClass):
     """A class representing a contact person with their details."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.email: str = data.get("Email")
         self.name: str = data.get("Name")
         self.phone: str = data.get("Phone")
         self.gender: str = data.get("Gender")
         self.mobile_phone: str = data.get("MobilePhone")
         self.fax: str = data.get("Fax")
         self.function: str = data.get("Function")
         self.department: str = data.get("Department")
         self.number: int = data.get("Number")
 
 
 class GuidConvertor(DataClass):
     """A class representing the mappings between integer IDs and GUIDs for a specific entity."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.entity: str = data.get("Entity")
         mappings_data = data.get("Mappings", [])
         mappings_data = mappings_data.get("Mapping", [])
         if not isinstance(mappings_data, list):
             mappings_data = [mappings_data]
         self.mappings: list[Mapping] = [Mapping(mapping_data) for mapping_data in mappings_data]
 
@@ -120,41 +156,45 @@
         self.id: int = data.get("IdInt")
         self.guid: str = data.get("IdGuid")
 
 
 class CostCenter(DataClass):
     """A class representing a cost center."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.id: int = data.get("Id")
         self.code: int = data.get("Code")
         self.description: str = data.get("Description")
 
 
 class CostUnit(DataClass):
     """A class representing a cost unit."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.id: int = data.get("Id")
         self.code: int = data.get("Code")
         self.description: str = data.get("Description")
 
 
 class HourCode(DataClass):
     """A class representing an hour code."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.code: int = data.get("Code")
         self.description: str = data.get("Description")
 
 
 class Pension(DataClass):
     """A class representing a pension exports information."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.pension_export_id: int = data.get("PensionExportID")
         self.serial_number: int = data.get("SerialNumber")
         self.period: int = data.get("Period")
         self.year: int = data.get("Year")
         self.status: str = data.get("Status")
         self.send_at: datetime = data.get("SentAt")
         self.correctie_tijdvak_start: datetime = data.get("CorrectionTijdvakStart")
@@ -171,58 +211,63 @@
         """Convert the instance to a dictionary."""
         return parse_xml_to_dict(self.xml)
 
 
 class RunRequest(DataClass):
     """A class representing a run request."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id: company_id
         self.period: int = data.get("Period")
         self.year: int = data.get("Year")
         self.status: str = data.get("Status")
         self.handle_delete: datetime = data.get("HandledDate")
 
 
 class RunInfo(DataClass):
     """A class representing a run info."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.id: int = data.get("ID")
         self.number: int = data.get("Number")
         self.year: int = data.get("Year")
         self.period_start: int = data.get("PeriodStart")
         self.period_end: int = data.get("PeriodEnd")
         self.description: int = data.get("Description")
         self.run_at: datetime = data.get("RunAt")
         self.locked: datetime = data.get("IsLocked")
 
 
 class SalaryTable(DataClass):
     """A class representing a salary table."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.code: int = data.get("Code")
         self.description: str = data.get("Description")
 
 
 class SalaryTableScale(DataClass):
     """A class representing a salary table scale."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.scale: str = data.get("Scale")
         self.description: str = data.get("Description")
         self.value: Decimal = data.get("ScaleValue")
         self.percentage_max: Decimal = data.get("ScalePercentageMax")
         self.percentage_min: Decimal = data.get("ScalePercentageMin")
 
 
 class SalaryTableStep(DataClass):
     """A class representing a salary table scale."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.step: str = data.get("Step")
         self.description: str = data.get("StepDescription")
         self.value: Decimal = data.get("StepValue")
 
 
 class SVWSettings(DataClass):
     """A class representing a svw settings."""
@@ -237,15 +282,16 @@
         self.wga_wg: Decimal = data.get("Gediff_WGA_wg")
         self.sector: int = data.get("Sector")
 
 
 class SVW(DataClass):
     """A class representing a svw."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.settings: SVWSettings = SVWSettings(data.get("SVWSettings"))
         self.sector: CodeDescription = CodeDescription(data.get("Sector"))
         self.risc_group: CodeDescription = CodeDescription(data.get("Risicogroep"))
         self.cao: CodeDescription = CodeDescription(data.get("CAO"))
 
     def insert_dict(self) -> dict:
         """Method used in combination with the Insert methode in the company.svw service"""
@@ -271,23 +317,25 @@
             },
         }
 
 
 class DefaultEmployeeTemplate(DataClass):
     """A class representing a default employee template scale."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.id: str = data.get("DefaultEmployeeTemplateId")
         self.description: str = data.get("Description")
 
 
 class FulltimeSchedules(DataClass):
     """A class representing all fulltime schedules."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.schedule_one: FulltimeSchedule = FulltimeSchedule(data.get("FulltimeScheduleOne"))
         self.schedule_two: FulltimeSchedule = FulltimeSchedule(data.get("FulltimeScheduleTwo"))
         self.schedule_three: FulltimeSchedule = FulltimeSchedule(data.get("FulltimeScheduleThree"))
         self.schedule_four: FulltimeSchedule = FulltimeSchedule(data.get("FulltimeScheduleFour"))
 
 
 class FulltimeSchedule(DataClass):
@@ -321,31 +369,70 @@
         self.action_status: str = data.get("ActionStatus")
         self.run_at: datetime = data.get("RunAt")
 
 
 class PayrollWorkflowTrack(DataClass):
     """A class representing a payroll workflow track."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.track_name: str = data.get("TrackName")
         self.track_status: str = data.get("TrackStatus")
         self.actions: list[PayrollWorkflowAction] = [PayrollWorkflowAction(action) for action in data.get("Actions", [])]
 
 
 class LeaveTypeGroup(DataClass):
     """A class representing a leave type group."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
         self.type: str = data.get("Type")
         self.description: str = data.get("Description")
         self.company_leave_balance: list[CompanyLeaveType] = [
             CompanyLeaveType(leave_type) for leave_type in data.get("CompanyLeaveBalance", [])
         ]
 
 
 class CompanyLeaveType(DataClass):
     """A class representing a company leave type."""
 
     def __init__(self, data: dict) -> None:
         self.description_leave_balance: str = data.get("DescriptionLeaveBalance")
         self.full_time_balance: Decimal = data.get("FullTimeBalance")
         self.leave_rounding_method: str = data.get("LeaveRoundingMethod")
+
+
+class WageComponent(DataClass):
+    """A class representing a wage component."""
+
+    def __init__(self, company_id: int, component_type: str, data: dict) -> None:
+        self.company_id = company_id
+        self.type = component_type
+        self.id: int = data.get("Id")
+        self.code: int = data.get("Code")
+        self.value: str = data.get("Value")
+
+
+class WageCost(DataClass):
+    """A class representing a wage cost."""
+
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
+        self.period: int = data.get("Period")
+        self.year: int = data.get("Year")
+        self.payroll: Decimal = data.get("WorkCostPayroll")
+        self.financial: Decimal = data.get("WorkCostFinancial")
+        self.fiscal_wage: Decimal = data.get("FiscalWage")
+        self.available_space: Decimal = data.get("WorkCostAvailableSpace")
+        self.base: Decimal = data.get("WorkCostBase")
+        self.to_pay: Decimal = data.get("WorkCostToPay")
+        self.estimated: Decimal = data.get("WorkCostEstimated")
+        self.paid: Decimal = data.get("WorkCostPaid")
+
+
+class WageModel(DataClass):
+    """A class representing a wage model."""
+
+    def __init__(self, company_id: int, data: dict) -> None:
+        self.company_id = company_id
+        self.code: int = data.get("Code")
+        self.description: str = data.get("Description")
```

### Comparing `nmbrs-0.0.405/src/nmbrs/data_classes/debtor.py` & `nmbrs-0.1.0/src/nmbrs/data_classes/debtor.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,44 +28,47 @@
             "xml": parse_xml_to_dict(self.xml),
         }
 
 
 class Address(DataClass):
     """A class representing an address."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.id: int = data.get("Id", None)
         self.default: bool = data.get("Default", None)
         self.street: str = data.get("Street", None)
         self.house_number: str = data.get("HouseNumber", None)
         self.house_number_addition: str = data.get("HouseNumberAddition", None)
         self.postal_code: str = data.get("PostalCode", None)
         self.city: str = data.get("City", None)
         self.state_province: str = data.get("StateProvince", None)
         self.country_iso_code: str = data.get("CountryISOCode", None)
 
 
 class BankAccount(DataClass):
     """A class representing a bank account."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.id: int = data.get("Id", None)
         self.number: str = data.get("Number", None)
         self.description: str = data.get("Description", None)
         self.iban: str = data.get("IBAN", None)
         self.bic: str = data.get("BIC", None)
         self.city: str = data.get("City", None)
         self.name: str = data.get("Name", None)
         self.type: str = data.get("Type", None)
 
 
 class ContactInfo(DataClass):
     """A class representing a contact info."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.email: str = data.get("Email", None)
         self.name: str = data.get("Name", None)
         self.phone: str = data.get("Phone", None)
 
 
 class Debtor(DataClass):
     """A class representing a debtor."""
@@ -75,69 +78,75 @@
         self.number: str = data.get("Number", None)
         self.name: str = data.get("Name", None)
 
 
 class Department(DataClass):
     """A class representing a department."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.id: int = data.get("Id", None)
         self.code: int = data.get("Code", None)
         self.description: str = data.get("Description", None)
 
 
 class Function(DataClass):
     """A class representing a function."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.id: int = data.get("Id", None)
         self.code: int = data.get("Code", None)
         self.description: str = data.get("Description", None)
 
 
 class LabourAgreementSettings(DataClass):
     """A class representing labour agreement settings."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.id: int = data.get("Id", None)
         self.guid: str = data.get("Guid", None)
         self.int_number: int = data.get("IntNumber", None)
         self.str_name: str = data.get("StrName", None)
         self.debtor_id: int = data.get("IntDebiteurID", None)
 
 
 class Manager(DataClass):
     """A class representing manager information."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.number: int = data.get("Number", None)
         self.first_name: str = data.get("FirstName", None)
         self.name: str = data.get("Name", None)
         self.department: str = data.get("Department", None)
         self.function: str = data.get("Function", None)
         self.phone_number: str = data.get("PhoneNumber", None)
         self.mobile: str = data.get("Mobile", None)
         self.fax: str = data.get("Fax", None)
         self.email: str = data.get("Email", None)
 
 
 class ServiceLevel(DataClass):
     """A class representing service level information."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.start_period: int = data.get("StartPeriod", None)
         self.start_year: int = data.get("StartYear", None)
         self.service_level: str = data.get("ServiceLevel", None)
         self.start_contract: datetime = data.get("StartContract", None)
 
 
 class Tag(DataClass):
     """A class representing debtor tag information."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.number: int = data.get("Number", None)
         self.hex_color: str = data.get("HexColor", None)
         self.tag: str = data.get("Tag", None)
 
 
 class Event(DataClass):
     """A class representing an event."""
@@ -158,15 +167,16 @@
             "Active": self.active,
         }
 
 
 class WebhookSetting(DataClass):
     """A class representing a webhook setting."""
 
-    def __init__(self, data: dict) -> None:
+    def __init__(self, debtor_id: int, data: dict) -> None:
+        self.debtor_id = debtor_id
         self.webhook_setting_id: int = data.get("WebhookSettingId", None)
         self.name: str = data.get("Name", None)
         self.endpoint: str = data.get("Endpoint", None)
         self.active: bool = data.get("Active", None)
         events_data = data.get("Event", [])
         if not isinstance(events_data, list):
             events_data = [events_data]
```

### Comparing `nmbrs-0.0.405/src/nmbrs/data_classes/utils/xml.py` & `nmbrs-0.1.0/src/nmbrs/data_classes/utils/xml.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/exceptions/exceptions.py` & `nmbrs-0.1.0/src/nmbrs/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/exceptions/nmbrs_exceptions.py` & `nmbrs-0.1.0/src/nmbrs/exceptions/nmbrs_exceptions.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/exceptions/sso_exceptions.py` & `nmbrs-0.1.0/src/nmbrs/exceptions/sso_exceptions.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/company_service.py` & `nmbrs-0.1.0/src/nmbrs/service/company_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 
         # Micro services
         self.address = CompanyAddressService(self.client)
         self.bank_account = CompanyBankAccountService(self.client)
         self.cost_center = CompanyCostCenterService(self.client)
         self.cost_unit = CompanyCostUnitService(self.client)
         self.hour_model = CompanyHourModelService(self.client)
-        self.journal = CompanyJournalService(self.client)
+        self.journal = CompanyJournalService(self.client)  # TO BE implemented
         self.labour_agreement = CompanyLabourAgreementService(self.client)
         self.pension = CompanyPensionService(self.client)
         self.run = CompanyRunService(self.client)
-        self.salary_documents = CompanySalaryDocumentService(self.client)
+        self.salary_documents = CompanySalaryDocumentService(self.client)  # TO BE implemented
         self.salary_table = CompanySalaryTableService(self.client)
         self.svw = CompanySvwService(self.client)
         self.wage_component = CompanyWageComponentService(self.client)
         self.wage_cost = CompanyWageCostService(self.client)
         self.wage_model = CompanyWageModelService(self.client)
         self.wage_tax = CompanyWageTaxService(self.client)
 
@@ -158,15 +158,15 @@
 
         Returns:
             Period: year, period and period type and the company.
         """
         period = self.client.service.Company_GetCurrentPeriod(CompanyId=company_id, _soapheaders=self.auth_header)
         if period is None:
             return None
-        return Period(serialize_object(period))
+        return Period(company_id=company_id, data=serialize_object(period))
 
     @nmbrs_exception_handler(resources=["CompanyService:Company_Insert"])
     def insert(
         self, debtor_id: int, name: str, period_type: int, default_id: int, labour_agreement_group_id: str, pay_in_advance: bool
     ) -> int:
         """
         Insert a new company.
@@ -209,15 +209,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             ContactPerson: The contact person details.
         """
         contact_person = self.client.service.ContactPerson_Get(CompanyId=company_id, _soapheaders=self.auth_header)
-        return ContactPerson(serialize_object(contact_person))
+        return ContactPerson(company_id=company_id, data=serialize_object(contact_person))
 
     @nmbrs_exception_handler(resources=["CompanyService:Converter_GetByCompany_IntToGuid"])
     def get_converter_mappings(self, company_id: int, entity: str) -> GuidConvertor:
         """
         Get converter mappings for the given entity and company ID.
 
         For more information, refer to the official documentation:
@@ -227,15 +227,15 @@
             company_id (int): The ID of the company.
             entity (str): The entity type (e.g., Employee, Company, Debtor).
 
         Returns:
             GuidConvertor: The converter mappings response.
         """
         guids = self.client.service.Converter_GetByCompany_IntToGuid(Entity=entity, CompanyId=company_id, _soapheaders=self.auth_header)
-        return GuidConvertor(serialize_object(guids))
+        return GuidConvertor(company_id=company_id, data=serialize_object(guids))
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:DefaultEmployeeTemplates_GetByCompany"])
     def get_default_employee_templates(self, company_id: int) -> list[DefaultEmployeeTemplate]:
         """
         Get available default employee templates by company.
 
@@ -245,15 +245,18 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Company]: A list of Company objects.
         """
         employee_templates = self.client.service.DefaultEmployeeTemplates_GetByCompany(CompanyId=company_id, _soapheaders=self.auth_header)
-        employee_templates = [DefaultEmployeeTemplate(employee_template) for employee_template in serialize_object(employee_templates)]
+        employee_templates = [
+            DefaultEmployeeTemplate(company_id=company_id, data=employee_template)
+            for employee_template in serialize_object(employee_templates)
+        ]
         return employee_templates
 
     @nmbrs_exception_handler(resources=["CompanyService:FileExplorer_UploadFile"])
     def upload_file(self, company_id: int, document_name: str, document_sub_folder: str, data: bytes) -> None:
         """
         Upload a document for a company.
 
@@ -290,15 +293,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             FulltimeSchedules: A FulltimeSchedules object.
         """
         response = self.client.service.Schedule_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
-        return FulltimeSchedules(serialize_object(response))
+        return FulltimeSchedules(company_id=company_id, data=serialize_object(response))
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:PayrollWorkflow_Get"])
     def get_payroll_workflow(self, company_id: int, year: int, period: int) -> list[PayrollWorkflowTrack]:
         """
         Get the company's payroll workflow tracks and actions.
 
@@ -310,9 +313,9 @@
             year (int): The year.
             period (int): The period.
 
         Returns:
             List[PayrollWorkflowTrack]: A list of PayrollWorkflowTrack objects.
         """
         responses = self.client.service.PayrollWorkflow_Get(CompanyId=company_id, Year=year, Period=period, _soapheaders=self.auth_header)
-        responses = [PayrollWorkflowTrack(response) for response in serialize_object(responses)]
+        responses = [PayrollWorkflowTrack(company_id=company_id, data=response) for response in serialize_object(responses)]
         return responses
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/debtor_service.py` & `nmbrs-0.1.0/src/nmbrs/service/debtor_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[ContactInfo]: A list of ContactInfo objects representing the accountant contact information.
         """
         accountants = self.debtor_service.service.AccountantContact_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
-        accountants = [ContactInfo(accountant) for accountant in serialize_object(accountants)]
+        accountants = [ContactInfo(debtor_id=debtor_id, data=accountant) for accountant in serialize_object(accountants)]
         return accountants
 
     @nmbrs_exception_handler(resources=["DebtorService:Address_Get"])
     def get_address(self, debtor_id: int) -> Address | None:
         """
         Retrieve address information for a debtor.
 
@@ -220,15 +220,15 @@
 
         Returns:
             Address | None: An Address object representing the address if found, otherwise None.
         """
         address = self.debtor_service.service.Address_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if address is None:
             return None
-        return Address(serialize_object(address))
+        return Address(debtor_id=debtor_id, data=serialize_object(address))
 
     @nmbrs_exception_handler(resources=["DebtorService:BankAccount_Get"])
     def get_bank_account(self, debtor_id: int) -> BankAccount | None:
         """
         Retrieve bank account information for a debtor.
 
         For more information, refer to the official documentation:
@@ -239,15 +239,15 @@
 
         Returns:
             BankAccount | None: A BankAccount object representing the bank account if found, otherwise None.
         """
         bank_account = self.debtor_service.service.BankAccount_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if bank_account is None:
             return None
-        return BankAccount(serialize_object(bank_account))
+        return BankAccount(debtor_id=debtor_id, data=serialize_object(bank_account))
 
     @nmbrs_exception_handler(resources=["DebtorService:ContactPerson_Get"])
     def get_contact_person(self, debtor_id: int) -> ContactInfo | None:
         """
         Retrieve contact person information for a debtor.
 
         For more information, refer to the official documentation:
@@ -258,15 +258,15 @@
 
         Returns:
             ContactInfo | None: A ContactInfo object representing the contact person if found, otherwise None.
         """
         contact_person = self.debtor_service.service.ContactPerson_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if contact_person is None:
             return None
-        return ContactInfo(serialize_object(contact_person))
+        return ContactInfo(debtor_id=debtor_id, data=serialize_object(contact_person))
 
     @nmbrs_exception_handler(resources=["DebtorService:Debtor_IsOwner"])
     def is_owner(self) -> bool:
         """
         Check if the current user is the owner of the debtor.
 
         For more information, refer to the official documentation:
@@ -295,15 +295,17 @@
         Returns:
             list[LabourAgreementSettings]: A list of LabourAgreementSettings objects representing all labour
             agreement settings.
         """
         labour_agreements = self.debtor_service.service.LabourAgreementSettings_GetList(
             DebtorId=debtor_id, Year=year, Period=period, _soapheaders=self.auth_header
         )
-        labour_agreements = [LabourAgreementSettings(labour_agreement) for labour_agreement in serialize_object(labour_agreements)]
+        labour_agreements = [
+            LabourAgreementSettings(debtor_id=debtor_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
+        ]
         return labour_agreements
 
     @return_list
     @nmbrs_exception_handler(resources=["DebtorService:Manager_GetList"])
     def get_all_managers(self, debtor_id: int) -> list[Manager]:
         """
         Retrieve all managers for a debtor.
@@ -314,15 +316,15 @@
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[Manager]: A list of Manager objects representing all managers for the debtor.
         """
         managers = self.debtor_service.service.Manager_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
-        managers = [Manager(manager) for manager in serialize_object(managers)]
+        managers = [Manager(debtor_id=debtor_id, data=manager) for manager in serialize_object(managers)]
         return managers
 
     @nmbrs_exception_handler(resources=["DebtorService:ServiceLevel_Get"])
     def get_service_level(self, debtor_id: int) -> ServiceLevel | None:
         """
         Retrieve service level information for a debtor.
 
@@ -335,15 +337,15 @@
         Returns:
             ServiceLevel | None: A ServiceLevel object representing the service level information if found, otherwise
             None.
         """
         service_level = self.debtor_service.service.ServiceLevel_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if service_level is None:
             return None
-        return ServiceLevel(serialize_object(service_level))
+        return ServiceLevel(debtor_id=debtor_id, data=serialize_object(service_level))
 
     @return_list
     @nmbrs_exception_handler(resources=["DebtorService:Tags_Get"])
     def get_tags(self, debtor_id: int) -> list[Tag]:
         """
         Retrieve all tags for a debtor.
 
@@ -353,9 +355,9 @@
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[Tag]: A list of Tag objects representing all tags associated with the debtor.
         """
         tags = self.debtor_service.service.Tags_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
-        tags = [Tag(tag) for tag in serialize_object(tags)]
+        tags = [Tag(debtor_id=debtor_id, data=tag) for tag in serialize_object(tags)]
         return tags
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/employee_service.py` & `nmbrs-0.1.0/src/nmbrs/service/employee_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,58 +32,57 @@
     EmployeeServiceService,
     EmployeeSpaarloonService,
     EmployeeSvwService,
     EmployeeTimeRegistrationService,
     EmployeeTimeScheduleService,
 )
 from .service import Service
-from ..data_classes.company import Period
-from ..data_classes.employee import EmployeeTypes, Employee
+from ..data_classes.employee import EmployeeTypes, Employee, Period
 from ..utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ..utils.return_list import return_list
 
 
 class EmployeeService(Service):
     """A class representing Employee Service for interacting with Nmbrs employee-related functionalities."""
 
     def __init__(self, sandbox: bool = True) -> None:
         super().__init__(sandbox)
 
         # Initialize nmbrs services
         self.client = Client(f"{self.base_uri}{self.employee_uri}")
 
         # Micro services
-        self.absence = EmployeeAbsenceService(self.client)
-        self.address = EmployeeAddressService(self.client)
-        self.bank_account = EmployeeBankAccountService(self.client)
-        self.child = EmployeeChildService(self.client)
-        self.contract = EmployeeContractService(self.client)
-        self.cost_center = EmployeeCostCenterService(self.client)
-        self.days = EmployeeDaysService(self.client)
-        self.department = EmployeeDepartmentsService(self.client)
-        self.document = EmployeeDocumentService(self.client)
-        self.employment = EmployeeEmploymentService(self.client)
-        self.function = EmployeeFunctionService(self.client)
-        self.hour_component = EmployeeHourComponentFixedService(self.client)
-        self.labour_agreement = EmployeeLabourAgreementService(self.client)
-        self.lease_car = EmployeeLeaseCarService(self.client)
-        self.leave = EmployeeLeaveService(self.client)
-        self.levensloop = EmployeeLevensLoopService(self.client)
-        self.manager = EmployeeManagerService(self.client)
-        self.partner = EmployeePartnerService(self.client)
-        self.personal_info = EmployeePersonalInfoService(self.client)
-        self.salary = EmployeeSalaryService(self.client)
-        self.schedule = EmployeeScheduleService(self.client)
-        self.service = EmployeeServiceService(self.client)
-        self.spaarloon = EmployeeSpaarloonService(self.client)
-        self.svw = EmployeeSvwService(self.client)
-        self.time_registration = EmployeeTimeRegistrationService(self.client)
-        self.time_schedule = EmployeeTimeScheduleService(self.client)
-        self.wage_component = EmployeeWageComponentsService(self.client)
-        self.wage_tax = EmployeeWageTaxService(self.client)
+        self.absence = EmployeeAbsenceService(self.client)  # TO BE implemented
+        self.address = EmployeeAddressService(self.client)  # TO BE implemented
+        self.bank_account = EmployeeBankAccountService(self.client)  # TO BE implemented
+        self.child = EmployeeChildService(self.client)  # TO BE implemented
+        self.contract = EmployeeContractService(self.client)  # TO BE implemented
+        self.cost_center = EmployeeCostCenterService(self.client)  # TO BE implemented
+        self.days = EmployeeDaysService(self.client)  # TO BE implemented
+        self.department = EmployeeDepartmentsService(self.client)  # TO BE implemented
+        self.document = EmployeeDocumentService(self.client)  # TO BE implemented
+        self.employment = EmployeeEmploymentService(self.client)  # TO BE implemented
+        self.function = EmployeeFunctionService(self.client)  # TO BE implemented
+        self.hour_component = EmployeeHourComponentFixedService(self.client)  # TO BE implemented
+        self.labour_agreement = EmployeeLabourAgreementService(self.client)  # TO BE implemented
+        self.lease_car = EmployeeLeaseCarService(self.client)  # TO BE implemented
+        self.leave = EmployeeLeaveService(self.client)  # TO BE implemented
+        self.levensloop = EmployeeLevensLoopService(self.client)  # TO BE implemented
+        self.manager = EmployeeManagerService(self.client)  # TO BE implemented
+        self.partner = EmployeePartnerService(self.client)  # TO BE implemented
+        self.personal_info = EmployeePersonalInfoService(self.client)  # TO BE implemented
+        self.salary = EmployeeSalaryService(self.client)  # TO BE implemented
+        self.schedule = EmployeeScheduleService(self.client)  # TO BE implemented
+        self.service = EmployeeServiceService(self.client)  # TO BE implemented
+        self.spaarloon = EmployeeSpaarloonService(self.client)  # TO BE implemented
+        self.svw = EmployeeSvwService(self.client)  # TO BE implemented
+        self.time_registration = EmployeeTimeRegistrationService(self.client)  # TO BE implemented
+        self.time_schedule = EmployeeTimeScheduleService(self.client)  # TO BE implemented
+        self.wage_component = EmployeeWageComponentsService(self.client)  # TO BE implemented
+        self.wage_tax = EmployeeWageTaxService(self.client)  # TO BE implemented
 
     def set_auth_header(self, auth_header: dict) -> None:
         """
         Method to set the authentication.
 
         Args:
             auth_header (dict): A dictionary containing authentication details.
@@ -149,15 +148,15 @@
 
         Returns:
             Period: year, period and period type and the company.
         """
         period = self.client.service.Employee_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_header)
         if period is None:
             return None
-        return Period(serialize_object(period))
+        return Period(employee_id=employee_id, data=serialize_object(period))
 
     @return_list
     @nmbrs_exception_handler(resources=["EmployeeService:List_GetByCompany"])
     def get_by_company(self, company_id: int, employee_type: int) -> list[Employee]:
         """
         Get all employees that belong to a company and to a specific employee type.
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/__init__.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/address.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Microservice responsible for address-related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
-from ....data_classes.debtor import Address
+from ....data_classes.company import Address
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ..micro_service import MicroService
 
 
 class CompanyAddressService(MicroService):
     """Microservice responsible for address-related actions on the company level."""
 
@@ -30,15 +30,15 @@
 
         Returns:
             Address | None: An Address object if found, otherwise None.
         """
         address = self.client.service.Address_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         if address is None:
             return None
-        return Address(serialize_object(address))
+        return Address(company_id=company_id, data=serialize_object(address))
 
     @nmbrs_exception_handler(resources=["CompanyService:Address_Insert"])
     def insert(
         self,
         company_id: int,
         address_id: int,
         default: bool,
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/bank_account.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/bank_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """Microservice responsible for bank account related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
-from ....data_classes.debtor import BankAccount
+from ....data_classes.company import BankAccount
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class CompanyBankAccountService(MicroService):
     """Microservice responsible for bank account related actions on the company level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @nmbrs_exception_handler(resources=["CompanyService:BankAccount_GetCurrent"])
-    def get_current(self, company_id: int) -> BankAccount:
+    def get_current(self, company_id: int) -> BankAccount | None:
         """
         Get the company's current bank account.
 
         For more information, refer to the official documentation:
             [BankAccount_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=BankAccount_GetCurrent)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             BankAccount: An BankAccount object.
         """
         bank_account = self.client.service.BankAccount_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         if bank_account is None:
-            return BankAccount({})
-        return BankAccount(serialize_object(bank_account))
+            return None
+        return BankAccount(company_id=company_id, data=serialize_object(bank_account))
 
     @nmbrs_exception_handler(resources=["CompanyService:BankAccount_Insert"])
     def insert(
         self,
         company_id: int,
         account_id: int,
         account_number: str,
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/cost_center.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/cost_center.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[CostCenter]: A list of cost center objects.
         """
         cost_centers = self.client.service.CostCenter_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
-        return [CostCenter(cost_center) for cost_center in serialize_object(cost_centers)]
+        return [CostCenter(company_id=company_id, data=cost_center) for cost_center in serialize_object(cost_centers)]
 
     @nmbrs_exception_handler(resources=["CompanyService:CostCenter_Insert"])
     def insert(self, company_id: int, cost_center_id: int, code: str, description: str) -> int:
         """
         Insert or update a cost center within a company.
 
         For further details, see the official documentation:
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/cost_unit.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/cost_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[CostUnit]: A list of cost unit objects.
         """
         cost_units = self.client.service.CostUnit_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
-        return [CostUnit(cost_unit) for cost_unit in serialize_object(cost_units)]
+        return [CostUnit(company_id=company_id, data=cost_unit) for cost_unit in serialize_object(cost_units)]
 
     @nmbrs_exception_handler(resources=["CompanyService:CostUnit_Insert"])
     def insert(self, company_id: int, cost_unit_id: int, code: str, description: str) -> int:
         """
         Update or insert a Cost Unit into a company.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/hour_model.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/hour_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[HourCode]: A list of hour code objects.
         """
         hour_codes = self.client.service.HourModel_GetHourCodes(CompanyId=company_id, _soapheaders=self.auth_header)
-        return [HourCode(hour_code) for hour_code in serialize_object(hour_codes)]
+        return [HourCode(company_id=company_id, data=hour_code) for hour_code in serialize_object(hour_codes)]
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:HourModel2_GetHourCodes"])
     def get_2(self, company_id: int) -> list[HourCode]:
         """
         Get hour codes that belong to a company's hour model 2.
 
@@ -48,8 +48,8 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[HourCode]: A list of hour code objects.
         """
         hour_codes = self.client.service.HourModel2_GetHourCodes(CompanyId=company_id, _soapheaders=self.auth_header)
-        return [HourCode(hour_code) for hour_code in serialize_object(hour_codes)]
+        return [HourCode(company_id=company_id, data=hour_code) for hour_code in serialize_object(hour_codes)]
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/journal.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/journal.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/labout_aggreement.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/labout_aggreement.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,17 @@
         """
         labour_agreements = self.client.service.LabourAgreements_Get(
             CompanyId=company_id,
             Period=period,
             Year=year,
             _soapheaders=self.auth_header,
         )
-        labour_agreements = [LabourAgreement(labour_agreement) for labour_agreement in serialize_object(labour_agreements)]
+        labour_agreements = [
+            LabourAgreement(company_id=company_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
+        ]
         return labour_agreements
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:LabourAgreements_GetCurrent"])
     def get_current(self, company_id: int):
         """
         Get a list of current labour agreements assigned to a company.
@@ -58,15 +60,17 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[LabourAgreement]: A list of LabourAgreement objects representing the current labour agreements.
         """
         labour_agreements = self.client.service.LabourAgreements_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
-        labour_agreements = [LabourAgreement(labour_agreement) for labour_agreement in serialize_object(labour_agreements)]
+        labour_agreements = [
+            LabourAgreement(company_id=company_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
+        ]
         return labour_agreements
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:CompanyLeaveTypeGroups_Get"])
     def get_leave_type_groups(
         self, company_id: int, labour_agreement_settings_group_id: int, year: int, period: int
     ) -> list[LeaveTypeGroup]:
@@ -88,8 +92,8 @@
         responses = self.client.service.CompanyLeaveTypeGroups_Get(
             CompanyId=company_id,
             LabourAgreementSettingsGroupId=labour_agreement_settings_group_id,
             Year=year,
             Period=period,
             _soapheaders=self.auth_header,
         )
-        return [LeaveTypeGroup(response) for response in serialize_object(responses)]
+        return [LeaveTypeGroup(company_id=company_id, data=response) for response in serialize_object(responses)]
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/pension.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/pension.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Pension]: A list of pension objects.
         """
         pensions = self.client.service.PensionExport_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
-        return [Pension(pension) for pension in serialize_object(pensions)]
+        return [Pension(company_id=company_id, data=pension) for pension in serialize_object(pensions)]
 
     @nmbrs_exception_handler(resources=["CompanyService:PensionExport_GetXML"])
     def get_xml(self, company_id: int, pension_export_id: int) -> PensionXML:
         """
         Returns one XML pension export by ID that belong to a company.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/run.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             company_id (int): The ID of the company.
             year (int): year.
 
         Returns:
             list[RunRequest]: A list of run requests objects.
         """
         run_requests = self.client.service.RunRequest_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_header)
-        return [RunRequest(run_request) for run_request in serialize_object(run_requests)]
+        return [RunRequest(company_id=company_id, data=run_request) for run_request in serialize_object(run_requests)]
 
     @nmbrs_exception_handler(resources=["CompanyService:RunRequest_Insert"])
     def insert_request(self, company_id: int):
         """
         Requests a run for given company.
 
         For more information, refer to the official documentation:
@@ -64,15 +64,15 @@
             company_id (int): The ID of the company.
             year (int): year.
 
         Returns:
             list[RunInfo]: A list of run info objects.
         """
         runs = self.client.service.Run_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_header)
-        return [RunInfo(run) for run in serialize_object(runs)]
+        return [RunInfo(company_id=company_id, data=run) for run in serialize_object(runs)]
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:Run_GetEmployeesByRunCompany"])
     def get_all_employees_by_run(self, company_id: int, year: int, run_id: int) -> list[Employee]:
         """
         Get the employee's list for a specified company id, run id and year
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/salary_document.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/salary_document.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/salary_table.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/salary_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             period (int): Period.
             year (int): Year.
 
         Returns:
             list[SalaryTable]: A list of salary table objects.
         """
         salary_tables = self.client.service.SalaryTable_Get(CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header)
-        return [SalaryTable(salary_table) for salary_table in serialize_object(salary_tables)]
+        return [SalaryTable(company_id=company_id, data=salary_table) for salary_table in serialize_object(salary_tables)]
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:SalaryTable2_Get"])
     def get_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
         Returns a list of available tables for the company with unique identifiers.
 
@@ -72,15 +72,15 @@
             period (int): Period.
             year (int): Year.
 
         Returns:
             list[SalaryTableScale]: A list of salary table scale objects.
         """
         scales = self.client.service.SalaryTable_GetScales(CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header)
-        return [SalaryTableScale(scale) for scale in serialize_object(scales)]
+        return [SalaryTableScale(company_id=company_id, data=scale) for scale in serialize_object(scales)]
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:SalaryTable2_GetScales"])
     def get_scale_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
         Returns a list of available scales for the company salary table with unique identifiers.
 
@@ -124,15 +124,15 @@
             "ScaleValue": scale.value,
             "ScalePercentageMax": scale.percentage_max,
             "ScalePercentageMin": scale.percentage_min,
         }
         steps = self.client.service.SalaryTable_GetSteps(
             CompanyId=company_id, Period=period, Year=year, Scale=_scale, _soapheaders=self.auth_header
         )
-        return [SalaryTableStep(step) for step in serialize_object(steps)]
+        return [SalaryTableStep(company_id=company_id, data=step) for step in serialize_object(steps)]
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:SalaryTable2_GetSteps"])
     def get_step_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
         Returns a list of available steps for the company salary table and selected scale with unique identifiers.
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/svw.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/svw.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             SVW: object representing svw settings
         """
         svw = self.client.service.SVW_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
-        return SVW(serialize_object(svw))
+        return SVW(company_id=company_id, data=serialize_object(svw))
 
     @nmbrs_exception_handler(resources=["CompanyService:SVW_UpdateCurrent"])
     def insert_current(self, company_id: int, svw: SVW) -> None:
         """
         Update the current SVW settings.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/wage_component.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/wage_component.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,147 +1,199 @@
 # pylint: disable=line-too-long
-"""Microservice responsible for wage component related actions on the company level."""
+"""Microservice responsible for wage components related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class CompanyWageComponentService(MicroService):
-    """Microservice responsible for wage component related actions on the company level."""
+class EmployeeWageComponentsService(MicroService):
+    """Microservice responsible for wage components related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_Get"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponent_Delete"])
+    def delete(self):
+        """
+        Delete a wage component by ID.
+
+        For more information, refer to the official documentation:
+            [WageComponent_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponent_Delete)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponent_Update"])
+    def update(self):
+        """
+        Update any wage Component Variable or Fixed.
+        In case of being a Fixed Wage Component the parameters EndYear and EndPeriod inside the method can be specified.
+        If the period is before the company's current period, unprotected mode flag is required.
+
+        For more information, refer to the official documentation:
+            [WageComponent_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponent_Update)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Get"])
     def fixed_get(self):
         """
         Get all fixed wage components for given period.
 
         For more information, refer to the official documentation:
-            [WageComponentFixed_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_Get)
+            [WageComponentFixed_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_GetCurrent"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_GetCurrent"])
     def fixed_get_current(self):
         """
         Get all fixed wage components for the current period.
 
         For more information, refer to the official documentation:
-            [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_GetCurrent)
+            [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_Insert"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_GetCurrent"])
     def fixed_insert(self):
         """
         Insert a wage component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [WageComponentFixed_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_Insert)
+            [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_InsertCurrent"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Insert_With_End"])
+    def fixed_insert_with_end(self):
+        """
+        Insert a wage component to given period of time. If the start period is before the company's current period, unprotected mode flag is required.
+
+        For more information, refer to the official documentation:
+            [WageComponentFixed_Insert_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_With_End)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_InsertCurrent"])
     def fixed_insert_current(self):
         """
         Insert a wage component to the current period.
 
         For more information, refer to the official documentation:
-            [WageComponentFixed_InsertCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_InsertCurrent)
+            [WageComponentFixed_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_InsertCurrent)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_InsertCurrent_With_End"])
+    def fixed_insert_current_with_end(self):
+        """
+        Insert a wage component to the current period with end period.
+
+        For more information, refer to the official documentation:
+            [WageComponentFixed_InsertCurrent_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_InsertCurrent_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_Insert_Batch"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Insert_Batch"])
     def fixed_insert_batch(self):
         """
         Insert a batch of wage components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [WageComponentFixed_Insert_Batch](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_Insert_Batch)
+            [WageComponentFixed_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_Batch)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Insert_Batch_With_End"])
+    def fixed_insert_batch_with_end(self):
+        """
+        Insert a batch of wage components to given period of time. If the start period is before the company's current period, unprotected mode flag is required.
+
+        For more information, refer to the official documentation:
+            [WageComponentFixed_Insert_Batch_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_Batch_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_Stop"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Stop"])
     def fixed_stop(self):
         """
         Stop a wage component ending after given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [WageComponentFixed_Stop](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_Stop)
+            [WageComponentFixed_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Stop)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_Get"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_Get"])
     def variable_get(self):
         """
-        Get all fixed wage components for given period.
+        Get all variable wage components for given period.
 
         For more information, refer to the official documentation:
-            [WageComponentVar_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_Get)
+            [WageComponentVar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_GetCurrent"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_GetCurrent"])
     def variable_get_current(self):
         """
-        Get all fixed wage components for the current period.
+        Get all variable wage components for the current period.
 
         For more information, refer to the official documentation:
-            [WageComponentVar_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_GetCurrent)
+            [WageComponentVar_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_Insert"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_Insert"])
     def variable_insert(self):
         """
         Insert a wage component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [WageComponentVar_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_Insert)
+            [WageComponentVar_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_InsertCurrent"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_InsertCurrent"])
     def variable_insert_current(self):
         """
-        Insert a wage component to the current period.
+        Insert a wage components to the current period.
 
         For more information, refer to the official documentation:
-            [WageComponentVar_InsertCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_InsertCurrent)
+            [WageComponentVar_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_Insert_Batch"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_Insert_Batch"])
     def variable_insert_batch(self):
         """
         Insert a batch of wage components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [WageComponentVar_Insert_Batch](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_Insert_Batch)
+            [WageComponentVar_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_Clear"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_Clear"])
     def variable_clear(self):
         """
         Clear all variable wage components for given period.
 
         For more information, refer to the official documentation:
-            [WageComponentVar_Clear](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_Clear)
+            [WageComponentVar_Clear](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Clear)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_ClearCurrent"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_ClearCurrent"])
     def variable_clear_current(self):
         """
         Clear all variable wage components for the current period.
 
         For more information, refer to the official documentation:
-            [WageComponentVar_ClearCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_ClearCurrent)
+            [WageComponentVar_ClearCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_ClearCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/company/wage_tax.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/company/wage_tax.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,84 @@
-"""Microservice responsible for wagetax-related actions on the company level."""
+"""Microservice responsible for managing wage tax-related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ....data_classes.company import WageTax, WageTaxXML
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyWageTaxService(MicroService):
-    """Microservice responsible for wagetax-related actions on the company level."""
+    """Microservice responsible for managing wage tax-related actions on the company level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
     @nmbrs_exception_handler(resources=["CompanyService:WageTax_GetList"])
     def get_all_wagetax(self, company_id: int, year: int) -> list[WageTax]:
         """
         Retrieve all wage taxes for a specific company and year.
 
         For more information, refer to the official documentation:
-            [Soap call WageTax_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageTax_GetList)
+            [WageTax_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageTax_GetList)
 
         Args:
             company_id (int): The ID of the company.
             year (int): The year for which wage taxes are retrieved.
 
         Returns:
             list[WageTax]: A list of WageTax objects for the specified company and year.
         """
         wage_taxes = self.client.service.WageTax_GetList(CompanyId=company_id, intYear=year, _soapheaders=self.auth_header)
-        wage_taxes = [WageTax(wage_tax) for wage_tax in serialize_object(wage_taxes)]
+        wage_taxes = [WageTax(company_id=company_id, data=wage_tax) for wage_tax in serialize_object(wage_taxes)]
         return wage_taxes
 
     @nmbrs_exception_handler(resources=["CompanyService:WageTax_GetXML"])
-    def get_wagetax_details(self, company_id: int, loonaangifte_id) -> WageTaxXML:
+    def get_wagetax_details(self, company_id: int, loonaangifte_id: int) -> WageTaxXML:
         """
         Retrieve wage tax details for a specific company and loonaangifte ID.
 
         For more information, refer to the official documentation:
-            [Soap call WageTax_GetXML](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageTax_GetXML)
+            [WageTax_GetXML](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageTax_GetXML)
 
         Args:
             company_id (int): The ID of the company.
-            loonaangifte_id: The loonaangifte ID.
+            loonaangifte_id (int): The loonaangifte ID.
 
         Returns:
             WageTaxXML: An wage tax object detailing the specified company and loonaangifte ID.
         """
         wage_tax_details = self.client.service.WageTax_GetXML(
             CompanyId=company_id,
             LoonaangifteID=loonaangifte_id,
             _soapheaders=self.auth_header,
         )
         wage_tax_details = WageTaxXML(wage_tax_details)
         return wage_tax_details
 
     @nmbrs_exception_handler(resources=["CompanyService:WageTax_SetSentExternal"])
-    def set_send_as_external(self):
+    def set_send_as_external(self, company_id: int, loonaangifte_id: int) -> bool:
         """
-        Set wage tax status to Sent as External.
+        Set the wage tax status to Sent as External.
 
         For more information, refer to the official documentation:
             [WageTax_SetSentExternal](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageTax_SetSentExternal)
+
+        Args:
+            company_id (int): The ID of the company.
+            loonaangifte_id (int): The loonaangifte ID.
+
+        Returns:
+            bool: A boolean indicating if the wage tax was send externally.
         """
-        raise NotImplementedError()  # pragma: no cover
+        response = self.client.service.WageTax_SetSentExternal(
+            CompanyId=company_id,
+            LoonaangifteID=loonaangifte_id,
+            _soapheaders=self.auth_header,
+        )
+        return response
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/department.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/department.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[Department]: A list of Department objects representing all departments of the debtor.
         """
         departments = self.client.service.Department_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
-        departments = [Department(department) for department in serialize_object(departments)]
+        departments = [Department(debtor_id=debtor_id, data=department) for department in serialize_object(departments)]
         return departments
 
     @nmbrs_exception_handler(resources=["DebtorService:Department_Insert"])
     def insert(self, debtor_id: int, department_id: int, code: int, description: str) -> int:
         """
         Insert a new department for a debtor.
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/function.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,30 +30,30 @@
             debtor_id (int): The ID of the debtor.
             function_id (int): The ID of the function to be deleted.
         """
         self.client.service.Function_Delete(DebtorId=debtor_id, id=function_id, _soapheaders=self.auth_header)
 
     @return_list
     @nmbrs_exception_handler(resources=["DebtorService:Function_GetList"])
-    def get_all(self, debtor_id: int, function_id: int) -> list[Function]:
+    def get_all(self, debtor_id: int) -> list[Function]:
         """
         Retrieve all functions of a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Function_GetList](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Function_GetList)
 
         Args:
             debtor_id (int): The ID of the debtor.
             function_id (int): The ID of the function.
 
         Returns:
             list[Function]: A list of Function objects representing all functions of the debtor.
         """
-        functions = self.client.service.Function_GetList(DebtorId=debtor_id, id=function_id, _soapheaders=self.auth_header)
-        functions = [Function(function) for function in serialize_object(functions)]
+        functions = self.client.service.Function_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        functions = [Function(debtor_id=debtor_id, data=function) for function in serialize_object(functions)]
         return functions
 
     @nmbrs_exception_handler(resources=["DebtorService:Function_Insert"])
     def insert(self, debtor_id: int, function_id: int, code: int, description: str) -> int:
         """
         Insert a new function for a debtor.
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/title.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/title.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/debtor/webook.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/debtor/webook.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[WebhookSetting]: A list of WebhookSetting objects representing all webhooks associated with the debtor.
         """
         webhooks = self.client.service.WebhookSettings_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
-        webhooks = [WebhookSetting(webhook) for webhook in serialize_object(webhooks)]
+        webhooks = [WebhookSetting(debtor_id=debtor_id, data=webhook) for webhook in serialize_object(webhooks)]
         return webhooks
 
     @return_list
     @nmbrs_exception_handler(resources=["DebtorService:WebhookSettings_GetEvents"])
     def get_all_events(self) -> list[Event]:
         """
         Retrieve all webhook events.
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/__init__.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/absence.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/absence.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/address.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/address.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/bank_account.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/bank_account.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/child.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/child.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/contract.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,78 @@
 # pylint: disable=line-too-long
-"""Microservice responsible for contract related actions on the employee level."""
+"""Microservice responsible for service related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeContractService(MicroService):
-    """Microservice responsible for contract related actions on the employee level."""
+class EmployeeServiceService(MicroService):
+    """Microservice responsible for service related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_GetAll"])
+    @nmbrs_exception_handler(resources=["EmployeeService:Service_GetList"])
     def get_all(self):
         """
-        Get all contracts for the specified employee.
+        Get all service intervals.
 
         For more information, refer to the official documentation:
-            [Contract_GetAll](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_GetAll)
+            [Service_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_GetCurrentPeriod"])
-    def get_current(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:Service_Insert"])
+    def insert(self):
         """
-        Get a list of all active contracts for specified employee in current period.
+        Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [Contract_GetCurrentPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_GetCurrentPeriod)
+            [Service_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_GetAll_AllEmployeesByCompany"])
-    def get_all_by_company(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:Service_Insert2"])
+    def insert_2(self):
         """
-        Get all contracts of all employees.
+        Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [Contract_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_GetAll_AllEmployeesByCompany)
+            [Service_Insert2](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_Delete"])
+    @nmbrs_exception_handler(resources=["EmployeeService:Service_Delete"])
     def delete(self):
         """
-        Delete a contract from the system. This action can not be undone.
-
-        For more information, refer to the official documentation:
-            [Contract_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_Delete)
-        """
-        raise NotImplementedError()  # pragma: no cover
-
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_Update"])
-    def update(self):
-        """
-        Update the specified contract for specified employee. Contract start date can’t be updated, this field will be ignored.
+        Delete a service interval.
 
         For more information, refer to the official documentation:
-            [Contract_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_Update)
+            [Service_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_Insert"])
-    def insert(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:Service_StopCurrent"])
+    def stop_current(self):
         """
-        Insert Contract. If the start date is before the company's current period, unprotected mode flag is required.
+        Stop the current service interval. If the date is before the company's current period, unprotected mode flag is required.
+        If the employee income type requires and the employee is an applicant the EndServiceReasonId is mandatory, otherwise this field is ignored whatever the value is passed.
 
         For more information, refer to the official documentation:
-            [Contract_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_Insert)
+            [Service_StopCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_StopCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_InsertCurrentPeriod"])
-    def insert_current(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:Service_RemoveOutService"])
+    def remove_out_service(self):
         """
-        Insert Contract in current period for specified employee.
+        Remove out of service date.
 
         For more information, refer to the official documentation:
-            [Contract_InsertCurrentPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_InsertCurrentPeriod)
+            [Service_RemoveOutService](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_RemoveOutService)
         """
         raise NotImplementedError()  # pragma: no cover
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/cost_center.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/cost_center.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/days.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/days.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/department.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/department.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/document.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/document.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/employment.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/employment.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/function.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/function.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/hour_component.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/hour_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/labour_agreement.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/labour_agreement.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/lease_car.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/lease_car.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/leave.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/leave.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/levensloop.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/levensloop.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/manager.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/manager.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/partner.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/partner.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/personal_info.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/personal_info.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/salary.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/salary.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/schedule.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/schedule.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pylint: disable=line-too-long
 """Microservice responsible for schedule related actions on the employee level."""
 
 from zeep import Client
+from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....data_classes.employee import Schedule
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeScheduleService(MicroService):
     """Microservice responsible for schedule related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
@@ -43,22 +45,34 @@
 
         For more information, refer to the official documentation:
             [Schedule_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resources=["EmployeeService:Schedule_GetAll_AllEmployeesByCompany"])
-    def get_all_by_company(self):
+    def get_all_by_company(self, company_id: int) -> list[Schedule]:
         """
         Get all schedules of all employees from company.
 
         For more information, refer to the official documentation:
             [Schedule_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_GetAll_AllEmployeesByCompany)
+
+        Args:
+            company_id (int): The ID of the company.
+
+        Returns:
+            list[Contract]: a list of contract objects
         """
-        raise NotImplementedError()  # pragma: no cover
+        schedules = self.client.service.Schedule_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        schedules = serialize_object(schedules)
+        _schedules = []
+        for employee in schedules:
+            for schedule in employee["EmployeeSchedules"]["Schedule_V2"]:
+                _schedules.append(Schedule(employee_id=employee["EmployeeId"], data=schedule))
+        return _schedules
 
     @nmbrs_exception_handler(resources=["EmployeeService:ScheduleCalendar_Get"])
     def get_calender(self):
         """
         Get the employee's schedule calendar for given period.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/service.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/svw.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,76 @@
-# pylint: disable=line-too-long
-"""Microservice responsible for service related actions on the employee level."""
+"""Microservice responsible for svw related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeServiceService(MicroService):
-    """Microservice responsible for service related actions on the employee level."""
+class EmployeeSvwService(MicroService):
+    """Microservice responsible for svw related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_GetList"])
-    def get_all(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:SVW_Get"])
+    def get(self):
         """
-        Get all service intervals.
+        Get the active SVW settings for given period.
 
         For more information, refer to the official documentation:
-            [Service_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_GetList)
+            [SVW_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_Insert"])
-    def insert(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetCurrent"])
+    def get_current(self):
         """
-        Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
+        Get the currently active SVW settings.
 
         For more information, refer to the official documentation:
-            [Service_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert)
+            [SVW_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_Insert2"])
-    def insert_2(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetList"])
+    def get_all(self):
         """
-        Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
+        Get a list of all SVW settings.
 
         For more information, refer to the official documentation:
-            [Service_Insert2](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert2)
+            [SVW_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_Delete"])
-    def delete(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetAll_AllEmployeesByCompany"])
+    def get_all_by_company(self):
         """
-        Delete a service interval.
+        Get all (historical) svw setting records for all employees that belong to the company.
 
         For more information, refer to the official documentation:
-            [Service_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Delete)
+            [SVW_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_StopCurrent"])
-    def stop_current(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:SVW_Update"])
+    def update(self):
         """
-        Stop the current service interval. If the date is before the company's current period, unprotected mode flag is required.
-        If the employee income type requires and the employee is an applicant the EndServiceReasonId is mandatory, otherwise this field is ignored whatever the value is passed.
+        Update SVW settings starting from given period.
 
         For more information, refer to the official documentation:
-            [Service_StopCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_StopCurrent)
+            [SVW_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_RemoveOutService"])
-    def remove_out_service(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:SVW_UpdateCurrent"])
+    def update_current(self):
         """
-        Remove out of service date.
+        Update SVW settings starting from the current period.
 
         For more information, refer to the official documentation:
-            [Service_RemoveOutService](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_RemoveOutService)
+            [SVW_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_UpdateCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/spaarloon.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/spaarloon.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/svw.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/wage_tax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-"""Microservice responsible for svw related actions on the employee level."""
+"""Microservice responsible for wage tax related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeSvwService(MicroService):
-    """Microservice responsible for svw related actions on the employee level."""
+class EmployeeWageTaxService(MicroService):
+    """Microservice responsible for wage tax related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_Get"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageTax_Get"])
     def get(self):
         """
-        Get the active SVW settings for given period.
+        Get the active loonheffing settings for given period.
 
         For more information, refer to the official documentation:
-            [SVW_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_Get)
+            [WageTax_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetCurrent"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageTax_GetCurrent"])
     def get_current(self):
         """
-        Get the currently active SVW settings.
+        Get the currently active loonheffing settings.
 
         For more information, refer to the official documentation:
-            [SVW_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetCurrent)
+            [WageTax_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetList"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageTax_GetList"])
     def get_all(self):
         """
-        Get a list of all SVW settings.
+        Get a list of all loonheffing settings.
 
         For more information, refer to the official documentation:
-            [SVW_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetList)
+            [WageTax_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetAll_AllEmployeesByCompany"])
-    def get_all_by_company(self):
+    @nmbrs_exception_handler(resources=["EmployeeService:WageTax_Get_SE"])
+    def get_settings(self):
         """
-        Get all (historical) svw setting records for all employees that belong to the company.
+        Get active wage tax settings for a specific period.
 
         For more information, refer to the official documentation:
-            [SVW_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetAll_AllEmployeesByCompany)
+            [WageTax_Get_SE](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Get_SE)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_Update"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageTax_Update"])
     def update(self):
         """
-        Update SVW settings starting from given period.
+        Update loonheffing settings starting from given period
 
         For more information, refer to the official documentation:
-            [SVW_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_Update)
+            [WageTax_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_UpdateCurrent"])
+    @nmbrs_exception_handler(resources=["EmployeeService:WageTax_UpdateCurrent"])
     def update_current(self):
         """
-        Update SVW settings starting from the current period.
+        Update loonheffing settings starting from the current period.
 
         For more information, refer to the official documentation:
-            [SVW_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_UpdateCurrent)
+            [WageTax_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_UpdateCurrent)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resources=["EmployeeService:WageTax_Update_SE"])
+    def update_settings(self):
+        """
+        Update loonheffing settings starting from given period.
+
+        For more information, refer to the official documentation:
+            [WageTax_Update_SE](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Update_SE)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/time_registration.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/time_registration.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/employee/time_schedule.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/employee/time_schedule.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/microservices/micro_service.py` & `nmbrs-0.1.0/src/nmbrs/service/microservices/micro_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/service.py` & `nmbrs-0.1.0/src/nmbrs/service/service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/service/sso_service.py` & `nmbrs-0.1.0/src/nmbrs/service/sso_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/utils/find_empty_params.py` & `nmbrs-0.1.0/src/nmbrs/utils/find_empty_params.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/utils/nmbrs_exception_handler.py` & `nmbrs-0.1.0/src/nmbrs/utils/nmbrs_exception_handler.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs/utils/return_list.py` & `nmbrs-0.1.0/src/nmbrs/utils/return_list.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.0.405/src/nmbrs.egg-info/PKG-INFO` & `nmbrs-0.1.0/src/nmbrs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.0.405
+Version: 0.1.0
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/Visma-NMBRS-SOAP-API-SDK
```

### Comparing `nmbrs-0.0.405/src/nmbrs.egg-info/SOURCES.txt` & `nmbrs-0.1.0/src/nmbrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

