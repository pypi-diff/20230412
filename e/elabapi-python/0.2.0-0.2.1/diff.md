# Comparing `tmp/elabapi-python-0.2.0.tar.gz` & `tmp/elabapi-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elabapi-python-0.2.0.tar", last modified: Mon Apr 10 15:18:54 2023, max compression
+gzip compressed data, was "elabapi-python-0.2.1.tar", last modified: Tue Apr 11 22:39:09 2023, max compression
```

## Comparing `elabapi-python-0.2.0.tar` & `elabapi-python-0.2.1.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.564270 elabapi-python-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-10 15:18:54.564270 elabapi-python-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.532268 elabapi-python-0.2.0/elabapi_python/
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.536269 elabapi-python-0.2.0/elabapi_python/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23562 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/experiments_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/favorite_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/idps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19746 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/items_types_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/links_to_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/links_to_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18459 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22933 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/team_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20313 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/teamgroups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/todolist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/unfinished_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.548269 elabapi-python-0.2.0/elabapi_python/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/apikey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/apikeys_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    72181 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    31781 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/events_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/events_id_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/eventsid_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiment_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_templates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_templates_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/favtags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_comments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_status_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_steps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_teamgroups_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_uploads_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/idp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/idps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/idps_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_types_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/steps_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/tags_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/team_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/team_tags_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/team_tags_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/teamgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/teamgroup_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/teamgroups_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/todoitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/todolist_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/todolist_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/unfinished_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/unfinished_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/uploads_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/users_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/users_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.532268 elabapi-python-0.2.0/elabapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:18:54.564270 elabapi-python-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.564270 elabapi-python-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_apikey.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_apikeys_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_events_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_events_id_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_eventsid_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiment_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_experiments_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_templates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_templates_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_favorite_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_favtags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id1.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id2.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id3.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_comments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_status_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_steps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_teamgroups_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_uploads_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_idp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_idps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_idps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_idps_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_items_types_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_types_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_links_to_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_links_to_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_steps_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_tags_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_team_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_team_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_team_tags_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_team_tags_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_teamgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_teamgroup_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_teamgroups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_teamgroups_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_todoitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_todolist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_todolist_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_todolist_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_unfinished_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_unfinished_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_unfinished_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_uploads_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users_teams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:39:09.116362 elabapi-python-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 22:39:09.116362 elabapi-python-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:39:09.096362 elabapi-python-0.2.1/elabapi_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:39:09.100362 elabapi-python-0.2.1/elabapi_python/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23562 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/experiments_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/favorite_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/idps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19746 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/items_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/links_to_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/links_to_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18459 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22933 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/team_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20313 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/teamgroups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/todolist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/unfinished_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:39:09.108362 elabapi-python-0.2.1/elabapi_python/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/apikeys_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72181 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32079 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/events_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/events_id_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/eventsid_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/experiment_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/experiments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/experiments_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/experiments_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/experiments_templates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/experiments_templates_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/favtags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id_comments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id_status_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id_steps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id_teamgroups_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/id_uploads_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/idps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/idps_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/items_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/items_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/items_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/items_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/items_types_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/steps_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/tags_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/team_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/team_tags_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/elabapi_python/models/team_tags_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/teamgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/teamgroup_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/teamgroups_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/todoitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/todolist_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/todolist_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/unfinished_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/unfinished_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/uploads_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/users_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/models/users_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/elabapi_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:39:09.096362 elabapi-python-0.2.1/elabapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 22:39:09.000000 elabapi-python-0.2.1/elabapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-11 22:39:09.000000 elabapi-python-0.2.1/elabapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:39:09.000000 elabapi-python-0.2.1/elabapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 22:39:09.000000 elabapi-python-0.2.1/elabapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 22:39:09.000000 elabapi-python-0.2.1/elabapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 22:39:09.116362 elabapi-python-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:39:09.116362 elabapi-python-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_apikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_apikeys_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_events_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_events_id_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_eventsid_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_experiment_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_experiments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_experiments_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_experiments_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_experiments_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_experiments_templates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_experiments_templates_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_favorite_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_favtags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id_comments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id_status_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id_steps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id_teamgroups_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_id_uploads_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_idps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_idps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_idps_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_items_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_items_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_items_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_items_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_items_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_items_types_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_links_to_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_links_to_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_steps_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_tags_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_team_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_team_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_team_tags_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-11 22:39:00.000000 elabapi-python-0.2.1/test/test_team_tags_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_teamgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_teamgroup_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_teamgroups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_teamgroups_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_todoitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_todolist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_todolist_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_todolist_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_unfinished_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_unfinished_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_unfinished_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_uploads_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_users_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-11 22:39:01.000000 elabapi-python-0.2.1/test/test_users_teams.py
```

### Comparing `elabapi-python-0.2.0/README.md` & `elabapi-python-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # elabapi-python
 This document describes all available endpoints and methods for eLabFTW's API version 2. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 2.0.0
-- Package version: 0.2.0
+- Package version: 0.2.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `elabapi-python-0.2.0/elabapi_python/__init__.py` & `elabapi-python-0.2.1/elabapi_python/__init__.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/__init__.py` & `elabapi-python-0.2.1/elabapi_python/api/__init__.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/api_keys_api.py` & `elabapi-python-0.2.1/elabapi_python/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/comments_api.py` & `elabapi-python-0.2.1/elabapi_python/api/comments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/config_api.py` & `elabapi-python-0.2.1/elabapi_python/api/config_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/events_api.py` & `elabapi-python-0.2.1/elabapi_python/api/events_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/experiments_api.py` & `elabapi-python-0.2.1/elabapi_python/api/experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/experiments_templates_api.py` & `elabapi-python-0.2.1/elabapi_python/api/experiments_templates_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/favorite_tags_api.py` & `elabapi-python-0.2.1/elabapi_python/api/favorite_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/idps_api.py` & `elabapi-python-0.2.1/elabapi_python/api/idps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/items_api.py` & `elabapi-python-0.2.1/elabapi_python/api/items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/items_types_api.py` & `elabapi-python-0.2.1/elabapi_python/api/items_types_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/links_to_experiments_api.py` & `elabapi-python-0.2.1/elabapi_python/api/links_to_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/links_to_items_api.py` & `elabapi-python-0.2.1/elabapi_python/api/links_to_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/notifications_api.py` & `elabapi-python-0.2.1/elabapi_python/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/status_api.py` & `elabapi-python-0.2.1/elabapi_python/api/status_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/steps_api.py` & `elabapi-python-0.2.1/elabapi_python/api/steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/tags_api.py` & `elabapi-python-0.2.1/elabapi_python/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/team_tags_api.py` & `elabapi-python-0.2.1/elabapi_python/api/team_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/teamgroups_api.py` & `elabapi-python-0.2.1/elabapi_python/api/teamgroups_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/teams_api.py` & `elabapi-python-0.2.1/elabapi_python/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/todolist_api.py` & `elabapi-python-0.2.1/elabapi_python/api/todolist_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/unfinished_steps_api.py` & `elabapi-python-0.2.1/elabapi_python/api/unfinished_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/uploads_api.py` & `elabapi-python-0.2.1/elabapi_python/api/uploads_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api/users_api.py` & `elabapi-python-0.2.1/elabapi_python/api/users_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/api_client.py` & `elabapi-python-0.2.1/elabapi_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/0.2.0/python'
+        self.user_agent = 'Swagger-Codegen/0.2.1/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `elabapi-python-0.2.0/elabapi_python/configuration.py` & `elabapi-python-0.2.1/elabapi_python/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,9 +243,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.0.0\n"\
-               "SDK Package Version: 0.2.0".\
+               "SDK Package Version: 0.2.1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `elabapi-python-0.2.0/elabapi_python/models/__init__.py` & `elabapi-python-0.2.1/elabapi_python/models/__init__.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/apikey.py` & `elabapi-python-0.2.1/elabapi_python/models/apikey.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/apikeys_body.py` & `elabapi-python-0.2.1/elabapi_python/models/apikeys_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/comment.py` & `elabapi-python-0.2.1/elabapi_python/models/comment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/config.py` & `elabapi-python-0.2.1/elabapi_python/models/config.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/entity.py` & `elabapi-python-0.2.1/elabapi_python/models/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,24 +435,26 @@
 
         self._comments = comments
 
     @property
     def content_type(self):
         """Gets the content_type of this Entity.  # noqa: E501
 
+        How the body is stored. 1 for HTML, 2 for Markdown. If you plan on creating an entity with markdown, make sure to set it to 2.  # noqa: E501
 
         :return: The content_type of this Entity.  # noqa: E501
         :rtype: int
         """
         return self._content_type
 
     @content_type.setter
     def content_type(self, content_type):
         """Sets the content_type of this Entity.
 
+        How the body is stored. 1 for HTML, 2 for Markdown. If you plan on creating an entity with markdown, make sure to set it to 2.  # noqa: E501
 
         :param content_type: The content_type of this Entity.  # noqa: E501
         :type: int
         """
 
         self._content_type = content_type
```

### Comparing `elabapi-python-0.2.0/elabapi_python/models/event.py` & `elabapi-python-0.2.1/elabapi_python/models/event.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/events_id_body.py` & `elabapi-python-0.2.1/elabapi_python/models/events_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/events_id_body1.py` & `elabapi-python-0.2.1/elabapi_python/models/events_id_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/eventsid_delta.py` & `elabapi-python-0.2.1/elabapi_python/models/eventsid_delta.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/experiment.py` & `elabapi-python-0.2.1/elabapi_python/models/experiment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/experiment_template.py` & `elabapi-python-0.2.1/elabapi_python/models/experiment_template.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/experiments_body.py` & `elabapi-python-0.2.1/elabapi_python/models/experiments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/experiments_id_body.py` & `elabapi-python-0.2.1/elabapi_python/models/experiments_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/experiments_links_subid_body.py` & `elabapi-python-0.2.1/elabapi_python/models/experiments_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/experiments_templates_body.py` & `elabapi-python-0.2.1/elabapi_python/models/experiments_templates_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/experiments_templates_id_body.py` & `elabapi-python-0.2.1/elabapi_python/models/experiments_templates_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/favtags_body.py` & `elabapi-python-0.2.1/elabapi_python/models/favtags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id.py` & `elabapi-python-0.2.1/elabapi_python/models/id.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id1.py` & `elabapi-python-0.2.1/elabapi_python/models/id1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id2.py` & `elabapi-python-0.2.1/elabapi_python/models/id2.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id3.py` & `elabapi-python-0.2.1/elabapi_python/models/id3.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id_comments_body.py` & `elabapi-python-0.2.1/elabapi_python/models/id_comments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id_status_body.py` & `elabapi-python-0.2.1/elabapi_python/models/id_status_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id_steps_body.py` & `elabapi-python-0.2.1/elabapi_python/models/id_steps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id_tags_body.py` & `elabapi-python-0.2.1/elabapi_python/models/id_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id_teamgroups_body.py` & `elabapi-python-0.2.1/elabapi_python/models/id_teamgroups_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/id_uploads_body.py` & `elabapi-python-0.2.1/elabapi_python/models/id_uploads_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/idp.py` & `elabapi-python-0.2.1/elabapi_python/models/idp.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/idps_body.py` & `elabapi-python-0.2.1/elabapi_python/models/idps_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,32 +71,23 @@
         self._x509_new = None
         self._email_attr = None
         self._team_attr = None
         self._fname_attr = None
         self._lname_attr = None
         self._orgid_attr = None
         self.discriminator = None
-        if name is not None:
-            self.name = name
-        if entityid is not None:
-            self.entityid = entityid
-        if sso_url is not None:
-            self.sso_url = sso_url
-        if sso_binding is not None:
-            self.sso_binding = sso_binding
-        if slo_url is not None:
-            self.slo_url = slo_url
-        if slo_binding is not None:
-            self.slo_binding = slo_binding
-        if x509 is not None:
-            self.x509 = x509
-        if x509_new is not None:
-            self.x509_new = x509_new
-        if email_attr is not None:
-            self.email_attr = email_attr
+        self.name = name
+        self.entityid = entityid
+        self.sso_url = sso_url
+        self.sso_binding = sso_binding
+        self.slo_url = slo_url
+        self.slo_binding = slo_binding
+        self.x509 = x509
+        self.x509_new = x509_new
+        self.email_attr = email_attr
         if team_attr is not None:
             self.team_attr = team_attr
         if fname_attr is not None:
             self.fname_attr = fname_attr
         if lname_attr is not None:
             self.lname_attr = lname_attr
         if orgid_attr is not None:
@@ -118,14 +109,16 @@
         """Sets the name of this IdpsBody.
 
         A name for the IDP.  # noqa: E501
 
         :param name: The name of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def entityid(self):
         """Gets the entityid of this IdpsBody.  # noqa: E501
 
@@ -141,14 +134,16 @@
         """Sets the entityid of this IdpsBody.
 
         Entityid.  # noqa: E501
 
         :param entityid: The entityid of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if entityid is None:
+            raise ValueError("Invalid value for `entityid`, must not be `None`")  # noqa: E501
 
         self._entityid = entityid
 
     @property
     def sso_url(self):
         """Gets the sso_url of this IdpsBody.  # noqa: E501
 
@@ -164,14 +159,16 @@
         """Sets the sso_url of this IdpsBody.
 
         URL for Single Sign-On.  # noqa: E501
 
         :param sso_url: The sso_url of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if sso_url is None:
+            raise ValueError("Invalid value for `sso_url`, must not be `None`")  # noqa: E501
 
         self._sso_url = sso_url
 
     @property
     def sso_binding(self):
         """Gets the sso_binding of this IdpsBody.  # noqa: E501
 
@@ -187,14 +184,16 @@
         """Sets the sso_binding of this IdpsBody.
 
         Binding for SSO.  # noqa: E501
 
         :param sso_binding: The sso_binding of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if sso_binding is None:
+            raise ValueError("Invalid value for `sso_binding`, must not be `None`")  # noqa: E501
 
         self._sso_binding = sso_binding
 
     @property
     def slo_url(self):
         """Gets the slo_url of this IdpsBody.  # noqa: E501
 
@@ -210,14 +209,16 @@
         """Sets the slo_url of this IdpsBody.
 
         URL for Single Log-Out.  # noqa: E501
 
         :param slo_url: The slo_url of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if slo_url is None:
+            raise ValueError("Invalid value for `slo_url`, must not be `None`")  # noqa: E501
 
         self._slo_url = slo_url
 
     @property
     def slo_binding(self):
         """Gets the slo_binding of this IdpsBody.  # noqa: E501
 
@@ -233,14 +234,16 @@
         """Sets the slo_binding of this IdpsBody.
 
         Binding for SLO.  # noqa: E501
 
         :param slo_binding: The slo_binding of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if slo_binding is None:
+            raise ValueError("Invalid value for `slo_binding`, must not be `None`")  # noqa: E501
 
         self._slo_binding = slo_binding
 
     @property
     def x509(self):
         """Gets the x509 of this IdpsBody.  # noqa: E501
 
@@ -256,14 +259,16 @@
         """Sets the x509 of this IdpsBody.
 
         Certificate in PEM format.  # noqa: E501
 
         :param x509: The x509 of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if x509 is None:
+            raise ValueError("Invalid value for `x509`, must not be `None`")  # noqa: E501
 
         self._x509 = x509
 
     @property
     def x509_new(self):
         """Gets the x509_new of this IdpsBody.  # noqa: E501
 
@@ -279,14 +284,16 @@
         """Sets the x509_new of this IdpsBody.
 
         Certificate in PEM format for renewal period.  # noqa: E501
 
         :param x509_new: The x509_new of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if x509_new is None:
+            raise ValueError("Invalid value for `x509_new`, must not be `None`")  # noqa: E501
 
         self._x509_new = x509_new
 
     @property
     def email_attr(self):
         """Gets the email_attr of this IdpsBody.  # noqa: E501
 
@@ -302,14 +309,16 @@
         """Sets the email_attr of this IdpsBody.
 
         What attribute to look for the email.  # noqa: E501
 
         :param email_attr: The email_attr of this IdpsBody.  # noqa: E501
         :type: str
         """
+        if email_attr is None:
+            raise ValueError("Invalid value for `email_attr`, must not be `None`")  # noqa: E501
 
         self._email_attr = email_attr
 
     @property
     def team_attr(self):
         """Gets the team_attr of this IdpsBody.  # noqa: E501
```

### Comparing `elabapi-python-0.2.0/elabapi_python/models/idps_id_body.py` & `elabapi-python-0.2.1/elabapi_python/models/idps_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/inline_response200.py` & `elabapi-python-0.2.1/elabapi_python/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/inline_response2001.py` & `elabapi-python-0.2.1/elabapi_python/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/inline_response2002.py` & `elabapi-python-0.2.1/elabapi_python/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/inline_response2003.py` & `elabapi-python-0.2.1/elabapi_python/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/item.py` & `elabapi-python-0.2.1/elabapi_python/models/item.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/items_body.py` & `elabapi-python-0.2.1/elabapi_python/models/items_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/items_id_body.py` & `elabapi-python-0.2.1/elabapi_python/models/items_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/items_links_subid_body.py` & `elabapi-python-0.2.1/elabapi_python/models/items_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/items_type.py` & `elabapi-python-0.2.1/elabapi_python/models/items_type.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/items_types_body.py` & `elabapi-python-0.2.1/elabapi_python/models/items_types_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/link.py` & `elabapi-python-0.2.1/elabapi_python/models/link.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/notification.py` & `elabapi-python-0.2.1/elabapi_python/models/notification.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/status.py` & `elabapi-python-0.2.1/elabapi_python/models/status.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/step.py` & `elabapi-python-0.2.1/elabapi_python/models/step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/steps_subid_body.py` & `elabapi-python-0.2.1/elabapi_python/models/steps_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/tag.py` & `elabapi-python-0.2.1/elabapi_python/models/tag.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/tags_subid_body.py` & `elabapi-python-0.2.1/elabapi_python/models/tags_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/team.py` & `elabapi-python-0.2.1/elabapi_python/models/team.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/team_tags_body.py` & `elabapi-python-0.2.1/elabapi_python/models/team_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/team_tags_body1.py` & `elabapi-python-0.2.1/elabapi_python/models/team_tags_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/team_tags_id_body.py` & `elabapi-python-0.2.1/elabapi_python/models/team_tags_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/teamgroup.py` & `elabapi-python-0.2.1/elabapi_python/models/teamgroup.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/teamgroup_users.py` & `elabapi-python-0.2.1/elabapi_python/models/teamgroup_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/teamgroups_subid_body.py` & `elabapi-python-0.2.1/elabapi_python/models/teamgroups_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/teams_body.py` & `elabapi-python-0.2.1/elabapi_python/models/teams_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/todoitem.py` & `elabapi-python-0.2.1/elabapi_python/models/todoitem.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/todolist_body.py` & `elabapi-python-0.2.1/elabapi_python/models/todolist_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/todolist_id_body.py` & `elabapi-python-0.2.1/elabapi_python/models/todolist_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/unfinished_step.py` & `elabapi-python-0.2.1/elabapi_python/models/unfinished_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/unfinished_steps.py` & `elabapi-python-0.2.1/elabapi_python/models/unfinished_steps.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/upload.py` & `elabapi-python-0.2.1/elabapi_python/models/upload.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/uploads_subid_body.py` & `elabapi-python-0.2.1/elabapi_python/models/uploads_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/users.py` & `elabapi-python-0.2.1/elabapi_python/models/users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/users_body.py` & `elabapi-python-0.2.1/elabapi_python/models/users_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/users_id_body.py` & `elabapi-python-0.2.1/elabapi_python/models/users_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/models/users_teams.py` & `elabapi-python-0.2.1/elabapi_python/models/users_teams.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python/rest.py` & `elabapi-python-0.2.1/elabapi_python/rest.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/elabapi_python.egg-info/SOURCES.txt` & `elabapi-python-0.2.1/elabapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/setup.py` & `elabapi-python-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "elabapi-python"
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `elabapi-python-0.2.0/test/test_api_keys_api.py` & `elabapi-python-0.2.1/test/test_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_apikey.py` & `elabapi-python-0.2.1/test/test_apikey.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_apikeys_body.py` & `elabapi-python-0.2.1/test/test_apikeys_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_comment.py` & `elabapi-python-0.2.1/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_comments_api.py` & `elabapi-python-0.2.1/test/test_comments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_config.py` & `elabapi-python-0.2.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_config_api.py` & `elabapi-python-0.2.1/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_entity.py` & `elabapi-python-0.2.1/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_event.py` & `elabapi-python-0.2.1/test/test_event.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_events_api.py` & `elabapi-python-0.2.1/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_events_id_body.py` & `elabapi-python-0.2.1/test/test_events_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_events_id_body1.py` & `elabapi-python-0.2.1/test/test_events_id_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_eventsid_delta.py` & `elabapi-python-0.2.1/test/test_eventsid_delta.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiment.py` & `elabapi-python-0.2.1/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiment_template.py` & `elabapi-python-0.2.1/test/test_experiment_template.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiments_api.py` & `elabapi-python-0.2.1/test/test_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiments_body.py` & `elabapi-python-0.2.1/test/test_experiments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiments_id_body.py` & `elabapi-python-0.2.1/test/test_experiments_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiments_links_subid_body.py` & `elabapi-python-0.2.1/test/test_experiments_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiments_templates_api.py` & `elabapi-python-0.2.1/test/test_experiments_templates_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiments_templates_body.py` & `elabapi-python-0.2.1/test/test_experiments_templates_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_experiments_templates_id_body.py` & `elabapi-python-0.2.1/test/test_experiments_templates_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_favorite_tags_api.py` & `elabapi-python-0.2.1/test/test_favorite_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_favtags_body.py` & `elabapi-python-0.2.1/test/test_favtags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id.py` & `elabapi-python-0.2.1/test/test_id.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id1.py` & `elabapi-python-0.2.1/test/test_id1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id2.py` & `elabapi-python-0.2.1/test/test_id2.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id3.py` & `elabapi-python-0.2.1/test/test_id3.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id_comments_body.py` & `elabapi-python-0.2.1/test/test_id_comments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id_status_body.py` & `elabapi-python-0.2.1/test/test_id_status_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id_steps_body.py` & `elabapi-python-0.2.1/test/test_id_steps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id_tags_body.py` & `elabapi-python-0.2.1/test/test_id_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id_teamgroups_body.py` & `elabapi-python-0.2.1/test/test_id_teamgroups_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_id_uploads_body.py` & `elabapi-python-0.2.1/test/test_id_uploads_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_idp.py` & `elabapi-python-0.2.1/test/test_idp.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_idps_api.py` & `elabapi-python-0.2.1/test/test_idps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_idps_body.py` & `elabapi-python-0.2.1/test/test_idps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_idps_id_body.py` & `elabapi-python-0.2.1/test/test_idps_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_inline_response200.py` & `elabapi-python-0.2.1/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_inline_response2001.py` & `elabapi-python-0.2.1/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_inline_response2002.py` & `elabapi-python-0.2.1/test/test_inline_response2002.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_inline_response2003.py` & `elabapi-python-0.2.1/test/test_inline_response2003.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_item.py` & `elabapi-python-0.2.1/test/test_item.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_items_api.py` & `elabapi-python-0.2.1/test/test_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_items_body.py` & `elabapi-python-0.2.1/test/test_items_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_items_id_body.py` & `elabapi-python-0.2.1/test/test_items_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_items_links_subid_body.py` & `elabapi-python-0.2.1/test/test_items_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_items_type.py` & `elabapi-python-0.2.1/test/test_items_type.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_items_types_api.py` & `elabapi-python-0.2.1/test/test_items_types_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_items_types_body.py` & `elabapi-python-0.2.1/test/test_items_types_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_link.py` & `elabapi-python-0.2.1/test/test_link.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_links_to_experiments_api.py` & `elabapi-python-0.2.1/test/test_links_to_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_links_to_items_api.py` & `elabapi-python-0.2.1/test/test_links_to_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_notification.py` & `elabapi-python-0.2.1/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_notifications_api.py` & `elabapi-python-0.2.1/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_status.py` & `elabapi-python-0.2.1/test/test_status.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_status_api.py` & `elabapi-python-0.2.1/test/test_status_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_step.py` & `elabapi-python-0.2.1/test/test_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_steps_api.py` & `elabapi-python-0.2.1/test/test_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_steps_subid_body.py` & `elabapi-python-0.2.1/test/test_steps_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_tag.py` & `elabapi-python-0.2.1/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_tags_api.py` & `elabapi-python-0.2.1/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_tags_subid_body.py` & `elabapi-python-0.2.1/test/test_tags_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_team.py` & `elabapi-python-0.2.1/test/test_team.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_team_tags_api.py` & `elabapi-python-0.2.1/test/test_team_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_team_tags_body.py` & `elabapi-python-0.2.1/test/test_team_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_team_tags_body1.py` & `elabapi-python-0.2.1/test/test_team_tags_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_team_tags_id_body.py` & `elabapi-python-0.2.1/test/test_team_tags_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_teamgroup.py` & `elabapi-python-0.2.1/test/test_teamgroup.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_teamgroup_users.py` & `elabapi-python-0.2.1/test/test_teamgroup_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_teamgroups_api.py` & `elabapi-python-0.2.1/test/test_teamgroups_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_teamgroups_subid_body.py` & `elabapi-python-0.2.1/test/test_teamgroups_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_teams_api.py` & `elabapi-python-0.2.1/test/test_teams_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_teams_body.py` & `elabapi-python-0.2.1/test/test_teams_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_todoitem.py` & `elabapi-python-0.2.1/test/test_todoitem.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_todolist_api.py` & `elabapi-python-0.2.1/test/test_todolist_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_todolist_body.py` & `elabapi-python-0.2.1/test/test_todolist_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_todolist_id_body.py` & `elabapi-python-0.2.1/test/test_todolist_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_unfinished_step.py` & `elabapi-python-0.2.1/test/test_unfinished_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_unfinished_steps.py` & `elabapi-python-0.2.1/test/test_unfinished_steps.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_unfinished_steps_api.py` & `elabapi-python-0.2.1/test/test_unfinished_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_upload.py` & `elabapi-python-0.2.1/test/test_upload.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_uploads_api.py` & `elabapi-python-0.2.1/test/test_uploads_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_uploads_subid_body.py` & `elabapi-python-0.2.1/test/test_uploads_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_users.py` & `elabapi-python-0.2.1/test/test_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_users_api.py` & `elabapi-python-0.2.1/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_users_body.py` & `elabapi-python-0.2.1/test/test_users_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_users_id_body.py` & `elabapi-python-0.2.1/test/test_users_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.0/test/test_users_teams.py` & `elabapi-python-0.2.1/test/test_users_teams.py`

 * *Files identical despite different names*

