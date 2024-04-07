# Comparing `tmp/akello-0.0.21.tar.gz` & `tmp/akello-0.0.22.tar.gz`

## Comparing `akello-0.0.21.tar` & `akello-0.0.22.tar`

### file list

```diff
@@ -1,136 +1,135 @@
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 akello-0.0.21/.dockerignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 akello-0.0.21/Dockerfile
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 akello-0.0.21/Dockerfile.aws.lambda
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/__init__.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 akello-0.0.21/management.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/module_name.md
--rw-r--r--   0        0        0    24160 2020-02-02 00:00:00.000000 akello-0.0.21/openapi.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 akello-0.0.21/openapi.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 akello-0.0.21/publish_test_pypi.sh
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 akello-0.0.21/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/.gitignore
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/api-server.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/modules.xml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/vcs.xml
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/workspace.xml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 akello-0.0.21/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 akello-0.0.21/akello/app_configs.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 akello-0.0.21/akello/main.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 akello-0.0.21/akello/secrets.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 akello-0.0.21/akello/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/endpoints/__init__.py
--rw-r--r--   0        0        0    21517 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/endpoints/registry.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/endpoints/reports.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 akello-0.0.21/akello/api/app/v1/endpoints/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/provider.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/aws_cognito/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/aws_cognito/__init__.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/aws_cognito/auth_settings.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 akello-0.0.21/akello/auth/aws_cognito/aws_cognito.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.template.api.env
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.template.env
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/akello.py
--rwxr-xr-x   0        0        0      510 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/dev-build-single.sh
--rwxr-xr-x   0        0        0     2581 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/dev-setup-local.sh
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/docker-compose.yml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.cognito/config.json
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.cognito/db/clients.json
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/.cognito/db/local_4yfGDg3h.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/__init__.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/analytics.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/local.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/setup.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 akello-0.0.21/akello/cli/commands/start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/__init__.py
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/models.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/connector/__init__.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/connector/dynamodb.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 akello-0.0.21/akello/db/connector/s3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/decorators/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 akello-0.0.21/akello/decorators/akello_plan_tier.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 akello-0.0.21/akello/decorators/mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/__init__.py
--rw-r--r--   0        0        0  4322416 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/fhir.schema.json
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/hl7/README.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/hl7/__init__.py
--rw-r--r--   0        0        0   648807 2020-02-02 00:00:00.000000 akello-0.0.21/akello/fhir/hl7/fhir_v6_models.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/__init__.py
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/FHIR/phq9_fhir.json
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/FHIR/phq9_response.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/R4/__init__.py
--rw-r--r--   0        0        0    22471 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/R4/gad7.R4.json
--rw-r--r--   0        0        0    32684 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/R4/phq9.R4.json
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/FHIR_weights.template
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/api_weights.template
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/survey_GAD-7.yaml
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/survey_HEADS-ED.yaml
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/survey_PHQ-9.yaml
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/measurements/survey_PMQ.yaml
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/questionnaires/gad7.json
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 akello-0.0.21/akello/screeners/questionnaires/phq9.json
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/__init__.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/akello_apps.py
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/registry.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/reports.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/screeners.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/stripe_payment.py
--rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/user.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_decorators.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_registry_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_reports_service.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_screeners_service.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 akello-0.0.21/akello/services/tests/test_user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/akello/utils/email.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 akello-0.0.21/commands/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/commands/__init__.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/__init__.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/patient.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/registry.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/treatment_log.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 akello-0.0.21/commands/mock/user.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 akello-0.0.21/docs/Makefile
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.api.fhir.rst
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.api.fhir.v1.endpoints.rst
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.api.fhir.v1.rst
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.api.rst
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.auth.aws_cognito.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.auth.rst
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.db.connector.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.db.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.decorators.rst
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.fhir.hl7.rst
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.fhir.rst
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.rst
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.screeners.R4.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.screeners.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.services.rst
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.services.tests.rst
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 akello-0.0.21/docs/akello.utils.rst
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 akello-0.0.21/docs/conf.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 akello-0.0.21/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 akello-0.0.21/docs/make.bat
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 akello-0.0.21/docs/modules.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/README.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/generate_data.sh
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/load_fhir_data.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 akello-0.0.21/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 akello-0.0.21/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 akello-0.0.21/LICENSE
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 akello-0.0.21/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 akello-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 akello-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 akello-0.0.22/.dockerignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 akello-0.0.22/Dockerfile
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 akello-0.0.22/Dockerfile.aws.lambda
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/__init__.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 akello-0.0.22/management.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/module_name.md
+-rw-r--r--   0        0        0    24160 2020-02-02 00:00:00.000000 akello-0.0.22/openapi.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 akello-0.0.22/openapi.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 akello-0.0.22/publish_test_pypi.sh
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 akello-0.0.22/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/.gitignore
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/api-server.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/modules.xml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/vcs.xml
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/workspace.xml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 akello-0.0.22/akello/app_configs.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 akello-0.0.22/akello/main.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 akello-0.0.22/akello/secrets.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 akello-0.0.22/akello/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/endpoints/__init__.py
+-rw-r--r--   0        0        0    21517 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/endpoints/registry.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/endpoints/reports.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/endpoints/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/provider.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/aws_cognito/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/aws_cognito/__init__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/aws_cognito/auth_settings.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/aws_cognito/aws_cognito.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.template.api.env
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.template.env
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/akello.py
+-rwxr-xr-x   0        0        0      510 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/dev-build-single.sh
+-rwxr-xr-x   0        0        0     2581 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/dev-setup-local.sh
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/docker-compose.yml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.cognito/config.json
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.cognito/db/clients.json
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.cognito/db/local_4yfGDg3h.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/analytics.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/build.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/setup.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/__init__.py
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/models.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/connector/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/connector/dynamodb.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/connector/s3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/decorators/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 akello-0.0.22/akello/decorators/akello_plan_tier.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 akello-0.0.22/akello/decorators/mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/__init__.py
+-rw-r--r--   0        0        0  4322416 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/fhir.schema.json
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/hl7/README.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/hl7/__init__.py
+-rw-r--r--   0        0        0   648807 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/hl7/fhir_v6_models.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/__init__.py
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/FHIR/phq9_fhir.json
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/FHIR/phq9_response.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/R4/__init__.py
+-rw-r--r--   0        0        0    22471 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/R4/gad7.R4.json
+-rw-r--r--   0        0        0    32684 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/R4/phq9.R4.json
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/FHIR_weights.template
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/api_weights.template
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/survey_GAD-7.yaml
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/survey_HEADS-ED.yaml
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/survey_PHQ-9.yaml
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/survey_PMQ.yaml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/questionnaires/gad7.json
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/questionnaires/phq9.json
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/__init__.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/akello_apps.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/registry.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/reports.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/screeners.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/stripe_payment.py
+-rw-r--r--   0        0        0    10559 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/user.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_decorators.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_registry_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_reports_service.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_screeners_service.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/utils/email.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 akello-0.0.22/commands/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/commands/__init__.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/__init__.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/patient.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/registry.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/treatment_log.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/user.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 akello-0.0.22/docs/Makefile
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.api.fhir.rst
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.api.fhir.v1.endpoints.rst
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.api.fhir.v1.rst
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.api.rst
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.auth.aws_cognito.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.auth.rst
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.db.connector.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.db.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.decorators.rst
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.fhir.hl7.rst
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.fhir.rst
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.screeners.R4.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.screeners.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.services.rst
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.services.tests.rst
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.utils.rst
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 akello-0.0.22/docs/conf.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 akello-0.0.22/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 akello-0.0.22/docs/make.bat
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 akello-0.0.22/docs/modules.rst
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/README.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/generate_data.sh
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/load_fhir_data.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 akello-0.0.22/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 akello-0.0.22/LICENSE
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 akello-0.0.22/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 akello-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 akello-0.0.22/PKG-INFO
```

### Comparing `akello-0.0.21/.dockerignore` & `akello-0.0.22/.dockerignore`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/management.py` & `akello-0.0.22/management.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/openapi.json` & `akello-0.0.22/openapi.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/requirements.txt` & `akello-0.0.22/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 charset-normalizer==3.3.0
 click==8.1.7
 cognitojwt==1.4.1
 commonmark==0.9.1
 constructs==10.3.0
 cryptography==42.0.4
 dnspython==2.4.2
+docker==7.0.0
 docutils==0.20.1
 ecdsa==0.18.0
 email-validator==2.0.0.post2
 exceptiongroup==1.1.3
 Faker==22.6.0
 fastapi==0.109.1
 fastapi-cognito==2.4.2
@@ -68,14 +69,15 @@
 more-itertools==10.1.0
 multidict==6.0.4
 nh3==0.2.14
 numpy==1.26.4
 orjson==3.9.15
 packaging==23.2
 pandas==2.2.1
+pkginfo==1.10.0
 ply==3.11
 publication==0.0.3
 pyasn1==0.5.0
 pycparser==2.21
 pydantic==2.4.2
 pydantic-extra-types==2.1.0
 pydantic-settings==2.0.3
@@ -116,14 +118,15 @@
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
 starkbank-ecdsa==2.2.0
 starlette==0.35.1
 stripe==8.8.0
 tabulate==0.9.0
+twine==5.0.0
 typeguard==2.13.3
 typer==0.9.0
 typing_extensions==4.8.0
 tzdata==2024.1
 ua-parser==0.18.0
 ujson==5.8.0
 urllib3==1.26.18
```

### Comparing `akello-0.0.21/.idea/api-server.iml` & `akello-0.0.22/.idea/api-server.iml`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/.idea/workspace.xml` & `akello-0.0.22/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/app_configs.yaml` & `akello-0.0.22/akello/app_configs.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/main.py` & `akello-0.0.22/akello/main.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/secrets.py` & `akello-0.0.22/akello/secrets.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/api/app/v1/endpoints/registry.py` & `akello-0.0.22/akello/api/app/v1/endpoints/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/api/app/v1/endpoints/reports.py` & `akello-0.0.22/akello/api/app/v1/endpoints/reports.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/api/app/v1/endpoints/user.py` & `akello-0.0.22/akello/api/app/v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/auth/aws_cognito/README.md` & `akello-0.0.22/akello/auth/aws_cognito/README.md`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/auth/aws_cognito/auth_settings.py` & `akello-0.0.22/akello/auth/aws_cognito/auth_settings.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/auth/aws_cognito/aws_cognito.py` & `akello-0.0.22/akello/auth/aws_cognito/aws_cognito.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/cli/dev-setup-local.sh` & `akello-0.0.22/akello/cli/dev-setup-local.sh`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/cli/.cognito/db/local_4yfGDg3h.json` & `akello-0.0.22/akello/cli/.cognito/db/local_4yfGDg3h.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/cli/commands/analytics.py` & `akello-0.0.22/akello/cli/commands/analytics.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,46 +22,46 @@
     UNDERLINE = '\033[4m'
 
 @click.command()
 @click.option('--region', required=True, help='AWS region.')
 @click.option('--profile', required=True, help='AWS profile to use.')
 @click.option('--userpool-id', required=True, help='AWS cognito user-pool')
 @click.option('--dynamodb-table', required=True, help='DynamoDB Table used to analyze.')
-def analytics(region, profile, userpool_id, dynamodb_table):    
+def analytics(region, profile, userpool_id, dynamodb_table):
     """Export analytics from the accounts to trak engagement and product metrics."""
     session = Session(profile_name=profile)
     db = session.resource('dynamodb', region_name=region)
     cognito = session.client('cognito-idp')
     tables = list(db.tables.all())
-    
+
     print(bcolors.OKCYAN + "------------------------------" + bcolors.ENDC)
     print(bcolors.OKCYAN + f"Info: List of dynamodb tables using AWS profile {profile}" + bcolors.ENDC)
     for idx, table in enumerate(tables):
-        print(bcolors.OKBLUE + f"{idx + 1}. {table.table_name}" + bcolors.ENDC)    
+        print(bcolors.OKBLUE + f"{idx + 1}. {table.table_name}" + bcolors.ENDC)
     print(bcolors.OKCYAN + "------------------------------" + bcolors.ENDC)
-    print(bcolors.OKGREEN + f"You selected to run an anlytics request on the table {dynamodb_table}" + bcolors.ENDC)        
-        
-    print(bcolors.OKGREEN + f"Report generated successfully" + bcolors.ENDC)        
+    print(bcolors.OKGREEN + f"You selected to run an anlytics request on the table {dynamodb_table}" + bcolors.ENDC)
+
+    print(bcolors.OKGREEN + f"Report generated successfully" + bcolors.ENDC)
 
     registry_ids = scan_registeries(db.Table(dynamodb_table))
     print('registry_id,first_name, last_name, email, last_login, date_refered, patients_refered')
-    for registry_id in registry_ids:        
+    for registry_id in registry_ids:
         scan_patients(cognito, userpool_id, db.Table(dynamodb_table), registry_id.split(':')[1])
 
 
-def scan_registeries(db_table):    
+def scan_registeries(db_table):
     response = db_table.scan(
         FilterExpression=Key('partition_key').begins_with('registry:') & Key('sort_key').eq('metadata')
     )
-    return [item['partition_key'] for item in response['Items']]        
+    return [item['partition_key'] for item in response['Items']]
 
 def get_users_in_registry(db_table, registry_id):
     partition_key = f'registry-user:{registry_id}'
     response = db_table.scan(
-        FilterExpression=Key('partition_key').eq(partition_key) 
+        FilterExpression=Key('partition_key').eq(partition_key)
     )
     return response['Items']
 
 def get_user(db_table, user_id):
     partition_key = f'user:{user_id}'
     response = db_table.get_item(
         Key={
@@ -71,27 +71,25 @@
     )
     return response['Item']
 
 def scan_patients(cognito, userpool_id, db_table, registry_id):
     partition_key = f'registry-patient:{registry_id}'
 
     response = db_table.scan(
-        FilterExpression=Key('partition_key').eq(partition_key) 
+        FilterExpression=Key('partition_key').eq(partition_key)
     )
-    users = get_users_in_registry(db_table, registry_id)    
-    
-    
-    
+    users = get_users_in_registry(db_table, registry_id)
+
     user_emails = []
-    for user in users:        
+    for user in users:
         user_object = get_user(db_table, user['user_id'])
-        try:  
+        try:
             user_profile = cognito.admin_get_user(
                 UserPoolId=userpool_id,
-                Username=user_object['email']            
+                Username=user_object['email']
             )
             given_name = user_profile['UserAttributes'][2]['Value']
             family_name = user_profile['UserAttributes'][3]['Value']
         except Exception as e:
             given_name = ''
             family_name = ''
 
@@ -99,28 +97,27 @@
             {
                 'email': user_object['email'],
                 'given_name': given_name,
                 'family_name': family_name,
                 'date_created': datetime.strftime(datetime.fromtimestamp(int(user_object['date_created'])), '%m-%d-%y'),
                 'last_login': datetime.strftime(datetime.fromtimestamp(int(user_object['last_login'])), '%m-%d-%y')
             }
-        )                
+        )
 
     patient_created_stats = {}
     for patient in response['Items']:
-        date_created = datetime.strftime(datetime.fromtimestamp(int(patient['date_created'])), '%m-%d-%y')         
+        date_created = datetime.strftime(datetime.fromtimestamp(int(patient['date_created'])), '%m-%d-%y')
         if date_created in patient_created_stats:
             patient_created_stats[date_created] += 1
         else:
             patient_created_stats[date_created] = 1
 
-    
-    
+
+
     if len(patient_created_stats.items()) == 0:
         for user_email in user_emails:
-                print(f"{registry_id},{user_email['given_name']},{user_email['family_name']},{user_email['email']},{user_email['last_login']},,")        
-        
-    else:        
+                print(f"{registry_id},{user_email['given_name']},{user_email['family_name']},{user_email['email']},{user_email['last_login']},,")
+
+    else:
         for key, value in patient_created_stats.items():
             for user_email in user_emails:
-                print(f"{registry_id},{user_email['given_name']},{user_email['family_name']},{user_email['email']},{user_email['last_login']}, {key}, {value}")        
-        
+                print(f"{registry_id},{user_email['given_name']},{user_email['family_name']},{user_email['email']},{user_email['last_login']}, {key}, {value}")
```

### Comparing `akello-0.0.21/akello/db/models.py` & `akello-0.0.22/akello/db/models.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/db/types.py` & `akello-0.0.22/akello/db/types.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/db/connector/dynamodb.py` & `akello-0.0.22/akello/db/connector/dynamodb.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/db/connector/s3.py` & `akello-0.0.22/akello/db/connector/s3.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/decorators/akello_plan_tier.py` & `akello-0.0.22/akello/decorators/akello_plan_tier.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/decorators/mixin.py` & `akello-0.0.22/akello/decorators/mixin.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/fhir/fhir.schema.json` & `akello-0.0.22/akello/fhir/fhir.schema.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/fhir/hl7/README.md` & `akello-0.0.22/akello/fhir/hl7/README.md`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/fhir/hl7/fhir_v6_models.py` & `akello-0.0.22/akello/fhir/hl7/fhir_v6_models.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/FHIR/phq9_fhir.json` & `akello-0.0.22/akello/screeners/FHIR/phq9_fhir.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/FHIR/phq9_response.json` & `akello-0.0.22/akello/screeners/FHIR/phq9_response.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/R4/gad7.R4.json` & `akello-0.0.22/akello/screeners/R4/gad7.R4.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/R4/phq9.R4.json` & `akello-0.0.22/akello/screeners/R4/phq9.R4.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/measurements/FHIR_weights.template` & `akello-0.0.22/akello/screeners/measurements/FHIR_weights.template`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/measurements/survey_GAD-7.yaml` & `akello-0.0.22/akello/screeners/measurements/survey_GAD-7.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/measurements/survey_HEADS-ED.yaml` & `akello-0.0.22/akello/screeners/measurements/survey_HEADS-ED.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/measurements/survey_PHQ-9.yaml` & `akello-0.0.22/akello/screeners/measurements/survey_PHQ-9.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/measurements/survey_PMQ.yaml` & `akello-0.0.22/akello/screeners/measurements/survey_PMQ.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/questionnaires/gad7.json` & `akello-0.0.22/akello/screeners/questionnaires/gad7.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/screeners/questionnaires/phq9.json` & `akello-0.0.22/akello/screeners/questionnaires/phq9.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/services/akello_apps.py` & `akello-0.0.22/akello/services/akello_apps.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/services/registry.py` & `akello-0.0.22/akello/services/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/services/reports.py` & `akello-0.0.22/akello/services/reports.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/services/screeners.py` & `akello-0.0.22/akello/services/screeners.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/services/stripe_payment.py` & `akello-0.0.22/akello/services/stripe_payment.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/services/user.py` & `akello-0.0.22/akello/services/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,24 @@
 
         Returns:
             List[Dict]: A list of items representing the user's profile.
 
         Raises:
             ClientError: If the query to the database fails.
         """
-        try:            
+        try:
             response = registry_db.query(
                 KeyConditionExpression=Key('partition_key').eq('user:%s' % cognito_user_id)
                                        & Key('sort_key').eq('profile')
             )
             return response['Items']
         except ClientError as e:
             print(e)
-            print(e.response['No item found'])        
-                
+            print(e.response['No item found'])
+
 
     @staticmethod
     def get_user_sessions(cognito_user_id):
         """
         Retrieves the sessions of a user sorted in reverse chronological order.
 
         Parameters:
@@ -52,18 +52,18 @@
 
         Returns:
             List[Dict]: A list of items representing the user's sessions.
 
         Raises:
             ClientError: If the query to the database fails.
         """
-        try:                        
+        try:
             response = registry_db.query(
-                KeyConditionExpression=Key('partition_key').eq('user-session:%s' % cognito_user_id), 
-                ScanIndexForward=False                                       
+                KeyConditionExpression=Key('partition_key').eq('user-session:%s' % cognito_user_id),
+                ScanIndexForward=False
             )
             return response['Items']
         except ClientError as e:
             print(e)
             print(e.response['No item found'])
 
     @staticmethod
@@ -75,27 +75,27 @@
             cognito_user_id (str): The Cognito user ID of the user.
             user_agent (str): The user agent string of the user's device.
             ip_address (str): The IP address of the user's device.
 
         Raises:
             ClientError: If saving the session to the database fails.
         """
-        try:            
+        try:
             response = registry_db.put_item(
                 Item={
                     "partition_key": 'user-session:%s' % cognito_user_id,
                     "sort_key": str(Decimal(datetime.datetime.utcnow().timestamp())),
                     "user_agent": user_agent,
                     "ip_address": ip_address
                 }
             )
-            status_code = response['ResponseMetadata']['HTTPStatusCode']            
+            status_code = response['ResponseMetadata']['HTTPStatusCode']
             assert status_code == 200
-        except ClientError as e:            
-            print(e)        
+        except ClientError as e:
+            print(e)
 
 
     @staticmethod
     def update_profile_photo(cognito_user_id, photo_url):
         """
         Updates the profile photo URL of a user.
 
@@ -138,33 +138,31 @@
                 "date_created": Decimal(datetime.datetime.utcnow().timestamp()),
                 "last_login": Decimal(datetime.datetime.utcnow().timestamp()),
             }
         )
         status_code = response['ResponseMetadata']['HTTPStatusCode']
         assert status_code == 200
 
-        sg = SendGridAPIClient(os.environ.get('SENDGRID_API_KEY'))
-        data = {
-            "contacts": [
-                {
-                    "email": email,
-                    "first_name": first_name,
-                    "last_name": last_name,
-                    "custom_fields": {                        
+        sg_api_key = os.environ.get('SENDGRID_API_KEY')
+        if sg_api_key:
+            sg = SendGridAPIClient(os.environ.get('SENDGRID_API_KEY'))
+            data = {
+                "contacts": [
+                    {
+                        "email": email,
+                        "first_name": first_name,
+                        "last_name": last_name,
+                        "custom_fields": {
+                        }
                     }
-                }
-            ]
-        }
-        response = sg.client.marketing.contacts.put(
-            request_body=data
-        )
-
-
-
-
+                ]
+            }
+            response = sg.client.marketing.contacts.put(
+                request_body=data
+            )
 
     @staticmethod
     def create_registry_user(registry_id, first_name, last_name, email, user_id, role: UserRole, is_admin: bool):
         """
         Creates a new registry user association in the database.
 
         Parameters:
```

### Comparing `akello-0.0.21/akello/services/tests/__init__.py` & `akello-0.0.22/akello/services/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/services/tests/test_registry_service.py` & `akello-0.0.22/akello/services/tests/test_registry_service.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/akello/services/tests/test_user_service.py` & `akello-0.0.22/akello/services/tests/test_user_service.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/commands/mock_registry.py` & `akello-0.0.22/commands/mock_registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/commands/mock/patient.py` & `akello-0.0.22/commands/mock/patient.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/commands/mock/registry.py` & `akello-0.0.22/commands/mock/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/commands/mock/treatment_log.py` & `akello-0.0.22/commands/mock/treatment_log.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/Makefile` & `akello-0.0.22/docs/Makefile`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/akello.auth.aws_cognito.rst` & `akello-0.0.22/docs/akello.auth.aws_cognito.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/akello.db.connector.rst` & `akello-0.0.22/docs/akello.db.connector.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/akello.db.rst` & `akello-0.0.22/docs/akello.db.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/akello.rst` & `akello-0.0.22/docs/akello.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/akello.services.rst` & `akello-0.0.22/docs/akello.services.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/akello.services.tests.rst` & `akello-0.0.22/docs/akello.services.tests.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/conf.py` & `akello-0.0.22/docs/conf.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/index.rst` & `akello-0.0.22/docs/index.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/docs/make.bat` & `akello-0.0.22/docs/make.bat`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/synthetic_data/load_fhir_data.py` & `akello-0.0.22/synthetic_data/load_fhir_data.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json` & `akello-0.0.22/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/.gitignore` & `akello-0.0.22/.gitignore`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/LICENSE` & `akello-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `akello-0.0.21/pyproject.toml` & `akello-0.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "akello"
-version = "0.0.21"
+version = "0.0.22"
 authors = [
   { name="Vijay Selvaraj", email="vijay@akellohealth.com" },
 ]
 description = "FastAPI server akello.io"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `akello-0.0.21/PKG-INFO` & `akello-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: akello
-Version: 0.0.21
+Version: 0.0.22
 Summary: FastAPI server akello.io
 Project-URL: Homepage, https://akello.io
 Project-URL: Issues, https://github.com/akello-io/akello/issues
 Author-email: Vijay Selvaraj <vijay@akellohealth.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

