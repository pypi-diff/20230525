# Comparing `tmp/pyFipper-0.1.2.dev3.tar.gz` & `tmp/pyFipper-0.1.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFipper-0.1.2.dev3.tar", last modified: Wed May 24 09:13:41 2023, max compression
+gzip compressed data, was "pyFipper-0.1.2.dev4.tar", last modified: Wed May 24 09:30:51 2023, max compression
```

## Comparing `pyFipper-0.1.2.dev3.tar` & `pyFipper-0.1.2.dev4.tar`

### file list

```diff
@@ -1,486 +1,486 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:41.025056 pyFipper-0.1.2.dev3/
--rw-rw-rw-   0        0        0    35184 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/LICENSE
--rw-rw-rw-   0        0        0      301 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/MANIFEST.in
--rw-rw-rw-   0        0        0      791 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/NOTICE
--rw-rw-rw-   0        0        0     2230 2023-05-24 09:13:41.024057 pyFipper-0.1.2.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     1313 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.868263 pyFipper-0.1.2.dev3/compiler/
--rw-rw-rw-   0        0        0      835 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.872260 pyFipper-0.1.2.dev3/compiler/api/
--rw-rw-rw-   0        0        0      835 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/api/__init__.py
--rw-rw-rw-   0        0        0    23054 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/api/compiler.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.880254 pyFipper-0.1.2.dev3/compiler/api/source/
--rw-rw-rw-   0        0        0     2273 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/api/source/auth_key.tl
--rw-rw-rw-   0        0        0   159892 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/api/source/main_api.tl
--rw-rw-rw-   0        0        0     3501 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/api/source/sys_msgs.tl
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.884251 pyFipper-0.1.2.dev3/compiler/api/template/
--rw-rw-rw-   0        0        0      778 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/api/template/combinator.txt
--rw-rw-rw-   0        0        0      658 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/api/template/type.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.890247 pyFipper-0.1.2.dev3/compiler/errors/
--rw-rw-rw-   0        0        0      835 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/__init__.py
--rw-rw-rw-   0        0        0     5059 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/compiler.py
--rw-rw-rw-   0        0        0     1298 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/sort.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.909236 pyFipper-0.1.2.dev3/compiler/errors/source/
--rw-rw-rw-   0        0        0      475 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/source/303_SEE_OTHER.tsv
--rw-rw-rw-   0        0        0    22646 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-rw-rw-   0        0        0      687 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-rw-rw-   0        0        0     2027 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/source/403_FORBIDDEN.tsv
--rw-rw-rw-   0        0        0     1189 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-rw-rw-   0        0        0      475 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/source/420_FLOOD.tsv
--rw-rw-rw-   0        0        0     4263 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-rw-rw-   0        0        0      157 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.914233 pyFipper-0.1.2.dev3/compiler/errors/template/
--rw-rw-rw-   0        0        0      190 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/template/class.txt
--rw-rw-rw-   0        0        0      127 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/compiler/errors/template/sub_class.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.955208 pyFipper-0.1.2.dev3/pyFipper.egg-info/
--rw-rw-rw-   0        0        0     2230 2023-05-24 09:13:39.000000 pyFipper-0.1.2.dev3/pyFipper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18746 2023-05-24 09:13:39.000000 pyFipper-0.1.2.dev3/pyFipper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:13:39.000000 pyFipper-0.1.2.dev3/pyFipper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 09:13:39.000000 pyFipper-0.1.2.dev3/pyFipper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       54 2023-05-24 09:13:39.000000 pyFipper-0.1.2.dev3/pyFipper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 09:13:39.000000 pyFipper-0.1.2.dev3/pyFipper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.992187 pyFipper-0.1.2.dev3/pyrogram/
--rw-rw-rw-   0        0        0     1447 2023-05-24 09:13:14.000000 pyFipper-0.1.2.dev3/pyrogram/__init__.py
--rw-rw-rw-   0        0        0    43160 2023-05-24 09:13:14.000000 pyFipper-0.1.2.dev3/pyrogram/client.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.996184 pyFipper-0.1.2.dev3/pyrogram/connection/
--rw-rw-rw-   0        0        0      873 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/__init__.py
--rw-rw-rw-   0        0        0     2916 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/connection.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:39.999184 pyFipper-0.1.2.dev3/pyrogram/connection/transport/
--rw-rw-rw-   0        0        0      857 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.014173 pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/
--rw-rw-rw-   0        0        0     1068 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/__init__.py
--rw-rw-rw-   0        0        0     4225 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp.py
--rw-rw-rw-   0        0        0     1825 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-rw-rw-   0        0        0     2916 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-rw-rw-   0        0        0     1970 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_full.py
--rw-rw-rw-   0        0        0     1556 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-rw-rw-   0        0        0     2532 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.027163 pyFipper-0.1.2.dev3/pyrogram/crypto/
--rw-rw-rw-   0        0        0      835 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/crypto/__init__.py
--rw-rw-rw-   0        0        0     4143 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/crypto/aes.py
--rw-rw-rw-   0        0        0     4894 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/crypto/mtproto.py
--rw-rw-rw-   0        0        0     2528 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/crypto/prime.py
--rw-rw-rw-   0        0        0    11002 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/crypto/rsa.py
--rw-rw-rw-   0        0        0    10485 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/dispatcher.py
--rw-rw-rw-   0        0        0   212040 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/emoji.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.062142 pyFipper-0.1.2.dev3/pyrogram/enums/
--rw-rw-rw-   0        0        0     1785 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/auto_name.py
--rw-rw-rw-   0        0        0     2379 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/chat_action.py
--rw-rw-rw-   0        0        0     4330 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/chat_event_action.py
--rw-rw-rw-   0        0        0     1308 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/chat_member_status.py
--rw-rw-rw-   0        0        0     1488 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/chat_members_filter.py
--rw-rw-rw-   0        0        0     1278 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/chat_type.py
--rw-rw-rw-   0        0        0     2548 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/message_entity_type.py
--rw-rw-rw-   0        0        0     1669 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/message_media_type.py
--rw-rw-rw-   0        0        0     1973 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/message_service_type.py
--rw-rw-rw-   0        0        0     2481 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/messages_filter.py
--rw-rw-rw-   0        0        0     1460 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/next_code_type.py
--rw-rw-rw-   0        0        0     1225 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/parse_mode.py
--rw-rw-rw-   0        0        0     1078 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/poll_type.py
--rw-rw-rw-   0        0        0     1571 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/sent_code_type.py
--rw-rw-rw-   0        0        0     1342 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/enums/user_status.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.068138 pyFipper-0.1.2.dev3/pyrogram/errors/
--rw-rw-rw-   0        0        0     2659 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/errors/__init__.py
--rw-rw-rw-   0        0        0     3418 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/errors/rpc_error.py
--rw-rw-rw-   0        0        0    15635 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/file_id.py
--rw-rw-rw-   0        0        0    25527 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/filters.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.101118 pyFipper-0.1.2.dev3/pyrogram/handlers/
--rw-rw-rw-   0        0        0     1560 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/__init__.py
--rw-rw-rw-   0        0        0     2075 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/callback_query_handler.py
--rw-rw-rw-   0        0        0     2060 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/chat_join_request_handler.py
--rw-rw-rw-   0        0        0     2095 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/chat_member_updated_handler.py
--rw-rw-rw-   0        0        0     2151 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/chosen_inline_result_handler.py
--rw-rw-rw-   0        0        0     2508 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/conversation_handler.py
--rw-rw-rw-   0        0        0     2604 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/deleted_messages_handler.py
--rw-rw-rw-   0        0        0     1745 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/disconnect_handler.py
--rw-rw-rw-   0        0        0     2028 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/edited_message_handler.py
--rw-rw-rw-   0        0        0     1593 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/handler.py
--rw-rw-rw-   0        0        0     2033 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/inline_query_handler.py
--rw-rw-rw-   0        0        0     2910 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/message_handler.py
--rw-rw-rw-   0        0        0     1964 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/poll_handler.py
--rw-rw-rw-   0        0        0     3009 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/raw_update_handler.py
--rw-rw-rw-   0        0        0     2036 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/handlers/user_status_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.103116 pyFipper-0.1.2.dev3/pyrogram/methods/
--rw-rw-rw-   0        0        0     1365 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.111111 pyFipper-0.1.2.dev3/pyrogram/methods/advanced/
--rw-rw-rw-   0        0        0     1017 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/advanced/__init__.py
--rw-rw-rw-   0        0        0     3222 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/advanced/invoke.py
--rw-rw-rw-   0        0        0     4685 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/advanced/resolve_peer.py
--rw-rw-rw-   0        0        0     8394 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/advanced/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.158591 pyFipper-0.1.2.dev3/pyrogram/methods/auth/
--rw-rw-rw-   0        0        0     1708 2023-05-24 08:53:09.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/__init__.py
--rw-rw-rw-   0        0        0     1512 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/accept_terms_of_service.py
--rw-rw-rw-   0        0        0     2002 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/check_password.py
--rw-rw-rw-   0        0        0     1800 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/connect.py
--rw-rw-rw-   0        0        0     1544 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/disconnect.py
--rw-rw-rw-   0        0        0     1345 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/get_password_hint.py
--rw-rw-rw-   0        0        0     1790 2023-05-24 09:13:14.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/initialize.py
--rw-rw-rw-   0        0        0     1677 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/log_out.py
--rw-rw-rw-   0        0        0     1888 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/recover_password.py
--rw-rw-rw-   0        0        0     2214 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/resend_code.py
--rw-rw-rw-   0        0        0     2865 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/send_code.py
--rw-rw-rw-   0        0        0     1516 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/send_recovery_code.py
--rw-rw-rw-   0        0        0     3165 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/sign_in.py
--rw-rw-rw-   0        0        0     2802 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/sign_in_bot.py
--rw-rw-rw-   0        0        0     2428 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/sign_up.py
--rw-rw-rw-   0        0        0     1913 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/auth/terminate.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.197567 pyFipper-0.1.2.dev3/pyrogram/methods/bots/
--rw-rw-rw-   0        0        0     2096 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/answer_callback_query.py
--rw-rw-rw-   0        0        0     5102 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/answer_inline_query.py
--rw-rw-rw-   0        0        0     2042 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/answer_web_app_query.py
--rw-rw-rw-   0        0        0     2422 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/delete_bot_commands.py
--rw-rw-rw-   0        0        0     2640 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_bot_commands.py
--rw-rw-rw-   0        0        0     2110 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-rw-rw-   0        0        0     2385 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_chat_menu_button.py
--rw-rw-rw-   0        0        0     2870 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_game_high_scores.py
--rw-rw-rw-   0        0        0     3457 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_inline_bot_results.py
--rw-rw-rw-   0        0        0     2924 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/request_callback_answer.py
--rw-rw-rw-   0        0        0     4056 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/send_game.py
--rw-rw-rw-   0        0        0     2883 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/send_inline_bot_result.py
--rw-rw-rw-   0        0        0     2783 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/set_bot_commands.py
--rw-rw-rw-   0        0        0     3267 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-rw-rw-   0        0        0     2104 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/set_chat_menu_button.py
--rw-rw-rw-   0        0        0     4046 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/bots/set_game_score.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.291509 pyFipper-0.1.2.dev3/pyrogram/methods/chats/
--rw-rw-rw-   0        0        0     3540 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/__init__.py
--rw-rw-rw-   0        0        0     3454 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/add_chat_members.py
--rw-rw-rw-   0        0        0     2287 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/archive_chats.py
--rw-rw-rw-   0        0        0     4731 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/ban_chat_member.py
--rw-rw-rw-   0        0        0     1873 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/create_channel.py
--rw-rw-rw-   0        0        0     2348 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/create_group.py
--rw-rw-rw-   0        0        0     2015 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/create_supergroup.py
--rw-rw-rw-   0        0        0     1637 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/delete_channel.py
--rw-rw-rw-   0        0        0     2377 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/delete_chat_photo.py
--rw-rw-rw-   0        0        0     1655 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/delete_supergroup.py
--rw-rw-rw-   0        0        0     2024 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/delete_user_history.py
--rw-rw-rw-   0        0        0     3369 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat.py
--rw-rw-rw-   0        0        0     4141 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_event_log.py
--rw-rw-rw-   0        0        0     3430 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_member.py
--rw-rw-rw-   0        0        0     5440 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_members.py
--rw-rw-rw-   0        0        0     2333 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_members_count.py
--rw-rw-rw-   0        0        0     1774 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_online_count.py
--rw-rw-rw-   0        0        0     3464 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_dialogs.py
--rw-rw-rw-   0        0        0     2159 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_dialogs_count.py
--rw-rw-rw-   0        0        0     2479 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_nearby_chats.py
--rw-rw-rw-   0        0        0     2201 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_send_as_chats.py
--rw-rw-rw-   0        0        0     2768 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/join_chat.py
--rw-rw-rw-   0        0        0     2682 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/leave_chat.py
--rw-rw-rw-   0        0        0     1575 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/mark_chat_unread.py
--rw-rw-rw-   0        0        0     3238 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/pin_chat_message.py
--rw-rw-rw-   0        0        0     3962 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/promote_chat_member.py
--rw-rw-rw-   0        0        0     4411 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/restrict_chat_member.py
--rw-rw-rw-   0        0        0     3221 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_administrator_title.py
--rw-rw-rw-   0        0        0     2313 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_description.py
--rw-rw-rw-   0        0        0     3502 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_permissions.py
--rw-rw-rw-   0        0        0     4722 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_photo.py
--rw-rw-rw-   0        0        0     1780 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_protected_content.py
--rw-rw-rw-   0        0        0     2650 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_title.py
--rw-rw-rw-   0        0        0     2364 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_username.py
--rw-rw-rw-   0        0        0     2039 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_send_as_chat.py
--rw-rw-rw-   0        0        0     2146 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_slow_mode.py
--rw-rw-rw-   0        0        0     2301 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/unarchive_chats.py
--rw-rw-rw-   0        0        0     2369 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/unban_chat_member.py
--rw-rw-rw-   0        0        0     1995 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-rw-rw-   0        0        0     2200 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/chats/unpin_chat_message.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.305500 pyFipper-0.1.2.dev3/pyrogram/methods/contacts/
--rw-rw-rw-   0        0        0     1187 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/contacts/__init__.py
--rw-rw-rw-   0        0        0     2644 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/contacts/add_contact.py
--rw-rw-rw-   0        0        0     2514 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/contacts/delete_contacts.py
--rw-rw-rw-   0        0        0     1652 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/contacts/get_contacts.py
--rw-rw-rw-   0        0        0     1463 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/contacts/get_contacts_count.py
--rw-rw-rw-   0        0        0     1992 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/contacts/import_contacts.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.334483 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/
--rw-rw-rw-   0        0        0     1671 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_callback_query.py
--rw-rw-rw-   0        0        0     2229 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_chat_join_request.py
--rw-rw-rw-   0        0        0     2250 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-rw-rw-   0        0        0     2278 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-rw-rw-   0        0        0     2244 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_deleted_messages.py
--rw-rw-rw-   0        0        0     1596 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_disconnect.py
--rw-rw-rw-   0        0        0     2233 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_edited_message.py
--rw-rw-rw-   0        0        0     2228 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_inline_query.py
--rw-rw-rw-   0        0        0     2199 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_message.py
--rw-rw-rw-   0        0        0     2181 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_poll.py
--rw-rw-rw-   0        0        0     1873 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_raw_update.py
--rw-rw-rw-   0        0        0     2213 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_user_status.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.385452 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/
--rw-rw-rw-   0        0        0     2493 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-rw-rw-   0        0        0     1981 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-rw-rw-   0        0        0     3456 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-rw-rw-   0        0        0     1950 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-rw-rw-   0        0        0     1982 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-rw-rw-   0        0        0     2085 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-rw-rw-   0        0        0     1803 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-rw-rw-   0        0        0     3625 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-rw-rw-   0        0        0     2647 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-rw-rw-   0        0        0     3666 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-rw-rw-   0        0        0     2397 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-rw-rw-   0        0        0     2053 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-rw-rw-   0        0        0     1981 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-rw-rw-   0        0        0     3015 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-rw-rw-   0        0        0     1985 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-rw-rw-   0        0        0     3035 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-rw-rw-   0        0        0     2397 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.570337 pyFipper-0.1.2.dev3/pyrogram/methods/messages/
--rw-rw-rw-   0        0        0     4194 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/__init__.py
--rw-rw-rw-   0        0        0     6103 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/copy_media_group.py
--rw-rw-rw-   0        0        0     5300 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/copy_message.py
--rw-rw-rw-   0        0        0     3232 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/delete_messages.py
--rw-rw-rw-   0        0        0     7717 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/download_media.py
--rw-rw-rw-   0        0        0     2336 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_inline_caption.py
--rw-rw-rw-   0        0        0    10010 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_inline_media.py
--rw-rw-rw-   0        0        0     2533 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-rw-rw-   0        0        0     3203 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_inline_text.py
--rw-rw-rw-   0        0        0     3054 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_message_caption.py
--rw-rw-rw-   0        0        0    12745 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_message_media.py
--rw-rw-rw-   0        0        0     3053 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-rw-rw-   0        0        0     4004 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_message_text.py
--rw-rw-rw-   0        0        0     4674 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/forward_messages.py
--rw-rw-rw-   0        0        0     4162 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_chat_history.py
--rw-rw-rw-   0        0        0     2461 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_chat_history_count.py
--rw-rw-rw-   0        0        0     2035 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-rw-rw-   0        0        0     2294 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_discussion_message.py
--rw-rw-rw-   0        0        0     2894 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_discussion_replies.py
--rw-rw-rw-   0        0        0     2012 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-rw-rw-   0        0        0     3019 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_media_group.py
--rw-rw-rw-   0        0        0     4860 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_messages.py
--rw-rw-rw-   0        0        0     2239 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/inline_session.py
--rw-rw-rw-   0        0        0     2600 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/read_chat_history.py
--rw-rw-rw-   0        0        0     2185 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/retract_vote.py
--rw-rw-rw-   0        0        0     4277 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/search_global.py
--rw-rw-rw-   0        0        0     2218 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/search_global_count.py
--rw-rw-rw-   0        0        0     5500 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/search_messages.py
--rw-rw-rw-   0        0        0     3287 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/search_messages_count.py
--rw-rw-rw-   0        0        0    12545 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_animation.py
--rw-rw-rw-   0        0        0    11360 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_audio.py
--rw-rw-rw-   0        0        0     5603 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_cached_media.py
--rw-rw-rw-   0        0        0     2897 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_chat_action.py
--rw-rw-rw-   0        0        0     4988 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_contact.py
--rw-rw-rw-   0        0        0     4957 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_dice.py
--rw-rw-rw-   0        0        0    10688 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_document.py
--rw-rw-rw-   0        0        0     4689 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_location.py
--rw-rw-rw-   0        0        0    19667 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_media_group.py
--rw-rw-rw-   0        0        0     7442 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_message.py
--rw-rw-rw-   0        0        0     9335 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_photo.py
--rw-rw-rw-   0        0        0     8252 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_poll.py
--rw-rw-rw-   0        0        0     2434 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_reaction.py
--rw-rw-rw-   0        0        0     8517 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_sticker.py
--rw-rw-rw-   0        0        0     5534 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_venue.py
--rw-rw-rw-   0        0        0    11909 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_video.py
--rw-rw-rw-   0        0        0     9515 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_video_note.py
--rw-rw-rw-   0        0        0     9632 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_voice.py
--rw-rw-rw-   0        0        0     2896 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/stop_poll.py
--rw-rw-rw-   0        0        0     4043 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/stream_media.py
--rw-rw-rw-   0        0        0     2573 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/vote_poll.py
--rw-rw-rw-   0        0        0     2901 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/wait_for_callback_query.py
--rw-rw-rw-   0        0        0     2822 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/messages/wait_for_message.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.584329 pyFipper-0.1.2.dev3/pyrogram/methods/password/
--rw-rw-rw-   0        0        0     1117 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/password/__init__.py
--rw-rw-rw-   0        0        0     2879 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/password/change_cloud_password.py
--rw-rw-rw-   0        0        0     3094 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/password/enable_cloud_password.py
--rw-rw-rw-   0        0        0     2207 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/password/remove_cloud_password.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.617308 pyFipper-0.1.2.dev3/pyrogram/methods/users/
--rw-rw-rw-   0        0        0     1708 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/__init__.py
--rw-rw-rw-   0        0        0     1825 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/block_user.py
--rw-rw-rw-   0        0        0     2300 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/delete_profile_photos.py
--rw-rw-rw-   0        0        0     4556 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/get_chat_photos.py
--rw-rw-rw-   0        0        0     2583 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/get_chat_photos_count.py
--rw-rw-rw-   0        0        0     2426 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/get_common_chats.py
--rw-rw-rw-   0        0        0     1711 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-rw-rw-   0        0        0     1614 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/get_me.py
--rw-rw-rw-   0        0        0     2633 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/get_users.py
--rw-rw-rw-   0        0        0     1940 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/set_emoji_status.py
--rw-rw-rw-   0        0        0     2793 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/set_profile_photo.py
--rw-rw-rw-   0        0        0     1933 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/set_username.py
--rw-rw-rw-   0        0        0     1835 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/unblock_user.py
--rw-rw-rw-   0        0        0     2448 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/users/update_profile.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.643292 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/
--rw-rw-rw-   0        0        0     1292 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/__init__.py
--rw-rw-rw-   0        0        0     2413 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/add_handler.py
--rw-rw-rw-   0        0        0     2310 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/compose.py
--rw-rw-rw-   0        0        0     1597 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/export_session_string.py
--rw-rw-rw-   0        0        0     2837 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/idle.py
--rw-rw-rw-   0        0        0     2273 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/remove_handler.py
--rw-rw-rw-   0        0        0     2366 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/restart.py
--rw-rw-rw-   0        0        0     2943 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/run.py
--rw-rw-rw-   0        0        0     2442 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/start.py
--rw-rw-rw-   0        0        0     2186 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/stop.py
--rw-rw-rw-   0        0        0     1753 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/methods/utilities/stop_transmission.py
--rw-rw-rw-   0        0        0    63796 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/mime_types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.658284 pyFipper-0.1.2.dev3/pyrogram/parser/
--rw-rw-rw-   0        0        0      865 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/parser/__init__.py
--rw-rw-rw-   0        0        0     7599 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/parser/html.py
--rw-rw-rw-   0        0        0     5943 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/parser/markdown.py
--rw-rw-rw-   0        0        0     2138 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/parser/parser.py
--rw-rw-rw-   0        0        0     1586 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/parser/utils.py
--rw-rw-rw-   0        0        0        0 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.660282 pyFipper-0.1.2.dev3/pyrogram/raw/
--rw-rw-rw-   0        0        0     1066 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.678269 pyFipper-0.1.2.dev3/pyrogram/raw/core/
--rw-rw-rw-   0        0        0     1343 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/__init__.py
--rw-rw-rw-   0        0        0     1745 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/future_salt.py
--rw-rw-rw-   0        0        0     1954 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/future_salts.py
--rw-rw-rw-   0        0        0     1876 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/gzip_packed.py
--rw-rw-rw-   0        0        0     1074 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/list.py
--rw-rw-rw-   0        0        0     1907 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/message.py
--rw-rw-rw-   0        0        0     1667 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/msg_container.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.695260 pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/
--rw-rw-rw-   0        0        0     1036 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/bool.py
--rw-rw-rw-   0        0        0     1814 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/bytes.py
--rw-rw-rw-   0        0        0     1225 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/double.py
--rw-rw-rw-   0        0        0     1403 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/int.py
--rw-rw-rw-   0        0        0     1225 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/string.py
--rw-rw-rw-   0        0        0     2081 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/vector.py
--rw-rw-rw-   0        0        0     2577 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/raw/core/tl_object.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.703256 pyFipper-0.1.2.dev3/pyrogram/session/
--rw-rw-rw-   0        0        0      891 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/session/__init__.py
--rw-rw-rw-   0        0        0    10774 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/session/auth.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.713248 pyFipper-0.1.2.dev3/pyrogram/session/internals/
--rw-rw-rw-   0        0        0      938 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/session/internals/__init__.py
--rw-rw-rw-   0        0        0     2446 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/session/internals/data_center.py
--rw-rw-rw-   0        0        0     1412 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/session/internals/msg_factory.py
--rw-rw-rw-   0        0        0     1632 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/session/internals/msg_id.py
--rw-rw-rw-   0        0        0     1291 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/session/internals/seq_no.py
--rw-rw-rw-   0        0        0    12821 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/session/session.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.724242 pyFipper-0.1.2.dev3/pyrogram/storage/
--rw-rw-rw-   0        0        0      949 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/storage/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/storage/file_storage.py
--rw-rw-rw-   0        0        0     2823 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/storage/memory_storage.py
--rw-rw-rw-   0        0        0     6640 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/storage/sqlite_storage.py
--rw-rw-rw-   0        0        0     2872 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/storage/storage.py
--rw-rw-rw-   0        0        0     3852 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/sync.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.733238 pyFipper-0.1.2.dev3/pyrogram/types/
--rw-rw-rw-   0        0        0     1137 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.741231 pyFipper-0.1.2.dev3/pyrogram/types/authorization/
--rw-rw-rw-   0        0        0      960 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/authorization/__init__.py
--rw-rw-rw-   0        0        0     2350 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/authorization/sent_code.py
--rw-rw-rw-   0        0        0     1986 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/authorization/terms_of_service.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.811187 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/
--rw-rw-rw-   0        0        0     2901 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/__init__.py
--rw-rw-rw-   0        0        0     1791 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-rw-rw-   0        0        0     2861 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-rw-rw-   0        0        0     1325 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-rw-rw-   0        0        0     1290 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-rw-rw-   0        0        0     1281 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-rw-rw-   0        0        0     1605 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-rw-rw-   0        0        0     1682 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-rw-rw-   0        0        0     1865 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-rw-rw-   0        0        0     1341 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-rw-rw-   0        0        0     1058 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-rw-rw-   0        0        0    13110 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-rw-rw-   0        0        0     2449 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-rw-rw-   0        0        0     2286 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-rw-rw-   0        0        0     8328 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-rw-rw-   0        0        0     2536 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-rw-rw-   0        0        0     3609 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-rw-rw-   0        0        0     3802 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/login_url.py
--rw-rw-rw-   0        0        0     1647 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-rw-rw-   0        0        0     1241 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-rw-rw-   0        0        0     1244 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-rw-rw-   0        0        0     1860 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-rw-rw-   0        0        0     4231 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-rw-rw-   0        0        0     2397 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-rw-rw-   0        0        0     1606 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-rw-rw-   0        0        0     1350 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.860158 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/
--rw-rw-rw-   0        0        0     2802 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/__init__.py
--rw-rw-rw-   0        0        0     3761 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-rw-rw-   0        0        0     7479 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query.py
--rw-rw-rw-   0        0        0     2474 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result.py
--rw-rw-rw-   0        0        0     5931 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-rw-rw-   0        0        0     3403 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-rw-rw-   0        0        0     4625 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-rw-rw-   0        0        0     4353 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-rw-rw-   0        0        0     4130 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-rw-rw-   0        0        0     4501 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-rw-rw-   0        0        0     4423 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-rw-rw-   0        0        0     3109 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-rw-rw-   0        0        0     4508 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-rw-rw-   0        0        0     4310 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-rw-rw-   0        0        0     4246 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-rw-rw-   0        0        0     5385 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-rw-rw-   0        0        0     4741 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-rw-rw-   0        0        0     5408 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-rw-rw-   0        0        0     4885 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-rw-rw-   0        0        0     5625 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-rw-rw-   0        0        0     4474 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.878147 pyFipper-0.1.2.dev3/pyrogram/types/input_media/
--rw-rw-rw-   0        0        0     1344 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_media/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media.py
--rw-rw-rw-   0        0        0     3309 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_animation.py
--rw-rw-rw-   0        0        0     3364 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_audio.py
--rw-rw-rw-   0        0        0     2836 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_document.py
--rw-rw-rw-   0        0        0     2542 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_photo.py
--rw-rw-rw-   0        0        0     3506 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_video.py
--rw-rw-rw-   0        0        0     1788 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_phone_contact.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.884143 pyFipper-0.1.2.dev3/pyrogram/types/input_message_content/
--rw-rw-rw-   0        0        0     1030 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_message_content/__init__.py
--rw-rw-rw-   0        0        0     1453 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_message_content/input_message_content.py
--rw-rw-rw-   0        0        0     2706 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/input_message_content/input_text_message_content.py
--rw-rw-rw-   0        0        0     1123 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/list.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:40.942109 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/
--rw-rw-rw-   0        0        0     1883 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/__init__.py
--rw-rw-rw-   0        0        0     4165 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/animation.py
--rw-rw-rw-   0        0        0     4190 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/audio.py
--rw-rw-rw-   0        0        0     2278 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/contact.py
--rw-rw-rw-   0        0        0     1634 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/dice.py
--rw-rw-rw-   0        0        0     3507 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/document.py
--rw-rw-rw-   0        0        0     3143 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/game.py
--rw-rw-rw-   0        0        0     1715 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/location.py
--rw-rw-rw-   0        0        0   150763 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/message.py
--rw-rw-rw-   0        0        0     4476 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/message_entity.py
--rw-rw-rw-   0        0        0     1856 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/message_reactions.py
--rw-rw-rw-   0        0        0     4439 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/photo.py
--rw-rw-rw-   0        0        0     7240 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/poll.py
--rw-rw-rw-   0        0        0     1582 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/poll_option.py
--rw-rw-rw-   0        0        0     2703 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/reaction.py
--rw-rw-rw-   0        0        0     7115 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/sticker.py
--rw-rw-rw-   0        0        0     1478 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-rw-rw-   0        0        0     3866 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/thumbnail.py
--rw-rw-rw-   0        0        0     2365 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/venue.py
--rw-rw-rw-   0        0        0     4523 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/video.py
--rw-rw-rw-   0        0        0     3709 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/video_note.py
--rw-rw-rw-   0        0        0     3300 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/voice.py
--rw-rw-rw-   0        0        0     1616 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/web_app_data.py
--rw-rw-rw-   0        0        0     6538 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/web_page.py
--rw-rw-rw-   0        0        0     3983 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/object.py
--rw-rw-rw-   0        0        0     1029 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/update.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:41.012064 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/
--rw-rw-rw-   0        0        0     2364 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/__init__.py
--rw-rw-rw-   0        0        0    33812 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat.py
--rw-rw-rw-   0        0        0     2299 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-rw-rw-   0        0        0    20324 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_event.py
--rw-rw-rw-   0        0        0     5689 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-rw-rw-   0        0        0     4709 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-rw-rw-   0        0        0     4384 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_join_request.py
--rw-rw-rw-   0        0        0     2646 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_joiner.py
--rw-rw-rw-   0        0        0     9671 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_member.py
--rw-rw-rw-   0        0        0     3776 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-rw-rw-   0        0        0     4480 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_permissions.py
--rw-rw-rw-   0        0        0     4074 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_photo.py
--rw-rw-rw-   0        0        0     2671 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_preview.py
--rw-rw-rw-   0        0        0     5063 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_privileges.py
--rw-rw-rw-   0        0        0     2425 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_reactions.py
--rw-rw-rw-   0        0        0     2761 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/dialog.py
--rw-rw-rw-   0        0        0     2499 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/emoji_status.py
--rw-rw-rw-   0        0        0     2012 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-rw-rw-   0        0        0     1713 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/restriction.py
--rw-rw-rw-   0        0        0    13509 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/user.py
--rw-rw-rw-   0        0        0     1387 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-rw-rw-   0        0        0     1660 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-rw-rw-   0        0        0     1574 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-rw-rw-   0        0        0     1072 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/video_chat_started.py
--rw-rw-rw-   0        0        0    10943 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/pyrogram/utils.py
--rw-rw-rw-   0        0        0       57 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 09:13:41.026056 pyFipper-0.1.2.dev3/setup.cfg
--rw-rw-rw-   0        0        0     2124 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:41.017063 pyFipper-0.1.2.dev3/tests/
--rw-rw-rw-   0        0        0      835 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:41.022058 pyFipper-0.1.2.dev3/tests/filters/
--rw-rw-rw-   0        0        0     1237 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/tests/filters/__init__.py
--rw-rw-rw-   0        0        0     3520 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/tests/filters/test_command.py
--rw-rw-rw-   0        0        0     8402 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev3/tests/test_file_id.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:51.011127 pyFipper-0.1.2.dev4/
+-rw-rw-rw-   0        0        0    35184 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/LICENSE
+-rw-rw-rw-   0        0        0      301 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/MANIFEST.in
+-rw-rw-rw-   0        0        0      791 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/NOTICE
+-rw-rw-rw-   0        0        0     2230 2023-05-24 09:30:51.009129 pyFipper-0.1.2.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     1313 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:49.912804 pyFipper-0.1.2.dev4/compiler/
+-rw-rw-rw-   0        0        0      835 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:49.916802 pyFipper-0.1.2.dev4/compiler/api/
+-rw-rw-rw-   0        0        0      835 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/api/__init__.py
+-rw-rw-rw-   0        0        0    23054 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/api/compiler.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:49.923797 pyFipper-0.1.2.dev4/compiler/api/source/
+-rw-rw-rw-   0        0        0     2273 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/api/source/auth_key.tl
+-rw-rw-rw-   0        0        0   159892 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/api/source/main_api.tl
+-rw-rw-rw-   0        0        0     3501 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/api/source/sys_msgs.tl
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:49.927795 pyFipper-0.1.2.dev4/compiler/api/template/
+-rw-rw-rw-   0        0        0      778 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/api/template/combinator.txt
+-rw-rw-rw-   0        0        0      658 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/api/template/type.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:49.935791 pyFipper-0.1.2.dev4/compiler/errors/
+-rw-rw-rw-   0        0        0      835 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/__init__.py
+-rw-rw-rw-   0        0        0     5059 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/compiler.py
+-rw-rw-rw-   0        0        0     1298 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/sort.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:49.953779 pyFipper-0.1.2.dev4/compiler/errors/source/
+-rw-rw-rw-   0        0        0      475 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-rw-rw-   0        0        0    22646 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-rw-rw-   0        0        0      687 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-rw-rw-   0        0        0     2027 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-rw-rw-   0        0        0     1189 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-rw-rw-   0        0        0      475 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/source/420_FLOOD.tsv
+-rw-rw-rw-   0        0        0     4263 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-rw-rw-   0        0        0      157 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:49.957776 pyFipper-0.1.2.dev4/compiler/errors/template/
+-rw-rw-rw-   0        0        0      190 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/template/class.txt
+-rw-rw-rw-   0        0        0      127 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/compiler/errors/template/sub_class.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:49.995752 pyFipper-0.1.2.dev4/pyFipper.egg-info/
+-rw-rw-rw-   0        0        0     2230 2023-05-24 09:30:49.000000 pyFipper-0.1.2.dev4/pyFipper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18746 2023-05-24 09:30:49.000000 pyFipper-0.1.2.dev4/pyFipper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:30:49.000000 pyFipper-0.1.2.dev4/pyFipper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 09:30:49.000000 pyFipper-0.1.2.dev4/pyFipper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       54 2023-05-24 09:30:49.000000 pyFipper-0.1.2.dev4/pyFipper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 09:30:49.000000 pyFipper-0.1.2.dev4/pyFipper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.032730 pyFipper-0.1.2.dev4/pyrogram/
+-rw-rw-rw-   0        0        0     1447 2023-05-24 09:30:43.000000 pyFipper-0.1.2.dev4/pyrogram/__init__.py
+-rw-rw-rw-   0        0        0    43213 2023-05-24 09:30:43.000000 pyFipper-0.1.2.dev4/pyrogram/client.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.037728 pyFipper-0.1.2.dev4/pyrogram/connection/
+-rw-rw-rw-   0        0        0      873 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/__init__.py
+-rw-rw-rw-   0        0        0     2916 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/connection.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.039726 pyFipper-0.1.2.dev4/pyrogram/connection/transport/
+-rw-rw-rw-   0        0        0      857 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.056716 pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/
+-rw-rw-rw-   0        0        0     1068 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/__init__.py
+-rw-rw-rw-   0        0        0     4225 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp.py
+-rw-rw-rw-   0        0        0     1825 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-rw-rw-   0        0        0     2916 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-rw-rw-   0        0        0     1970 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-rw-rw-   0        0        0     1556 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-rw-rw-   0        0        0     2532 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.067708 pyFipper-0.1.2.dev4/pyrogram/crypto/
+-rw-rw-rw-   0        0        0      835 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/crypto/__init__.py
+-rw-rw-rw-   0        0        0     4143 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/crypto/aes.py
+-rw-rw-rw-   0        0        0     4894 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/crypto/mtproto.py
+-rw-rw-rw-   0        0        0     2528 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/crypto/prime.py
+-rw-rw-rw-   0        0        0    11002 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/crypto/rsa.py
+-rw-rw-rw-   0        0        0    10485 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/dispatcher.py
+-rw-rw-rw-   0        0        0   212040 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/emoji.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.103688 pyFipper-0.1.2.dev4/pyrogram/enums/
+-rw-rw-rw-   0        0        0     1785 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/__init__.py
+-rw-rw-rw-   0        0        0     1029 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/auto_name.py
+-rw-rw-rw-   0        0        0     2379 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/chat_action.py
+-rw-rw-rw-   0        0        0     4330 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/chat_event_action.py
+-rw-rw-rw-   0        0        0     1308 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/chat_member_status.py
+-rw-rw-rw-   0        0        0     1488 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/chat_members_filter.py
+-rw-rw-rw-   0        0        0     1278 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/chat_type.py
+-rw-rw-rw-   0        0        0     2548 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/message_entity_type.py
+-rw-rw-rw-   0        0        0     1669 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/message_media_type.py
+-rw-rw-rw-   0        0        0     1973 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/message_service_type.py
+-rw-rw-rw-   0        0        0     2481 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/messages_filter.py
+-rw-rw-rw-   0        0        0     1460 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/next_code_type.py
+-rw-rw-rw-   0        0        0     1225 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/parse_mode.py
+-rw-rw-rw-   0        0        0     1078 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/poll_type.py
+-rw-rw-rw-   0        0        0     1571 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/sent_code_type.py
+-rw-rw-rw-   0        0        0     1342 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/enums/user_status.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.108684 pyFipper-0.1.2.dev4/pyrogram/errors/
+-rw-rw-rw-   0        0        0     2659 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/errors/__init__.py
+-rw-rw-rw-   0        0        0     3418 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/errors/rpc_error.py
+-rw-rw-rw-   0        0        0    15635 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/file_id.py
+-rw-rw-rw-   0        0        0    25527 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/filters.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.142662 pyFipper-0.1.2.dev4/pyrogram/handlers/
+-rw-rw-rw-   0        0        0     1560 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2075 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/callback_query_handler.py
+-rw-rw-rw-   0        0        0     2060 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/chat_join_request_handler.py
+-rw-rw-rw-   0        0        0     2095 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/chat_member_updated_handler.py
+-rw-rw-rw-   0        0        0     2151 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-rw-rw-   0        0        0     2508 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/conversation_handler.py
+-rw-rw-rw-   0        0        0     2604 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/deleted_messages_handler.py
+-rw-rw-rw-   0        0        0     1745 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/disconnect_handler.py
+-rw-rw-rw-   0        0        0     2028 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/edited_message_handler.py
+-rw-rw-rw-   0        0        0     1593 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/handler.py
+-rw-rw-rw-   0        0        0     2033 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/inline_query_handler.py
+-rw-rw-rw-   0        0        0     2910 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/message_handler.py
+-rw-rw-rw-   0        0        0     1964 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/poll_handler.py
+-rw-rw-rw-   0        0        0     3009 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/raw_update_handler.py
+-rw-rw-rw-   0        0        0     2036 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/handlers/user_status_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.144662 pyFipper-0.1.2.dev4/pyrogram/methods/
+-rw-rw-rw-   0        0        0     1365 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.152655 pyFipper-0.1.2.dev4/pyrogram/methods/advanced/
+-rw-rw-rw-   0        0        0     1017 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/advanced/__init__.py
+-rw-rw-rw-   0        0        0     3222 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/advanced/invoke.py
+-rw-rw-rw-   0        0        0     4685 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/advanced/resolve_peer.py
+-rw-rw-rw-   0        0        0     8394 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/advanced/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.203626 pyFipper-0.1.2.dev4/pyrogram/methods/auth/
+-rw-rw-rw-   0        0        0     1708 2023-05-24 08:53:09.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/__init__.py
+-rw-rw-rw-   0        0        0     1512 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-rw-rw-   0        0        0     2002 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/check_password.py
+-rw-rw-rw-   0        0        0     1800 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/connect.py
+-rw-rw-rw-   0        0        0     1544 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/disconnect.py
+-rw-rw-rw-   0        0        0     1345 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/get_password_hint.py
+-rw-rw-rw-   0        0        0     1713 2023-05-24 09:30:43.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/initialize.py
+-rw-rw-rw-   0        0        0     1677 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/log_out.py
+-rw-rw-rw-   0        0        0     1888 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/recover_password.py
+-rw-rw-rw-   0        0        0     2214 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/resend_code.py
+-rw-rw-rw-   0        0        0     2865 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/send_code.py
+-rw-rw-rw-   0        0        0     1516 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/send_recovery_code.py
+-rw-rw-rw-   0        0        0     3165 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/sign_in.py
+-rw-rw-rw-   0        0        0     2802 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/sign_in_bot.py
+-rw-rw-rw-   0        0        0     2428 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/sign_up.py
+-rw-rw-rw-   0        0        0     1913 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/auth/terminate.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.247597 pyFipper-0.1.2.dev4/pyrogram/methods/bots/
+-rw-rw-rw-   0        0        0     2096 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/__init__.py
+-rw-rw-rw-   0        0        0     3392 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/answer_callback_query.py
+-rw-rw-rw-   0        0        0     5102 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/answer_inline_query.py
+-rw-rw-rw-   0        0        0     2042 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/answer_web_app_query.py
+-rw-rw-rw-   0        0        0     2422 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/delete_bot_commands.py
+-rw-rw-rw-   0        0        0     2640 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_bot_commands.py
+-rw-rw-rw-   0        0        0     2110 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-rw-rw-   0        0        0     2385 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-rw-rw-   0        0        0     2870 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_game_high_scores.py
+-rw-rw-rw-   0        0        0     3457 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-rw-rw-   0        0        0     2924 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/request_callback_answer.py
+-rw-rw-rw-   0        0        0     4056 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/send_game.py
+-rw-rw-rw-   0        0        0     2883 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-rw-rw-   0        0        0     2783 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/set_bot_commands.py
+-rw-rw-rw-   0        0        0     3267 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-rw-rw-   0        0        0     2104 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-rw-rw-   0        0        0     4046 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/bots/set_game_score.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.342539 pyFipper-0.1.2.dev4/pyrogram/methods/chats/
+-rw-rw-rw-   0        0        0     3540 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0     3454 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/add_chat_members.py
+-rw-rw-rw-   0        0        0     2287 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/archive_chats.py
+-rw-rw-rw-   0        0        0     4731 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/ban_chat_member.py
+-rw-rw-rw-   0        0        0     1873 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/create_channel.py
+-rw-rw-rw-   0        0        0     2348 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/create_group.py
+-rw-rw-rw-   0        0        0     2015 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/create_supergroup.py
+-rw-rw-rw-   0        0        0     1637 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/delete_channel.py
+-rw-rw-rw-   0        0        0     2377 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/delete_chat_photo.py
+-rw-rw-rw-   0        0        0     1655 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/delete_supergroup.py
+-rw-rw-rw-   0        0        0     2024 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/delete_user_history.py
+-rw-rw-rw-   0        0        0     3369 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat.py
+-rw-rw-rw-   0        0        0     4141 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_event_log.py
+-rw-rw-rw-   0        0        0     3430 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_member.py
+-rw-rw-rw-   0        0        0     5440 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_members.py
+-rw-rw-rw-   0        0        0     2333 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_members_count.py
+-rw-rw-rw-   0        0        0     1774 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_online_count.py
+-rw-rw-rw-   0        0        0     3464 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_dialogs.py
+-rw-rw-rw-   0        0        0     2159 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_dialogs_count.py
+-rw-rw-rw-   0        0        0     2479 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_nearby_chats.py
+-rw-rw-rw-   0        0        0     2201 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_send_as_chats.py
+-rw-rw-rw-   0        0        0     2768 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/join_chat.py
+-rw-rw-rw-   0        0        0     2682 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/leave_chat.py
+-rw-rw-rw-   0        0        0     1575 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/mark_chat_unread.py
+-rw-rw-rw-   0        0        0     3238 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/pin_chat_message.py
+-rw-rw-rw-   0        0        0     3962 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/promote_chat_member.py
+-rw-rw-rw-   0        0        0     4411 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/restrict_chat_member.py
+-rw-rw-rw-   0        0        0     3221 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_administrator_title.py
+-rw-rw-rw-   0        0        0     2313 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_description.py
+-rw-rw-rw-   0        0        0     3502 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_permissions.py
+-rw-rw-rw-   0        0        0     4722 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_photo.py
+-rw-rw-rw-   0        0        0     1780 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-rw-rw-   0        0        0     2650 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_title.py
+-rw-rw-rw-   0        0        0     2364 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_username.py
+-rw-rw-rw-   0        0        0     2039 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_send_as_chat.py
+-rw-rw-rw-   0        0        0     2146 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_slow_mode.py
+-rw-rw-rw-   0        0        0     2301 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/unarchive_chats.py
+-rw-rw-rw-   0        0        0     2369 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/unban_chat_member.py
+-rw-rw-rw-   0        0        0     1995 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-rw-rw-   0        0        0     2200 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/chats/unpin_chat_message.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.355533 pyFipper-0.1.2.dev4/pyrogram/methods/contacts/
+-rw-rw-rw-   0        0        0     1187 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/contacts/__init__.py
+-rw-rw-rw-   0        0        0     2644 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/contacts/add_contact.py
+-rw-rw-rw-   0        0        0     2514 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/contacts/delete_contacts.py
+-rw-rw-rw-   0        0        0     1652 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/contacts/get_contacts.py
+-rw-rw-rw-   0        0        0     1463 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/contacts/get_contacts_count.py
+-rw-rw-rw-   0        0        0     1992 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/contacts/import_contacts.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.385512 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/
+-rw-rw-rw-   0        0        0     1671 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_callback_query.py
+-rw-rw-rw-   0        0        0     2229 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-rw-rw-   0        0        0     2250 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-rw-rw-   0        0        0     2278 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-rw-rw-   0        0        0     2244 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-rw-rw-   0        0        0     1596 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_disconnect.py
+-rw-rw-rw-   0        0        0     2233 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_edited_message.py
+-rw-rw-rw-   0        0        0     2228 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_inline_query.py
+-rw-rw-rw-   0        0        0     2199 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_message.py
+-rw-rw-rw-   0        0        0     2181 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_poll.py
+-rw-rw-rw-   0        0        0     1873 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_raw_update.py
+-rw-rw-rw-   0        0        0     2213 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_user_status.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.428486 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/
+-rw-rw-rw-   0        0        0     2493 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-rw-rw-   0        0        0     1981 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-rw-rw-   0        0        0     3456 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-rw-rw-   0        0        0     1950 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-rw-rw-   0        0        0     1982 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-rw-rw-   0        0        0     2085 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-rw-rw-   0        0        0     1803 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3625 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-rw-rw-   0        0        0     2647 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3666 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-rw-rw-   0        0        0     2397 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-rw-rw-   0        0        0     2053 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-rw-rw-   0        0        0     1981 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3015 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-rw-rw-   0        0        0     1985 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-rw-rw-   0        0        0     3035 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-rw-rw-   0        0        0     2397 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.570398 pyFipper-0.1.2.dev4/pyrogram/methods/messages/
+-rw-rw-rw-   0        0        0     4194 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0     6103 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/copy_media_group.py
+-rw-rw-rw-   0        0        0     5300 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/copy_message.py
+-rw-rw-rw-   0        0        0     3232 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/delete_messages.py
+-rw-rw-rw-   0        0        0     7717 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/download_media.py
+-rw-rw-rw-   0        0        0     2336 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_inline_caption.py
+-rw-rw-rw-   0        0        0    10010 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_inline_media.py
+-rw-rw-rw-   0        0        0     2533 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-rw-rw-   0        0        0     3203 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_inline_text.py
+-rw-rw-rw-   0        0        0     3054 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_message_caption.py
+-rw-rw-rw-   0        0        0    12745 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_message_media.py
+-rw-rw-rw-   0        0        0     3053 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-rw-rw-   0        0        0     4004 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_message_text.py
+-rw-rw-rw-   0        0        0     4674 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/forward_messages.py
+-rw-rw-rw-   0        0        0     4162 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_chat_history.py
+-rw-rw-rw-   0        0        0     2461 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_chat_history_count.py
+-rw-rw-rw-   0        0        0     2035 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-rw-rw-   0        0        0     2294 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_discussion_message.py
+-rw-rw-rw-   0        0        0     2894 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_discussion_replies.py
+-rw-rw-rw-   0        0        0     2012 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-rw-rw-   0        0        0     3019 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_media_group.py
+-rw-rw-rw-   0        0        0     4860 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_messages.py
+-rw-rw-rw-   0        0        0     2239 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/inline_session.py
+-rw-rw-rw-   0        0        0     2600 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/read_chat_history.py
+-rw-rw-rw-   0        0        0     2185 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/retract_vote.py
+-rw-rw-rw-   0        0        0     4277 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/search_global.py
+-rw-rw-rw-   0        0        0     2218 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/search_global_count.py
+-rw-rw-rw-   0        0        0     5500 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/search_messages.py
+-rw-rw-rw-   0        0        0     3287 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/search_messages_count.py
+-rw-rw-rw-   0        0        0    12545 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_animation.py
+-rw-rw-rw-   0        0        0    11360 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_audio.py
+-rw-rw-rw-   0        0        0     5603 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_cached_media.py
+-rw-rw-rw-   0        0        0     2897 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_chat_action.py
+-rw-rw-rw-   0        0        0     4988 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_contact.py
+-rw-rw-rw-   0        0        0     4957 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_dice.py
+-rw-rw-rw-   0        0        0    10688 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_document.py
+-rw-rw-rw-   0        0        0     4689 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_location.py
+-rw-rw-rw-   0        0        0    19667 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_media_group.py
+-rw-rw-rw-   0        0        0     7442 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     9335 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_photo.py
+-rw-rw-rw-   0        0        0     8252 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_poll.py
+-rw-rw-rw-   0        0        0     2434 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_reaction.py
+-rw-rw-rw-   0        0        0     8517 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_sticker.py
+-rw-rw-rw-   0        0        0     5534 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_venue.py
+-rw-rw-rw-   0        0        0    11909 2023-05-24 07:27:38.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_video.py
+-rw-rw-rw-   0        0        0     9515 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_video_note.py
+-rw-rw-rw-   0        0        0     9632 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_voice.py
+-rw-rw-rw-   0        0        0     2896 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/stop_poll.py
+-rw-rw-rw-   0        0        0     4043 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/stream_media.py
+-rw-rw-rw-   0        0        0     2573 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/vote_poll.py
+-rw-rw-rw-   0        0        0     2901 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/wait_for_callback_query.py
+-rw-rw-rw-   0        0        0     2822 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/messages/wait_for_message.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.579393 pyFipper-0.1.2.dev4/pyrogram/methods/password/
+-rw-rw-rw-   0        0        0     1117 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/password/__init__.py
+-rw-rw-rw-   0        0        0     2879 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/password/change_cloud_password.py
+-rw-rw-rw-   0        0        0     3094 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/password/enable_cloud_password.py
+-rw-rw-rw-   0        0        0     2207 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/password/remove_cloud_password.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.612372 pyFipper-0.1.2.dev4/pyrogram/methods/users/
+-rw-rw-rw-   0        0        0     1708 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/__init__.py
+-rw-rw-rw-   0        0        0     1825 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/block_user.py
+-rw-rw-rw-   0        0        0     2300 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/delete_profile_photos.py
+-rw-rw-rw-   0        0        0     4556 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/get_chat_photos.py
+-rw-rw-rw-   0        0        0     2583 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/get_chat_photos_count.py
+-rw-rw-rw-   0        0        0     2426 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/get_common_chats.py
+-rw-rw-rw-   0        0        0     1711 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-rw-rw-   0        0        0     1614 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/get_me.py
+-rw-rw-rw-   0        0        0     2633 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/get_users.py
+-rw-rw-rw-   0        0        0     1940 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/set_emoji_status.py
+-rw-rw-rw-   0        0        0     2793 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/set_profile_photo.py
+-rw-rw-rw-   0        0        0     1933 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/set_username.py
+-rw-rw-rw-   0        0        0     1835 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/unblock_user.py
+-rw-rw-rw-   0        0        0     2448 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/users/update_profile.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.642354 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/
+-rw-rw-rw-   0        0        0     1292 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/add_handler.py
+-rw-rw-rw-   0        0        0     2310 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/compose.py
+-rw-rw-rw-   0        0        0     1597 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/export_session_string.py
+-rw-rw-rw-   0        0        0     2837 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/idle.py
+-rw-rw-rw-   0        0        0     2273 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/remove_handler.py
+-rw-rw-rw-   0        0        0     2366 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/restart.py
+-rw-rw-rw-   0        0        0     2943 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/run.py
+-rw-rw-rw-   0        0        0     2442 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/start.py
+-rw-rw-rw-   0        0        0     2186 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/stop.py
+-rw-rw-rw-   0        0        0     1753 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/methods/utilities/stop_transmission.py
+-rw-rw-rw-   0        0        0    63796 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/mime_types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.653347 pyFipper-0.1.2.dev4/pyrogram/parser/
+-rw-rw-rw-   0        0        0      865 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/parser/__init__.py
+-rw-rw-rw-   0        0        0     7599 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/parser/html.py
+-rw-rw-rw-   0        0        0     5943 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/parser/markdown.py
+-rw-rw-rw-   0        0        0     2138 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/parser/parser.py
+-rw-rw-rw-   0        0        0     1586 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/parser/utils.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.655346 pyFipper-0.1.2.dev4/pyrogram/raw/
+-rw-rw-rw-   0        0        0     1066 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.674334 pyFipper-0.1.2.dev4/pyrogram/raw/core/
+-rw-rw-rw-   0        0        0     1343 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/__init__.py
+-rw-rw-rw-   0        0        0     1745 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/future_salt.py
+-rw-rw-rw-   0        0        0     1954 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/future_salts.py
+-rw-rw-rw-   0        0        0     1876 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/gzip_packed.py
+-rw-rw-rw-   0        0        0     1074 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/list.py
+-rw-rw-rw-   0        0        0     1907 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/message.py
+-rw-rw-rw-   0        0        0     1667 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/msg_container.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.690324 pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/
+-rw-rw-rw-   0        0        0     1036 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/bool.py
+-rw-rw-rw-   0        0        0     1814 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/bytes.py
+-rw-rw-rw-   0        0        0     1225 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/double.py
+-rw-rw-rw-   0        0        0     1403 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/int.py
+-rw-rw-rw-   0        0        0     1225 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/string.py
+-rw-rw-rw-   0        0        0     2081 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/vector.py
+-rw-rw-rw-   0        0        0     2577 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/raw/core/tl_object.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.697320 pyFipper-0.1.2.dev4/pyrogram/session/
+-rw-rw-rw-   0        0        0      891 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/session/__init__.py
+-rw-rw-rw-   0        0        0    10774 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/session/auth.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.709313 pyFipper-0.1.2.dev4/pyrogram/session/internals/
+-rw-rw-rw-   0        0        0      938 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/session/internals/__init__.py
+-rw-rw-rw-   0        0        0     2446 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/session/internals/data_center.py
+-rw-rw-rw-   0        0        0     1412 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/session/internals/msg_factory.py
+-rw-rw-rw-   0        0        0     1632 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/session/internals/msg_id.py
+-rw-rw-rw-   0        0        0     1291 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/session/internals/seq_no.py
+-rw-rw-rw-   0        0        0    12821 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/session/session.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.720306 pyFipper-0.1.2.dev4/pyrogram/storage/
+-rw-rw-rw-   0        0        0      949 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/storage/__init__.py
+-rw-rw-rw-   0        0        0     2231 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/storage/file_storage.py
+-rw-rw-rw-   0        0        0     2823 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/storage/memory_storage.py
+-rw-rw-rw-   0        0        0     6640 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/storage/sqlite_storage.py
+-rw-rw-rw-   0        0        0     2872 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/storage/storage.py
+-rw-rw-rw-   0        0        0     3852 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/sync.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.730300 pyFipper-0.1.2.dev4/pyrogram/types/
+-rw-rw-rw-   0        0        0     1137 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.736297 pyFipper-0.1.2.dev4/pyrogram/types/authorization/
+-rw-rw-rw-   0        0        0      960 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/authorization/__init__.py
+-rw-rw-rw-   0        0        0     2350 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/authorization/sent_code.py
+-rw-rw-rw-   0        0        0     1986 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/authorization/terms_of_service.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.797258 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/
+-rw-rw-rw-   0        0        0     2901 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-rw-rw-   0        0        0     1791 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-rw-rw-   0        0        0     2861 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-rw-rw-   0        0        0     1325 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-rw-rw-   0        0        0     1290 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-rw-rw-   0        0        0     1281 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-rw-rw-   0        0        0     1605 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-rw-rw-   0        0        0     1682 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-rw-rw-   0        0        0     1865 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-rw-rw-   0        0        0     1341 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-rw-rw-   0        0        0     1058 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-rw-rw-   0        0        0    13110 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-rw-rw-   0        0        0     2449 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-rw-rw-   0        0        0     2286 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-rw-rw-   0        0        0     8328 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0     2536 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-rw-rw-   0        0        0     3609 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-rw-rw-   0        0        0     3802 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-rw-rw-   0        0        0     1647 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-rw-rw-   0        0        0     1241 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-rw-rw-   0        0        0     1244 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-rw-rw-   0        0        0     1860 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-rw-rw-   0        0        0     4231 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-rw-rw-   0        0        0     2397 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-rw-rw-   0        0        0     1606 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-rw-rw-   0        0        0     1350 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.846228 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/
+-rw-rw-rw-   0        0        0     2802 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/__init__.py
+-rw-rw-rw-   0        0        0     3761 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-rw-rw-   0        0        0     7479 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query.py
+-rw-rw-rw-   0        0        0     2474 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result.py
+-rw-rw-rw-   0        0        0     5931 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-rw-rw-   0        0        0     3403 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-rw-rw-   0        0        0     4625 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-rw-rw-   0        0        0     4353 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-rw-rw-   0        0        0     4130 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-rw-rw-   0        0        0     4501 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-rw-rw-   0        0        0     4423 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-rw-rw-   0        0        0     3109 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-rw-rw-   0        0        0     4508 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-rw-rw-   0        0        0     4310 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-rw-rw-   0        0        0     4246 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-rw-rw-   0        0        0     5385 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-rw-rw-   0        0        0     4741 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-rw-rw-   0        0        0     5408 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-rw-rw-   0        0        0     4885 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-rw-rw-   0        0        0     5625 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-rw-rw-   0        0        0     4474 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.865217 pyFipper-0.1.2.dev4/pyrogram/types/input_media/
+-rw-rw-rw-   0        0        0     1344 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_media/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media.py
+-rw-rw-rw-   0        0        0     3309 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_animation.py
+-rw-rw-rw-   0        0        0     3364 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_audio.py
+-rw-rw-rw-   0        0        0     2836 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_document.py
+-rw-rw-rw-   0        0        0     2542 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_photo.py
+-rw-rw-rw-   0        0        0     3506 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_video.py
+-rw-rw-rw-   0        0        0     1788 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_phone_contact.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.873212 pyFipper-0.1.2.dev4/pyrogram/types/input_message_content/
+-rw-rw-rw-   0        0        0     1030 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_message_content/__init__.py
+-rw-rw-rw-   0        0        0     1453 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_message_content/input_message_content.py
+-rw-rw-rw-   0        0        0     2706 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-rw-rw-   0        0        0     1123 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/list.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.938171 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/
+-rw-rw-rw-   0        0        0     1883 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/__init__.py
+-rw-rw-rw-   0        0        0     4165 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/animation.py
+-rw-rw-rw-   0        0        0     4190 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/audio.py
+-rw-rw-rw-   0        0        0     2278 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/contact.py
+-rw-rw-rw-   0        0        0     1634 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/dice.py
+-rw-rw-rw-   0        0        0     3507 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/document.py
+-rw-rw-rw-   0        0        0     3143 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/game.py
+-rw-rw-rw-   0        0        0     1715 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/location.py
+-rw-rw-rw-   0        0        0   150763 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/message.py
+-rw-rw-rw-   0        0        0     4476 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/message_entity.py
+-rw-rw-rw-   0        0        0     1856 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/message_reactions.py
+-rw-rw-rw-   0        0        0     4439 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/photo.py
+-rw-rw-rw-   0        0        0     7240 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/poll.py
+-rw-rw-rw-   0        0        0     1582 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/poll_option.py
+-rw-rw-rw-   0        0        0     2703 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/reaction.py
+-rw-rw-rw-   0        0        0     7115 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/sticker.py
+-rw-rw-rw-   0        0        0     1478 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-rw-rw-   0        0        0     3866 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/thumbnail.py
+-rw-rw-rw-   0        0        0     2365 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/venue.py
+-rw-rw-rw-   0        0        0     4523 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/video.py
+-rw-rw-rw-   0        0        0     3709 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/video_note.py
+-rw-rw-rw-   0        0        0     3300 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/voice.py
+-rw-rw-rw-   0        0        0     1616 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/web_app_data.py
+-rw-rw-rw-   0        0        0     6538 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/web_page.py
+-rw-rw-rw-   0        0        0     3983 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/object.py
+-rw-rw-rw-   0        0        0     1029 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/update.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:50.994138 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/
+-rw-rw-rw-   0        0        0     2364 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/__init__.py
+-rw-rw-rw-   0        0        0    33812 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat.py
+-rw-rw-rw-   0        0        0     2299 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-rw-rw-   0        0        0    20324 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_event.py
+-rw-rw-rw-   0        0        0     5689 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-rw-rw-   0        0        0     4709 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-rw-rw-   0        0        0     4384 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-rw-rw-   0        0        0     2646 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-rw-rw-   0        0        0     9671 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_member.py
+-rw-rw-rw-   0        0        0     3776 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-rw-rw-   0        0        0     4480 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-rw-rw-   0        0        0     4074 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_photo.py
+-rw-rw-rw-   0        0        0     2671 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_preview.py
+-rw-rw-rw-   0        0        0     5063 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-rw-rw-   0        0        0     2425 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-rw-rw-   0        0        0     2761 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/dialog.py
+-rw-rw-rw-   0        0        0     2499 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/emoji_status.py
+-rw-rw-rw-   0        0        0     2012 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-rw-rw-   0        0        0     1713 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/restriction.py
+-rw-rw-rw-   0        0        0    13509 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/user.py
+-rw-rw-rw-   0        0        0     1387 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-rw-rw-   0        0        0     1660 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-rw-rw-   0        0        0     1574 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-rw-rw-   0        0        0     1072 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-rw-rw-   0        0        0    10943 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/pyrogram/utils.py
+-rw-rw-rw-   0        0        0       57 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:30:51.012127 pyFipper-0.1.2.dev4/setup.cfg
+-rw-rw-rw-   0        0        0     2124 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:51.000133 pyFipper-0.1.2.dev4/tests/
+-rw-rw-rw-   0        0        0      835 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:30:51.005130 pyFipper-0.1.2.dev4/tests/filters/
+-rw-rw-rw-   0        0        0     1237 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/tests/filters/__init__.py
+-rw-rw-rw-   0        0        0     3520 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/tests/filters/test_command.py
+-rw-rw-rw-   0        0        0     8402 2023-05-24 07:27:39.000000 pyFipper-0.1.2.dev4/tests/test_file_id.py
```

### Comparing `pyFipper-0.1.2.dev3/LICENSE` & `pyFipper-0.1.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/NOTICE` & `pyFipper-0.1.2.dev4/NOTICE`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/PKG-INFO` & `pyFipper-0.1.2.dev4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFipper
-Version: 0.1.2.dev3
+Version: 0.1.2.dev4
 Summary: Pyrogram - Telegram MTProto API Client Library for Python.
 Home-page: https://github.com/AyiinXd/pyrogram
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/pyrogram/issues
 Project-URL: Documentation, https://pyrogram.tech
```

### Comparing `pyFipper-0.1.2.dev3/README.md` & `pyFipper-0.1.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/__init__.py` & `pyFipper-0.1.2.dev4/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/api/__init__.py` & `pyFipper-0.1.2.dev4/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/api/compiler.py` & `pyFipper-0.1.2.dev4/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/api/source/auth_key.tl` & `pyFipper-0.1.2.dev4/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/api/source/main_api.tl` & `pyFipper-0.1.2.dev4/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/api/source/sys_msgs.tl` & `pyFipper-0.1.2.dev4/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/api/template/combinator.txt` & `pyFipper-0.1.2.dev4/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/api/template/type.txt` & `pyFipper-0.1.2.dev4/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/errors/__init__.py` & `pyFipper-0.1.2.dev4/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/errors/compiler.py` & `pyFipper-0.1.2.dev4/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/errors/sort.py` & `pyFipper-0.1.2.dev4/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/errors/source/400_BAD_REQUEST.tsv` & `pyFipper-0.1.2.dev4/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pyFipper-0.1.2.dev4/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/errors/source/403_FORBIDDEN.tsv` & `pyFipper-0.1.2.dev4/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pyFipper-0.1.2.dev4/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pyFipper-0.1.2.dev4/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyFipper.egg-info/PKG-INFO` & `pyFipper-0.1.2.dev4/pyFipper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFipper
-Version: 0.1.2.dev3
+Version: 0.1.2.dev4
 Summary: Pyrogram - Telegram MTProto API Client Library for Python.
 Home-page: https://github.com/AyiinXd/pyrogram
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/pyrogram/issues
 Project-URL: Documentation, https://pyrogram.tech
```

### Comparing `pyFipper-0.1.2.dev3/pyFipper.egg-info/SOURCES.txt` & `pyFipper-0.1.2.dev4/pyFipper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.1.2.dev03"
+__version__ = "0.1.2.dev04"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyFipper-0.1.2.dev3/pyrogram/client.py` & `pyFipper-0.1.2.dev4/pyrogram/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,14 +332,16 @@
             return
 
         listener['future'].set_exception(ListenerCanceled())
         self.clear_listener(chat_id, listener['future'])
 
 
     def should_stop(self):
+        if not self.end_client:
+            return
         current_time = datetime.now()
         stop_time = current_time + timedelta(minutes=self.end_client)
         return current_time >= stop_time
 
 
     def endclient(
         self: "pyrogram.Client",
```

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/connection.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/transport/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_full.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyFipper-0.1.2.dev4/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/crypto/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/crypto/aes.py` & `pyFipper-0.1.2.dev4/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/crypto/mtproto.py` & `pyFipper-0.1.2.dev4/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/crypto/prime.py` & `pyFipper-0.1.2.dev4/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/crypto/rsa.py` & `pyFipper-0.1.2.dev4/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/dispatcher.py` & `pyFipper-0.1.2.dev4/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/emoji.py` & `pyFipper-0.1.2.dev4/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/auto_name.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/chat_action.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/chat_event_action.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/chat_member_status.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/chat_members_filter.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/chat_type.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/message_entity_type.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/message_media_type.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/message_service_type.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/messages_filter.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/next_code_type.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/parse_mode.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/poll_type.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/sent_code_type.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/enums/user_status.py` & `pyFipper-0.1.2.dev4/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/errors/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/errors/rpc_error.py` & `pyFipper-0.1.2.dev4/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/file_id.py` & `pyFipper-0.1.2.dev4/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/filters.py` & `pyFipper-0.1.2.dev4/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/callback_query_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/chat_join_request_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/chat_member_updated_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/chosen_inline_result_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/conversation_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/conversation_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/deleted_messages_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/disconnect_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/edited_message_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/inline_query_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/message_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/poll_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/raw_update_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/handlers/user_status_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/advanced/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/advanced/invoke.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/advanced/resolve_peer.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/advanced/save_file.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/accept_terms_of_service.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/check_password.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/connect.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/disconnect.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/get_password_hint.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/initialize.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/initialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,11 @@
         if not self.is_connected:
             raise ConnectionError("Can't initialize a disconnected client")
 
         if self.is_initialized:
             raise ConnectionError("Client is already initialized")
 
         self.load_plugins()
-        if not self.end_client:
-            pass
-        self.endclient()
 
         await self.dispatcher.start()
 
         self.is_initialized = True
```

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/log_out.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/recover_password.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/resend_code.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/send_code.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/send_recovery_code.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/sign_in.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/sign_in_bot.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/sign_up.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/auth/terminate.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/answer_callback_query.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/answer_inline_query.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/answer_web_app_query.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/delete_bot_commands.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_bot_commands.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_chat_menu_button.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_game_high_scores.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/get_inline_bot_results.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/request_callback_answer.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/send_game.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/send_inline_bot_result.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/set_bot_commands.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/set_chat_menu_button.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/bots/set_game_score.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/add_chat_members.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/archive_chats.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/ban_chat_member.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/create_channel.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/create_group.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/create_supergroup.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/delete_channel.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/delete_chat_photo.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/delete_supergroup.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/delete_user_history.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_event_log.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_member.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_members.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_members_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_chat_online_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_dialogs.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_dialogs_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_nearby_chats.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/get_send_as_chats.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/join_chat.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/leave_chat.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/mark_chat_unread.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/pin_chat_message.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/promote_chat_member.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/restrict_chat_member.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_administrator_title.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_description.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_permissions.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_photo.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_protected_content.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_title.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_chat_username.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_send_as_chat.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/set_slow_mode.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/unarchive_chats.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/unban_chat_member.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/chats/unpin_chat_message.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/contacts/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/contacts/add_contact.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/contacts/delete_contacts.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/contacts/get_contacts.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/contacts/get_contacts_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/contacts/import_contacts.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_callback_query.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_chat_join_request.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_deleted_messages.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_disconnect.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_edited_message.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_inline_query.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_message.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_poll.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_raw_update.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/decorators/on_user_status.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/copy_media_group.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/copy_message.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/delete_messages.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/download_media.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_inline_caption.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_inline_media.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_inline_text.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_message_caption.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_message_media.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/edit_message_text.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/forward_messages.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_chat_history.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_chat_history_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_discussion_message.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_discussion_replies.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_media_group.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/get_messages.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/inline_session.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/read_chat_history.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/retract_vote.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/search_global.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/search_global_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/search_messages.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/search_messages_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_animation.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_audio.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_cached_media.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_chat_action.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_contact.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_dice.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_document.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_location.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_media_group.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_message.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_photo.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_poll.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_reaction.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_sticker.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_venue.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_video.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_video_note.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/send_voice.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/stop_poll.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/stream_media.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/vote_poll.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/wait_for_callback_query.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/wait_for_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/messages/wait_for_message.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/messages/wait_for_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/password/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/password/change_cloud_password.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/password/enable_cloud_password.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/password/remove_cloud_password.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/block_user.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/delete_profile_photos.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/get_chat_photos.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/get_chat_photos_count.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/get_common_chats.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/get_me.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/get_users.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/set_emoji_status.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/set_profile_photo.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/set_username.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/unblock_user.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/users/update_profile.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/add_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/compose.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/export_session_string.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/idle.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/remove_handler.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/restart.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/run.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/start.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/stop.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/methods/utilities/stop_transmission.py` & `pyFipper-0.1.2.dev4/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/mime_types.py` & `pyFipper-0.1.2.dev4/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/parser/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/parser/html.py` & `pyFipper-0.1.2.dev4/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/parser/markdown.py` & `pyFipper-0.1.2.dev4/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/parser/parser.py` & `pyFipper-0.1.2.dev4/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/parser/utils.py` & `pyFipper-0.1.2.dev4/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/future_salt.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/future_salts.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/gzip_packed.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/list.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/message.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/msg_container.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/bool.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/bytes.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/double.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/int.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/string.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/primitives/vector.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/raw/core/tl_object.py` & `pyFipper-0.1.2.dev4/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/session/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/session/auth.py` & `pyFipper-0.1.2.dev4/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/session/internals/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/session/internals/data_center.py` & `pyFipper-0.1.2.dev4/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/session/internals/msg_factory.py` & `pyFipper-0.1.2.dev4/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/session/internals/msg_id.py` & `pyFipper-0.1.2.dev4/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/session/internals/seq_no.py` & `pyFipper-0.1.2.dev4/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/session/session.py` & `pyFipper-0.1.2.dev4/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/storage/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/storage/file_storage.py` & `pyFipper-0.1.2.dev4/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/storage/memory_storage.py` & `pyFipper-0.1.2.dev4/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/storage/sqlite_storage.py` & `pyFipper-0.1.2.dev4/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/storage/storage.py` & `pyFipper-0.1.2.dev4/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/sync.py` & `pyFipper-0.1.2.dev4/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/authorization/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/authorization/sent_code.py` & `pyFipper-0.1.2.dev4/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/authorization/terms_of_service.py` & `pyFipper-0.1.2.dev4/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/login_url.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyFipper-0.1.2.dev4/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyFipper-0.1.2.dev4/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_media/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_animation.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_audio.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_document.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_photo.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_media_video.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_media/input_phone_contact.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_message_content/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_message_content/input_message_content.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/input_message_content/input_text_message_content.py` & `pyFipper-0.1.2.dev4/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/list.py` & `pyFipper-0.1.2.dev4/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/animation.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/audio.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/contact.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/dice.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/document.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/game.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/location.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/message.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/message_entity.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/message_reactions.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/photo.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/poll.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/poll_option.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/reaction.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/sticker.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/thumbnail.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/venue.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/video.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/video_note.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/voice.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/web_app_data.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/messages_and_media/web_page.py` & `pyFipper-0.1.2.dev4/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/object.py` & `pyFipper-0.1.2.dev4/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/update.py` & `pyFipper-0.1.2.dev4/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/__init__.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_event.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_join_request.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_joiner.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_member.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_permissions.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_photo.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_preview.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_privileges.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/chat_reactions.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/dialog.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/emoji_status.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/restriction.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/user.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/types/user_and_chats/video_chat_started.py` & `pyFipper-0.1.2.dev4/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/pyrogram/utils.py` & `pyFipper-0.1.2.dev4/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/setup.py` & `pyFipper-0.1.2.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/tests/__init__.py` & `pyFipper-0.1.2.dev4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/tests/filters/__init__.py` & `pyFipper-0.1.2.dev4/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/tests/filters/test_command.py` & `pyFipper-0.1.2.dev4/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `pyFipper-0.1.2.dev3/tests/test_file_id.py` & `pyFipper-0.1.2.dev4/tests/test_file_id.py`

 * *Files identical despite different names*

