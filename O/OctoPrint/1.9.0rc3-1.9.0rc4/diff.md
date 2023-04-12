# Comparing `tmp/OctoPrint-1.9.0rc3.tar.gz` & `tmp/OctoPrint-1.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OctoPrint-1.9.0rc3.tar", last modified: Wed Mar 22 13:00:39 2023, max compression
+gzip compressed data, was "dist/OctoPrint-1.9.0rc4.tar", last modified: Wed Apr 12 13:35:33 2023, max compression
```

## Comparing `OctoPrint-1.9.0rc3.tar` & `OctoPrint-1.9.0rc4.tar`

### file list

```diff
@@ -1,801 +1,801 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/SUPPORTERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/THIRDPARTYLICENSES.md
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32952 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/
--rw-r--r--   0 runner    (1001) docker     (123)    34215 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/access/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23546 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/access/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/access/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    47892 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/access/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/systeminfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/timelapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/filemanager/
--rw-r--r--   0 runner    (1001) docker     (123)    37796 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/filemanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/filemanager/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/filemanager/destinations.py
--rw-r--r--   0 runner    (1001) docker     (123)    73987 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/filemanager/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/filemanager/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/logging/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85631 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugin/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   106266 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugin/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/clientjs/action_command_notification.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/css/action_command_notification.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/js/action_command_notification.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/templates/action_command_notification_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/templates/action_command_notification_sidebar.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/templates/action_command_notification_sidebar_header.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/static/clientjs/action_command_prompt.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/static/js/action_command_prompt.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/templates/action_command_prompt_navbar.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/templates/action_command_prompt_settings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/
--rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/css/announcements.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/js/announcements.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/less/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/less/announcements.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/templates/announcements.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/templates/announcements_navbar.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/templates/announcements_settings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/
--rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/clientjs/appkeys.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/css/appkeys.css
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/css/authdialog.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/js/appkeys.js
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/js/authdialog.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/less/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/less/appkeys.less
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/less/authdialog.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/appkeys.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/appkeys_authdialog.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/appkeys_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/appkeys_usersettings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/
--rw-r--r--   0 runner    (1001) docker     (123)    58519 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/clientjs/backup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/css/backup.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/js/backup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/less/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/less/backup.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/templates/backup_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/templates/backup_wizard.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/templates/snippets/backup_plugin_upload_form.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/css/classicwebcam.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/js/classicwebcam.js
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/js/classicwebcam_settings.js
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/js/classicwebcam_wizard.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/less/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/less/classicwebcam.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/classicwebcam_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/classicwebcam_webcam.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/classicwebcam_wizard.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamCacheBuster.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamOrientation.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamSnapshotUrl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamRatio.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamTimeout.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamUrl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamWebrtcIceServers.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/static/css/corewizard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/static/js/corewizard.js
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/subwizards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_acl_wizard.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_onlinecheck_wizard.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_pluginblacklist_wizard.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_printerprofile_wizard.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_servercommands_wizard.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/discovery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/discovery/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/discovery/templates/discovery.xml.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/static/js/errortracking.js
--rw-r--r--   0 runner    (1001) docker     (123)    65254 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/static/js/sentry.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/templates/errortracking_javascripts.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/templates/errortracking_settings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/static/js/events.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/templates/eventmanager_settings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/css/gcodeviewer.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   273987 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/lib/pako.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/reader.js
--rw-r--r--   0 runner    (1001) docker     (123)    48111 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/renderer.js
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    30670 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/less/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/less/gcodeviewer.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_initscript.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_tab.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/clientjs/logging.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/css/logging.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/js/logging.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/less/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/less/logging.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/templates/logging_navbar_plugintimingslog.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/templates/logging_navbar_seriallog.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/templates/logging_settings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    86141 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/clientjs/pluginmanager.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/css/pluginmanager.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/img/repo_unavailable.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    97381 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/less/
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/less/pluginmanager.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/templates/pluginmanager_about.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    37493 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/
--rw-r--r--   0 runner    (1001) docker     (123)   100021 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/scripts/update-octoprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/clientjs/softwareupdate.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/css/softwareupdate.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    58418 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/js/softwareupdate.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/less/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/less/softwareupdate.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/checkoutFolder.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/githubToken.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/pipEnableCheck.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/pipTarget.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/releaseChannel.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/trackedBranch.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/versionTracking.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    15776 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/softwareupdate_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/softwareupdate_wizard_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/softwareupdate_wizard_update.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/python_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/single_file_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/sleep_a_bit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/update_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/always_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/bitbucket_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/commandline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/git_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/github_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/github_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/httpheader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/never_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/pypi_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/python_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)    19953 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/static/clientjs/usage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/static/js/usage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/templates/snippets/trackingDescription.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/templates/snippets/trackingDetails.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/templates/tracking_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/templates/tracking_wizard.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/virtual_printer/
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/virtual_printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/virtual_printer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/virtual_printer/templates/virtual_printer_settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    86569 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/plugins/virtual_printer/virtual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/printer/
--rw-r--r--   0 runner    (1001) docker     (123)    28922 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/printer/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    28139 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/printer/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    75213 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/printer/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/appearance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/devel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/gcode_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/printer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/printer_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/slicing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/terminalfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/config/webcam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/webcam/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/schema/webcam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/server/
--rw-r--r--   0 runner    (1001) docker     (123)   109005 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/
--rw-r--r--   0 runner    (1001) docker     (123)    24429 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    49926 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/printer_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    52843 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/slicing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/timelapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/api/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/server/util/
--rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/util/csrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    64469 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/util/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    27987 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/util/sockjs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65693 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/util/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/util/watchdog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/util/webassets.py
--rw-r--r--   0 runner    (1001) docker     (123)    61629 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/server/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/settings/
--rw-r--r--   0 runner    (1001) docker     (123)    73662 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/slicing/
--rw-r--r--   0 runner    (1001) docker     (123)    31325 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/slicing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/slicing/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-modal.css
--rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-responsive.css
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-responsive.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-slider.css
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-tabdrop.css
--rw-r--r--   0 runner    (1001) docker     (123)   124223 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   103314 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/jquery.fileupload-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/login.css
--rw-r--r--   0 runner    (1001) docker     (123)    92244 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/octoprint.css
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/pnotify.buttons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/pnotify.core.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/pnotify.history.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/css/recovery.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/css/forcelogin.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/js/forcelogin.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/less/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/less/forcelogin.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/glyphicons-halflings-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/glyphicons-halflings.png
--rw-r--r--   0 runner    (1001) docker     (123)    28174 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/graph-background.png
--rw-r--r--   0 runner    (1001) docker     (123)    46027 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/mask-theme.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/mask.svg
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/play.svg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-20x20-light.png
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-20x20-light@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-20x20.png
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-20x20@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-22x22.png
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-56x56.png
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-76x76.png
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/trans-background.png
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/img/watermark.png
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/intermediary.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/allowbindings.js
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/contextmenu.js
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/gettext.js
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/invisible.js
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/popover.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/qrcode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/slimscrolledforeach.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/toggle.js
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/togglecontent.js
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/valuewithinit.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/access.js
--rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/browser.js
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/connection.js
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/control.js
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/files.js
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/job.js
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/languages.js
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/printer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/printerprofiles.js
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/slicing.js
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/socket.js
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/system.js
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/timelapse.js
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/users.js
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/util.js
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/wizard.js
--rw-r--r--   0 runner    (1001) docker     (123)    20273 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/dataupdater.js
--rw-r--r--   0 runner    (1001) docker     (123)    52896 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/helpers.js
--rw-r--r--   0 runner    (1001) docker     (123)    41489 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/about.js
--rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/access.js
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/appearance.js
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/connection.js
--rw-r--r--   0 runner    (1001) docker     (123)    25329 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/control.js
--rw-r--r--   0 runner    (1001) docker     (123)    75182 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/files.js
--rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/loginstate.js
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/loginui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/navigation.js
--rw-r--r--   0 runner    (1001) docker     (123)    27913 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/printerprofiles.js
--rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/printerstate.js
--rw-r--r--   0 runner    (1001) docker     (123)    61077 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/slicing.js
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/system.js
--rw-r--r--   0 runner    (1001) docker     (123)    40085 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/temperature.js
--rw-r--r--   0 runner    (1001) docker     (123)    20045 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/terminal.js
--rw-r--r--   0 runner    (1001) docker     (123)    30932 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/timelapse.js
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/uistate.js
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/users.js
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/usersettings.js
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/wizard.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    99405 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/babel-polyfill.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/babel.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap-modal.js
--rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap-modalmanager.js
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap-slider.js
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap-tabdrop.js
--rw-r--r--   0 runner    (1001) docker     (123)    62124 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap-slider-knockout-binding.js
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/detectmobilebrowser.js
--rw-r--r--   0 runner    (1001) docker     (123)   710906 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/hls.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)    25960 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.bootstrap.wizard.js
--rw-r--r--   0 runner    (1001) docker     (123)    56680 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.fileupload.js
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.flot.crosshair.js
--rw-r--r--   0 runner    (1001) docker     (123)   122971 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.flot.js
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.flot.resize.js
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.flot.time.js
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.iframe-transport.js
--rw-r--r--   0 runner    (1001) docker     (123)   287630 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)    89476 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    25788 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.slimscroll.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    68249 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/knockout.js
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/knockout.mapping-latest.js
--rw-r--r--   0 runner    (1001) docker     (123)   475065 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/less.js
--rw-r--r--   0 runner    (1001) docker     (123)   411376 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/lodash.js
--rw-r--r--   0 runner    (1001) docker     (123)    50543 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/lodash.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/loglevel.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/md5.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/modernizr.custom.js
--rw-r--r--   0 runner    (1001) docker     (123)   369125 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/moment-with-locales.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.buttons.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.callbacks.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.confirm.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.core.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.desktop.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.history.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.maxheight.js
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.mobile.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.nonblock.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.reference.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.tooltip.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pusher.color.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    63624 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/sockjs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/sprintf.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/ua-parser.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/login/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/login/login.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/recovery/
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/recovery/recovery.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/reverse_proxy_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/js/reverse_proxy_test/reverse_proxy_test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/accordion.less
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/alerts.less
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/bootstrap.less
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/breadcrumbs.less
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/button-groups.less
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/buttons.less
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/carousel.less
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/close.less
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/code.less
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/component-animations.less
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/dropdowns.less
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/forms.less
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/grid.less
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/hero-unit.less
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/labels-badges.less
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/layouts.less
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/media.less
--rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/mixins.less
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/modals.less
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/navbar.less
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/navs.less
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/pager.less
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/pagination.less
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/popovers.less
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/progress-bars.less
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/reset.less
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-1200px-min.less
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-767px-max.less
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-768px-979px.less
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-navbar.less
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-utilities.less
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive.less
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/scaffolding.less
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/sprites.less
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/tables.less
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/thumbnails.less
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/tooltip.less
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/type.less
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/utilities.less
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/variables.less
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/wells.less
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/font-awesome.less
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/login.less
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/mixins.less
--rw-r--r--   0 runner    (1001) docker     (123)    30768 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/octoprint.less
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/recovery.less
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/less/variables.less
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    95915 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fa5-power-transforms.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/css/
--rw-r--r--   0 runner    (1001) docker     (123)    27215 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    61896 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    37405 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   197829 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)    79076 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    43572 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/
--rw-r--r--   0 runner    (1001) docker     (123)   137917 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/all.css
--rw-r--r--   0 runner    (1001) docker     (123)   100782 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    40712 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/v4-shims.css
--rw-r--r--   0 runner    (1001) docker     (123)    26235 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/v4-shims.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   388460 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   154228 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/systemcommands/
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/systemcommands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/_data/
--rw-r--r--   0 runner    (1001) docker     (123)    38161 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/_data/agpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/about.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/authors.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/license.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/supporters.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/systeminfo.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/thirdparty.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/files.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/accesscontrol.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/api.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/appearance.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/features.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/folders.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/gcodescripts.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/printerprofiles.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    54245 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/serialconnection.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/server.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/temperatures.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/terminalfilters.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/webcam.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/slicing.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/temperature.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/timelapse.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/usersettings/
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/usersettings/access.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/usersettings/interface.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/usersettings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/wizard/firstrun_end.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/wizard/firstrun_start.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/wizard.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/footer.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/i18n.js.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/index.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/initscript.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/javascripts-preload.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/javascripts.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/login.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/navbar/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/navbar/login.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/navbar/offlineindicator.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/navbar/settings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/navbar/systemmenu.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/overlays/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/overlays/dragndrop.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/overlays/offline.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/overlays/reloadui.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/recovery.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/reverse_proxy_test.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/connection.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/connection_header.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/files.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/files_header.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/state.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/group_list.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/groups.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/permission_list.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/subgroup_list.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/users.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditor.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorAxes.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorBuildvolume.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorExtruder.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorGeneral.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profiles.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverAllowFraming.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverCommandServerRestart.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverCommandSystemRestart.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverCommandSystemShutdown.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheck.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckDescription.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckEnabled.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckHost.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckInterval.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckName.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckPort.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckTestConnectivity.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckTestResolution.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginBlacklist.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistDescription.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistEnabled.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistTtl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistUrl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginTimings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/ffmpegBitrate.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/ffmpegCommandline.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/ffmpegPath.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/ffmpegThreads.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/ffmpegVideoCodec.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/timelapseEnabled.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/watermark.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/webcamEnabled.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/webcamSnapshotSslValidation.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/webcamSnapshotTimeout.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/webcamSnapshotUrl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/stylesheets-preload.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/stylesheets.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/control.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/temperature.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/terminal.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    18255 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/timelapse.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    44603 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/timelapse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   216940 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   383798 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/util/
--rw-r--r--   0 runner    (1001) docker     (123)    54507 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   262719 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/commandline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)    31001 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/gcodeInterpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/jinja.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/util/json/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/json/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/json/serializing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/net.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/util/piptestballoon/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/piptestballoon/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/util/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/awesome_slugify/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/awesome_slugify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/awesome_slugify/alt_translates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/awesome_slugify/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/flask_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/imp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/basehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/router.py
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/sessioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/eventsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/htmlfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/jsonp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/pollingbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/rawwebsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/streamingbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/xhr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/xhrstreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/vendor/with_attrs_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint/webcams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint_client/
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:00:39.000000 OctoPrint-1.9.0rc3/src/octoprint_setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/src/octoprint_setuptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81241 2023-03-22 13:00:33.000000 OctoPrint-1.9.0rc3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/SUPPORTERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/THIRDPARTYLICENSES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32952 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/
+-rw-r--r--   0 runner    (1001) docker     (123)    34215 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/access/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23546 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/access/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/access/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47892 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/access/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/systeminfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/timelapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/filemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    37796 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/filemanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/filemanager/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/filemanager/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73987 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/filemanager/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/filemanager/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/logging/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85631 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugin/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106454 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugin/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/clientjs/action_command_notification.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/css/action_command_notification.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/js/action_command_notification.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/templates/action_command_notification_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/templates/action_command_notification_sidebar.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/templates/action_command_notification_sidebar_header.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/static/clientjs/action_command_prompt.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/static/js/action_command_prompt.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/templates/action_command_prompt_navbar.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/templates/action_command_prompt_settings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/
+-rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/css/announcements.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/js/announcements.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/less/announcements.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/templates/announcements.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/templates/announcements_navbar.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/templates/announcements_settings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/clientjs/appkeys.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/css/appkeys.css
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/css/authdialog.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/js/appkeys.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/js/authdialog.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/less/appkeys.less
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/less/authdialog.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/appkeys.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/appkeys_authdialog.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/appkeys_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/appkeys_usersettings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)    58519 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/clientjs/backup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/css/backup.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/js/backup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/less/backup.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/templates/backup_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/templates/backup_wizard.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/templates/snippets/backup_plugin_upload_form.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/css/classicwebcam.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/js/classicwebcam.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/js/classicwebcam_settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/js/classicwebcam_wizard.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/less/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/less/classicwebcam.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/classicwebcam_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/classicwebcam_webcam.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/classicwebcam_wizard.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamCacheBuster.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamOrientation.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamSnapshotUrl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamRatio.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamTimeout.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamUrl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamWebrtcIceServers.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/static/css/corewizard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/static/js/corewizard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/subwizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_acl_wizard.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_onlinecheck_wizard.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_pluginblacklist_wizard.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_printerprofile_wizard.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_servercommands_wizard.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/discovery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/discovery/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/discovery/templates/discovery.xml.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/static/js/errortracking.js
+-rw-r--r--   0 runner    (1001) docker     (123)    65254 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/static/js/sentry.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/templates/errortracking_javascripts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/templates/errortracking_settings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/static/js/events.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/templates/eventmanager_settings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/css/gcodeviewer.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    40188 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   273987 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/lib/pako.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/reader.js
+-rw-r--r--   0 runner    (1001) docker     (123)    48111 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/renderer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30681 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/less/gcodeviewer.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_initscript.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_tab.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/clientjs/logging.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/css/logging.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/js/logging.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/less/logging.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/templates/logging_navbar_plugintimingslog.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/templates/logging_navbar_seriallog.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/templates/logging_settings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    86141 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/clientjs/pluginmanager.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/css/pluginmanager.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/img/repo_unavailable.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    97381 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/less/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/less/pluginmanager.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/templates/pluginmanager_about.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    37493 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/
+-rw-r--r--   0 runner    (1001) docker     (123)   100021 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/scripts/update-octoprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/clientjs/softwareupdate.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/css/softwareupdate.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    58418 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/js/softwareupdate.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/less/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/less/softwareupdate.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/checkoutFolder.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/githubToken.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/pipEnableCheck.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/pipTarget.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/releaseChannel.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/trackedBranch.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/versionTracking.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    15776 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/softwareupdate_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/softwareupdate_wizard_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/softwareupdate_wizard_update.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/python_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/single_file_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/sleep_a_bit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/update_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/always_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/bitbucket_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/commandline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/git_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/github_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/github_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/httpheader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/never_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/pypi_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/python_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)    19953 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/static/clientjs/usage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/static/js/usage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/templates/snippets/trackingDescription.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/templates/snippets/trackingDetails.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/templates/tracking_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/templates/tracking_wizard.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/virtual_printer/
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/virtual_printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/virtual_printer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/virtual_printer/templates/virtual_printer_settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    86569 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/plugins/virtual_printer/virtual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)    28922 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/printer/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28139 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/printer/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75213 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/printer/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/appearance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/devel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/gcode_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/printer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/printer_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/slicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/terminalfilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/config/webcam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/webcam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/schema/webcam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/server/
+-rw-r--r--   0 runner    (1001) docker     (123)   109005 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    24429 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49926 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/printer_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53031 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/slicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/timelapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/api/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/server/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/util/csrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64469 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/util/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27987 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/util/sockjs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65777 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/util/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/util/watchdog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/util/webassets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61629 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/server/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    73662 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/slicing/
+-rw-r--r--   0 runner    (1001) docker     (123)    31325 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/slicing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/slicing/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-modal.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-responsive.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-responsive.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-tabdrop.css
+-rw-r--r--   0 runner    (1001) docker     (123)   124223 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   103314 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/jquery.fileupload-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/login.css
+-rw-r--r--   0 runner    (1001) docker     (123)    92244 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/octoprint.css
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/pnotify.buttons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/pnotify.core.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/pnotify.history.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/css/recovery.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/css/forcelogin.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/js/forcelogin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/less/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/less/forcelogin.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/glyphicons-halflings-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/glyphicons-halflings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28174 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/graph-background.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46027 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/mask-theme.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/mask.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/play.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-20x20-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-20x20-light@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-20x20.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-20x20@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-22x22.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-56x56.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/trans-background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/img/watermark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/intermediary.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/allowbindings.js
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/contextmenu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/gettext.js
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/invisible.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/popover.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/qrcode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/slimscrolledforeach.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/toggle.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/togglecontent.js
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/valuewithinit.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/access.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/browser.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/connection.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/control.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/files.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/job.js
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/languages.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/printer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/printerprofiles.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/slicing.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/socket.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/system.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/timelapse.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/users.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/util.js
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/wizard.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20273 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/dataupdater.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52896 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/helpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41489 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/about.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/access.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/appearance.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/connection.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26065 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/control.js
+-rw-r--r--   0 runner    (1001) docker     (123)    75182 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/files.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/loginstate.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/loginui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/navigation.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27913 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/printerprofiles.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/printerstate.js
+-rw-r--r--   0 runner    (1001) docker     (123)    61077 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/slicing.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/system.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40085 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/temperature.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20045 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/terminal.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/timelapse.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/uistate.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/users.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/usersettings.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/wizard.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    99405 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/babel-polyfill.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/babel.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap-modal.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap-modalmanager.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap-slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap-tabdrop.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62124 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap-slider-knockout-binding.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/detectmobilebrowser.js
+-rw-r--r--   0 runner    (1001) docker     (123)   710906 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/hls.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    25960 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.bootstrap.wizard.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56680 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.fileupload.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.flot.crosshair.js
+-rw-r--r--   0 runner    (1001) docker     (123)   122971 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.flot.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.flot.resize.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.flot.time.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.iframe-transport.js
+-rw-r--r--   0 runner    (1001) docker     (123)   287630 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89476 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25788 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.slimscroll.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    68249 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/knockout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/knockout.mapping-latest.js
+-rw-r--r--   0 runner    (1001) docker     (123)   475065 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/less.js
+-rw-r--r--   0 runner    (1001) docker     (123)   411376 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/lodash.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50543 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/lodash.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/loglevel.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/md5.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/modernizr.custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)   369125 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/moment-with-locales.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.buttons.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.callbacks.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.confirm.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.core.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.desktop.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.history.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.maxheight.js
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.mobile.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.nonblock.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.reference.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.tooltip.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pusher.color.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    63624 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/sockjs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/sprintf.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/ua-parser.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/login/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/login/login.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/recovery/
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/recovery/recovery.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/reverse_proxy_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/js/reverse_proxy_test/reverse_proxy_test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/accordion.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/alerts.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/breadcrumbs.less
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/button-groups.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/buttons.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/carousel.less
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/close.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/code.less
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/component-animations.less
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/dropdowns.less
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/forms.less
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/grid.less
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/hero-unit.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/labels-badges.less
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/layouts.less
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/media.less
+-rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/mixins.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/modals.less
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/navbar.less
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/navs.less
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/pager.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/pagination.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/popovers.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/progress-bars.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/reset.less
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-1200px-min.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-767px-max.less
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-768px-979px.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-navbar.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-utilities.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive.less
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/scaffolding.less
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/sprites.less
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/tables.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/thumbnails.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/tooltip.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/type.less
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/utilities.less
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/wells.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/font-awesome.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/login.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/mixins.less
+-rw-r--r--   0 runner    (1001) docker     (123)    30768 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/octoprint.less
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/recovery.less
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/less/variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    95915 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fa5-power-transforms.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    27215 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    61896 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    37405 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   197829 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    79076 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    43572 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   137917 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)   100782 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    40712 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/v4-shims.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26235 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/v4-shims.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   388460 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   154228 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/systemcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/systemcommands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    38161 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/_data/agpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/about.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/authors.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/license.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/supporters.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/systeminfo.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/thirdparty.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/files.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/accesscontrol.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/api.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/appearance.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/features.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/folders.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/gcodescripts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/printerprofiles.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    54245 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/serialconnection.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/server.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/temperatures.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/terminalfilters.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/webcam.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/slicing.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/temperature.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/timelapse.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/usersettings/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/usersettings/access.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/usersettings/interface.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/usersettings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/wizard/firstrun_end.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/wizard/firstrun_start.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/wizard.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/footer.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/i18n.js.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/index.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/initscript.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/javascripts-preload.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/javascripts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/login.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/navbar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/navbar/login.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/navbar/offlineindicator.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/navbar/settings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/navbar/systemmenu.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/overlays/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/overlays/dragndrop.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/overlays/offline.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/overlays/reloadui.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/recovery.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/reverse_proxy_test.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/connection.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/connection_header.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/files.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/files_header.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/state.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/group_list.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/groups.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/permission_list.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/subgroup_list.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/users.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditor.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorAxes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorBuildvolume.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorExtruder.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorGeneral.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profiles.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverAllowFraming.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverCommandServerRestart.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverCommandSystemRestart.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverCommandSystemShutdown.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheck.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckDescription.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckEnabled.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckHost.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckInterval.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckName.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckPort.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckTestConnectivity.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckTestResolution.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginBlacklist.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistDescription.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistEnabled.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistTtl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistUrl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginTimings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/ffmpegBitrate.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/ffmpegCommandline.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/ffmpegPath.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/ffmpegThreads.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/ffmpegVideoCodec.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/timelapseEnabled.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/watermark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/webcamEnabled.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/webcamSnapshotSslValidation.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/webcamSnapshotTimeout.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/webcamSnapshotUrl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/stylesheets-preload.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/stylesheets.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/control.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/temperature.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/terminal.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/timelapse.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    44603 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/timelapse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:32.000000 OctoPrint-1.9.0rc4/src/octoprint/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   219284 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   386001 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    54507 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   262719 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/commandline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31001 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/gcodeInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/jinja.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/util/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/json/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/json/serializing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/util/piptestballoon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/piptestballoon/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/util/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/awesome_slugify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/awesome_slugify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/awesome_slugify/alt_translates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/awesome_slugify/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/flask_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/imp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/basehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/sessioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/eventsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/htmlfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/jsonp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/pollingbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/rawwebsocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/streamingbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/xhr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/xhrstreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/vendor/with_attrs_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint/webcams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:35:33.000000 OctoPrint-1.9.0rc4/src/octoprint_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/src/octoprint_setuptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81241 2023-04-12 13:35:29.000000 OctoPrint-1.9.0rc4/versioneer.py
```

### Comparing `OctoPrint-1.9.0rc3/AUTHORS.md` & `OctoPrint-1.9.0rc4/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/LICENSE.txt` & `OctoPrint-1.9.0rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/PKG-INFO` & `OctoPrint-1.9.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoPrint
-Version: 1.9.0rc3
+Version: 1.9.0rc4
 Summary: The snappy web interface for your 3D printer
 Home-page: https://octoprint.org
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: GNU Affero General Public License v3
 Project-URL: Community Forum, https://community.octoprint.org
 Project-URL: Bug Reports, https://github.com/OctoPrint/OctoPrint/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OctoPrint Version: 1.9.0rc3 Summary: The snappy web
+Metadata-Version: 2.1 Name: OctoPrint Version: 1.9.0rc4 Summary: The snappy web
 interface for your 3D printer Home-page: https://octoprint.org Author: Gina
 HÃ¤uÃge Author-email: gina@octoprint.org License: GNU Affero General Public
 License v3 Project-URL: Community Forum, https://community.octoprint.org
 Project-URL: Bug Reports, https://github.com/OctoPrint/OctoPrint/issues
 Project-URL: Source, https://github.com/OctoPrint/OctoPrint Project-URL:
 Funding, https://support.octoprint.org Description:
                               [OctoPrint's logo]
```

### Comparing `OctoPrint-1.9.0rc3/README.md` & `OctoPrint-1.9.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/SUPPORTERS.md` & `OctoPrint-1.9.0rc4/SUPPORTERS.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,69 +5,64 @@
 thanks to everyone who contributed!
 
 ## Patrons & Sponsors
 
   * 3D-TECH
   * 3DPrinterOS
   * Al Mucci
-  * Arnljot Arntsen
   * Ash King
   * Ben Fritsch
   * BigTreeTech
   * Boris Hussein
   * Brad Jackson
   * Christian Petropolis
   * Christian Wolf
   * Christian Würthner
   * Christoph Sigrist
-  * CooperSpartan
   * Creality3D
   * DeltaMaker 3D Printers
   * Dennis Breining
   * Douglas Floyd
   * Ed Crump
   * Ernesto Martinez
   * Franziska Kunsmann
   * Hog Duske
   * Jacob Renstrom
-  * James Mackay
   * Jeff Green
   * Jeff Moe
-  * jeffiel
   * Jeremy Cole
   * John Cassel
   * Julian Melo
   * Justin Kaufman
   * Kaile Riser
   * Kazuhiro Ogura
   * Kenneth Jiang
   * Kurt Wubbels
   * Lachlan Bell
   * Lefteris Lertas
   * LulzBot
+  * Makerbase
   * Makespace Madrid
   * Mark Greenwald
   * Mark Walker
   * Michael Aumock
-  * Mike Kershaw
+  * Michael Badagliacco
   * Mosaic Manufacturing
   * Norman Jaffe
   * Obico
   * Ory Weaver
   * Peopoly
   * Pete Barnwell
   * Raise3D
   * Randy C. Will
   * Ranjib Dey
   * Richard McGuire
-  * Richard Michaud
   * Richard Stocks
   * Robert Gusek
-  * Sean Jensen-Grey
-  * Sebastien Andrivet
   * SimplyPrint
+  * Songyin Zheng
   * Stefan Krister
   * Steve Dougherty
   * Steve Thompson
   * Ulrich Kempken
 
-and 2041 more wonderful people pledging on the [Patreon campaign](https://patreon.com/foosel) or via [GitHub Sponsors](https://github.com/users/foosel/sponsorship)!
+and 2025 more wonderful people pledging on the [Patreon campaign](https://patreon.com/foosel) or via [GitHub Sponsors](https://github.com/users/foosel/sponsorship)!
```

### Comparing `OctoPrint-1.9.0rc3/THIRDPARTYLICENSES.md` & `OctoPrint-1.9.0rc4/THIRDPARTYLICENSES.md`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/setup.cfg` & `OctoPrint-1.9.0rc4/setup.cfg`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/setup.py` & `OctoPrint-1.9.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,45 +44,45 @@
     "cachelib>=0.10.2,<0.11",
     "Click>=8.1.3,<9",
     "colorlog>=6.7.0,<7",
     "emoji>=2.2.0,<3",
     "feedparser>=6.0.10,<7",
     "filetype>=1.2.0,<2",
     "Flask-Assets>=2.0,<3",
-    "Flask-Babel>=3.0.1,<4",
+    "Flask-Babel>=3.1.0,<4",
     "Flask-Login>=0.6.2,<0.7",  # breaking changes can happen on minor version increases
     "Flask-Limiter>=3.3.0,<4",
     "flask>=2.2.3,<2.3",  # breaking changes can happen on minor version increases (with deprecation warnings)
-    "frozendict>=2.3.5,<3",
+    "frozendict>=2.3.7,<3",
     "future>=0.18.3,<1",  # not really needed anymore, but leaving in for py2/3 compat plugins
-    "markdown>=3.4.1,<4",
+    "markdown>=3.4.3,<4",
     "netaddr>=0.8,<0.9",  # changelog hints at breaking changes on minor version increases
     "netifaces>=0.11,<1",
     "passlib>=1.7.4,<2",
     "pathvalidate>=2.5.2,<3",
     "pkginfo>=1.9.6,<2",
     "psutil>=5.9.4,<6",
-    "pydantic>=1.10.5,<2",
+    "pydantic>=1.10.7,<2",
     "pylru>=1.2.1,<2",
     "pyserial>=3.5,<4",
     "PyYAML>=5.4.1,<6",  # no changelog available for version 6, so we're not risking it
     "requests>=2.28.2,<3",
     "sarge==0.1.7.post1",
     "semantic_version>=2.10.0,<3",
-    "sentry-sdk>=1.16.0,<2",
+    "sentry-sdk>=1.19.1,<2",
     "tornado>=6.2,<7",
     "watchdog>=2.3.1,<3",
     "websocket-client>=1.5.1,<2",
     "werkzeug>=2.2.3,<2.3",  # breaking changes can happen on minor version increases
     "wrapt>=1.15,<1.16",
     "zeroconf==0.39.4",  # final version to include universal wheel, later takes ages to compiles on rpi, piwheels has no wheels for latest either
-    "zipstream-ng>=1.4.0,<2.0.0",
+    "zipstream-ng>=1.5.0,<2.0.0",
 ]
 vendored_deps = [
-    "blinker>=1.5,<2",  # dependency of flask_principal
+    "blinker>=1.6.1,<2",  # dependency of flask_principal
     "class-doc>=0.2.6,<0.3",  # dependency of with_attrs_docs
     "regex",  # dependency of awesome-slugify
     "unidecode",  # dependency of awesome-slugify
 ]
 plugin_deps = [
     # "OctoPrint-Setuptools>=1.0.3",  # makes sure plugins can import this on setup.py based install
     "wheel",  # makes sure plugins can be built as wheels in OctoPrint's venv, see #4682
@@ -98,15 +98,15 @@
     ],
     # Dependencies for core development
     "develop": [
         # Testing dependencies
         "ddt",
         "mock>=5.0.1,<6",
         "pytest-doctest-custom>=1.0.0,<2",
-        "pytest>=7.2.2,<8",
+        "pytest>=7.3.0,<8",
         # pre-commit
         "pre-commit",
         # profiler
         "pyinstrument",
     ],
     # Dependencies for developing OctoPrint plugins
     "plugins": ["cookiecutter>=2.1.1,<3"],
```

### Comparing `OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/PKG-INFO` & `OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoPrint
-Version: 1.9.0rc3
+Version: 1.9.0rc4
 Summary: The snappy web interface for your 3D printer
 Home-page: https://octoprint.org
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: GNU Affero General Public License v3
 Project-URL: Community Forum, https://community.octoprint.org
 Project-URL: Bug Reports, https://github.com/OctoPrint/OctoPrint/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OctoPrint Version: 1.9.0rc3 Summary: The snappy web
+Metadata-Version: 2.1 Name: OctoPrint Version: 1.9.0rc4 Summary: The snappy web
 interface for your 3D printer Home-page: https://octoprint.org Author: Gina
 HÃ¤uÃge Author-email: gina@octoprint.org License: GNU Affero General Public
 License v3 Project-URL: Community Forum, https://community.octoprint.org
 Project-URL: Bug Reports, https://github.com/OctoPrint/OctoPrint/issues
 Project-URL: Source, https://github.com/OctoPrint/OctoPrint Project-URL:
 Funding, https://support.octoprint.org Description:
                               [OctoPrint's logo]
```

### Comparing `OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/SOURCES.txt` & `OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/OctoPrint.egg-info/requires.txt` & `OctoPrint-1.9.0rc4/src/OctoPrint.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,56 +6,56 @@
 cachelib<0.11,>=0.10.2
 Click<9,>=8.1.3
 colorlog<7,>=6.7.0
 emoji<3,>=2.2.0
 feedparser<7,>=6.0.10
 filetype<2,>=1.2.0
 Flask-Assets<3,>=2.0
-Flask-Babel<4,>=3.0.1
+Flask-Babel<4,>=3.1.0
 Flask-Login<0.7,>=0.6.2
 Flask-Limiter<4,>=3.3.0
 flask<2.3,>=2.2.3
-frozendict<3,>=2.3.5
+frozendict<3,>=2.3.7
 future<1,>=0.18.3
-markdown<4,>=3.4.1
+markdown<4,>=3.4.3
 netaddr<0.9,>=0.8
 netifaces<1,>=0.11
 passlib<2,>=1.7.4
 pathvalidate<3,>=2.5.2
 pkginfo<2,>=1.9.6
 psutil<6,>=5.9.4
-pydantic<2,>=1.10.5
+pydantic<2,>=1.10.7
 pylru<2,>=1.2.1
 pyserial<4,>=3.5
 PyYAML<6,>=5.4.1
 requests<3,>=2.28.2
 sarge==0.1.7.post1
 semantic_version<3,>=2.10.0
-sentry-sdk<2,>=1.16.0
+sentry-sdk<2,>=1.19.1
 tornado<7,>=6.2
 watchdog<3,>=2.3.1
 websocket-client<2,>=1.5.1
 werkzeug<2.3,>=2.2.3
 wrapt<1.16,>=1.15
 zeroconf==0.39.4
-zipstream-ng<2.0.0,>=1.4.0
-blinker<2,>=1.5
+zipstream-ng<2.0.0,>=1.5.0
+blinker<2,>=1.6.1
 class-doc<0.3,>=0.2.6
 regex
 unidecode
 wheel
 
 [:sys_platform == 'darwin']
 appdirs<2,>=1.4.4
 
 [develop]
 ddt
 mock<6,>=5.0.1
 pytest-doctest-custom<2,>=1.0.0
-pytest<8,>=7.2.2
+pytest<8,>=7.3.0
 pre-commit
 pyinstrument
 
 [docs]
 sphinx
 sphinxcontrib-httpdomain
 sphinxcontrib-mermaid
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/access/groups.py` & `OctoPrint-1.9.0rc4/src/octoprint/access/groups.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/access/permissions.py` & `OctoPrint-1.9.0rc4/src/octoprint/access/permissions.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/access/users.py` & `OctoPrint-1.9.0rc4/src/octoprint/access/users.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/analysis.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/analysis.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/client.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/client.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/common.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/common.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/config.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/config.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/dev.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/dev.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/plugins.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/server.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/server.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/systeminfo.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/systeminfo.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/timelapse.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/timelapse.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/cli/user.py` & `OctoPrint-1.9.0rc4/src/octoprint/cli/user.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/daemon.py` & `OctoPrint-1.9.0rc4/src/octoprint/daemon.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/environment.py` & `OctoPrint-1.9.0rc4/src/octoprint/environment.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/events.py` & `OctoPrint-1.9.0rc4/src/octoprint/events.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/filemanager/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/filemanager/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/filemanager/analysis.py` & `OctoPrint-1.9.0rc4/src/octoprint/filemanager/analysis.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/filemanager/storage.py` & `OctoPrint-1.9.0rc4/src/octoprint/filemanager/storage.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/filemanager/util.py` & `OctoPrint-1.9.0rc4/src/octoprint/filemanager/util.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/logging/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/logging/filters.py` & `OctoPrint-1.9.0rc4/src/octoprint/logging/filters.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/logging/handlers.py` & `OctoPrint-1.9.0rc4/src/octoprint/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugin/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugin/core.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugin/core.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugin/types.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugin/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -2342,14 +2342,16 @@
         """
         pass
 
 
 class WebcamProviderPlugin(OctoPrintPlugin):
     """
     The ``WebcamProviderPlugin`` can be used to provide one or more webcams visible on the frontend and used for snapshots/timelapses.
+
+    For an example of how to utilize this, see the bundled ``classicwebcam`` plugin, or the ``testpicture`` plugin available `here <https://github.com/OctoPrint/OctoPrint-Testpicture>`_.
     """
 
     def get_webcam_configurations(self):
         """
         Used to retrieve a list of available webcams
 
         Returns:
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/clientjs/action_command_notification.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/clientjs/action_command_notification.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/static/js/action_command_notification.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/static/js/action_command_notification.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/templates/action_command_notification_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/templates/action_command_notification_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/templates/action_command_notification_sidebar.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/templates/action_command_notification_sidebar.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_notification/templates/action_command_notification_sidebar_header.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_notification/templates/action_command_notification_sidebar_header.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/static/clientjs/action_command_prompt.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/static/clientjs/action_command_prompt.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/static/js/action_command_prompt.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/static/js/action_command_prompt.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/action_command_prompt/templates/action_command_prompt_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/action_command_prompt/templates/action_command_prompt_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/css/announcements.css` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/css/announcements.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/js/announcements.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/js/announcements.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/static/less/announcements.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/static/less/announcements.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/templates/announcements.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/templates/announcements.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/templates/announcements_navbar.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/templates/announcements_navbar.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/announcements/templates/announcements_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/announcements/templates/announcements_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/clientjs/appkeys.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/clientjs/appkeys.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/css/appkeys.css` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/css/appkeys.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/js/appkeys.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/js/appkeys.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/js/authdialog.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/js/authdialog.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/less/appkeys.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/less/appkeys.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/static/less/authdialog.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/static/less/authdialog.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/appkeys.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/appkeys.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/appkeys_authdialog.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/appkeys_authdialog.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/appkeys_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/appkeys_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/appkeys/templates/appkeys_usersettings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/appkeys/templates/appkeys_usersettings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/clientjs/backup.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/clientjs/backup.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/css/backup.css` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/css/backup.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/js/backup.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/js/backup.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/static/less/backup.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/static/less/backup.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/templates/backup_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/templates/backup_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/backup/templates/snippets/backup_plugin_upload_form.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/backup/templates/snippets/backup_plugin_upload_form.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
         with self._capture_mutex:
             self._logger.debug(f"Capturing image from {snapshot_url}")
             r = requests.get(
                 snapshot_url,
                 stream=True,
                 timeout=self._settings.get_int(["snapshotTimeout"]),
-                verify=self._settings.get_boolean(["rosnapshotSslValidationtate90"]),
+                verify=self._settings.get_boolean(["snapshotSslValidation"]),
             )
             r.raise_for_status()
             return r.iter_content(chunk_size=1024)
 
     # ~~ SettingsPlugin API
 
     def get_settings_defaults(self):
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/css/classicwebcam.css` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/css/classicwebcam.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/js/classicwebcam.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/js/classicwebcam.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -50,15 +50,15 @@
 
             self.webcamStreamValid = ko.pureComputed(function() {
                 var url = self.streamUrlEscaped();
                 return !url || validateWebcamUrl(url);
             });
         };
 
-        self.onWebcamVisbilityChange = function(visible) {
+        self.onWebcamVisibilityChange = function(visible) {
             self.webcamStreamVisible = visible;
             if (self.webcamStreamVisible) {
                 self._enableWebcam();
             } else {
                 self._disableWebcam();
             }
         };
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/js/classicwebcam_settings.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/js/classicwebcam_settings.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/static/less/classicwebcam.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/static/less/classicwebcam.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/classicwebcam_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/classicwebcam_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/classicwebcam_webcam.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/classicwebcam_webcam.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/classicwebcam_wizard.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/classicwebcam_wizard.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamCacheBuster.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamCacheBuster.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamOrientation.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamOrientation.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamSnapshotUrl.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamSnapshotUrl.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamRatio.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamRatio.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamUrl.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamUrl.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamWebrtcIceServers.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/classicwebcam/templates/snippets/classicwebcamStreamWebrtcIceServers.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/static/js/corewizard.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/static/js/corewizard.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/subwizards.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/subwizards.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_acl_wizard.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_acl_wizard.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_onlinecheck_wizard.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_onlinecheck_wizard.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_pluginblacklist_wizard.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_pluginblacklist_wizard.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_printerprofile_wizard.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_printerprofile_wizard.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/corewizard/templates/corewizard_servercommands_wizard.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/corewizard/templates/corewizard_servercommands_wizard.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/discovery/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/discovery/templates/discovery.xml.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/discovery/templates/discovery.xml.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 from octoprint.util import get_fully_qualified_classname as fqcn  # noqa: F401
 from octoprint.util.version import (
     get_octoprint_version_string,
     is_released_octoprint_version,
 )
 
 SENTRY_URL_SERVER = (
-    "https://cb1ee590a2f34baca47dd207d7f294d5@o118517.ingest.sentry.io/1373987"
+    "https://1af1a737d9684867859b6baec346addd@o118517.ingest.sentry.io/1373987"
 )
 SENTRY_URL_COREUI = (
-    "https://a32c80a4a282468d8d41fc2accb77088@o118517.ingest.sentry.io/1374096"
+    "https://9823e9176ee54cf385e31cbbef50dda7@o118517.ingest.sentry.io/1374096"
 )
 
 SETTINGS_DEFAULTS = {
     "enabled": False,
     "enabled_unreleased": False,
     "unique_id": None,
     "url_server": SENTRY_URL_SERVER,
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/static/js/errortracking.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/static/js/errortracking.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/static/js/sentry.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/static/js/sentry.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/templates/errortracking_javascripts.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/templates/errortracking_javascripts.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/errortracking/templates/errortracking_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/errortracking/templates/errortracking_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/static/js/events.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/static/js/events.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/eventmanager/templates/eventmanager_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/eventmanager/templates/eventmanager_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/css/gcodeviewer.css` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/css/gcodeviewer.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -342,16 +342,14 @@
         self.loadedFileDate = undefined;
         self.loadedFileSize = undefined;
         self.status = "idle";
         self.enabled = false;
 
         self.currentlyPrinting = false;
 
-        self.errorCount = 0;
-
         self.layerSlider = undefined;
         self.layerCommandSlider = undefined;
 
         self.currentLayer = undefined;
         self.currentCommand = undefined;
         self.maxLayer = undefined;
 
@@ -507,15 +505,20 @@
                 }
             });
         };
 
         self.loadFile = function(path, date, size) {
             self.enableReload(false);
             self.needsLoad = false;
-            if (self.status === "idle" && self.errorCount < 3) {
+            if (
+                self.status === "idle" &&
+                self.cachedPath !== path &&
+                self.cachedDate !== date &&
+                self.cachedSize !== size
+            ) {
                 self.status = "request";
 
                 self.cachedPath = path;
                 self.cachedDate = date;
                 self.cachedSize = size;
                 var par = {
                     url: OctoPrint.files.downloadPath("local", path),
@@ -606,15 +609,14 @@
                     self.tabActive &&
                     self.currentlyPrinting &&
                     self.renderer_syncProgress() &&
                     !self.waitForApproval()
                 ) {
                     self._renderPercentage(data.progress.completion);
                 }
-                self.errorCount = 0;
             } else {
                 if (self.status === "idle") self.clear();
                 if (
                     data.job.file.path &&
                     data.job.file.origin !== "sdcard" &&
                     self.status !== "request" &&
                     (!self.waitForApproval() ||
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/lib/pako.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/lib/pako.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/reader.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/reader.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -144,15 +144,18 @@
         // position on screen.
         if (key == null) return {
             layer: cachedLayer,
             cmd: cachedCmd
         };
 
         var layer = searchInLayers(0, rendererModel.length - 1, key);
-        var cmd = searchInCmds(layer, 0, GCODE.renderer.getLayer(layer).length - 1, key);
+        var cmds = GCODE.renderer.getLayer(layer);
+        if (cmds === undefined) return undefined;
+
+        var cmd = searchInCmds(layer, 0, cmds.length - 1, key);
 
         // remember last position
         cachedLayer = layer;
         cachedCmd = cmd;
 
         return {
             layer: layer,
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/renderer.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/renderer.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/ui.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/ui.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/js/viewer/worker.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/js/viewer/worker.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -391,15 +391,15 @@
     // the download failed.
     if (!response.ok) return;
 
     // create a reader object that will read the incoming data
     const reader = response.body.getReader();
 
     // we use these two variables to calculate the percentage.
-    var totalDownloadLength = response.headers.get("content-length");
+    var totalDownloadLength = response.headers.get("X-Original-Content-Length");
     var currentDownloadLength = 0;
 
     // lets read a first data chunk
     let {
         value: chunk,
         done: readerDone
     } = await reader.read();
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/static/less/gcodeviewer.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/static/less/gcodeviewer.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_tab.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_tab.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/clientjs/logging.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/clientjs/logging.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/css/logging.css` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/css/logging.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/js/logging.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/js/logging.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/static/less/logging.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/static/less/logging.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/logging/templates/logging_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/logging/templates/logging_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/clientjs/pluginmanager.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/clientjs/pluginmanager.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/css/pluginmanager.css` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/css/pluginmanager.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/img/repo_unavailable.png` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/img/repo_unavailable.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/static/less/pluginmanager.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/static/less/pluginmanager.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/templates/pluginmanager_about.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/templates/pluginmanager_about.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/cli.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/cli.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/exceptions.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/exceptions.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/scripts/update-octoprint.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/scripts/update-octoprint.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/clientjs/softwareupdate.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/clientjs/softwareupdate.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/css/softwareupdate.css` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/css/softwareupdate.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/js/softwareupdate.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/js/softwareupdate.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/static/less/softwareupdate.less` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/static/less/softwareupdate.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/githubToken.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/githubToken.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/pipEnableCheck.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/pipEnableCheck.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/snippets/releaseChannel.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/snippets/releaseChannel.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/softwareupdate_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/softwareupdate_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/templates/softwareupdate_wizard_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/templates/softwareupdate_wizard_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/pip.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/pip.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/python_updater.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/python_updater.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/single_file_plugin.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/single_file_plugin.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/sleep_a_bit.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/sleep_a_bit.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/updaters/update_script.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/updaters/update_script.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/util.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/util.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/always_current.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/always_current.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/bitbucket_commit.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/bitbucket_commit.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/commandline.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/commandline.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/git_commit.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/git_commit.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/github_commit.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/github_commit.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/github_release.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/github_release.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/httpheader.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/httpheader.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/jsondata.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/jsondata.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/never_current.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/never_current.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/pypi_release.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/pypi_release.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/softwareupdate/version_checks/python_checker.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/softwareupdate/version_checks/python_checker.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/static/clientjs/usage.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/static/clientjs/usage.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/static/js/usage.js` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/static/js/usage.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/templates/tracking_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/templates/tracking_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/tracking/templates/tracking_wizard.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/tracking/templates/tracking_wizard.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/virtual_printer/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/virtual_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/virtual_printer/templates/virtual_printer_settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/virtual_printer/templates/virtual_printer_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/plugins/virtual_printer/virtual.py` & `OctoPrint-1.9.0rc4/src/octoprint/plugins/virtual_printer/virtual.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/printer/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/printer/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/printer/estimation.py` & `OctoPrint-1.9.0rc4/src/octoprint/printer/estimation.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/printer/profile.py` & `OctoPrint-1.9.0rc4/src/octoprint/printer/profile.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/printer/standard.py` & `OctoPrint-1.9.0rc4/src/octoprint/printer/standard.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/access_control.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/access_control.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/api.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/api.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/appearance.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/appearance.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/controls.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/controls.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/devel.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/devel.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/estimation.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/estimation.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/events.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/events.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/feature.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/feature.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/folder.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/folder.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/gcode_analysis.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/gcode_analysis.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/plugins.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/plugins.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/scripts.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/scripts.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/serial.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/serial.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/server.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/server.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/slicing.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/slicing.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/system.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/system.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/temperature.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/temperature.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/terminalfilters.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/terminalfilters.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/config/webcam.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/config/webcam.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,7 +74,10 @@
     """The default timelapse settings."""
 
     cleanTmpAfterDays: int = 7
     """After how many days unrendered timelapses will be deleted."""
 
     defaultWebcam: str = "classic"
     """The name of the default webcam"""
+
+    snapshotWebcam: str = "classic"
+    """The name of the default webcam to use for snapshots"""
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/schema/webcam/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/schema/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/access.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/access.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/connection.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/connection.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/files.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/files.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/job.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/job.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/languages.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/languages.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/printer.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/printer.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/printer_profiles.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/printer_profiles.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/settings.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import octoprint.plugin
 import octoprint.util
 from octoprint.access.permissions import Permissions
 from octoprint.server import pluginManager, printer, userManager
 from octoprint.server.api import NO_CONTENT, api
 from octoprint.server.util.flask import no_firstrun_access, with_revalidation_checking
 from octoprint.settings import settings, valid_boolean_trues
+from octoprint.timelapse import configure_timelapse
 from octoprint.webcams import (
     get_default_webcam,
     get_snapshot_webcam,
     get_webcams_as_dicts,
 )
 
 # ~~ settings
@@ -652,14 +653,17 @@
         if "watermark" in data["webcam"]:
             s.setBoolean(["webcam", "watermark"], data["webcam"]["watermark"])
         if "defaultWebcam" in data["webcam"]:
             s.set(["webcam", "defaultWebcam"], data["webcam"]["defaultWebcam"])
         if "snapshotWebcam" in data["webcam"]:
             s.set(["webcam", "snapshotWebcam"], data["webcam"]["snapshotWebcam"])
 
+            # timelapse needs to be reconfigured now since it depends on the current snapshot webcam
+            configure_timelapse()
+
     if "feature" in data:
         if "temperatureGraph" in data["feature"]:
             s.setBoolean(
                 ["feature", "temperatureGraph"], data["feature"]["temperatureGraph"]
             )
         if "sdSupport" in data["feature"]:
             s.setBoolean(["feature", "sdSupport"], data["feature"]["sdSupport"])
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/slicing.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/slicing.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/system.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/system.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/timelapse.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/timelapse.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/api/users.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/api/users.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/util/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/util/csrf.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/util/csrf.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/util/flask.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/util/flask.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/util/sockjs.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/util/sockjs.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/util/tornado.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/util/tornado.py`

 * *Files 0% similar despite different names*

```diff
@@ -1188,14 +1188,16 @@
                 ),
             )
 
         if not self._allow_client_caching:
             self.set_header("Cache-Control", "max-age=0, must-revalidate, private")
             self.set_header("Expires", "-1")
 
+        self.set_header("X-Original-Content-Length", str(self.get_content_size()))
+
     @property
     def original_absolute_path(self):
         """The path of the uncompressed file corresponding to the compressed file"""
         if self._is_pre_compressed:
             return self.absolute_path.rstrip(".gz")
         return self.absolute_path
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/util/watchdog.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/util/watchdog.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/util/webassets.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/util/webassets.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/server/views.py` & `OctoPrint-1.9.0rc4/src/octoprint/server/views.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/settings/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/slicing/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/slicing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/slicing/exceptions.py` & `OctoPrint-1.9.0rc4/src/octoprint/slicing/exceptions.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-modal.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-modal.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-responsive.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-responsive.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-responsive.min.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap-slider.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap-slider.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/bootstrap.min.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/jquery.fileupload-ui.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/jquery.fileupload-ui.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/login.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/login.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/octoprint.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/octoprint.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/pnotify.core.min.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/pnotify.core.min.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/css/pnotify.history.min.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/css/pnotify.history.min.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/css/forcelogin.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/css/forcelogin.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/js/forcelogin.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/js/forcelogin.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/forcelogin/less/forcelogin.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/forcelogin/less/forcelogin.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/apple-touch-icon-114x114.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/apple-touch-icon-144x144.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/glyphicons-halflings-white.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/glyphicons-halflings.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/graph-background.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/graph-background.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/logo.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/mask-theme.svg` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/mask-theme.svg`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/mask.svg` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/mask.svg`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-20x20-light.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-20x20-light.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-20x20-light@2x.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-20x20-light@2x.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-20x20.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-20x20.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-20x20@2x.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-20x20@2x.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-22x22.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-22x22.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-32x32.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-32x32.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-56x56.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-56x56.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/tentacle-76x76.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/tentacle-76x76.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/trans-background.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/trans-background.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/img/watermark.png` & `OctoPrint-1.9.0rc4/src/octoprint/static/img/watermark.png`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/intermediary.html` & `OctoPrint-1.9.0rc4/src/octoprint/static/intermediary.html`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/contextmenu.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/contextmenu.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/gettext.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/gettext.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/invisible.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/invisible.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/popover.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/popover.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/qrcode.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/qrcode.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/slimscrolledforeach.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/slimscrolledforeach.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/toggle.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/toggle.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/bindings/togglecontent.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/bindings/togglecontent.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/access.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/access.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/base.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/base.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/browser.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/browser.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/connection.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/connection.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/control.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/control.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/files.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/files.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/job.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/job.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/languages.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/languages.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/printer.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/printer.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/printerprofiles.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/printerprofiles.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/settings.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/settings.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/slicing.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/slicing.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/socket.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/socket.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/system.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/system.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/timelapse.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/timelapse.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/users.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/users.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/util.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/util.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/client/wizard.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/client/wizard.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/dataupdater.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/dataupdater.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/helpers.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/helpers.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/main.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/main.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/about.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/about.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/access.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/access.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/appearance.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/appearance.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/connection.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/connection.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/control.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/control.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -62,33 +62,52 @@
                 console.debug(
                     `VM for webcam #${target.id} is not bound, skipping visibility update`
                 );
             } else if (vm === undefined) {
                 console.debug(
                     `VM for webcam #${target.id} not found, skipping visibility update`
                 );
-            } else if (typeof vm.onWebcamVisbilityChange === "function") {
-                vm.onWebcamVisbilityChange(visible);
+            } else if (typeof vm.onWebcamVisibilityChange === "function") {
+                vm.onWebcamVisibilityChange(visible);
             } else {
                 console.debug(
-                    `VM for webcam #${target.id} does not declare 'onWebcamVisbilityChange(visible)', skipping visibility update (vm=${vm.constructor.name})`
+                    `VM for webcam #${target.id} does not declare 'onWebcamVisibilityChange(visible)', skipping visibility update (vm=${vm.constructor.name})`
                 );
             }
         };
 
+        const selectedCameraStorageKey = "core.control.selectedCamera";
+        self.selectDefaultWebcam = function() {
+            let div = localStorage[selectedCameraStorageKey];
+
+            if (!div || document.getElementById(div.slice(1)) === null) {
+                div = undefined;
+            }
+
+            if (div !== undefined) {
+                $(`${div}_link a`).tab("show");
+            } else {
+                $("#webcam_plugins_container .nav li:first a").tab("show");
+            }
+        };
+
         self.onStartupComplete = function() {
+            $("#webcam_plugins_container .nav a[data-toggle='tab']").on("shown", (e) => {
+                localStorage[selectedCameraStorageKey] = e.target.hash;
+            });
+            self.selectDefaultWebcam();
             self.recreateIntersectionObservers();
         };
 
         self.recreateIntersectionObservers = function() {
             // We are using the IntersectionObserver API to determine whether a webcam is visible or not.
             // A webcam will not intersect with the control tab if the control tab is invisible because another tab
             // is selected or if the webcam isn't shown because another webcam is active.
             //
-            // Whenever the webacam changes visibility we will call onWebcamVisbilityChange() which the webcam's
+            // Whenever the webacam changes visibility we will call onWebcamVisibilityChange() which the webcam's
             //  VM can use to start or stop the stream.
             self.intersectionObservers.forEach(function(observer) {
                 observer.disconnect();
             });
             self.intersectionObservers = [];
 
             document
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/files.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/files.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/loginstate.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/loginstate.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/loginui.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/loginui.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/navigation.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/navigation.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/printerprofiles.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/printerprofiles.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/printerstate.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/printerstate.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/settings.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/settings.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/slicing.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/slicing.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/system.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/system.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/temperature.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/temperature.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/terminal.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/terminal.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/timelapse.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/timelapse.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -707,15 +707,15 @@
                 return;
             }
             self._warnedAboutCaptureFail = true;
 
             var html =
                 "<p>" +
                 gettext(
-                    "Failed repeatedly to capture timelapse frame from webcam - is the snapshot URL configured correctly and the camera on?"
+                    "Failed repeatedly to capture timelapse frame from webcam - is the snapshot webcam configured correctly and the camera on?"
                 );
 
             var additional = "";
             if (payload.snapshotDisplay) {
                 additional +=
                     'Snapshot info: <pre style="overflow: auto">' +
                     payload.snapshotDisplay +
@@ -771,15 +771,15 @@
 
             if (payload.reason === "no_frames") {
                 title = gettext("Cannot render timelapse");
                 html =
                     "<p>" +
                     _.sprintf(
                         gettext(
-                            "Rendering of timelapse %(movie_prefix)s is not possible since no frames were captured. Is the webcam configured correctly?"
+                            "Rendering of timelapse %(movie_prefix)s is not possible since no frames were captured. Is the snapshot webcam configured correctly?"
                         ), {
                             movie_prefix: _.escape(payload.movie_prefix)
                         }
                     ) +
                     "</p>";
             } else if ((payload.reason = "returncode")) {
                 title = gettext("Rendering timelapse failed");
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/uistate.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/uistate.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/users.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/users.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/usersettings.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/usersettings.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/app/viewmodels/wizard.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/app/viewmodels/wizard.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/babel-polyfill.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/babel-polyfill.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/babel.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/babel.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap-modal.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap-modal.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap-modalmanager.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap-modalmanager.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap-slider.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap-tabdrop.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap-tabdrop.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap/bootstrap.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap/bootstrap.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/bootstrap-slider-knockout-binding.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/bootstrap-slider-knockout-binding.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/detectmobilebrowser.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/detectmobilebrowser.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/hls.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/hls.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery-ui.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.bootstrap.wizard.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.bootstrap.wizard.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.fileupload.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.fileupload.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.flot.crosshair.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.flot.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.flot.resize.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.flot.time.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.flot.time.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.iframe-transport.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.iframe-transport.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.qrcode.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.qrcode.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/jquery/jquery.slimscroll.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/jquery/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/knockout.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/knockout.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/knockout.mapping-latest.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/knockout.mapping-latest.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/less.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/less.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/lodash.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/lodash.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/lodash.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/lodash.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/loglevel.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/loglevel.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/md5.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/md5.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/modernizr.custom.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/modernizr.custom.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/moment-with-locales.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.buttons.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.buttons.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.callbacks.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.callbacks.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.confirm.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.confirm.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.core.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.core.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.desktop.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.desktop.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.history.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.history.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.maxheight.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.maxheight.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.nonblock.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.nonblock.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pnotify/pnotify.reference.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pnotify/pnotify.reference.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/pusher.color.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/pusher.color.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/sockjs.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/sockjs.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/sprintf.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/sprintf.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/lib/ua-parser.min.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/lib/ua-parser.min.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/login/login.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/login/login.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/recovery/recovery.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/recovery/recovery.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/js/reverse_proxy_test/reverse_proxy_test.js` & `OctoPrint-1.9.0rc4/src/octoprint/static/js/reverse_proxy_test/reverse_proxy_test.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/accordion.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/accordion.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/alerts.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/alerts.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/bootstrap.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/bootstrap.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/button-groups.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/button-groups.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/buttons.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/buttons.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/carousel.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/carousel.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/close.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/close.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/code.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/code.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/dropdowns.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/dropdowns.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/forms.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/forms.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/hero-unit.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/hero-unit.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/labels-badges.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/labels-badges.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/media.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/media.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/mixins.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/mixins.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/modals.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/modals.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/navbar.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/navbar.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/navs.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/navs.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/pager.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/pager.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/pagination.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/pagination.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/popovers.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/popovers.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/progress-bars.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/progress-bars.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/reset.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/reset.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-1200px-min.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-1200px-min.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-767px-max.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-767px-max.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-navbar.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-navbar.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive-utilities.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/responsive.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/responsive.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/scaffolding.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/scaffolding.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/sprites.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/sprites.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/tables.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/tables.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/thumbnails.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/thumbnails.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/tooltip.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/tooltip.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/type.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/type.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/variables.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/variables.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/bootstrap/wells.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/bootstrap/wells.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/font-awesome.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/font-awesome.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/login.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/login.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/mixins.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/mixins.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/less/octoprint.less` & `OctoPrint-1.9.0rc4/src/octoprint/static/less/octoprint.less`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fa5-power-transforms.min.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fa5-power-transforms.min.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/css/font-awesome.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/css/font-awesome.min.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/FontAwesome.otf` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.eot` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.svg` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.ttf` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.woff` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/font-awesome-3.2.1/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/all.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/all.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/all.min.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/all.min.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/v4-shims.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/css/v4-shims.min.css` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-brands-400.ttf` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-brands-400.woff2` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-regular-400.ttf` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-regular-400.woff2` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-solid-900.ttf` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-solid-900.woff2` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-v4compatibility.ttf` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-v4compatibility.woff2` & `OctoPrint-1.9.0rc4/src/octoprint/static/vendor/fontawesome-6.1.1/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/systemcommands/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/systemcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/_data/agpl.html` & `OctoPrint-1.9.0rc4/src/octoprint/templates/_data/agpl.html`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/about.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/about.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about/systeminfo.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about/systeminfo.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/about.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/about.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/files.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/files.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/accesscontrol.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/accesscontrol.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/api.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/api.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/appearance.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/appearance.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/features.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/features.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/folders.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/folders.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/gcodescripts.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/gcodescripts.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/serialconnection.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/serialconnection.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/server.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/server.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/temperatures.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/temperatures.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings/terminalfilters.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings/terminalfilters.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/settings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/slicing.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/slicing.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/temperature.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/temperature.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/timelapse.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/timelapse.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/usersettings/access.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/usersettings/access.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/usersettings/interface.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/usersettings/interface.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/usersettings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/usersettings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/wizard/firstrun_end.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/wizard/firstrun_end.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/dialogs/wizard.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/dialogs/wizard.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/footer.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/footer.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/index.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/initscript.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/initscript.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/javascripts-preload.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/javascripts-preload.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/javascripts.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/javascripts.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/login.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/login.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/navbar/login.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/navbar/login.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/navbar/systemmenu.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/navbar/systemmenu.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/overlays/dragndrop.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/overlays/dragndrop.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/overlays/offline.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/overlays/offline.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/overlays/reloadui.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/overlays/reloadui.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/recovery.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/recovery.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/reverse_proxy_test.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/reverse_proxy_test.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/connection.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/connection.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/files.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/files.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/files_header.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/files_header.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/sidebar/state.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/sidebar/state.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/group_list.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/group_list.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/groups.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/groups.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/permission_list.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/permission_list.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/subgroup_list.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/subgroup_list.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/accesscontrol/users.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/accesscontrol/users.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditor.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditor.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorAxes.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorAxes.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorBuildvolume.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorBuildvolume.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorExtruder.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorExtruder.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorGeneral.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profileEditorGeneral.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/printerprofiles/profiles.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/printerprofiles/profiles.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheck.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheck.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckTestConnectivity.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckTestConnectivity.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverOnlineCheckTestResolution.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverOnlineCheckTestResolution.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginBlacklist.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginBlacklist.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistDescription.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistDescription.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistTtl.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginBlacklistTtl.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/server/serverPluginTimings.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/server/serverPluginTimings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
- <div class="control-group" title="">
-    <label class="control-label" for="settings-defaultWebcam">{{ _('Default Webcam') }}</label>
+ <div class="control-group" title="{{ _('Fallback Webcam')|edq }}">
+    <label class="control-label" for="settings-defaultWebcam">{{ _('Fallback Webcam') }}</label>
     <div class="controls">
         <select id="settings-defaultWebcam" data-bind="options: webcam_webcams,
                                 optionsText: function(key) { return key.displayName },
                                 optionsValue: function(key) { return key.name },
                                 value: webcam_defaultWebcam">
         </select>
 
 
         <!-- ko foreach: webcam_webcams -->
             <!-- ko if: name == $parent.webcam_defaultWebcam() -->
-                <span class="help-inline" style="padding-top: 10px; padding-bottom: 10px;">
-                    <span><b>{{ _('MJPEG stream')}}&nbsp;</b></span>
+                <div class="help-block">
+                    <span><strong>{{ _('MJPEG stream')}}&nbsp;</strong></span>
                     <!-- ko if: compat != null && compat.stream -->
-                        <span data-bind="text: compat.stream"></span>&nbsp;
-                        <a data-bind="attr: { href: compat.stream }" target="_blank"><i class="fa-solid fa-up-right-from-square"></i></a>
+                        <a data-bind="attr: { href: compat.stream }, text: compat.stream" rel="noreferer noopener" target="_blank"></a>
                     <!-- /ko -->
                     <!-- ko ifnot: compat != null && compat.stream -->
-                        <span>{{ _('Not supported')}}</span>
+                        {{ _('Not supported') }}
                     <!-- /ko -->
-                </span>
+                </div>
             <!-- /ko -->
         <!-- /ko -->
 
-        <span class="help-inline">{{ _('Selects the default webcam. If this webcam provides a MJPEG video stream, it will be available for old clients that do not make use of the webcam plugin system introduced with OctoPrint 1.9.0') }}</span>
-
-        <span class="help-inline" style="padding-top: 10px;">{{ _('You can make changes to this webcam in the plugin\'s settings.') }}</span>
-
+        <div class="help-block" style="padding-top: 10px;">{% trans %}
+            <p>
+                You can make changes to this webcam's configuration in its plugin settings if it provides any.
+            </p>
+        {% endtrans %}</div>
     </div>
 </div>
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/ffmpegCommandline.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/ffmpegCommandline.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/ffmpegPath.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/ffmpegPath.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,40 @@
- <div class="control-group" title="">
+ <div class="control-group" title="{{ _('Snapshot Webcam')|edq }}">
     <label class="control-label" for="settings-snapshotWebcam">{{ _('Snapshot Webcam') }}</label>
     <div class="controls">
         <select id="settings-snapshotWebcam" data-bind="options: webcam_webcams,
                                 optionsText: function(key) { return key.displayName },
                                 optionsValue: function(key) { return key.name },
                                 value: webcam_snapshotWebcam">
         </select>
 
         <!-- ko foreach: webcam_webcams -->
             <!-- ko if: name == $parent.webcam_snapshotWebcam() -->
-              <span class="help-inline" style="padding-top: 10px;">
-                    <span><b>{{ _('Snapshot stream')}}&nbsp;</b></span>
+              <div class="help-block">
+                    <span><strong>{{ _('Snapshot stream')}}&nbsp;</strong></span>
                     <!-- ko if: canSnapshot -->
                         <!-- ko if: snapshotDisplay -->
                             <span data-bind="text: snapshotDisplay"></span>&nbsp;
                             <a data-bind="attr: { href: snapshotDisplay }, visible: $parent.validURL(snapshotDisplay)" target="_blank"><i class="fa-solid fa-up-right-from-square"></i></a>
                         <!-- /ko -->
                         <!-- ko ifnot: snapshotDisplay -->
                             <span>{{ _('Supported')}}</span>
                         <!-- /ko -->
                     <!-- /ko -->
                     <!-- ko ifnot: canSnapshot -->
                         <span>{{ _('Not supported')}}</span>
                     <!-- /ko -->
-                </span>
+                </div>
             <!-- /ko -->
         <!-- /ko -->
 
-        <span class="help-inline" style="padding-top: 10px;">{{ _('You can make changes to this webcam in the plugin\'s settings.') }}</span>
+        <div class="help-block" style="padding-top: 10px;">{% trans %}
+            <p>
+                Selects the webcam to use to take snapshots for the timelapse.
+            </p>
+            <p>
+                You can make changes to this webcam's configuration in its plugin settings, if it provides any.
+            </p>
+        {% endtrans %}</div>
 
     </div>
 </div>
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/snippets/settings/webcam/webcamSnapshotUrl.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/snippets/settings/webcam/webcamSnapshotUrl.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/stylesheets-preload.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/stylesheets-preload.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/stylesheets.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/stylesheets.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/control.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/control.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 {% if enableWebcam %}
     <div id="webcam_plugins_container" tabindex="0" data-bind="visible: loginState.hasPermissionKo(access.permissions.WEBCAM), event: { keydown: onKeyDown, mouseover: onMouseOver, mouseout: onMouseOut, focus: onFocus }">
         <div class="tabbable row-fluid">
-            {% set nsContent = namespace(mark_active = True) %}
-            {% set nsTab = namespace(mark_active = True) %}
-
             <div class="tab-content" id="webcam-group">
             {% for key in templates.webcam.order %}
                 {% set entry, data = templates.webcam.entries[key] %}
                 {% if data is not none %}
                     {% if "custom_bindings" not in data or data["custom_bindings"] %}<!-- ko allowBindings: false -->{% endif %}
                     <div id="{{ data._div }}"
                             {% if "data_bind" in data %}data-bind="{{ data.data_bind }}"{% endif %}
-                            class="tab-pane {% if nsContent.mark_active %}active{% set nsContent.mark_active = False %}{% endif %} {% if classes_content in data %}{{ data.classes_content|join(' ') }}{% elif classes in data %}{{ data.classes|join(' ') }}{% endif %}"
+                            class="tab-pane {% if classes_content in data %}{{ data.classes_content|join(' ') }}{% elif classes in data %}{{ data.classes|join(' ') }}{% endif %}"
                             {% if "styles_content" in data %} style="{{ data.styles_content|join(', ') }}" {% elif styles in data %} style="{{ data.styles|join(', ') }}" {% endif %}
                             >
                         {% try "There was an error with the template {filename} at line number {lineno}: {exception}" %}{% include data.template ignore missing %}{% endtry %}
                     </div>
                     {% if "custom_bindings" not in data or data["custom_bindings"] %}<!-- /ko -->{% endif %}
                 {% endif %}
             {% endfor %}
@@ -25,15 +22,15 @@
 
         {% if templates.webcam.order|length > 1 %}
         <ul class="nav justify-content-end">
             {% for key in templates.webcam.order %}
                 {% set entry, data = templates.webcam.entries[key] %}
                 <li id="{{ data._div }}_link"
                     {% if "data_bind" in data %}data-bind="{{ data.data_bind }}"{% endif %}
-                    class="nav-item {% if nsTab.mark_active %}active{% set nsTab.mark_active = False %}{% endif %}">
+                    class="nav-item">
                     <a class="nav-link" href="#{{ data._div }}" data-toggle="tab">{{ entry|e }}</a>
                 </li>
             {% endfor %}
         </ul>
         {% endif %}
 
         <div class="keycontrol_overlay" data-bind="visible: showKeycontrols">
```

#### html2text {}

```diff
@@ -1,30 +1,25 @@
 {% if enableWebcam %}
-{% set nsContent = namespace(mark_active = True) %} {% set nsTab = namespace
-(mark_active = True) %}
 {% for key in templates.webcam.order %} {% set entry, data =
 templates.webcam.entries[key] %} {% if data is not none %} {% if
 "custom_bindings" not in data or data["custom_bindings"] %}{% endif %}
 % if "data_bind" in data %}data-bind="{{ data.data_bind }}"{% endif %}
-class="tab-pane {% if nsContent.mark_active %}active{% set
-nsContent.mark_active = False %}{% endif %} {% if classes_content in data %}{
-{ data.classes_content|join(' ') }}{% elif classes in data %}{
-{ data.classes|join(' ') }}{% endif %}" {% if "styles_content" in data %}
-style="{{ data.styles_content|join(', ') }}" {% elif styles in data %} style="{
-{ data.styles|join(', ') }}" {% endif %} > {% try "There was an error with the
-template {filename} at line number {lineno}: {exception}" %}{% include
-data.template ignore missing %}{% endtry %}
+class="tab-pane {% if classes_content in data %}{{ data.classes_content|join('
+') }}{% elif classes in data %}{{ data.classes|join(' ') }}{% endif %}" {% if
+"styles_content" in data %} style="{{ data.styles_content|join(', ') }}" {%
+elif styles in data %} style="{{ data.styles|join(', ') }}" {% endif %} > {%
+try "There was an error with the template {filename} at line number {lineno}:
+{exception}" %}{% include data.template ignore missing %}{% endtry %}
 {% if "custom_bindings" not in data or data["custom_bindings"] %}{% endif %} {%
 endif %} {% endfor %}
 {% if templates.webcam.order|length > 1 %}
     * {% for key in templates.webcam.order %} {% set entry, data =
       templates.webcam.entries[key] %}
     * % if "data_bind" in data %}data-bind="{{ data.data_bind }}"{% endif %}
-      class="nav-item {% if nsTab.mark_active %}active{% set nsTab.mark_active
-      = False %}{% endif %}"> {{_entry|e_}}
+      class="nav-item"> {{_entry|e_}}
 {% endfor %}
 {% endif %}
 {{ _("Keyboard controls active") }}
 → / ←: {{ _("X Axis") }} +/-
 ↑ / ↓: {{ _("Y Axis") }} +/-
 W, {{ _("Page↑") }} / S, {{ _("Page↓") }}: {{ _("Z Axis") }} +/-
 Home: {{ _("Home X/Y") }}
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/temperature.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/temperature.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/terminal.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/terminal.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/templates/tabs/timelapse.jinja2` & `OctoPrint-1.9.0rc4/src/octoprint/templates/tabs/timelapse.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
                     <button class="btn btn-block" data-bind="click: reset, enable: resetButtonEnabled">{{ _('Reset to active configuration') }}</button>
                 </div>
             </div>
         </form>
     </div>
     <div class="alert" style="display: none" data-bind="visible: !canSnapshot() || !settings.webcam_ffmpegPath()">
         <p><strong>{{ _('Timelapse not fully configured') }}</strong></p>
-        <p data-bind="visible: !loginState.isAdmin()">{{ _('The snapshot URL and/or the path to FFMPEG are missing. To have this fixed, get in touch with an administrator of this OctoPrint instance.') }}</p>
-        <p data-bind="visible: loginState.isAdmin">{{ _('The snapshot URL and/or the path to FFMPEG are missing. You can change both under "Settings" > "Webcam & Timelapse". If you don\'t have a webcam or don\'t want to enable timelapse support you can also just disable it there.') }}</p>
+        <p data-bind="visible: !loginState.isAdmin()">{{ _('A working snapshot setup and/or the path to FFMPEG are missing. To have this fixed, get in touch with an administrator of this OctoPrint instance.') }}</p>
+        <p data-bind="visible: loginState.isAdmin">{{ _('A working snapshot setup and/or the path to FFMPEG are missing. You can change both under "Settings" > "Webcam & Timelapse" and in the settings of your chosen webcam plugin. If you don\'t have a webcam or don\'t want to enable timelapse support you can also just disable it there.') }}</p>
         <p data-bind="visible: loginState.isUser"><small>
             <!-- ko if: canSnapshot -->
                 <!-- ko if: snapshotDisplay -->
                 {{ _('Currently configured snapshot (from default webcam)') }}: <span data-bind="text: snapshotDisplay"></span><br/>
                 <!-- /ko -->
                 <!-- ko ifnot: snapshotDisplay -->
                 {{ _('Snapshots supported by default webcam') }}<br/>
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/timelapse.py` & `OctoPrint-1.9.0rc4/src/octoprint/timelapse.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/translations/de/LC_MESSAGES/messages.mo` & `OctoPrint-1.9.0rc4/src/octoprint/translations/de/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: OctoPrint 1.8.0\n"
+"Project-Id-Version: OctoPrint 1.9.0\n"
 "Report-Msgid-Bugs-To: i18n@octoprint.org\n"
-"POT-Creation-Date: 2023-03-06 16:18+0100\n"
-"PO-Revision-Date: 2021-08-04 11:01+0200\n"
+"POT-Creation-Date: 2023-04-12 12:02+0200\n"
+"PO-Revision-Date: 2023-04-12 12:02+0200\n"
 "Last-Translator: Gina Häußge <gina@octoprint.org>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -217,14 +217,37 @@
 "\n"
 "                Der Server ist offline. Du kannst diesen Tab jetzt "
 "schließen.\n"
 "            "
 
 msgid ""
 "\n"
+"            <p>\n"
+"                Selects the webcam to use to take snapshots for the "
+"timelapse.\n"
+"            </p>\n"
+"            <p>\n"
+"                You can make changes to this webcam's configuration in its "
+"plugin settings, if it provides any.\n"
+"            </p>\n"
+"        "
+msgstr ""
+"\n"
+"            <p>\n"
+"                Wählt die Webcam aus, die für Timelapse-Snapshots verwendet "
+"wird.\n"
+"            </p>\n"
+"            <p>\n"
+"                Du kannst Änderungen an der Konfiguration dieser Webcam in "
+"ihren Plugineinstellungen vornehmen, so sie welche hat.\n"
+"            </p>\n"
+"        "
+
+msgid ""
+"\n"
 "            How do you want to proceed?\n"
 "        "
 msgstr ""
 "\n"
 "            Wie möchtest du fortfahren?\n"
 "        "
 
@@ -1260,14 +1283,49 @@
 msgstr ""
 "<p>OctoPrint kann externe Befehle aufrufen, um sich selbst neu zu starten "
 "oder das System, auf dem es läuft, neu zu starten und/oder herunterzufahren. "
 "Du kannst diese Befehle hier konfigurieren.</p>"
 
 msgid ""
 "<p>\n"
+"    Select the webcam to fall back to to populate the stream and snapshot "
+"URLs on the settings\n"
+"    API used by old clients that do not yet utilize the webcam plugin\n"
+"    system introduced in OctoPrint 1.9.0. If the selected webcam does not\n"
+"    provide a snapshot or stream URL, it won't be available on the settings "
+"API and thus\n"
+"    to older clients.\n"
+"</p>\n"
+"<p>\n"
+"    Note that this does not affect the webcam stream options available\n"
+"    in OctoPrint's core UI, nor the snapshot camera used for timelapse "
+"recordings.\n"
+"    It is exclusively relevant for the compatibility layer provided on the "
+"settings API.\n"
+"</p>"
+msgstr ""
+"<p>\n"
+"    Wählt die Webcam aus, die als Fallback für die Stream- und Snapshot-URLs "
+"auf der Settings-API verwendet werden soll, die von alten Clients verwendet "
+"wird, die das neue Webcam-Plugin-System von OctoPrint 1.9.0+ noch nicht "
+"unterstützen.\n"
+"    Falls die ausgewählte Webcam keine Snapshot- oder Stream-URL "
+"bereitstellt, wird sie nicht auf der Settings-API verfügbar sein und somit "
+"auch nicht für ältere Clients.\n"
+"</p>\n"
+"<p>\n"
+"    Beachte, dass diese Einstellung weder die Webcam-Stream-Optionen in "
+"OctoPrints Core-UI beeinflusst, noch die Snapshot-Kamera für "
+"Zeitrafferaufnahmen.\n"
+"    Sie ist ausschließlich relevant für die Kompatibilitäts-Schicht auf der "
+"Settings-API relevant.\n"
+"</p>"
+
+msgid ""
+"<p>\n"
 "    The <strong>Stream URL</strong> is the URL OctoPrint uses to embed the\n"
 "    actual webcam stream (which should be an MJPG stream) into the web\n"
 "    interface. This needs to be reachable <strong>from your browser</"
 "strong>.\n"
 "</p><p>\n"
 "    It may be\n"
 "    <ul>\n"
@@ -1474,14 +1532,34 @@
 "werden."
 
 msgid "A restart is needed for the changes to take effect."
 msgstr ""
 "Ein Neustart von OctoPrint ist notwendig, damit die Änderungen wirksam "
 "werden."
 
+msgid ""
+"A working snapshot setup and/or the path to FFMPEG are missing. To have this "
+"fixed, get in touch with an administrator of this OctoPrint instance."
+msgstr ""
+"Ein funktionierende Snapshot-Konfiguration und/oder the Pfad zu FFMPEG "
+"fehlen. Setz dich mit einem Administrator dieser OctoPrint-Instanz in "
+"Verbindung, um das korrigieren zu lassen."
+
+msgid ""
+"A working snapshot setup and/or the path to FFMPEG are missing. You can "
+"change both under \"Settings\" > \"Webcam & Timelapse\" and in the settings "
+"of your chosen webcam plugin. If you don't have a webcam or don't want to "
+"enable timelapse support you can also just disable it there."
+msgstr ""
+"Eine funktionierende Snapshot-Konfiguration und/oder the Pfad zu FFMPEG "
+"fehlen. Du kannst beide unter \"Einstellungen\" > \"Webcam & Zeitraffer\" "
+"und in den Einstellungen des gewählten Webcam-Plugins anpassen. Falls du "
+"keine Webcam hast oder Zeitrafferunterstützung nicht einschalten willst, "
+"kannst du beides auch dort abschalten."
+
 msgid "API"
 msgstr "API"
 
 msgid "API Key"
 msgstr "API Key"
 
 msgid "API error while checking for update, please check the logs"
@@ -2621,17 +2699,14 @@
 
 msgid "Default Language"
 msgstr "Standardsprache"
 
 msgid "Default Printer Profile"
 msgstr "Default Druckerprofil"
 
-msgid "Default Webcam"
-msgstr "Standard Webcam"
-
 msgid "Default extrusion length"
 msgstr "Standard Extrusionslänge"
 
 msgid "Default group"
 msgstr "Standardgruppe"
 
 msgid "Delete"
@@ -3096,32 +3171,35 @@
 msgstr "Zu nutzende FFMPEG Befehlszeile"
 
 msgid "FFMPEG threads"
 msgstr "FFMPEG Threads"
 
 msgid ""
 "Failed repeatedly to capture timelapse frame from webcam - is the snapshot "
-"URL configured correctly and the camera on?"
+"webcam configured correctly and the camera on?"
 msgstr ""
 "Konnte wiederholt kein Zeitrafferbild von der Webcam beziehen - ist die "
-"Snapshot-URL korrekt konfiguriert und die Kamera an?"
+"Snapshot-Webcam korrekt konfiguriert und die Kamera an?"
 
 msgid "Failed to remove entry"
 msgstr "Löschen fehlgeschlagen"
 
 msgid ""
 "Failed to remove timelapse %(name)s.</p><p>Please consult octoprint.log for "
 "details.</p>"
 msgstr ""
 "Konnte Zeitrafferaufnahme %(name)s nicht entfernen.</p><p>Bitte konsultiere "
 "octoprint.log für Details.</p>"
 
 msgid "Fake Acknowledgement"
 msgstr "Bestätigung faken"
 
+msgid "Fallback Webcam"
+msgstr "Fallback-Webcam"
+
 msgid "Fan off"
 msgstr "Lüfter aus"
 
 msgid "Fan on"
 msgstr "Lüfter an"
 
 msgid "Features"
@@ -3754,14 +3832,25 @@
 "It might not be configured correctly or require authentication. To have this "
 "fixed, get in touch with an administrator of this OctoPrint instance."
 msgstr ""
 "Es liegt evtl. eine Fehlkonfiguration vor oder es werden Logindaten "
 "benötigt. Um dies zu beheben wende dich bitte an einen Administrator dieser "
 "OctoPrint Instanz."
 
+msgid ""
+"It might not be configured correctly or require authentication. You can "
+"change the URL of the stream under \"Settings\" > \"Classic Webcam\" > "
+"\"Stream URL\". If you don't have a webcam you can also just disable webcam "
+"support there."
+msgstr ""
+"Es liegt evtl. eine Fehlkonfiguration vor oder es werden Logindaten "
+"benötigt. Du kannst die URL des Streams unter \"Einstellungen\" > "
+"\"Klassische Webcam\" > \"Stream-URL\" ändern. Falls du keine Webcam hast "
+"kannst du Webcam-Unterstützung dort auch deaktivieren."
+
 msgid "Keep data"
 msgstr "Daten behalten"
 
 msgid "Keep enabled"
 msgstr "Aktiviert lassen"
 
 msgid "Keep installed"
@@ -4938,14 +5027,21 @@
 msgid ""
 "Rendering of timelapse %(movie_prefix)s failed with return code "
 "%(returncode)s"
 msgstr ""
 "Rendering der Zeitrafferaufnahme %(movie_prefix)s fehlgeschlagen mit "
 "Returncode %(returncode)s"
 
+msgid ""
+"Rendering of timelapse %(movie_prefix)s is not possible since no frames were "
+"captured. Is the snapshot webcam configured correctly?"
+msgstr ""
+"Rendering des Zeitraffers %(movie_prefix)s ist nicht möglich, da keine "
+"Frames gespeichert wurden. Ist die Snapshot-Webcam korrekt konfiguriert?"
+
 msgid "Rendering timelapse"
 msgstr "Zeitrafferaufnahme wird gerendert"
 
 msgid "Rendering timelapse failed"
 msgstr "Rendern von Zeitrafferaufnahme fehlgeschlagen"
 
 msgid "RepRap Firmware"
@@ -5191,23 +5287,14 @@
 
 msgid "Select destination folder for "
 msgstr "Wähle Zielverzeichnis für "
 
 msgid "Select for printing"
 msgstr "Zum Drucken auswählen"
 
-msgid ""
-"Selects the default webcam. If this webcam provides a MJPEG video stream, it "
-"will be available for old clients that do not make use of the webcam plugin "
-"system introduced with OctoPrint 1.9.0"
-msgstr ""
-"Wählt die Standard Webcam aus. Wenn diese Webcam einen MJPEG Video Stream "
-"bietet, wird er für alte Clients verfügbar sein, die das Webcam Plugin "
-"System, das mit OctoPrint 1.9.0 eingeführt wurde, nicht nutzen."
-
 msgid "Send"
 msgstr "Senden"
 
 msgid "Send <code>M112</code> on disconnect due to error"
 msgstr "Sende <code>M112</code> bei fehlerbedingten Disconnects"
 
 msgid ""
@@ -5889,32 +5976,14 @@
 msgid "The server is reachable"
 msgstr "Der Server ist erreichbar"
 
 msgid "The snappy web interface for your 3D printer"
 msgstr "The snappy web interface for your 3D printer"
 
 msgid ""
-"The snapshot URL and/or the path to FFMPEG are missing. To have this fixed, "
-"get in touch with an administrator of this OctoPrint instance."
-msgstr ""
-"Die Snapshot-URL und/oder the Pfad zu FFMPEG fehlen. Setz dich mit einem "
-"Administrator dieser OctoPrint-Instanz in Verbindung, um das korrigieren zu "
-"lassen."
-
-msgid ""
-"The snapshot URL and/or the path to FFMPEG are missing. You can change both "
-"under \"Settings\" > \"Webcam & Timelapse\". If you don't have a webcam or "
-"don't want to enable timelapse support you can also just disable it there."
-msgstr ""
-"Die Snapshot-URL und/oder the Pfad zu FFMPEG fehlen. Du kannst beide unter "
-"\"Einstellungen\" > \"Webcam & Zeitraffer\" anpassen. Falls du keine Webcam "
-"hast oder Zeitrafferunterstützung nicht einschalten willst, kannst du beides "
-"auch dort abschalten."
-
-msgid ""
 "The update could not be started. Is it already active? Please consult "
 "octoprint.log for details."
 msgstr ""
 "Die Aktualisierung konnte nicht gestartet werden. Läuft bereits eine? Bitte "
 "konsultiere octoprint.log für Details."
 
 msgid ""
@@ -6776,14 +6845,17 @@
 
 msgid "Webcam & Timelapse"
 msgstr "Webcam & Zeitraffer"
 
 msgid "Webcam &amp; Timelapse Recordings"
 msgstr "Webcam &amp; Zeitrafferaufnahmen"
 
+msgid "Webcam Streaming"
+msgstr "Webcamstreaming"
+
 msgid "Webcam stream loading..."
 msgstr "Webcamstream lädt..."
 
 msgid "Webcam stream not loaded"
 msgstr "Webcamstream nicht geladen"
 
 msgid "What to do on a firmware error (<code>Error:</code> or <code>!!</code>)"
@@ -7034,18 +7106,14 @@
 "Benachrichtigungen konfigurieren."
 
 msgid "You can find more info on this issue in the FAQ at %(url)s"
 msgstr ""
 "Du kannst weitere Information zu diesem Problem in der FAQ unter %(url)s "
 "finden"
 
-msgid "You can make changes to this webcam in the plugin's settings."
-msgstr ""
-"Du kannst Änderungen an dieser Webcam in den Plugineinstellungen vornehmen."
-
 msgid ""
 "You can make this message display again via \"Settings\" > \"Software "
 "Update\" > \"Check for update now\""
 msgstr ""
 "Du kannst diese Nachricht erneut anzeigen lassen mittels \"Einstellungen\" > "
 "\"Software Update\" > \"Jetzt nach Aktualisierungen suchen\""
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/translations/de/LC_MESSAGES/messages.po` & `OctoPrint-1.9.0rc4/src/octoprint/translations/de/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # German translations for OctoPrint.
 # Copyright (C) 2017-2021 The OctoPrint Project
 # This file is distributed under the same license as the OctoPrint project.
 msgid ""
 msgstr ""
-"Project-Id-Version: OctoPrint 1.8.0\n"
+"Project-Id-Version: OctoPrint 1.9.0\n"
 "Report-Msgid-Bugs-To: i18n@octoprint.org\n"
-"POT-Creation-Date: 2023-03-06 16:18+0100\n"
-"PO-Revision-Date: 2021-08-04 11:01+0200\n"
+"POT-Creation-Date: 2023-04-12 12:02+0200\n"
+"PO-Revision-Date: 2023-04-12 12:02+0200\n"
 "Last-Translator: Gina Häußge <gina@octoprint.org>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -129,15 +129,17 @@
 
 #: src/octoprint/access/permissions.py:417
 msgid "Allows to delete timelapse videos"
 msgstr "Erlaubt das Löschen von Zeitrafferaufnahmen"
 
 #: src/octoprint/access/permissions.py:423
 msgid "Allows to list, delete and render unrendered timelapses"
-msgstr "Erlaubt die Auflistung, das Löschen und Rendern von ungerenderte Zeitrafferaufnahmen"
+msgstr ""
+"Erlaubt die Auflistung, das Löschen und Rendern von ungerenderte "
+"Zeitrafferaufnahmen"
 
 #: src/octoprint/access/permissions.py:429
 msgid "Allows to change the timelapse settings."
 msgstr "Erlaubt die Änderung von Zeitraffereinstellungen"
 
 #: src/octoprint/access/permissions.py:436
 msgid ""
@@ -266,15 +268,15 @@
 #: src/octoprint/plugins/classicwebcam/templates/classicwebcam_settings.jinja2:9
 #: src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_tab.jinja2:79
 #: src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2:356
 #: src/octoprint/templates/dialogs/settings/serialconnection.jinja2:96
 #: src/octoprint/templates/dialogs/settings/serialconnection.jinja2:237
 #: src/octoprint/templates/dialogs/settings/serialconnection.jinja2:370
 #: src/octoprint/templates/dialogs/settings/serialconnection.jinja2:506
-#: src/octoprint/templates/dialogs/settings/webcam.jinja2:21
+#: src/octoprint/templates/dialogs/settings/webcam.jinja2:20
 #: src/octoprint/templates/snippets/settings/server/serverPluginBlacklist.jinja2:5
 #: src/octoprint/templates/tabs/terminal.jinja2:35
 msgid "Advanced options"
 msgstr "Erweiterte Optionen"
 
 #: src/octoprint/plugins/action_command_prompt/templates/action_command_prompt_settings.jinja2:22
 msgid "Dialog command"
@@ -446,25 +448,25 @@
 msgstr "Erlaubt Zugriffsgewährung für Apps"
 
 #: src/octoprint/plugins/appkeys/__init__.py:142
 #: src/octoprint/plugins/appkeys/__init__.py:143
 msgid "Application Keys"
 msgstr "Application Keys"
 
-#: src/octoprint/plugins/appkeys/__init__.py:254
+#: src/octoprint/plugins/appkeys/__init__.py:256
 #: src/octoprint/plugins/appkeys/static/js/appkeys.js:115
 #, python-format
 msgid ""
 "\"<strong>%(app)s</strong>\" has requested access to control OctoPrint "
 "through the API."
 msgstr ""
 "\"<strong>%(app)s</strong>\" möchte Zugriff auf OctoPrint über die API "
 "haben."
 
-#: src/octoprint/plugins/appkeys/__init__.py:543
+#: src/octoprint/plugins/appkeys/__init__.py:545
 msgid ""
 "Without this plugin third party clients will no longer be able to obtain "
 "an API key without you manually copy-pasting it."
 msgstr ""
 "Ohne dieses Plugin können Third Party Clients keine API Keys mehr "
 "erlangen, ohne dass du sie manuell übertragen musst."
 
@@ -1047,17 +1049,18 @@
 
 #: src/octoprint/plugins/classicwebcam/__init__.py:243
 msgid ""
 "This plugin provides the standard webcam in OctoPrint. If you do not have"
 " any other plugin providing a webcam set up, the webcam section in the "
 "control tab will no longer be visible."
 msgstr ""
-"Dieses Plugin stellt die klassische Webcam in OctoPrint zur Verfügung. Falls du"
-" keine anderen Plugins installiert hast, die eine Webcam bereitstellen,"
-" wird die Webcam-Sektion im Kontroll-Tab nicht mehr angezeigt."
+"Dieses Plugin stellt die klassische Webcam in OctoPrint zur Verfügung. "
+"Falls du keine anderen Plugins installiert hast, die eine Webcam "
+"bereitstellen, wird die Webcam-Sektion im Kontroll-Tab nicht mehr "
+"angezeigt."
 
 #: src/octoprint/plugins/classicwebcam/static/js/classicwebcam_settings.js:77
 msgid "If you see your webcam stream below, the entered stream URL is ok."
 msgstr "Falls du unten den Webcamstream sehen kannst, ist die Stream-URL ok."
 
 #: src/octoprint/plugins/classicwebcam/static/js/classicwebcam_settings.js:126
 msgid "Stream test"
@@ -1116,25 +1119,24 @@
 "instance."
 msgstr ""
 "Es liegt evtl. eine Fehlkonfiguration vor oder es werden Logindaten "
 "benötigt. Um dies zu beheben wende dich bitte an einen Administrator "
 "dieser OctoPrint Instanz."
 
 #: src/octoprint/plugins/classicwebcam/templates/classicwebcam_webcam.jinja2:35
-#, fuzzy
 msgid ""
 "It might not be configured correctly or require authentication. You can "
 "change the URL of the stream under \"Settings\" > \"Classic Webcam\" > "
 "\"Stream URL\". If you don't have a webcam you can also just disable "
 "webcam support there."
 msgstr ""
 "Es liegt evtl. eine Fehlkonfiguration vor oder es werden Logindaten "
 "benötigt. Du kannst die URL des Streams unter \"Einstellungen\" > "
-"\"Klassische Webcam\" > \"Stream-URL\" ändern. Falls du "
-"keine Webcam hast kannst du Webcam-Unterstützung dort auch deaktivieren."
+"\"Klassische Webcam\" > \"Stream-URL\" ändern. Falls du keine Webcam hast"
+" kannst du Webcam-Unterstützung dort auch deaktivieren."
 
 #: src/octoprint/plugins/classicwebcam/templates/classicwebcam_webcam.jinja2:36
 msgid "Currently configured stream URL"
 msgstr "Aktuell konfigurierte Stream-URL"
 
 #: src/octoprint/plugins/classicwebcam/templates/classicwebcam_wizard.jinja2:1
 msgid "Webcam &amp; Timelapse Recordings"
@@ -1144,15 +1146,14 @@
 msgid ""
 "<p>\n"
 "    If you have a webcam, you may now configure it here.\n"
 "</p>"
 msgstr "<p>Falls du eine Webcam hast kannst du diese nun hier konfigurieren.</p>"
 
 #: src/octoprint/plugins/classicwebcam/templates/classicwebcam_wizard.jinja2:7
-#: src/octoprint/templates/dialogs/settings/webcam.jinja2:5
 msgid "Webcam"
 msgstr "Webcam"
 
 #: src/octoprint/plugins/classicwebcam/templates/classicwebcam_wizard.jinja2:9
 msgid ""
 "<p>\n"
 "    The <strong>Stream URL</strong> is the URL OctoPrint uses to embed "
@@ -1357,15 +1358,15 @@
 #: src/octoprint/plugins/corewizard/subwizards.py:37
 #: src/octoprint/plugins/corewizard/templates/corewizard_servercommands_wizard.jinja2:1
 msgid "Server Commands"
 msgstr "Serverbefehle"
 
 #: src/octoprint/plugins/corewizard/subwizards.py:52
 #: src/octoprint/plugins/corewizard/templates/corewizard_acl_wizard.jinja2:1
-#: src/octoprint/server/views.py:1101
+#: src/octoprint/server/views.py:1108
 #: src/octoprint/templates/dialogs/settings/accesscontrol.jinja2:1
 msgid "Access Control"
 msgstr "Zugangsbeschränkung"
 
 #: src/octoprint/plugins/corewizard/subwizards.py:104
 msgid "Online Connectivity Check"
 msgstr "Onlineprüfung"
@@ -1687,15 +1688,15 @@
 "Druckerprofile unter Einstellungen > Druckerprofile konfigurieren"
 
 #: src/octoprint/plugins/corewizard/templates/corewizard_printerprofile_wizard.jinja2:7
 #: src/octoprint/templates/dialogs/settings/serialconnection.jinja2:7
 #: src/octoprint/templates/snippets/settings/accesscontrol/groups.jinja2:60
 #: src/octoprint/templates/snippets/settings/accesscontrol/users.jinja2:70
 #: src/octoprint/templates/snippets/settings/printerprofiles/profileEditor.jinja2:9
-#: src/octoprint/templates/tabs/control.jinja2:147
+#: src/octoprint/templates/tabs/control.jinja2:144
 msgid "General"
 msgstr "Allgemein"
 
 #: src/octoprint/plugins/corewizard/templates/corewizard_printerprofile_wizard.jinja2:8
 #: src/octoprint/templates/snippets/settings/printerprofiles/profileEditor.jinja2:10
 msgid "Print bed & build volume"
 msgstr "Druckbett & -volumen"
@@ -1959,66 +1960,66 @@
 msgid "Analyzing..."
 msgstr "Analysiere..."
 
 #: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:36
 msgid "Ready!"
 msgstr "Fertig!"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:692
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:694
 #: src/octoprint/static/js/app/viewmodels/files.js:1066
 msgid "Model size"
 msgstr "Modelgröße"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:702
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:704
 msgid "Estimated layer height"
 msgstr "Geschätzte Schichthöhe"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:705
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:707
 #: src/octoprint/templates/tabs/timelapse.jinja2:69
 msgid "mm"
 msgstr "mm"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:708
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:710
 msgid "Estimated total print time"
 msgstr "Geschätzte Gesamtdauer"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:713
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:715
 msgid "Layers with extrusion"
 msgstr "Layer mit Extrusion"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:746
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:748
 msgid "Layer number"
 msgstr "Schichtnummer"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:747
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:749
 msgid "Layer height"
 msgstr "Schichthöhe"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:748
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:750
 msgid "GCODE commands"
 msgstr "GCODE Befehle"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:752
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:761
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:754
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:763
 #: src/octoprint/static/js/app/viewmodels/files.js:1081
 #: src/octoprint/static/js/app/viewmodels/files.js:1097
 msgid "Filament"
 msgstr "Filament"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:763
-#: src/octoprint/static/js/app/viewmodels/control.js:141
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:765
+#: src/octoprint/static/js/app/viewmodels/control.js:171
 #: src/octoprint/static/js/app/viewmodels/files.js:1099
 #: src/octoprint/static/js/app/viewmodels/printerstate.js:357
 #: src/octoprint/static/js/app/viewmodels/temperature.js:147
 #: src/octoprint/static/js/app/viewmodels/temperature.js:158
 #: src/octoprint/static/js/app/viewmodels/temperature.js:394
 msgid "Tool"
 msgstr "Tool"
 
-#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:775
+#: src/octoprint/plugins/gcodeviewer/static/js/gcodeviewer.js:777
 #: src/octoprint/static/js/app/viewmodels/files.js:1109
 msgid "Estimated print time"
 msgstr "Geschätzte Dauer"
 
 #: src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_settings.jinja2:3
 msgid "Skip/hide gcode until this string"
 msgstr "GCODE bis zu diesem String überspringen"
@@ -2078,17 +2079,18 @@
 "\n"
 "            In-memory model compression can help in reducing the memory "
 "consumption of the GCode Viewer and thus enable processing of files that "
 "would be too large to view otherwise.\n"
 "        "
 msgstr ""
 "\n"
-"            In-memory Modell-Kompression kann helfen, den Speicherverbrauch"
-" des GCode Viewers zu reduzieren und somit die Verarbeitung von Dateien zu"
-" ermöglichen, die ansonsten dafür zu groß wären.\n"
+"            In-memory Modell-Kompression kann helfen, den "
+"Speicherverbrauch des GCode Viewers zu reduzieren und somit die "
+"Verarbeitung von Dateien zu ermöglichen, die ansonsten dafür zu groß "
+"wären.\n"
 "        "
 
 #: src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_settings.jinja2:36
 msgid "Always enable compression"
 msgstr "Kompression immer aktivieren"
 
 #: src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_settings.jinja2:38
@@ -2106,19 +2108,19 @@
 #: src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_settings.jinja2:47
 msgid ""
 "If this is non-zero, the GCode Viewer will always use in-memory "
 "compression for GCode files if they exceed this size. Provide values "
 "including size unit. Allowed units are: b, byte, bytes, kb, mb, gb, tb "
 "(case insensitive). Example: <code>5MB</code>, <code>500KB</code>"
 msgstr ""
-"Falls nicht 0, wird der GCode Viewer immer die In-memory Kompression "
-"der Schichtdaten aktivieren, wenn die Datei größer als dieser Wert ist. "
-"Wert inklusive Größeneinheit. Erlaubte Einheiten sind: b, byte, bytes, "
-"kb, mb, gb, tb (Groß-/Kleinschreibung irrelevant). Beispiel: "
-"<code>5MB</code>, <code>500KB</code>"
+"Falls nicht 0, wird der GCode Viewer immer die In-memory Kompression der "
+"Schichtdaten aktivieren, wenn die Datei größer als dieser Wert ist. Wert "
+"inklusive Größeneinheit. Erlaubte Einheiten sind: b, byte, bytes, kb, mb,"
+" gb, tb (Groß-/Kleinschreibung irrelevant). Beispiel: <code>5MB</code>, "
+"<code>500KB</code>"
 
 #: src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_tab.jinja2:11
 msgid "Previous layer"
 msgstr "Vorherige Schicht"
 
 #: src/octoprint/plugins/gcodeviewer/templates/gcodeviewer_tab.jinja2:14
 msgid "Next layer"
@@ -2531,22 +2533,24 @@
 #: src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js:501
 #: src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js:617
 msgid "Confirm installation of multiple plugins"
 msgstr "Bestätige Installation mehrerer Plugins"
 
 #: src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js:502
 msgid "Please confirm you want to perform all plugins specified in the json file."
-msgstr "Bitte bestätige, dass du alle Plugins aus der JSON-Datei installieren möchtest."
+msgstr ""
+"Bitte bestätige, dass du alle Plugins aus der JSON-Datei installieren "
+"möchtest."
 
 #: src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js:505
 #: src/octoprint/plugins/pluginmanager/static/js/pluginmanager.js:620
 #: src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2:458
 #: src/octoprint/plugins/softwareupdate/templates/softwareupdate_settings.jinja2:205
 #: src/octoprint/static/js/app/helpers.js:816
-#: src/octoprint/static/js/app/viewmodels/temperature.js:515
+#: src/octoprint/static/js/app/viewmodels/temperature.js:518
 #: src/octoprint/templates/dialogs/files.jinja2:18
 #: src/octoprint/templates/dialogs/files.jinja2:48
 #: src/octoprint/templates/dialogs/files.jinja2:78
 #: src/octoprint/templates/dialogs/slicing.jinja2:57
 #: src/octoprint/templates/dialogs/temperature.jinja2:31
 #: src/octoprint/templates/sidebar/state.jinja2:31
 msgid "Cancel"
@@ -3108,15 +3112,15 @@
 msgstr ""
 "\n"
 "    Es gab einen Fehler beim Abruf der Plugindaten vom Backend. Bitte "
 "melde dies im\n"
 "    Bugtracker mit allen erbetenen Logs.\n"
 
 #: src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2:47
-#: src/octoprint/server/views.py:867
+#: src/octoprint/server/views.py:874
 msgid "Plugins"
 msgstr "Plugins"
 
 #: src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2:50
 #: src/octoprint/plugins/pluginmanager/templates/pluginmanager_settings.jinja2:177
 msgid "Cleanup"
 msgstr "Löschen"
@@ -3568,15 +3572,15 @@
 
 #: src/octoprint/plugins/softwareupdate/__init__.py:1498
 #: src/octoprint/plugins/softwareupdate/templates/softwareupdate_wizard_update.jinja2:1
 msgid "Update?"
 msgstr "Aktualisieren?"
 
 #: src/octoprint/plugins/softwareupdate/__init__.py:2340
-#: src/octoprint/server/views.py:1099
+#: src/octoprint/server/views.py:1106
 #: src/octoprint/static/js/app/viewmodels/appearance.js:106
 #: src/octoprint/static/js/app/viewmodels/appearance.js:110
 #: src/octoprint/static/js/app/viewmodels/appearance.js:111
 #: src/octoprint/static/js/app/viewmodels/appearance.js:115
 #: src/octoprint/static/js/app/viewmodels/appearance.js:116
 #: src/octoprint/templates/dialogs/about/about.jinja2:1
 #: src/octoprint/templates/footer.jinja2:3
@@ -4352,16 +4356,16 @@
 
 #: src/octoprint/plugins/softwareupdate/templates/snippets/githubToken.jinja2:14
 #, fuzzy
 msgid ""
 "Please note that the deletion of the access token is applied immediately,"
 " without having to \"Confirm\" first."
 msgstr ""
-"Bitte beachte, dass das Löschen des Access Tokens sofort angewandt wird, ohne "
-"dass \"Bestätigen\" geklickt werden muss."
+"Bitte beachte, dass das Löschen des Access Tokens sofort angewandt wird, "
+"ohne dass \"Bestätigen\" geklickt werden muss."
 
 #: src/octoprint/plugins/softwareupdate/templates/snippets/pipEnableCheck.jinja2:4
 msgid "Enable <code>pip</code> update checks"
 msgstr "<code>pip</code> Updatechecks aktivieren"
 
 #: src/octoprint/plugins/softwareupdate/templates/snippets/pipEnableCheck.jinja2:5
 msgid ""
@@ -4609,115 +4613,115 @@
 "available for connecting, backed by a fake printer implementation. Useful"
 " for development."
 msgstr ""
 "Wenn aktiviert, so wird ein zusätzlicher Serialport <code>VIRTUAL</code> "
 "zur Verbindung zur Verfügung gestellt, mit einer Fake-"
 "Druckerimplementierung. Sinnvoll für die Entwicklung."
 
-#: src/octoprint/server/views.py:955
+#: src/octoprint/server/views.py:962
 #: src/octoprint/templates/dialogs/settings/serialconnection.jinja2:16
 msgid "Connection"
 msgstr "Verbindung"
 
-#: src/octoprint/server/views.py:966
+#: src/octoprint/server/views.py:973
 #: src/octoprint/templates/sidebar/state.jinja2:1
 msgid "State"
 msgstr "Status"
 
-#: src/octoprint/server/views.py:976
+#: src/octoprint/server/views.py:983
 msgid "Files"
 msgstr "Dateien"
 
-#: src/octoprint/server/views.py:993
+#: src/octoprint/server/views.py:1000
 msgid "Temperature"
 msgstr "Temperatur"
 
-#: src/octoprint/server/views.py:1002
+#: src/octoprint/server/views.py:1009
 msgid "Control"
 msgstr "Steuerung"
 
-#: src/octoprint/server/views.py:1011
+#: src/octoprint/server/views.py:1018
 msgid "Terminal"
 msgstr "Terminal"
 
-#: src/octoprint/server/views.py:1020
+#: src/octoprint/server/views.py:1027
 #: src/octoprint/templates/sidebar/state.jinja2:11
 msgid "Timelapse"
 msgstr "Zeitraffer"
 
-#: src/octoprint/server/views.py:1033
+#: src/octoprint/server/views.py:1040
 msgid "Printer"
 msgstr "Drucker"
 
-#: src/octoprint/server/views.py:1035
+#: src/octoprint/server/views.py:1042
 msgid "Serial Connection"
 msgstr "Serielle Verbindung"
 
-#: src/octoprint/server/views.py:1043
+#: src/octoprint/server/views.py:1050
 #: src/octoprint/templates/dialogs/settings/printerprofiles.jinja2:1
 msgid "Printer Profiles"
 msgstr "Druckerprofile"
 
-#: src/octoprint/server/views.py:1051
+#: src/octoprint/server/views.py:1058
 msgid "Temperatures"
 msgstr "Temperaturen"
 
-#: src/octoprint/server/views.py:1059
+#: src/octoprint/server/views.py:1066
 #: src/octoprint/templates/dialogs/settings/terminalfilters.jinja2:1
 msgid "Terminal Filters"
 msgstr "Terminalfilter"
 
-#: src/octoprint/server/views.py:1067
+#: src/octoprint/server/views.py:1074
 #: src/octoprint/templates/dialogs/settings/gcodescripts.jinja2:1
 msgid "GCODE Scripts"
 msgstr "GCODE Scripts"
 
-#: src/octoprint/server/views.py:1074 src/octoprint/server/views.py:1076
+#: src/octoprint/server/views.py:1081 src/octoprint/server/views.py:1083
 #: src/octoprint/templates/dialogs/settings/features.jinja2:1
 msgid "Features"
 msgstr "Funktionen"
 
-#: src/octoprint/server/views.py:1084
+#: src/octoprint/server/views.py:1091
 msgid "Webcam & Timelapse"
 msgstr "Webcam & Zeitraffer"
 
-#: src/octoprint/server/views.py:1092
+#: src/octoprint/server/views.py:1099
 msgid "API"
 msgstr "API"
 
-#: src/octoprint/server/views.py:1109
+#: src/octoprint/server/views.py:1116
 #: src/octoprint/templates/dialogs/settings/folders.jinja2:2
 #: src/octoprint/templates/sidebar/files_header.jinja2:13
 msgid "Folders"
 msgstr "Verzeichnisse"
 
-#: src/octoprint/server/views.py:1117
+#: src/octoprint/server/views.py:1124
 #: src/octoprint/templates/dialogs/settings/appearance.jinja2:1
 msgid "Appearance"
 msgstr "Aussehen"
 
-#: src/octoprint/server/views.py:1125
+#: src/octoprint/server/views.py:1132
 #: src/octoprint/templates/dialogs/settings/server.jinja2:1
 msgid "Server"
 msgstr "Server"
 
-#: src/octoprint/server/views.py:1138
+#: src/octoprint/server/views.py:1145
 msgid "Access"
 msgstr "Zugriff"
 
-#: src/octoprint/server/views.py:1146
+#: src/octoprint/server/views.py:1153
 msgid "Interface"
 msgstr "Interface"
 
-#: src/octoprint/server/views.py:1176
-#: src/octoprint/static/js/app/viewmodels/temperature.js:513
+#: src/octoprint/server/views.py:1183
+#: src/octoprint/static/js/app/viewmodels/temperature.js:516
 msgid "Start"
 msgstr "Start"
 
-#: src/octoprint/server/views.py:1183
+#: src/octoprint/server/views.py:1190
 #: src/octoprint/templates/dialogs/wizard.jinja2:57
 msgid "Finish"
 msgstr "Beenden"
 
 #: src/octoprint/server/api/system.py:237
 #: src/octoprint/templates/snippets/settings/server/serverCommandSystemShutdown.jinja2:2
 msgid "Shutdown system"
@@ -5244,15 +5248,15 @@
 msgid "Are you sure you want to disconnect from the printer?"
 msgstr "Bist Du sicher, dass du die Verbindung zum Drucker trennen willst?"
 
 #: src/octoprint/static/js/app/viewmodels/connection.js:200
 msgid "Stay Connected"
 msgstr "Verbunden bleiben"
 
-#: src/octoprint/static/js/app/viewmodels/control.js:147
+#: src/octoprint/static/js/app/viewmodels/control.js:177
 msgid "Hotend"
 msgstr "Hotend"
 
 #: src/octoprint/static/js/app/viewmodels/files.js:56
 msgid "Your available free disk space is critically low."
 msgstr "Dein verfügbarer freier Plattenplatz ist auf einem kritischen Tiefstand."
 
@@ -5349,14 +5353,15 @@
 msgstr "Zuletzt gedruckt"
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1129
 msgid "Last print time"
 msgstr "Letzte Dauer"
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1208
+#, python-format
 msgid "%(culprit)s exceeds print volume in %(dimension)s.<br>"
 msgstr "%(culprit)st überschreitet Druckvolumen in %(dimension)s.<br>"
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1215
 #: src/octoprint/static/js/app/viewmodels/files.js:1219
 #: src/octoprint/static/js/app/viewmodels/files.js:1223
 msgid "Object"
@@ -5409,22 +5414,24 @@
 "%(profile.maxZ).2f)"
 msgstr ""
 "Druckvolumen: (%(profile.minX).2f, %(profile.minY).2f, "
 "%(profile.minZ).2f) &times; (%(profile.maxX).2f, %(profile.maxY).2f, "
 "%(profile.maxZ).2f)"
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1279
+#, python-format
 msgid ""
 "%(culprit)s in %(name)s exceeds the print volume of the currently "
 "selected printer profile, be careful when printing this."
 msgstr ""
-"%(culprit)s in %(name)s überschreitet das Druckvolumen des aktuell gewählten "
-"Druckerprofils, sei vorsichtig, das zu drucken."
+"%(culprit)s in %(name)s überschreitet das Druckvolumen des aktuell "
+"gewählten Druckerprofils, sei vorsichtig, das zu drucken."
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1294
+#, python-format
 msgid "%(culprit)s exceeds print volume"
 msgstr "%(culprit)s überschreitet Druckvolumen"
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1486
 msgid "Slicing ..."
 msgstr "Slice ..."
 
@@ -5471,15 +5478,17 @@
 #: src/octoprint/static/js/app/viewmodels/files.js:1692
 #, python-format
 msgid "File already exists: %(name)s"
 msgstr "Datei existiert bereits: %(name)s"
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1777
 msgid "Could not upload the file. There is not enough disk space remaining."
-msgstr "Konnte die Datei nicht hochladen. Es steht nicht genug Speicherplatz zur Verfügung."
+msgstr ""
+"Konnte die Datei nicht hochladen. Es steht nicht genug Speicherplatz zur "
+"Verfügung."
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1784
 #, python-format
 msgid "Free Space: %(freespace)s"
 msgstr "Freier Speicher: %(freespace)s"
 
 #: src/octoprint/static/js/app/viewmodels/files.js:1788
@@ -5804,15 +5813,15 @@
 msgstr "Basiert auf der berechneten Schätzung (beste Genauigkeit)"
 
 #: src/octoprint/static/js/app/viewmodels/printerstate.js:224
 msgid "Continue"
 msgstr "Fortsetzen"
 
 #: src/octoprint/static/js/app/viewmodels/printerstate.js:225
-#: src/octoprint/static/js/app/viewmodels/temperature.js:516
+#: src/octoprint/static/js/app/viewmodels/temperature.js:519
 #: src/octoprint/templates/sidebar/state.jinja2:30
 msgid "Pause"
 msgstr "Pause"
 
 #: src/octoprint/static/js/app/viewmodels/printerstate.js:235
 #: src/octoprint/templates/tabs/timelapse.jinja2:16
 msgid "On Z Change"
@@ -6015,33 +6024,33 @@
 #: src/octoprint/static/js/app/viewmodels/temperature.js:386
 #: src/octoprint/templates/tabs/temperature.jinja2:30
 #: src/octoprint/templates/tabs/temperature.jinja2:68
 #: src/octoprint/templates/tabs/timelapse.jinja2:14
 msgid "Off"
 msgstr "Aus"
 
-#: src/octoprint/static/js/app/viewmodels/temperature.js:514
+#: src/octoprint/static/js/app/viewmodels/temperature.js:517
 msgid "Done"
 msgstr "Fertig"
 
-#: src/octoprint/static/js/app/viewmodels/temperature.js:517
+#: src/octoprint/static/js/app/viewmodels/temperature.js:520
 #: src/octoprint/templates/sidebar/state.jinja2:30
 msgid "Resume"
 msgstr "Weiter"
 
-#: src/octoprint/static/js/app/viewmodels/temperature.js:560
+#: src/octoprint/static/js/app/viewmodels/temperature.js:563
 msgid "min"
 msgstr "Min"
 
-#: src/octoprint/static/js/app/viewmodels/temperature.js:624
+#: src/octoprint/static/js/app/viewmodels/temperature.js:627
 #: src/octoprint/templates/tabs/temperature.jinja2:23
 msgid "Actual"
 msgstr "Ist"
 
-#: src/octoprint/static/js/app/viewmodels/temperature.js:634
+#: src/octoprint/static/js/app/viewmodels/temperature.js:637
 #: src/octoprint/templates/tabs/temperature.jinja2:25
 msgid "Target"
 msgstr "Soll"
 
 #: src/octoprint/static/js/app/viewmodels/terminal.js:109
 #, python-format
 msgid ""
@@ -6188,18 +6197,18 @@
 msgstr ""
 "Zeichne jetzt Zeitraffernachlauf auf, dies wird voraussichtlich "
 "%(duration)s dauern..."
 
 #: src/octoprint/static/js/app/viewmodels/timelapse.js:712
 msgid ""
 "Failed repeatedly to capture timelapse frame from webcam - is the "
-"snapshot URL configured correctly and the camera on?"
+"snapshot webcam configured correctly and the camera on?"
 msgstr ""
 "Konnte wiederholt kein Zeitrafferbild von der Webcam beziehen - ist die "
-"Snapshot-URL korrekt konfiguriert und die Kamera an?"
+"Snapshot-Webcam korrekt konfiguriert und die Kamera an?"
 
 #: src/octoprint/static/js/app/viewmodels/timelapse.js:738
 msgid "Could not capture snapshots"
 msgstr "Konnte keine Snapshots aufnehmen"
 
 #: src/octoprint/static/js/app/viewmodels/timelapse.js:747
 msgid "Rendering timelapse"
@@ -6216,21 +6225,21 @@
 "so lange die Aufnahme noch gerendert wird."
 
 #: src/octoprint/static/js/app/viewmodels/timelapse.js:771
 msgid "Cannot render timelapse"
 msgstr "Kann Zeitrafferaufnahme nicht rendern"
 
 #: src/octoprint/static/js/app/viewmodels/timelapse.js:775
-#, fuzzy, python-format
+#, python-format
 msgid ""
 "Rendering of timelapse %(movie_prefix)s is not possible since no frames "
-"were captured. Is the webcam configured correctly?"
+"were captured. Is the snapshot webcam configured correctly?"
 msgstr ""
 "Rendering des Zeitraffers %(movie_prefix)s ist nicht möglich, da keine "
-"Frames gespeichert wurden. Ist die Snapshot-URL korrekt konfiguriert?"
+"Frames gespeichert wurden. Ist die Snapshot-Webcam korrekt konfiguriert?"
 
 #: src/octoprint/static/js/app/viewmodels/timelapse.js:782
 #: src/octoprint/static/js/app/viewmodels/timelapse.js:799
 msgid "Rendering timelapse failed"
 msgstr "Rendern von Zeitrafferaufnahme fehlgeschlagen"
 
 #: src/octoprint/static/js/app/viewmodels/timelapse.js:786
@@ -7849,16 +7858,16 @@
 "Handshake Versuche zu antworten."
 
 #: src/octoprint/templates/dialogs/settings/serialconnection.jinja2:465
 msgid ""
 "Wait to load the SD card file list until the firmware capability report "
 "is processed."
 msgstr ""
-"Warte mit dem Laden der SD-Karten Dateiliste, bis der Firmware "
-"Capability Report verarbeitet wurde."
+"Warte mit dem Laden der SD-Karten Dateiliste, bis der Firmware Capability"
+" Report verarbeitet wurde."
 
 #: src/octoprint/templates/dialogs/settings/serialconnection.jinja2:466
 msgid ""
 "Try checking this if the SD card file list loads improperly after "
 "connecting to the printer."
 msgstr "Deaktiviere das, falls die SD-Karten Dateiliste fehlerhaft geladen wird."
 
@@ -8279,18 +8288,64 @@
 "Bitte beachte, dass OctoPrint den Webcam Stream lediglich einbettet und "
 "die Snapshot URL lediglich abruft. Es beinhaltet keinen eigenen "
 "Webcamserver oder interagiert sonstwie direkt mit deiner Kamera. Es kann "
 "keine Zugriffbeschränkungen auf die Kamera forcieren oder den Stream "
 "ein-/ausschalten. Bitte konsultiere <a href=\"%(url)s\" "
 "target=\"_blank\">diesen FAQ Eintrag</a> für weitere Erläuterungen."
 
-#: src/octoprint/templates/dialogs/settings/webcam.jinja2:12
+#: src/octoprint/templates/dialogs/settings/webcam.jinja2:5
+msgid "Webcam Streaming"
+msgstr "Webcamstreaming"
+
+#: src/octoprint/templates/dialogs/settings/webcam.jinja2:11
 msgid "Timelapse Recordings"
 msgstr "Zeitrafferaufnahmen"
 
+#: src/octoprint/templates/dialogs/settings/webcam.jinja2:32
+#: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:1
+#: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:2
+msgid "Fallback Webcam"
+msgstr "Fallback-Webcam"
+
+#: src/octoprint/templates/dialogs/settings/webcam.jinja2:34
+msgid ""
+"<p>\n"
+"    Select the webcam to fall back to to populate the stream and snapshot"
+" URLs on the settings\n"
+"    API used by old clients that do not yet utilize the webcam plugin\n"
+"    system introduced in OctoPrint 1.9.0. If the selected webcam does not"
+"\n"
+"    provide a snapshot or stream URL, it won't be available on the "
+"settings API and thus\n"
+"    to older clients.\n"
+"</p>\n"
+"<p>\n"
+"    Note that this does not affect the webcam stream options available\n"
+"    in OctoPrint's core UI, nor the snapshot camera used for timelapse "
+"recordings.\n"
+"    It is exclusively relevant for the compatibility layer provided on "
+"the settings API.\n"
+"</p>"
+msgstr ""
+"<p>\n"
+"    Wählt die Webcam aus, die als Fallback für die Stream- und Snapshot-URLs"
+" auf der Settings-API verwendet werden soll, die von alten Clients verwendet"
+" wird, die das neue Webcam-Plugin-System von OctoPrint 1.9.0+ noch nicht unterstützen.\n"
+"    Falls die ausgewählte Webcam keine Snapshot- oder Stream-URL bereitstellt,"
+" wird sie nicht auf der Settings-API verfügbar sein und somit auch nicht für"
+" ältere Clients.\n"
+"</p>\n"
+"<p>\n"
+"    Beachte, dass diese Einstellung weder die Webcam-Stream-Optionen in OctoPrints Core-UI"
+" beeinflusst, noch die Snapshot-Kamera für Zeitrafferaufnahmen.\n"
+"    Sie ist ausschließlich relevant für die Kompatibilitäts-Schicht auf der Settings-API relevant.\n"
+"</p>"
+
+
+
 #: src/octoprint/templates/dialogs/usersettings/access.jinja2:5
 msgid ""
 "If you do not wish to change your password, just leave the following "
 "fields empty."
 msgstr ""
 "Falls Du Dein Passwort nicht ändern willst, lass die folgenden Felder "
 "leer."
@@ -9227,41 +9282,32 @@
 " performance issues observed outside of safe mode."
 msgstr ""
 "Dies kann zwar die Performance negativ beeinflussen, ein "
 "<code>plugintimings.log</code> ist jedoch unglaublich nützlich beim "
 "Debugging jeglicher Performanceprobleme, die außerhalb von Safemode "
 "beobachtet werden."
 
-#: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:2
-msgid "Default Webcam"
-msgstr "Standard Webcam"
-
 #: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:14
 msgid "MJPEG stream"
 msgstr "MJPEG Stream"
 
-#: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:20
+#: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:19
 #: src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2:24
 msgid "Not supported"
 msgstr "Nicht unterstützt"
 
-#: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:26
+#: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:25
 msgid ""
-"Selects the default webcam. If this webcam provides a MJPEG video stream,"
-" it will be available for old clients that do not make use of the webcam "
-"plugin system introduced with OctoPrint 1.9.0"
+"\n"
+"            <p>\n"
+"                Du kannst Änderungen an der Konfiguration dieser Webcam in ihren "
+"Plugineinstellungen vornehmen, so sie welche hat.\n"
+"            </p>\n"
+"        "
 msgstr ""
-"Wählt die Standard Webcam aus. Wenn diese Webcam einen MJPEG Video Stream "
-"bietet, wird er für alte Clients verfügbar sein, die das Webcam Plugin "
-"System, das mit OctoPrint 1.9.0 eingeführt wurde, nicht nutzen."
-
-#: src/octoprint/templates/snippets/settings/webcam/defaultWebcam.jinja2:28
-#: src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2:30
-msgid "You can make changes to this webcam in the plugin's settings."
-msgstr "Du kannst Änderungen an dieser Webcam in den Plugineinstellungen vornehmen."
 
 #: src/octoprint/templates/snippets/settings/webcam/ffmpegBitrate.jinja2:1
 msgid "Bitrate to use for encoding the timelapse video"
 msgstr "Bitrate für die Enkodierung der Zeitrafferaufnahme"
 
 #: src/octoprint/templates/snippets/settings/webcam/ffmpegBitrate.jinja2:2
 msgid "Timelapse bitrate"
@@ -9329,26 +9375,50 @@
 msgid "Video codec used for encoding"
 msgstr "Zum Encoding genutzter Videocodec"
 
 #: src/octoprint/templates/snippets/settings/webcam/ffmpegVideoCodec.jinja2:2
 msgid "Video codec"
 msgstr "Videocodec"
 
+#: src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2:1
 #: src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2:2
 msgid "Snapshot Webcam"
 msgstr "Snapshot Webcam"
 
 #: src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2:13
 msgid "Snapshot stream"
 msgstr "Snapshot Stream"
 
 #: src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2:20
 msgid "Supported"
 msgstr "Unterstützt"
 
+#: src/octoprint/templates/snippets/settings/webcam/snapshotWebcam.jinja2:30
+msgid ""
+"\n"
+"            <p>\n"
+"                Selects the webcam to use to take snapshots for the "
+"timelapse.\n"
+"            </p>\n"
+"            <p>\n"
+"                You can make changes to this webcam's configuration in "
+"its plugin settings, if it provides any.\n"
+"            </p>\n"
+"        "
+msgstr ""
+"\n"
+"            <p>\n"
+"                Wählt die Webcam aus, die für Timelapse-Snapshots verwendet wird.\n"
+"            </p>\n"
+"            <p>\n"
+"                Du kannst Änderungen an der Konfiguration dieser Webcam in ihren "
+"Plugineinstellungen vornehmen, so sie welche hat.\n"
+"            </p>\n"
+"        "
+
 #: src/octoprint/templates/snippets/settings/webcam/timelapseEnabled.jinja2:4
 msgid "Enable timelapse support"
 msgstr "Zeitraffer-Unterstützung aktivieren"
 
 #: src/octoprint/templates/snippets/settings/webcam/watermark.jinja2:4
 msgid "Enable OctoPrint watermark in timelapse movies"
 msgstr "OctoPrint Wasserzeichen in Zeitrafferaufnahmen aktivieren"
@@ -9365,153 +9435,153 @@
 msgid "Timeout for taking a snapshot"
 msgstr "Timeout für die Aufnahme eines Snapshots"
 
 #: src/octoprint/templates/snippets/settings/webcam/webcamSnapshotTimeout.jinja2:2
 msgid "Snapshot timeout"
 msgstr "Snapshot Timeout"
 
-#: src/octoprint/templates/tabs/control.jinja2:40
+#: src/octoprint/templates/tabs/control.jinja2:37
 msgid "Keyboard controls active"
 msgstr "Tastatursteuerung aktiv"
 
-#: src/octoprint/templates/tabs/control.jinja2:43
+#: src/octoprint/templates/tabs/control.jinja2:40
 msgid "X Axis"
 msgstr "X-Achse"
 
-#: src/octoprint/templates/tabs/control.jinja2:44
+#: src/octoprint/templates/tabs/control.jinja2:41
 msgid "Y Axis"
 msgstr "Y-Achse"
 
-#: src/octoprint/templates/tabs/control.jinja2:45
+#: src/octoprint/templates/tabs/control.jinja2:42
 msgid "Page&uarr;"
 msgstr "Bild&uarr;"
 
-#: src/octoprint/templates/tabs/control.jinja2:45
+#: src/octoprint/templates/tabs/control.jinja2:42
 msgid "Page&darr;"
 msgstr "Bild&darr;"
 
-#: src/octoprint/templates/tabs/control.jinja2:45
+#: src/octoprint/templates/tabs/control.jinja2:42
 msgid "Z Axis"
 msgstr "Z-Achse"
 
-#: src/octoprint/templates/tabs/control.jinja2:48
+#: src/octoprint/templates/tabs/control.jinja2:45
 msgid "Home X/Y"
 msgstr "Home X/Y"
 
-#: src/octoprint/templates/tabs/control.jinja2:49
+#: src/octoprint/templates/tabs/control.jinja2:46
 msgid "Home Z"
 msgstr "Home Z"
 
-#: src/octoprint/templates/tabs/control.jinja2:50
+#: src/octoprint/templates/tabs/control.jinja2:47
 msgid "Stepsize"
 msgstr "Schrittgröße"
 
-#: src/octoprint/templates/tabs/control.jinja2:58
+#: src/octoprint/templates/tabs/control.jinja2:55
 msgid ""
 "Hint: If you move your mouse over the picture, you enter keyboard control"
 " mode."
 msgstr "Hinweis: Bewegen der Maus über das Bild aktiviert die Tastatursteuerung."
 
-#: src/octoprint/templates/tabs/control.jinja2:67
+#: src/octoprint/templates/tabs/control.jinja2:64
 msgid "Move front"
 msgstr "Nach vorne bewegen"
 
-#: src/octoprint/templates/tabs/control.jinja2:70
+#: src/octoprint/templates/tabs/control.jinja2:67
 msgid "Move left"
 msgstr "Nach links bewegen"
 
-#: src/octoprint/templates/tabs/control.jinja2:71
-#: src/octoprint/templates/tabs/control.jinja2:85
+#: src/octoprint/templates/tabs/control.jinja2:68
+#: src/octoprint/templates/tabs/control.jinja2:82
 msgid "Home"
 msgstr "Homen"
 
-#: src/octoprint/templates/tabs/control.jinja2:72
+#: src/octoprint/templates/tabs/control.jinja2:69
 msgid "Move right"
 msgstr "Nach rechts bewegen"
 
-#: src/octoprint/templates/tabs/control.jinja2:75
+#: src/octoprint/templates/tabs/control.jinja2:72
 msgid "Move back"
 msgstr "Nach hinten bewegen"
 
-#: src/octoprint/templates/tabs/control.jinja2:82
+#: src/octoprint/templates/tabs/control.jinja2:79
 msgid "Move up"
 msgstr "Nach oben bewegen"
 
-#: src/octoprint/templates/tabs/control.jinja2:88
+#: src/octoprint/templates/tabs/control.jinja2:85
 msgid "Move down"
 msgstr "Nach unten bewegen"
 
-#: src/octoprint/templates/tabs/control.jinja2:103
+#: src/octoprint/templates/tabs/control.jinja2:100
 msgid "Feed rate modifier:"
 msgstr "Feedrate-Modifier:"
 
-#: src/octoprint/templates/tabs/control.jinja2:103
-#: src/octoprint/templates/tabs/control.jinja2:131
-#: src/octoprint/templates/tabs/control.jinja2:136
+#: src/octoprint/templates/tabs/control.jinja2:100
+#: src/octoprint/templates/tabs/control.jinja2:128
+#: src/octoprint/templates/tabs/control.jinja2:133
 msgid "Please note!"
 msgstr "Bitte beachten!"
 
-#: src/octoprint/templates/tabs/control.jinja2:103
+#: src/octoprint/templates/tabs/control.jinja2:100
 msgid ""
 "The feed rate can only be set, it cannot be read back from the firmware "
 "due to a limitation of the communication protocol. There is no way to "
 "show the current setting."
 msgstr ""
 "Die Feedrate kann nur gesetzt werden, sie kann nicht von der Firmware "
 "zurück gelesen werden. Dies ist eine Beschränkung im "
 "Kommunikationsprotokoll. Es gibt keine Möglichkeit, den aktuellen Wert "
 "anzuzeigen."
 
-#: src/octoprint/templates/tabs/control.jinja2:119
+#: src/octoprint/templates/tabs/control.jinja2:116
 msgid "Extrude"
 msgstr "Extrude"
 
-#: src/octoprint/templates/tabs/control.jinja2:120
+#: src/octoprint/templates/tabs/control.jinja2:117
 msgid "Retract"
 msgstr "Retract"
 
-#: src/octoprint/templates/tabs/control.jinja2:124
+#: src/octoprint/templates/tabs/control.jinja2:121
 msgid "Switch Tool..."
 msgstr "Werkzeugwechsel..."
 
-#: src/octoprint/templates/tabs/control.jinja2:131
+#: src/octoprint/templates/tabs/control.jinja2:128
 msgid ""
 "The selected tool can only be set, it cannot be read back from the "
 "firmware due to a limitation of the communication protocol. There is no "
 "way to show the current setting."
 msgstr ""
 "Das gewählte Werkzeug kann nur gesetzt werden, es kann nicht von der "
 "Firmware zurück gelesen werden. Dies ist eine Beschränkung im "
 "Kommunikationsprotokoll. Es gibt keine Möglichkeit, den aktuellen Wert "
 "anzuzeigen."
 
-#: src/octoprint/templates/tabs/control.jinja2:136
+#: src/octoprint/templates/tabs/control.jinja2:133
 msgid "Flow rate modifier:"
 msgstr "Flowrate-Modifier:"
 
-#: src/octoprint/templates/tabs/control.jinja2:136
+#: src/octoprint/templates/tabs/control.jinja2:133
 msgid ""
 "The flow rate can only be set, it cannot be read back from the firmware "
 "due to a limitation of the communication protocol. There is no way to "
 "show the current setting."
 msgstr ""
 "Die Flowrate kann nur gesetzt werden, sie kann nicht von der Firmware "
 "zurück gelesen werden. Dies ist eine Beschränkung im "
 "Kommunikationsprotokoll. Es gibt keine Möglichkeit, den aktuellen Wert "
 "anzuzeigen."
 
-#: src/octoprint/templates/tabs/control.jinja2:149
+#: src/octoprint/templates/tabs/control.jinja2:146
 msgid "Motors off"
 msgstr "Motoren aus"
 
-#: src/octoprint/templates/tabs/control.jinja2:150
+#: src/octoprint/templates/tabs/control.jinja2:147
 msgid "Fan on"
 msgstr "Lüfter an"
 
-#: src/octoprint/templates/tabs/control.jinja2:151
+#: src/octoprint/templates/tabs/control.jinja2:148
 msgid "Fan off"
 msgstr "Lüfter aus"
 
 #: src/octoprint/templates/tabs/temperature.jinja2:9
 msgid "Show state marks"
 msgstr "Statusmarker anzeigen"
 
@@ -9728,32 +9798,34 @@
 
 #: src/octoprint/templates/tabs/timelapse.jinja2:94
 msgid "Timelapse not fully configured"
 msgstr "Zeitraffer nicht vollständig konfiguriert"
 
 #: src/octoprint/templates/tabs/timelapse.jinja2:95
 msgid ""
-"The snapshot URL and/or the path to FFMPEG are missing. To have this "
-"fixed, get in touch with an administrator of this OctoPrint instance."
+"A working snapshot setup and/or the path to FFMPEG are missing. To have "
+"this fixed, get in touch with an administrator of this OctoPrint "
+"instance."
 msgstr ""
-"Die Snapshot-URL und/oder the Pfad zu FFMPEG fehlen. Setz dich mit einem "
+"Ein funktionierende Snapshot-Konfiguration und/oder the Pfad zu FFMPEG fehlen. Setz dich mit einem "
 "Administrator dieser OctoPrint-Instanz in Verbindung, um das korrigieren "
 "zu lassen."
 
 #: src/octoprint/templates/tabs/timelapse.jinja2:96
 msgid ""
-"The snapshot URL and/or the path to FFMPEG are missing. You can change "
-"both under \"Settings\" > \"Webcam & Timelapse\". If you don't have a "
-"webcam or don't want to enable timelapse support you can also just "
-"disable it there."
-msgstr ""
-"Die Snapshot-URL und/oder the Pfad zu FFMPEG fehlen. Du kannst beide "
-"unter \"Einstellungen\" > \"Webcam & Zeitraffer\" "
-"anpassen. Falls du keine Webcam hast oder Zeitrafferunterstützung nicht "
-"einschalten willst, kannst du beides auch dort abschalten."
+"A working snapshot setup and/or the path to FFMPEG are missing. You can "
+"change both under \"Settings\" > \"Webcam & Timelapse\" and in the "
+"settings of your chosen webcam plugin. If you don't have a webcam or "
+"don't want to enable timelapse support you can also just disable it "
+"there."
+msgstr ""
+"Eine funktionierende Snapshot-Konfiguration und/oder the Pfad zu FFMPEG fehlen. Du kannst beide "
+"unter \"Einstellungen\" > \"Webcam & Zeitraffer\" und in den Einstellungen des gewählten Webcam-Plugins "
+"anpassen. Falls du keine Webcam hast oder Zeitrafferunterstützung nicht einschalten willst, "
+"kannst du beides auch dort abschalten."
 
 #: src/octoprint/templates/tabs/timelapse.jinja2:100
 msgid "Currently configured snapshot (from default webcam)"
 msgstr "Aktuell konfigurierte Snapshot-URL (von Standard-Webcam)"
 
 #: src/octoprint/templates/tabs/timelapse.jinja2:103
 msgid "Snapshots supported by default webcam"
```

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/users.py` & `OctoPrint-1.9.0rc4/src/octoprint/users.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/comm.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/comm.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/commandline.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/commandline.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/connectivity.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/connectivity.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/dev.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/dev.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/files.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/files.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/gcodeInterpreter.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/gcodeInterpreter.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/jinja.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/jinja.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/json/encoding.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/json/encoding.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/json/serializing.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/json/serializing.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/net.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/net.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/paths.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/paths.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/pip.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/pip.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/piptestballoon/setup.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/piptestballoon/setup.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/platform/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/text.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/text.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/version.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/version.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/util/yaml.py` & `OctoPrint-1.9.0rc4/src/octoprint/util/yaml.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/awesome_slugify/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/awesome_slugify/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/awesome_slugify/alt_translates.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/awesome_slugify/alt_translates.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/awesome_slugify/main.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/awesome_slugify/main.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/flask_principal.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/flask_principal.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/imp.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/imp.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/basehandler.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/basehandler.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/conn.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/conn.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/migrate.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/migrate.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/periodic.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/periodic.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/proto.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/proto.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/router.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/router.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/session.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/session.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/sessioncontainer.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/sessioncontainer.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/static.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/static.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/stats.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/stats.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/base.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/base.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/eventsource.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/eventsource.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/htmlfile.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/htmlfile.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/jsonp.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/jsonp.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/pollingbase.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/pollingbase.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/rawwebsocket.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/rawwebsocket.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/streamingbase.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/streamingbase.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/websocket.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/websocket.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/xhr.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/xhr.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/transports/xhrstreaming.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/transports/xhrstreaming.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/util.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/util.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/sockjs/tornado/websocket.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/sockjs/tornado/websocket.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/vendor/with_attrs_docs.py` & `OctoPrint-1.9.0rc4/src/octoprint/vendor/with_attrs_docs.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint/webcams.py` & `OctoPrint-1.9.0rc4/src/octoprint/webcams.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint_client/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint_client/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/src/octoprint_setuptools/__init__.py` & `OctoPrint-1.9.0rc4/src/octoprint_setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoPrint-1.9.0rc3/versioneer.py` & `OctoPrint-1.9.0rc4/versioneer.py`

 * *Files identical despite different names*

