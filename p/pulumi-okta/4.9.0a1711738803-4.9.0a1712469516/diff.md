# Comparing `tmp/pulumi_okta-4.9.0a1711738803.tar.gz` & `tmp/pulumi_okta-4.9.0a1712469516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.9.0a1711738803.tar", last modified: Fri Mar 29 19:22:26 2024, max compression
+gzip compressed data, was "pulumi_okta-4.9.0a1712469516.tar", last modified: Sun Apr  7 06:00:59 2024, max compression
```

## Comparing `pulumi_okta-4.9.0a1711738803.tar` & `pulumi_okta-4.9.0a1712469516.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.096836 pulumi_okta-4.9.0a1711738803/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-29 19:22:26.096836 pulumi_okta-4.9.0a1711738803/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.076836 pulumi_okta-4.9.0a1711738803/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.084836 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/access_policy_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    64105 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    37151 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    40464 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    32406 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)   147306 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/oauth_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   138292 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    72919 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    59554 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)    67010 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    66199 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    91842 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    51059 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.084836 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23581 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    47955 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    47597 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20134 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24178 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.084836 pulumi_okta-4.9.0a1711738803/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18126 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.084836 pulumi_okta-4.9.0a1711738803/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.084836 pulumi_okta-4.9.0a1711738803/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24129 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    20949 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.088836 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (127)    90649 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    83512 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    72978 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.088836 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18671 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/customized_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/get_default_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/get_log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/get_org_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/index/preview_signin_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.092836 pulumi_okta-4.9.0a1711738803/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.092836 pulumi_okta-4.9.0a1711738803/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26479 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    35541 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    37606 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.092836 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16040 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_android.py
--rw-r--r--   0 runner    (1001) docker     (127)    46046 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_chromeos.py
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_ios.py
--rw-r--r--   0 runner    (1001) docker     (127)    55879 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_macos.py
--rw-r--r--   0 runner    (1001) docker     (127)    71271 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    69300 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    79741 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    30920 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    66504 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    65473 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    71555 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    35011 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.096836 pulumi_okta-4.9.0a1711738803/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23956 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.096836 pulumi_okta-4.9.0a1711738803/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.096836 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25722 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    99171 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    51854 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:22:26.096836 pulumi_okta-4.9.0a1711738803/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-29 19:22:26.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-03-29 19:22:26.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:22:26.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 19:22:26.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 19:22:26.000000 pulumi_okta-4.9.0a1711738803/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-29 19:22:19.000000 pulumi_okta-4.9.0a1711738803/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:22:26.096836 pulumi_okta-4.9.0a1711738803/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.273711 pulumi_okta-4.9.0a1712469516/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-07 06:00:59.273711 pulumi_okta-4.9.0a1712469516/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.249711 pulumi_okta-4.9.0a1712469516/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.257711 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/access_policy_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64105 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37151 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40464 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32406 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147044 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/oauth_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138292 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72919 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59554 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67010 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66199 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91388 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51059 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.257711 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23581 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47955 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47597 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20134 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24178 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.257711 pulumi_okta-4.9.0a1712469516/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18126 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.261711 pulumi_okta-4.9.0a1712469516/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.261711 pulumi_okta-4.9.0a1712469516/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24129 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20949 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.261711 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90649 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83512 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72978 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.265711 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18671 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/customized_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/get_default_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/get_log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/get_org_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/index/preview_signin_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.265711 pulumi_okta-4.9.0a1712469516/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.265711 pulumi_okta-4.9.0a1712469516/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26479 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35541 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37606 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.269711 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16040 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46046 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_chromeos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55879 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71271 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69300 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79741 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30920 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66504 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65473 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71555 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35011 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.269711 pulumi_okta-4.9.0a1712469516/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23956 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.269711 pulumi_okta-4.9.0a1712469516/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.273711 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25722 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99171 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51854 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:59.273711 pulumi_okta-4.9.0a1712469516/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-07 06:00:59.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-07 06:00:59.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:00:59.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 06:00:59.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 06:00:59.000000 pulumi_okta-4.9.0a1712469516/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-07 06:00:47.000000 pulumi_okta-4.9.0a1712469516/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:00:59.273711 pulumi_okta-4.9.0a1712469516/setup.cfg
```

### Comparing `pulumi_okta-4.9.0a1711738803/PKG-INFO` & `pulumi_okta-4.9.0a1712469516/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1711738803
+Version: 4.9.0a1712469516
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1711738803/README.md` & `pulumi_okta-4.9.0a1712469516/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/__init__.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/_inputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/_utilities.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/__init__.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/access_policy_assignment.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/access_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/get_app.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/get_oauth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/o_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1801,20 +1801,14 @@
         The operator either uploads their own private key or Okta can generate one in
         the Admin UI Panel under the apps Client Credentials. PKCS#8 format can be
         identified by a header that starts with `-----BEGIN PRIVATE KEY-----`. If the
         operator has a PKCS#1 (unencrypted) format private key (the header starts with
         `-----BEGIN RSA PRIVATE KEY-----`) they can generate a PKCS#8 format
         key with `openssl`:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         An OIDC Application can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/oAuth:OAuth example &#60;app id&#62;
         ```
@@ -1973,20 +1967,14 @@
         The operator either uploads their own private key or Okta can generate one in
         the Admin UI Panel under the apps Client Credentials. PKCS#8 format can be
         identified by a header that starts with `-----BEGIN PRIVATE KEY-----`. If the
         operator has a PKCS#1 (unencrypted) format private key (the header starts with
         `-----BEGIN RSA PRIVATE KEY-----`) they can generate a PKCS#8 format
         key with `openssl`:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         An OIDC Application can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/oAuth:OAuth example &#60;app id&#62;
         ```
```

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/oauth_role_assignment.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/oauth_role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/outputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/saml.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/swa.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/three_field.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app/user.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app_oauth_api_scope.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,20 +130,14 @@
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Manages API scopes for OAuth applications.
 
         This resource allows you to grant or revoke API scopes for OAuth2 applications within your organization.
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
@@ -178,20 +172,14 @@
                  args: AppOauthApiScopeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages API scopes for OAuth applications.
 
         This resource allows you to grant or revoke API scopes for OAuth2 applications within your organization.
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
```

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app_signon_policy_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -919,14 +919,16 @@
         test_app_signon_policy = okta.get_app_signon_policy_output(app_id=test_saml.id)
         test_app_signon_policy_rule = okta.AppSignonPolicyRule("testAppSignonPolicyRule", policy_id=test_app_signon_policy.id)
         ```
         <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
+        ### Rule with Constraints
+
         ### Example 1:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
@@ -939,20 +941,14 @@
                 },
             })])
         ```
         <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
         ### Example 2:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
@@ -970,20 +966,14 @@
                 },
             })])
         ```
         <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
         More examples can be
         found [here](https://developer.okta.com/docs/reference/api/policy/#verification-method-json-examples).
 
         ### Complex example
 
         <!--Start PulumiCodeChooser -->
         ```python
@@ -1231,14 +1221,16 @@
         test_app_signon_policy = okta.get_app_signon_policy_output(app_id=test_saml.id)
         test_app_signon_policy_rule = okta.AppSignonPolicyRule("testAppSignonPolicyRule", policy_id=test_app_signon_policy.id)
         ```
         <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
+        ### Rule with Constraints
+
         ### Example 1:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
@@ -1251,20 +1243,14 @@
                 },
             })])
         ```
         <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
         ### Example 2:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
@@ -1282,20 +1268,14 @@
                 },
             })])
         ```
         <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
         More examples can be
         found [here](https://developer.okta.com/docs/reference/api/policy/#verification-method-json-examples).
 
         ### Complex example
 
         <!--Start PulumiCodeChooser -->
         ```python
```

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/authenticator.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/behaviour.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/brand.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/captcha.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/config/__init__.pyi` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/config/vars.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/domain.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/domain_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,33 @@
         ...
         nUFLNE8pXSnsqb0eOL74f3uQ
         -----END PRIVATE KEY-----
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
+        ## Let's Encrypt Certbot
+
+        This example demonstrates generatoring a domain certificate with letsencrypt
+        certbot https://letsencrypt.org/getting-started/
+
+        Use letsencrypt's certbot to generate domain certificates in RSA output mode.
+        The generator's output corresponds to `DomainCertificate` fields in the
+        following manner.
+
+        Okta Field          | Certbot file
+        --------------------|--------------
+        `certificate`       | `cert.pem`
+        `certificate_chain` | `chain.pem`
+        `private_key`       | `privkey.pem`
+
+        ## Import
+
+        This resource does not support importing.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] certificate: Certificate content.
         :param pulumi.Input[str] certificate_chain: Certificate certificate chain.
         :param pulumi.Input[str] domain_id: Domain ID.
         :param pulumi.Input[str] private_key: Certificate private key.
         :param pulumi.Input[str] type: Certificate type. Valid value is `"PEM"`.
@@ -293,14 +312,33 @@
         ...
         nUFLNE8pXSnsqb0eOL74f3uQ
         -----END PRIVATE KEY-----
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
+        ## Let's Encrypt Certbot
+
+        This example demonstrates generatoring a domain certificate with letsencrypt
+        certbot https://letsencrypt.org/getting-started/
+
+        Use letsencrypt's certbot to generate domain certificates in RSA output mode.
+        The generator's output corresponds to `DomainCertificate` fields in the
+        following manner.
+
+        Okta Field          | Certbot file
+        --------------------|--------------
+        `certificate`       | `cert.pem`
+        `certificate_chain` | `chain.pem`
+        `private_key`       | `privkey.pem`
+
+        ## Import
+
+        This resource does not support importing.
+
         :param str resource_name: The name of the resource.
         :param DomainCertificateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(DomainCertificateArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/domain_verification.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/email_customization.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/email_sender.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/email_sender.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/email_sender_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/event_hook.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/factor/factor.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/factor_totp.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_app_user_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_brand.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_brands.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_groups.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_template.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_templates.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_theme.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_themes.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/group/get_group.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/group/get_rule.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/group/get_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/group/group.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/group/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/group/role.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/group/rule.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/group_memberships.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/saml.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/idp/social.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/__init__.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/_inputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/customized_signin_page.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/customized_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/email_domain.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/email_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/email_domain_verification.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/email_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/get_default_signin_page.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/get_default_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/get_log_stream.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/get_log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/get_org_metadata.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/get_org_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/log_stream.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/outputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/index/preview_signin_page.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/index/preview_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/inline/hook.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/link_definition.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/link_value.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/network/zone.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/org_configuration.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/org_support.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/outputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_android.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_android.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_chromeos.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_chromeos.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_ios.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_ios.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_macos.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_macos.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/device_assurance_windows.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/device_assurance_windows.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/password.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/rule_mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy/signon.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy/signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/provider.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/resource_set.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/role_subscription.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/template_sms.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/theme.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user/get_user.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user/get_users.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user/outputs.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user/user.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user/user_type.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user_admin_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.9.0a1712469516/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.9.0a1712469516/pulumi_okta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1711738803
+Version: 4.9.0a1712469516
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1711738803/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.9.0a1712469516/pulumi_okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

