# Comparing `tmp/PythonTwitchBotFramework-2.8.1.tar.gz` & `tmp/PythonTwitchBotFramework-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonTwitchBotFramework-2.8.1.tar", last modified: Wed Feb  8 00:24:21 2023, max compression
+gzip compressed data, was "PythonTwitchBotFramework-2.9.0.tar", last modified: Mon Mar  6 22:56:56 2023, max compression
```

## Comparing `PythonTwitchBotFramework-2.8.1.tar` & `PythonTwitchBotFramework-2.9.0.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.801739 PythonTwitchBotFramework-2.8.1/
--rw-rw-rw-   0        0        0     1088 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/LICENSE
--rw-rw-rw-   0        0        0       60 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0    27187 2023-02-08 00:24:20.800741 PythonTwitchBotFramework-2.8.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:19.878483 PythonTwitchBotFramework-2.8.1/PythonTwitchBotFramework.egg-info/
--rw-rw-rw-   0        0        0    27187 2023-02-08 00:24:19.000000 PythonTwitchBotFramework-2.8.1/PythonTwitchBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3836 2023-02-08 00:24:19.000000 PythonTwitchBotFramework-2.8.1/PythonTwitchBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 00:24:19.000000 PythonTwitchBotFramework-2.8.1/PythonTwitchBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-02-08 00:24:19.000000 PythonTwitchBotFramework-2.8.1/PythonTwitchBotFramework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-02-08 00:24:19.000000 PythonTwitchBotFramework-2.8.1/PythonTwitchBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    26859 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/README.md
--rw-rw-rw-   0        0        0       90 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/debug_requirements.txt
--rw-rw-rw-   0        0        0       70 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-08 00:24:20.801739 PythonTwitchBotFramework-2.8.1/setup.cfg
--rw-rw-rw-   0        0        0      858 2022-10-08 02:00:29.000000 PythonTwitchBotFramework-2.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:19.880478 PythonTwitchBotFramework-2.8.1/tests/
--rw-rw-rw-   0        0        0        0 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/tests/__init__.py
--rw-rw-rw-   0        0        0       62 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/tests/mock_irc.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:19.884467 PythonTwitchBotFramework-2.8.1/tests/test_events/
--rw-rw-rw-   0        0        0        0 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/tests/test_events/__init__.py
--rw-rw-rw-   0        0        0      338 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/tests/test_events/test_has_events.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.212318 PythonTwitchBotFramework-2.8.1/twitchbot/
--rw-rw-rw-   0        0        0     1072 2023-02-08 00:18:10.000000 PythonTwitchBotFramework-2.8.1/twitchbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.345958 PythonTwitchBotFramework-2.8.1/twitchbot/api/
--rw-rw-rw-   0        0        0       82 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/api/__init__.py
--rw-rw-rw-   0        0        0      872 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/api/baseapi.py
--rw-rw-rw-   0        0        0     2891 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/api/chatters.py
--rw-rw-rw-   0        0        0     1812 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/api/streaminfoapi.py
--rw-rw-rw-   0        0        0     1205 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/api/userinfoapi.py
--rw-rw-rw-   0        0        0     2279 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/arena.py
--rw-rw-rw-   0        0        0     1214 2023-02-01 02:10:30.000000 PythonTwitchBotFramework-2.8.1/twitchbot/argument_annotations.py
--rw-rw-rw-   0        0        0     1889 2023-02-01 00:55:07.000000 PythonTwitchBotFramework-2.8.1/twitchbot/auto_cast_handler.py
--rw-rw-rw-   0        0        0      228 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/bot_package_path.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.379950 PythonTwitchBotFramework-2.8.1/twitchbot/bots/
--rw-rw-rw-   0        0        0       22 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/bots/__init__.py
--rw-rw-rw-   0        0        0    19827 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/bots/basebot.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.468631 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/
--rw-rw-rw-   0        0        0        0 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/__init__.py
--rw-rw-rw-   0        0        0      499 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/admin_commands.py
--rw-rw-rw-   0        0        0     4008 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/cmd_management_commands.py
--rw-rw-rw-   0        0        0    16630 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/currency_commands.py
--rw-rw-rw-   0        0        0     3765 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/custom_commands.py
--rw-rw-rw-   0        0        0     3216 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/dbcounter_commands.py
--rw-rw-rw-   0        0        0     1038 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/debug_commands.py
--rw-rw-rw-   0        0        0     2178 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/fun_commands.py
--rw-rw-rw-   0        0        0     3351 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/misc_commands.py
--rw-rw-rw-   0        0        0     3731 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/mod_management_commands.py
--rw-rw-rw-   0        0        0     4540 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/permission_commands.py
--rw-rw-rw-   0        0        0     4974 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/poll_commands.py
--rw-rw-rw-   0        0        0     2867 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/quote_commands.py
--rw-rw-rw-   0        0        0     6335 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/timer_commands.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.505531 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/
--rw-rw-rw-   0        0        0        0 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/__init__.py
--rw-rw-rw-   0        0        0      309 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/channel_privmsg_time_updater_mod.py
--rw-rw-rw-   0        0        0     1117 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/channel_viewer_updater.py
--rw-rw-rw-   0        0        0     1063 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/loyalty_ticker_mod.py
--rw-rw-rw-   0        0        0      373 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/permissions_mod.py
--rw-rw-rw-   0        0        0      535 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/poll_announcer_mod.py
--rw-rw-rw-   0        0        0     1492 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/reply_waiter_mod.py
--rw-rw-rw-   0        0        0      492 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/timer_auto_start_mod.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.509521 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_translations/
--rw-rw-rw-   0        0        0    15019 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_translations/de_de.json
--rw-rw-rw-   0        0        0    19693 2023-02-08 00:24:17.000000 PythonTwitchBotFramework-2.8.1/twitchbot/builtin_translations/en_us.json
--rw-rw-rw-   0        0        0     2124 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/cached_property.py
--rw-rw-rw-   0        0        0     3757 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/channel.py
--rw-rw-rw-   0        0        0      350 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/colors.py
--rw-rw-rw-   0        0        0    16976 2023-02-08 00:17:49.000000 PythonTwitchBotFramework-2.8.1/twitchbot/command.py
--rw-rw-rw-   0        0        0    12666 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/command_server.py
--rw-rw-rw-   0        0        0     1290 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/command_whitelist.py
--rw-rw-rw-   0        0        0     8522 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/config.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.534454 PythonTwitchBotFramework-2.8.1/twitchbot/data/
--rw-rw-rw-   0        0        0      141 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/data/__init__.py
--rw-rw-rw-   0        0        0      362 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/data/follower.py
--rw-rw-rw-   0        0        0      954 2023-01-31 21:35:51.000000 PythonTwitchBotFramework-2.8.1/twitchbot/data/ratelimit.py
--rw-rw-rw-   0        0        0      940 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/data/user_followers.py
--rw-rw-rw-   0        0        0      283 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/data/userinfo.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.588310 PythonTwitchBotFramework-2.8.1/twitchbot/database/
--rw-rw-rw-   0        0        0      174 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/database/__init__.py
--rw-rw-rw-   0        0        0     1921 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/database/commands.py
--rw-rw-rw-   0        0        0     3562 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/database/currency.py
--rw-rw-rw-   0        0        0     4112 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/database/dbcounter.py
--rw-rw-rw-   0        0        0     5377 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/database/message_timer.py
--rw-rw-rw-   0        0        0     4178 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/database/models.py
--rw-rw-rw-   0        0        0     2549 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/database/quotes.py
--rw-rw-rw-   0        0        0     2410 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/database/session.py
--rw-rw-rw-   0        0        0     1167 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/disabled_commands.py
--rw-rw-rw-   0        0        0     2022 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/disabled_mods.py
--rw-rw-rw-   0        0        0     3101 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/duel.py
--rw-rw-rw-   0        0        0      611 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/emote.py
--rw-rw-rw-   0        0        0     2216 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/enums.py
--rw-rw-rw-   0        0        0     3030 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/event_util.py
--rw-rw-rw-   0        0        0     1179 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/events.py
--rw-rw-rw-   0        0        0      991 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.598284 PythonTwitchBotFramework-2.8.1/twitchbot/extra_configs/
--rw-rw-rw-   0        0        0       29 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/extra_configs/__init__.py
--rw-rw-rw-   0        0        0      298 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/extra_configs/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.601275 PythonTwitchBotFramework-2.8.1/twitchbot/gui/
--rw-rw-rw-   0        0        0       27 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/gui/__init__.py
--rw-rw-rw-   0        0        0     1112 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/gui/getpassgui.py
--rw-rw-rw-   0        0        0     9222 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/irc.py
--rw-rw-rw-   0        0        0    16849 2022-11-22 18:23:39.000000 PythonTwitchBotFramework-2.8.1/twitchbot/message.py
--rw-rw-rw-   0        0        0    16614 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/modloader.py
--rw-rw-rw-   0        0        0     7200 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/permission.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.609254 PythonTwitchBotFramework-2.8.1/twitchbot/poll/
--rw-rw-rw-   0        0        0       25 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/poll/__init__.py
--rw-rw-rw-   0        0        0     5583 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/poll/polldata.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.673083 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/
--rw-rw-rw-   0        0        0      477 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/__init__.py
--rw-rw-rw-   0        0        0     2125 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/bits_model.py
--rw-rw-rw-   0        0        0     9730 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/client.py
--rw-rw-rw-   0        0        0     5885 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/models.py
--rw-rw-rw-   0        0        0     4195 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/point_redemption_model.py
--rw-rw-rw-   0        0        0     1558 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/pubsub_follow.py
--rw-rw-rw-   0        0        0     1477 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/pubsub_moderation_action.py
--rw-rw-rw-   0        0        0     2703 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/pubsub_poll_update.py
--rw-rw-rw-   0        0        0     2385 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/subscription_model.py
--rw-rw-rw-   0        0        0      481 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/topics.py
--rw-rw-rw-   0        0        0      738 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/twitch_poll_vote_choice.py
--rw-rw-rw-   0        0        0     1046 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/whisper_model.py
--rw-rw-rw-   0        0        0     1900 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/ratelimit.py
--rw-rw-rw-   0        0        0     1513 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/regex.py
--rw-rw-rw-   0        0        0     5587 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/replywaiter.py
--rw-rw-rw-   0        0        0      753 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/shared.py
--rw-rw-rw-   0        0        0     4365 2023-01-31 21:35:51.000000 PythonTwitchBotFramework-2.8.1/twitchbot/tags.py
--rw-rw-rw-   0        0        0     2110 2022-09-29 03:34:02.000000 PythonTwitchBotFramework-2.8.1/twitchbot/translations.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.789771 PythonTwitchBotFramework-2.8.1/twitchbot/util/
--rw-rw-rw-   0        0        0      349 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/__init__.py
--rw-rw-rw-   0        0        0     3325 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/command_util.py
--rw-rw-rw-   0        0        0     1566 2023-01-31 20:17:00.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/cooldown_manager.py
--rw-rw-rw-   0        0        0      369 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/database_util.py
--rw-rw-rw-   0        0        0      916 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/dict_util.py
--rw-rw-rw-   0        0        0      391 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/environment_util.py
--rw-rw-rw-   0        0        0     1207 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/message_util.py
--rw-rw-rw-   0        0        0     1187 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/misc_util.py
--rw-rw-rw-   0        0        0      740 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/register_util.py
--rw-rw-rw-   0        0        0      218 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/string_util.py
--rw-rw-rw-   0        0        0     2204 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/task_util.py
--rw-rw-rw-   0        0        0    12171 2022-11-22 19:56:14.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/twitch_api_util.py
--rw-rw-rw-   0        0        0     7152 2023-02-08 00:22:21.000000 PythonTwitchBotFramework-2.8.1/twitchbot/util/typing_utils.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:20.790769 PythonTwitchBotFramework-2.8.1/util/
--rw-rw-rw-   0        0        0     8115 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.8.1/util/command_console.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:55.491456 PythonTwitchBotFramework-2.9.0/
+-rw-rw-rw-   0        0        0     1088 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    27187 2023-03-06 22:56:55.035058 PythonTwitchBotFramework-2.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.924353 PythonTwitchBotFramework-2.9.0/PythonTwitchBotFramework.egg-info/
+-rw-rw-rw-   0        0        0    27187 2023-03-06 22:56:53.000000 PythonTwitchBotFramework-2.9.0/PythonTwitchBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3876 2023-03-06 22:56:53.000000 PythonTwitchBotFramework-2.9.0/PythonTwitchBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-06 22:56:53.000000 PythonTwitchBotFramework-2.9.0/PythonTwitchBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-03-06 22:56:53.000000 PythonTwitchBotFramework-2.9.0/PythonTwitchBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-03-06 22:56:53.000000 PythonTwitchBotFramework-2.9.0/PythonTwitchBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    26859 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/README.md
+-rw-rw-rw-   0        0        0       90 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/debug_requirements.txt
+-rw-rw-rw-   0        0        0       70 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-03-06 22:56:55.491456 PythonTwitchBotFramework-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      858 2022-10-08 02:00:29.000000 PythonTwitchBotFramework-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.926349 PythonTwitchBotFramework-2.9.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/tests/__init__.py
+-rw-rw-rw-   0        0        0       62 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/tests/mock_irc.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.928345 PythonTwitchBotFramework-2.9.0/tests/test_events/
+-rw-rw-rw-   0        0        0        0 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/tests/test_events/__init__.py
+-rw-rw-rw-   0        0        0      338 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/tests/test_events/test_has_events.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.959260 PythonTwitchBotFramework-2.9.0/twitchbot/
+-rw-rw-rw-   0        0        0     1115 2023-03-06 22:44:51.000000 PythonTwitchBotFramework-2.9.0/twitchbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.964249 PythonTwitchBotFramework-2.9.0/twitchbot/api/
+-rw-rw-rw-   0        0        0       82 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/api/__init__.py
+-rw-rw-rw-   0        0        0      872 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/api/baseapi.py
+-rw-rw-rw-   0        0        0     2891 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/api/chatters.py
+-rw-rw-rw-   0        0        0     1812 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/api/streaminfoapi.py
+-rw-rw-rw-   0        0        0     1205 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/api/userinfoapi.py
+-rw-rw-rw-   0        0        0     2279 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/arena.py
+-rw-rw-rw-   0        0        0     1214 2023-02-01 02:10:30.000000 PythonTwitchBotFramework-2.9.0/twitchbot/argument_annotations.py
+-rw-rw-rw-   0        0        0     1889 2023-02-01 00:55:07.000000 PythonTwitchBotFramework-2.9.0/twitchbot/auto_cast_handler.py
+-rw-rw-rw-   0        0        0      228 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/bot_package_path.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.966244 PythonTwitchBotFramework-2.9.0/twitchbot/bots/
+-rw-rw-rw-   0        0        0       22 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/bots/__init__.py
+-rw-rw-rw-   0        0        0    20038 2023-03-06 22:38:10.000000 PythonTwitchBotFramework-2.9.0/twitchbot/bots/basebot.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.980204 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/
+-rw-rw-rw-   0        0        0        0 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/__init__.py
+-rw-rw-rw-   0        0        0      499 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/admin_commands.py
+-rw-rw-rw-   0        0        0     4008 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/cmd_management_commands.py
+-rw-rw-rw-   0        0        0    16630 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/currency_commands.py
+-rw-rw-rw-   0        0        0     3765 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/custom_commands.py
+-rw-rw-rw-   0        0        0     3216 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/dbcounter_commands.py
+-rw-rw-rw-   0        0        0     1038 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/debug_commands.py
+-rw-rw-rw-   0        0        0     2178 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/fun_commands.py
+-rw-rw-rw-   0        0        0     3351 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/misc_commands.py
+-rw-rw-rw-   0        0        0     3731 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/mod_management_commands.py
+-rw-rw-rw-   0        0        0     4540 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/permission_commands.py
+-rw-rw-rw-   0        0        0     4974 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/poll_commands.py
+-rw-rw-rw-   0        0        0     2867 2022-09-14 02:40:08.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/quote_commands.py
+-rw-rw-rw-   0        0        0     6335 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/timer_commands.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.987186 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/
+-rw-rw-rw-   0        0        0        0 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/__init__.py
+-rw-rw-rw-   0        0        0      309 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/channel_privmsg_time_updater_mod.py
+-rw-rw-rw-   0        0        0     1117 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/channel_viewer_updater.py
+-rw-rw-rw-   0        0        0     1063 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/loyalty_ticker_mod.py
+-rw-rw-rw-   0        0        0      373 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/permissions_mod.py
+-rw-rw-rw-   0        0        0      535 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/poll_announcer_mod.py
+-rw-rw-rw-   0        0        0     1492 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/reply_waiter_mod.py
+-rw-rw-rw-   0        0        0      492 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/timer_auto_start_mod.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.993169 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_translations/
+-rw-rw-rw-   0        0        0    15019 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_translations/de_de.json
+-rw-rw-rw-   0        0        0    19693 2023-03-06 22:56:52.000000 PythonTwitchBotFramework-2.9.0/twitchbot/builtin_translations/en_us.json
+-rw-rw-rw-   0        0        0     2124 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/cached_property.py
+-rw-rw-rw-   0        0        0     4596 2023-03-06 22:38:10.000000 PythonTwitchBotFramework-2.9.0/twitchbot/channel.py
+-rw-rw-rw-   0        0        0      350 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/colors.py
+-rw-rw-rw-   0        0        0    16976 2023-02-08 00:17:49.000000 PythonTwitchBotFramework-2.9.0/twitchbot/command.py
+-rw-rw-rw-   0        0        0    12666 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/command_server.py
+-rw-rw-rw-   0        0        0     1290 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/command_whitelist.py
+-rw-rw-rw-   0        0        0     8522 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/config.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:54.998159 PythonTwitchBotFramework-2.9.0/twitchbot/data/
+-rw-rw-rw-   0        0        0      141 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/data/__init__.py
+-rw-rw-rw-   0        0        0      362 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/data/follower.py
+-rw-rw-rw-   0        0        0     1048 2023-03-06 22:38:10.000000 PythonTwitchBotFramework-2.9.0/twitchbot/data/ratelimit.py
+-rw-rw-rw-   0        0        0      940 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/data/user_followers.py
+-rw-rw-rw-   0        0        0      283 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/data/userinfo.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:55.005138 PythonTwitchBotFramework-2.9.0/twitchbot/database/
+-rw-rw-rw-   0        0        0      174 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/database/__init__.py
+-rw-rw-rw-   0        0        0     1921 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/database/commands.py
+-rw-rw-rw-   0        0        0     3562 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/database/currency.py
+-rw-rw-rw-   0        0        0     4112 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/database/dbcounter.py
+-rw-rw-rw-   0        0        0     5377 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/database/message_timer.py
+-rw-rw-rw-   0        0        0     4178 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/database/models.py
+-rw-rw-rw-   0        0        0     2549 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/database/quotes.py
+-rw-rw-rw-   0        0        0     2410 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/database/session.py
+-rw-rw-rw-   0        0        0     1167 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/disabled_commands.py
+-rw-rw-rw-   0        0        0     2022 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/disabled_mods.py
+-rw-rw-rw-   0        0        0     3101 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/duel.py
+-rw-rw-rw-   0        0        0      611 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/emote.py
+-rw-rw-rw-   0        0        0     2216 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/enums.py
+-rw-rw-rw-   0        0        0     3030 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/event_util.py
+-rw-rw-rw-   0        0        0     1179 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/events.py
+-rw-rw-rw-   0        0        0      991 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:55.007133 PythonTwitchBotFramework-2.9.0/twitchbot/extra_configs/
+-rw-rw-rw-   0        0        0       29 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/extra_configs/__init__.py
+-rw-rw-rw-   0        0        0      298 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/extra_configs/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:55.008129 PythonTwitchBotFramework-2.9.0/twitchbot/gui/
+-rw-rw-rw-   0        0        0       27 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/gui/__init__.py
+-rw-rw-rw-   0        0        0     1112 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/gui/getpassgui.py
+-rw-rw-rw-   0        0        0     9222 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/irc.py
+-rw-rw-rw-   0        0        0    17106 2023-03-06 22:38:10.000000 PythonTwitchBotFramework-2.9.0/twitchbot/message.py
+-rw-rw-rw-   0        0        0    16614 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/modloader.py
+-rw-rw-rw-   0        0        0     7200 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/permission.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:55.010126 PythonTwitchBotFramework-2.9.0/twitchbot/poll/
+-rw-rw-rw-   0        0        0       25 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/poll/__init__.py
+-rw-rw-rw-   0        0        0     5583 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/poll/polldata.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:55.021095 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/
+-rw-rw-rw-   0        0        0      477 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/__init__.py
+-rw-rw-rw-   0        0        0     2125 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/bits_model.py
+-rw-rw-rw-   0        0        0     9730 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/client.py
+-rw-rw-rw-   0        0        0     5885 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/models.py
+-rw-rw-rw-   0        0        0     4195 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/point_redemption_model.py
+-rw-rw-rw-   0        0        0     1558 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/pubsub_follow.py
+-rw-rw-rw-   0        0        0     1477 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/pubsub_moderation_action.py
+-rw-rw-rw-   0        0        0     2703 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/pubsub_poll_update.py
+-rw-rw-rw-   0        0        0     2385 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/subscription_model.py
+-rw-rw-rw-   0        0        0      481 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/topics.py
+-rw-rw-rw-   0        0        0      738 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/twitch_poll_vote_choice.py
+-rw-rw-rw-   0        0        0     1046 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/whisper_model.py
+-rw-rw-rw-   0        0        0     1900 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/ratelimit.py
+-rw-rw-rw-   0        0        0     5335 2023-03-06 22:38:10.000000 PythonTwitchBotFramework-2.9.0/twitchbot/ratelimit_twitch_api_queue.py
+-rw-rw-rw-   0        0        0     1513 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/regex.py
+-rw-rw-rw-   0        0        0     5587 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/replywaiter.py
+-rw-rw-rw-   0        0        0      753 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/shared.py
+-rw-rw-rw-   0        0        0     4365 2023-01-31 21:35:51.000000 PythonTwitchBotFramework-2.9.0/twitchbot/tags.py
+-rw-rw-rw-   0        0        0     2110 2022-09-29 03:34:02.000000 PythonTwitchBotFramework-2.9.0/twitchbot/translations.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:55.033064 PythonTwitchBotFramework-2.9.0/twitchbot/util/
+-rw-rw-rw-   0        0        0      349 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/__init__.py
+-rw-rw-rw-   0        0        0     3325 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/command_util.py
+-rw-rw-rw-   0        0        0     1566 2023-01-31 20:17:00.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/cooldown_manager.py
+-rw-rw-rw-   0        0        0      369 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/database_util.py
+-rw-rw-rw-   0        0        0      916 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/dict_util.py
+-rw-rw-rw-   0        0        0      391 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/environment_util.py
+-rw-rw-rw-   0        0        0     1207 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/message_util.py
+-rw-rw-rw-   0        0        0     1187 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/misc_util.py
+-rw-rw-rw-   0        0        0      740 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/register_util.py
+-rw-rw-rw-   0        0        0      218 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/string_util.py
+-rw-rw-rw-   0        0        0     2204 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/task_util.py
+-rw-rw-rw-   0        0        0    17890 2023-03-06 22:46:50.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/twitch_api_util.py
+-rw-rw-rw-   0        0        0     7152 2023-02-08 00:22:21.000000 PythonTwitchBotFramework-2.9.0/twitchbot/util/typing_utils.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:56:55.034061 PythonTwitchBotFramework-2.9.0/util/
+-rw-rw-rw-   0        0        0     8115 2022-09-14 02:40:09.000000 PythonTwitchBotFramework-2.9.0/util/command_console.py
```

### Comparing `PythonTwitchBotFramework-2.8.1/LICENSE` & `PythonTwitchBotFramework-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/PKG-INFO` & `PythonTwitchBotFramework-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonTwitchBotFramework
-Version: 2.8.1
+Version: 2.9.0
 Summary: asynchronous twitch-bot framework made in pure python
 Home-page: https://github.com/sharkbound/PythonTwitchBotFramework
 Author: sharkbound
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PythonTwitchBotFramework-2.8.1/PythonTwitchBotFramework.egg-info/PKG-INFO` & `PythonTwitchBotFramework-2.9.0/PythonTwitchBotFramework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonTwitchBotFramework
-Version: 2.8.1
+Version: 2.9.0
 Summary: asynchronous twitch-bot framework made in pure python
 Home-page: https://github.com/sharkbound/PythonTwitchBotFramework
 Author: sharkbound
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PythonTwitchBotFramework-2.8.1/PythonTwitchBotFramework.egg-info/SOURCES.txt` & `PythonTwitchBotFramework-2.9.0/PythonTwitchBotFramework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 twitchbot/events.py
 twitchbot/exceptions.py
 twitchbot/irc.py
 twitchbot/message.py
 twitchbot/modloader.py
 twitchbot/permission.py
 twitchbot/ratelimit.py
+twitchbot/ratelimit_twitch_api_queue.py
 twitchbot/regex.py
 twitchbot/replywaiter.py
 twitchbot/shared.py
 twitchbot/tags.py
 twitchbot/translations.py
 twitchbot/api/__init__.py
 twitchbot/api/baseapi.py
```

### Comparing `PythonTwitchBotFramework-2.8.1/README.md` & `PythonTwitchBotFramework-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/setup.py` & `PythonTwitchBotFramework-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/__init__.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .bot_package_path import _set_bot_package_path, get_bot_package_path
 
-BOT_VERSION = (2, 8, 1)
+BOT_VERSION = (2, 9, 0)
 _set_bot_package_path(__path__[0])
 
 from .arena import *
 from .channel import *
 from .api.chatters import *
 from .colors import *
 from .command import *
@@ -32,8 +32,9 @@
 from .command_whitelist import *
 from .poll import *
 from .event_util import *
 from .extra_configs import *
 from .pubsub import *
 from .translations import *
 from .argument_annotations import *
-from .auto_cast_handler import *
+from .auto_cast_handler import *
+from .ratelimit_twitch_api_queue import *
```

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/api/baseapi.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/api/baseapi.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/api/chatters.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/api/chatters.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/api/streaminfoapi.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/api/streaminfoapi.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/api/userinfoapi.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/api/userinfoapi.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/arena.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/arena.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/argument_annotations.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/argument_annotations.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/auto_cast_handler.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/auto_cast_handler.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/bots/basebot.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/bots/basebot.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,19 +391,23 @@
 
         await self._init_bot()
 
         util.add_task('poll_event_processor', poll_event_processor_loop())
         self._create_channels()
 
         await self.irc.connect_to_twitch()
-
+        
+        from ..ratelimit_twitch_api_queue import start_twitch_api_queue_send_handler_loop
+        start_twitch_api_queue_send_handler_loop()
+        
         await self.on_connected()
+        
         await trigger_mod_event(Event.on_connected)
         await trigger_event(Event.on_connected)
-
+        
         await self._read_process_loop()
 
         # clean up mods when the bot is exiting
         for mod in mods.values():
             # notify all mods of being unloaded,
             # this is put in a try/except
             # so that any exceptions raised from unloaded overrides will not cancel unloading the others
@@ -413,14 +417,15 @@
                 print(f'\nwhen unloading mod "{mod.name}" this exception occurred:\n')
                 logging.exception(e)
 
     async def _read_process_loop(self):
         while self._running:
             try:
                 raw_msg = await self.irc.get_next_message()
+                print(raw_msg)
             except BotNotRunningError:
                 return
 
             if not raw_msg:
                 continue
 
             msg = Message(raw_msg, irc=self.irc, bot=self)
```

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/cmd_management_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/cmd_management_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/currency_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/currency_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/custom_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/custom_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/dbcounter_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/dbcounter_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/debug_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/debug_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/fun_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/fun_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/misc_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/misc_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/mod_management_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/mod_management_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/permission_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/permission_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/poll_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/poll_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/quote_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/quote_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_commands/timer_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_commands/timer_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/channel_viewer_updater.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/channel_viewer_updater.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/loyalty_ticker_mod.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/loyalty_ticker_mod.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/poll_announcer_mod.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/poll_announcer_mod.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_mods/reply_waiter_mod.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_mods/reply_waiter_mod.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_translations/de_de.json` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_translations/de_de.json`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/builtin_translations/en_us.json` & `PythonTwitchBotFramework-2.9.0/twitchbot/builtin_translations/en_us.json`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/cached_property.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/cached_property.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/channel.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/channel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import asyncio
 import time
 import typing
+import warnings
+from json import JSONEncoder
 from datetime import datetime
 from typing import Dict
 
 from .api import StreamInfoApi
 from .api.chatters import Chatters
 from .config import get_nick, get_client_id
 from .data import UserFollowers
 from .permission import perms
 from .shared import get_bot
-from .util import get_user_followers, get_headers, strip_twitch_command_prefix, normalize_string
+from .util import get_user_followers, get_headers, strip_twitch_command_prefix, normalize_string, send_announcement, send_shoutout, send_ban
 
 if typing.TYPE_CHECKING:
     from .bots import BaseBot
     from .irc import Irc
 
 
 class Channel:
@@ -62,14 +64,19 @@
                 self.is_vip = get_nick().lower() in self.chatters.vips
                 await asyncio.sleep(120)  # update viewers every 2 minutes
 
     async def ban(self, user: str, reason: str = ''):
         """purges a user's messages then permabans them from the channel"""
         await self.send_command(f'ban {user} {reason}')
 
+    async def ban2(self, user: str, reason: str = '', timeout: int = None):
+        """purges a user's messages then bans a user a given time in seconds (1 - 1209600 [2 weeks]; default permanent) from the channel using twitch API"""
+        await send_ban(self.name, user, reason, timeout)
+        
+
     async def timeout(self, user: str, duration: int = 600):
         """
         purges a user's messages then times out the user (makes them unable to chat)
         for the specified duration (default 600 seconds)
         """
         await self.send_command(f'timeout {user} {duration}')
 
@@ -79,14 +86,26 @@
         :param user: user to purge
         """
         await self.timeout(user, 1)
 
     async def color(self, color: str):
         """sets the bots chat color"""
         await self.send_command(f'color {color}')
+    
+    async def shoutout(self, target: str):
+        """
+        Sends a shoutout to another streamer
+        """
+        await send_shoutout(self.name, target)
+
+    async def announcement(self, message:str, color:str = None):
+        """
+        Creates an announcement with a message of maximum 500 chars and optional a color: blue, green, orange, purple
+        """
+        await send_announcement(self.name, message, color)
 
     def __str__(self):
         return f'<Channel name={repr(self.name)}>'
 
     def __eq__(self, other):
         if isinstance(other, str):
             return self.name.lower() == other.lower()
```

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/command.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/command.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/command_server.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/command_server.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/command_whitelist.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/command_whitelist.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/config.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/config.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/data/user_followers.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/data/user_followers.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/database/commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/database/commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/database/currency.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/database/currency.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/database/dbcounter.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/database/dbcounter.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/database/message_timer.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/database/message_timer.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/database/models.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/database/models.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/database/quotes.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/database/quotes.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/database/session.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/database/session.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/disabled_commands.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/disabled_commands.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/disabled_mods.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/disabled_mods.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/duel.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/duel.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/emote.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/emote.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/enums.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/enums.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/event_util.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/event_util.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/events.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/events.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/exceptions.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/gui/getpassgui.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/gui/getpassgui.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/irc.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/irc.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/message.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import traceback
+import warnings
 from datetime import datetime
 from itertools import islice
 from typing import List, Tuple, TYPE_CHECKING, Optional, Callable, Awaitable, Union
 
 from .util import get_message_mentions
 from .channel import Channel, channels
 from .regex import RE_PRIVMSG, RE_WHISPER, RE_USER_JOIN, RE_USERNOTICE, RE_USER_PART, RE_NOTICE, RE_TIMEOUT_DURATION
@@ -285,14 +286,16 @@
 
     @property
     def has_required_tags_for_twitch_reply(self):
         tags = self.tags
         return tags is not None and all((tags.display_name, self.content is not None, tags.id, tags.user_id, self.author))
 
     async def send_command(self, msg: str = '', whisper=False):
+        warnings.warn('twitch moved commands to API Calls, sending them via chat commands using IRC no longer works,'
+                      ' instead use the `send_` functions from the twitchbot import', DeprecationWarning, stacklevel=2)
         msg = f'/{strip_twitch_command_prefix(msg)}'
         await self.reply(msg=msg, whisper=whisper, strip_command_prefix=False)
 
     async def reply(self, msg: str = '', whisper=False, strip_command_prefix: bool = True, as_twitch_reply: bool = False):
         if not msg:
             raise ValueError('msg is empty, msg must be a non-empty string')
```

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/modloader.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/modloader.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/permission.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/permission.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/poll/polldata.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/poll/polldata.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/bits_model.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/bits_model.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/client.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/client.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/models.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/models.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/point_redemption_model.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/point_redemption_model.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/pubsub_follow.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/pubsub_follow.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/pubsub_moderation_action.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/pubsub_moderation_action.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/pubsub_poll_update.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/pubsub_poll_update.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/subscription_model.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/subscription_model.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/twitch_poll_vote_choice.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/twitch_poll_vote_choice.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/pubsub/whisper_model.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/pubsub/whisper_model.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/ratelimit.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/ratelimit.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/regex.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/regex.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/replywaiter.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/replywaiter.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/shared.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/shared.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/tags.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/tags.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/translations.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/translations.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/command_util.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/command_util.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/cooldown_manager.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/cooldown_manager.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/dict_util.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/dict_util.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/message_util.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/message_util.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/misc_util.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/misc_util.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/register_util.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/register_util.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/task_util.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/task_util.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/twitch_api_util.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/twitch_api_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import warnings
+
+from typing import Dict, Tuple, NamedTuple, Optional, Any
 from collections import namedtuple
 from datetime import datetime
-from json import JSONDecodeError
-from typing import Dict, Tuple, NamedTuple, Optional
+from json import JSONDecodeError, JSONEncoder, dumps as json_dumps
 
 from aiohttp import ClientSession, ClientResponse, ContentTypeError
 from async_timeout import timeout
 
-from ..config import get_client_id, get_oauth, DEFAULT_CLIENT_ID
+from ..config import get_client_id, get_oauth, get_nick, DEFAULT_CLIENT_ID
 from ..data import UserFollowers, UserInfo, Follower
 
 __all__ = ('CHANNEL_CHATTERS_URL', 'get_channel_chatters', 'get_stream_data', 'get_url', 'get_user_data', 'get_user_id',
            'STREAM_API_URL', 'USER_API_URL', 'get_user_followers', 'USER_FOLLOWERS_API_URL', 'get_headers',
            'get_user_info', 'USER_ACCOUNT_AGE_API', 'CHANNEL_INFO_API', 'get_channel_info', 'ChannelInfo',
            'get_channel_name_from_user_id', 'OauthTokenInfo', 'get_oauth_token_info', '_check_token', 'post_url', 'USER_FOLLOWAGE_API_URL',
-           'get_user_followage')
+           'get_user_followage', 'send_shoutout', 'send_announcement', 'send_ban')
 
 USER_API_URL = 'https://api.twitch.tv/helix/users?login={}'
 STREAM_API_URL = 'https://api.twitch.tv/helix/streams?user_login={}'
 CHANNEL_CHATTERS_URL = 'https://tmi.twitch.tv/group/user/{}/chatters'
 USER_FOLLOWERS_API_URL = 'https://api.twitch.tv/helix/users/follows?to_id={}'
 USER_ACCOUNT_AGE_API = 'https://api.twitch.tv/kraken/users/{}'
 CHANNEL_INFO_API = 'https://api.twitch.tv/helix/channels?broadcaster_id={}'
 USER_FOLLOWAGE_API_URL = 'https://api.twitch.tv/helix/users/follows?to_id={}&from_id={}'
+SHOUTOUT_API_URL = 'https://api.twitch.tv/helix/chat/shoutouts?from_broadcaster_id={}&to_broadcaster_id={}&moderator_id={}'
+ANNOUNCEMENTS_API_URL = 'https://api.twitch.tv/helix/chat/announcements?broadcaster_id={}&moderator_id={}'
+BAN_API_URL = 'https://api.twitch.tv/helix/moderation/bans?broadcaster_id={}&moderator_id={}'
 
 user_id_cache: Dict[str, int] = {}
 
 
 async def get_url(url: str, headers: dict = None) -> Tuple[ClientResponse, dict]:
     headers = headers if headers is not None else get_headers()
     async with ClientSession(headers=headers) as session:
         async with timeout(10):
             async with session.get(url) as resp:
                 return await _extract_response_and_json_from_request(resp)
 
 
-async def post_url(url: str, headers: dict = None) -> Tuple[ClientResponse, dict]:
+async def post_url(url: str, headers: dict = None, body: Any = None) -> Tuple[ClientResponse, dict]:
     headers = headers if headers is not None else get_headers()
     async with ClientSession(headers=headers) as session:
         async with timeout(10):
-            async with session.post(url) as resp:
+            async with session.post(url, data=body) as resp:
                 return await _extract_response_and_json_from_request(resp)
 
 
 def _check_headers_has_auth(headers: dict) -> bool:
     return CLIENT_ID_KEY in headers and AUTHORIZATION_KEY in headers
 
 
@@ -53,15 +57,15 @@
     except (ContentTypeError, JSONDecodeError, TypeError):
         return resp, {}
 
 
 async def get_user_info(user: str) -> UserInfo:
     headers = get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_USER_INFO] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_USER_INFO] headers for the twitch api request are missing authorization', stacklevel=2)
         return UserInfo(-1, '', '', '', '', '', '', '', -1)
 
     _, json = await get_url(USER_API_URL.format(user), headers)
 
     if 'error' in json or not json.get('data', None):
         return UserInfo(-1, '', '', '', '', '', '', '', -1)
 
@@ -78,15 +82,15 @@
         view_count=data['view_count']
     )
 
 
 async def get_user_followers(user: str, headers: dict = None) -> UserFollowers:
     headers = headers if headers is not None else get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_USER_FOLLOWERS] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_USER_FOLLOWERS] headers for the twitch api request are missing authorization', stacklevel=2)
         return UserFollowers(-1, '', -1, '', -1, [])
 
     user_id = await get_user_id(user, headers)
     _, json = await get_url(USER_FOLLOWERS_API_URL.format(user_id), headers)
 
     # covers invalid user id, or some other API error, such as invalid client-id
     if not json or json.get('status', -1) == 400:
@@ -99,15 +103,15 @@
                          id=user_id_cache[user],
                          followers=json['data'])
 
 
 async def get_user_followage(channel_name: str, follower: str, headers: dict = None) -> Follower:
     headers = headers if headers is not None else get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_USER_FOLLOWAGE] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_USER_FOLLOWAGE] headers for the twitch api request are missing authorization', stacklevel=2)
         return Follower(-1, '', -1, '', datetime.min)
 
     channel_id = await get_user_id(channel_name, headers)
     follower_id = await get_user_id(follower, headers)
     _, json = await get_url(USER_FOLLOWAGE_API_URL.format(channel_id, follower_id), headers)
 
     # verify that the api response has data, and its total is not 0
@@ -119,66 +123,170 @@
                     following_id=channel_id,
                     id=follower_id,
                     name=json['data'][0]['from_name'],
                     # datetime format: 2019-10-23T23:12:06Z
                     followed_at=datetime.fromisoformat(json['data'][0]['followed_at'][:-1]))
 
 
+async def send_shoutout(channel_name: str, target_name: str, headers: dict = None) -> None:
+    headers = (headers.copy() if headers is not None else get_headers())
+    if not _check_headers_has_auth(headers):
+        warnings.warn('[SHOUTOUT] headers for the twitch api request are missing authorization', stacklevel=2)
+
+    channel_id = await get_user_id(channel_name, headers)
+    target_id = await get_user_id(target_name, headers)
+    moderator_id = await get_user_id(get_nick(), headers)
+
+    from ..ratelimit_twitch_api_queue import enqueue_twitch_api_request, PendingTwitchAPIRequestMode
+    resp, json = await enqueue_twitch_api_request(
+        SHOUTOUT_API_URL.format(channel_id, target_id, moderator_id),
+        headers=headers,
+        mode=PendingTwitchAPIRequestMode.POST
+    )
+
+    if (resp.status != 204):
+        warnings.warn(f'Shoutout failed with error code: {resp.status}.\nResponse: {await resp.text("utf-8")}\nSee "https://dev.twitch.tv/docs/api/reference/#send-a-shoutout"', stacklevel=2)
+
+    return
+
+
+async def send_announcement(channel_name: str, message: str, color: str = None, headers: dict = None) -> None:
+    headers = headers.copy() if headers is not None else get_headers()
+    if not _check_headers_has_auth(headers):
+        warnings.warn('[ANNOUNCEMENT] headers for the twitch api request are missing authorization', stacklevel=2)
+
+    channel_id = await get_user_id(channel_name, headers)
+    moderator_id = await get_user_id(get_nick(), headers)
+
+    if len(message) > 500:
+        warnings.warn(f'Announcements messages above 500 Characters are trunscated by Twitch. Given length is {len(message)}', stacklevel=2)
+
+    if color not in {'blue', 'green', 'orange', 'purple'}:
+        warnings.warn(f'Announcements color can only be blue, green, orange or purple. Given color is {color} defaulting to primary', stacklevel=2)
+        color = 'primary'
+
+    body = json_dumps({'message': message, 'color': color})
+
+    headers.update({'Content-Type': 'application/json'})
+    from ..ratelimit_twitch_api_queue import enqueue_twitch_api_request, PendingTwitchAPIRequestMode
+    resp, json = await enqueue_twitch_api_request(
+        ANNOUNCEMENTS_API_URL.format(channel_id, moderator_id),
+        headers=headers,
+        body=body,
+        mode=PendingTwitchAPIRequestMode.POST
+    )
+    # resp, json = await post_url(ANNOUNCEMENTS_API_URL.format(channel_id, moderator_id), headers, body=body)
+
+    if (resp.status != 204):
+        warnings.warn(f'Announcement failed with error code: {resp.status}.\nResponse Text: {await resp.text()}.\nSee "https://dev.twitch.tv/docs/api/reference/#send-chat-announcement"', stacklevel=2)
+
+    return
+
+
+async def send_ban(channel_name: str, username: str, reason: str = None, timeout: int = None, headers: dict = None) -> None:
+    headers = headers.copy() if headers is not None else get_headers()
+    if not _check_headers_has_auth(headers):
+        warnings.warn('[BAN] headers for the twitch api request are missing authorization', stacklevel=2)
+
+    channel_id = await get_user_id(channel_name, headers)
+    user_id = await get_user_id(username, headers)
+    moderator_id = await get_user_id(get_nick(), headers)
+
+    if len(reason) > 500:
+        reason = reason[:500]
+        warnings.warn(f'[BAN] reasons above 500 Characters is limited by Twitch and will be trunscated. Given length is {len(reason)}.', stacklevel=2)
+
+    # Split it into two If-statements for better understanding
+    if timeout is not None:
+        # Just for safety
+        if not isinstance(timeout, int):
+            warnings.warn(f'[BAN] timeout need to be of type integer. Given type is {type(timeout)}. ABORTING!', stacklevel=2)
+            return
+
+        elif not 1 <= timeout <= 1209600:
+            warnings.warn(f'[BAN] timeout needs to be between 1 or 1209600 Seconds (2 Weeks). Given timout is {timeout}, setting to 600 Seconds.', stacklevel=2)
+            timeout = 600
+
+        body = json_dumps({'data': {'user_id': user_id, 'duration': timeout, 'reason': reason}})
+    else:
+        # Permanent Ban
+        body = json_dumps({'data': {'user_id': user_id, 'reason': reason}})
+
+    headers.update({'Content-Type': 'application/json'})
+    from ..ratelimit_twitch_api_queue import enqueue_twitch_api_request, PendingTwitchAPIRequestMode
+    resp, json = await enqueue_twitch_api_request(
+        BAN_API_URL.format(channel_id, moderator_id),
+        headers=headers,
+        body=body,
+        mode=PendingTwitchAPIRequestMode.POST
+    )
+
+    if (resp is not None and resp.status != 200):
+        returnMessage = json['message']
+        warnings.warn(
+            f'Ban failed with error code: {resp.status} with message "{returnMessage}". See "https://dev.twitch.tv/docs/api/reference/#ban-user"', stacklevel=2)
+
+    return resp
+
+
 async def get_user_data(user: str, headers: dict = None) -> dict:
     headers = headers if headers is not None else get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_USER_DATA] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_USER_DATA] headers for the twitch api request are missing authorization', stacklevel=2)
         return {}
 
-    _, json = await get_url(USER_API_URL.format(user), headers)
+    # _, json = await get_url(USER_API_URL.format(user), headers)
+    from ..ratelimit_twitch_api_queue import enqueue_twitch_api_request, PendingTwitchAPIRequestMode
+    _, json = await enqueue_twitch_api_request(USER_API_URL.format(user), headers, PendingTwitchAPIRequestMode.GET)
+
     if not json.get('data'):
         return {}
 
     return json['data'][0]
 
 
 async def get_user_id(user: str, headers: dict = None, verbose=True) -> int:
     # shortcut if the user's id was already requested
     if user in user_id_cache:
         return user_id_cache[user]
 
     headers = headers if headers is not None else get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_USER_DATA] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_USER_DATA] headers for the twitch api request are missing authorization', stacklevel=2)
         return -1
 
     data = await get_user_data(user, headers)
 
     if not data:
         if verbose:
-            warnings.warn(f'[GET_USER_ID] unable to get user_id for username "{user}"')
+            warnings.warn(f'[GET_USER_ID] unable to get user_id for username "{user}"', stacklevel=2)
         return -1
 
     user_id_cache[user] = data['id']
     return data['id']
 
 
 async def get_stream_data(user_id: str, headers: dict = None) -> dict:
     headers = headers if headers is not None else get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_STREAM_DATA] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_STREAM_DATA] headers for the twitch api request are missing authorization', stacklevel=2)
         return {}
 
     _, json = await get_url(STREAM_API_URL.format(user_id), headers)
 
     if not json.get('data'):
         return {}
 
     return json['data'][0]
 
 
 async def get_channel_chatters(channel: str, headers: dict = None) -> dict:
     headers = headers if headers is not None else get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_CHANNEL_CHATTERS] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_CHANNEL_CHATTERS] headers for the twitch api request are missing authorization', stacklevel=2)
         return {}
 
     _, data = await get_url(CHANNEL_CHATTERS_URL.format(channel))
     return data
 
 
 CLIENT_ID_KEY = 'Client-ID'
@@ -207,15 +315,15 @@
 
 
 async def get_channel_info(broadcaster_name_or_id: str, headers: dict = None) -> Optional[ChannelInfo]:
     from ..util import dict_get_value
 
     headers = headers if headers is not None else get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_CHANNEL_INFO] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_CHANNEL_INFO] headers for the twitch api request are missing authorization', stacklevel=2)
         return None
 
     if not broadcaster_name_or_id.strip().isnumeric():
         user_id = await get_user_id(broadcaster_name_or_id, headers=headers)
         if user_id == -1:
             return None
     else:
@@ -238,15 +346,15 @@
     user_id = user_id.strip()
 
     if user_id in _channel_id_to_name_cache:
         return _channel_id_to_name_cache[user_id]
 
     headers = headers if headers is not None else get_headers()
     if not _check_headers_has_auth(headers):
-        warnings.warn('[GET_CHANNEL_NAME_FROM_USER_ID] headers for the twitch api request are missing authorization')
+        warnings.warn('[GET_CHANNEL_NAME_FROM_USER_ID] headers for the twitch api request are missing authorization', stacklevel=2)
         return ''
 
     channel_info = await get_channel_info(user_id, headers=headers)
 
     if not channel_info:
         return ''
```

### Comparing `PythonTwitchBotFramework-2.8.1/twitchbot/util/typing_utils.py` & `PythonTwitchBotFramework-2.9.0/twitchbot/util/typing_utils.py`

 * *Files identical despite different names*

### Comparing `PythonTwitchBotFramework-2.8.1/util/command_console.py` & `PythonTwitchBotFramework-2.9.0/util/command_console.py`

 * *Files identical despite different names*

