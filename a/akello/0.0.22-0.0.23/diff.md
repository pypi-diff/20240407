# Comparing `tmp/akello-0.0.22.tar.gz` & `tmp/akello-0.0.23.tar.gz`

## Comparing `akello-0.0.22.tar` & `akello-0.0.23.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 akello-0.0.22/.dockerignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 akello-0.0.22/Dockerfile
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 akello-0.0.22/Dockerfile.aws.lambda
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/__init__.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 akello-0.0.22/management.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/module_name.md
--rw-r--r--   0        0        0    24160 2020-02-02 00:00:00.000000 akello-0.0.22/openapi.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 akello-0.0.22/openapi.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 akello-0.0.22/publish_test_pypi.sh
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 akello-0.0.22/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/.gitignore
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/api-server.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/modules.xml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/vcs.xml
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/workspace.xml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 akello-0.0.22/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 akello-0.0.22/akello/app_configs.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 akello-0.0.22/akello/main.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 akello-0.0.22/akello/secrets.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 akello-0.0.22/akello/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/endpoints/__init__.py
--rw-r--r--   0        0        0    21517 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/endpoints/registry.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/endpoints/reports.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 akello-0.0.22/akello/api/app/v1/endpoints/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/provider.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/aws_cognito/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/aws_cognito/__init__.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/aws_cognito/auth_settings.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 akello-0.0.22/akello/auth/aws_cognito/aws_cognito.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.template.api.env
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.template.env
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/akello.py
--rwxr-xr-x   0        0        0      510 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/dev-build-single.sh
--rwxr-xr-x   0        0        0     2581 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/dev-setup-local.sh
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/docker-compose.yml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.cognito/config.json
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.cognito/db/clients.json
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/.cognito/db/local_4yfGDg3h.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/__init__.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/analytics.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/build.py
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/setup.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 akello-0.0.22/akello/cli/commands/start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/__init__.py
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/models.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/connector/__init__.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/connector/dynamodb.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 akello-0.0.22/akello/db/connector/s3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/decorators/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 akello-0.0.22/akello/decorators/akello_plan_tier.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 akello-0.0.22/akello/decorators/mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/__init__.py
--rw-r--r--   0        0        0  4322416 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/fhir.schema.json
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/hl7/README.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/hl7/__init__.py
--rw-r--r--   0        0        0   648807 2020-02-02 00:00:00.000000 akello-0.0.22/akello/fhir/hl7/fhir_v6_models.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/__init__.py
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/FHIR/phq9_fhir.json
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/FHIR/phq9_response.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/R4/__init__.py
--rw-r--r--   0        0        0    22471 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/R4/gad7.R4.json
--rw-r--r--   0        0        0    32684 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/R4/phq9.R4.json
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/FHIR_weights.template
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/api_weights.template
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/survey_GAD-7.yaml
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/survey_HEADS-ED.yaml
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/survey_PHQ-9.yaml
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/measurements/survey_PMQ.yaml
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/questionnaires/gad7.json
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 akello-0.0.22/akello/screeners/questionnaires/phq9.json
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/__init__.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/akello_apps.py
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/registry.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/reports.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/screeners.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/stripe_payment.py
--rw-r--r--   0        0        0    10559 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/user.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_decorators.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_registry_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_reports_service.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_screeners_service.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 akello-0.0.22/akello/services/tests/test_user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/akello/utils/email.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 akello-0.0.22/commands/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/commands/__init__.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/__init__.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/patient.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/registry.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/treatment_log.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 akello-0.0.22/commands/mock/user.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 akello-0.0.22/docs/Makefile
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.api.fhir.rst
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.api.fhir.v1.endpoints.rst
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.api.fhir.v1.rst
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.api.rst
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.auth.aws_cognito.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.auth.rst
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.db.connector.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.db.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.decorators.rst
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.fhir.hl7.rst
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.fhir.rst
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.rst
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.screeners.R4.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.screeners.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.services.rst
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.services.tests.rst
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 akello-0.0.22/docs/akello.utils.rst
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 akello-0.0.22/docs/conf.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 akello-0.0.22/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 akello-0.0.22/docs/make.bat
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 akello-0.0.22/docs/modules.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/README.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/generate_data.sh
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/load_fhir_data.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 akello-0.0.22/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 akello-0.0.22/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 akello-0.0.22/LICENSE
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 akello-0.0.22/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 akello-0.0.22/pyproject.toml
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 akello-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 akello-0.0.23/.dockerignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 akello-0.0.23/Dockerfile
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 akello-0.0.23/Dockerfile.aws.lambda
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/__init__.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 akello-0.0.23/management.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/module_name.md
+-rw-r--r--   0        0        0    24160 2020-02-02 00:00:00.000000 akello-0.0.23/openapi.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 akello-0.0.23/openapi.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 akello-0.0.23/publish_test_pypi.sh
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 akello-0.0.23/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 akello-0.0.23/.idea/.gitignore
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 akello-0.0.23/.idea/api-server.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 akello-0.0.23/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 akello-0.0.23/.idea/modules.xml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 akello-0.0.23/.idea/vcs.xml
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 akello-0.0.23/.idea/workspace.xml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 akello-0.0.23/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 akello-0.0.23/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 akello-0.0.23/akello/app_configs.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 akello-0.0.23/akello/main.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 akello-0.0.23/akello/secrets.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 akello-0.0.23/akello/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/api/app/v1/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 akello-0.0.23/akello/api/app/v1/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/api/app/v1/endpoints/__init__.py
+-rw-r--r--   0        0        0    21517 2020-02-02 00:00:00.000000 akello-0.0.23/akello/api/app/v1/endpoints/registry.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 akello-0.0.23/akello/api/app/v1/endpoints/reports.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 akello-0.0.23/akello/api/app/v1/endpoints/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/auth/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 akello-0.0.23/akello/auth/provider.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 akello-0.0.23/akello/auth/aws_cognito/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/auth/aws_cognito/__init__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 akello-0.0.23/akello/auth/aws_cognito/auth_settings.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 akello-0.0.23/akello/auth/aws_cognito/aws_cognito.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/.template.api.env
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/.template.env
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/akello.py
+-rwxr-xr-x   0        0        0      510 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/dev-build-single.sh
+-rwxr-xr-x   0        0        0     2581 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/dev-setup-local.sh
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/docker-compose.yml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/.cognito/config.json
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/.cognito/db/clients.json
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/.cognito/db/local_4yfGDg3h.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/commands/analytics.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/commands/build.py
+-rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/commands/setup.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 akello-0.0.23/akello/cli/commands/start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/db/__init__.py
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 akello-0.0.23/akello/db/models.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 akello-0.0.23/akello/db/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/db/connector/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 akello-0.0.23/akello/db/connector/dynamodb.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 akello-0.0.23/akello/db/connector/s3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/decorators/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 akello-0.0.23/akello/decorators/akello_plan_tier.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 akello-0.0.23/akello/decorators/mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/fhir/__init__.py
+-rw-r--r--   0        0        0  4322416 2020-02-02 00:00:00.000000 akello-0.0.23/akello/fhir/fhir.schema.json
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 akello-0.0.23/akello/fhir/hl7/README.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 akello-0.0.23/akello/fhir/hl7/__init__.py
+-rw-r--r--   0        0        0   648807 2020-02-02 00:00:00.000000 akello-0.0.23/akello/fhir/hl7/fhir_v6_models.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/__init__.py
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/FHIR/phq9_fhir.json
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/FHIR/phq9_response.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/R4/__init__.py
+-rw-r--r--   0        0        0    22471 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/R4/gad7.R4.json
+-rw-r--r--   0        0        0    32684 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/R4/phq9.R4.json
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/measurements/FHIR_weights.template
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/measurements/api_weights.template
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/measurements/survey_GAD-7.yaml
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/measurements/survey_HEADS-ED.yaml
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/measurements/survey_PHQ-9.yaml
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/measurements/survey_PMQ.yaml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/questionnaires/gad7.json
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 akello-0.0.23/akello/screeners/questionnaires/phq9.json
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/__init__.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/akello_apps.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/registry.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/reports.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/screeners.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/stripe_payment.py
+-rw-r--r--   0        0        0    10559 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/user.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/tests/test_decorators.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/tests/test_registry_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/tests/test_reports_service.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/tests/test_screeners_service.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 akello-0.0.23/akello/services/tests/test_user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/akello/utils/email.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 akello-0.0.23/commands/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/commands/__init__.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 akello-0.0.23/commands/mock_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akello-0.0.23/commands/mock/__init__.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 akello-0.0.23/commands/mock/patient.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 akello-0.0.23/commands/mock/registry.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 akello-0.0.23/commands/mock/treatment_log.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 akello-0.0.23/commands/mock/user.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 akello-0.0.23/docs/Makefile
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.api.fhir.rst
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.api.fhir.v1.endpoints.rst
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.api.fhir.v1.rst
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.api.rst
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.auth.aws_cognito.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.auth.rst
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.db.connector.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.db.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.decorators.rst
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.fhir.hl7.rst
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.fhir.rst
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.screeners.R4.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.screeners.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.services.rst
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.services.tests.rst
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 akello-0.0.23/docs/akello.utils.rst
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 akello-0.0.23/docs/conf.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 akello-0.0.23/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 akello-0.0.23/docs/make.bat
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 akello-0.0.23/docs/modules.rst
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 akello-0.0.23/synthetic_data/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 akello-0.0.23/synthetic_data/README.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 akello-0.0.23/synthetic_data/generate_data.sh
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 akello-0.0.23/synthetic_data/load_fhir_data.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 akello-0.0.23/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 akello-0.0.23/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 akello-0.0.23/LICENSE
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 akello-0.0.23/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 akello-0.0.23/pyproject.toml
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 akello-0.0.23/PKG-INFO
```

### Comparing `akello-0.0.22/.dockerignore` & `akello-0.0.23/.dockerignore`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/management.py` & `akello-0.0.23/management.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/openapi.json` & `akello-0.0.23/openapi.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/requirements.txt` & `akello-0.0.23/requirements.txt`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/.idea/api-server.iml` & `akello-0.0.23/.idea/api-server.iml`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/.idea/workspace.xml` & `akello-0.0.23/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/app_configs.yaml` & `akello-0.0.23/akello/app_configs.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/main.py` & `akello-0.0.23/akello/main.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/secrets.py` & `akello-0.0.23/akello/secrets.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/api/app/v1/endpoints/registry.py` & `akello-0.0.23/akello/api/app/v1/endpoints/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/api/app/v1/endpoints/reports.py` & `akello-0.0.23/akello/api/app/v1/endpoints/reports.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/api/app/v1/endpoints/user.py` & `akello-0.0.23/akello/api/app/v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/auth/aws_cognito/README.md` & `akello-0.0.23/akello/auth/aws_cognito/README.md`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/auth/aws_cognito/auth_settings.py` & `akello-0.0.23/akello/auth/aws_cognito/auth_settings.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/auth/aws_cognito/aws_cognito.py` & `akello-0.0.23/akello/auth/aws_cognito/aws_cognito.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/cli/akello.py` & `akello-0.0.23/akello/cli/akello.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/cli/dev-setup-local.sh` & `akello-0.0.23/akello/cli/dev-setup-local.sh`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/cli/.cognito/db/local_4yfGDg3h.json` & `akello-0.0.23/akello/cli/.cognito/db/local_4yfGDg3h.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/cli/commands/analytics.py` & `akello-0.0.23/akello/cli/commands/analytics.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/cli/commands/setup.py` & `akello-0.0.23/akello/cli/commands/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import click
 import os, json
 import pathlib
 import subprocess
+import webbrowser
+
 
 current_file_path = pathlib.Path(__file__).parent.resolve()
 
 class bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
@@ -52,19 +54,19 @@
         return True
     except:
         print("Docker is not running")
         return False
 
 def is_aws_cli_installed():
     try:
-        subprocess.check_output('aws', shell=True)
+        subprocess.check_output('aws help', shell=True)
         return True
     except:
         print("AWS cli is not installed")
-        return False
+
 
 def run_setup():
     if not is_docker_running():
         print(bcolors.FAIL + "Error: Docker isn't installed or running?" + bcolors.ENDC)
         raise Exception("Docker is not running")
 
     if not is_aws_cli_installed():
@@ -101,14 +103,15 @@
     os.environ["AWS_COGNITO_APP_CLIENT_ID"] = client_id
     os.environ["AWS_DYNAMODB_TABLE"] = "akello-local"
     os.environ["AWS_REGION"] = "us-east-1"
     os.environ["AKELLO_API_URL"] = "http://127.0.0.1:8000/v1"
     os.environ["AKELLO_COGNITO_URL"] = "http://localhost:9229"
     os.environ["AKELLO_DYNAMODB_LOCAL_URL"] = "http://localhost:8001"
 
+
     akello_ascii = """
                               ██████                                      ████        ████
                         ████████                                 █████████  ██████████
                            █████                                    ██████      ██████
                            █████                                     █████      ██████
                            █████                                     █████      ██████
                            █████                                     █████      ██████
@@ -123,28 +126,32 @@
 ██████          █████     ██████    ███████   ███████                █████      ██████   ██████           ██████
 ███████         █████   ████████      ███████  ███████          ██   █████      ██████    ██████         ██████
  █████████   ███████████████████       ████████ ██████████████████   ██████     ██████     ███████     ███████
    ████████████ ████████   ███████       ███████  ██████████████  ███████████████████████    ███████████████
       █████     █████                                 ██████                                     ███████
     """
 
+
     print(akello_ascii)
     print("\n\n")
     print("Add the following to your .env file")
     print("-----------------------------------")
     print(f"export AWS_COGNITO_USERPOOL_ID={user_pool_id}")
     print(f"export AWS_COGNITO_APP_CLIENT_ID={client_id}")
     print(f"export AWS_DYNAMODB_TABLE='akello-local'")
     print(f"export AWS_REGION=us-east-1")
     print(f"export AKELLO_API_URL=http://127.0.0.1:8000/v1")
     print(f"export AKELLO_COGNITO_URL=http://localhost:9229")
     print(f"export AKELLO_DYNAMODB_LOCAL_URL=http://localhost:8001")
     print(f"export STRIPE_API_KEY=xxxx set it manually for now xxxxx")
     print("\n\n")
 
+    print(bcolors.OKBLUE + "API Server is now starting on http://localhost:8000" + bcolors.ENDC)
+
+
 @click.command()
 def setup():
     # packages_path = os.path.join(current_file_path, '../../../')
     # os.system(f"cd {current_file_path}/.. && ls {packages_path}/server/akello/ -all && cp .template.api.env {packages_path}/server/akello/.env")
     run_setup()
 
 @click.command()
```

### Comparing `akello-0.0.22/akello/db/models.py` & `akello-0.0.23/akello/db/models.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/db/types.py` & `akello-0.0.23/akello/db/types.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/db/connector/dynamodb.py` & `akello-0.0.23/akello/db/connector/dynamodb.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/db/connector/s3.py` & `akello-0.0.23/akello/db/connector/s3.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/decorators/akello_plan_tier.py` & `akello-0.0.23/akello/decorators/akello_plan_tier.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/decorators/mixin.py` & `akello-0.0.23/akello/decorators/mixin.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/fhir/fhir.schema.json` & `akello-0.0.23/akello/fhir/fhir.schema.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/fhir/hl7/README.md` & `akello-0.0.23/akello/fhir/hl7/README.md`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/fhir/hl7/fhir_v6_models.py` & `akello-0.0.23/akello/fhir/hl7/fhir_v6_models.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/FHIR/phq9_fhir.json` & `akello-0.0.23/akello/screeners/FHIR/phq9_fhir.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/FHIR/phq9_response.json` & `akello-0.0.23/akello/screeners/FHIR/phq9_response.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/R4/gad7.R4.json` & `akello-0.0.23/akello/screeners/R4/gad7.R4.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/R4/phq9.R4.json` & `akello-0.0.23/akello/screeners/R4/phq9.R4.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/measurements/FHIR_weights.template` & `akello-0.0.23/akello/screeners/measurements/FHIR_weights.template`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/measurements/survey_GAD-7.yaml` & `akello-0.0.23/akello/screeners/measurements/survey_GAD-7.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/measurements/survey_HEADS-ED.yaml` & `akello-0.0.23/akello/screeners/measurements/survey_HEADS-ED.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/measurements/survey_PHQ-9.yaml` & `akello-0.0.23/akello/screeners/measurements/survey_PHQ-9.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/measurements/survey_PMQ.yaml` & `akello-0.0.23/akello/screeners/measurements/survey_PMQ.yaml`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/questionnaires/gad7.json` & `akello-0.0.23/akello/screeners/questionnaires/gad7.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/screeners/questionnaires/phq9.json` & `akello-0.0.23/akello/screeners/questionnaires/phq9.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/akello_apps.py` & `akello-0.0.23/akello/services/akello_apps.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/registry.py` & `akello-0.0.23/akello/services/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/reports.py` & `akello-0.0.23/akello/services/reports.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/screeners.py` & `akello-0.0.23/akello/services/screeners.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/stripe_payment.py` & `akello-0.0.23/akello/services/stripe_payment.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/user.py` & `akello-0.0.23/akello/services/user.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/tests/__init__.py` & `akello-0.0.23/akello/services/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/tests/test_registry_service.py` & `akello-0.0.23/akello/services/tests/test_registry_service.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/akello/services/tests/test_user_service.py` & `akello-0.0.23/akello/services/tests/test_user_service.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/commands/mock_registry.py` & `akello-0.0.23/commands/mock_registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/commands/mock/patient.py` & `akello-0.0.23/commands/mock/patient.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/commands/mock/registry.py` & `akello-0.0.23/commands/mock/registry.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/commands/mock/treatment_log.py` & `akello-0.0.23/commands/mock/treatment_log.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/Makefile` & `akello-0.0.23/docs/Makefile`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/akello.auth.aws_cognito.rst` & `akello-0.0.23/docs/akello.auth.aws_cognito.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/akello.db.connector.rst` & `akello-0.0.23/docs/akello.db.connector.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/akello.db.rst` & `akello-0.0.23/docs/akello.db.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/akello.rst` & `akello-0.0.23/docs/akello.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/akello.services.rst` & `akello-0.0.23/docs/akello.services.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/akello.services.tests.rst` & `akello-0.0.23/docs/akello.services.tests.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/conf.py` & `akello-0.0.23/docs/conf.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/index.rst` & `akello-0.0.23/docs/index.rst`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/docs/make.bat` & `akello-0.0.23/docs/make.bat`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/synthetic_data/load_fhir_data.py` & `akello-0.0.23/synthetic_data/load_fhir_data.py`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json` & `akello-0.0.23/synthetic_data/metadata/2024_03_05T00_53_07Z_100_Massachusetts_fbb6949c_02b6_442d_9a57_8c7f7e1d6272.json`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/.gitignore` & `akello-0.0.23/.gitignore`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/LICENSE` & `akello-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `akello-0.0.22/pyproject.toml` & `akello-0.0.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "akello"
-version = "0.0.22"
+version = "0.0.23"
 authors = [
   { name="Vijay Selvaraj", email="vijay@akellohealth.com" },
 ]
 description = "FastAPI server akello.io"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `akello-0.0.22/PKG-INFO` & `akello-0.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: akello
-Version: 0.0.22
+Version: 0.0.23
 Summary: FastAPI server akello.io
 Project-URL: Homepage, https://akello.io
 Project-URL: Issues, https://github.com/akello-io/akello/issues
 Author-email: Vijay Selvaraj <vijay@akellohealth.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

