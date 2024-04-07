# Comparing `tmp/ado_wrapper-0.0.3.tar.gz` & `tmp/ado_wrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-0.0.3.tar", max compression
+gzip compressed data, was "ado_wrapper-0.0.4.tar", max compression
```

## Comparing `ado_wrapper-0.0.3.tar` & `ado_wrapper-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.3/LICENSE
--rw-r--r--   0        0        0      516 2024-04-05 11:51:02.152589 ado_wrapper-0.0.3/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.3/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6471 2024-04-05 14:34:46.569797 ado_wrapper-0.0.3/ado_wrapper/__main__.py
--rw-r--r--   0        0        0      757 2024-03-18 13:18:23.074326 ado_wrapper-0.0.3/ado_wrapper/attribute_types.py
--rw-r--r--   0        0        0     1789 2024-04-05 11:26:50.366793 ado_wrapper-0.0.3/ado_wrapper/client.py
--rw-r--r--   0        0        0    16521 2024-04-05 11:26:35.608888 ado_wrapper-0.0.3/ado_wrapper/dumps.py
--rw-r--r--   0        0        0      933 2024-04-05 11:26:35.608861 ado_wrapper-0.0.3/ado_wrapper/generate_type_hints.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.3/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.3/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     2999 2024-04-05 15:06:59.436804 ado_wrapper-0.0.3/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1173 2024-04-05 15:06:51.254984 ado_wrapper-0.0.3/ado_wrapper/plan_resources/singletons.py
--rw-r--r--   0        0        0      592 2024-04-05 11:26:35.608910 ado_wrapper-0.0.3/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4647 2024-04-05 11:26:35.611010 ado_wrapper-0.0.3/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14311 2024-04-05 15:08:13.711235 ado_wrapper-0.0.3/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6680 2024-04-05 11:26:35.611906 ado_wrapper-0.0.3/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3582 2024-04-05 11:26:35.622227 ado_wrapper-0.0.3/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0     2226 2024-04-05 11:26:35.611094 ado_wrapper-0.0.3/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    10175 2024-04-05 11:26:35.611081 ado_wrapper-0.0.3/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12933 2024-04-05 11:26:35.608871 ado_wrapper-0.0.3/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0     9370 2024-04-05 15:06:28.103613 ado_wrapper-0.0.3/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5133 2024-04-05 14:34:26.887910 ado_wrapper-0.0.3/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8223 2024-04-05 11:26:35.611032 ado_wrapper-0.0.3/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     5384 2024-04-05 11:26:35.622212 ado_wrapper-0.0.3/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     6204 2024-04-05 14:46:36.791614 ado_wrapper-0.0.3/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8239 2024-04-05 14:54:03.323466 ado_wrapper-0.0.3/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     3919 2024-04-05 11:26:35.608850 ado_wrapper-0.0.3/ado_wrapper/utils.py
--rw-r--r--   0        0        0     1997 2024-04-05 15:08:55.949910 ado_wrapper-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 ado_wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.4/LICENSE
+-rw-r--r--   0        0        0      516 2024-04-05 11:51:02.152589 ado_wrapper-0.0.4/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.4/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6432 2024-04-06 09:40:50.980917 ado_wrapper-0.0.4/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     1878 2024-04-07 10:54:07.604713 ado_wrapper-0.0.4/ado_wrapper/client.py
+-rw-r--r--   0        0        0    17154 2024-04-07 10:01:31.474982 ado_wrapper-0.0.4/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.4/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.4/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     2999 2024-04-05 15:06:59.436804 ado_wrapper-0.0.4/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1173 2024-04-05 15:06:51.254984 ado_wrapper-0.0.4/ado_wrapper/plan_resources/singletons.py
+-rw-r--r--   0        0        0      659 2024-04-07 11:10:47.369677 ado_wrapper-0.0.4/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     4568 2024-04-07 12:20:36.607817 ado_wrapper-0.0.4/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    13854 2024-04-07 12:25:08.207236 ado_wrapper-0.0.4/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6586 2024-04-07 12:41:44.539525 ado_wrapper-0.0.4/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3622 2024-04-07 10:59:40.805971 ado_wrapper-0.0.4/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0     2087 2024-04-07 12:49:21.264048 ado_wrapper-0.0.4/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14999 2024-04-07 12:28:52.324575 ado_wrapper-0.0.4/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    13064 2024-04-07 11:01:07.349289 ado_wrapper-0.0.4/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0     9139 2024-04-07 12:30:48.891543 ado_wrapper-0.0.4/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5084 2024-04-07 12:49:15.437789 ado_wrapper-0.0.4/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4762 2024-04-07 12:49:33.320370 ado_wrapper-0.0.4/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8229 2024-04-07 12:50:04.637373 ado_wrapper-0.0.4/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     5117 2024-04-07 12:32:55.829004 ado_wrapper-0.0.4/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     7045 2024-04-07 12:41:33.897870 ado_wrapper-0.0.4/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8104 2024-04-06 09:40:50.988258 ado_wrapper-0.0.4/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4230 2024-04-07 10:39:34.190691 ado_wrapper-0.0.4/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     1997 2024-04-06 09:49:20.016252 ado_wrapper-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 ado_wrapper-0.0.4/PKG-INFO
```

### Comparing `ado_wrapper-0.0.3/LICENSE` & `ado_wrapper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.3/README.md` & `ado_wrapper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.3/ado_wrapper/__main__.py` & `ado_wrapper-0.0.4/ado_wrapper/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 
-from ado_wrapper.attribute_types import ResourceType
 from ado_wrapper.client import AdoClient
-from ado_wrapper.utils import get_internal_field_names, get_resource_variables
+from ado_wrapper.utils import get_internal_field_names, get_resource_variables, ResourceType
 
 
 def main() -> None:
     ALL_RESOURCES = get_resource_variables()
 
     parser = argparse.ArgumentParser(
         prog="AdoWrapper", description="A tool to manage Azure DevOps resources and interface with the ADO API", usage=""
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/client.py` & `ado_wrapper-0.0.4/ado_wrapper/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 from requests.auth import HTTPBasicAuth
 
 from ado_wrapper.state_manager import StateManager
+from ado_wrapper.utils import AuthenticationError
 
 
 class AdoClient:
     def __init__(  # pylint: disable=too-many-arguments
         self, ado_email: str, ado_pat: str, ado_org: str, ado_project: str,
         state_file_name: str | None = "main.state", bypass_initialisation: bool = False # fmt: skip
     ) -> None:
@@ -16,16 +17,17 @@
         self.auth = HTTPBasicAuth(ado_email, ado_pat)
         self.ado_org = ado_org
         self.ado_project = ado_project
         self.plan = False
 
         if not bypass_initialisation:
             # Verify Token is working (helps with setup for first time users):
-            request = requests.get(f"https://dev.azure.com/{self.ado_org}/_apis/projects?api-version=6.0", auth=self.auth)
-            assert request.status_code == 200, f"Failed to authenticate with ADO: {request.text}"
+            request = requests.get(f"https://dev.azure.com/{self.ado_org}/_apis/projects?api-version=7.1", auth=self.auth)
+            if request.status_code != 200:
+                raise AuthenticationError(f"Failed to authenticate with ADO: {request.text}")
 
             from ado_wrapper.resources.projects import Project  # Stop circular import
             self.ado_project_id = Project.get_by_name(self, self.ado_project).project_id  # type: ignore[union-attr]
 
             from ado_wrapper.resources.users import AdoUser  # Stop circular import
             try:
                 self.pat_author: AdoUser = AdoUser.get_by_email(self, ado_email)
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/dumps.py` & `ado_wrapper-0.0.4/ado_wrapper/dumps.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     'id': '<32_char_uuid>',
     'name': '<project_name>',
     'description': '<description>',
     'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/<project_id>',
     'state': 'wellFormed',
     'revision': 194,
     'visibility': 'private',
-    'lastUpdateTime': '2024-03-18T16:41:25.14Z',
+    'lastUpdateTime': '2024-03-18T16:41:05.14Z',
 }
 
 PULL_REQUEST_DUMP = {
     'repository ': {'id': '<repo_id>', 'name': 'ado_wrapper-test-repo-for-get-pull-request-by-id', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>', 'project': {'id': '<project_id>', 'name': '<project_name>', 'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}', 'state': 'wellFormed', 'revision': 399, 'visibility': 'private', 'lastUpdateTime': '2024-02-06T14:14:30.36Z'}, 'size': 980, 'remoteUrl': 'https://{ado_client.org}@dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-get-pull-request-by-id', 'sshUrl': 'git@ssh.dev.azure.com:v3/{ado_client.org}/{ado_client.project}/ado_wrapper-test-repo-for-get-pull-request-by-id', 'webUrl': 'https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-get-pull-request-by-id', 'isDisabled': False, 'isInMaintenance': False},
     'pullRequestId': "{pull_request_id}",
     'codeReviewId': "{code_review_id}",
     'status': 'active',
@@ -148,14 +148,30 @@
     'remoteUrl': 'https://{ado_client.org}@dev.azure.com/{ado_client.org}/{ado_client.project}/_git/{repo_name}',
     'sshUrl': 'git@ssh.dev.azure.com:v3/{ado_client.org}/{ado_client.project}/{repo_name}',
     'webUrl': 'https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/{repo_name}',
     'isDisabled': False,
     'isInMaintenance': False,
 }
 
+SERVICE_ENDPOINT_DUMP = {
+    'data': {},
+    'id': '{service_endpoint_id}',
+    'name': '{service_connection_name}',
+    'type': 'github',
+    'url': 'https://github.com',
+    'createdBy': "<Member>",
+    'description': '{description}',
+    'authorization': {'parameters': {'AccessToken': None}, 'scheme': 'Token'},
+    'isShared': False,
+    'isOutdated': False, 'isReady': True,
+    'owner': 'Library',
+    'serviceEndpointProjectReferences': [{'projectReference': {'id': '{project_id}', 'name': '{project_name}'},
+                                          'name': '{service_connection_name}', 'description': '{description}'}]
+}
+
 TEAM_DUMP = {
     'id': '<32_char_uuid>',
     'name': 'Systems Team',
     'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}/teams/<32_char_uuid>',
     'description': '<description>',
     'identityUrl': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<32_char_uuid>',
     'projectName': '<project_name',
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-0.0.4/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.3/ado_wrapper/plan_resources/singletons.py` & `ado_wrapper-0.0.4/ado_wrapper/plan_resources/singletons.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/__init__.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,7 +4,8 @@
 from ado_wrapper.resources.projects import Project
 from ado_wrapper.resources.pull_requests import PullRequest
 from ado_wrapper.resources.releases import Release, ReleaseDefinition
 from ado_wrapper.resources.repo import Repo, BuildRepository
 from ado_wrapper.resources.teams import Team
 from ado_wrapper.resources.users import AdoUser, TeamMember, Member, Reviewer
 from ado_wrapper.resources.variable_groups import VariableGroup
+from ado_wrapper.resources.service_endpoint import ServiceEndpoint
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/branches.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/branches.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field
+from typing import Literal
 
 from ado_wrapper.client import AdoClient
 from ado_wrapper.state_managed_abc import StateManagedResource
 
-# from editable_attribute_types import BranchEditableAttribute
-
+BranchEditableAttribute = Literal["name"]
 
 @dataclass
 class Branch(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/refs?view=azure-devops-rest-7.1
     This isn't entirely what I wanted, you can't branch without a commit, so I need to add a commit method to this class
     And overall, just use commits if you can.
     """
@@ -41,27 +41,27 @@
         # Commit.create(ado_client, repo_id, source_branch, branch_name, {}, "add", "Abc")
         # return cls.get_by_name(ado_client, repo_id, branch_name)
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, repo_id: str, branch_id: str) -> None:
         return super().delete_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/refs/{branch_id}?api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/refs/{branch_id}?api-version=7.1",
             branch_id,
         )
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_all_by_repo(cls, ado_client: AdoClient, repo_id: str) -> list["Branch"]:
         return super().get_all(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/refs?filter=heads&api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/refs?filter=heads&api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "Branch":
         for branch in cls.get_all_by_repo(ado_client, repo_id):
             if branch.name == branch_name:
                 return branch
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/builds.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/builds.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import requests
 
 from ado_wrapper.client import AdoClient
 from ado_wrapper.utils import from_ado_date_string
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
 from ado_wrapper.resources.repo import BuildRepository
-from ado_wrapper.attribute_types import BuildDefinitionEditableAttribute
 
+BuildDefinitionEditableAttribute = Literal["name", "description"]
 BuildStatus = Literal["notStarted", "inProgress", "completed", "cancelling", "postponed", "notSet", "none"]
 QueuePriority = Literal["low", "belowNormal", "normal", "aboveNormal", "high"]
 
 # ========================================================================================================
 
 
 def get_build_definition(
@@ -72,15 +72,15 @@
                    build_definition, from_ado_date_string(data.get("startTime")), from_ado_date_string(data.get("finishTime")),
                    from_ado_date_string(data.get("queueTime")), data["reason"], data["priority"])  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, build_id: str) -> "Build":
         return super().get_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds/{build_id}?api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/build/builds/{build_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, definition_id: str, source_branch: str = "refs/heads/main", permit_use_of_var_groups: bool = False,  # fmt: skip
     ) -> "Build":
         """`permit_var_groups` defines whether the variable group will be automatically allowed for the build or need manual approval."""
@@ -88,42 +88,42 @@
         #     rint(f"Variable Groups: {BuildDefinition.get_by_id(ado_client, definition_id).variable_groups}")
         #     for var_group_id in BuildDefinition.get_by_id(ado_client, definition_id).variable_groups:
         #         request = requests.patch(f"https://dev.azure.com/{ado_client.ado_org}/{definition_id}/_apis/pipelines/pipelinePermissions/variablegroup/{var_group_id}")  # fmt: skip
         #         rint(request.text, request.status_code)
         #         assert request.status_code <= 204
         return super().create(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds?definitionId={definition_id}&api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/build/builds?definitionId={definition_id}&api-version=7.1",
             {"reason": "An automated build created with the ado_wrapper Python library", "sourceBranch": source_branch},
         )  # type: ignore[return-value]
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, build_id: str) -> None:  # type: ignore[override]
         cls.delete_all_leases(ado_client, build_id)
         return super().delete_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds/{build_id}?api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/build/builds/{build_id}?api-version=7.1",
             build_id,
         )
 
     def update(self, ado_client: AdoClient, attribute_name: str, attribute_value: Any) -> None:  # type: ignore[override]
         return super().update(
             ado_client, "patch",
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds/{self.build_id}?api-version=7.1-preview.7",
+            f"/{ado_client.ado_project}/_apis/build/builds/{self.build_id}?api-version=7.1",
             attribute_name, attribute_value, {attribute_name: attribute_value}  # fmt: skip
         )
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_all_by_definition(cls, ado_client: AdoClient, definition_id: str) -> "list[Build]":
         return super().get_all(ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds?api-version=7.1&definitions={definition_id}",
+            f"/{ado_client.ado_project}/_apis/build/builds?definitions={definition_id}&api-version=7.1",
         )  # type: ignore[return-value]
 
     def delete(self, ado_client: AdoClient) -> None:
         return self.delete_by_id(ado_client, self.build_id)
 
     @classmethod
     def create_and_wait_until_completion(cls, ado_client: AdoClient, definition_id: str, branch_name: str = "main",
@@ -140,15 +140,15 @@
                 raise TimeoutError(f"The build did not complete within {max_timeout_seconds} seconds ({max_timeout_seconds//60} minutes)")
             time.sleep(3)
         return build
 
     @staticmethod
     def delete_all_leases(ado_client: AdoClient, build_id: str) -> None:
         leases_request = requests.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds/{build_id}/leases?api-version=7.1-preview.1",
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds/{build_id}/leases?api-version=7.1",
             auth=ado_client.auth,
         )
         if leases_request.status_code != 200:
             print(f"Could not delete leases, {leases_request.status_code}")
             return
         leases = leases_request.json()["value"]
         for lease in leases:
@@ -192,25 +192,25 @@
         return cls(str(data["id"]), data["name"], data.get("description", ""), data.get("process", {"yamlFilename": "UNKNOWN"})["yamlFilename"], created_by,
                 from_ado_date_string(data.get("createdDate")), build_repository, str(data["revision"]), data.get("process"), data.get("variables", {}), data.get("variableGroups", []))  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, build_definition_id: str) -> "BuildDefinition":
         return super().get_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/definitions/{build_definition_id}?api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/build/definitions/{build_definition_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, name: str, repo_id: str, repo_name: str, path_to_pipeline: str,
         description: str, agent_pool_id: str, variable_groups: list[str], branch_name: str = "main",  # fmt: skip
     ) -> "BuildDefinition":
         return super().create(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/definitions?api-version=7.0",
+            f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.0",
             payload=get_build_definition(name, repo_id, repo_name, path_to_pipeline, description, ado_client.ado_project,
                                          agent_pool_id, branch_name)  # fmt: skip
         )  # type: ignore[return-value]
         #  | {"variableGroups": [{"id": x for x in variable_groups}]},
 
     def update(self, ado_client: AdoClient, attribute_name: BuildDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         if self.build_repo is None or self.process is None:
@@ -219,39 +219,39 @@
             {"name": self.name, "id": self.build_definition_id, "revision": int(self.revision),
              "repository": {"id": self.build_repo.build_repository_id, "type": self.build_repo.type},
              "process": {"yamlFilename": self.process["yamlFilename"], "type": self.process["type"]}} | # fmt: skip
             {attribute_name: attribute_value}  # fmt: skip
         )
         super().update(
             ado_client, "put",
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/definitions/{self.build_definition_id}?api-version=6.0", #secretsSourceDefinitionRevision={self.revision}&
+            f"/{ado_client.ado_project}/_apis/build/definitions/{self.build_definition_id}?api-version=7.1", #secretsSourceDefinitionRevision={self.revision}&
             attribute_name, attribute_value, payload  # fmt: skip
         )
         self.revision = str(int(self.revision) + 1)
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, resource_id: str) -> None:  # type: ignore[override]
         builds = Build.get_all_by_definition(ado_client, resource_id)
         for build in builds:
             build.delete(ado_client)
         return super().delete_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/definitions/{resource_id}?forceDelete=true&api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/build/definitions/{resource_id}?forceDelete=true&api-version=7.1",
             resource_id,
         )
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_all(cls, ado_client: AdoClient) -> "list[BuildDefinition]":  # type: ignore[override]
         return super().get_all(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/definitions?api-version=7.1-preview.7",
+            f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.1",
         )  # type: ignore[return-value]
 
     def get_all_builds_by_definition(self, ado_client: AdoClient) -> "list[Build]":
         return Build.get_all_by_definition(ado_client, self.build_definition_id)
 
     @classmethod
     def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str) -> "list[BuildDefinition]":
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/commits.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/commits.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     }
 
 
 @dataclass
 class Commit(StateManagedResource):
     """
     https://learn.microsoft.com/en-us/rest/api/azure/devops/git/commits?view=azure-devops-rest-7.1
-    https://learn.microsoft.com/en-us/rest/api/azure/devops/git/pushes?view=azure-devops-rest-5.1
+    https://learn.microsoft.com/en-us/rest/api/azure/devops/git/pushes?view=azure-devops-rest-7.1
     """
 
     commit_id: str = field(metadata={"is_id_field": True})  # None are editable
     author: Member
     date: datetime
     message: str
 
@@ -62,15 +62,15 @@
         member = Member(data["author"]["name"], data["author"]["email"], "UNKNOWN")
         return cls(data["commitId"], member, from_ado_date_string(data["author"]["date"]), data["comment"])
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, repo_id: str, commit_id: str) -> "Commit":  # type: ignore[override]
         return super().get_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/commits/{commit_id}?api-version=5.1",
+            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/commits/{commit_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, repo_id: str, from_branch_name: str, to_branch_name: str, updates: dict[str, str], change_type: ChangeType, commit_message: str,  # fmt: skip
     ) -> "Commit":
         """Creates a commit in the given repository with the given updates and returns the commit object.
@@ -79,15 +79,15 @@
             from_branch_name.startswith("refs/heads/") or to_branch_name.startswith("refs/heads/")
         ), "Branch names should not start with 'refs/heads/'"
         if not updates:
             raise ValueError("No updates provided! It's not possible to create a commit without updates.")
         latest_commit = cls.get_latest_by_repo(ado_client, repo_id, from_branch_name)
         latest_commit_id = None if latest_commit is None else latest_commit.commit_id
         data = get_commit_body_template(latest_commit_id, updates, to_branch_name, change_type, commit_message)
-        request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=5.1", json=data, auth=ado_client.auth)  # fmt: skip
+        request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=7.1", json=data, auth=ado_client.auth)  # fmt: skip
         if request.status_code == 400:
             raise ValueError("The commit was not created successfully, the file(s) you're trying to add might already exist there.")
         if request.status_code == 403:
             raise InvalidPermissionsError("You do not have permission to create a commit in this repo (possibly due to main branch protections)")  # fmt: skip
         if not request.json().get("commits"):
             raise ValueError("The commit was not created successfully.\nError:", request.json())
         return cls.from_request_payload(request.json()["commits"][-1])
@@ -107,24 +107,25 @@
     @classmethod
     def get_all_by_repo(cls, ado_client: AdoClient, repo_id: str, branch_name: str | None = None) -> "list[Commit]":
         """Returns a list of all commits in the given repository."""
         extra_query = (f"searchCriteria.itemVersion.version={branch_name}&searchCriteria.itemVersion.versionType={'branch'}&"
                        if branch_name is not None else "")  # fmt: skip
         return super().get_all(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/commits?{extra_query}api-version=7.1-preview.1",
+            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/commits?{extra_query}api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def add_initial_readme(cls, ado_client: AdoClient, repo_id: str) -> "Commit":
         default_commit_body = get_commit_body_template(None, {}, "main", "add", "")
         default_commit_body["commits"] = [{
-                "comment": "Add README.md",
-                "changes": [
-                    {"changeType": 1, "item": {"path": "/README.md"}, "newContentTemplate": {"name": "README.md", "type": "readme"}}
-                ],
+            "comment": "Add README.md",
+            "changes": [{
+                "changeType": 1, "item": {"path": "/README.md"},
+                "newContentTemplate": {"name": "README.md", "type": "readme"}
+            }],
         }]  # fmt: skip
         request = requests.post(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=5.1",
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=7.1",
             json=default_commit_body, auth=ado_client.auth,  # fmt: skip
         )
         return cls.from_request_payload(request.json()["commits"][0])
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/groups.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,30 +31,30 @@
     def from_request_payload(cls, data: dict[str, str]) -> "Group":
         return cls(data["url"].split("/_apis/Graph/Groups/", maxsplit=1)[1], data["displayName"], data.get("description", ""),
                    data["domain"].removeprefix("vstfs:///Classification/TeamProject/"), data["originId"])  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, group_descriptor: str) -> "Group":
         return super().get_by_id(
-            ado_client,
+            ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/groups/{group_descriptor}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(cls, ado_client: AdoClient, name: str) -> "Group":  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, group_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
     def get_all(cls, ado_client: AdoClient) -> list["Group"]:  # type: ignore[override]
         return super().get_all(
-            ado_client,
+            ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/groups?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/projects.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/projects.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,33 +18,32 @@
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Project":
         return cls(data["id"], data["name"], data.get("description", ""), data.get("lastUpdateTime"))
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, project_id: str) -> "Project":
-        request = requests.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects/{project_id}?api-version=7.1-preview.4",
-            auth=ado_client.auth,
-        ).json()
-        return cls.from_request_payload(request)
+        return super().get_by_id(
+            ado_client,
+            f"/_apis/projects/{project_id}?api-version=7.1",
+        )  # type: ignore[return-value]
 
     @classmethod
     def create(cls, ado_client: AdoClient, project_name: str, project_description: str) -> "Project":  # type: ignore[override]
         raise NotImplementedError
 
     @staticmethod
     def delete_by_id(ado_client: AdoClient, project_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
     def get_all(cls, ado_client: AdoClient) -> list["Project"]:  # type: ignore[override]
         return super().get_all(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects?api-version=7.1-preview.4",
+            "/_apis/projects?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/repo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,176 +1,187 @@
 from __future__ import annotations
 
-from datetime import datetime
-from typing import Any, Literal, TYPE_CHECKING
+import io
+import zipfile
 from dataclasses import dataclass, field
+from typing import Any, Literal
 
 import requests
 
-from ado_wrapper.utils import from_ado_date_string, ResourceNotFound
+from ado_wrapper.client import AdoClient
 from ado_wrapper.state_managed_abc import StateManagedResource
-from ado_wrapper.resources.users import Member, Reviewer
-from ado_wrapper.attribute_types import PullRequestEditableAttribute
+from ado_wrapper.resources.pull_requests import PullRequest, PullRequestStatus
+from ado_wrapper.resources.commits import Commit
+from ado_wrapper.utils import ResourceNotFound, UnknownError
 
-if TYPE_CHECKING:
-    from ado_wrapper.client import AdoClient
-    from ado_wrapper.resources.repo import Repo
+# from plan_resources.singletons import plannable_resource
+RepoEditableAttribute = Literal["name", "default_branch", "is_disabled"]
 
-PullRequestStatus = Literal["active", "completed", "abandoned", "all", "notSet"]
-MergeStatus = Literal["succeeded", "conflicts", "rejectedByPolicy", "rejectedByUser", "queued", "notSet"]
+# ====================================================================
 
 
 @dataclass
-class PullRequest(StateManagedResource):
-    """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/pull-requests?view=azure-devops-rest-7.1"""
+class Repo(StateManagedResource):
+    """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/repositories?view=azure-devops-rest-7.1"""
 
-    pull_request_id: str = field(metadata={"is_id_field": True})
-    title: str = field(metadata={"editable": True})
-    description: str = field(metadata={"editable": True})
-    source_branch: str = field(repr=False)
-    target_branch: str = field(repr=False)
-    author: Member
-    creation_date: datetime = field(repr=False)
-    repository: Repo
-    close_date: datetime | None = field(default=None, repr=False)
-    is_draft: bool = field(default=False, repr=False)  # , metadata={"editable": True, "internal_name": "isDraft"})  # Hmmm
-    status: MergeStatus = field(
-        default="notSet", metadata={"editable": True}
-    )  # It's actual name is mergeStatus, but the update endpoint uses this name
-    reviewers: list[Reviewer] = field(default_factory=list, repr=False)  # Static(ish)
+    repo_id: str = field(metadata={"is_id_field": True})
+    name: str = field(metadata={"editable": True})
+    default_branch: str = field(default="main", repr=False, metadata={"editable": True, "internal_name": "defaultBranch"})
+    is_disabled: bool = field(default=False, repr=False, metadata={"editable": True, "internal_name": "isDisabled"})
+    # WARNING, disabling a repo means it's not able to be deleted, proceed with caution.
 
     def __str__(self) -> str:
-        return f"PullRequest(id={self.pull_request_id}, title={self.title}, author={self.author!s}, status={self.status})"
+        return f"Repo(name={self.name}, id={self.repo_id})"
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "PullRequest":
-        from ado_wrapper.resources.repo import Repo  # Circular import
-
-        member = Member(data["createdBy"]["displayName"], data["createdBy"]["uniqueName"], data["createdBy"]["id"])
-        reviewers = [Reviewer.from_request_payload(reviewer) for reviewer in data["reviewers"]]
-        repository = Repo(data["repository"]["id"], data["repository"]["name"])
-        return cls(str(data["pullRequestId"]), data["title"], data.get("description", ""), data["sourceRefName"],
-                   data["targetRefName"], member, from_ado_date_string(data["creationDate"]), repository,
-                   from_ado_date_string(data.get("closedDate")), data["isDraft"], data.get("mergeStatus", "notSet"), reviewers)  # fmt: skip
+    def from_request_payload(cls, data: dict[str, str]) -> "Repo":
+        return cls(
+            data["id"], data["name"], data.get("defaultBranch", "main").removeprefix("refs/heads/"), bool(data.get("isDisabled", False))
+        )
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, pull_request_id: str) -> "PullRequest":
+    def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> "Repo":
         return super().get_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/pullrequests/{pull_request_id}?api-version=7.1-preview.1",
+            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(  # type: ignore[override]
-        cls, ado_client: AdoClient, repo_id: str, from_branch_name: str, pull_request_title: str,
-        pull_request_description: str, is_draft: bool = False
-    ) -> "PullRequest":  # fmt: skip
-        """Takes a list of reviewer ids, a branch to pull into main, and an option to start as draft"""
-        # https://stackoverflow.com/questions/64655138/add-reviewers-to-azure-devops-pull-request-in-api-call   <- Why we can't allow reviewers from the get go
-        # , "reviewers": [{"id": reviewer_id for reviewer_id in reviewer_ids}]
-        payload = {"sourceRefName": f"refs/heads/{from_branch_name}", "targetRefName": "refs/heads/main", "title": pull_request_title,
-                   "description": pull_request_description, "isDraft": is_draft}  # fmt: skip
-        request = requests.post(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullrequests?api-version=7.1-preview.1",
-            json=payload, auth=ado_client.auth,  # fmt: skip
-        ).json()
-        if request.get("message", "").startswith("TF401398"):
-            raise ValueError("The branch you are trying to create a pull request from does not exist.")
-        obj = cls.from_request_payload(request)
-        ado_client.state_manager.add_resource_to_state(cls.__name__, obj.pull_request_id, obj.to_json())  # type: ignore[arg-type]
-        return obj
-
-    @classmethod
-    def delete_by_id(cls, ado_client: AdoClient, pull_request_id: str) -> None:  # type: ignore[override]
-        # raise NotImplementedError("You can't delete pull requests, only close them.")
-        pr = cls.get_by_id(ado_client, pull_request_id)
-        pr.update(ado_client, "status", "abandoned")
-        ado_client.state_manager.remove_resource_from_state("PullRequest", pull_request_id)
+    # @plannable_resource
+    def create(cls, ado_client: AdoClient, name: str, include_readme: bool = True) -> "Repo":  # type: ignore[override]
+        repo: Repo = super().create(
+            ado_client,
+            f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
+            {"name": name},
+        )  # type: ignore[assignment]
+        if include_readme:
+            Commit.add_initial_readme(ado_client, repo.repo_id)
+        return repo
 
-    def update(self, ado_client: AdoClient, attribute_name: PullRequestEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
+    def update(self, ado_client: AdoClient, attribute_name: RepoEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         return super().update(
             ado_client, "patch",
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repository.repo_id}/pullRequests/{self.pull_request_id}?api-version=7.1-preview.1",
-            attribute_name, attribute_value, {}  # fmt: skip
+            f"/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}?api-version=7.1",
+            attribute_name, attribute_value, {},  # fmt: skip
+        )
+
+    @classmethod
+    def delete_by_id(cls, ado_client: AdoClient, repo_id: str) -> None:  # type: ignore[override]
+        for pull_request in Repo.get_all_pull_requests(ado_client, repo_id, "all"):
+            ado_client.state_manager.remove_resource_from_state("PullRequest", pull_request.pull_request_id)
+        return super().delete_by_id(
+            ado_client,
+            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
+            repo_id,
         )
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient, status: PullRequestStatus = "all") -> list[PullRequest]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list["Repo"]:  # type: ignore[override]
         return super().get_all(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/pullrequests?searchCriteria.status={status}&api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
-    def add_reviewer(self, ado_client: AdoClient, reviewer_id: str) -> None:
-        return self.add_reviewer_static(ado_client, self.repository.repo_id, self.pull_request_id, reviewer_id)
+    @classmethod
+    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> "Repo":
+        """Warning, this function must fetch `all` repos to work, be cautious when calling it in a loop."""
+        for repo in cls.get_all(ado_client):
+            if repo.name == repo_name:
+                return repo
+        raise ValueError(f"Repo {repo_name} not found")
 
-    @staticmethod
-    def add_reviewer_static(ado_client: AdoClient, repo_id: str, pull_request_id: str, reviewer_id: str) -> None:
-        """Copy of the add_reviewer method, but static, i.e. if you have the repo id and pr id, you don't need to fetch them again"""
-        request = requests.put(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/reviewers/{reviewer_id}?api-version=7.1-preview.1",
-                                json={"vote": "0", "isRequired": "true"}, auth=ado_client.auth)  # fmt: skip
-        assert request.status_code < 300
+    def get_file(self, ado_client: AdoClient, file_path: str, branch_name: str = "main") -> str:
+        request = requests.get(
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?path={file_path}&versionType={'Branch'}&version={branch_name}&api-version=7.1",
+            auth=ado_client.auth,
+        )
+        if request.status_code == 404:
+            raise ResourceNotFound(f"File {file_path} not found in repo {self.repo_id}")
+        if request.status_code != 200:
+            raise UnknownError(f"Error getting file {file_path} from repo {self.repo_id}: {request.text}")
+        return request.text  # This is the file content
+
+    def get_contents(self, ado_client: AdoClient, file_types: list[str] | None = None, branch_name: str = "main") -> dict[str, str]:
+        """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/items/get?view=azure-devops-rest-7.1&tabs=HTTP
+        This function downloads the contents of a repo, and returns a dictionary of the files and their contents
+        The file_types parameter is a list of file types to filter for, e.g. ["json", "yaml"]"""
+        try:
+            request = requests.get(
+                f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?recursionLevel={'Full'}&download={True}&$format={'Zip'}&versionDescriptor.version={branch_name}&api-version=7.1",
+                auth=ado_client.auth,
+            )
+        except requests.exceptions.ConnectionError:
+            print(f"=== Connection error, failed to download {self.repo_id}")
+            return {}
+        if request.status_code != 200:
+            print(f"Error getting repo contents for {self.name} ({self.repo_id}):", request.text)
+            return {}
+        # ============ We do this because ADO ===================
+        bytes_io = io.BytesIO()
+        for chunk in request.iter_content(chunk_size=128):
+            bytes_io.write(chunk)
 
-    def change_status(self, ado_client: AdoClient, status: PullRequestStatus) -> None:
-        self.update(ado_client, "status", status)
+        files = {}
+        try:
+            with zipfile.ZipFile(bytes_io) as zip_ref:
+                # For each file, read the bytes and convert to string
+                for file_name in [x for x in zip_ref.namelist() if file_types is None or x.split(".")[-1] in file_types]:
+                    try:
+                        files[file_name] = zip_ref.read(file_name).decode()  # fmt: skip
+                    except UnicodeDecodeError:
+                        print(f"Error decoding file: {file_name} in {self.name}")
+        except zipfile.BadZipFile as e:
+            print(f"{self.name} ({self.repo_id}) couldn't be unzipped:", e)
+
+        bytes_io.close()
+        # =========== That's all I have to say ==================
+        return files
+
+    def create_pull_request(self, ado_client: AdoClient, branch_name: str, pull_request_title: str, pull_request_description: str) -> "PullRequest":  # fmt: skip
+        """Helper function which redirects to the PullRequest class to make a PR"""
+        return PullRequest.create(ado_client, self.repo_id, branch_name, pull_request_title, pull_request_description)
 
-    def close(self, ado_client: AdoClient) -> None:
-        self.update(ado_client, "status", "abandoned")
+    @staticmethod
+    def get_all_pull_requests(ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list["PullRequest"]:
+        return PullRequest.get_all_by_repo_id(ado_client, repo_id, status)
 
     def delete(self, ado_client: AdoClient) -> None:
-        self.delete_by_id(ado_client, self.pull_request_id)
+        if self.is_disabled:
+            self.update(ado_client, "is_disabled", False)
+        self.delete_by_id(ado_client, self.repo_id)
 
-    def mark_as_draft(self, ado_client: AdoClient, is_draft: bool = True) -> None:
-        json_payload = {"isDraft": is_draft}
-        request = requests.patch(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repository.repo_id}/pullRequests/{self.pull_request_id}?api-version=7.1",
-            json=json_payload,
-            auth=ado_client.auth,
-        )
-        if request.status_code == 404:
-            raise ValueError("The pull request or repo could not be found!")
-        assert request.status_code < 300
-        self.is_draft = is_draft
+    @staticmethod
+    def get_content_static(
+        ado_client: AdoClient, repo_id: str, file_types: list[str] | None = None, branch_name: str = "main"
+    ) -> dict[str, str]:
+        repo = Repo.get_by_id(ado_client, repo_id)
+        return repo.get_contents(ado_client, file_types, branch_name)
 
-    def unmark_as_draft(self, ado_client: AdoClient) -> None:
-        self.mark_as_draft(ado_client, False)
 
-    def get_reviewers(self, ado_client: AdoClient) -> list[Member]:
-        request = requests.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repository.repo_id}/pullRequests/{self.pull_request_id}/reviewers?api-version=7.1",
-            auth=ado_client.auth,
-        ).json()
-        return [Member(reviewer["displayName"], reviewer["uniqueName"], reviewer["id"]) for reviewer in request["value"]]
+# ====================================================================
 
-    @classmethod
-    def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list[PullRequest]:
-        pull_requests = requests.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullrequests?searchCriteria.status={status}&api-version=7.1",
-            auth=ado_client.auth,
-        ).json()
-        try:
-            return [PullRequest.from_request_payload(pr) for pr in pull_requests["value"]]
-        except KeyError:
-            if pull_requests.get("message", "").startswith("TF401019"):
-                print(f"Repo `{pull_requests['message'].split('identifier')[1].split(' ')[0]}` was disabled, or you had no access.")
-                return []
-            raise ResourceNotFound(pull_requests)  # pylint: disable=raise-missing-from
-
-    @classmethod
-    def get_all_by_author(cls, ado_client: AdoClient, author_email: str, status: PullRequestStatus = "all") -> list[PullRequest]:
-        all_pull_requests: list[PullRequest] = cls.get_all(ado_client, status)
-        return [pr for pr in all_pull_requests if pr.author.email == author_email]
-
-    @classmethod
-    def get_my_pull_requests(cls, ado_client: AdoClient) -> list[PullRequest]:
-        """This is super tempremental, I have to do a bunch of splits, it's not official so might not work"""
-        import json
-
-        request = requests.get(f"https://dev.azure.com/{ado_client.ado_org}/_pulls", auth=ado_client.auth)
-        raw_data = (
-            request.text.split("application/json")[1].split('pullRequests"')[1].split("queries")[0].removeprefix(":").removesuffix(',"')
-        )
-        return [cls.from_request_payload(pr) for pr in json.loads(raw_data).values()]
+
+@dataclass
+class BuildRepository:
+    build_repository_id: str = field(metadata={"is_id_field": True})
+    name: str | None = None
+    type: str = "TfsGit"
+    clean: bool | None = None
+    checkout_submodules: bool = field(default=False, metadata={"internal_name": "checkoutSubmodules"})
+
+    @classmethod
+    def from_request_payload(cls, data: dict[str, str | bool]) -> "BuildRepository":
+        return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
+
+    @classmethod
+    def from_json(cls, data: dict[str, str | bool]) -> "BuildRepository":
+        return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
+
+    def to_json(self) -> dict[str, str | bool | None]:
+        return {
+            "id": self.build_repository_id, "name": self.name, "type": self.type,
+            "clean": self.clean, "checkoutSubmodules": self.checkout_submodules,  # fmt: skip
+        }
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/releases.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/releases.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import requests
 
 from ado_wrapper.client import AdoClient
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.utils import from_ado_date_string
 from ado_wrapper.resources.users import Member
 
+ReleaseDefinitionEditableAttribute = Literal["name", "description", "release_name_format", "variable_groups"]
 ReleaseStatus = Literal["active", "abandoned", "draft", "undefined"]
 
 # ========================================================================================================
 # WARNING: THIS FILE IS MAINLY UNTESTED, AND MAY NOT WORK AS EXPECTED
 # FEEL FREE TO MAKE A PR TO FIX/IMPROVE THIS FILE
 # ========================================================================================================
 
@@ -208,15 +209,15 @@
             release.delete(ado_client)
         return super().delete_by_id(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions/{release_definition_id}?forceDelete=True&api-version=7.1",
             release_definition_id,
         )
 
-    def update(self, ado_client: AdoClient, attribute_name: str, attribute_value: Any) -> None:  # type: ignore[override]
+    def update(self, ado_client: AdoClient, attribute_name: ReleaseDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         self.revision = str(int(self.revision) + 1)
         return super().update(
             ado_client, "put",
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions/{self.release_definition_id}?api-version=7.1",
             attribute_name, attribute_value, self._raw_data,  # fmt: skip
         )
 
@@ -234,15 +235,15 @@
             auth=ado_client.auth,
         ).json()
         return [Release.from_request_payload(release) for release in response["value"]]
 
     @classmethod
     def get_all(cls, ado_client: AdoClient) -> "list[ReleaseDefinition]":  # type: ignore[override]
         response = requests.get(
-            f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions?api-version=7.1-preview.4",
+            f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions?api-version=7.1",
             auth=ado_client.auth,
         ).json()["value"]
         return [cls.from_request_payload(data) for data in response]
 
 
 # ========================================================================================================
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/teams.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/teams.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,39 +29,37 @@
     def from_request_payload(cls, data: dict[str, str]) -> "Team":
         return cls(data["id"], data["name"], data.get("description", ""), [])
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, team_id: str) -> "Team":
         resource: Team = super().get_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects/{ado_client.ado_project}/teams/{team_id}?$expandIdentity={True}&api-version=7.1-preview.2",
+            f"/_apis/projects/{ado_client.ado_project}/teams/{team_id}?$expandIdentity={True}&api-version=7.1-preview.1",
         )  # type: ignore[assignment]
         resource.team_members = resource.get_members(ado_client)
         return resource
 
     @classmethod
     def create(cls, ado_client: AdoClient, name: str, description: str) -> "Team":  # type: ignore[override]
         raise NotImplementedError
-        # request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/_apis/teams?api-version=7.1-preview.2", json={"name": name, "description": description}, auth=ado_client.auth).json()
+        # request = requests.post(f"/_apis/teams?api-version=7.1", json={"name": name, "description": description}, auth=ado_client.auth).json()
         # return cls.from_request_payload(request)
 
     def update(self, ado_client: AdoClient, attribute_name: str, attribute_value: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, team_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
-        # request = requests.delete(f"https://dev.azure.com/{ado_client.ado_org}/_apis/teams/{team_id}?api-version=7.1-preview.2", auth=ado_client.auth)
-        # assert request.status_code < 300
 
     @classmethod
     def get_all(cls, ado_client: AdoClient) -> list["Team"]:  # type: ignore[override]
         return super().get_all(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/_apis/teams?api-version=7.1-preview.2",  # /projects/{ado_client.ado_project}
+            "/_apis/teams?api-version=7.1-preview.2",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/users.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,32 +43,31 @@
     @classmethod
     def from_request_payload(cls, data: dict[str, str]) -> "AdoUser":
         return cls(data["descriptor"], data["displayName"], data["mailAddress"].removeprefix("vstfs:///Classification/TeamProject/"),
                    data["origin"], data["originId"])  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, descriptor_id: str) -> "AdoUser":
-        request = requests.get(
-            f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users/{descriptor_id}?api-version=6.0-preview.1",
-            auth=ado_client.auth,
-        ).json()
-        return cls.from_request_payload(request)
+        return super().get_by_id(
+            ado_client,  # Preview required
+            f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users/{descriptor_id}?api-version=7.1-preview.1",
+        )  # type: ignore[return-value]
 
     @classmethod
     def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> "AdoUser":  # type: ignore[override]
         raise NotImplementedError("Creating a new user is not supported")
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, member_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError("Deleting a user is not supported")
 
     @classmethod
     def get_all(cls, ado_client: AdoClient) -> list["AdoUser"]:  # type: ignore[override]
         return super().get_all(
-            ado_client,
+            ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-0.0.4/ado_wrapper/resources/variable_groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Any, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING, Literal
 from dataclasses import dataclass, field
 
 from ado_wrapper.utils import from_ado_date_string
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
-from ado_wrapper.attribute_types import VariableGroupEditableAttribute
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
+VariableGroupEditableAttribute = Literal["variables"]
+
 
 @dataclass
 class VariableGroup(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/distributedtask/variablegroups?view=azure-devops-rest-7.1"""
 
     variable_group_id: str = field(metadata={"is_id_field": True})
     name: str  # Cannot currently change the name of a variable group
@@ -37,15 +38,15 @@
                    {key: value["value"] if isinstance(value, dict) else value for key, value in data["variables"].items()},
                    from_ado_date_string(data["createdOn"]), created_by, modified_by, from_ado_date_string(data.get("modifiedOn")))  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, variable_group_id: str) -> "VariableGroup":
         return super().get_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/distributedtask/variablegroups/{variable_group_id}?api-version=7.1-preview.2",
+            f"/{ado_client.ado_project}/_apis/distributedtask/variablegroups/{variable_group_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, variable_group_name: str, variable_group_description: str, variables: dict[str, str]  # fmt: skip
     ) -> "VariableGroup":
         payload = {
@@ -59,43 +60,43 @@
                     "name": variable_group_name,
                     "projectReference": {"id": ado_client.ado_project_id, "name": ado_client.ado_project},
                 }
             ],
         }
         return super().create(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/distributedtask/variablegroups?api-version=7.1-preview.2",
+            f"/{ado_client.ado_project}/_apis/distributedtask/variablegroups?api-version=7.1",
             payload,
         )  # type: ignore[return-value]
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, variable_group_id: str) -> None:  # type: ignore[override]
         return super().delete_by_id(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/_apis/distributedtask/variablegroups/{variable_group_id}?projectIds={ado_client.ado_project_id}&api-version=7.1-preview.2",
+            f"/_apis/distributedtask/variablegroups/{variable_group_id}?projectIds={ado_client.ado_project_id}&api-version=7.1",
             variable_group_id,
         )
 
     def update(self, ado_client: AdoClient, attribute_name: VariableGroupEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         # WARNING: This method works 80-90% of the time, for some reason, it fails randomly, ADO API is at fault.
         params = {
             "variableGroupProjectReferences": [{"name": self.name, "projectReference": {"id": ado_client.ado_project_id}}],
              "id": self.variable_group_id, "name": self.name, "type": "Vsts", "variables": self.variables  # fmt: skip
         }
         super().update(
             ado_client, "put",
-            f"https://dev.azure.com/{ado_client.ado_org}/_apis/distributedtask/variablegroups/{self.variable_group_id}?api-version=7.1-preview.2",
+            f"/_apis/distributedtask/variablegroups/{self.variable_group_id}?api-version=7.1",
             attribute_name, attribute_value, params  # fmt: skip
         )
 
     @classmethod
     def get_all(cls, ado_client: AdoClient) -> list["VariableGroup"]:  # type: ignore[override]
         return super().get_all(
             ado_client,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/distributedtask/variablegroups?api-version=7.1-preview.2",
+            f"/{ado_client.ado_project}/_apis/distributedtask/variablegroups?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     def delete(self, ado_client: AdoClient) -> None:
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/state_managed_abc.py` & `ado_wrapper-0.0.4/ado_wrapper/state_managed_abc.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,29 +13,29 @@
     from ado_wrapper.client import AdoClient
 
 
 def recursively_convert_to_json(attribute_name: str, attribute_value: Any) -> tuple[str, Any]:
     if isinstance(attribute_value, dict):
         return attribute_name, {key: recursively_convert_to_json("", value)[1] for key, value in attribute_value.items()}
     if isinstance(attribute_value, list):
-        return attribute_name, [recursively_convert_to_json(attribute_name, value) for value in attribute_value]
+        return attribute_name, [recursively_convert_to_json(attribute_name, value)[1] for value in attribute_value]
     if isinstance(attribute_value, datetime):
         return f"{attribute_name}::datetime", attribute_value.isoformat()
     if type(attribute_value) in get_resource_variables().values():
         class_name = str(type(attribute_value)).rsplit(".", maxsplit=1)[-1].removesuffix("'>")
         return attribute_name + "::" + class_name, attribute_value.to_json()
     return attribute_name, str(attribute_value)
 
 
 def recursively_convert_from_json(dictionary: dict[str, Any]) -> Any:
     data_copy = dict(dictionary.items())  # Deep copy
     for key, value in dictionary.items():
         if isinstance(key, str) and "::" in key and key.split("::")[-1] != "datetime":
             instance_name, class_type = key.split("::")
-            class_ = [x for x in get_resource_variables().values() if x.__name__ == class_type][0]
+            class_ = get_resource_variables()[class_type]
             del data_copy[key]
             data_copy[instance_name] = class_.from_json(value)
         elif isinstance(key, str) and key.endswith("::datetime"):
             del data_copy[key]
             data_copy[key.split("::")[0]] = datetime.fromisoformat(value)
     return data_copy
 
@@ -53,62 +53,76 @@
     def from_json(cls, data: dict[str, Any]) -> "StateManagedResource":
         return cls(**recursively_convert_from_json(data))
 
     def to_json(self) -> dict[str, Any]:
         attribute_names = [field_obj.name for field_obj in fields(self)]
         attribute_values = [getattr(self, field_obj.name) for field_obj in fields(self)]
         combined = zip(attribute_names, attribute_values)
-        return dict(recursively_convert_to_json(attribute_name, attribute_value) for attribute_name, attribute_value in combined)
+        return dict(recursively_convert_to_json(attribute_name, attribute_value) for attribute_name, attribute_value in combined) ####
 
     @classmethod
     def get_by_id(cls, ado_client: "AdoClient", url: str) -> "StateManagedResource":
+        if not url.startswith("https://"):
+            url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
         request = requests.get(url, auth=ado_client.auth)
         if request.status_code == 404:
             raise ResourceNotFound(f"No {cls.__name__} found with that identifier!")
         if request.status_code >= 300:
             raise ValueError(f"Error getting {cls.__name__} by id: {request.text}")
+        if "value" in request.json():
+            return cls.from_request_payload(request.json()["value"][0])
         return cls.from_request_payload(request.json())
 
     @classmethod
     def create(cls, ado_client: "AdoClient", url: str, payload: dict[str, Any] | None = None) -> "StateManagedResource":
+        if not url.startswith("https://"):
+            url = f"https://dev.azure.com/{ado_client.ado_org}" + url
         request = requests.post(url, json=payload or {}, auth=ado_client.auth)  # Create a brand new dict
         if request.status_code == 401:
             raise PermissionError(f"You do not have permission to create this {cls.__name__}!")
         if request.status_code == 409:
             raise ResourceAlreadyExists(f"The {cls.__name__} with that identifier already exist!")
         resource = cls.from_request_payload(request.json())
         ado_client.state_manager.add_resource_to_state(cls.__name__, extract_id(resource), resource.to_json())  # type: ignore[arg-type]
         return resource
 
     @classmethod
     def delete_by_id(cls, ado_client: "AdoClient", url: str, resource_id: str) -> None:
+        """Deletes an object by its id. The id is passed so it can be removed from state"""
+        if not url.startswith("https://"):
+            url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
         request = requests.delete(url, auth=ado_client.auth)
         if request.status_code != 204:
             if request.status_code == 404:
                 print("[ADO_WRAPPER] Resource not found, probably already deleted, removing from state")
             else:
                 raise DeletionFailed(f"[ADO_WRAPPER] Error deleting {cls.__name__} ({resource_id}): {request.json()['message']}")
         ado_client.state_manager.remove_resource_from_state(cls.__name__, resource_id)  # type: ignore[arg-type]
 
     def update(self, ado_client: "AdoClient", update_action: Literal["put", "patch"], url: str,  # pylint: disable=too-many-arguments
                attribute_name: str, attribute_value: Any, params: dict[str, Any]) -> None:  # fmt: skip
         """The params should be a dictionary which will be combined with the internal name and value of the attribute to be updated."""
         interal_names = get_internal_field_names(self.__class__)
         if attribute_name not in get_internal_field_names(self.__class__):
-            raise ValueError(f"The attribute {attribute_name} is not editable!  Editable attributes: {interal_names}")
+            raise ValueError(f"The attribute `{attribute_name}` is not editable!  Editable attributes are: {list(interal_names.keys())}")
         params |= {interal_names[attribute_name]: attribute_value}
 
         func = requests.put if update_action == "put" else requests.patch
+        # request = requests.request(update_action, url, json=params, auth=ado_client.auth)
+        if not url.startswith("https://"):
+            url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
         request = func(url, json=params, auth=ado_client.auth)
         if request.status_code != 200:
             raise UpdateFailed(
                 f"Failed to update {self.__class__.__name__} with id {extract_id(self)} and attribute {attribute_name} to {attribute_value}. \nReason:\n{request.text}"
             )
         setattr(self, attribute_name, attribute_value)
         ado_client.state_manager.update_resource_in_state(self.__class__.__name__, extract_id(self), self.to_json())  # type: ignore[arg-type]
 
     @classmethod
     def get_all(cls, ado_client: "AdoClient", url: str) -> list["StateManagedResource"]:
+        if not url.startswith("https://"):
+            url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
         request = requests.get(url, auth=ado_client.auth)
         if request.status_code >= 300:
             raise ValueError(f"Error getting all {cls.__name__}: {request.text}")
         return [cls.from_request_payload(resource) for resource in request.json()["value"]]
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/state_manager.py` & `ado_wrapper-0.0.4/ado_wrapper/state_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 from pathlib import Path
 from datetime import datetime
 from uuid import uuid4
 from typing import Any, TypedDict, TYPE_CHECKING  # , Generator
 
-from ado_wrapper.attribute_types import ResourceType
-from ado_wrapper.utils import DeletionFailed, get_resource_variables
+from ado_wrapper.utils import DeletionFailed, get_resource_variables, ResourceType
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 STATE_FILE_VERSION = "1.4"
 
 
@@ -47,15 +46,15 @@
         if self.state_file_name is None:
             print("[ADO_WRAPPER] Not storing state, so not adding resource to state")
             return None
         all_states = self.load_state()
         if resource_id in all_states["resources"][resource_type]:
             self.remove_resource_from_state(resource_type, resource_id)
         metadata = {"created_datetime": datetime.now().isoformat(), "run_id": self.run_id}
-        all_data = {resource_id: {"data": resource_data, "metadata": metadata, "lifecycle-status": {}}}
+        all_data = {resource_id: {"data": resource_data, "metadata": metadata, "lifecycle-policies": {}}}
         all_states["resources"][resource_type] |= all_data
         return self.write_state_file(all_states)
 
     def remove_resource_from_state(self, resource_type: ResourceType, resource_id: str) -> None:
         if self.state_file_name is None:
             print("[ADO_WRAPPER] Not storing state, so not removing resource to state")
             return None
@@ -97,16 +96,15 @@
             for resource_id in resources:
                 try:
                     self.delete_resource(resource_type, resource_id)  # pyright: ignore[reportArgumentType]
                 except DeletionFailed as e:
                     print(f"[ADO_WRAPPER] Error deleting {resource_type} {resource_id}: {e}")
 
     def import_into_state(self, resource_type: ResourceType, resource_id: str) -> None:
-        all_resource_classes = get_resource_variables()
-        class_reference = [value for key, value in all_resource_classes.items() if key == resource_type][0]
+        class_reference = get_resource_variables()[resource_type]
         data = class_reference.get_by_id(self.ado_client, resource_id).to_json()
         self.add_resource_to_state(resource_type, resource_id, data)
 
     def wipe_state(self) -> None:
         if self.state_file_name is None:
             return
         with open(self.state_file_name, "w", encoding="utf-8") as state_file:
```

### Comparing `ado_wrapper-0.0.3/ado_wrapper/utils.py` & `ado_wrapper-0.0.4/ado_wrapper/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from datetime import datetime, timezone
-from typing import overload, TYPE_CHECKING, Any
+from typing import overload, TYPE_CHECKING, Any, Literal
 from dataclasses import fields
 
 if TYPE_CHECKING:
     from ado_wrapper.state_managed_abc import StateManagedResource
 
+ResourceType = Literal[
+    "Branch", "Build", "BuildDefinition", "Commit", "Project", "PullRequest", "Release", "ReleaseDefinition",
+    "Repo", "Team", "AdoUser", "Member", "ServiceEndpoint", "Reviewer", "VariableGroup"  # fmt: skip
+]
+
 
 @overload
 def from_ado_date_string(date_string: str) -> datetime:
     ...
 
 
 @overload
@@ -111,18 +116,20 @@
 class InvalidPermissionsError(Exception):
     pass
 
 
 class UpdateFailed(Exception):
     pass
 
+class AuthenticationError(Exception):
+    pass
+
 
 def get_resource_variables() -> dict[str, type["StateManagedResource"]]:  # We do this to avoid circular imports
     """This returns a mapping of resource name (str) to the class type of the resource. This is used to dynamically create instances of resources."""
     from ado_wrapper.resources import (  # type: ignore[attr-defined]  # pylint: disable=possibly-unused-variable
         Branch, Build, BuildDefinition, Commit, Project, PullRequest, Release, ReleaseDefinition, Repo, BuildRepository, Team,
-        AdoUser, Member, Reviewer, VariableGroup,  # fmt: skip
+        AdoUser, Member, ServiceEndpoint, Reviewer, VariableGroup,  # fmt: skip
     )
 
     # When you update that ^, also run generate_type hints.py
-
     return locals()
```

### Comparing `ado_wrapper-0.0.3/pyproject.toml` & `ado_wrapper-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "0.0.3"
+version = "0.0.4"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-0.0.3/PKG-INFO` & `ado_wrapper-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

