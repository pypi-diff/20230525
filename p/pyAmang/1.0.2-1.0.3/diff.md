# Comparing `tmp/pyAmang-1.0.2.tar.gz` & `tmp/pyAmang-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAmang-1.0.2.tar", last modified: Wed May 24 22:24:50 2023, max compression
+gzip compressed data, was "pyAmang-1.0.3.tar", last modified: Wed May 24 22:43:52 2023, max compression
```

## Comparing `pyAmang-1.0.2.tar` & `pyAmang-1.0.3.tar`

### file list

```diff
@@ -1,493 +1,487 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.080059 pyAmang-1.0.2/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-05-24 21:41:11.000000 pyAmang-1.0.2/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-05-24 21:41:11.000000 pyAmang-1.0.2/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      305 2023-05-24 21:41:11.000000 pyAmang-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-24 21:41:11.000000 pyAmang-1.0.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4917 2023-05-24 22:24:50.080059 pyAmang-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2472 2023-05-24 21:41:11.000000 pyAmang-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/api/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22402 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/api/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/api/source/
--rw-r--r--   0 root         (0) root         (0)     2233 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/api/source/auth_key.tl
--rw-r--r--   0 root         (0) root         (0)   168867 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/api/source/main_api.tl
--rw-r--r--   0 root         (0) root         (0)     3425 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/api/template/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/api/template/combinator.txt
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/api/template/type.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/docs/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19230 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/docs/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/docs/template/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/docs/template/page.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/errors/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4917 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/compiler.py
--rw-r--r--   0 root         (0) root         (0)     1263 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/errors/source/
--rw-r--r--   0 root         (0) root         (0)      470 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 root         (0) root         (0)    22642 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 root         (0) root         (0)     2000 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 root         (0) root         (0)     1177 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 root         (0) root         (0)      470 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 root         (0) root         (0)     4219 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.012059 pyAmang-1.0.2/compiler/errors/template/
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/template/class.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-05-24 21:41:11.000000 pyAmang-1.0.2/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.016059 pyAmang-1.0.2/pyAmang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4917 2023-05-24 22:24:49.000000 pyAmang-1.0.2/pyAmang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18784 2023-05-24 22:24:49.000000 pyAmang-1.0.2/pyAmang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:24:49.000000 pyAmang-1.0.2/pyAmang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:24:49.000000 pyAmang-1.0.2/pyAmang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-24 22:24:49.000000 pyAmang-1.0.2/pyAmang.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 22:24:49.000000 pyAmang-1.0.2/pyAmang.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.016059 pyAmang-1.0.2/pyrogram/
--rw-r--r--   0 root         (0) root         (0)     1423 2023-05-24 22:03:12.000000 pyAmang-1.0.2/pyrogram/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41922 2023-05-24 21:47:20.000000 pyAmang-1.0.2/pyrogram/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.016059 pyAmang-1.0.2/pyrogram/connection/
--rw-r--r--   0 root         (0) root         (0)      854 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2542 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.016059 pyAmang-1.0.2/pyrogram/connection/transport/
--rw-r--r--   0 root         (0) root         (0)      838 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.016059 pyAmang-1.0.2/pyrogram/connection/transport/tcp/
--rw-r--r--   0 root         (0) root         (0)     1044 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4089 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.016059 pyAmang-1.0.2/pyrogram/crypto/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4013 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/crypto/aes.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/crypto/mtproto.py
--rw-r--r--   0 root         (0) root         (0)     2446 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/crypto/prime.py
--rw-r--r--   0 root         (0) root         (0)    13437 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/crypto/rsa.py
--rw-r--r--   0 root         (0) root         (0)    10054 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)   208021 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/emoji.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.020059 pyAmang-1.0.2/pyrogram/enums/
--rw-r--r--   0 root         (0) root         (0)     1736 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/auto_name.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4203 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/chat_type.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/message_media_type.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/message_service_type.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/messages_filter.py
--rw-r--r--   0 root         (0) root         (0)     1521 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/next_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/parse_mode.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/poll_type.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1299 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/enums/user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.020059 pyAmang-1.0.2/pyrogram/errors/
--rw-r--r--   0 root         (0) root         (0)     2605 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/errors/rpc_error.py
--rw-r--r--   0 root         (0) root         (0)    15154 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/file_id.py
--rw-r--r--   0 root         (0) root         (0)    24836 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.020059 pyAmang-1.0.2/pyrogram/handlers/
--rw-r--r--   0 root         (0) root         (0)     1475 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)     2101 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/handler.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.020059 pyAmang-1.0.2/pyrogram/methods/
--rw-r--r--   0 root         (0) root         (0)     1320 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.020059 pyAmang-1.0.2/pyrogram/methods/advanced/
--rw-r--r--   0 root         (0) root         (0)      988 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3133 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 root         (0) root         (0)     4560 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 root         (0) root         (0)     8421 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.028059 pyAmang-1.0.2/pyrogram/methods/auth/
--rw-r--r--   0 root         (0) root         (0)     1655 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/connect.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 root         (0) root         (0)     2723 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.032059 pyAmang-1.0.2/pyrogram/methods/bots/
--rw-r--r--   0 root         (0) root         (0)     2041 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3311 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     4990 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 root         (0) root         (0)     3365 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 root         (0) root         (0)     2847 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 root         (0) root         (0)     3956 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 root         (0) root         (0)     2826 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     3946 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.036059 pyAmang-1.0.2/pyrogram/methods/chats/
--rw-r--r--   0 root         (0) root         (0)     3439 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 root         (0) root         (0)     3282 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 root         (0) root         (0)     4032 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 root         (0) root         (0)     3338 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2264 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 root         (0) root         (0)     3360 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 root         (0) root         (0)     2401 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 root         (0) root         (0)     2136 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 root         (0) root         (0)     2694 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3136 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 root         (0) root         (0)     2247 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     4601 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 root         (0) root         (0)     2083 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.036059 pyAmang-1.0.2/pyrogram/methods/contacts/
--rw-r--r--   0 root         (0) root         (0)     1154 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 root         (0) root         (0)     1934 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.040059 pyAmang-1.0.2/pyrogram/methods/decorators/
--rw-r--r--   0 root         (0) root         (0)     1624 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 root         (0) root         (0)     2167 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.040059 pyAmang-1.0.2/pyrogram/methods/invite_links/
--rw-r--r--   0 root         (0) root         (0)     2435 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     3369 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2031 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2582 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3566 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 root         (0) root         (0)     2947 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     2329 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.052059 pyAmang-1.0.2/pyrogram/methods/messages/
--rw-r--r--   0 root         (0) root         (0)     3921 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5963 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 root         (0) root         (0)     3148 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 root         (0) root         (0)     7530 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 root         (0) root         (0)    10375 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3115 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 root         (0) root         (0)     2978 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 root         (0) root         (0)    13022 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 root         (0) root         (0)     2976 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     4564 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 root         (0) root         (0)     4041 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 root         (0) root         (0)     2175 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 root         (0) root         (0)     5349 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 root         (0) root         (0)     3203 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 root         (0) root         (0)    12584 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 root         (0) root         (0)    11118 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 root         (0) root         (0)     2817 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4867 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 root         (0) root         (0)     4841 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 root         (0) root         (0)    10468 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 root         (0) root         (0)     4576 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 root         (0) root         (0)    19906 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 root         (0) root         (0)     7265 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 root         (0) root         (0)     9438 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 root         (0) root         (0)     8071 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 root         (0) root         (0)     8338 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 root         (0) root         (0)     5397 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 root         (0) root         (0)    11954 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 root         (0) root         (0)     9312 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 root         (0) root         (0)     9428 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 root         (0) root         (0)     2819 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 root         (0) root         (0)     3937 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 root         (0) root         (0)     2504 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.052059 pyAmang-1.0.2/pyrogram/methods/password/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     3006 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.052059 pyAmang-1.0.2/pyrogram/methods/users/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/block_user.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 root         (0) root         (0)     4421 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/get_me.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/get_users.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     2718 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/set_username.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.056059 pyAmang-1.0.2/pyrogram/methods/utilities/
--rw-r--r--   0 root         (0) root         (0)     1253 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2346 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 root         (0) root         (0)     2232 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 root         (0) root         (0)     2210 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 root         (0) root         (0)     2294 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/run.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/start.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 root         (0) root         (0)    61915 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/mime_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.056059 pyAmang-1.0.2/pyrogram/parser/
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8684 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/parser/html.py
--rw-r--r--   0 root         (0) root         (0)     5770 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/parser/markdown.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/parser/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.056059 pyAmang-1.0.2/pyrogram/raw/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.056059 pyAmang-1.0.2/pyrogram/raw/core/
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/list.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/message.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.060059 pyAmang-1.0.2/pyrogram/raw/core/primitives/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-05-19 02:13:28.000000 pyAmang-1.0.2/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.060059 pyAmang-1.0.2/pyrogram/session/
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/session/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11446 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/session/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.060059 pyAmang-1.0.2/pyrogram/session/internals/
--rw-r--r--   0 root         (0) root         (0)      917 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/session/internals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/session/internals/data_center.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 root         (0) root         (0)     1162 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 root         (0) root         (0)    13419 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/session/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.060059 pyAmang-1.0.2/pyrogram/storage/
--rw-r--r--   0 root         (0) root         (0)      928 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/storage/file_storage.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/storage/memory_storage.py
--rw-r--r--   0 root         (0) root         (0)     6224 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/storage/storage.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.060059 pyAmang-1.0.2/pyrogram/types/
--rw-r--r--   0 root         (0) root         (0)     1109 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.060059 pyAmang-1.0.2/pyrogram/types/authorization/
--rw-r--r--   0 root         (0) root         (0)      938 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.064059 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 root         (0) root         (0)     2830 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1738 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 root         (0) root         (0)     1293 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 root         (0) root         (0)    12797 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 root         (0) root         (0)     8120 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     3514 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 root         (0) root         (0)     4575 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.068059 pyAmang-1.0.2/pyrogram/types/inline_mode/
--rw-r--r--   0 root         (0) root         (0)     2755 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2411 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 root         (0) root         (0)     5776 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 root         (0) root         (0)     3304 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 root         (0) root         (0)     4505 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 root         (0) root         (0)     4388 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 root         (0) root         (0)     4394 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 root         (0) root         (0)     4132 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 root         (0) root         (0)     5240 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 root         (0) root         (0)     5261 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 root         (0) root         (0)     4754 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 root         (0) root         (0)     5474 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 root         (0) root         (0)     4360 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.068059 pyAmang-1.0.2/pyrogram/types/input_media/
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 root         (0) root         (0)     3282 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 root         (0) root         (0)     2771 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 root         (0) root         (0)     2685 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.072059 pyAmang-1.0.2/pyrogram/types/input_message_content/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 root         (0) root         (0)     2638 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.072059 pyAmang-1.0.2/pyrogram/types/messages_and_media/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 root         (0) root         (0)     4069 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 root         (0) root         (0)     3409 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 root         (0) root         (0)     3044 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 root         (0) root         (0)   144519 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 root         (0) root         (0)     4352 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 root         (0) root         (0)     1800 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 root         (0) root         (0)     4309 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 root         (0) root         (0)     7037 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 root         (0) root         (0)     6909 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 root         (0) root         (0)     4389 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 root         (0) root         (0)     3601 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 root         (0) root         (0)     3204 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 root         (0) root         (0)     6351 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 root         (0) root         (0)     3862 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/object.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.080059 pyAmang-1.0.2/pyrogram/types/user_and_chats/
--rw-r--r--   0 root         (0) root         (0)     2297 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32559 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)    19835 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 root         (0) root         (0)     5514 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3674 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     4382 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 root         (0) root         (0)     2422 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     1951 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 root         (0) root         (0)    12836 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 root         (0) root         (0)     1531 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 root         (0) root         (0)    10572 2023-05-24 21:41:11.000000 pyAmang-1.0.2/pyrogram/utils.py
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-24 21:41:11.000000 pyAmang-1.0.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 22:24:50.080059 pyAmang-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3513 2023-05-24 21:41:11.000000 pyAmang-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.080059 pyAmang-1.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 21:41:11.000000 pyAmang-1.0.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.080059 pyAmang-1.0.2/tests/filters/
--rw-r--r--   0 root         (0) root         (0)     1201 2023-05-24 21:41:11.000000 pyAmang-1.0.2/tests/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-05-24 21:41:11.000000 pyAmang-1.0.2/tests/filters/test_command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:24:50.080059 pyAmang-1.0.2/tests/parser/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 21:41:11.000000 pyAmang-1.0.2/tests/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6264 2023-05-24 21:41:11.000000 pyAmang-1.0.2/tests/parser/test_html.py
--rw-r--r--   0 root         (0) root         (0)     8208 2023-05-24 21:41:11.000000 pyAmang-1.0.2/tests/test_file_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.400642 pyAmang-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-05-24 22:43:36.000000 pyAmang-1.0.3/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-05-24 22:43:36.000000 pyAmang-1.0.3/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      305 2023-05-24 22:43:36.000000 pyAmang-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      774 2023-05-24 22:43:36.000000 pyAmang-1.0.3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-05-24 22:43:52.400642 pyAmang-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-05-24 22:43:36.000000 pyAmang-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.356641 pyAmang-1.0.3/compiler/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.356641 pyAmang-1.0.3/compiler/api/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22402 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/api/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.356641 pyAmang-1.0.3/compiler/api/source/
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/api/source/auth_key.tl
+-rw-r--r--   0 root         (0) root         (0)   168867 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/api/source/main_api.tl
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.360641 pyAmang-1.0.3/compiler/api/template/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/api/template/combinator.txt
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/api/template/type.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.360641 pyAmang-1.0.3/compiler/errors/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.360641 pyAmang-1.0.3/compiler/errors/source/
+-rw-r--r--   0 root         (0) root         (0)      470 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 root         (0) root         (0)    22642 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 root         (0) root         (0)      470 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.360641 pyAmang-1.0.3/compiler/errors/template/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/template/class.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-05-24 22:43:36.000000 pyAmang-1.0.3/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.360641 pyAmang-1.0.3/pyAmang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-05-24 22:43:52.000000 pyAmang-1.0.3/pyAmang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18665 2023-05-24 22:43:52.000000 pyAmang-1.0.3/pyAmang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:43:52.000000 pyAmang-1.0.3/pyAmang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:43:52.000000 pyAmang-1.0.3/pyAmang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-24 22:43:52.000000 pyAmang-1.0.3/pyAmang.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 22:43:52.000000 pyAmang-1.0.3/pyAmang.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.364641 pyAmang-1.0.3/pyrogram/
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41976 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.364641 pyAmang-1.0.3/pyrogram/connection/
+-rw-r--r--   0 root         (0) root         (0)      854 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.364641 pyAmang-1.0.3/pyrogram/connection/transport/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.364641 pyAmang-1.0.3/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4089 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.364641 pyAmang-1.0.3/pyrogram/crypto/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/crypto/aes.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/crypto/prime.py
+-rw-r--r--   0 root         (0) root         (0)    13437 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/crypto/rsa.py
+-rw-r--r--   0 root         (0) root         (0)    10054 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)   208021 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/emoji.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.364641 pyAmang-1.0.3/pyrogram/enums/
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/auto_name.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4203 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/chat_type.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/poll_type.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/enums/user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.364641 pyAmang-1.0.3/pyrogram/errors/
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 root         (0) root         (0)    15154 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/file_id.py
+-rw-r--r--   0 root         (0) root         (0)    24836 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.368641 pyAmang-1.0.3/pyrogram/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/handler.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.368641 pyAmang-1.0.3/pyrogram/methods/
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.368641 pyAmang-1.0.3/pyrogram/methods/advanced/
+-rw-r--r--   0 root         (0) root         (0)      988 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 root         (0) root         (0)     8421 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.368641 pyAmang-1.0.3/pyrogram/methods/auth/
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.368641 pyAmang-1.0.3/pyrogram/methods/bots/
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     4990 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.372641 pyAmang-1.0.3/pyrogram/methods/chats/
+-rw-r--r--   0 root         (0) root         (0)     3439 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 root         (0) root         (0)     4032 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 root         (0) root         (0)     3338 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2136 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2694 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     4601 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.372641 pyAmang-1.0.3/pyrogram/methods/contacts/
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.376641 pyAmang-1.0.3/pyrogram/methods/decorators/
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.376641 pyAmang-1.0.3/pyrogram/methods/invite_links/
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3566 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.380641 pyAmang-1.0.3/pyrogram/methods/messages/
+-rw-r--r--   0 root         (0) root         (0)     3921 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5963 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     7530 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 root         (0) root         (0)    10375 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 root         (0) root         (0)    13022 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 root         (0) root         (0)     2976 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     4564 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 root         (0) root         (0)     4041 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 root         (0) root         (0)     5349 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 root         (0) root         (0)    12584 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 root         (0) root         (0)    11118 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4867 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 root         (0) root         (0)    10468 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 root         (0) root         (0)    19906 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     7265 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 root         (0) root         (0)     9438 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 root         (0) root         (0)     8071 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     8338 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     5397 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 root         (0) root         (0)    11954 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 root         (0) root         (0)     9312 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 root         (0) root         (0)     9428 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 root         (0) root         (0)     3937 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.380641 pyAmang-1.0.3/pyrogram/methods/password/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.380641 pyAmang-1.0.3/pyrogram/methods/users/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 root         (0) root         (0)     4421 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.384641 pyAmang-1.0.3/pyrogram/methods/utilities/
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/run.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 root         (0) root         (0)    61915 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/mime_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.384641 pyAmang-1.0.3/pyrogram/parser/
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8684 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/parser/html.py
+-rw-r--r--   0 root         (0) root         (0)     5770 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/parser/markdown.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.384641 pyAmang-1.0.3/pyrogram/raw/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.384641 pyAmang-1.0.3/pyrogram/raw/core/
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/list.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.384641 pyAmang-1.0.3/pyrogram/raw/core/primitives/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.384641 pyAmang-1.0.3/pyrogram/session/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/session/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11446 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/session/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.388641 pyAmang-1.0.3/pyrogram/session/internals/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 root         (0) root         (0)    13419 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/session/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.388641 pyAmang-1.0.3/pyrogram/storage/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/storage/file_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/storage/storage.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.388641 pyAmang-1.0.3/pyrogram/types/
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.388641 pyAmang-1.0.3/pyrogram/types/authorization/
+-rw-r--r--   0 root         (0) root         (0)      938 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.388641 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 root         (0) root         (0)     8120 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.392641 pyAmang-1.0.3/pyrogram/types/inline_mode/
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2411 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 root         (0) root         (0)     5776 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     4505 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4388 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 root         (0) root         (0)     4132 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 root         (0) root         (0)     5240 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 root         (0) root         (0)     5261 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     4754 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 root         (0) root         (0)     5474 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 root         (0) root         (0)     4360 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.392641 pyAmang-1.0.3/pyrogram/types/input_media/
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.392641 pyAmang-1.0.3/pyrogram/types/input_message_content/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.396642 pyAmang-1.0.3/pyrogram/types/messages_and_media/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 root         (0) root         (0)     4069 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 root         (0) root         (0)     3044 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 root         (0) root         (0)   144519 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     4309 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 root         (0) root         (0)     7037 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 root         (0) root         (0)     6909 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 root         (0) root         (0)     3601 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 root         (0) root         (0)     6351 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3862 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/object.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.396642 pyAmang-1.0.3/pyrogram/types/user_and_chats/
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32559 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)    19835 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3674 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 root         (0) root         (0)    12836 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 root         (0) root         (0)    10572 2023-05-24 22:43:36.000000 pyAmang-1.0.3/pyrogram/utils.py
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-24 22:43:36.000000 pyAmang-1.0.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 22:43:52.400642 pyAmang-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-05-24 22:43:36.000000 pyAmang-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.400642 pyAmang-1.0.3/tests/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 22:43:36.000000 pyAmang-1.0.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.400642 pyAmang-1.0.3/tests/filters/
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-05-24 22:43:36.000000 pyAmang-1.0.3/tests/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-05-24 22:43:36.000000 pyAmang-1.0.3/tests/filters/test_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:43:52.400642 pyAmang-1.0.3/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)      818 2023-05-24 22:43:36.000000 pyAmang-1.0.3/tests/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6264 2023-05-24 22:43:36.000000 pyAmang-1.0.3/tests/parser/test_html.py
+-rw-r--r--   0 root         (0) root         (0)     8208 2023-05-24 22:43:36.000000 pyAmang-1.0.3/tests/test_file_id.py
```

### Comparing `pyAmang-1.0.2/COPYING` & `pyAmang-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/COPYING.lesser` & `pyAmang-1.0.3/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/NOTICE` & `pyAmang-1.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/PKG-INFO` & `pyAmang-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAmang
-Version: 1.0.2
+Version: 1.0.3
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/amanqs
 Author: amanqs
 Author-email: amanqs@github.com
 License: LGPLv3
 Download-URL: https://github.com/amanqs/pyAmang/releases/latest
 Project-URL: Tracker, https://github.com/amanqs/pyAmang/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyAmang Version: 1.0.2 Summary: Elegant, modern and
+Metadata-Version: 2.1 Name: pyAmang Version: 1.0.3 Summary: Elegant, modern and
 asynchronous Telegram MTProto API framework in Python for users and bots Home-
 page: https://github.com/amanqs Author: amanqs Author-email: amanqs@github.com
 License: LGPLv3 Download-URL: https://github.com/amanqs/pyAmang/releases/latest
 Project-URL: Tracker, https://github.com/amanqs/pyAmang/issues Project-URL:
 Community, https://t.me/amwangsupport Project-URL: Source, https://github.com/
 amanqs/pyAmang Project-URL: Documentation, https://docs.amanqs/pyAmang.org
 Description:
```

### Comparing `pyAmang-1.0.2/README.md` & `pyAmang-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/__init__.py` & `pyAmang-1.0.3/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/api/__init__.py` & `pyAmang-1.0.3/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/api/compiler.py` & `pyAmang-1.0.3/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/api/source/auth_key.tl` & `pyAmang-1.0.3/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/api/source/main_api.tl` & `pyAmang-1.0.3/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/api/source/sys_msgs.tl` & `pyAmang-1.0.3/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/api/template/combinator.txt` & `pyAmang-1.0.3/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/api/template/type.txt` & `pyAmang-1.0.3/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/docs/__init__.py` & `pyAmang-1.0.3/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/errors/__init__.py` & `pyAmang-1.0.3/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/errors/compiler.py` & `pyAmang-1.0.3/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/errors/sort.py` & `pyAmang-1.0.3/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/errors/source/400_BAD_REQUEST.tsv` & `pyAmang-1.0.3/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pyAmang-1.0.3/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/errors/source/403_FORBIDDEN.tsv` & `pyAmang-1.0.3/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pyAmang-1.0.3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pyAmang-1.0.3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyAmang.egg-info/PKG-INFO` & `pyAmang-1.0.3/pyAmang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAmang
-Version: 1.0.2
+Version: 1.0.3
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/amanqs
 Author: amanqs
 Author-email: amanqs@github.com
 License: LGPLv3
 Download-URL: https://github.com/amanqs/pyAmang/releases/latest
 Project-URL: Tracker, https://github.com/amanqs/pyAmang/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyAmang Version: 1.0.2 Summary: Elegant, modern and
+Metadata-Version: 2.1 Name: pyAmang Version: 1.0.3 Summary: Elegant, modern and
 asynchronous Telegram MTProto API framework in Python for users and bots Home-
 page: https://github.com/amanqs Author: amanqs Author-email: amanqs@github.com
 License: LGPLv3 Download-URL: https://github.com/amanqs/pyAmang/releases/latest
 Project-URL: Tracker, https://github.com/amanqs/pyAmang/issues Project-URL:
 Community, https://t.me/amwangsupport Project-URL: Source, https://github.com/
 amanqs/pyAmang Project-URL: Documentation, https://docs.amanqs/pyAmang.org
 Description:
```

### Comparing `pyAmang-1.0.2/pyAmang.egg-info/SOURCES.txt` & `pyAmang-1.0.3/pyAmang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 compiler/api/__init__.py
 compiler/api/compiler.py
 compiler/api/source/auth_key.tl
 compiler/api/source/main_api.tl
 compiler/api/source/sys_msgs.tl
 compiler/api/template/combinator.txt
 compiler/api/template/type.txt
-compiler/docs/__init__.py
-compiler/docs/compiler.py
-compiler/docs/template/page.txt
-compiler/docs/template/toctree.txt
 compiler/errors/__init__.py
 compiler/errors/compiler.py
 compiler/errors/sort.py
 compiler/errors/source/303_SEE_OTHER.tsv
 compiler/errors/source/400_BAD_REQUEST.tsv
 compiler/errors/source/401_UNAUTHORIZED.tsv
 compiler/errors/source/403_FORBIDDEN.tsv
```

### Comparing `pyAmang-1.0.2/pyrogram/__init__.py` & `pyAmang-1.0.3/pyrogram/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
-__copyright__ = "Copyright (C) 2023-present Amang <https://t.me/amwang> - Kynan <https://t.me/rizzvbss>"
+__copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
     pass
```

### Comparing `pyAmang-1.0.2/pyrogram/client.py` & `pyAmang-1.0.3/pyrogram/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,16 +175,16 @@
 
         max_concurrent_transmissions (``bool``, *optional*):
             Set the maximum amount of concurrent transmissions (uploads & downloads).
             A value that is too high may result in network related issues.
             Defaults to 1.
     """
 
-    APP_VERSION = f"KymangSession V1"
-    DEVICE_MODEL = f"KyMang Synergy"
+    APP_VERSION = f"Pyrogram {__version__}"
+    DEVICE_MODEL = f"{platform.python_implementation()} {platform.python_version()}"
     SYSTEM_VERSION = f"{platform.system()} {platform.release()}"
 
     LANG_CODE = "en"
 
     PARENT_DIR = Path(sys.argv[0]).parent
 
     INVITE_LINK_RE = re.compile(r"^(?:https?://)?(?:www\.)?(?:t(?:elegram)?\.(?:org|me|dog)/(?:joinchat/|\+))([\w-]+)$")
```

### Comparing `pyAmang-1.0.2/pyrogram/connection/__init__.py` & `pyAmang-1.0.3/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/connection.py` & `pyAmang-1.0.3/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/transport/__init__.py` & `pyAmang-1.0.3/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/transport/tcp/__init__.py` & `pyAmang-1.0.3/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp.py` & `pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_full.py` & `pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyAmang-1.0.3/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/crypto/__init__.py` & `pyAmang-1.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/crypto/aes.py` & `pyAmang-1.0.3/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/crypto/mtproto.py` & `pyAmang-1.0.3/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/crypto/prime.py` & `pyAmang-1.0.3/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/crypto/rsa.py` & `pyAmang-1.0.3/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/dispatcher.py` & `pyAmang-1.0.3/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/emoji.py` & `pyAmang-1.0.3/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/__init__.py` & `pyAmang-1.0.3/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/auto_name.py` & `pyAmang-1.0.3/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/chat_action.py` & `pyAmang-1.0.3/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/chat_event_action.py` & `pyAmang-1.0.3/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/chat_member_status.py` & `pyAmang-1.0.3/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/chat_members_filter.py` & `pyAmang-1.0.3/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/chat_type.py` & `pyAmang-1.0.3/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/message_entity_type.py` & `pyAmang-1.0.3/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/message_media_type.py` & `pyAmang-1.0.3/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/message_service_type.py` & `pyAmang-1.0.3/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/messages_filter.py` & `pyAmang-1.0.3/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/next_code_type.py` & `pyAmang-1.0.3/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/parse_mode.py` & `pyAmang-1.0.3/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/poll_type.py` & `pyAmang-1.0.3/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/sent_code_type.py` & `pyAmang-1.0.3/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/enums/user_status.py` & `pyAmang-1.0.3/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/errors/__init__.py` & `pyAmang-1.0.3/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/errors/rpc_error.py` & `pyAmang-1.0.3/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/file_id.py` & `pyAmang-1.0.3/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/filters.py` & `pyAmang-1.0.3/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/__init__.py` & `pyAmang-1.0.3/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/callback_query_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/chat_join_request_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/chat_member_updated_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/chosen_inline_result_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/deleted_messages_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/disconnect_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/edited_message_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/handler.py` & `pyAmang-1.0.3/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/inline_query_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/message_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/poll_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/raw_update_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/handlers/user_status_handler.py` & `pyAmang-1.0.3/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/advanced/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/advanced/invoke.py` & `pyAmang-1.0.3/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/advanced/resolve_peer.py` & `pyAmang-1.0.3/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/advanced/save_file.py` & `pyAmang-1.0.3/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/accept_terms_of_service.py` & `pyAmang-1.0.3/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/check_password.py` & `pyAmang-1.0.3/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/connect.py` & `pyAmang-1.0.3/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/disconnect.py` & `pyAmang-1.0.3/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/get_password_hint.py` & `pyAmang-1.0.3/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/initialize.py` & `pyAmang-1.0.3/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/log_out.py` & `pyAmang-1.0.3/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/recover_password.py` & `pyAmang-1.0.3/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/resend_code.py` & `pyAmang-1.0.3/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/send_code.py` & `pyAmang-1.0.3/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/send_recovery_code.py` & `pyAmang-1.0.3/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/sign_in.py` & `pyAmang-1.0.3/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/sign_in_bot.py` & `pyAmang-1.0.3/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/sign_up.py` & `pyAmang-1.0.3/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/auth/terminate.py` & `pyAmang-1.0.3/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/answer_callback_query.py` & `pyAmang-1.0.3/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/answer_inline_query.py` & `pyAmang-1.0.3/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/answer_web_app_query.py` & `pyAmang-1.0.3/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/delete_bot_commands.py` & `pyAmang-1.0.3/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/get_bot_commands.py` & `pyAmang-1.0.3/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyAmang-1.0.3/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/get_chat_menu_button.py` & `pyAmang-1.0.3/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/get_game_high_scores.py` & `pyAmang-1.0.3/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/get_inline_bot_results.py` & `pyAmang-1.0.3/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/request_callback_answer.py` & `pyAmang-1.0.3/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/send_game.py` & `pyAmang-1.0.3/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/send_inline_bot_result.py` & `pyAmang-1.0.3/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/set_bot_commands.py` & `pyAmang-1.0.3/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyAmang-1.0.3/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/set_chat_menu_button.py` & `pyAmang-1.0.3/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/bots/set_game_score.py` & `pyAmang-1.0.3/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/add_chat_members.py` & `pyAmang-1.0.3/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/archive_chats.py` & `pyAmang-1.0.3/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/ban_chat_member.py` & `pyAmang-1.0.3/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/create_channel.py` & `pyAmang-1.0.3/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/create_group.py` & `pyAmang-1.0.3/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/create_supergroup.py` & `pyAmang-1.0.3/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/delete_channel.py` & `pyAmang-1.0.3/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/delete_chat_photo.py` & `pyAmang-1.0.3/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/delete_supergroup.py` & `pyAmang-1.0.3/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/delete_user_history.py` & `pyAmang-1.0.3/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_chat.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_chat_event_log.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_chat_member.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_chat_members.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_chat_members_count.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_chat_online_count.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_dialogs.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_dialogs_count.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_nearby_chats.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/get_send_as_chats.py` & `pyAmang-1.0.3/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/join_chat.py` & `pyAmang-1.0.3/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/leave_chat.py` & `pyAmang-1.0.3/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/mark_chat_unread.py` & `pyAmang-1.0.3/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/pin_chat_message.py` & `pyAmang-1.0.3/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/promote_chat_member.py` & `pyAmang-1.0.3/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/restrict_chat_member.py` & `pyAmang-1.0.3/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_administrator_title.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_chat_description.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_chat_permissions.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_chat_photo.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_chat_protected_content.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_chat_title.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_chat_username.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_send_as_chat.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/set_slow_mode.py` & `pyAmang-1.0.3/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/unarchive_chats.py` & `pyAmang-1.0.3/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/unban_chat_member.py` & `pyAmang-1.0.3/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyAmang-1.0.3/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/chats/unpin_chat_message.py` & `pyAmang-1.0.3/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/contacts/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/contacts/add_contact.py` & `pyAmang-1.0.3/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/contacts/delete_contacts.py` & `pyAmang-1.0.3/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/contacts/get_contacts.py` & `pyAmang-1.0.3/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/contacts/get_contacts_count.py` & `pyAmang-1.0.3/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/contacts/import_contacts.py` & `pyAmang-1.0.3/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_callback_query.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_chat_join_request.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_deleted_messages.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_disconnect.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_edited_message.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_inline_query.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_message.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_poll.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_raw_update.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/decorators/on_user_status.py` & `pyAmang-1.0.3/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyAmang-1.0.3/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/copy_media_group.py` & `pyAmang-1.0.3/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/copy_message.py` & `pyAmang-1.0.3/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/delete_messages.py` & `pyAmang-1.0.3/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/download_media.py` & `pyAmang-1.0.3/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/edit_inline_caption.py` & `pyAmang-1.0.3/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/edit_inline_media.py` & `pyAmang-1.0.3/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyAmang-1.0.3/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/edit_inline_text.py` & `pyAmang-1.0.3/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/edit_message_caption.py` & `pyAmang-1.0.3/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/edit_message_media.py` & `pyAmang-1.0.3/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyAmang-1.0.3/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/edit_message_text.py` & `pyAmang-1.0.3/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/forward_messages.py` & `pyAmang-1.0.3/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/get_chat_history.py` & `pyAmang-1.0.3/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/get_chat_history_count.py` & `pyAmang-1.0.3/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyAmang-1.0.3/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/get_discussion_message.py` & `pyAmang-1.0.3/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/get_discussion_replies.py` & `pyAmang-1.0.3/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyAmang-1.0.3/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/get_media_group.py` & `pyAmang-1.0.3/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/get_messages.py` & `pyAmang-1.0.3/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/inline_session.py` & `pyAmang-1.0.3/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/read_chat_history.py` & `pyAmang-1.0.3/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/retract_vote.py` & `pyAmang-1.0.3/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/search_global.py` & `pyAmang-1.0.3/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/search_global_count.py` & `pyAmang-1.0.3/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/search_messages.py` & `pyAmang-1.0.3/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/search_messages_count.py` & `pyAmang-1.0.3/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_animation.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_audio.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_cached_media.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_chat_action.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_contact.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_dice.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_document.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_location.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_media_group.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_message.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_photo.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_poll.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_reaction.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_sticker.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_venue.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_video.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_video_note.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/send_voice.py` & `pyAmang-1.0.3/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/stop_poll.py` & `pyAmang-1.0.3/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/stream_media.py` & `pyAmang-1.0.3/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/messages/vote_poll.py` & `pyAmang-1.0.3/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/password/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/password/change_cloud_password.py` & `pyAmang-1.0.3/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/password/enable_cloud_password.py` & `pyAmang-1.0.3/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/password/remove_cloud_password.py` & `pyAmang-1.0.3/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/block_user.py` & `pyAmang-1.0.3/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/delete_profile_photos.py` & `pyAmang-1.0.3/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/get_chat_photos.py` & `pyAmang-1.0.3/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/get_chat_photos_count.py` & `pyAmang-1.0.3/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/get_common_chats.py` & `pyAmang-1.0.3/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyAmang-1.0.3/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/get_me.py` & `pyAmang-1.0.3/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/get_users.py` & `pyAmang-1.0.3/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/set_emoji_status.py` & `pyAmang-1.0.3/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/set_profile_photo.py` & `pyAmang-1.0.3/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/set_username.py` & `pyAmang-1.0.3/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/unblock_user.py` & `pyAmang-1.0.3/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/users/update_profile.py` & `pyAmang-1.0.3/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/__init__.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/add_handler.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/compose.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/export_session_string.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/idle.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/remove_handler.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/restart.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/run.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/start.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/stop.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/methods/utilities/stop_transmission.py` & `pyAmang-1.0.3/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/mime_types.py` & `pyAmang-1.0.3/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/parser/__init__.py` & `pyAmang-1.0.3/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/parser/html.py` & `pyAmang-1.0.3/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/parser/markdown.py` & `pyAmang-1.0.3/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/parser/parser.py` & `pyAmang-1.0.3/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/parser/utils.py` & `pyAmang-1.0.3/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/__init__.py` & `pyAmang-1.0.3/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/__init__.py` & `pyAmang-1.0.3/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/future_salt.py` & `pyAmang-1.0.3/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/future_salts.py` & `pyAmang-1.0.3/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/gzip_packed.py` & `pyAmang-1.0.3/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/list.py` & `pyAmang-1.0.3/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/message.py` & `pyAmang-1.0.3/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/msg_container.py` & `pyAmang-1.0.3/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/primitives/__init__.py` & `pyAmang-1.0.3/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/primitives/bool.py` & `pyAmang-1.0.3/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/primitives/bytes.py` & `pyAmang-1.0.3/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/primitives/double.py` & `pyAmang-1.0.3/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/primitives/int.py` & `pyAmang-1.0.3/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/primitives/string.py` & `pyAmang-1.0.3/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/primitives/vector.py` & `pyAmang-1.0.3/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/raw/core/tl_object.py` & `pyAmang-1.0.3/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/session/__init__.py` & `pyAmang-1.0.3/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/session/auth.py` & `pyAmang-1.0.3/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/session/internals/__init__.py` & `pyAmang-1.0.3/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/session/internals/data_center.py` & `pyAmang-1.0.3/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/session/internals/msg_factory.py` & `pyAmang-1.0.3/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/session/internals/msg_id.py` & `pyAmang-1.0.3/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/session/internals/seq_no.py` & `pyAmang-1.0.3/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/session/session.py` & `pyAmang-1.0.3/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/storage/__init__.py` & `pyAmang-1.0.3/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/storage/file_storage.py` & `pyAmang-1.0.3/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/storage/memory_storage.py` & `pyAmang-1.0.3/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/storage/sqlite_storage.py` & `pyAmang-1.0.3/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/storage/storage.py` & `pyAmang-1.0.3/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/sync.py` & `pyAmang-1.0.3/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/__init__.py` & `pyAmang-1.0.3/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/authorization/__init__.py` & `pyAmang-1.0.3/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/authorization/sent_code.py` & `pyAmang-1.0.3/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/authorization/terms_of_service.py` & `pyAmang-1.0.3/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/__init__.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/login_url.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyAmang-1.0.3/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/__init__.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyAmang-1.0.3/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_media/__init__.py` & `pyAmang-1.0.3/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_media/input_media.py` & `pyAmang-1.0.3/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_media/input_media_animation.py` & `pyAmang-1.0.3/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_media/input_media_audio.py` & `pyAmang-1.0.3/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_media/input_media_document.py` & `pyAmang-1.0.3/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_media/input_media_photo.py` & `pyAmang-1.0.3/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_media/input_media_video.py` & `pyAmang-1.0.3/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_media/input_phone_contact.py` & `pyAmang-1.0.3/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_message_content/__init__.py` & `pyAmang-1.0.3/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_message_content/input_message_content.py` & `pyAmang-1.0.3/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/input_message_content/input_text_message_content.py` & `pyAmang-1.0.3/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/list.py` & `pyAmang-1.0.3/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/__init__.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/animation.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/audio.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/contact.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/dice.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/document.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/game.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/location.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/message.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/message_entity.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/message_reactions.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/photo.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/poll.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/poll_option.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/reaction.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/sticker.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/thumbnail.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/venue.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/video.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/video_note.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/voice.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/web_app_data.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/messages_and_media/web_page.py` & `pyAmang-1.0.3/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/object.py` & `pyAmang-1.0.3/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/update.py` & `pyAmang-1.0.3/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/__init__.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_event.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_join_request.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_joiner.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_member.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_permissions.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_photo.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_preview.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_privileges.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/chat_reactions.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/dialog.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/emoji_status.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/restriction.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/user.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/types/user_and_chats/video_chat_started.py` & `pyAmang-1.0.3/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/pyrogram/utils.py` & `pyAmang-1.0.3/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/setup.py` & `pyAmang-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/tests/__init__.py` & `pyAmang-1.0.3/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/tests/filters/__init__.py` & `pyAmang-1.0.3/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/tests/filters/test_command.py` & `pyAmang-1.0.3/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/tests/parser/test_html.py` & `pyAmang-1.0.3/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `pyAmang-1.0.2/tests/test_file_id.py` & `pyAmang-1.0.3/tests/test_file_id.py`

 * *Files identical despite different names*

