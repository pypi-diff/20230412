# Comparing `tmp/discord-py-interactions-5.0.0.tar.gz` & `tmp/discord-py-interactions-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-py-interactions-5.0.0.tar", last modified: Mon Apr 10 11:44:03 2023, max compression
+gzip compressed data, was "discord-py-interactions-5.0.1.tar", last modified: Wed Apr 12 16:39:30 2023, max compression
```

## Comparing `discord-py-interactions-5.0.0.tar` & `discord-py-interactions-5.0.1.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.259178 discord-py-interactions-5.0.0/
--rw-rw-rw-   0        0        0    35823 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/LICENSE
--rw-rw-rw-   0        0        0      194 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4478 2023-04-10 11:44:03.259178 discord-py-interactions-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3150 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.139566 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/
--rw-rw-rw-   0        0        0     4478 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6418 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1169 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.141568 discord-py-interactions-5.0.0/interactions/
--rw-rw-rw-   0        0        0    15600 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.141568 discord-py-interactions-5.0.0/interactions/api/
--rw-rw-rw-   0        0        0       47 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.144570 discord-py-interactions-5.0.0/interactions/api/events/
--rw-rw-rw-   0        0        0     3921 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/__init__.py
--rw-rw-rw-   0        0        0     2844 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/base.py
--rw-rw-rw-   0        0        0    24582 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/discord.py
--rw-rw-rw-   0        0        0     8542 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/internal.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.156581 discord-py-interactions-5.0.0/interactions/api/events/processors/
--rw-rw-rw-   0        0        0      811 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/__init__.py
--rw-rw-rw-   0        0        0     1626 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/_template.py
--rw-rw-rw-   0        0        0      459 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/_template.pyi
--rw-rw-rw-   0        0        0     1590 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/auto_mod.py
--rw-rw-rw-   0        0        0     2135 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/channel_events.py
--rw-rw-rw-   0        0        0     4943 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/guild_events.py
--rw-rw-rw-   0        0        0     1337 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/integrations.py
--rw-rw-rw-   0        0        0     1532 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/member_events.py
--rw-rw-rw-   0        0        0     2878 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/message_events.py
--rw-rw-rw-   0        0        0     3303 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/reaction_events.py
--rw-rw-rw-   0        0        0     1776 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/role_events.py
--rw-rw-rw-   0        0        0      998 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/stage_events.py
--rw-rw-rw-   0        0        0     2335 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/thread_events.py
--rw-rw-rw-   0        0        0     2155 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/user_events.py
--rw-rw-rw-   0        0        0     2002 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/voice_events.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.160585 discord-py-interactions-5.0.0/interactions/api/gateway/
--rw-rw-rw-   0        0        0       78 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/gateway/__init__.py
--rw-rw-rw-   0        0        0    13930 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/gateway/gateway.py
--rw-rw-rw-   0        0        0     8445 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/gateway/state.py
--rw-rw-rw-   0        0        0    11904 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/gateway/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.162587 discord-py-interactions-5.0.0/interactions/api/http/
--rw-rw-rw-   0        0        0        0 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/__init__.py
--rw-rw-rw-   0        0        0    19920 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_client.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.172597 discord-py-interactions-5.0.0/interactions/api/http/http_requests/
--rw-rw-rw-   0        0        0      835 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/bot.py
--rw-rw-rw-   0        0        0    22688 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/channels.py
--rw-rw-rw-   0        0        0     3188 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/emojis.py
--rw-rw-rw-   0        0        0    35035 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/guild.py
--rw-rw-rw-   0        0        0    10705 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/interactions.py
--rw-rw-rw-   0        0        0     6739 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/members.py
--rw-rw-rw-   0        0        0     5200 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/messages.py
--rw-rw-rw-   0        0        0     4930 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/reactions.py
--rw-rw-rw-   0        0        0     5061 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/scheduled_events.py
--rw-rw-rw-   0        0        0     4202 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/stickers.py
--rw-rw-rw-   0        0        0     8434 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/threads.py
--rw-rw-rw-   0        0        0     4307 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/users.py
--rw-rw-rw-   0        0        0     6995 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/webhooks.py
--rw-rw-rw-   0        0        0     2176 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/route.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.178602 discord-py-interactions-5.0.0/interactions/api/voice/
--rw-rw-rw-   0        0        0        0 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/__init__.py
--rw-rw-rw-   0        0        0    12295 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/audio.py
--rw-rw-rw-   0        0        0     9276 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/audio_writer.py
--rw-rw-rw-   0        0        0     3754 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/encryption.py
--rw-rw-rw-   0        0        0    11836 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/opus.py
--rw-rw-rw-   0        0        0     5596 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/player.py
--rw-rw-rw-   0        0        0     8005 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/recorder.py
--rw-rw-rw-   0        0        0    15611 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/voice_gateway.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.183108 discord-py-interactions-5.0.0/interactions/client/
--rw-rw-rw-   0        0        0     1771 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/__init__.py
--rw-rw-rw-   0        0        0     9799 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/auto_shard_client.py
--rw-rw-rw-   0        0        0    87510 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/client.py
--rw-rw-rw-   0        0        0     6562 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/const.py
--rw-rw-rw-   0        0        0    13632 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.188113 discord-py-interactions-5.0.0/interactions/client/mixins/
--rw-rw-rw-   0        0        0      118 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/mixins/__init__.py
--rw-rw-rw-   0        0        0      891 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/mixins/modal.py
--rw-rw-rw-   0        0        0     4313 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/mixins/send.py
--rw-rw-rw-   0        0        0     3746 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/mixins/serialization.py
--rw-rw-rw-   0        0        0    31016 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/smart_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.196120 discord-py-interactions-5.0.0/interactions/client/utils/
--rw-rw-rw-   0        0        0     2159 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/__init__.py
--rw-rw-rw-   0        0        0     2436 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/attr_converters.py
--rw-rw-rw-   0        0        0     2285 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/attr_utils.py
--rw-rw-rw-   0        0        0     1210 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/attr_utils.pyi
--rw-rw-rw-   0        0        0     4806 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/cache.py
--rw-rw-rw-   0        0        0     3632 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/deserialise_app_cmds.py
--rw-rw-rw-   0        0        0     3189 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/formatting.py
--rw-rw-rw-   0        0        0     3642 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/input_utils.py
--rw-rw-rw-   0        0        0     7524 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/misc_utils.py
--rw-rw-rw-   0        0        0     4688 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/serializer.py
--rw-rw-rw-   0        0        0     1079 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/text_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.199123 discord-py-interactions-5.0.0/interactions/ext/
--rw-rw-rw-   0        0        0        0 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/__init__.py
--rw-rw-rw-   0        0        0     1883 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/console.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.203127 discord-py-interactions-5.0.0/interactions/ext/debug_extension/
--rw-rw-rw-   0        0        0     3300 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/__init__.py
--rw-rw-rw-   0        0        0     5112 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_application_cmd.py
--rw-rw-rw-   0        0        0     4646 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_exec.py
--rw-rw-rw-   0        0        0     1418 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_exts.py
--rw-rw-rw-   0        0        0     6234 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/utils.py
--rw-rw-rw-   0        0        0     8196 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/jurigged.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.204128 discord-py-interactions-5.0.0/interactions/ext/mypy/
--rw-rw-rw-   0        0        0     1085 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/mypy/__init__.py
--rw-rw-rw-   0        0        0    16283 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/paginators.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.208131 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/
--rw-rw-rw-   0        0        0      554 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/__init__.py
--rw-rw-rw-   0        0        0    28658 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/command.py
--rw-rw-rw-   0        0        0     3516 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/context.py
--rw-rw-rw-   0        0        0     7778 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/help.py
--rw-rw-rw-   0        0        0    14481 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/manager.py
--rw-rw-rw-   0        0        0     1205 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/utils.py
--rw-rw-rw-   0        0        0     3661 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/sentry.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.209132 discord-py-interactions-5.0.0/interactions/models/
--rw-rw-rw-   0        0        0    12743 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.235156 discord-py-interactions-5.0.0/interactions/models/discord/
--rw-rw-rw-   0        0        0     8257 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/__init__.py
--rw-rw-rw-   0        0        0     5628 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/activity.py
--rw-rw-rw-   0        0        0     3105 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/app_perms.py
--rw-rw-rw-   0        0        0     4829 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/application.py
--rw-rw-rw-   0        0        0     3939 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/asset.py
--rw-rw-rw-   0        0        0    12872 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/auto_mod.py
--rw-rw-rw-   0        0        0     1779 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/base.py
--rw-rw-rw-   0        0        0   104561 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/channel.py
--rw-rw-rw-   0        0        0     8310 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/color.py
--rw-rw-rw-   0        0        0    25482 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/components.py
--rw-rw-rw-   0        0        0    16775 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/embed.py
--rw-rw-rw-   0        0        0     9326 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/emoji.py
--rw-rw-rw-   0        0        0    29369 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/enums.py
--rw-rw-rw-   0        0        0     2323 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/file.py
--rw-rw-rw-   0        0        0    96518 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/guild.py
--rw-rw-rw-   0        0        0     6212 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/invite.py
--rw-rw-rw-   0        0        0    38197 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/message.py
--rw-rw-rw-   0        0        0     5139 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/modal.py
--rw-rw-rw-   0        0        0     3609 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/reaction.py
--rw-rw-rw-   0        0        0     8309 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/role.py
--rw-rw-rw-   0        0        0     9570 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/scheduled_event.py
--rw-rw-rw-   0        0        0     5353 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/snowflake.py
--rw-rw-rw-   0        0        0     1479 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/stage_instance.py
--rw-rw-rw-   0        0        0     5378 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/sticker.py
--rw-rw-rw-   0        0        0     2871 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/team.py
--rw-rw-rw-   0        0        0     5828 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/thread.py
--rw-rw-rw-   0        0        0     4429 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/timestamp.py
--rw-rw-rw-   0        0        0    25473 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/user.py
--rw-rw-rw-   0        0        0     6891 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/user.pyi
--rw-rw-rw-   0        0        0     4971 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/voice_state.py
--rw-rw-rw-   0        0        0    12721 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/webhooks.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.246166 discord-py-interactions-5.0.0/interactions/models/internal/
--rw-rw-rw-   0        0        0     4981 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/__init__.py
--rw-rw-rw-   0        0        0    11584 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/active_voice_state.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.247167 discord-py-interactions-5.0.0/interactions/models/internal/annotations/
--rw-rw-rw-   0        0        0      523 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/annotations/__init__.py
--rw-rw-rw-   0        0        0     7673 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/annotations/slash.py
--rw-rw-rw-   0        0        0    56500 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/application_commands.py
--rw-rw-rw-   0        0        0     1470 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/auto_defer.py
--rw-rw-rw-   0        0        0     1238 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/callback.py
--rw-rw-rw-   0        0        0     2485 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/checks.py
--rw-rw-rw-   0        0        0    12548 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/command.py
--rw-rw-rw-   0        0        0    35380 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/context.py
--rw-rw-rw-   0        0        0    19957 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/converters.py
--rw-rw-rw-   0        0        0     8652 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/cooldowns.py
--rw-rw-rw-   0        0        0    10438 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/extension.py
--rw-rw-rw-   0        0        0     4671 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/listener.py
--rw-rw-rw-   0        0        0     6168 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/localisation.py
--rw-rw-rw-   0        0        0     1405 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/protocols.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.250170 discord-py-interactions-5.0.0/interactions/models/internal/tasks/
--rw-rw-rw-   0        0        0      212 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/tasks/__init__.py
--rw-rw-rw-   0        0        0     5295 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/tasks/task.py
--rw-rw-rw-   0        0        0     4194 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/tasks/triggers.py
--rw-rw-rw-   0        0        0     1228 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/wait.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.252171 discord-py-interactions-5.0.0/interactions/models/misc/
--rw-rw-rw-   0        0        0      115 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/misc/__init__.py
--rw-rw-rw-   0        0        0      996 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/misc/context_manager.py
--rw-rw-rw-   0        0        0     3216 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/misc/iterator.py
--rw-rw-rw-   0        0        0        0 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/interactions/py.typed
--rw-rw-rw-   0        0        0     5833 2023-04-10 11:43:08.000000 discord-py-interactions-5.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       71 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/requirements-docs.txt
--rw-rw-rw-   0        0        0       34 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/requirements-lint.txt
--rw-rw-rw-   0        0        0       54 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/requirements.txt
--rw-rw-rw-   0        0        0      456 2023-04-10 11:44:03.260178 discord-py-interactions-5.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2483 2023-04-10 11:42:49.000000 discord-py-interactions-5.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.258177 discord-py-interactions-5.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     4500 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/consts.py
--rw-rw-rw-   0        0        0    17477 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_bot.py
--rw-rw-rw-   0        0        0     1956 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_cache.py
--rw-rw-rw-   0        0        0     2056 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_contexts.py
--rw-rw-rw-   0        0        0     2278 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_cooldowns.py
--rw-rw-rw-   0        0        0     3907 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_emoji.py
--rw-rw-rw-   0        0        0     1081 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.579614 discord-py-interactions-5.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 16:34:04.000000 discord-py-interactions-5.0.1/LICENSE
+-rw-rw-rw-   0        0        0      167 2023-04-12 16:34:38.000000 discord-py-interactions-5.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4478 2023-04-12 16:39:30.580615 discord-py-interactions-5.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3150 2023-04-12 08:27:21.000000 discord-py-interactions-5.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.452996 discord-py-interactions-5.0.1/discord_py_interactions.egg-info/
+-rw-rw-rw-   0        0        0     4478 2023-04-12 16:39:30.000000 discord-py-interactions-5.0.1/discord_py_interactions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6434 2023-04-12 16:39:30.000000 discord-py-interactions-5.0.1/discord_py_interactions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 16:39:30.000000 discord-py-interactions-5.0.1/discord_py_interactions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1169 2023-04-12 16:39:30.000000 discord-py-interactions-5.0.1/discord_py_interactions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-12 16:39:30.000000 discord-py-interactions-5.0.1/discord_py_interactions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.454998 discord-py-interactions-5.0.1/interactions/
+-rw-rw-rw-   0        0        0    15600 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/interactions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.455999 discord-py-interactions-5.0.1/interactions/api/
+-rw-rw-rw-   0        0        0       47 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.459002 discord-py-interactions-5.0.1/interactions/api/events/
+-rw-rw-rw-   0        0        0     3921 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/__init__.py
+-rw-rw-rw-   0        0        0     2844 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/base.py
+-rw-rw-rw-   0        0        0    24582 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/discord.py
+-rw-rw-rw-   0        0        0     8542 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/internal.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.471013 discord-py-interactions-5.0.1/interactions/api/events/processors/
+-rw-rw-rw-   0        0        0      811 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/__init__.py
+-rw-rw-rw-   0        0        0     1626 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/_template.py
+-rw-rw-rw-   0        0        0      459 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/_template.pyi
+-rw-rw-rw-   0        0        0     1590 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/auto_mod.py
+-rw-rw-rw-   0        0        0     2135 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/channel_events.py
+-rw-rw-rw-   0        0        0     4943 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/guild_events.py
+-rw-rw-rw-   0        0        0     1337 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/integrations.py
+-rw-rw-rw-   0        0        0     1532 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/member_events.py
+-rw-rw-rw-   0        0        0     2878 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/message_events.py
+-rw-rw-rw-   0        0        0     3303 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/reaction_events.py
+-rw-rw-rw-   0        0        0     1776 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/role_events.py
+-rw-rw-rw-   0        0        0      998 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/stage_events.py
+-rw-rw-rw-   0        0        0     2335 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/thread_events.py
+-rw-rw-rw-   0        0        0     2155 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/user_events.py
+-rw-rw-rw-   0        0        0     2002 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/events/processors/voice_events.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.474015 discord-py-interactions-5.0.1/interactions/api/gateway/
+-rw-rw-rw-   0        0        0       78 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/gateway/__init__.py
+-rw-rw-rw-   0        0        0    13930 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/interactions/api/gateway/gateway.py
+-rw-rw-rw-   0        0        0     8445 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/gateway/state.py
+-rw-rw-rw-   0        0        0    11904 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/interactions/api/gateway/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.476017 discord-py-interactions-5.0.1/interactions/api/http/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/__init__.py
+-rw-rw-rw-   0        0        0    19920 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_client.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.488029 discord-py-interactions-5.0.1/interactions/api/http/http_requests/
+-rw-rw-rw-   0        0        0      835 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/bot.py
+-rw-rw-rw-   0        0        0    22688 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/channels.py
+-rw-rw-rw-   0        0        0     3188 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/emojis.py
+-rw-rw-rw-   0        0        0    35035 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/guild.py
+-rw-rw-rw-   0        0        0    10705 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/interactions.py
+-rw-rw-rw-   0        0        0     6739 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/members.py
+-rw-rw-rw-   0        0        0     5200 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/messages.py
+-rw-rw-rw-   0        0        0     4930 2023-04-11 11:01:25.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/reactions.py
+-rw-rw-rw-   0        0        0     5061 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/scheduled_events.py
+-rw-rw-rw-   0        0        0     4202 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/stickers.py
+-rw-rw-rw-   0        0        0     8434 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/threads.py
+-rw-rw-rw-   0        0        0     4307 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/users.py
+-rw-rw-rw-   0        0        0     6995 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/http_requests/webhooks.py
+-rw-rw-rw-   0        0        0     2176 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/http/route.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.494035 discord-py-interactions-5.0.1/interactions/api/voice/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/voice/__init__.py
+-rw-rw-rw-   0        0        0    12295 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/voice/audio.py
+-rw-rw-rw-   0        0        0     9276 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/voice/audio_writer.py
+-rw-rw-rw-   0        0        0     3754 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/voice/encryption.py
+-rw-rw-rw-   0        0        0    11836 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/voice/opus.py
+-rw-rw-rw-   0        0        0     5596 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/voice/player.py
+-rw-rw-rw-   0        0        0     8005 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/voice/recorder.py
+-rw-rw-rw-   0        0        0    15611 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/api/voice/voice_gateway.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.496036 discord-py-interactions-5.0.1/interactions/bin/
+-rw-rw-rw-   0        0        0   441856 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/bin/opus-x64.dll
+-rw-rw-rw-   0        0        0   366080 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/bin/opus-x86.dll
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.501543 discord-py-interactions-5.0.1/interactions/client/
+-rw-rw-rw-   0        0        0     1771 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/__init__.py
+-rw-rw-rw-   0        0        0     9799 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/auto_shard_client.py
+-rw-rw-rw-   0        0        0    87510 2023-04-12 16:34:04.000000 discord-py-interactions-5.0.1/interactions/client/client.py
+-rw-rw-rw-   0        0        0     6562 2023-04-12 16:34:04.000000 discord-py-interactions-5.0.1/interactions/client/const.py
+-rw-rw-rw-   0        0        0    13632 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/interactions/client/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.504546 discord-py-interactions-5.0.1/interactions/client/mixins/
+-rw-rw-rw-   0        0        0      118 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/mixins/__init__.py
+-rw-rw-rw-   0        0        0      891 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/mixins/modal.py
+-rw-rw-rw-   0        0        0     4313 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/mixins/send.py
+-rw-rw-rw-   0        0        0     3746 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/mixins/serialization.py
+-rw-rw-rw-   0        0        0    31016 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/smart_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.512553 discord-py-interactions-5.0.1/interactions/client/utils/
+-rw-rw-rw-   0        0        0     2159 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/__init__.py
+-rw-rw-rw-   0        0        0     2436 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/attr_converters.py
+-rw-rw-rw-   0        0        0     2285 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/attr_utils.py
+-rw-rw-rw-   0        0        0     1210 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/attr_utils.pyi
+-rw-rw-rw-   0        0        0     4806 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/cache.py
+-rw-rw-rw-   0        0        0     3632 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/deserialise_app_cmds.py
+-rw-rw-rw-   0        0        0     3189 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/formatting.py
+-rw-rw-rw-   0        0        0     3642 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/input_utils.py
+-rw-rw-rw-   0        0        0     7524 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/misc_utils.py
+-rw-rw-rw-   0        0        0     4688 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/serializer.py
+-rw-rw-rw-   0        0        0     1079 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/client/utils/text_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.516557 discord-py-interactions-5.0.1/interactions/ext/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/__init__.py
+-rw-rw-rw-   0        0        0     1883 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/console.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.521561 discord-py-interactions-5.0.1/interactions/ext/debug_extension/
+-rw-rw-rw-   0        0        0     3300 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/debug_extension/__init__.py
+-rw-rw-rw-   0        0        0     5112 2023-04-12 08:27:21.000000 discord-py-interactions-5.0.1/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-rw-rw-   0        0        0     4646 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/debug_extension/debug_exec.py
+-rw-rw-rw-   0        0        0     1418 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/debug_extension/debug_exts.py
+-rw-rw-rw-   0        0        0     6234 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/debug_extension/utils.py
+-rw-rw-rw-   0        0        0     8196 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/jurigged.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.521561 discord-py-interactions-5.0.1/interactions/ext/mypy/
+-rw-rw-rw-   0        0        0     1085 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/mypy/__init__.py
+-rw-rw-rw-   0        0        0    16283 2023-04-12 07:41:04.000000 discord-py-interactions-5.0.1/interactions/ext/paginators.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.527567 discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/
+-rw-rw-rw-   0        0        0      554 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/__init__.py
+-rw-rw-rw-   0        0        0    28658 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/command.py
+-rw-rw-rw-   0        0        0     3516 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/context.py
+-rw-rw-rw-   0        0        0     7778 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/help.py
+-rw-rw-rw-   0        0        0    14481 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/manager.py
+-rw-rw-rw-   0        0        0     1205 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/utils.py
+-rw-rw-rw-   0        0        0     3661 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/ext/sentry.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.528568 discord-py-interactions-5.0.1/interactions/models/
+-rw-rw-rw-   0        0        0    12743 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/interactions/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.553590 discord-py-interactions-5.0.1/interactions/models/discord/
+-rw-rw-rw-   0        0        0     8257 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/__init__.py
+-rw-rw-rw-   0        0        0     5628 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/activity.py
+-rw-rw-rw-   0        0        0     3105 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/app_perms.py
+-rw-rw-rw-   0        0        0     4829 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/application.py
+-rw-rw-rw-   0        0        0     3939 2023-04-12 16:34:04.000000 discord-py-interactions-5.0.1/interactions/models/discord/asset.py
+-rw-rw-rw-   0        0        0    12872 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/auto_mod.py
+-rw-rw-rw-   0        0        0     1779 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/base.py
+-rw-rw-rw-   0        0        0   104561 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/channel.py
+-rw-rw-rw-   0        0        0     8310 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/color.py
+-rw-rw-rw-   0        0        0    25482 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/components.py
+-rw-rw-rw-   0        0        0    16775 2023-04-12 16:38:08.000000 discord-py-interactions-5.0.1/interactions/models/discord/embed.py
+-rw-rw-rw-   0        0        0     9326 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/emoji.py
+-rw-rw-rw-   0        0        0    29369 2023-04-12 16:34:04.000000 discord-py-interactions-5.0.1/interactions/models/discord/enums.py
+-rw-rw-rw-   0        0        0     2323 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/file.py
+-rw-rw-rw-   0        0        0    96518 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/guild.py
+-rw-rw-rw-   0        0        0     6212 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/invite.py
+-rw-rw-rw-   0        0        0    38197 2023-04-11 11:01:25.000000 discord-py-interactions-5.0.1/interactions/models/discord/message.py
+-rw-rw-rw-   0        0        0     5139 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/modal.py
+-rw-rw-rw-   0        0        0     3609 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/reaction.py
+-rw-rw-rw-   0        0        0     8309 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/role.py
+-rw-rw-rw-   0        0        0     9570 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0     5353 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/snowflake.py
+-rw-rw-rw-   0        0        0     1479 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/stage_instance.py
+-rw-rw-rw-   0        0        0     5378 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/sticker.py
+-rw-rw-rw-   0        0        0     2871 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/team.py
+-rw-rw-rw-   0        0        0     5828 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/thread.py
+-rw-rw-rw-   0        0        0     4429 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/timestamp.py
+-rw-rw-rw-   0        0        0    25473 2023-04-12 16:34:04.000000 discord-py-interactions-5.0.1/interactions/models/discord/user.py
+-rw-rw-rw-   0        0        0     6891 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/user.pyi
+-rw-rw-rw-   0        0        0     4971 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/voice_state.py
+-rw-rw-rw-   0        0        0    12721 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/discord/webhooks.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.566603 discord-py-interactions-5.0.1/interactions/models/internal/
+-rw-rw-rw-   0        0        0     4981 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/interactions/models/internal/__init__.py
+-rw-rw-rw-   0        0        0    11584 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/active_voice_state.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.567603 discord-py-interactions-5.0.1/interactions/models/internal/annotations/
+-rw-rw-rw-   0        0        0      523 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/annotations/__init__.py
+-rw-rw-rw-   0        0        0     7673 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/annotations/slash.py
+-rw-rw-rw-   0        0        0    56514 2023-04-12 16:34:16.000000 discord-py-interactions-5.0.1/interactions/models/internal/application_commands.py
+-rw-rw-rw-   0        0        0     1470 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/auto_defer.py
+-rw-rw-rw-   0        0        0     1238 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/callback.py
+-rw-rw-rw-   0        0        0     2485 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/checks.py
+-rw-rw-rw-   0        0        0    12548 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/interactions/models/internal/command.py
+-rw-rw-rw-   0        0        0    35380 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/context.py
+-rw-rw-rw-   0        0        0    19957 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/converters.py
+-rw-rw-rw-   0        0        0     8652 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/interactions/models/internal/cooldowns.py
+-rw-rw-rw-   0        0        0    10438 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/extension.py
+-rw-rw-rw-   0        0        0     4671 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/listener.py
+-rw-rw-rw-   0        0        0     6168 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/localisation.py
+-rw-rw-rw-   0        0        0     1405 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/protocols.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.570606 discord-py-interactions-5.0.1/interactions/models/internal/tasks/
+-rw-rw-rw-   0        0        0      212 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5295 2023-04-11 11:01:25.000000 discord-py-interactions-5.0.1/interactions/models/internal/tasks/task.py
+-rw-rw-rw-   0        0        0     4194 2023-04-11 11:01:25.000000 discord-py-interactions-5.0.1/interactions/models/internal/tasks/triggers.py
+-rw-rw-rw-   0        0        0     1228 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/internal/wait.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.572607 discord-py-interactions-5.0.1/interactions/models/misc/
+-rw-rw-rw-   0        0        0      115 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/misc/__init__.py
+-rw-rw-rw-   0        0        0      996 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/misc/context_manager.py
+-rw-rw-rw-   0        0        0     3216 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/interactions/models/misc/iterator.py
+-rw-rw-rw-   0        0        0        0 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.1/interactions/py.typed
+-rw-rw-rw-   0        0        0     5833 2023-04-12 16:39:29.000000 discord-py-interactions-5.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       54 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/requirements.txt
+-rw-rw-rw-   0        0        0      456 2023-04-12 16:39:30.581616 discord-py-interactions-5.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2483 2023-04-12 16:34:04.000000 discord-py-interactions-5.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:39:30.579614 discord-py-interactions-5.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     4500 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/tests/consts.py
+-rw-rw-rw-   0        0        0    17477 2023-04-12 16:34:04.000000 discord-py-interactions-5.0.1/tests/test_bot.py
+-rw-rw-rw-   0        0        0     1956 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/tests/test_cache.py
+-rw-rw-rw-   0        0        0     2056 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/tests/test_contexts.py
+-rw-rw-rw-   0        0        0     2278 2023-04-12 09:19:48.000000 discord-py-interactions-5.0.1/tests/test_cooldowns.py
+-rw-rw-rw-   0        0        0     3907 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/tests/test_emoji.py
+-rw-rw-rw-   0        0        0     1081 2023-04-11 10:58:23.000000 discord-py-interactions-5.0.1/tests/utils.py
```

### Comparing `discord-py-interactions-5.0.0/LICENSE` & `discord-py-interactions-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/PKG-INFO` & `discord-py-interactions-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.0.0
+Version: 5.0.1
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.0.0/README.md` & `discord-py-interactions-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/discord_py_interactions.egg-info/PKG-INFO` & `discord-py-interactions-5.0.1/discord_py_interactions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.0.0
+Version: 5.0.1
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.0.0/discord_py_interactions.egg-info/SOURCES.txt` & `discord-py-interactions-5.0.1/discord_py_interactions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements-docs.txt
-requirements-lint.txt
 requirements.txt
 setup.cfg
 setup.py
 discord_py_interactions.egg-info/PKG-INFO
 discord_py_interactions.egg-info/SOURCES.txt
 discord_py_interactions.egg-info/dependency_links.txt
 discord_py_interactions.egg-info/requires.txt
@@ -59,14 +57,16 @@
 interactions/api/voice/audio.py
 interactions/api/voice/audio_writer.py
 interactions/api/voice/encryption.py
 interactions/api/voice/opus.py
 interactions/api/voice/player.py
 interactions/api/voice/recorder.py
 interactions/api/voice/voice_gateway.py
+interactions/bin/opus-x64.dll
+interactions/bin/opus-x86.dll
 interactions/client/__init__.py
 interactions/client/auto_shard_client.py
 interactions/client/client.py
 interactions/client/const.py
 interactions/client/errors.py
 interactions/client/smart_cache.py
 interactions/client/mixins/__init__.py
```

### Comparing `discord-py-interactions-5.0.0/discord_py_interactions.egg-info/requires.txt` & `discord-py-interactions-5.0.1/discord_py_interactions.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/__init__.py` & `discord-py-interactions-5.0.1/interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/__init__.py` & `discord-py-interactions-5.0.1/interactions/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/base.py` & `discord-py-interactions-5.0.1/interactions/api/events/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/discord.py` & `discord-py-interactions-5.0.1/interactions/api/events/discord.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/internal.py` & `discord-py-interactions-5.0.1/interactions/api/events/internal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/__init__.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/_template.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/auto_mod.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/auto_mod.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/channel_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/guild_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/integrations.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/member_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/message_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/reaction_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/reaction_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/role_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/stage_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/thread_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/thread_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/user_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/events/processors/voice_events.py` & `discord-py-interactions-5.0.1/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/gateway/gateway.py` & `discord-py-interactions-5.0.1/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/gateway/state.py` & `discord-py-interactions-5.0.1/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/gateway/websocket.py` & `discord-py-interactions-5.0.1/interactions/api/gateway/websocket.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_client.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/__init__.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/bot.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/channels.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/channels.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/emojis.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/guild.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/guild.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/interactions.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/members.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/messages.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/reactions.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/scheduled_events.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/stickers.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/threads.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/threads.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/users.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/users.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/http_requests/webhooks.py` & `discord-py-interactions-5.0.1/interactions/api/http/http_requests/webhooks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/http/route.py` & `discord-py-interactions-5.0.1/interactions/api/http/route.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/voice/audio.py` & `discord-py-interactions-5.0.1/interactions/api/voice/audio.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/voice/audio_writer.py` & `discord-py-interactions-5.0.1/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/voice/encryption.py` & `discord-py-interactions-5.0.1/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/voice/opus.py` & `discord-py-interactions-5.0.1/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/voice/player.py` & `discord-py-interactions-5.0.1/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/voice/recorder.py` & `discord-py-interactions-5.0.1/interactions/api/voice/recorder.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/api/voice/voice_gateway.py` & `discord-py-interactions-5.0.1/interactions/api/voice/voice_gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/__init__.py` & `discord-py-interactions-5.0.1/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/auto_shard_client.py` & `discord-py-interactions-5.0.1/interactions/client/auto_shard_client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/client.py` & `discord-py-interactions-5.0.1/interactions/client/client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/const.py` & `discord-py-interactions-5.0.1/interactions/client/const.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/errors.py` & `discord-py-interactions-5.0.1/interactions/client/errors.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/mixins/modal.py` & `discord-py-interactions-5.0.1/interactions/client/mixins/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/mixins/send.py` & `discord-py-interactions-5.0.1/interactions/client/mixins/send.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/mixins/serialization.py` & `discord-py-interactions-5.0.1/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/smart_cache.py` & `discord-py-interactions-5.0.1/interactions/client/smart_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/__init__.py` & `discord-py-interactions-5.0.1/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/attr_converters.py` & `discord-py-interactions-5.0.1/interactions/client/utils/attr_converters.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/attr_utils.py` & `discord-py-interactions-5.0.1/interactions/client/utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/attr_utils.pyi` & `discord-py-interactions-5.0.1/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/cache.py` & `discord-py-interactions-5.0.1/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/deserialise_app_cmds.py` & `discord-py-interactions-5.0.1/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/formatting.py` & `discord-py-interactions-5.0.1/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/input_utils.py` & `discord-py-interactions-5.0.1/interactions/client/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/misc_utils.py` & `discord-py-interactions-5.0.1/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/serializer.py` & `discord-py-interactions-5.0.1/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/client/utils/text_utils.py` & `discord-py-interactions-5.0.1/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/console.py` & `discord-py-interactions-5.0.1/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/debug_extension/__init__.py` & `discord-py-interactions-5.0.1/interactions/ext/debug_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_application_cmd.py` & `discord-py-interactions-5.0.1/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_exec.py` & `discord-py-interactions-5.0.1/interactions/ext/debug_extension/debug_exec.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_exts.py` & `discord-py-interactions-5.0.1/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/debug_extension/utils.py` & `discord-py-interactions-5.0.1/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/jurigged.py` & `discord-py-interactions-5.0.1/interactions/ext/jurigged.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/mypy/__init__.py` & `discord-py-interactions-5.0.1/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/paginators.py` & `discord-py-interactions-5.0.1/interactions/ext/paginators.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/__init__.py` & `discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/command.py` & `discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/context.py` & `discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/context.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/help.py` & `discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/manager.py` & `discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/utils.py` & `discord-py-interactions-5.0.1/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/ext/sentry.py` & `discord-py-interactions-5.0.1/interactions/ext/sentry.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/__init__.py` & `discord-py-interactions-5.0.1/interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/__init__.py` & `discord-py-interactions-5.0.1/interactions/models/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/activity.py` & `discord-py-interactions-5.0.1/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/app_perms.py` & `discord-py-interactions-5.0.1/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/application.py` & `discord-py-interactions-5.0.1/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/asset.py` & `discord-py-interactions-5.0.1/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/auto_mod.py` & `discord-py-interactions-5.0.1/interactions/models/discord/auto_mod.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/base.py` & `discord-py-interactions-5.0.1/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/channel.py` & `discord-py-interactions-5.0.1/interactions/models/discord/channel.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/color.py` & `discord-py-interactions-5.0.1/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/components.py` & `discord-py-interactions-5.0.1/interactions/models/discord/components.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/embed.py` & `discord-py-interactions-5.0.1/interactions/models/discord/embed.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/emoji.py` & `discord-py-interactions-5.0.1/interactions/models/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/enums.py` & `discord-py-interactions-5.0.1/interactions/models/discord/enums.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/file.py` & `discord-py-interactions-5.0.1/interactions/models/discord/file.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/guild.py` & `discord-py-interactions-5.0.1/interactions/models/discord/guild.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/invite.py` & `discord-py-interactions-5.0.1/interactions/models/discord/invite.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/message.py` & `discord-py-interactions-5.0.1/interactions/models/discord/message.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/modal.py` & `discord-py-interactions-5.0.1/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/reaction.py` & `discord-py-interactions-5.0.1/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/role.py` & `discord-py-interactions-5.0.1/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/scheduled_event.py` & `discord-py-interactions-5.0.1/interactions/models/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/snowflake.py` & `discord-py-interactions-5.0.1/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/stage_instance.py` & `discord-py-interactions-5.0.1/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/sticker.py` & `discord-py-interactions-5.0.1/interactions/models/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/team.py` & `discord-py-interactions-5.0.1/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/thread.py` & `discord-py-interactions-5.0.1/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/timestamp.py` & `discord-py-interactions-5.0.1/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/user.py` & `discord-py-interactions-5.0.1/interactions/models/discord/user.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/user.pyi` & `discord-py-interactions-5.0.1/interactions/models/discord/user.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/voice_state.py` & `discord-py-interactions-5.0.1/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/discord/webhooks.py` & `discord-py-interactions-5.0.1/interactions/models/discord/webhooks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/__init__.py` & `discord-py-interactions-5.0.1/interactions/models/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/active_voice_state.py` & `discord-py-interactions-5.0.1/interactions/models/internal/active_voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/annotations/__init__.py` & `discord-py-interactions-5.0.1/interactions/models/internal/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/annotations/slash.py` & `discord-py-interactions-5.0.1/interactions/models/internal/annotations/slash.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/application_commands.py` & `discord-py-interactions-5.0.1/interactions/models/internal/application_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -717,15 +717,15 @@
         return SlashCommand(
             name=self.name,
             description=self.description,
             group_name=name,
             group_description=description,
             scopes=self.scopes,
             dm_permission=self.dm_permission,
-            checks=self.checks if inherit_checks else [],
+            checks=self.checks.copy() if inherit_checks else [],
         )
 
     def subcommand(
         self,
         sub_cmd_name: Absent[LocalisedName | str] = MISSING,
         group_name: LocalisedName | str = None,
         sub_cmd_description: Absent[LocalisedDesc | str] = MISSING,
@@ -754,15 +754,15 @@
                 sub_cmd_description=sub_cmd_description,
                 default_member_permissions=self.default_member_permissions,
                 dm_permission=self.dm_permission,
                 options=options,
                 callback=call,
                 scopes=self.scopes,
                 nsfw=nsfw,
-                checks=self.checks if inherit_checks else [],
+                checks=self.checks.copy() if inherit_checks else [],
             )
 
         return wrapper
 
     async def call_callback(self, callback: typing.Callable, ctx: "InteractionContext") -> None:
         if not self.parameters:
             if self._uses_arg:
```

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/auto_defer.py` & `discord-py-interactions-5.0.1/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/callback.py` & `discord-py-interactions-5.0.1/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/checks.py` & `discord-py-interactions-5.0.1/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/command.py` & `discord-py-interactions-5.0.1/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/context.py` & `discord-py-interactions-5.0.1/interactions/models/internal/context.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/converters.py` & `discord-py-interactions-5.0.1/interactions/models/internal/converters.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/cooldowns.py` & `discord-py-interactions-5.0.1/interactions/models/internal/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/extension.py` & `discord-py-interactions-5.0.1/interactions/models/internal/extension.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/listener.py` & `discord-py-interactions-5.0.1/interactions/models/internal/listener.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/localisation.py` & `discord-py-interactions-5.0.1/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/protocols.py` & `discord-py-interactions-5.0.1/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/tasks/task.py` & `discord-py-interactions-5.0.1/interactions/models/internal/tasks/task.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/tasks/triggers.py` & `discord-py-interactions-5.0.1/interactions/models/internal/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/internal/wait.py` & `discord-py-interactions-5.0.1/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/misc/context_manager.py` & `discord-py-interactions-5.0.1/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/interactions/models/misc/iterator.py` & `discord-py-interactions-5.0.1/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/pyproject.toml` & `discord-py-interactions-5.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discord-py-interactions"
-version = "5.0.0"
+version = "5.0.1"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `discord-py-interactions-5.0.0/setup.py` & `discord-py-interactions-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/tests/consts.py` & `discord-py-interactions-5.0.1/tests/consts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/tests/test_bot.py` & `discord-py-interactions-5.0.1/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/tests/test_cache.py` & `discord-py-interactions-5.0.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/tests/test_contexts.py` & `discord-py-interactions-5.0.1/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/tests/test_cooldowns.py` & `discord-py-interactions-5.0.1/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/tests/test_emoji.py` & `discord-py-interactions-5.0.1/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.0.0/tests/utils.py` & `discord-py-interactions-5.0.1/tests/utils.py`

 * *Files identical despite different names*

