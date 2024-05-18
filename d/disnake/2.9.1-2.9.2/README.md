# Comparing `tmp/disnake-2.9.1.tar.gz` & `tmp/disnake-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disnake-2.9.1.tar", last modified: Mon Oct 30 20:22:13 2023, max compression
+gzip compressed data, was "disnake-2.9.2.tar", last modified: Sat May 18 12:52:55 2024, max compression
```

## Comparing `disnake-2.9.1.tar` & `disnake-2.9.2.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.175201 disnake-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-10-30 20:21:01.000000 disnake-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-10-30 20:21:01.000000 disnake-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2023-10-30 20:22:13.175201 disnake-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2023-10-30 20:21:01.000000 disnake-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.155200 disnake-2.9.1/disnake/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71323 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25789 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    36921 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    11361 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/appinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/application_role_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    31795 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28631 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/automod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/bans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.159200 disnake-2.9.1/disnake/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/bin/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)   441856 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/bin/libopus-0.x64.dll
--rw-r--r--   0 runner    (1001) docker     (127)   366080 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/bin/libopus-0.x86.dll
--rw-r--r--   0 runner    (1001) docker     (127)   159210 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    94112 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/colour.py
--rw-r--r--   0 runner    (1001) docker     (127)    22659 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/custom_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    28024 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)    44336 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    13422 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.143200 disnake-2.9.1/disnake/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.163200 disnake-2.9.1/disnake/ext/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    27590 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/base_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    21156 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/bot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    34441 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/cog.py
--rw-r--r--   0 runner    (1001) docker     (127)    23084 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/common_bot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    43768 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11885 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (127)    89205 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15025 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/ctx_menus_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/custom_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    31414 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    20527 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/flag_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    47682 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    54256 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/interaction_bot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    50306 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/params.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    31091 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/slash_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/commands/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.163200 disnake-2.9.1/disnake/ext/mypy_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/mypy_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.163200 disnake-2.9.1/disnake/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)    26807 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ext/tasks/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    75334 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    37894 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)   183827 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/guild_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)    25609 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/guild_scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    90490 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    13069 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)    12872 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.163200 disnake-2.9.1/disnake/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/interactions/application_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    71563 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/interactions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/interactions/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/interactions/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)    21666 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/invite.py
--rw-r--r--   0 runner    (1001) docker     (127)    36098 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    40694 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/mentions.py
--rw-r--r--   0 runner    (1001) docker     (127)    92464 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/oggparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/opus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/partial_emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)    45359 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26457 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/player.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/raw_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    17974 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    21116 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/shard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    90451 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    15314 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/sticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    40792 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.167200 disnake-2.9.1/disnake/types/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/appinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/application_role_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/audit_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/automod.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)    15913 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/guild_scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/interactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/invite.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/sticker.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/team.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/voice.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/welcome_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/types/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.171201 disnake-2.9.1/disnake/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29552 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/action_row.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.171201 disnake-2.9.1/disnake/ui/select/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/select/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/select/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/select/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/select/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/select/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/select/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/text_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    19534 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/ui/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    15669 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    38666 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/voice_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/voice_region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.171201 disnake-2.9.1/disnake/webhook/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/webhook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67023 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/webhook/async_.py
--rw-r--r--   0 runner    (1001) docker     (127)    43233 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/webhook/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/welcome_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)    13998 2023-10-30 20:21:01.000000 disnake-2.9.1/disnake/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.159200 disnake-2.9.1/disnake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2023-10-30 20:22:13.000000 disnake-2.9.1/disnake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-10-30 20:22:13.000000 disnake-2.9.1/disnake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 20:22:13.000000 disnake-2.9.1/disnake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-10-30 20:22:13.000000 disnake-2.9.1/disnake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-30 20:22:13.000000 disnake-2.9.1/disnake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2023-10-30 20:21:01.000000 disnake-2.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 20:22:13.175201 disnake-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-10-30 20:21:01.000000 disnake-2.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 20:22:13.171201 disnake-2.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_colour.py
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14421 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_mentions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_onboarding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25406 2023-10-30 20:21:01.000000 disnake-2.9.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.690123 disnake-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-18 12:52:05.000000 disnake-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-18 12:52:05.000000 disnake-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-18 12:52:55.690123 disnake-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-18 12:52:05.000000 disnake-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.666123 disnake-2.9.2/disnake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71452 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25789 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36921 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/appinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/application_role_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14980 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31795 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28631 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/automod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/bans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.670122 disnake-2.9.2/disnake/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/bin/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)   441856 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/bin/libopus-0.x64.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/bin/libopus-0.x86.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   159339 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94112 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/colour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22659 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/custom_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44336 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.650122 disnake-2.9.2/disnake/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.674123 disnake-2.9.2/disnake/ext/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27590 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/base_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21156 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/bot_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34441 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/cog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/common_bot_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43768 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11885 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89205 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/ctx_menus_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/custom_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20527 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/flag_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54256 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/interaction_bot_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50306 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    31091 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/slash_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/commands/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.674123 disnake-2.9.2/disnake/ext/mypy_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/mypy_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.674123 disnake-2.9.2/disnake/ext/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)    26807 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ext/tasks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75334 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38024 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)   183827 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/guild_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25609 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/guild_scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90490 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.674123 disnake-2.9.2/disnake/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/interactions/application_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71563 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/interactions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/interactions/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/interactions/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21666 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36098 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40694 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92464 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/oggparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/opus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/partial_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45359 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27028 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/raw_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17974 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21940 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/shard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90451 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40792 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.682123 disnake-2.9.2/disnake/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/appinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/application_role_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/automod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/guild_scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/welcome_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/types/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.682123 disnake-2.9.2/disnake/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29552 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/action_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.682123 disnake-2.9.2/disnake/ui/select/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/select/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/select/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/select/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/select/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/select/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/select/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/text_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/ui/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38666 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/voice_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/voice_region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.682123 disnake-2.9.2/disnake/webhook/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/webhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67074 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/webhook/async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43233 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/webhook/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/welcome_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13998 2024-05-18 12:52:05.000000 disnake-2.9.2/disnake/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.686123 disnake-2.9.2/disnake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-18 12:52:55.000000 disnake-2.9.2/disnake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-18 12:52:55.000000 disnake-2.9.2/disnake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:52:55.000000 disnake-2.9.2/disnake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-18 12:52:55.000000 disnake-2.9.2/disnake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 12:52:55.000000 disnake-2.9.2/disnake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-18 12:52:05.000000 disnake-2.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:52:55.690123 disnake-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-18 12:52:05.000000 disnake-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:52:55.686123 disnake-2.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_colour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14421 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25406 2024-05-18 12:52:05.000000 disnake-2.9.2/tests/test_utils.py
```

### Comparing `disnake-2.9.1/LICENSE` & `disnake-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/PKG-INFO` & `disnake-2.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disnake
-Version: 2.9.1
+Version: 2.9.2
 Summary: A Python wrapper for the Discord API
 Author: Disnake Development
 License: MIT
 Project-URL: Changelog, https://docs.disnake.dev/page/whats_new.html
 Project-URL: Documentation, https://docs.disnake.dev/
 Project-URL: Repository, https://github.com/DisnakeDev/disnake
 Keywords: disnake,discord,discord api
@@ -144,15 +144,15 @@
 @bot.command()
 async def ping(ctx):
     await ctx.send("Pong!")
 
 bot.run("BOT_TOKEN")
 ```
 
-You can find more examples in the [examples directory](./examples).
+You can find more examples in the [examples directory](https://github.com/DisnakeDev/disnake/tree/master/examples).
 
 <br>
 <p align="center">
     <a href="https://docs.disnake.dev/">Documentation</a>
     ⁕
     <a href="https://guide.disnake.dev/">Guide</a>
     ⁕
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disnake Version: 2.9.1 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: disnake Version: 2.9.2 Summary: A Python wrapper
 for the Discord API Author: Disnake Development License: MIT Project-URL:
 Changelog, https://docs.disnake.dev/page/whats_new.html Project-URL:
 Documentation, https://docs.disnake.dev/ Project-URL: Repository, https://
 github.com/DisnakeDev/disnake Keywords: disnake,discord,discord api Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
@@ -56,10 +56,11 @@
 disnake from disnake.ext import commands bot = commands.InteractionBot
 (test_guilds=[12345]) @bot.user_command() async def avatar(inter, user): embed
 = disnake.Embed(title=str(user)) embed.set_image(url=user.display_avatar.url)
 await inter.response.send_message(embed=embed) bot.run("BOT_TOKEN") ``` ###
 Prefix Commands Example ``` py import disnake from disnake.ext import commands
 bot = commands.Bot(command_prefix=commands.when_mentioned) @bot.command() async
 def ping(ctx): await ctx.send("Pong!") bot.run("BOT_TOKEN") ``` You can find
-more examples in the [examples directory](./examples).
+more examples in the [examples directory](https://github.com/DisnakeDev/
+disnake/tree/master/examples).
        _D_o_c_u_m_e_n_t_a_t_i_o_n â _G_u_i_d_e â _D_i_s_c_o_r_d_ _S_e_r_v_e_r â _D_i_s_c_o_r_d_ _D_e_v_e_l_o_p_e_r_s
```

### Comparing `disnake-2.9.1/README.md` & `disnake-2.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 @bot.command()
 async def ping(ctx):
     await ctx.send("Pong!")
 
 bot.run("BOT_TOKEN")
 ```
 
-You can find more examples in the [examples directory](./examples).
+You can find more examples in the [examples directory](https://github.com/DisnakeDev/disnake/tree/master/examples).
 
 <br>
 <p align="center">
     <a href="https://docs.disnake.dev/">Documentation</a>
     ⁕
     <a href="https://guide.disnake.dev/">Guide</a>
     ⁕
```

#### html2text {}

```diff
@@ -30,10 +30,11 @@
 disnake from disnake.ext import commands bot = commands.InteractionBot
 (test_guilds=[12345]) @bot.user_command() async def avatar(inter, user): embed
 = disnake.Embed(title=str(user)) embed.set_image(url=user.display_avatar.url)
 await inter.response.send_message(embed=embed) bot.run("BOT_TOKEN") ``` ###
 Prefix Commands Example ``` py import disnake from disnake.ext import commands
 bot = commands.Bot(command_prefix=commands.when_mentioned) @bot.command() async
 def ping(ctx): await ctx.send("Pong!") bot.run("BOT_TOKEN") ``` You can find
-more examples in the [examples directory](./examples).
+more examples in the [examples directory](https://github.com/DisnakeDev/
+disnake/tree/master/examples).
        _D_o_c_u_m_e_n_t_a_t_i_o_n â _G_u_i_d_e â _D_i_s_c_o_r_d_ _S_e_r_v_e_r â _D_i_s_c_o_r_d_ _D_e_v_e_l_o_p_e_r_s
```

### Comparing `disnake-2.9.1/disnake/__init__.py` & `disnake-2.9.2/disnake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 """
 
 __title__ = "disnake"
 __author__ = "Rapptz, EQUENOS"
 __license__ = "MIT"
 __copyright__ = "Copyright 2015-present Rapptz, 2021-present EQUENOS"
-__version__ = "2.9.1"
+__version__ = "2.9.2"
 
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
 import logging
 from typing import Literal, NamedTuple
 
 from . import abc as abc, opus as opus, ui as ui, utils as utils  # explicitly re-export modules
@@ -78,11 +78,11 @@
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
 # fmt: off
-version_info: VersionInfo = VersionInfo(major=2, minor=9, micro=1, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=2, minor=9, micro=2, releaselevel="final", serial=0)
 # fmt: on
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `disnake-2.9.1/disnake/__main__.py` & `disnake-2.9.2/disnake/__main__.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/abc.py` & `disnake-2.9.2/disnake/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from .flags import ChannelFlags, MessageFlags
 from .invite import Invite
 from .mentions import AllowedMentions
 from .object import Object
 from .partial_emoji import PartialEmoji
 from .permissions import PermissionOverwrite, Permissions
 from .role import Role
-from .sticker import GuildSticker, StickerItem
+from .sticker import GuildSticker, StandardSticker, StickerItem
 from .ui.action_row import components_to_dict
 from .utils import _overload_with_permissions
 from .voice_client import VoiceClient, VoiceProtocol
 
 __all__ = (
     "Snowflake",
     "User",
@@ -1423,15 +1423,15 @@
     async def send(
         self,
         content: Optional[str] = ...,
         *,
         tts: bool = ...,
         embed: Embed = ...,
         file: File = ...,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = ...,
         delete_after: float = ...,
         nonce: Union[str, int] = ...,
         suppress_embeds: bool = ...,
         flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         reference: Union[Message, MessageReference, PartialMessage] = ...,
         mention_author: bool = ...,
@@ -1444,15 +1444,15 @@
     async def send(
         self,
         content: Optional[str] = ...,
         *,
         tts: bool = ...,
         embed: Embed = ...,
         files: List[File] = ...,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = ...,
         delete_after: float = ...,
         nonce: Union[str, int] = ...,
         suppress_embeds: bool = ...,
         flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         reference: Union[Message, MessageReference, PartialMessage] = ...,
         mention_author: bool = ...,
@@ -1465,15 +1465,15 @@
     async def send(
         self,
         content: Optional[str] = ...,
         *,
         tts: bool = ...,
         embeds: List[Embed] = ...,
         file: File = ...,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = ...,
         delete_after: float = ...,
         nonce: Union[str, int] = ...,
         suppress_embeds: bool = ...,
         flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         reference: Union[Message, MessageReference, PartialMessage] = ...,
         mention_author: bool = ...,
@@ -1486,15 +1486,15 @@
     async def send(
         self,
         content: Optional[str] = ...,
         *,
         tts: bool = ...,
         embeds: List[Embed] = ...,
         files: List[File] = ...,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = ...,
         delete_after: float = ...,
         nonce: Union[str, int] = ...,
         suppress_embeds: bool = ...,
         flags: MessageFlags = ...,
         allowed_mentions: AllowedMentions = ...,
         reference: Union[Message, MessageReference, PartialMessage] = ...,
         mention_author: bool = ...,
@@ -1508,15 +1508,15 @@
         content: Optional[str] = None,
         *,
         tts: bool = False,
         embed: Optional[Embed] = None,
         embeds: Optional[List[Embed]] = None,
         file: Optional[File] = None,
         files: Optional[List[File]] = None,
-        stickers: Optional[Sequence[Union[GuildSticker, StickerItem]]] = None,
+        stickers: Optional[Sequence[Union[GuildSticker, StandardSticker, StickerItem]]] = None,
         delete_after: Optional[float] = None,
         nonce: Optional[Union[str, int]] = None,
         suppress_embeds: Optional[bool] = None,
         flags: Optional[MessageFlags] = None,
         allowed_mentions: Optional[AllowedMentions] = None,
         reference: Optional[Union[Message, MessageReference, PartialMessage]] = None,
         mention_author: Optional[bool] = None,
@@ -1561,15 +1561,15 @@
             .. versionadded:: 2.0
 
         file: :class:`.File`
             The file to upload. This cannot be mixed with the ``files`` parameter.
         files: List[:class:`.File`]
             A list of files to upload. Must be a maximum of 10.
             This cannot be mixed with the ``file`` parameter.
-        stickers: Sequence[Union[:class:`.GuildSticker`, :class:`.StickerItem`]]
+        stickers: Sequence[Union[:class:`.GuildSticker`, :class:`.StandardSticker`, :class:`.StickerItem`]]
             A list of stickers to upload. Must be a maximum of 3.
 
             .. versionadded:: 2.0
 
         nonce: Union[:class:`str`, :class:`int`]
             The nonce to use for sending this message. If the message was successfully sent,
             then the message will have a nonce with this value.
```

### Comparing `disnake-2.9.1/disnake/activity.py` & `disnake-2.9.2/disnake/activity.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/app_commands.py` & `disnake-2.9.2/disnake/app_commands.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/appinfo.py` & `disnake-2.9.2/disnake/appinfo.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/application_role_connection.py` & `disnake-2.9.2/disnake/application_role_connection.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/asset.py` & `disnake-2.9.2/disnake/asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,14 +191,17 @@
         "_url",
         "_animated",
         "_key",
     )
 
     BASE = "https://cdn.discordapp.com"
 
+    # only used in special cases where Discord doesn't provide an asset on the CDN url
+    BASE_MEDIA = "https://media.discordapp.net"
+
     def __init__(self, state: AnyState, *, url: str, key: str, animated: bool = False) -> None:
         self._state: AnyState = state
         self._url: str = url
         self._animated: bool = animated
         self._key: str = key
 
     @classmethod
```

### Comparing `disnake-2.9.1/disnake/audit_logs.py` & `disnake-2.9.2/disnake/audit_logs.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/automod.py` & `disnake-2.9.2/disnake/automod.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/backoff.py` & `disnake-2.9.2/disnake/backoff.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/bin/COPYING` & `disnake-2.9.2/disnake/bin/COPYING`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/bin/libopus-0.x64.dll` & `disnake-2.9.2/disnake/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/bin/libopus-0.x86.dll` & `disnake-2.9.2/disnake/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/channel.py` & `disnake-2.9.2/disnake/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     from .embeds import Embed
     from .emoji import Emoji
     from .guild import Guild, GuildChannel as GuildChannelType
     from .member import Member, VoiceState
     from .message import AllowedMentions, Message, PartialMessage
     from .role import Role
     from .state import ConnectionState
-    from .sticker import GuildSticker, StickerItem
+    from .sticker import GuildSticker, StandardSticker, StickerItem
     from .threads import AnyThreadArchiveDuration, ThreadType
     from .types.channel import (
         CategoryChannel as CategoryChannelPayload,
         DefaultReaction as DefaultReactionPayload,
         DMChannel as DMChannelPayload,
         ForumChannel as ForumChannelPayload,
         GroupDMChannel as GroupChannelPayload,
@@ -3765,15 +3765,15 @@
         slowmode_delay: Optional[int] = ...,
         applied_tags: Sequence[Snowflake] = ...,
         content: str = ...,
         embed: Embed = ...,
         file: File = ...,
         suppress_embeds: bool = ...,
         flags: MessageFlags = ...,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components = ...,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         ...
 
@@ -3786,15 +3786,15 @@
         slowmode_delay: Optional[int] = ...,
         applied_tags: Sequence[Snowflake] = ...,
         content: str = ...,
         embed: Embed = ...,
         files: List[File] = ...,
         suppress_embeds: bool = ...,
         flags: MessageFlags = ...,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components = ...,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         ...
 
@@ -3807,15 +3807,15 @@
         slowmode_delay: Optional[int] = ...,
         applied_tags: Sequence[Snowflake] = ...,
         content: str = ...,
         embeds: List[Embed] = ...,
         file: File = ...,
         suppress_embeds: bool = ...,
         flags: MessageFlags = ...,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components = ...,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         ...
 
@@ -3828,15 +3828,15 @@
         slowmode_delay: Optional[int] = ...,
         applied_tags: Sequence[Snowflake] = ...,
         content: str = ...,
         embeds: List[Embed] = ...,
         files: List[File] = ...,
         suppress_embeds: bool = ...,
         flags: MessageFlags = ...,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = ...,
         allowed_mentions: AllowedMentions = ...,
         view: View = ...,
         components: Components = ...,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         ...
 
@@ -3850,15 +3850,15 @@
         content: str = MISSING,
         embed: Embed = MISSING,
         embeds: List[Embed] = MISSING,
         file: File = MISSING,
         files: List[File] = MISSING,
         suppress_embeds: bool = MISSING,
         flags: MessageFlags = MISSING,
-        stickers: Sequence[Union[GuildSticker, StickerItem]] = MISSING,
+        stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = MISSING,
         allowed_mentions: AllowedMentions = MISSING,
         view: View = MISSING,
         components: Components[MessageUIComponent] = MISSING,
         reason: Optional[str] = None,
     ) -> ThreadWithMessage:
         """|coro|
 
@@ -3914,15 +3914,15 @@
             .. versionadded:: 2.9
 
         file: :class:`.File`
             The file to upload. This cannot be mixed with the ``files`` parameter.
         files: List[:class:`.File`]
             A list of files to upload. Must be a maximum of 10.
             This cannot be mixed with the ``file`` parameter.
-        stickers: Sequence[Union[:class:`.GuildSticker`, :class:`.StickerItem`]]
+        stickers: Sequence[Union[:class:`.GuildSticker`, :class:`.StandardSticker`, :class:`.StickerItem`]]
             A list of stickers to upload. Must be a maximum of 3.
         allowed_mentions: :class:`.AllowedMentions`
             Controls the mentions being processed in this message. If this is
             passed, then the object is merged with :attr:`.Client.allowed_mentions`.
             The merging behaviour only overrides attributes that have been explicitly passed
             to the object, otherwise it uses the attributes set in :attr:`.Client.allowed_mentions`.
             If no object is passed at all then the defaults given by :attr:`.Client.allowed_mentions`
```

### Comparing `disnake-2.9.1/disnake/client.py` & `disnake-2.9.2/disnake/client.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/colour.py` & `disnake-2.9.2/disnake/colour.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/components.py` & `disnake-2.9.2/disnake/components.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/context_managers.py` & `disnake-2.9.2/disnake/context_managers.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/custom_warnings.py` & `disnake-2.9.2/disnake/custom_warnings.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/embeds.py` & `disnake-2.9.2/disnake/embeds.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/emoji.py` & `disnake-2.9.2/disnake/emoji.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/enums.py` & `disnake-2.9.2/disnake/enums.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/errors.py` & `disnake-2.9.2/disnake/errors.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/__init__.py` & `disnake-2.9.2/disnake/ext/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/_types.py` & `disnake-2.9.2/disnake/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/base_core.py` & `disnake-2.9.2/disnake/ext/commands/base_core.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/bot.py` & `disnake-2.9.2/disnake/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/bot_base.py` & `disnake-2.9.2/disnake/ext/commands/bot_base.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/cog.py` & `disnake-2.9.2/disnake/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/common_bot_base.py` & `disnake-2.9.2/disnake/ext/commands/common_bot_base.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/context.py` & `disnake-2.9.2/disnake/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/converter.py` & `disnake-2.9.2/disnake/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/cooldowns.py` & `disnake-2.9.2/disnake/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/core.py` & `disnake-2.9.2/disnake/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/ctx_menus_core.py` & `disnake-2.9.2/disnake/ext/commands/ctx_menus_core.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/errors.py` & `disnake-2.9.2/disnake/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/flag_converter.py` & `disnake-2.9.2/disnake/ext/commands/flag_converter.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/flags.py` & `disnake-2.9.2/disnake/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/help.py` & `disnake-2.9.2/disnake/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/interaction_bot_base.py` & `disnake-2.9.2/disnake/ext/commands/interaction_bot_base.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/params.py` & `disnake-2.9.2/disnake/ext/commands/params.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/slash_core.py` & `disnake-2.9.2/disnake/ext/commands/slash_core.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/commands/view.py` & `disnake-2.9.2/disnake/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ext/tasks/__init__.py` & `disnake-2.9.2/disnake/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/file.py` & `disnake-2.9.2/disnake/file.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/flags.py` & `disnake-2.9.2/disnake/flags.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/gateway.py` & `disnake-2.9.2/disnake/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,15 +702,16 @@
             msg = await self.socket.receive(timeout=self._max_heartbeat_timeout)
             if msg.type is aiohttp.WSMsgType.TEXT:
                 await self.received_message(msg.data)
             elif msg.type is aiohttp.WSMsgType.BINARY:
                 await self.received_message(msg.data)
             elif msg.type is aiohttp.WSMsgType.ERROR:
                 _log.debug("Received %s", msg)
-                raise msg.data
+                # This is usually just an intermittent gateway hiccup, so try to reconnect again and resume
+                raise WebSocketClosure from msg.data
             elif msg.type in (
                 aiohttp.WSMsgType.CLOSED,
                 aiohttp.WSMsgType.CLOSING,
                 aiohttp.WSMsgType.CLOSE,
             ):
                 _log.debug("Received %s", msg)
                 raise WebSocketClosure
```

### Comparing `disnake-2.9.1/disnake/guild.py` & `disnake-2.9.2/disnake/guild.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/guild_preview.py` & `disnake-2.9.2/disnake/guild_preview.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/guild_scheduled_event.py` & `disnake-2.9.2/disnake/guild_scheduled_event.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/http.py` & `disnake-2.9.2/disnake/http.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/i18n.py` & `disnake-2.9.2/disnake/i18n.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,23 +232,28 @@
         ins._data = self._data
         return ins
 
     @property
     def data(self) -> Optional[Dict[str, str]]:
         """Optional[Dict[:class:`str`, :class:`str`]]: A dict with a locale -> localization mapping, if available."""
         if self._data is MISSING:
+            # This will happen when `_link(store)` hasn't been called yet, which *shouldn't* occur under normal circumstances.
             warnings.warn(
-                "value was never localized, this is likely a library bug",
+                f"Localization value ('{self._key}') was never linked to bot; this may be a library bug.",
                 LocalizationWarning,
                 stacklevel=2,
             )
             return None
         return self._data
 
     def __eq__(self, other) -> bool:
+        # if both are pending, compare keys instead
+        if self._data is MISSING and other._data is MISSING:
+            return self._key == other._key
+
         d1 = self.data
         d2 = other.data
         # consider values equal if they're both falsy, or actually equal
         # (it doesn't matter if localizations are `None` or `{}`)
         return (not d1 and not d2) or d1 == d2
```

### Comparing `disnake-2.9.1/disnake/integrations.py` & `disnake-2.9.2/disnake/integrations.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/interactions/application_command.py` & `disnake-2.9.2/disnake/interactions/application_command.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/interactions/base.py` & `disnake-2.9.2/disnake/interactions/base.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/interactions/message.py` & `disnake-2.9.2/disnake/interactions/message.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/interactions/modal.py` & `disnake-2.9.2/disnake/interactions/modal.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/invite.py` & `disnake-2.9.2/disnake/invite.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/iterators.py` & `disnake-2.9.2/disnake/iterators.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/member.py` & `disnake-2.9.2/disnake/member.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/mentions.py` & `disnake-2.9.2/disnake/mentions.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/message.py` & `disnake-2.9.2/disnake/message.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/mixins.py` & `disnake-2.9.2/disnake/mixins.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/object.py` & `disnake-2.9.2/disnake/object.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/oggparse.py` & `disnake-2.9.2/disnake/oggparse.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/onboarding.py` & `disnake-2.9.2/disnake/onboarding.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/opus.py` & `disnake-2.9.2/disnake/opus.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/partial_emoji.py` & `disnake-2.9.2/disnake/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/permissions.py` & `disnake-2.9.2/disnake/permissions.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/player.py` & `disnake-2.9.2/disnake/player.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,14 +122,20 @@
 class FFmpegAudio(AudioSource):
     """Represents an FFmpeg (or AVConv) based AudioSource.
 
     User created AudioSources using FFmpeg differently from how :class:`FFmpegPCMAudio` and
     :class:`FFmpegOpusAudio` work should subclass this.
 
     .. versionadded:: 1.3
+
+    .. danger::
+
+        As this wraps a subprocess call, ensure that
+        arguments such as ``executable`` are not
+        set from direct user input.
     """
 
     def __init__(
         self,
         source: Union[str, io.BufferedIOBase],
         *,
         executable: str = "ffmpeg",
@@ -165,15 +171,20 @@
         except FileNotFoundError:
             executable = args.partition(" ")[0] if isinstance(args, str) else args[0]
             raise ClientException(f"{executable} was not found.") from None
         except subprocess.SubprocessError as exc:
             raise ClientException(f"Popen failed: {exc.__class__.__name__}: {exc}") from exc
 
     def _kill_process(self) -> None:
-        proc = self._process
+        try:
+            proc = self._process
+        except AttributeError:
+            # may occur if something errors while spawning process
+            return
+
         if proc is MISSING:
             return
 
         _log.info("Preparing to terminate ffmpeg process %s.", proc.pid)
 
         try:
             proc.kill()
@@ -236,14 +247,19 @@
     ----------
     source: Union[:class:`str`, :class:`io.BufferedIOBase`]
         The input that ffmpeg will take and convert to PCM bytes.
         If ``pipe`` is ``True`` then this is a file-like object that is
         passed to the stdin of ffmpeg.
     executable: :class:`str`
         The executable name (and path) to use. Defaults to ``ffmpeg``.
+
+        .. danger::
+
+            As this wraps a subprocess call, ensure that
+            this argument is not set from direct user input.
     pipe: :class:`bool`
         If ``True``, denotes that ``source`` parameter will be passed
         to the stdin of ffmpeg. Defaults to ``False``.
     stderr: Optional[:term:`py:file object`]
         A file-like object to pass to the Popen constructor.
         Could also be an instance of ``subprocess.PIPE``.
     before_options: Optional[:class:`str`]
@@ -338,14 +354,19 @@
 
             Do not provide this parameter unless you are certain that the audio input is
             already Opus encoded.  For typical use :meth:`FFmpegOpusAudio.from_probe`
             should be used to determine the proper value for this parameter.
 
     executable: :class:`str`
         The executable name (and path) to use. Defaults to ``ffmpeg``.
+
+        .. danger::
+
+            As this wraps a subprocess call, ensure that
+            this argument is not set from direct user input.
     pipe: :class:`bool`
         If ``True``, denotes that ``source`` parameter will be passed
         to the stdin of ffmpeg. Defaults to ``False``.
     stderr: Optional[:term:`py:file object`]
         A file-like object to pass to the Popen constructor.
         Could also be an instance of ``subprocess.PIPE``.
     before_options: Optional[:class:`str`]
```

### Comparing `disnake-2.9.1/disnake/raw_models.py` & `disnake-2.9.2/disnake/raw_models.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/reaction.py` & `disnake-2.9.2/disnake/reaction.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/role.py` & `disnake-2.9.2/disnake/role.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/shard.py` & `disnake-2.9.2/disnake/shard.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,28 +186,46 @@
                 resume=exc.resume,
                 shard_id=self.id,
                 session=self.ws.session_id,
                 sequence=self.ws.sequence,
                 gateway=self.ws.resume_gateway if exc.resume else None,
             )
             self.ws = await asyncio.wait_for(coro, timeout=60.0)
+        # n.b. this is the same error handling as for the actual worker, but for the initial connect steps
+        except ReconnectWebSocket as e:
+            _log.debug(
+                "Unexpectedly received request to %s shard ID %s while attempting to %s",
+                e.op,
+                self.id,
+                exc.op,
+            )
+            etype = EventType.resume if e.resume else EventType.identify
+            self._queue_put(EventItem(etype, self, e))
         except self._handled_exceptions as e:
             await self._handle_disconnect(e)
         except asyncio.CancelledError:
             return
         except Exception as e:
             self._queue_put(EventItem(EventType.terminate, self, e))
         else:
             self.launch()
 
     async def reconnect(self) -> None:
         self._cancel_task()
         try:
             coro = DiscordWebSocket.from_client(self._client, shard_id=self.id)
             self.ws = await asyncio.wait_for(coro, timeout=60.0)
+        except ReconnectWebSocket as e:
+            _log.debug(
+                "Unexpectedly received request to %s shard ID %s while attempting to reconnect",
+                e.op,
+                self.id,
+            )
+            etype = EventType.resume if e.resume else EventType.identify
+            self._queue_put(EventItem(etype, self, e))
         except self._handled_exceptions as e:
             await self._handle_disconnect(e)
         except asyncio.CancelledError:
             return
         except Exception as e:
             self._queue_put(EventItem(EventType.terminate, self, e))
         else:
```

### Comparing `disnake-2.9.1/disnake/stage_instance.py` & `disnake-2.9.2/disnake/stage_instance.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/state.py` & `disnake-2.9.2/disnake/state.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/sticker.py` & `disnake-2.9.2/disnake/sticker.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,17 @@
 
     id: int
     format: StickerFormatType
 
     @property
     def url(self) -> str:
         """:class:`str`: The url for the sticker's image."""
-        return f"{Asset.BASE}/stickers/{self.id}.{self.format.file_extension}"
+        # https://github.com/discord/discord-api-docs/issues/6675#issuecomment-1954755672
+        base = Asset.BASE_MEDIA if self.format is StickerFormatType.gif else Asset.BASE
+        return f"{base}/stickers/{self.id}.{self.format.file_extension}"
 
     async def read(self) -> bytes:
         """|coro|
 
         Retrieves the content of this sticker as a :class:`bytes` object.
 
         .. note::
```

### Comparing `disnake-2.9.1/disnake/team.py` & `disnake-2.9.2/disnake/team.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/template.py` & `disnake-2.9.2/disnake/template.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/threads.py` & `disnake-2.9.2/disnake/threads.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/activity.py` & `disnake-2.9.2/disnake/types/activity.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/appinfo.py` & `disnake-2.9.2/disnake/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/audit_log.py` & `disnake-2.9.2/disnake/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/automod.py` & `disnake-2.9.2/disnake/types/automod.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/channel.py` & `disnake-2.9.2/disnake/types/channel.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/components.py` & `disnake-2.9.2/disnake/types/components.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/embed.py` & `disnake-2.9.2/disnake/types/embed.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/gateway.py` & `disnake-2.9.2/disnake/types/gateway.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/guild.py` & `disnake-2.9.2/disnake/types/guild.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/guild_scheduled_event.py` & `disnake-2.9.2/disnake/types/guild_scheduled_event.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/integration.py` & `disnake-2.9.2/disnake/types/integration.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/interactions.py` & `disnake-2.9.2/disnake/types/interactions.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/invite.py` & `disnake-2.9.2/disnake/types/invite.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/member.py` & `disnake-2.9.2/disnake/types/member.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/message.py` & `disnake-2.9.2/disnake/types/message.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/onboarding.py` & `disnake-2.9.2/disnake/types/onboarding.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/role.py` & `disnake-2.9.2/disnake/types/role.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/sticker.py` & `disnake-2.9.2/disnake/types/sticker.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/template.py` & `disnake-2.9.2/disnake/types/template.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/threads.py` & `disnake-2.9.2/disnake/types/threads.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/user.py` & `disnake-2.9.2/disnake/types/user.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/voice.py` & `disnake-2.9.2/disnake/types/voice.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/webhook.py` & `disnake-2.9.2/disnake/types/webhook.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/types/widget.py` & `disnake-2.9.2/disnake/types/widget.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/action_row.py` & `disnake-2.9.2/disnake/ui/action_row.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/button.py` & `disnake-2.9.2/disnake/ui/button.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/item.py` & `disnake-2.9.2/disnake/ui/item.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/modal.py` & `disnake-2.9.2/disnake/ui/modal.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/select/__init__.py` & `disnake-2.9.2/disnake/ui/select/__init__.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/select/base.py` & `disnake-2.9.2/disnake/ui/select/base.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/select/channel.py` & `disnake-2.9.2/disnake/ui/select/channel.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/select/mentionable.py` & `disnake-2.9.2/disnake/ui/select/mentionable.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/select/role.py` & `disnake-2.9.2/disnake/ui/select/role.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/select/string.py` & `disnake-2.9.2/disnake/ui/select/string.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/select/user.py` & `disnake-2.9.2/disnake/ui/select/user.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/text_input.py` & `disnake-2.9.2/disnake/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/ui/view.py` & `disnake-2.9.2/disnake/ui/view.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/user.py` & `disnake-2.9.2/disnake/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,35 +361,30 @@
     async def edit(
         self, *, username: str = MISSING, avatar: Optional[AssetBytes] = MISSING
     ) -> ClientUser:
         """|coro|
 
         Edits the current profile of the client.
 
-        .. note::
-
-            To upload an avatar, a resource (see below) or a :term:`py:bytes-like object`
-            must be passed in that represents the image being uploaded.
-
-            The only image formats supported for uploading are JPG and PNG.
-
         .. versionchanged:: 2.0
             The edit is no longer in-place, instead the newly edited client user is returned.
 
         .. versionchanged:: 2.6
             Raises :exc:`ValueError` instead of ``InvalidArgument``.
 
         Parameters
         ----------
         username: :class:`str`
             The new username you wish to change to.
         avatar: Optional[|resource_type|]
             A :term:`py:bytes-like object` or asset representing the image to upload.
             Could be ``None`` to denote no avatar.
 
+            Only JPG, PNG, WEBP (static), and GIF (static/animated) images are supported.
+
             .. versionchanged:: 2.5
                 Now accepts various resource types in addition to :class:`bytes`.
 
         Raises
         ------
         NotFound
             The ``avatar`` asset couldn't be found.
```

### Comparing `disnake-2.9.1/disnake/utils.py` & `disnake-2.9.2/disnake/utils.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/voice_client.py` & `disnake-2.9.2/disnake/voice_client.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/voice_region.py` & `disnake-2.9.2/disnake/voice_region.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/webhook/async_.py` & `disnake-2.9.2/disnake/webhook/async_.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     from ..embeds import Embed
     from ..file import File
     from ..guild import Guild
     from ..http import Response
     from ..mentions import AllowedMentions
     from ..message import Attachment
     from ..state import ConnectionState
-    from ..sticker import GuildSticker, StickerItem
+    from ..sticker import GuildSticker, StandardSticker, StickerItem
     from ..types.message import Message as MessagePayload
     from ..types.webhook import Webhook as WebhookPayload
     from ..ui.action_row import Components
     from ..ui.view import View
 
 MISSING = utils.MISSING
 
@@ -487,15 +487,15 @@
     attachments: Optional[List[Attachment]] = MISSING,
     embed: Optional[Embed] = MISSING,
     embeds: List[Embed] = MISSING,
     view: Optional[View] = MISSING,
     components: Optional[Components[MessageUIComponent]] = MISSING,
     allowed_mentions: Optional[AllowedMentions] = MISSING,
     previous_allowed_mentions: Optional[AllowedMentions] = None,
-    stickers: Sequence[Union[GuildSticker, StickerItem]] = MISSING,
+    stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = MISSING,
     thread_name: Optional[str] = None,
 ) -> DictPayloadParameters:
     if files is not MISSING and file is not MISSING:
         raise TypeError("Cannot mix file and files keyword arguments.")
     if embeds is not MISSING and embed is not MISSING:
         raise TypeError("Cannot mix embed and embeds keyword arguments.")
     if view is not MISSING and components is not MISSING:
@@ -574,15 +574,15 @@
     attachments: Optional[List[Attachment]] = MISSING,
     embed: Optional[Embed] = MISSING,
     embeds: List[Embed] = MISSING,
     view: Optional[View] = MISSING,
     components: Optional[Components[MessageUIComponent]] = MISSING,
     allowed_mentions: Optional[AllowedMentions] = MISSING,
     previous_allowed_mentions: Optional[AllowedMentions] = None,
-    stickers: Sequence[Union[GuildSticker, StickerItem]] = MISSING,
+    stickers: Sequence[Union[GuildSticker, StandardSticker, StickerItem]] = MISSING,
     thread_name: Optional[str] = None,
 ) -> PayloadParameters:
     params = handle_message_parameters_dict(
         content=content,
         username=username,
         avatar_url=avatar_url,
         tts=tts,
```

### Comparing `disnake-2.9.1/disnake/webhook/sync.py` & `disnake-2.9.2/disnake/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/welcome_screen.py` & `disnake-2.9.2/disnake/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake/widget.py` & `disnake-2.9.2/disnake/widget.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/disnake.egg-info/PKG-INFO` & `disnake-2.9.2/disnake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disnake
-Version: 2.9.1
+Version: 2.9.2
 Summary: A Python wrapper for the Discord API
 Author: Disnake Development
 License: MIT
 Project-URL: Changelog, https://docs.disnake.dev/page/whats_new.html
 Project-URL: Documentation, https://docs.disnake.dev/
 Project-URL: Repository, https://github.com/DisnakeDev/disnake
 Keywords: disnake,discord,discord api
@@ -144,15 +144,15 @@
 @bot.command()
 async def ping(ctx):
     await ctx.send("Pong!")
 
 bot.run("BOT_TOKEN")
 ```
 
-You can find more examples in the [examples directory](./examples).
+You can find more examples in the [examples directory](https://github.com/DisnakeDev/disnake/tree/master/examples).
 
 <br>
 <p align="center">
     <a href="https://docs.disnake.dev/">Documentation</a>
     ⁕
     <a href="https://guide.disnake.dev/">Guide</a>
     ⁕
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disnake Version: 2.9.1 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: disnake Version: 2.9.2 Summary: A Python wrapper
 for the Discord API Author: Disnake Development License: MIT Project-URL:
 Changelog, https://docs.disnake.dev/page/whats_new.html Project-URL:
 Documentation, https://docs.disnake.dev/ Project-URL: Repository, https://
 github.com/DisnakeDev/disnake Keywords: disnake,discord,discord api Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
@@ -56,10 +56,11 @@
 disnake from disnake.ext import commands bot = commands.InteractionBot
 (test_guilds=[12345]) @bot.user_command() async def avatar(inter, user): embed
 = disnake.Embed(title=str(user)) embed.set_image(url=user.display_avatar.url)
 await inter.response.send_message(embed=embed) bot.run("BOT_TOKEN") ``` ###
 Prefix Commands Example ``` py import disnake from disnake.ext import commands
 bot = commands.Bot(command_prefix=commands.when_mentioned) @bot.command() async
 def ping(ctx): await ctx.send("Pong!") bot.run("BOT_TOKEN") ``` You can find
-more examples in the [examples directory](./examples).
+more examples in the [examples directory](https://github.com/DisnakeDev/
+disnake/tree/master/examples).
        _D_o_c_u_m_e_n_t_a_t_i_o_n â _G_u_i_d_e â _D_i_s_c_o_r_d_ _S_e_r_v_e_r â _D_i_s_c_o_r_d_ _D_e_v_e_l_o_p_e_r_s
```

### Comparing `disnake-2.9.1/disnake.egg-info/SOURCES.txt` & `disnake-2.9.2/disnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/pyproject.toml` & `disnake-2.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/setup.py` & `disnake-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_abc.py` & `disnake-2.9.2/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_colour.py` & `disnake-2.9.2/tests/test_colour.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_embeds.py` & `disnake-2.9.2/tests/test_embeds.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_events.py` & `disnake-2.9.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_flags.py` & `disnake-2.9.2/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_http.py` & `disnake-2.9.2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_mentions.py` & `disnake-2.9.2/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_message.py` & `disnake-2.9.2/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_object.py` & `disnake-2.9.2/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_onboarding.py` & `disnake-2.9.2/tests/test_onboarding.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_permissions.py` & `disnake-2.9.2/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `disnake-2.9.1/tests/test_utils.py` & `disnake-2.9.2/tests/test_utils.py`

 * *Files identical despite different names*

