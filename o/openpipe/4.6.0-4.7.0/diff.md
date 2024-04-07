# Comparing `tmp/openpipe-4.6.0.tar.gz` & `tmp/openpipe-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpipe-4.6.0.tar", max compression
+gzip compressed data, was "openpipe-4.7.0.tar", max compression
```

## Comparing `openpipe-4.6.0.tar` & `openpipe-4.7.0.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0     2552 2024-02-23 22:32:58.732064 openpipe-4.6.0/README.md
--rw-r--r--   0        0        0    11357 2024-02-23 22:32:58.732154 openpipe-4.6.0/openpipe/LICENSE
--rw-r--r--   0        0        0      227 2024-02-23 22:32:58.732195 openpipe-4.6.0/openpipe/__init__.py
--rw-r--r--   0        0        0    20971 2024-04-05 05:12:27.519005 openpipe-4.6.0/openpipe/api_client/__init__.py
--rw-r--r--   0        0        0    43145 2024-04-05 05:12:27.519383 openpipe-4.6.0/openpipe/api_client/client.py
--rw-r--r--   0        0        0      519 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/api_error.py
--rw-r--r--   0        0        0     1273 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      167 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/environment.py
--rw-r--r--   0        0        0    31788 2024-04-05 05:12:27.519869 openpipe-4.6.0/openpipe/api_client/types/__init__.py
--rw-r--r--   0        0        0      991 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/check_cache_response.py
--rw-r--r--   0        0        0      390 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_function_call.py
--rw-r--r--   0        0        0      900 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_function_call_name.py
--rw-r--r--   0        0        0      997 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_functions_item.py
--rw-r--r--   0        0        0     2338 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item.py
--rw-r--r--   0        0        0     1630 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant.py
--rw-r--r--   0        0        0      240 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_content.py
--rw-r--r--   0        0        0      970 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_function_call.py
--rw-r--r--   0        0        0     1246 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item.py
--rw-r--r--   0        0        0      945 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item_function.py
--rw-r--r--   0        0        0     1111 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function.py
--rw-r--r--   0        0        0      239 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function_content.py
--rw-r--r--   0        0        0      922 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_system.py
--rw-r--r--   0        0        0      942 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_tool.py
--rw-r--r--   0        0        0     1098 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user.py
--rw-r--r--   0        0        0      367 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content.py
--rw-r--r--   0        0        0     1257 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item.py
--rw-r--r--   0        0        0     1167 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url.py
--rw-r--r--   0        0        0     1221 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url.py
--rw-r--r--   0        0        0      849 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url_detail.py
--rw-r--r--   0        0        0      915 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_text.py
--rw-r--r--   0        0        0     2357 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload.py
--rw-r--r--   0        0        0      450 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call.py
--rw-r--r--   0        0        0      910 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call_name.py
--rw-r--r--   0        0        0     1007 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_functions_item.py
--rw-r--r--   0        0        0     2665 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item.py
--rw-r--r--   0        0        0     1736 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant.py
--rw-r--r--   0        0        0      250 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_content.py
--rw-r--r--   0        0        0      980 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_function_call.py
--rw-r--r--   0        0        0     1288 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item.py
--rw-r--r--   0        0        0      955 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item_function.py
--rw-r--r--   0        0        0     1153 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function.py
--rw-r--r--   0        0        0      249 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function_content.py
--rw-r--r--   0        0        0      932 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_system.py
--rw-r--r--   0        0        0      952 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_tool.py
--rw-r--r--   0        0        0     1140 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user.py
--rw-r--r--   0        0        0      409 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content.py
--rw-r--r--   0        0        0     1371 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item.py
--rw-r--r--   0        0        0     1209 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url.py
--rw-r--r--   0        0        0     1263 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url.py
--rw-r--r--   0        0        0      889 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url_detail.py
--rw-r--r--   0        0        0      925 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_text.py
--rw-r--r--   0        0        0     1102 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format.py
--rw-r--r--   0        0        0      604 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format_type.py
--rw-r--r--   0        0        0      454 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice.py
--rw-r--r--   0        0        0     1243 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function.py
--rw-r--r--   0        0        0      920 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function_function.py
--rw-r--r--   0        0        0     1172 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item.py
--rw-r--r--   0        0        0     1011 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item_function.py
--rw-r--r--   0        0        0     1068 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_response_format.py
--rw-r--r--   0        0        0      574 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_response_format_type.py
--rw-r--r--   0        0        0      394 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice.py
--rw-r--r--   0        0        0     1201 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function.py
--rw-r--r--   0        0        0      910 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function_function.py
--rw-r--r--   0        0        0     1121 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tools_item.py
--rw-r--r--   0        0        0     1001 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tools_item_function.py
--rw-r--r--   0        0        0      280 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response.py
--rw-r--r--   0        0        0     1362 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices.py
--rw-r--r--   0        0        0     1561 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item.py
--rw-r--r--   0        0        0     1263 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_finish_reason.py
--rw-r--r--   0        0        0     1169 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs.py
--rw-r--r--   0        0        0     1297 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item.py
--rw-r--r--   0        0        0     1004 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item_top_logprobs_item.py
--rw-r--r--   0        0        0     1758 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message.py
--rw-r--r--   0        0        0      245 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_content.py
--rw-r--r--   0        0        0      975 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_function_call.py
--rw-r--r--   0        0        0     1267 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item.py
--rw-r--r--   0        0        0      950 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item_function.py
--rw-r--r--   0        0        0      961 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_usage.py
--rw-r--r--   0        0        0     1422 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/local_testing_only_get_latest_logged_call_response.py
--rw-r--r--   0        0        0      392 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload.py
--rw-r--r--   0        0        0     1516 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one.py
--rw-r--r--   0        0        0     1294 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item.py
--rw-r--r--   0        0        0      384 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content.py
--rw-r--r--   0        0        0     1283 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item.py
--rw-r--r--   0        0        0     1161 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image.py
--rw-r--r--   0        0        0     1303 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source.py
--rw-r--r--   0        0        0     1165 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source_media_type.py
--rw-r--r--   0        0        0      919 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_text.py
--rw-r--r--   0        0        0      582 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_role.py
--rw-r--r--   0        0        0     1087 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_metadata.py
--rw-r--r--   0        0        0      234 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_metadata_user_id.py
--rw-r--r--   0        0        0     1506 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero.py
--rw-r--r--   0        0        0     1301 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item.py
--rw-r--r--   0        0        0      388 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content.py
--rw-r--r--   0        0        0     1294 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item.py
--rw-r--r--   0        0        0     1165 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image.py
--rw-r--r--   0        0        0     1307 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source.py
--rw-r--r--   0        0        0     1170 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source_media_type.py
--rw-r--r--   0        0        0      920 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_text.py
--rw-r--r--   0        0        0      585 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_role.py
--rw-r--r--   0        0        0     1100 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_metadata.py
--rw-r--r--   0        0        0      235 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_metadata_user_id.py
--rw-r--r--   0        0        0     1746 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload.py
--rw-r--r--   0        0        0      971 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_content_item.py
--rw-r--r--   0        0        0      360 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_stop_reason.py
--rw-r--r--   0        0        0      224 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_stop_sequence.py
--rw-r--r--   0        0        0      930 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_usage.py
--rw-r--r--   0        0        0      223 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_tags_value.py
--rw-r--r--   0        0        0      984 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_response.py
--rw-r--r--   0        0        0      486 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_response_status.py
--rw-r--r--   0        0        0      214 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_request_tags_value.py
--rw-r--r--   0        0        0      947 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_response.py
--rw-r--r--   0        0        0      459 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_response_status.py
--rw-r--r--   0        0        0      974 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_create_response.py
--rw-r--r--   0        0        0     2506 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item.py
--rw-r--r--   0        0        0      479 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call.py
--rw-r--r--   0        0        0      917 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call_name.py
--rw-r--r--   0        0        0     1014 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_functions_item.py
--rw-r--r--   0        0        0     2870 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item.py
--rw-r--r--   0        0        0     1823 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant.py
--rw-r--r--   0        0        0      257 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_content.py
--rw-r--r--   0        0        0      987 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_function_call.py
--rw-r--r--   0        0        0     1317 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item.py
--rw-r--r--   0        0        0      962 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item_function.py
--rw-r--r--   0        0        0     1182 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function.py
--rw-r--r--   0        0        0      256 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function_content.py
--rw-r--r--   0        0        0      939 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_system.py
--rw-r--r--   0        0        0      959 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_tool.py
--rw-r--r--   0        0        0     1169 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user.py
--rw-r--r--   0        0        0      438 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content.py
--rw-r--r--   0        0        0     1450 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item.py
--rw-r--r--   0        0        0     1238 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url.py
--rw-r--r--   0        0        0     1306 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url.py
--rw-r--r--   0        0        0      917 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url_detail.py
--rw-r--r--   0        0        0      932 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_text.py
--rw-r--r--   0        0        0     1131 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format.py
--rw-r--r--   0        0        0      625 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format_type.py
--rw-r--r--   0        0        0      556 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_split.py
--rw-r--r--   0        0        0      483 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice.py
--rw-r--r--   0        0        0     1272 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function.py
--rw-r--r--   0        0        0      927 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function_function.py
--rw-r--r--   0        0        0     1201 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item.py
--rw-r--r--   0        0        0     1018 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item_function.py
--rw-r--r--   0        0        0     1170 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_response.py
--rw-r--r--   0        0        0      921 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_response_errors_item.py
--rw-r--r--   0        0        0     1133 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_create_request_base_model.py
--rw-r--r--   0        0        0      885 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_create_response.py
--rw-r--r--   0        0        0      890 2024-04-05 05:12:27.520179 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_delete_response.py
--rw-r--r--   0        0        0     1320 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_get_response.py
--rw-r--r--   0        0        0     1311 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_get_response_status.py
--rw-r--r--   0        0        0     1180 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/update_log_tags_request_filters_item.py
--rw-r--r--   0        0        0      151 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/update_log_tags_request_filters_item_equals.py
--rw-r--r--   0        0        0      221 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/update_log_tags_request_tags_value.py
--rw-r--r--   0        0        0      972 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/update_log_tags_response.py
--rw-r--r--   0        0        0     5963 2024-02-23 22:32:58.739376 openpipe-4.6.0/openpipe/client.py
--rw-r--r--   0        0        0     3074 2024-02-23 22:32:58.739440 openpipe-4.6.0/openpipe/langchain_llm.py
--rw-r--r--   0        0        0     3790 2024-02-23 22:32:58.739498 openpipe-4.6.0/openpipe/merge_openai_chunks.py
--rw-r--r--   0        0        0     7848 2024-04-05 05:24:04.792247 openpipe-4.6.0/openpipe/openai_async_wrapper.py
--rw-r--r--   0        0        0     7018 2024-02-23 22:32:58.739663 openpipe-4.6.0/openpipe/openai_sync_wrapper.py
--rw-r--r--   0        0        0     4629 2024-02-23 22:32:58.739734 openpipe-4.6.0/openpipe/shared.py
--rw-r--r--   0        0        0    15825 2024-04-05 17:59:18.064759 openpipe-4.6.0/openpipe/test_async_client.py
--rw-r--r--   0        0        0     4173 2024-02-23 22:32:58.740012 openpipe-4.6.0/openpipe/test_async_reporting.py
--rw-r--r--   0        0        0    13251 2024-02-23 22:32:58.740141 openpipe-4.6.0/openpipe/test_async_update_logged_call_tags.py
--rw-r--r--   0        0        0     1101 2024-02-23 22:32:58.740196 openpipe-4.6.0/openpipe/test_config.py
--rw-r--r--   0        0        0    13366 2024-04-05 17:59:18.066602 openpipe-4.6.0/openpipe/test_sync_client.py
--rw-r--r--   0        0        0     3765 2024-02-23 22:32:58.740380 openpipe-4.6.0/openpipe/test_sync_reporting.py
--rw-r--r--   0        0        0    12697 2024-02-23 22:32:58.740500 openpipe-4.6.0/openpipe/test_sync_update_logged_call_tags.py
--rw-r--r--   0        0        0      842 2024-04-05 17:59:18.068750 openpipe-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     3440 1970-01-01 00:00:00.000000 openpipe-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2552 2024-02-23 22:32:58.732064 openpipe-4.7.0/README.md
+-rw-r--r--   0        0        0    11357 2024-02-23 22:32:58.732154 openpipe-4.7.0/openpipe/LICENSE
+-rw-r--r--   0        0        0      227 2024-02-23 22:32:58.732195 openpipe-4.7.0/openpipe/__init__.py
+-rw-r--r--   0        0        0    20971 2024-04-05 05:12:27.519005 openpipe-4.7.0/openpipe/api_client/__init__.py
+-rw-r--r--   0        0        0    43145 2024-04-05 05:12:27.519383 openpipe-4.7.0/openpipe/api_client/client.py
+-rw-r--r--   0        0        0      519 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/core/api_error.py
+-rw-r--r--   0        0        0     1273 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      167 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/environment.py
+-rw-r--r--   0        0        0    31788 2024-04-05 05:12:27.519869 openpipe-4.7.0/openpipe/api_client/types/__init__.py
+-rw-r--r--   0        0        0      991 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/check_cache_response.py
+-rw-r--r--   0        0        0      390 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_function_call.py
+-rw-r--r--   0        0        0      900 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_function_call_name.py
+-rw-r--r--   0        0        0      997 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_functions_item.py
+-rw-r--r--   0        0        0     2338 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item.py
+-rw-r--r--   0        0        0     1630 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant.py
+-rw-r--r--   0        0        0      240 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_content.py
+-rw-r--r--   0        0        0      970 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_function_call.py
+-rw-r--r--   0        0        0     1246 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item.py
+-rw-r--r--   0        0        0      945 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item_function.py
+-rw-r--r--   0        0        0     1111 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function.py
+-rw-r--r--   0        0        0      239 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function_content.py
+-rw-r--r--   0        0        0      922 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_system.py
+-rw-r--r--   0        0        0      942 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_tool.py
+-rw-r--r--   0        0        0     1098 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user.py
+-rw-r--r--   0        0        0      367 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content.py
+-rw-r--r--   0        0        0     1257 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item.py
+-rw-r--r--   0        0        0     1167 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url.py
+-rw-r--r--   0        0        0     1221 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url.py
+-rw-r--r--   0        0        0      849 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url_detail.py
+-rw-r--r--   0        0        0      915 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_text.py
+-rw-r--r--   0        0        0     2357 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload.py
+-rw-r--r--   0        0        0      450 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call.py
+-rw-r--r--   0        0        0      910 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call_name.py
+-rw-r--r--   0        0        0     1007 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_functions_item.py
+-rw-r--r--   0        0        0     2665 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item.py
+-rw-r--r--   0        0        0     1736 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant.py
+-rw-r--r--   0        0        0      250 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_content.py
+-rw-r--r--   0        0        0      980 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_function_call.py
+-rw-r--r--   0        0        0     1288 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item.py
+-rw-r--r--   0        0        0      955 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item_function.py
+-rw-r--r--   0        0        0     1153 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function.py
+-rw-r--r--   0        0        0      249 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function_content.py
+-rw-r--r--   0        0        0      932 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_system.py
+-rw-r--r--   0        0        0      952 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_tool.py
+-rw-r--r--   0        0        0     1140 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user.py
+-rw-r--r--   0        0        0      409 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content.py
+-rw-r--r--   0        0        0     1371 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item.py
+-rw-r--r--   0        0        0     1209 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url.py
+-rw-r--r--   0        0        0     1263 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url.py
+-rw-r--r--   0        0        0      889 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url_detail.py
+-rw-r--r--   0        0        0      925 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_text.py
+-rw-r--r--   0        0        0     1102 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format.py
+-rw-r--r--   0        0        0      604 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format_type.py
+-rw-r--r--   0        0        0      454 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice.py
+-rw-r--r--   0        0        0     1243 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function.py
+-rw-r--r--   0        0        0      920 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function_function.py
+-rw-r--r--   0        0        0     1172 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item.py
+-rw-r--r--   0        0        0     1011 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item_function.py
+-rw-r--r--   0        0        0     1068 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_response_format.py
+-rw-r--r--   0        0        0      574 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_response_format_type.py
+-rw-r--r--   0        0        0      394 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tool_choice.py
+-rw-r--r--   0        0        0     1201 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function.py
+-rw-r--r--   0        0        0      910 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function_function.py
+-rw-r--r--   0        0        0     1121 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tools_item.py
+-rw-r--r--   0        0        0     1001 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tools_item_function.py
+-rw-r--r--   0        0        0      280 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response.py
+-rw-r--r--   0        0        0     1362 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices.py
+-rw-r--r--   0        0        0     1561 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item.py
+-rw-r--r--   0        0        0     1263 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_finish_reason.py
+-rw-r--r--   0        0        0     1169 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs.py
+-rw-r--r--   0        0        0     1297 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item.py
+-rw-r--r--   0        0        0     1004 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item_top_logprobs_item.py
+-rw-r--r--   0        0        0     1758 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message.py
+-rw-r--r--   0        0        0      245 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_content.py
+-rw-r--r--   0        0        0      975 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_function_call.py
+-rw-r--r--   0        0        0     1267 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item.py
+-rw-r--r--   0        0        0      950 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item_function.py
+-rw-r--r--   0        0        0      961 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_usage.py
+-rw-r--r--   0        0        0     1422 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/local_testing_only_get_latest_logged_call_response.py
+-rw-r--r--   0        0        0      392 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload.py
+-rw-r--r--   0        0        0     1516 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one.py
+-rw-r--r--   0        0        0     1294 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item.py
+-rw-r--r--   0        0        0      384 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content.py
+-rw-r--r--   0        0        0     1283 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item.py
+-rw-r--r--   0        0        0     1161 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image.py
+-rw-r--r--   0        0        0     1303 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source.py
+-rw-r--r--   0        0        0     1165 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source_media_type.py
+-rw-r--r--   0        0        0      919 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_text.py
+-rw-r--r--   0        0        0      582 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_role.py
+-rw-r--r--   0        0        0     1087 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_metadata.py
+-rw-r--r--   0        0        0      234 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_metadata_user_id.py
+-rw-r--r--   0        0        0     1506 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero.py
+-rw-r--r--   0        0        0     1301 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item.py
+-rw-r--r--   0        0        0      388 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content.py
+-rw-r--r--   0        0        0     1294 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item.py
+-rw-r--r--   0        0        0     1165 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image.py
+-rw-r--r--   0        0        0     1307 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source.py
+-rw-r--r--   0        0        0     1170 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source_media_type.py
+-rw-r--r--   0        0        0      920 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_text.py
+-rw-r--r--   0        0        0      585 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_role.py
+-rw-r--r--   0        0        0     1100 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_metadata.py
+-rw-r--r--   0        0        0      235 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_metadata_user_id.py
+-rw-r--r--   0        0        0     1746 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_resp_payload.py
+-rw-r--r--   0        0        0      971 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_resp_payload_content_item.py
+-rw-r--r--   0        0        0      360 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_resp_payload_stop_reason.py
+-rw-r--r--   0        0        0      224 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_resp_payload_stop_sequence.py
+-rw-r--r--   0        0        0      930 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_resp_payload_usage.py
+-rw-r--r--   0        0        0      223 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_tags_value.py
+-rw-r--r--   0        0        0      984 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_response.py
+-rw-r--r--   0        0        0      486 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_anthropic_response_status.py
+-rw-r--r--   0        0        0      214 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_request_tags_value.py
+-rw-r--r--   0        0        0      947 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_response.py
+-rw-r--r--   0        0        0      459 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/report_response_status.py
+-rw-r--r--   0        0        0      974 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_create_response.py
+-rw-r--r--   0        0        0     2506 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item.py
+-rw-r--r--   0        0        0      479 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call.py
+-rw-r--r--   0        0        0      917 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call_name.py
+-rw-r--r--   0        0        0     1014 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_functions_item.py
+-rw-r--r--   0        0        0     2870 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item.py
+-rw-r--r--   0        0        0     1823 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant.py
+-rw-r--r--   0        0        0      257 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_content.py
+-rw-r--r--   0        0        0      987 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_function_call.py
+-rw-r--r--   0        0        0     1317 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item.py
+-rw-r--r--   0        0        0      962 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item_function.py
+-rw-r--r--   0        0        0     1182 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function.py
+-rw-r--r--   0        0        0      256 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function_content.py
+-rw-r--r--   0        0        0      939 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_system.py
+-rw-r--r--   0        0        0      959 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_tool.py
+-rw-r--r--   0        0        0     1169 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user.py
+-rw-r--r--   0        0        0      438 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content.py
+-rw-r--r--   0        0        0     1450 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item.py
+-rw-r--r--   0        0        0     1238 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url.py
+-rw-r--r--   0        0        0     1306 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url.py
+-rw-r--r--   0        0        0      917 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url_detail.py
+-rw-r--r--   0        0        0      932 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_text.py
+-rw-r--r--   0        0        0     1131 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format.py
+-rw-r--r--   0        0        0      625 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format_type.py
+-rw-r--r--   0        0        0      556 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_split.py
+-rw-r--r--   0        0        0      483 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice.py
+-rw-r--r--   0        0        0     1272 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function.py
+-rw-r--r--   0        0        0      927 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function_function.py
+-rw-r--r--   0        0        0     1201 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item.py
+-rw-r--r--   0        0        0     1018 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item_function.py
+-rw-r--r--   0        0        0     1170 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_response.py
+-rw-r--r--   0        0        0      921 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_response_errors_item.py
+-rw-r--r--   0        0        0     1133 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_create_request_base_model.py
+-rw-r--r--   0        0        0      885 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_create_response.py
+-rw-r--r--   0        0        0      890 2024-04-05 05:12:27.520179 openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_delete_response.py
+-rw-r--r--   0        0        0     1320 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_get_response.py
+-rw-r--r--   0        0        0     1311 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_get_response_status.py
+-rw-r--r--   0        0        0     1180 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/update_log_tags_request_filters_item.py
+-rw-r--r--   0        0        0      151 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/update_log_tags_request_filters_item_equals.py
+-rw-r--r--   0        0        0      221 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/update_log_tags_request_tags_value.py
+-rw-r--r--   0        0        0      972 2024-04-05 01:17:30.000000 openpipe-4.7.0/openpipe/api_client/types/update_log_tags_response.py
+-rw-r--r--   0        0        0     7636 2024-04-07 05:43:35.909376 openpipe-4.7.0/openpipe/client.py
+-rw-r--r--   0        0        0     3074 2024-02-23 22:32:58.739440 openpipe-4.7.0/openpipe/langchain_llm.py
+-rw-r--r--   0        0        0     3790 2024-02-23 22:32:58.739498 openpipe-4.7.0/openpipe/merge_openai_chunks.py
+-rw-r--r--   0        0        0     7848 2024-04-05 05:24:04.792247 openpipe-4.7.0/openpipe/openai_async_wrapper.py
+-rw-r--r--   0        0        0     7018 2024-02-23 22:32:58.739663 openpipe-4.7.0/openpipe/openai_sync_wrapper.py
+-rw-r--r--   0        0        0     4629 2024-02-23 22:32:58.739734 openpipe-4.7.0/openpipe/shared.py
+-rw-r--r--   0        0        0    15825 2024-04-05 17:59:18.064759 openpipe-4.7.0/openpipe/test_async_client.py
+-rw-r--r--   0        0        0     5126 2024-04-07 05:43:35.909887 openpipe-4.7.0/openpipe/test_async_reporting.py
+-rw-r--r--   0        0        0    13251 2024-02-23 22:32:58.740141 openpipe-4.7.0/openpipe/test_async_update_logged_call_tags.py
+-rw-r--r--   0        0        0     1101 2024-02-23 22:32:58.740196 openpipe-4.7.0/openpipe/test_config.py
+-rw-r--r--   0        0        0    13366 2024-04-05 17:59:18.066602 openpipe-4.7.0/openpipe/test_sync_client.py
+-rw-r--r--   0        0        0     4675 2024-04-07 05:43:35.910295 openpipe-4.7.0/openpipe/test_sync_reporting.py
+-rw-r--r--   0        0        0    12697 2024-02-23 22:32:58.740500 openpipe-4.7.0/openpipe/test_sync_update_logged_call_tags.py
+-rw-r--r--   0        0        0      830 2024-04-07 05:45:04.917966 openpipe-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 openpipe-4.7.0/PKG-INFO
```

### Comparing `openpipe-4.6.0/README.md` & `openpipe-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/LICENSE` & `openpipe-4.7.0/openpipe/LICENSE`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/__init__.py` & `openpipe-4.7.0/openpipe/api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/client.py` & `openpipe-4.7.0/openpipe/api_client/client.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/core/__init__.py` & `openpipe-4.7.0/openpipe/api_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/core/client_wrapper.py` & `openpipe-4.7.0/openpipe/api_client/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/core/datetime_utils.py` & `openpipe-4.7.0/openpipe/api_client/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/core/jsonable_encoder.py` & `openpipe-4.7.0/openpipe/api_client/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/__init__.py` & `openpipe-4.7.0/openpipe/api_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/check_cache_response.py` & `openpipe-4.7.0/openpipe/api_client/types/check_cache_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_function_call_name.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_function_call_name.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_functions_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_functions_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_function_call.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_function_call.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_system.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_system.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_tool.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_tool.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url_detail.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url_detail.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_text.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_text.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call_name.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call_name.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_functions_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_functions_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_function_call.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_function_call.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_system.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_system.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_tool.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_tool.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url_detail.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url_detail.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_text.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_text.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format_type.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format_type.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_response_format.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_response_format.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_response_format_type.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_response_format_type.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tools_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tools_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tools_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_request_tools_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_finish_reason.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_finish_reason.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item_top_logprobs_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item_top_logprobs_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_function_call.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_function_call.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_usage.py` & `openpipe-4.7.0/openpipe/api_client/types/create_chat_completion_response_choices_usage.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/local_testing_only_get_latest_logged_call_response.py` & `openpipe-4.7.0/openpipe/api_client/types/local_testing_only_get_latest_logged_call_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source_media_type.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source_media_type.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_text.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_text.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_role.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_role.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_metadata.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_metadata.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source_media_type.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source_media_type.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_text.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_text.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_role.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_role.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_metadata.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_metadata.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_resp_payload.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_content_item.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_resp_payload_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_usage.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_request_resp_payload_usage.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_anthropic_response.py` & `openpipe-4.7.0/openpipe/api_client/types/report_anthropic_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/report_response.py` & `openpipe-4.7.0/openpipe/api_client/types/report_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_create_response.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_create_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call_name.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call_name.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_functions_item.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_functions_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_function_call.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_function_call.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_system.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_system.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_tool.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_tool.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url_detail.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url_detail.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_text.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_text.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format_type.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format_type.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_split.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_split.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function_function.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item_function.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_response.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_response_errors_item.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_dataset_entry_create_response_errors_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_create_request_base_model.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_create_request_base_model.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_create_response.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_create_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_delete_response.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_delete_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_get_response.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_get_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_get_response_status.py` & `openpipe-4.7.0/openpipe/api_client/types/unstable_finetune_get_response_status.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/update_log_tags_request_filters_item.py` & `openpipe-4.7.0/openpipe/api_client/types/update_log_tags_request_filters_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/api_client/types/update_log_tags_response.py` & `openpipe-4.7.0/openpipe/api_client/types/update_log_tags_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/client.py` & `openpipe-4.7.0/openpipe/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from importlib.metadata import version
 
 from .api_client.client import (
     OpenPipeApi,
     AsyncOpenPipeApi,
     ReportResponse,
     ReportRequestTagsValue,
+    ReportAnthropicResponse,
     UpdateLogTagsRequestFiltersItem,
     UpdateLogTagsRequestTagsValue,
     UpdateLogTagsResponse,
 )
 
 OMIT = typing.cast(typing.Any, ...)
 
@@ -87,14 +88,35 @@
             req_payload=req_payload,
             resp_payload=resp_payload,
             status_code=status_code,
             error_message=error_message,
             tags=add_sdk_info(tags),
         )
 
+    def report_anthropic(
+        self, 
+        *,
+        requested_at: typing.Optional[float] = OMIT,
+        received_at: typing.Optional[float] = OMIT,
+        req_payload: typing.Optional[typing.Any] = OMIT,
+        resp_payload: typing.Optional[typing.Any] = OMIT,
+        status_code: typing.Optional[float] = OMIT,
+        error_message: typing.Optional[str] = OMIT,
+        tags: typing.Optional[typing.Dict[str, ReportRequestTagsValue]] = {},
+    ) -> ReportAnthropicResponse:
+        return self.base_client.report_anthropic(
+            requested_at=requested_at,
+            received_at=received_at,
+            req_payload=req_payload,
+            resp_payload=resp_payload,
+            status_code=status_code,
+            error_message=error_message,
+            tags=add_sdk_info(tags),
+        )
+
     def update_log_tags(
         self,
         *,
         filters: typing.List[UpdateLogTagsRequestFiltersItem],
         tags: typing.Dict[str, UpdateLogTagsRequestTagsValue],
     ) -> UpdateLogTagsResponse:
         return self.base_client.update_log_tags(filters=filters, tags=tags)
@@ -162,14 +184,35 @@
             requested_at=requested_at,
             received_at=received_at,
             req_payload=req_payload,
             resp_payload=resp_payload,
             status_code=status_code,
             error_message=error_message,
             tags=add_sdk_info(tags),
+        )
+
+    async def report_anthropic(
+        self, 
+        *,
+        requested_at: typing.Optional[float] = OMIT,
+        received_at: typing.Optional[float] = OMIT,
+        req_payload: typing.Optional[typing.Any] = OMIT,
+        resp_payload: typing.Optional[typing.Any] = OMIT,
+        status_code: typing.Optional[float] = OMIT,
+        error_message: typing.Optional[str] = OMIT,
+        tags: typing.Optional[typing.Dict[str, ReportRequestTagsValue]] = {},
+    ) -> ReportAnthropicResponse:
+        return await self.base_client.report_anthropic(
+            requested_at=requested_at,
+            received_at=received_at,
+            req_payload=req_payload,
+            resp_payload=resp_payload,
+            status_code=status_code,
+            error_message=error_message,
+            tags=add_sdk_info(tags),
         )
 
     async def update_log_tags(
         self,
         *,
         filters: typing.List[UpdateLogTagsRequestFiltersItem],
         tags: typing.Dict[str, UpdateLogTagsRequestTagsValue],
```

### Comparing `openpipe-4.6.0/openpipe/langchain_llm.py` & `openpipe-4.7.0/openpipe/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/merge_openai_chunks.py` & `openpipe-4.7.0/openpipe/merge_openai_chunks.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/openai_async_wrapper.py` & `openpipe-4.7.0/openpipe/openai_async_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/openai_sync_wrapper.py` & `openpipe-4.7.0/openpipe/openai_sync_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/shared.py` & `openpipe-4.7.0/openpipe/shared.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/test_async_client.py` & `openpipe-4.7.0/openpipe/test_async_client.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/test_async_reporting.py` & `openpipe-4.7.0/openpipe/test_async_reporting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from functools import reduce
 import pytest
 from dotenv import load_dotenv
 import asyncio
 import time
+from anthropic import AsyncAnthropic
 
 from . import AsyncOpenAI
 from .client import AsyncOpenPipe
 from .test_config import TEST_LAST_LOGGED, OPENPIPE_BASE_URL, OPENPIPE_API_KEY
 
 load_dotenv()
 
 client = AsyncOpenAI()
 op_client = AsyncOpenPipe(api_key=OPENPIPE_API_KEY, base_url=OPENPIPE_BASE_URL)
-
+anthropic_client = AsyncAnthropic()
 
 async def last_logged_call():
     return await op_client.base_client.local_testing_only_get_latest_logged_call()
 
 
 @pytest.fixture(autouse=True)
 def setup():
@@ -139,7 +140,36 @@
     last_logged = await last_logged_call()
     assert last_logged.req_payload["messages"][0]["content"] == "count to 3"
     assert last_logged.resp_payload == None
     assert last_logged.tags["promptId"] == "test_async_reports_unusual_tags"
     assert last_logged.tags["numberTag"] == "1"
     assert last_logged.tags["booleanTag"] == "true"
     assert last_logged.tags.get("nullTag") == None
+
+async def test_async_report_anthropic():
+    payload = {
+        "model": "claude-3-opus-20240229",
+        "messages": [{"role": "user", "content": "Hello, Claude"}],
+        "max_tokens": 100,
+    }
+
+    completion = await anthropic_client.messages.create(**payload)
+
+    await op_client.report_anthropic(
+        requested_at=int(time.time() * 1000 - 1050),
+        received_at=int(time.time() * 1000),
+        req_payload=payload,
+        resp_payload=completion,
+        status_code=200,
+        tags={"promptId": "test_async_report_anthropic"},
+    )
+
+    if not TEST_LAST_LOGGED:
+        return
+
+    await asyncio.sleep(0.1)
+    last_logged = await last_logged_call()
+    assert last_logged.req_payload["messages"][0]["content"] == "Hello, Claude"
+    assert (
+        last_logged.resp_payload["choices"][0]["message"]["content"]
+        == completion.content[0].text
+    )
```

### Comparing `openpipe-4.6.0/openpipe/test_async_update_logged_call_tags.py` & `openpipe-4.7.0/openpipe/test_async_update_logged_call_tags.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/test_config.py` & `openpipe-4.7.0/openpipe/test_config.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/test_sync_client.py` & `openpipe-4.7.0/openpipe/test_sync_client.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/openpipe/test_sync_reporting.py` & `openpipe-4.7.0/openpipe/test_sync_reporting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from functools import reduce
 import pytest
 from dotenv import load_dotenv
 import time
+from anthropic import Anthropic
 
 from . import OpenAI
 from .client import OpenPipe
 from .test_config import TEST_LAST_LOGGED, OPENPIPE_BASE_URL, OPENPIPE_API_KEY
 
 load_dotenv()
 
 client = OpenAI()
 op_client = OpenPipe(api_key=OPENPIPE_API_KEY, base_url=OPENPIPE_BASE_URL)
+anthropic_client = Anthropic()
 
 
 def last_logged_call():
     return op_client.base_client.local_testing_only_get_latest_logged_call()
 
 
 def test_sync_reports_valid_response_payload():
@@ -129,7 +131,36 @@
     last_logged = last_logged_call()
     assert last_logged.req_payload["messages"][0]["content"] == "count to 3"
     assert last_logged.resp_payload == None
     assert last_logged.tags["promptId"] == "test_sync_reports_unusual_tags"
     assert last_logged.tags["numberTag"] == "1"
     assert last_logged.tags["booleanTag"] == "true"
     assert last_logged.tags.get("nullTag") == None
+
+def test_sync_report_anthropic():
+    payload = {
+        "model": "claude-3-opus-20240229",
+        "messages": [{"role": "user", "content": "Hello, Claude"}],
+        "max_tokens": 100,
+    }
+
+    completion = anthropic_client.messages.create(**payload)
+
+    op_client.report_anthropic(
+        requested_at=int(time.time() * 1000 - 1050),
+        received_at=int(time.time() * 1000),
+        req_payload=payload,
+        resp_payload=completion,
+        status_code=200,
+        tags={"promptId": "test_sync_report_anthropic"},
+    )
+
+    if not TEST_LAST_LOGGED:
+        return
+
+    time.sleep(0.1)
+    last_logged = last_logged_call()
+    assert last_logged.req_payload["messages"][0]["content"] == "Hello, Claude"
+    assert (
+        last_logged.resp_payload["choices"][0]["message"]["content"]
+        == completion.content[0].text
+    )
```

### Comparing `openpipe-4.6.0/openpipe/test_sync_update_logged_call_tags.py` & `openpipe-4.7.0/openpipe/test_sync_update_logged_call_tags.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.6.0/pyproject.toml` & `openpipe-4.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "openpipe"
-version = "4.6.0"
+version = "4.7.0"
 description = "Python client library for the OpenPipe service"
 authors = ["Kyle Corbitt <kyle@openpipe.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/OpenPipe/OpenPipe"
 repository = "https://github.com/OpenPipe/OpenPipe"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.1"
 attrs = "^23.1.0"
 python-dateutil = "^2.8.2"
 openai = ">=1.7,<1.16"
-
-[tool.poetry.dev-dependencies]
+anthropic = "<0.26"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
 autoflake = "^2.2.0"
 pytest = "^7.4.0"
 python-dotenv = "^1.0.0"
```

### Comparing `openpipe-4.6.0/PKG-INFO` & `openpipe-4.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: openpipe
-Version: 4.6.0
+Version: 4.7.0
 Summary: Python client library for the OpenPipe service
 Home-page: https://github.com/OpenPipe/OpenPipe
 License: Apache-2.0
 Author: Kyle Corbitt
 Author-email: kyle@openpipe.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: anthropic (<0.26)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: openai (>=1.7,<1.16)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/OpenPipe/OpenPipe
 Description-Content-Type: text/markdown
```

