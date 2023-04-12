# Comparing `tmp/terka-1.3.3.tar.gz` & `tmp/terka-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.3.3.tar", last modified: Tue Apr 11 15:55:08 2023, max compression
+gzip compressed data, was "terka-1.4.0.tar", last modified: Wed Apr 12 20:26:26 2023, max compression
```

## Comparing `terka-1.3.3.tar` & `terka-1.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:55:08.740476 terka-1.3.3/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.3.3/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-11 15:55:08.736477 terka-1.3.3/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.3.3/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-11 15:55:08.740476 terka-1.3.3/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-11 15:55:05.000000 terka-1.3.3/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:55:08.732478 terka-1.3.3/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.3/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:55:08.732478 terka-1.3.3/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.3/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    13439 2023-04-08 10:39:03.000000 terka-1.3.3/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.3.3/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:55:08.736477 terka-1.3.3/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.3/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.3.3/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    32550 2023-04-08 19:16:35.000000 terka-1.3.3/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)      827 2023-03-06 19:56:41.000000 terka-1.3.3/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.3.3/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.3.3/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.3.3/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.3.3/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.3.3/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.3.3/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.3.3/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.3.3/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.3.3/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.3.3/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.3.3/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:55:08.736477 terka-1.3.3/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.3.3/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.3.3/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:55:08.736477 terka-1.3.3/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.3/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    26699 2023-04-11 15:53:48.000000 terka-1.3.3/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.3.3/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.3.3/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.3.3/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     6764 2023-04-08 10:39:03.000000 terka-1.3.3/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:55:08.736477 terka-1.3.3/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-11 15:55:08.000000 terka-1.3.3/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-11 15:55:08.000000 terka-1.3.3/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-11 15:55:08.000000 terka-1.3.3/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-11 15:55:08.000000 terka-1.3.3/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-11 15:55:08.000000 terka-1.3.3/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-11 15:55:08.000000 terka-1.3.3/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:55:08.736477 terka-1.3.3/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.3/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.3.3/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.3.3/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.3.3/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.3.3/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.3.3/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.3.3/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.4.0/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-12 20:26:26.292028 terka-1.4.0/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.4.0/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-12 20:26:26.292028 terka-1.4.0/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-12 20:25:42.000000 terka-1.4.0/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.288028 terka-1.4.0/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.288028 terka-1.4.0/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.4.0/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.4.0/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.4.0/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    36138 2023-04-12 20:18:40.000000 terka-1.4.0/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.4.0/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.4.0/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.4.0/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.4.0/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.4.0/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.4.0/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.4.0/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.4.0/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.4.0/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.4.0/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.4.0/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.4.0/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.4.0/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.4.0/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27188 2023-04-12 20:20:05.000000 terka-1.4.0/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.4.0/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.4.0/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.4.0/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     6929 2023-04-12 19:45:59.000000 terka-1.4.0/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.4.0/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_utils.py
```

### Comparing `terka-1.3.3/LICENSE` & `terka-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/PKG-INFO` & `terka-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.3.3
+Version: 1.4.0
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.3.3/README.md` & `terka-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/setup.py` & `terka-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.3.3",
+    version="1.4.0",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.3.3/src/adapters/orm.py` & `terka-1.4.0/src/adapters/orm.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 )
 from sqlalchemy.orm import mapper, registry, relationship, validates, declarative_base
 
 from src.domain.task import Task, TaskStatus, TaskPriority
 from src.domain.user import User
 from src.domain.project import Project, ProjectStatus
 from src.domain.event_history import TaskEvent, ProjectEvent, EventType
-from src.domain.commentary import TaskCommentary, ProjectCommentary
+from src.domain.commentary import TaskCommentary, ProjectCommentary, EpicCommentary, StoryCommentary, SprintCommentary
 from src.domain.tag import BaseTag, TaskTag, ProjectTag
 from src.domain.collaborators import TaskCollaborator, ProjectCollaborator
 from src.domain.sprint import Sprint, SprintStatus, SprintTask
 from src.domain.time_tracker import TimeTrackerEntry
 from src.domain.epic import Epic, EpicTask
 from src.domain.story import Story, StoryTask
 
@@ -95,14 +95,41 @@
     metadata,
     Column("id", Integer, primary_key=True, autoincrement=True),
     Column("project", ForeignKey("projects.id"), nullable=True),
     Column("date", DateTime, nullable=False),
     Column("text", String(225)),
 )
 
+epic_commentaries = Table(
+    "epic_commentaries",
+    metadata,
+    Column("id", Integer, primary_key=True, autoincrement=True),
+    Column("epic", ForeignKey("epics.id"), nullable=True),
+    Column("date", DateTime, nullable=False),
+    Column("text", String(225)),
+)
+
+story_commentaries = Table(
+    "story_commentaries",
+    metadata,
+    Column("id", Integer, primary_key=True, autoincrement=True),
+    Column("story", ForeignKey("stories.id"), nullable=True),
+    Column("date", DateTime, nullable=False),
+    Column("text", String(225)),
+)
+
+sprint_commentaries = Table(
+    "sprint_commentaries",
+    metadata,
+    Column("id", Integer, primary_key=True, autoincrement=True),
+    Column("sprint", ForeignKey("sprints.id"), nullable=True),
+    Column("date", DateTime, nullable=False),
+    Column("text", String(225)),
+)
+
 users = Table("users", metadata,
               Column("id", Integer, primary_key=True, autoincrement=True),
               Column("name", String(50)))
 
 tags = Table("tags", metadata,
              Column("id", Integer, primary_key=True, autoincrement=True),
              Column("text", String(50)))
@@ -191,14 +218,17 @@
 #     sprint_id = Integer(nullable=False)
 #     ta
 
 
 def start_mappers():
     task_commentary_mapper = mapper(TaskCommentary, task_commentaries)
     project_commentary_mapper = mapper(ProjectCommentary, project_commentaries)
+    epic_commentary_mapper = mapper(EpicCommentary, epic_commentaries)
+    story_commentary_mapper = mapper(StoryCommentary, story_commentaries)
+    sprint_commentary_mapper = mapper(SprintCommentary, sprint_commentaries)
     task_event_mapper = mapper(TaskEvent, task_events)
     project_event_mapper = mapper(ProjectEvent, project_events)
     user_mapper = mapper(User, users)
     tag_mapper = mapper(BaseTag, tags)
     task_tag_mapper = mapper(TaskTag,
                              task_tags,
                              properties={
@@ -249,25 +279,33 @@
     epic_tasks_mapper = mapper(
         EpicTask,
         epic_tasks,
         properties={"tasks": relationship(task_mapper, collection_class=list)})
     epic_mapper = mapper(Epic,
                          epics,
                          properties={
+                             "commentaries":
+                             relationship(epic_commentary_mapper,
+                                          collection_class=list,
+                                          cascade="all, delete-orphan"),
                              "epic_tasks":
                              relationship(epic_tasks_mapper,
                                           collection_class=list)
                          })
     story_tasks_mapper = mapper(
         StoryTask,
         story_tasks,
         properties={"tasks": relationship(task_mapper, collection_class=list)})
     story_mapper = mapper(Story,
                           stories,
                           properties={
+                             "commentaries":
+                             relationship(story_commentary_mapper,
+                                          collection_class=list,
+                                          cascade="all, delete-orphan"),
                               "story_tasks":
                               relationship(story_tasks_mapper,
                                            collection_class=list)
                           })
     project_mapper = mapper(Project,
                             projects,
                             properties={
@@ -299,11 +337,15 @@
     sprint_tasks_mapper = mapper(
         SprintTask,
         sprint_tasks,
         properties={"tasks": relationship(task_mapper, collection_class=list)})
     sprint_mapper = mapper(Sprint,
                            sprints,
                            properties={
+                               "commentaries":
+                               relationship(sprint_commentary_mapper,
+                                            collection_class=list,
+                                        cascade="all, delete-orphan"),
                                "sprint_tasks":
                                relationship(sprint_tasks_mapper,
                                             collection_class=list)
                            })
```

### Comparing `terka-1.3.3/src/adapters/repository.py` & `terka-1.4.0/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/collaborators.py` & `terka-1.4.0/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/commands.py` & `terka-1.4.0/src/domain/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import rich
 from rich.console import Console
 from rich.table import Table
 
 from src.domain.task import Task
 from src.domain.project import Project
 from src.domain.user import User
-from src.domain.commentary import TaskCommentary, ProjectCommentary
+from src.domain.commentary import TaskCommentary, ProjectCommentary, EpicCommentary, StoryCommentary, SprintCommentary
 from src.domain.tag import BaseTag, TaskTag, ProjectTag
 from src.domain.collaborators import TaskCollaborator, ProjectCollaborator
 from src.domain.event_history import TaskEvent, ProjectEvent
 from src.domain.sprint import Sprint, SprintTask
 from src.domain.time_tracker import TimeTrackerEntry
 from src.domain.epic import Epic, EpicTask
 from src.domain.story import Story, StoryTask
@@ -188,16 +188,15 @@
 
     def handle(self, entity):
         return self.handler.handle(entity)
 
     def execute(self,
                 command,
                 entity_type=None,
-                kwargs: Dict[str, Any] = None
-                ):
+                kwargs: Dict[str, Any] = None):
         session = self.repo.session
         if entity_type:
             entity, entity_type = self.handle(entity_type)
         else:
             entity = None
         if not entity and command not in ("init", "unfocus", "log", "calendar",
                                           "help"):
@@ -265,15 +264,16 @@
                         del kwargs["tags"]
                     else:
                         self.console.print(
                             f"[red]No tasks with tag '{tag_text}' found![/red]"
                         )
                         exit()
                 else:
-                    self.console.print(f"[red]No tag '{tag_text}' found![/red]")
+                    self.console.print(
+                        f"[red]No tag '{tag_text}' found![/red]")
                     exit()
             entities = self.repo.list(entity, kwargs)
             if entity_type == "sprints":
                 self.printer.print_sprint(entities=entities,
                                           repo=self.repo,
                                           show_tasks=False)
                 exit()
@@ -511,30 +511,89 @@
                                                   {"id": kwargs["id"]})
                 if not existing_project:
                     raise ValueError(
                         f"Project with id {kwargs['id']} is not found!")
                 obj = ProjectCommentary(**kwargs)
                 self.repo.add(obj)
                 session.commit()
+            elif entity_type == "epics":
+                epic = self.repo.list(Epic, {"id": kwargs["id"]})
+                if not epic:
+                    raise ValueError(
+                        f"Epic with id {kwargs['id']} is not found!")
+                obj = EpicCommentary(**kwargs)
+                self.repo.add(obj)
+                session.commit()
+            elif entity_type == "stories":
+                epic = self.repo.list(Story, {"id": kwargs["id"]})
+                if not epic:
+                    raise ValueError(
+                        f"Story with id {kwargs['id']} is not found!")
+                obj = StoryCommentary(**kwargs)
+                self.repo.add(obj)
+                session.commit()
+            elif entity_type == "sprints":
+                sprint = self.repo.list(Sprint, {"id": kwargs["id"]})
+                if not sprint:
+                    raise ValueError(
+                        f"Sprint with id {kwargs['id']} is not found!")
+                obj = SprintCommentary(**kwargs)
+                self.repo.add(obj)
+                session.commit()
+        elif command == "delete":
+            if entity not in (Task, ):
+                raise ValueError("'delete' operation only allowed for tasks!")
+            task_ids = get_ids(kwargs.get("id"))
+            for task_id in task_ids:
+                if not self.repo.list(Task, {"id": task_id}):
+                    exit(f"Task id {task_id} is not found")
+                if epic_id := kwargs.get("epic_id"):
+                    epic = self.repo.list(Epic, {"id": epic_id})
+                    if not epic:
+                        exit(f"Epic id {epic_id} is not found")
+                    if not (epic_task := self.repo.list(
+                            EpicTask, {
+                                "task": task_id,
+                                "epic": epic_id
+                            })):
+                        exit("task is not in epic")
+                    self.repo.delete(EpicTask, epic_task[0].id)
+                if story_id := kwargs.get("story_id"):
+                    story = self.repo.list(Story, {"id": story_id})
+                    if not story:
+                        exit(f"Story id {story_id} is not found")
+                    if not (story_task := self.repo.list(
+                            StoryTask, {
+                                "task": task_id,
+                                "story": story_id
+                            })):
+                        exit("task is not in story")
+                    self.repo.delete(StoryTask, story_task[0].id)
+                if sprint_id := kwargs.get("sprint_id"):
+                    sprint = self.repo.list(Sprint, {"id": sprint_id})
+                    if not sprint:
+                        exit(f"Sprint id {sprint_id} is not found")
+                    if sprint[0].status.name == "COMPLETED":
+                        exit("Cannot add task to a finished sprint")
+                    if not (sprint_task := self.repo.list(
+                            SprintTask, {
+                                "task": task_id,
+                                "sprint": sprint_id
+                            })):
+                        exit("task is not in sprint")
+                    self.repo.delete(SprintTask, sprint_task[0].id)
+            session.commit()
         elif command == "add":
             if entity not in (Task, ):
                 raise ValueError("'add' operation only allowed for tasks!")
             task_ids = get_ids(kwargs.get("id"))
             for task_id in task_ids:
                 if not self.repo.list(Task, {"id": task_id}):
                     exit(f"Task id {task_id} is not found")
 
-                if story_points := kwargs.get("story_points"):
-                    sprint_task = self.execute("get", "sprint_tasks",
-                                               {"task": task_id})
-                    if sprint_task:
-                        self.repo.update(SprintTask, sprint_task[0].id,
-                                         {"story_points": story_points})
-                    else:
-                        exit(f"Task id {task_id} is not part of any sprint")
                 if epic_id := kwargs.get("epic_id"):
                     epic = self.repo.list(Epic, {"id": epic_id})
                     if not epic:
                         exit(f"Epic id {epic_id} is not found")
                     obj = EpicTask(task=task_id, epic=epic_id)
                     if self.repo.list(EpicTask, {
                             "task": obj.task,
@@ -564,19 +623,31 @@
                                      is_active_link=True)
                     if self.repo.list(SprintTask, {
                             "task": obj.task,
                             "sprint": obj.sprint
                     }):
                         exit("task already added to sprint")
                     self.repo.add(obj)
+                    sprint_task_id = obj.id
+                else:
+                    sprint_task_id = None
+                if story_points := kwargs.get("story_points"):
+                    if not sprint_task_id:
+                        sprint_task = self.execute("get", "sprint_tasks",
+                                                   {"task": task_id})
+                        if not sprint_task:
+                            exit(f"Task id {task_id} is not part of any sprint")
+                        else:
+                            sprint_task_id = sprint_task[0].id
+                    self.repo.update(SprintTask, sprint_task_id,
+                                         {"story_points": story_points})
             session.commit()
         elif command == "create":
             kwargs["created_by"] = services.lookup_user_id(
-                self.config.get("user"),
-                self.repo)
+                self.config.get("user"), self.repo)
             obj = entity(**kwargs)
             if entity in (Task, Project):
                 if (existing_obj := self.repo.list(entity,
                                                    {"name": obj.name})):
                     print("Found existing entity\n")
                     existing_id = str(existing_obj[0].id)
                     self.execute("show", entity_type, {"id": existing_id})
@@ -751,16 +822,15 @@
                 self.execute("create", "time_entry", kwargs)
             else:
                 exit("tracking missing -H (hours) or -M (minutes) value")
         else:
             raise ValueError(f"Uknown command: {command}")
 
     def _read_config(self) -> Dict[str, Any]:
-        with open(f"{self.home_dir}/.terka/config.yaml",
-                  "r",
+        with open(f"{self.home_dir}/.terka/config.yaml", "r",
                   encoding="utf-8") as f:
             config = yaml.safe_load(f)
         return config
 
 
 def get_ids(ids: Union[str, int]) -> List[Union[int, str]]:
     id_string = str(ids)
```

### Comparing `terka-1.3.3/src/domain/commentary.py` & `terka-1.4.0/src/domain/commentary.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,7 +26,37 @@
 
     def __init__(self, id: int,
                  text: str,
                  date: datetime = datetime.now(), **kwargs: str) -> None:
         self.project = id
         super().__init__(text=text,
                          date=date)
+
+
+class EpicCommentary(BaseCommentary):
+
+    def __init__(self, id: int,
+                 text: str,
+                 date: datetime = datetime.now(), **kwargs: str) -> None:
+        self.epic = id
+        super().__init__(text=text,
+                         date=date)
+
+
+class StoryCommentary(BaseCommentary):
+
+    def __init__(self, id: int,
+                 text: str,
+                 date: datetime = datetime.now(), **kwargs: str) -> None:
+        self.story = id
+        super().__init__(text=text,
+                         date=date)
+
+
+class SprintCommentary(BaseCommentary):
+
+    def __init__(self, id: int,
+                 text: str,
+                 date: datetime = datetime.now(), **kwargs: str) -> None:
+        self.sprint = id
+        super().__init__(text=text,
+                         date=date)
```

### Comparing `terka-1.3.3/src/domain/epic.py` & `terka-1.4.0/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/event_history.py` & `terka-1.4.0/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/project.py` & `terka-1.4.0/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/sprint.py` & `terka-1.4.0/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/story.py` & `terka-1.4.0/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/tag.py` & `terka-1.4.0/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/task.py` & `terka-1.4.0/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/time_tracker.py` & `terka-1.4.0/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/domain/user.py` & `terka-1.4.0/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/entrypoints/cli.py` & `terka-1.4.0/src/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/service_layer/printer.py` & `terka-1.4.0/src/service_layer/printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                           entity.date.strftime("%Y-%m-%d %H:%M"), entity.text)
         self.console.print(table)
 
     def print_epic(self, entities, repo, show_tasks=True):
         table = Table(box=self.box, title="EPICS", expand=True)
         for column in ("id", "name", "description", "project", "tasks"):
             table.add_column(column, style="bold")
-        for entity in entities:
+        for i, entity in enumerate(entities):
             tasks = []
             for epic_task in entity.epic_tasks:
                 task = epic_task.tasks
                 tasks.append(task)
             try:
                 project_obj = services.lookup_project_name(
                     entity.project, repo)
@@ -159,21 +159,24 @@
             table.add_row(f"E{entity.id}", str(entity.name),
                           entity.description, project, str(len(tasks)))
         self.console.print(table)
         if show_tasks:
             self.print_task(entities=tasks,
                             repo=repo,
                             show_completed=True,
-                            show_window=False)
+                            show_window=False,
+                            show_history_comments=False)
+        if i == 0 and (commentaries := entity.commentaries):
+            self.print_commentaries(commentaries)
 
     def print_story(self, entities, repo, show_tasks=True):
         table = Table(box=self.box, title="STORIES", expand=True)
         for column in ("id", "name", "description", "project", "tasks"):
             table.add_column(column, style="bold")
-        for entity in entities:
+        for i, entity in enumerate(entities):
             tasks = []
             for story_task in entity.story_tasks:
                 task = story_task.tasks
                 tasks.append(task)
             try:
                 project_obj = services.lookup_project_name(
                     entity.project, repo)
@@ -183,23 +186,26 @@
             table.add_row(f"S{entity.id}", str(entity.name),
                           entity.description, project, str(len(tasks)))
         self.console.print(table)
         if show_tasks and tasks:
             self.print_task(entities=tasks,
                             repo=repo,
                             show_completed=True,
-                            show_window=False)
+                            show_window=False,
+                            show_history_comments=False)
+        if i == 0 and (commentaries := entity.commentaries):
+            self.print_commentaries(commentaries)
 
     def print_sprint(self, entities, repo, show_tasks=True):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "start_date", "end_date", "goal", "status",
                        "open tasks", "tasks", "velocity", "collaborators",
                        "time_spent"):
             table.add_column(column)
-        for entity in entities:
+        for i, entity in enumerate(entities):
             story_points = []
             tasks = []
             collaborators = []
             collaborators_dict = defaultdict(int)
             for sprint_task in entity.sprint_tasks:
                 story_points.append(sprint_task.story_points)
                 task = sprint_task.tasks
@@ -234,14 +240,16 @@
                           collaborators_string, str(time_spent))
         self.console.print(table)
         if show_tasks:
             self.print_sprint_task(entities=tasks,
                                    repo=repo,
                                    show_completed=True,
                                    story_points=story_points)
+        if i == 0 and (commentaries := entity.commentaries):
+            self.print_commentaries(commentaries)
 
     def print_project(self,
                       entities,
                       zero_tasks: bool = False,
                       zero_tasks_only: bool = False,
                       show_tasks: bool = True,
                       show_completed_tasks: bool = False):
```

### Comparing `terka-1.3.3/src/service_layer/services.py` & `terka-1.4.0/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/service_layer/ui.py` & `terka-1.4.0/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/service_layer/vertical_layout.css` & `terka-1.4.0/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/src/utils.py` & `terka-1.4.0/src/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,17 @@
             "stale":
             new_dict.get("stale"),
             "goal": new_dict.get("goal"),
             "start_date":
             convert_date(new_dict.get("start-date")),
             "end_date":
             convert_date(new_dict.get("end-date")),
-            "sprint_id": new_dict.get("to-sprint"),
-            "story_id": new_dict.get("to-story"),
-            "epic_id": new_dict.get("to-epic"),
+            "sprint_id": new_dict.get("to-sprint") or new_dict.get("from-sprint") or new_dict.get("sprint"),
+            "story_id": new_dict.get("to-story") or new_dict.get("from-story") or new_dict.get("story"),
+            "epic_id": new_dict.get("to-epic") or new_dict.get("from-epic") or new_dict.get("epic"),
             "story_points": new_dict.get("story-points"),
             "hours": new_dict.get("H"),
             "minutes": new_dict.get("M"),
         }
         if "--show-completed" in kwargs:
             task_dict.update({"show_completed": True})
         if "--sort" in kwargs:
```

### Comparing `terka-1.3.3/terka.egg-info/PKG-INFO` & `terka-1.4.0/terka.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.3.3
+Version: 1.4.0
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.3.3/terka.egg-info/SOURCES.txt` & `terka-1.4.0/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/tests/test_orm.py` & `terka-1.4.0/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/tests/test_task.py` & `terka-1.4.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.3/tests/test_user.py` & `terka-1.4.0/tests/test_user.py`

 * *Files identical despite different names*

