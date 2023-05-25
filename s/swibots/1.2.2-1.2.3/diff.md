# Comparing `tmp/swibots-1.2.2.tar.gz` & `tmp/swibots-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.2.2.tar", last modified: Thu May 25 09:20:55 2023, max compression
+gzip compressed data, was "swibots-1.2.3.tar", last modified: Thu May 25 10:57:27 2023, max compression
```

## Comparing `swibots-1.2.2.tar` & `swibots-1.2.3.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.247755 swibots-1.2.2/
--rw-rw-rw-   0        0        0     1892 2023-05-25 09:20:55.246757 swibots-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1601 2023-05-24 12:58:14.000000 swibots-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 09:20:55.248755 swibots-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-05-25 09:19:33.000000 swibots-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.819759 swibots-1.2.2/swibots/
--rw-rw-rw-   0        0        0      247 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.836760 swibots-1.2.2/swibots/api/
--rw-rw-rw-   0        0        0      146 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/__init__.py
--rw-rw-rw-   0        0        0     2317 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.841796 swibots-1.2.2/swibots/api/auth/
--rw-rw-rw-   0        0        0       88 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/auth_client.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.845795 swibots-1.2.2/swibots/api/auth/controllers/
--rw-rw-rw-   0        0        0       75 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/controllers/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/controllers/user_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.853774 swibots-1.2.2/swibots/api/auth/methods/
--rw-rw-rw-   0        0        0       99 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/methods/__init__.py
--rw-rw-rw-   0        0        0      671 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/methods/get_me.py
--rw-rw-rw-   0        0        0      861 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/methods/login.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.857755 swibots-1.2.2/swibots/api/auth/models/
--rw-rw-rw-   0        0        0       59 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/models/__init__.py
--rw-rw-rw-   0        0        0     4765 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/auth/models/auth_user.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.861760 swibots-1.2.2/swibots/api/bot/
--rw-rw-rw-   0        0        0       86 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/__init__.py
--rw-rw-rw-   0        0        0     1177 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/bot_client.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.866757 swibots-1.2.2/swibots/api/bot/controllers/
--rw-rw-rw-   0        0        0       74 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/controllers/__init__.py
--rw-rw-rw-   0        0        0     1852 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/controllers/bot_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.875756 swibots-1.2.2/swibots/api/bot/methods/
--rw-rw-rw-   0        0        0      220 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/methods/__init__.py
--rw-rw-rw-   0        0        0      557 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/methods/delete_bot_info.py
--rw-rw-rw-   0        0        0      600 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/methods/get_bot_info.py
--rw-rw-rw-   0        0        0      633 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/methods/update_bot_info.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.882758 swibots-1.2.2/swibots/api/bot/models/
--rw-rw-rw-   0        0        0      120 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/models/__init__.py
--rw-rw-rw-   0        0        0      987 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/models/bot_command_info.py
--rw-rw-rw-   0        0        0     1633 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/bot/models/bot_info.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.887755 swibots-1.2.2/swibots/api/chat/
--rw-rw-rw-   0        0        0      111 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/__init__.py
--rw-rw-rw-   0        0        0     5512 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/chat_client.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.891755 swibots-1.2.2/swibots/api/chat/controllers/
--rw-rw-rw-   0        0        0       86 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/controllers/__init__.py
--rw-rw-rw-   0        0        0    22094 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/controllers/message_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.918754 swibots-1.2.2/swibots/api/chat/events/
--rw-rw-rw-   0        0        0      334 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/events/__init__.py
--rw-rw-rw-   0        0        0     2134 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/events/callback_query_event.py
--rw-rw-rw-   0        0        0     2809 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/events/chat_event.py
--rw-rw-rw-   0        0        0     2157 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/events/command_event.py
--rw-rw-rw-   0        0        0     2166 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/events/inline_query_event.py
--rw-rw-rw-   0        0        0     2503 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/events/message_event.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.976757 swibots-1.2.2/swibots/api/chat/methods/
--rw-rw-rw-   0        0        0     1761 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/__init__.py
--rw-rw-rw-   0        0        0      668 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/answer_inline_query.py
--rw-rw-rw-   0        0        0      714 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/clear_conversation.py
--rw-rw-rw-   0        0        0      726 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/delete_message.py
--rw-rw-rw-   0        0        0      728 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/delete_messages_from_user.py
--rw-rw-rw-   0        0        0     1392 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/download_media.py
--rw-rw-rw-   0        0        0      774 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/edit_message.py
--rw-rw-rw-   0        0        0      877 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/edit_message_text.py
--rw-rw-rw-   0        0        0      714 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/flag_message.py
--rw-rw-rw-   0        0        0     1223 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/forward_message.py
--rw-rw-rw-   0        0        0     1172 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_channel_chat_history.py
--rw-rw-rw-   0        0        0      748 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_community_media_files.py
--rw-rw-rw-   0        0        0      909 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_community_media_files_by_status.py
--rw-rw-rw-   0        0        0      655 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_flag_messages.py
--rw-rw-rw-   0        0        0     1122 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_group_chat_history.py
--rw-rw-rw-   0        0        0      670 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_message.py
--rw-rw-rw-   0        0        0      728 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_messages.py
--rw-rw-rw-   0        0        0     1134 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_messages_between_users.py
--rw-rw-rw-   0        0        0      576 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_unread_messages_count.py
--rw-rw-rw-   0        0        0      810 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/get_user_media_files.py
--rw-rw-rw-   0        0        0      906 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/reply_message.py
--rw-rw-rw-   0        0        0     1058 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/reply_message_text.py
--rw-rw-rw-   0        0        0      874 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/send_message.py
--rw-rw-rw-   0        0        0     1163 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/methods/send_text.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.993756 swibots-1.2.2/swibots/api/chat/models/
--rw-rw-rw-   0        0        0      312 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/__init__.py
--rw-rw-rw-   0        0        0      951 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/group_chat_history.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.024756 swibots-1.2.2/swibots/api/chat/models/inline/
--rw-rw-rw-   0        0        0      575 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rw-rw-rw-   0        0        0     2605 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/inline_query.py
--rw-rw-rw-   0        0        0     1931 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/inline_query_answer.py
--rw-rw-rw-   0        0        0     1021 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result.py
--rw-rw-rw-   0        0        0     1190 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-rw-rw-   0        0        0     1308 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-rw-rw-   0        0        0     1664 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-rw-rw-   0        0        0     1807 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result_video.py
--rw-rw-rw-   0        0        0      603 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/input_message_content.py
--rw-rw-rw-   0        0        0      211 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline/types.py
--rw-rw-rw-   0        0        0      919 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline_keyboard_button.py
--rw-rw-rw-   0        0        0      180 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline_keyboard_color.py
--rw-rw-rw-   0        0        0      154 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline_keyboard_size.py
--rw-rw-rw-   0        0        0     2123 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/inline_markup.py
--rw-rw-rw-   0        0        0    11038 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/chat/models/message.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.027758 swibots-1.2.2/swibots/api/common/
--rw-rw-rw-   0        0        0       46 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.031755 swibots-1.2.2/swibots/api/common/events/
--rw-rw-rw-   0        0        0       49 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/common/events/__init__.py
--rw-rw-rw-   0        0        0     2859 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/common/events/event.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.042755 swibots-1.2.2/swibots/api/common/models/
--rw-rw-rw-   0        0        0      104 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/common/models/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/common/models/media.py
--rw-rw-rw-   0        0        0     1613 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/common/models/media_upload_request.py
--rw-rw-rw-   0        0        0     1759 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/common/models/user.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.047756 swibots-1.2.2/swibots/api/community/
--rw-rw-rw-   0        0        0       93 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/__init__.py
--rw-rw-rw-   0        0        0     5180 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/community_client.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.058761 swibots-1.2.2/swibots/api/community/controllers/
--rw-rw-rw-   0        0        0      105 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/controllers/__init__.py
--rw-rw-rw-   0        0        0      618 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/controllers/channel_controller.py
--rw-rw-rw-   0        0        0      636 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/controllers/community_controller.py
--rw-rw-rw-   0        0        0      596 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/controllers/group_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.090762 swibots-1.2.2/swibots/api/community/events/
--rw-rw-rw-   0        0        0      577 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/channel_created_event.py
--rw-rw-rw-   0        0        0     1428 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/channel_deleted_event.py
--rw-rw-rw-   0        0        0     1428 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/channel_updated_event.py
--rw-rw-rw-   0        0        0     2373 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/community_event.py
--rw-rw-rw-   0        0        0     1424 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/community_updated_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/group_created_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/group_deleted_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/group_updated_event.py
--rw-rw-rw-   0        0        0     1421 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/member_joined_event.py
--rw-rw-rw-   0        0        0     1418 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/member_left_event.py
--rw-rw-rw-   0        0        0     1414 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/events/user_banned_event.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.099756 swibots-1.2.2/swibots/api/community/methods/
--rw-rw-rw-   0        0        0      205 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/methods/__init__.py
--rw-rw-rw-   0        0        0      664 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/methods/get_channel.py
--rw-rw-rw-   0        0        0      689 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/methods/get_community.py
--rw-rw-rw-   0        0        0      640 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/methods/get_group.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.109756 swibots-1.2.2/swibots/api/community/models/
--rw-rw-rw-   0        0        0      137 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/models/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/models/channel.py
--rw-rw-rw-   0        0        0     3033 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/models/community.py
--rw-rw-rw-   0        0        0     2792 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/api/community/models/group.py
--rw-rw-rw-   0        0        0     9630 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/app.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.124757 swibots-1.2.2/swibots/base/
--rw-rw-rw-   0        0        0      268 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/base/__init__.py
--rw-rw-rw-   0        0        0       71 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/base/rest_controller.py
--rw-rw-rw-   0        0        0      386 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/base/rest_request.py
--rw-rw-rw-   0        0        0      669 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/base/rest_response.py
--rw-rw-rw-   0        0        0     4380 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/base/switch_client.py
--rw-rw-rw-   0        0        0     1221 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/base/switch_object.py
--rw-rw-rw-   0        0        0      563 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/base/switch_ws_async_client.py
--rw-rw-rw-   0        0        0     4734 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bot_app.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.136760 swibots-1.2.2/swibots/bots/
--rw-rw-rw-   0        0        0      208 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/__init__.py
--rw-rw-rw-   0        0        0     4782 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/bot.py
--rw-rw-rw-   0        0        0     1690 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/bot_context.py
--rw-rw-rw-   0        0        0      111 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.173755 swibots-1.2.2/swibots/bots/decorators/
--rw-rw-rw-   0        0        0     1034 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/__init__.py
--rw-rw-rw-   0        0        0      558 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_callback_query.py
--rw-rw-rw-   0        0        0      526 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_channel_created.py
--rw-rw-rw-   0        0        0      562 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_channel_deleted.py
--rw-rw-rw-   0        0        0      559 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_channel_updated.py
--rw-rw-rw-   0        0        0      593 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_command.py
--rw-rw-rw-   0        0        0      562 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_community_updated.py
--rw-rw-rw-   0        0        0      554 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_group_created.py
--rw-rw-rw-   0        0        0      554 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_group_deleted.py
--rw-rw-rw-   0        0        0      552 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_group_updated.py
--rw-rw-rw-   0        0        0      554 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_inline_query.py
--rw-rw-rw-   0        0        0      552 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_member_joined.py
--rw-rw-rw-   0        0        0      547 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_member_left.py
--rw-rw-rw-   0        0        0      519 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_message.py
--rw-rw-rw-   0        0        0      561 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_unknown_command.py
--rw-rw-rw-   0        0        0      525 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/decorators/on_user_banned.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.177755 swibots-1.2.2/swibots/bots/filters/
--rw-rw-rw-   0        0        0       23 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/filters/__init__.py
--rw-rw-rw-   0        0        0     8057 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/filters/filter.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.220759 swibots-1.2.2/swibots/bots/handlers/
--rw-rw-rw-   0        0        0     1337 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/__init__.py
--rw-rw-rw-   0        0        0     1087 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/base_handler.py
--rw-rw-rw-   0        0        0     1016 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/callback_query_handler.py
--rw-rw-rw-   0        0        0      704 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/channel_created_handler.py
--rw-rw-rw-   0        0        0      711 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/channel_deleted_handler.py
--rw-rw-rw-   0        0        0      758 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/channel_updated_handler.py
--rw-rw-rw-   0        0        0     1557 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/command_handler.py
--rw-rw-rw-   0        0        0      709 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/community_updated_handler.py
--rw-rw-rw-   0        0        0     1365 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/event_handler.py
--rw-rw-rw-   0        0        0      703 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/group_created_handler.py
--rw-rw-rw-   0        0        0      800 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/group_deleted_handler.py
--rw-rw-rw-   0        0        0      800 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/group_updated_handler.py
--rw-rw-rw-   0        0        0      896 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/inline_query_handler.py
--rw-rw-rw-   0        0        0      702 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/member_joined_handler.py
--rw-rw-rw-   0        0        0      697 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/member_left_handler.py
--rw-rw-rw-   0        0        0      991 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/message_handler.py
--rw-rw-rw-   0        0        0      914 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/unknown_command_handler.py
--rw-rw-rw-   0        0        0      693 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/handlers/user_banned_handler.py
--rw-rw-rw-   0        0        0      298 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/bots/register_command.py
--rw-rw-rw-   0        0        0     1678 2023-05-25 09:18:55.000000 swibots-1.2.2/swibots/config.py
--rw-rw-rw-   0        0        0     1387 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/error.py
--rw-rw-rw-   0        0        0      878 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/types.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.227755 swibots-1.2.2/swibots/utils/
--rw-rw-rw-   0        0        0       78 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/__init__.py
--rw-rw-rw-   0        0        0     6029 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/rest_client.py
--rw-rw-rw-   0        0        0     2558 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.230756 swibots-1.2.2/swibots/utils/ws/
--rw-rw-rw-   0        0        0       50 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/ws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.237755 swibots-1.2.2/swibots/utils/ws/asyncstomp/
--rw-rw-rw-   0        0        0      154 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/ws/asyncstomp/__init__.py
--rw-rw-rw-   0        0        0    10026 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-rw-rw-   0        0        0     1010 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:55.244756 swibots-1.2.2/swibots/utils/ws/common/
--rw-rw-rw-   0        0        0      104 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/ws/common/__init__.py
--rw-rw-rw-   0        0        0     1716 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/ws/common/ws_frame.py
--rw-rw-rw-   0        0        0      441 2023-05-24 12:58:14.000000 swibots-1.2.2/swibots/utils/ws/common/ws_message.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:20:54.830757 swibots-1.2.2/swibots.egg-info/
--rw-rw-rw-   0        0        0     1892 2023-05-25 09:20:54.000000 swibots-1.2.2/swibots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7283 2023-05-25 09:20:54.000000 swibots-1.2.2/swibots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 09:20:54.000000 swibots-1.2.2/swibots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-25 09:20:54.000000 swibots-1.2.2/swibots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 09:20:54.000000 swibots-1.2.2/swibots.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.543618 swibots-1.2.3/
+-rw-rw-rw-   0        0        0     1892 2023-05-25 10:57:27.541616 swibots-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1601 2023-05-24 12:58:14.000000 swibots-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 10:57:27.543618 swibots-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-05-25 10:57:19.000000 swibots-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:26.956295 swibots-1.2.3/swibots/
+-rw-rw-rw-   0        0        0      247 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:26.977287 swibots-1.2.3/swibots/api/
+-rw-rw-rw-   0        0        0      146 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/__init__.py
+-rw-rw-rw-   0        0        0     2317 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:26.983287 swibots-1.2.3/swibots/api/auth/
+-rw-rw-rw-   0        0        0       88 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/auth_client.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:26.991287 swibots-1.2.3/swibots/api/auth/controllers/
+-rw-rw-rw-   0        0        0       75 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/controllers/__init__.py
+-rw-rw-rw-   0        0        0     1565 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/controllers/user_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:26.999289 swibots-1.2.3/swibots/api/auth/methods/
+-rw-rw-rw-   0        0        0       99 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/methods/__init__.py
+-rw-rw-rw-   0        0        0      671 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/methods/get_me.py
+-rw-rw-rw-   0        0        0      861 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/methods/login.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.006286 swibots-1.2.3/swibots/api/auth/models/
+-rw-rw-rw-   0        0        0       59 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/models/__init__.py
+-rw-rw-rw-   0        0        0     4765 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/auth/models/auth_user.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.012287 swibots-1.2.3/swibots/api/bot/
+-rw-rw-rw-   0        0        0       86 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/__init__.py
+-rw-rw-rw-   0        0        0     1177 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/bot_client.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.018285 swibots-1.2.3/swibots/api/bot/controllers/
+-rw-rw-rw-   0        0        0       74 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/controllers/__init__.py
+-rw-rw-rw-   0        0        0     1852 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/controllers/bot_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.031289 swibots-1.2.3/swibots/api/bot/methods/
+-rw-rw-rw-   0        0        0      220 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/methods/__init__.py
+-rw-rw-rw-   0        0        0      557 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/methods/delete_bot_info.py
+-rw-rw-rw-   0        0        0      600 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/methods/get_bot_info.py
+-rw-rw-rw-   0        0        0      633 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/methods/update_bot_info.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.041285 swibots-1.2.3/swibots/api/bot/models/
+-rw-rw-rw-   0        0        0      120 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/models/__init__.py
+-rw-rw-rw-   0        0        0      987 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/models/bot_command_info.py
+-rw-rw-rw-   0        0        0     1633 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/bot/models/bot_info.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.047289 swibots-1.2.3/swibots/api/chat/
+-rw-rw-rw-   0        0        0      111 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/__init__.py
+-rw-rw-rw-   0        0        0     5512 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/chat_client.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.054283 swibots-1.2.3/swibots/api/chat/controllers/
+-rw-rw-rw-   0        0        0       86 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/controllers/__init__.py
+-rw-rw-rw-   0        0        0    22094 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/controllers/message_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.076288 swibots-1.2.3/swibots/api/chat/events/
+-rw-rw-rw-   0        0        0      334 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/events/__init__.py
+-rw-rw-rw-   0        0        0     2134 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/events/callback_query_event.py
+-rw-rw-rw-   0        0        0     2809 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/events/chat_event.py
+-rw-rw-rw-   0        0        0     2157 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/events/command_event.py
+-rw-rw-rw-   0        0        0     2166 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/events/inline_query_event.py
+-rw-rw-rw-   0        0        0     2503 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/events/message_event.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.173287 swibots-1.2.3/swibots/api/chat/methods/
+-rw-rw-rw-   0        0        0     1761 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/answer_inline_query.py
+-rw-rw-rw-   0        0        0      714 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/clear_conversation.py
+-rw-rw-rw-   0        0        0      726 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/delete_message.py
+-rw-rw-rw-   0        0        0      728 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/delete_messages_from_user.py
+-rw-rw-rw-   0        0        0     1392 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/download_media.py
+-rw-rw-rw-   0        0        0      774 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/edit_message.py
+-rw-rw-rw-   0        0        0      877 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/edit_message_text.py
+-rw-rw-rw-   0        0        0      714 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/flag_message.py
+-rw-rw-rw-   0        0        0     1223 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/forward_message.py
+-rw-rw-rw-   0        0        0     1172 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_channel_chat_history.py
+-rw-rw-rw-   0        0        0      748 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_community_media_files.py
+-rw-rw-rw-   0        0        0      909 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rw-rw-rw-   0        0        0      655 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_flag_messages.py
+-rw-rw-rw-   0        0        0     1122 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_group_chat_history.py
+-rw-rw-rw-   0        0        0      670 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_message.py
+-rw-rw-rw-   0        0        0      728 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_messages.py
+-rw-rw-rw-   0        0        0     1134 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_messages_between_users.py
+-rw-rw-rw-   0        0        0      576 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_unread_messages_count.py
+-rw-rw-rw-   0        0        0      810 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/get_user_media_files.py
+-rw-rw-rw-   0        0        0      906 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/reply_message.py
+-rw-rw-rw-   0        0        0     1058 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/reply_message_text.py
+-rw-rw-rw-   0        0        0      874 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/send_message.py
+-rw-rw-rw-   0        0        0     1163 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/methods/send_text.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.197288 swibots-1.2.3/swibots/api/chat/models/
+-rw-rw-rw-   0        0        0      312 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/__init__.py
+-rw-rw-rw-   0        0        0      951 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/group_chat_history.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.232284 swibots-1.2.3/swibots/api/chat/models/inline/
+-rw-rw-rw-   0        0        0      575 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rw-rw-rw-   0        0        0     2605 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/inline_query.py
+-rw-rw-rw-   0        0        0     1931 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/inline_query_answer.py
+-rw-rw-rw-   0        0        0     1021 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result.py
+-rw-rw-rw-   0        0        0     1190 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-rw-rw-   0        0        0     1308 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-rw-rw-   0        0        0     1664 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-rw-rw-   0        0        0     1807 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result_video.py
+-rw-rw-rw-   0        0        0      603 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/input_message_content.py
+-rw-rw-rw-   0        0        0      211 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline/types.py
+-rw-rw-rw-   0        0        0      919 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0      180 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline_keyboard_color.py
+-rw-rw-rw-   0        0        0      154 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline_keyboard_size.py
+-rw-rw-rw-   0        0        0     2123 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/inline_markup.py
+-rw-rw-rw-   0        0        0    11038 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/chat/models/message.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.234285 swibots-1.2.3/swibots/api/common/
+-rw-rw-rw-   0        0        0       46 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.243287 swibots-1.2.3/swibots/api/common/events/
+-rw-rw-rw-   0        0        0       49 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/common/events/__init__.py
+-rw-rw-rw-   0        0        0     2859 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/common/events/event.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.254285 swibots-1.2.3/swibots/api/common/models/
+-rw-rw-rw-   0        0        0      104 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/common/models/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/common/models/media.py
+-rw-rw-rw-   0        0        0     1613 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/common/models/media_upload_request.py
+-rw-rw-rw-   0        0        0     1759 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/common/models/user.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.263287 swibots-1.2.3/swibots/api/community/
+-rw-rw-rw-   0        0        0       93 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/__init__.py
+-rw-rw-rw-   0        0        0     5180 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/community_client.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.278602 swibots-1.2.3/swibots/api/community/controllers/
+-rw-rw-rw-   0        0        0      105 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/controllers/__init__.py
+-rw-rw-rw-   0        0        0      618 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/controllers/channel_controller.py
+-rw-rw-rw-   0        0        0      636 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/controllers/community_controller.py
+-rw-rw-rw-   0        0        0      596 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/controllers/group_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.324618 swibots-1.2.3/swibots/api/community/events/
+-rw-rw-rw-   0        0        0      577 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/channel_created_event.py
+-rw-rw-rw-   0        0        0     1428 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/channel_deleted_event.py
+-rw-rw-rw-   0        0        0     1428 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/channel_updated_event.py
+-rw-rw-rw-   0        0        0     2373 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/community_event.py
+-rw-rw-rw-   0        0        0     1424 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/community_updated_event.py
+-rw-rw-rw-   0        0        0     1422 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/group_created_event.py
+-rw-rw-rw-   0        0        0     1422 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/group_deleted_event.py
+-rw-rw-rw-   0        0        0     1422 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/group_updated_event.py
+-rw-rw-rw-   0        0        0     1421 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/member_joined_event.py
+-rw-rw-rw-   0        0        0     1418 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/member_left_event.py
+-rw-rw-rw-   0        0        0     1414 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/events/user_banned_event.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.338618 swibots-1.2.3/swibots/api/community/methods/
+-rw-rw-rw-   0        0        0      205 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/methods/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/methods/get_channel.py
+-rw-rw-rw-   0        0        0      689 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/methods/get_community.py
+-rw-rw-rw-   0        0        0      640 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/methods/get_group.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.350616 swibots-1.2.3/swibots/api/community/models/
+-rw-rw-rw-   0        0        0      137 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/models/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/models/channel.py
+-rw-rw-rw-   0        0        0     3033 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/models/community.py
+-rw-rw-rw-   0        0        0     2792 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/api/community/models/group.py
+-rw-rw-rw-   0        0        0     9630 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/app.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.374620 swibots-1.2.3/swibots/base/
+-rw-rw-rw-   0        0        0      268 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/base/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/base/rest_controller.py
+-rw-rw-rw-   0        0        0      386 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/base/rest_request.py
+-rw-rw-rw-   0        0        0      669 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/base/rest_response.py
+-rw-rw-rw-   0        0        0     4380 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/base/switch_client.py
+-rw-rw-rw-   0        0        0     1221 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/base/switch_object.py
+-rw-rw-rw-   0        0        0      563 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/base/switch_ws_async_client.py
+-rw-rw-rw-   0        0        0     4734 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bot_app.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.389615 swibots-1.2.3/swibots/bots/
+-rw-rw-rw-   0        0        0      208 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/__init__.py
+-rw-rw-rw-   0        0        0     4782 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/bot.py
+-rw-rw-rw-   0        0        0     1690 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/bot_context.py
+-rw-rw-rw-   0        0        0      111 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.442616 swibots-1.2.3/swibots/bots/decorators/
+-rw-rw-rw-   0        0        0     1034 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_callback_query.py
+-rw-rw-rw-   0        0        0      526 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_channel_created.py
+-rw-rw-rw-   0        0        0      562 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_channel_deleted.py
+-rw-rw-rw-   0        0        0      559 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_channel_updated.py
+-rw-rw-rw-   0        0        0      593 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_command.py
+-rw-rw-rw-   0        0        0      562 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_community_updated.py
+-rw-rw-rw-   0        0        0      554 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_group_created.py
+-rw-rw-rw-   0        0        0      554 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_group_deleted.py
+-rw-rw-rw-   0        0        0      552 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_group_updated.py
+-rw-rw-rw-   0        0        0      554 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_inline_query.py
+-rw-rw-rw-   0        0        0      552 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_member_joined.py
+-rw-rw-rw-   0        0        0      547 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_member_left.py
+-rw-rw-rw-   0        0        0      519 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_message.py
+-rw-rw-rw-   0        0        0      561 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_unknown_command.py
+-rw-rw-rw-   0        0        0      525 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/decorators/on_user_banned.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.449618 swibots-1.2.3/swibots/bots/filters/
+-rw-rw-rw-   0        0        0       23 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/filters/__init__.py
+-rw-rw-rw-   0        0        0     8057 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/filters/filter.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.505620 swibots-1.2.3/swibots/bots/handlers/
+-rw-rw-rw-   0        0        0     1337 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1087 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/base_handler.py
+-rw-rw-rw-   0        0        0     1016 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/callback_query_handler.py
+-rw-rw-rw-   0        0        0      704 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/channel_created_handler.py
+-rw-rw-rw-   0        0        0      711 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/channel_deleted_handler.py
+-rw-rw-rw-   0        0        0      758 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/channel_updated_handler.py
+-rw-rw-rw-   0        0        0     1557 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/command_handler.py
+-rw-rw-rw-   0        0        0      709 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/community_updated_handler.py
+-rw-rw-rw-   0        0        0     1365 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/event_handler.py
+-rw-rw-rw-   0        0        0      703 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/group_created_handler.py
+-rw-rw-rw-   0        0        0      800 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/group_deleted_handler.py
+-rw-rw-rw-   0        0        0      800 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/group_updated_handler.py
+-rw-rw-rw-   0        0        0      896 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/inline_query_handler.py
+-rw-rw-rw-   0        0        0      702 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/member_joined_handler.py
+-rw-rw-rw-   0        0        0      697 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/member_left_handler.py
+-rw-rw-rw-   0        0        0      991 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/message_handler.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/unknown_command_handler.py
+-rw-rw-rw-   0        0        0      693 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/handlers/user_banned_handler.py
+-rw-rw-rw-   0        0        0      298 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/bots/register_command.py
+-rw-rw-rw-   0        0        0     1868 2023-05-25 10:56:39.000000 swibots-1.2.3/swibots/config.py
+-rw-rw-rw-   0        0        0     1387 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/error.py
+-rw-rw-rw-   0        0        0      878 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/types.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.516617 swibots-1.2.3/swibots/utils/
+-rw-rw-rw-   0        0        0       78 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/__init__.py
+-rw-rw-rw-   0        0        0     6029 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/rest_client.py
+-rw-rw-rw-   0        0        0     2558 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.518620 swibots-1.2.3/swibots/utils/ws/
+-rw-rw-rw-   0        0        0       50 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/ws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.529617 swibots-1.2.3/swibots/utils/ws/asyncstomp/
+-rw-rw-rw-   0        0        0      154 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/ws/asyncstomp/__init__.py
+-rw-rw-rw-   0        0        0    10026 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-rw-rw-   0        0        0     1010 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:27.537617 swibots-1.2.3/swibots/utils/ws/common/
+-rw-rw-rw-   0        0        0      104 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/ws/common/__init__.py
+-rw-rw-rw-   0        0        0     1716 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/ws/common/ws_frame.py
+-rw-rw-rw-   0        0        0      441 2023-05-24 12:58:14.000000 swibots-1.2.3/swibots/utils/ws/common/ws_message.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:57:26.970283 swibots-1.2.3/swibots.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-05-25 10:57:26.000000 swibots-1.2.3/swibots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7283 2023-05-25 10:57:26.000000 swibots-1.2.3/swibots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 10:57:26.000000 swibots-1.2.3/swibots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-25 10:57:26.000000 swibots-1.2.3/swibots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 10:57:26.000000 swibots-1.2.3/swibots.egg-info/top_level.txt
```

### Comparing `swibots-1.2.2/PKG-INFO` & `swibots-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.2.2
+Version: 1.2.3
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.2.2/README.md` & `swibots-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/setup.py` & `swibots-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
 
 setup(
     name="swibots",
-    version="1.2.2",
+    version="1.2.3",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/switchcollab/Switch-Bots-Python-Library",
     description="Switch bot api",
     author="switchadmin",
     author_email="support@switch.pe",
```

### Comparing `swibots-1.2.2/swibots/api/api_client.py` & `swibots-1.2.3/swibots/api/api_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/auth/auth_client.py` & `swibots-1.2.3/swibots/api/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/auth/controllers/user_controller.py` & `swibots-1.2.3/swibots/api/auth/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/auth/methods/get_me.py` & `swibots-1.2.3/swibots/api/auth/methods/get_me.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/auth/methods/login.py` & `swibots-1.2.3/swibots/api/auth/methods/login.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/auth/models/auth_user.py` & `swibots-1.2.3/swibots/api/auth/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/bot/bot_client.py` & `swibots-1.2.3/swibots/api/bot/bot_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.2.3/swibots/api/bot/controllers/bot_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/bot/methods/delete_bot_info.py` & `swibots-1.2.3/swibots/api/bot/methods/delete_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.2.3/swibots/api/bot/methods/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.2.3/swibots/api/bot/methods/update_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/bot/models/bot_command_info.py` & `swibots-1.2.3/swibots/api/bot/models/bot_command_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/bot/models/bot_info.py` & `swibots-1.2.3/swibots/api/bot/models/bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/chat_client.py` & `swibots-1.2.3/swibots/api/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/controllers/message_controller.py` & `swibots-1.2.3/swibots/api/chat/controllers/message_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/events/callback_query_event.py` & `swibots-1.2.3/swibots/api/chat/events/callback_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/events/chat_event.py` & `swibots-1.2.3/swibots/api/chat/events/chat_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/events/command_event.py` & `swibots-1.2.3/swibots/api/chat/events/command_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/events/inline_query_event.py` & `swibots-1.2.3/swibots/api/chat/events/inline_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/events/message_event.py` & `swibots-1.2.3/swibots/api/chat/events/message_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/__init__.py` & `swibots-1.2.3/swibots/api/chat/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.2.3/swibots/api/chat/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.2.3/swibots/api/chat/methods/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/delete_message.py` & `swibots-1.2.3/swibots/api/chat/methods/delete_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.2.3/swibots/api/chat/methods/delete_messages_from_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/download_media.py` & `swibots-1.2.3/swibots/api/chat/methods/download_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/edit_message.py` & `swibots-1.2.3/swibots/api/chat/methods/edit_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.2.3/swibots/api/chat/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/flag_message.py` & `swibots-1.2.3/swibots/api/chat/methods/flag_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/forward_message.py` & `swibots-1.2.3/swibots/api/chat/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.2.3/swibots/api/chat/methods/get_channel_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.2.3/swibots/api/chat/methods/get_community_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_community_media_files_by_status.py` & `swibots-1.2.3/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.2.3/swibots/api/chat/methods/get_flag_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_group_chat_history.py` & `swibots-1.2.3/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_message.py` & `swibots-1.2.3/swibots/api/chat/methods/get_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_messages.py` & `swibots-1.2.3/swibots/api/chat/methods/get_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.2.3/swibots/api/chat/methods/get_messages_between_users.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_unread_messages_count.py` & `swibots-1.2.3/swibots/api/chat/methods/get_unread_messages_count.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/get_user_media_files.py` & `swibots-1.2.3/swibots/api/chat/methods/get_user_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/reply_message.py` & `swibots-1.2.3/swibots/api/chat/methods/reply_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.2.3/swibots/api/chat/methods/reply_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/send_message.py` & `swibots-1.2.3/swibots/api/chat/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/methods/send_text.py` & `swibots-1.2.3/swibots/api/chat/methods/send_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/group_chat_history.py` & `swibots-1.2.3/swibots/api/chat/models/group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/__init__.py` & `swibots-1.2.3/swibots/api/chat/models/inline/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.2.3/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.2.3/swibots/api/chat/models/inline/inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.2.3/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/inline_query_result_video.py` & `swibots-1.2.3/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline/input_message_content.py` & `swibots-1.2.3/swibots/api/chat/models/inline/input_message_content.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline_keyboard_button.py` & `swibots-1.2.3/swibots/api/chat/models/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/inline_markup.py` & `swibots-1.2.3/swibots/api/chat/models/inline_markup.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/chat/models/message.py` & `swibots-1.2.3/swibots/api/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/common/events/event.py` & `swibots-1.2.3/swibots/api/common/events/event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/common/models/media.py` & `swibots-1.2.3/swibots/api/common/models/media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/common/models/media_upload_request.py` & `swibots-1.2.3/swibots/api/common/models/media_upload_request.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/common/models/user.py` & `swibots-1.2.3/swibots/api/common/models/user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/community_client.py` & `swibots-1.2.3/swibots/api/community/community_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/controllers/channel_controller.py` & `swibots-1.2.3/swibots/api/community/controllers/channel_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/controllers/community_controller.py` & `swibots-1.2.3/swibots/api/community/controllers/community_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/controllers/group_controller.py` & `swibots-1.2.3/swibots/api/community/controllers/group_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/__init__.py` & `swibots-1.2.3/swibots/api/community/events/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/channel_created_event.py` & `swibots-1.2.3/swibots/api/community/events/channel_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.2.3/swibots/api/community/events/channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/channel_updated_event.py` & `swibots-1.2.3/swibots/api/community/events/channel_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/community_event.py` & `swibots-1.2.3/swibots/api/community/events/community_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/community_updated_event.py` & `swibots-1.2.3/swibots/api/community/events/community_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/group_created_event.py` & `swibots-1.2.3/swibots/api/community/events/group_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/group_deleted_event.py` & `swibots-1.2.3/swibots/api/community/events/group_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/group_updated_event.py` & `swibots-1.2.3/swibots/api/community/events/group_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/member_joined_event.py` & `swibots-1.2.3/swibots/api/community/events/member_joined_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/member_left_event.py` & `swibots-1.2.3/swibots/api/community/events/member_left_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/events/user_banned_event.py` & `swibots-1.2.3/swibots/api/community/events/user_banned_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/methods/get_channel.py` & `swibots-1.2.3/swibots/api/community/methods/get_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/methods/get_community.py` & `swibots-1.2.3/swibots/api/community/methods/get_community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/methods/get_group.py` & `swibots-1.2.3/swibots/api/community/methods/get_group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/models/channel.py` & `swibots-1.2.3/swibots/api/community/models/channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/models/community.py` & `swibots-1.2.3/swibots/api/community/models/community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/api/community/models/group.py` & `swibots-1.2.3/swibots/api/community/models/group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/app.py` & `swibots-1.2.3/swibots/app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/base/rest_response.py` & `swibots-1.2.3/swibots/base/rest_response.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/base/switch_client.py` & `swibots-1.2.3/swibots/base/switch_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/base/switch_object.py` & `swibots-1.2.3/swibots/base/switch_object.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/base/switch_ws_async_client.py` & `swibots-1.2.3/swibots/base/switch_ws_async_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bot_app.py` & `swibots-1.2.3/swibots/bot_app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/bot.py` & `swibots-1.2.3/swibots/bots/bot.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/bot_context.py` & `swibots-1.2.3/swibots/bots/bot_context.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/__init__.py` & `swibots-1.2.3/swibots/bots/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_callback_query.py` & `swibots-1.2.3/swibots/bots/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_channel_created.py` & `swibots-1.2.3/swibots/bots/decorators/on_channel_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.2.3/swibots/bots/decorators/on_channel_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.2.3/swibots/bots/decorators/on_channel_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_command.py` & `swibots-1.2.3/swibots/bots/decorators/on_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_community_updated.py` & `swibots-1.2.3/swibots/bots/decorators/on_community_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_group_created.py` & `swibots-1.2.3/swibots/bots/decorators/on_group_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.2.3/swibots/bots/decorators/on_group_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_group_updated.py` & `swibots-1.2.3/swibots/bots/decorators/on_group_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_inline_query.py` & `swibots-1.2.3/swibots/bots/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_member_joined.py` & `swibots-1.2.3/swibots/bots/decorators/on_member_joined.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_member_left.py` & `swibots-1.2.3/swibots/bots/decorators/on_member_left.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_message.py` & `swibots-1.2.3/swibots/bots/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_unknown_command.py` & `swibots-1.2.3/swibots/bots/decorators/on_unknown_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/decorators/on_user_banned.py` & `swibots-1.2.3/swibots/bots/decorators/on_user_banned.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/filters/filter.py` & `swibots-1.2.3/swibots/bots/filters/filter.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/__init__.py` & `swibots-1.2.3/swibots/bots/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/base_handler.py` & `swibots-1.2.3/swibots/bots/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.2.3/swibots/bots/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.2.3/swibots/bots/handlers/channel_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.2.3/swibots/bots/handlers/channel_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.2.3/swibots/bots/handlers/channel_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/command_handler.py` & `swibots-1.2.3/swibots/bots/handlers/command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.2.3/swibots/bots/handlers/community_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/event_handler.py` & `swibots-1.2.3/swibots/bots/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/group_created_handler.py` & `swibots-1.2.3/swibots/bots/handlers/group_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.2.3/swibots/bots/handlers/group_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.2.3/swibots/bots/handlers/group_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.2.3/swibots/bots/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.2.3/swibots/bots/handlers/member_joined_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/member_left_handler.py` & `swibots-1.2.3/swibots/bots/handlers/member_left_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/message_handler.py` & `swibots-1.2.3/swibots/bots/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.2.3/swibots/bots/handlers/unknown_command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/bots/handlers/user_banned_handler.py` & `swibots-1.2.3/swibots/bots/handlers/user_banned_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/config.py` & `swibots-1.2.3/swibots/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import os
 
 
 APP_CONFIG = {
     "CHAT_SERVICE": {
-        "BASE_URL": os.getenv("CHAT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
+        "BASE_URL": os.getenv("CHAT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/chat-service",
         "WS_URL": os.getenv("CHAT_SERVICE_WS_URL")
-        or "wss://api-gateway.switch.pe/v1/websocket/message/ws",
+        or "wss://api-gateway.switch.pe/chat-service/v1/websocket/message/ws",
     },
     "BOT_SERVICE": {
-        "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
+        "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/chat-service",
     },
     "AUTH_SERVICE": {
-        "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api",
+        "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/user-service/api",
     },
     "COMMUNITY_SERVICE": {
-        "BASE_URL": os.getenv("COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
+        "BASE_URL": os.getenv("COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/community-service",
         "WS_URL": os.getenv("COMMUNITY_SERVICE_WS_URL")
-        or "wss://api-gateway.switch.pe/v1/websocket/community/ws",
+        or "wss://api-gateway.switch.pe/community-service/v1/websocket/community/ws",
     },
 }
 
 
 def get_config():
     return APP_CONFIG
 
 
 def reload_config():
     APP_CONFIG["CHAT_SERVICE"]['BASE_URL'] = os.getenv(
-        "CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe"
+        "CHAT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/chat-service"
     APP_CONFIG["CHAT_SERVICE"]['WS_URL'] = os.getenv(
-        "CHAT_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/message/ws"
+        "CHAT_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/chat-service/v1/websocket/message/ws"
     APP_CONFIG["BOT_SERVICE"]['BASE_URL'] = os.getenv(
-        "BOT_SERVICE_BASE_URL") or "https://chat.switch.pe"
+        "BOT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/chat-service"
     APP_CONFIG["AUTH_SERVICE"]['BASE_URL'] = os.getenv(
-        "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api"
+        "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/user-service/api"
     APP_CONFIG["COMMUNITY_SERVICE"]['BASE_URL'] = os.getenv(
-        "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
+        "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/community-service"
     APP_CONFIG["COMMUNITY_SERVICE"]['WS_URL'] = os.getenv(
-        "COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/community/ws"
+        "COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/community-service/v1/websocket/community/ws"
 
 
 reload_config()
```

### Comparing `swibots-1.2.2/swibots/error.py` & `swibots-1.2.3/swibots/error.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/types.py` & `swibots-1.2.3/swibots/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/utils/rest_client.py` & `swibots-1.2.3/swibots/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/utils/types.py` & `swibots-1.2.3/swibots/utils/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.2.3/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.2.3/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots/utils/ws/common/ws_frame.py` & `swibots-1.2.3/swibots/utils/ws/common/ws_frame.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.2/swibots.egg-info/PKG-INFO` & `swibots-1.2.3/swibots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.2.2
+Version: 1.2.3
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.2.2/swibots.egg-info/SOURCES.txt` & `swibots-1.2.3/swibots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

