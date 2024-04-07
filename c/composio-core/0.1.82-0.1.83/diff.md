# Comparing `tmp/composio_core-0.1.82.tar.gz` & `tmp/composio_core-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.82.tar", last modified: Sun Apr  7 18:19:40 2024, max compression
+gzip compressed data, was "composio_core-0.1.83.tar", last modified: Sun Apr  7 18:31:15 2024, max compression
```

## Comparing `composio_core-0.1.82.tar` & `composio_core-0.1.83.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:19:40.394109 composio_core-0.1.82/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.82/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 18:19:40.393854 composio_core-0.1.82/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.82/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:19:40.389556 composio_core-0.1.82/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.82/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    12769 2024-04-07 18:04:06.000000 composio_core-0.1.82/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:19:40.391419 composio_core-0.1.82/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.82/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5864 2024-04-07 18:09:53.000000 composio_core-0.1.82/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6973 2024-04-07 11:39:25.000000 composio_core-0.1.82/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    16559 2024-04-07 18:08:54.000000 composio_core-0.1.82/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2107 2024-04-07 11:38:27.000000 composio_core-0.1.82/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.82/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:19:40.393542 composio_core-0.1.82/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 18:19:40.000000 composio_core-0.1.82/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-07 18:19:40.000000 composio_core-0.1.82/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 18:19:40.000000 composio_core-0.1.82/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-07 18:19:40.000000 composio_core-0.1.82/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       91 2024-04-07 18:19:40.000000 composio_core-0.1.82/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-07 18:19:40.000000 composio_core-0.1.82/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      509 2024-04-06 14:07:21.000000 composio_core-0.1.82/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 14:07:21.000000 composio_core-0.1.82/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 18:19:40.394159 composio_core-0.1.82/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-07 18:19:29.000000 composio_core-0.1.82/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 18:31:15.186828 composio_core-0.1.83/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.83/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 18:31:15.186569 composio_core-0.1.83/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.83/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 18:31:15.181195 composio_core-0.1.83/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.83/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    12769 2024-04-07 18:30:34.000000 composio_core-0.1.83/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 18:31:15.183599 composio_core-0.1.83/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.83/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5864 2024-04-07 18:28:35.000000 composio_core-0.1.83/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    10555 2024-04-07 18:30:29.000000 composio_core-0.1.83/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    16559 2024-04-07 18:28:35.000000 composio_core-0.1.83/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2107 2024-04-07 15:47:29.000000 composio_core-0.1.83/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2861 2024-04-06 13:52:08.000000 composio_core-0.1.83/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 18:31:15.185644 composio_core-0.1.83/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 18:31:15.000000 composio_core-0.1.83/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-07 18:31:15.000000 composio_core-0.1.83/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 18:31:15.000000 composio_core-0.1.83/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-07 18:31:15.000000 composio_core-0.1.83/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       91 2024-04-07 18:31:15.000000 composio_core-0.1.83/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-07 18:31:15.000000 composio_core-0.1.83/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      509 2024-04-06 13:53:19.000000 composio_core-0.1.83/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       92 2024-04-06 13:54:53.000000 composio_core-0.1.83/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 18:31:15.186878 composio_core-0.1.83/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1134 2024-04-07 18:30:51.000000 composio_core-0.1.83/setup.py
```

### Comparing `composio_core-0.1.82/PKG-INFO` & `composio_core-0.1.83/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.82
+Version: 0.1.83
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.82/composio/composio_cli.py` & `composio_core-0.1.83/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.82/composio/sdk/core.py` & `composio_core-0.1.83/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.82/composio/sdk/enums.py` & `composio_core-0.1.83/composio/sdk/enums.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,130 +1,220 @@
 from enum import Enum
 
 class App(Enum):
+    GMAIL = "gmail"
+    ATTIO = "attio"
+    ZENDESK = "zendesk"
+    TODOIST = "todoist"
+    KLAVIYO = "klaviyo"
+    BITBUCKET = "bitbucket"
+    MONDAY = "monday"
+    SLACK = "slack"
     CLICKUP = "clickup"
-    GOOGLE_DRIVE = "google-drive"
+    DISCORD = "discord"
+    STRAVA = "strava"
+    DROPBOX = "dropbox"
+    INTERCOM = "intercom"
+    SHOPIFY = "shopify"
     GOOGLE_SHEETS = "google-sheets"
-    CALENDLY = "calendly"
-    ZENDESK = "zendesk"
     ASANA = "asana"
-    GITHUB = "github"
-    JIRA = "jira"
-    SLACK = "slack"
-    TRELLO = "trello"
-    GOOGLE_CALENDAR = "google-calendar"
-    GOOGLE_DOCS = "google-docs"
+    EVENTBRITE = "eventbrite"
     LINEAR = "linear"
+    HUBSPOT = "hubspot"
+    JIRA = "jira"
     NOTION = "notion"
-    DROPBOX = "dropbox"
+    TASKADE = "taskade"
+    GOOGLE_DRIVE = "google-drive"
+    GITLAB = "gitlab"
     MIXPANEL = "mixpanel"
-    MONDAY = "monday"
-    BITBUCKET = "bitbucket"
-    STRAVA = "strava"
-    INTERCOM = "intercom"
-    FIGMA = "figma"
-    KEAP = "keap"
-    KLAVIYO = "klaviyo"
-    MAILCHIMP = "mailchimp"
+    GOOGLE_DOCS = "google-docs"
     GUMROAD = "gumroad"
-    DISCORD = "discord"
+    MAILCHIMP = "mailchimp"
+    BOX = "box"
+    MIRO = "miro"
+    KEAP = "keap"
+    SPLITWISE = "splitwise"
+    PAGERDUTY = "pagerduty"
     ZOOM = "zoom"
-    TASKADE = "taskade"
-    TYPEFORM = "typeform"
     TIMELY = "timely"
-    TODOIST = "todoist"
-    TWITCH = "twitch"
-    BOX = "box"
     ZOHO = "zoho"
-    ATTIO = "attio"
-    SURVEY_MONKEY = "survey-monkey"
-    STACK_EXCHANGE = "stack-exchange"
-    PIPEDRIVE = "pipedrive"
-    PAGERDUTY = "pagerduty"
     FRESHDESK = "freshdesk"
-    HUBSPOT = "hubspot"
-    EVENTBRITE = "eventbrite"
-    GITLAB = "gitlab"
-    SHOPIFY = "shopify"
-    MIRO = "miro"
-    SPLITWISE = "splitwise"
+    FIGMA = "figma"
+    PIPEDRIVE = "pipedrive"
+    APIFY = "apify"
+    TWITCH = "twitch"
+    STACK_EXCHANGE = "stack-exchange"
+    GITHUB_OPEN_API_SPEC = "github_open_api_spec"
+    ACCELO = "accelo"
+    REDDIT = "reddit"
+    SURVEY_MONKEY = "survey-monkey"
+    TWITTER = "twitter"
+    XERO = "xero"
+    ZOHO_INVENTORY = "zoho_inventory"
+    ZOHO_MAIL = "zoho_mail"
+    AMAZON = "amazon"
+    SERVICEM8 = "servicem8"
+    SHORTCUT = "shortcut"
+    ZOHO_BOOKS = "zoho_books"
+    ZOHO_INVOICE = "zoho_invoice"
+    GORGIAS = "gorgias"
+    SALESFORCE = "salesforce"
+    SMUGMUG = "smugmug"
+    WAKATIME = "wakatime"
+    ZOHO_BIGIN = "zoho_bigin"
+    ZOHO_DESK = "zoho_desk"
+    HACKERRANK_WORK = "hackerrank-work"
+    BOLDSIGN = "boldsign"
+    GURU = "guru"
+    BAMBOOHR = "bamboohr"
+    HARVEST = "harvest"
+    ATLASSIAN = "atlassian"
+    DEEL = "deel"
+    FRONT = "front"
+    GITHUB = "github"
+    FRESHBOOKS = "freshbooks"
+    CALENDLY = "calendly"
+    TRELLO = "trello"
+    TYPEFORM = "typeform"
+    GOOGLE_CALENDAR = "google_calendar"
 
 class TestIntegration(Enum):
+    GMAIL = "test-gmail-connector"
+    ATTIO = "test-attio-connector"
+    ZENDESK = "test-zendesk-connector"
+    TODOIST = "test-todoist-connector"
+    KLAVIYO = "test-klaviyo-connector"
+    BITBUCKET = "test-bitbucket-connector"
+    MONDAY = "test-monday-connector"
+    SLACK = "test-slack-connector"
     CLICKUP = "test-clickup-connector"
-    GOOGLE_DRIVE = "test-google-drive-connector"
+    DISCORD = "test-discord-connector"
+    STRAVA = "test-strava-connector"
+    DROPBOX = "test-dropbox-connector"
+    INTERCOM = "test-intercom-connector"
+    SHOPIFY = "test-shopify-connector"
     GOOGLE_SHEETS = "test-google-sheets-connector"
-    CALENDLY = "test-calendly-connector"
-    ZENDESK = "test-zendesk-connector"
     ASANA = "test-asana-connector"
-    GITHUB = "test-github-connector"
-    JIRA = "test-jira-connector"
-    SLACK = "test-slack-connector"
-    TRELLO = "test-trello-connector"
-    GOOGLE_CALENDAR = "test-google-calendar-connector"
-    GOOGLE_DOCS = "test-google-docs-connector"
+    EVENTBRITE = "test-eventbrite-connector"
     LINEAR = "test-linear-connector"
+    HUBSPOT = "test-hubspot-connector"
+    JIRA = "test-jira-connector"
     NOTION = "test-notion-connector"
-    DROPBOX = "test-dropbox-connector"
+    TASKADE = "test-taskade-connector"
+    GOOGLE_DRIVE = "test-google-drive-connector"
+    GITLAB = "test-gitlab-connector"
     MIXPANEL = "test-mixpanel-connector"
-    MONDAY = "test-monday-connector"
-    BITBUCKET = "test-bitbucket-connector"
-    STRAVA = "test-strava-connector"
-    INTERCOM = "test-intercom-connector"
-    FIGMA = "test-figma-connector"
-    KEAP = "test-keap-connector"
-    KLAVIYO = "test-klaviyo-connector"
-    MAILCHIMP = "test-mailchimp-connector"
+    GOOGLE_DOCS = "test-google-docs-connector"
     GUMROAD = "test-gumroad-connector"
-    DISCORD = "test-discord-connector"
+    MAILCHIMP = "test-mailchimp-connector"
+    BOX = "test-box-connector"
+    MIRO = "test-miro-connector"
+    KEAP = "test-keap-connector"
+    SPLITWISE = "test-splitwise-connector"
+    PAGERDUTY = "test-pagerduty-connector"
     ZOOM = "test-zoom-connector"
-    TASKADE = "test-taskade-connector"
-    TYPEFORM = "test-typeform-connector"
     TIMELY = "test-timely-connector"
-    TODOIST = "test-todoist-connector"
-    TWITCH = "test-twitch-connector"
-    BOX = "test-box-connector"
     ZOHO = "test-zoho-connector"
-    ATTIO = "test-attio-connector"
-    SURVEY_MONKEY = "test-survey-monkey-connector"
-    STACK_EXCHANGE = "test-stack-exchange-connector"
-    PIPEDRIVE = "test-pipedrive-connector"
-    PAGERDUTY = "test-pagerduty-connector"
     FRESHDESK = "test-freshdesk-connector"
-    HUBSPOT = "test-hubspot-connector"
-    EVENTBRITE = "test-eventbrite-connector"
-    GITLAB = "test-gitlab-connector"
-    SHOPIFY = "test-shopify-connector"
-    MIRO = "test-miro-connector"
-    SPLITWISE = "test-splitwise-connector"
+    FIGMA = "test-figma-connector"
+    PIPEDRIVE = "test-pipedrive-connector"
+    APIFY = "test-apify-connector"
+    TWITCH = "test-twitch-connector"
+    STACK_EXCHANGE = "test-stack-exchange-connector"
+    GITHUB_OPEN_API_SPEC = "test-github_open_api_spec-connector"
+    ACCELO = "test-accelo-connector"
+    REDDIT = "test-reddit-connector"
+    SURVEY_MONKEY = "test-survey-monkey-connector"
+    TWITTER = "test-twitter-connector"
+    XERO = "test-xero-connector"
+    ZOHO_INVENTORY = "test-zoho_inventory-connector"
+    ZOHO_MAIL = "test-zoho_mail-connector"
+    AMAZON = "test-amazon-connector"
+    SERVICEM8 = "test-servicem8-connector"
+    SHORTCUT = "test-shortcut-connector"
+    ZOHO_BOOKS = "test-zoho_books-connector"
+    ZOHO_INVOICE = "test-zoho_invoice-connector"
+    GORGIAS = "test-gorgias-connector"
+    SALESFORCE = "test-salesforce-connector"
+    SMUGMUG = "test-smugmug-connector"
+    WAKATIME = "test-wakatime-connector"
+    ZOHO_BIGIN = "test-zoho_bigin-connector"
+    ZOHO_DESK = "test-zoho_desk-connector"
+    HACKERRANK_WORK = "test-hackerrank-work-connector"
+    BOLDSIGN = "test-boldsign-connector"
+    GURU = "test-guru-connector"
+    BAMBOOHR = "test-bamboohr-connector"
+    HARVEST = "test-harvest-connector"
+    ATLASSIAN = "test-atlassian-connector"
+    DEEL = "test-deel-connector"
+    FRONT = "test-front-connector"
+    GITHUB = "test-github-connector"
+    FRESHBOOKS = "test-freshbooks-connector"
+    CALENDLY = "test-calendly-connector"
+    TRELLO = "test-trello-connector"
+    TYPEFORM = "test-typeform-connector"
+    GOOGLE_CALENDAR = "test-google_calendar-connector"
 
 class Action(Enum):
     def __init__(self, service, action):
         self.service = service
         self.action = action
 
-    CLICKUP_CREATE_TASK = ("clickup", "clickup_create_task")
-    CLICKUP_GET_TASKS = ("clickup", "clickup_get_tasks")
-    CLICKUP_GET_TASK = ("clickup", "clickup_get_task")
-    CLICKUP_CREATE_LIST = ("clickup", "clickup_create_list")
-    CLICKUP_GET_LISTS = ("clickup", "clickup_get_lists")
-    CLICKUP_GET_SPACES = ("clickup", "clickup_get_spaces")
-    CLICKUP_CREATE_SPACE = ("clickup", "clickup_create_space")
-    CLICKUP_CREATE_FOLDER = ("clickup", "clickup_create_folder")
-    CLICKUP_GET_FOLDERS = ("clickup", "clickup_get_folders")
+    GMAIL_SEND_EMAIL = ("gmail", "gmail_send_email")
+    GMAIL_CREATE_EMAIL_DRAFT = ("gmail", "gmail_create_email_draft")
+    GMAIL_FIND_EMAIL_ID_IN_GMAIL = ("gmail", "gmail_find_email_id")
+    GMAIL_ADD_LABEL_TO_EMAIL = ("gmail", "gmail_add_label_to_email")
     ZENDESK_CREATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_create_zendesk_organization")
     ZENDESK_DELETE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_delete_zendesk_organization")
     ZENDESK_COUNT_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_count_zendesk_organizations")
     ZENDESK_GET_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_get_zendesk_organization")
     ZENDESK_GET_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_get_all_zendesk_organizations")
     ZENDESK_UPDATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_update_zendesk_organization")
     ZENDESK_CREATE_ZENDESK_TICKET = ("zendesk", "zendesk_create_zendesk_ticket")
     ZENDESK_DELETE_ZENDESK_TICKET = ("zendesk", "zendesk_delete_zendesk_ticket")
     ZENDESK_GET_ZENDESK_ABOUT_ME = ("zendesk", "zendesk_get_about_me")
+    SLACK_SEND_SLACK_MESSAGE = ("slack", "slack_send_slack_message")
+    SLACK_LIST_CHANNELS = ("slack", "slack_list_slack_channels")
+    SLACK_LIST_MEMBERS = ("slack", "slack_list_slack_members")
+    SLACK_LIST_MESSAGES = ("slack", "slack_list_slack_messages")
+    CLICKUP_CREATE_TASK = ("clickup", "clickup_create_task")
+    CLICKUP_GET_TASKS = ("clickup", "clickup_get_tasks")
+    CLICKUP_GET_TASK = ("clickup", "clickup_get_task")
+    CLICKUP_CREATE_LIST = ("clickup", "clickup_create_list")
+    CLICKUP_GET_LISTS = ("clickup", "clickup_get_lists")
+    CLICKUP_GET_SPACES = ("clickup", "clickup_get_spaces")
+    CLICKUP_CREATE_SPACE = ("clickup", "clickup_create_space")
+    CLICKUP_CREATE_FOLDER = ("clickup", "clickup_create_folder")
+    CLICKUP_GET_FOLDERS = ("clickup", "clickup_get_folders")
+    DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
     ASANA_CREATE_SUBTASK = ("asana", "asana_create_subtask")
     ASANA_GET_SUBTASKS = ("asana", "asana_get_subtasks")
+    LINEAR_CREATE_ISSUE = ("linear", "linear_create_linear_issue")
+    LINEAR_GET_PROJECTS = ("linear", "linear_list_linear_projects")
+    LINEAR_GET_TEAMS_BY_PROJECT = ("linear", "linear_list_linear_teams")
+    NOTION_GET_ABOUT_ME = ("notion", "notion_get_about_me")
+    NOTION_ADD_CONTENT_NOTION_PAGE = ("notion", "notion_add_notion_page_children")
+    NOTION_ARCHIVE_NOTION_PAGE = ("notion", "notion_archive_notion_page")
+    NOTION_CREATE_NOTION_DATABASE = ("notion", "notion_create_notion_database")
+    NOTION_CREATE_PAGE_COMMENT = ("notion", "notion_create_page_comment")
+    NOTION_CREATE_NOTION_PAGE = ("notion", "notion_create_notion_page")
+    NOTION_DELETE_BLOCKS = ("notion", "notion_delete_notion_page_children")
+    NOTION_FETCH_ALL_UNRESOLVED_COMMENTS = ("notion", "notion_fetch_notion_comment")
+    NOTION_FETCH_NOTION_DATABASE = ("notion", "notion_fetch_notion_database")
+    NOTION_FETCH_NOTION_PAGE = ("notion", "notion_fetch_notion_page")
+    NOTION_SEARCH_LIST_NOTION_PAGE = ("notion", "notion_search_notion_page")
+    NOTION_UPDATE_NOTION_DATABASE = ("notion", "notion_update_notion_database")
+    NOTION_FETCH_NOTION_BLOCKS = ("notion", "notion_fetch_notion_block")
+    NOTION_FETCH_NOTION_BLOCK_CHILDREN = ("notion", "notion_fetch_notion_child_block")
+    APIFY_GET_APIFY_ACTORS = ("apify", "apify_list_apify_actors")
+    APIFY_CREATE_APIFY_ACTOR = ("apify", "apify_create_apify_actor")
+    APIFY_GET_ACTOR_ID = ("apify", "apify_get_actor_id")
+    APIFY_SEARCH_APIFY_STORE = ("apify", "apify_search_store")
+    APIFY_GET_LAST_RUN_DATA = ("apify", "apify_get_last_run_data")
+    APIFY_GET_APIFY_TASKS = ("apify", "apify_list_apify_tasks")
     GITHUB_CREATE_ISSUE = ("github", "github_create_issue")
     GITHUB_GET_REPOSITORY = ("github", "github_list_github_repos")
     GITHUB_STAR_REPO = ("github", "github_star_repo")
     GITHUB_GET_ABOUT_ME = ("github", "github_get_about_me")
     GITHUB_FETCH_README = ("github", "github_fetch_readme")
     GITHUB_GET_COMMITS = ("github", "github_get_commits")
     GITHUB_GET_COMMITS_WITH_PATCH_FILE_FOR_THAT_COMMIT = ("github", "github_get_commits_with_code")
@@ -133,29 +223,20 @@
     TRELLO_CREATE_TRELLO_CARD = ("trello", "trello_create_trello_card")
     TRELLO_GET_TRELLO_BOARD_CARDS = ("trello", "trello_get_trello_board_cards")
     TRELLO_DELETE_TRELLO_CARD = ("trello", "trello_delete_trello_card")
     TRELLO_ADD_TRELLO_CARD_COMMENT = ("trello", "trello_add_trello_card_comment")
     TRELLO_CREATE_TRELLO_LABEL = ("trello", "trello_create_trello_label")
     TRELLO_UPDATE_TRELLO_BOARD = ("trello", "trello_update_trello_board")
     TRELLO_GET_ABOUT_ME = ("trello", "trello_get_about_me")
-    LINEAR_CREATE_ISSUE = ("linear", "linear_create_linear_issue")
-    LINEAR_GET_PROJECTS = ("linear", "linear_list_linear_projects")
-    LINEAR_GET_TEAMS_BY_PROJECT = ("linear", "linear_list_linear_teams")
-    NOTION_CREATE_NOTION_DATABASE = ("notion", "notion_create_notion_database")
-    NOTION_CREATE_NOTION_PAGE = ("notion", "notion_create_notion_page")
-    NOTION_FETCH_NOTION_PAGE = ("notion", "notion_fetch_notion_page")
-    NOTION_ARCHIVE_NOTION_PAGE = ("notion", "notion_archive_notion_page")
-    NOTION_FETCH_NOTION_DATABASE = ("notion", "notion_fetch_notion_database")
-    NOTION_UPDATE_NOTION_DATABASE = ("notion", "notion_update_notion_database")
-    NOTION_CREATE_PAGE_COMMENT = ("notion", "notion_create_page_comment")
-    NOTION_GET_ABOUT_ME = ("notion", "notion_get_about_me")
-    DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
+    TRELLO_SEARCH_TRELLO = ("trello", "trello_search_trello")
+    TRELLO_SEARCH_TRELLO_MEMBERS = ("trello", "trello_search_trello_member")
+    TRELLO_UPDATE_TRELLO_CARD = ("trello", "trello_update_trello_card")
     TYPEFORM_GET_ABOUT_ME = ("typeform", "typeform_get_about_me")
 
 class Trigger(Enum):
     def __init__(self, service, trigger):
         self.service = service
         self.trigger = trigger
 
+    SLACK_NEW_MESSAGE = ("slack", "slack_receive_message")
     GITHUB_PULL_REQUEST_EVENT = ("github", "github_pull_request_event")
     GITHUB_COMMIT_EVENT = ("github", "github_commit_event")
-    SLACK_NEW_MESSAGE = ("slack", "slack_receive_message")
```

### Comparing `composio_core-0.1.82/composio/sdk/sdk.py` & `composio_core-0.1.83/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.82/composio/sdk/storage.py` & `composio_core-0.1.83/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.82/composio/sdk/utils.py` & `composio_core-0.1.83/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.82/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.83/composio_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.82
+Version: 0.1.83
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.82/setup.py` & `composio_core-0.1.83/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.82",
+    version="0.1.83",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

