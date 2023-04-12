# Comparing `tmp/kedro-prefect-oliver-0.1.2.tar.gz` & `tmp/kedro-prefect-oliver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-prefect-oliver-0.1.2.tar", last modified: Wed Mar 29 21:57:47 2023, max compression
+gzip compressed data, was "kedro-prefect-oliver-0.1.3.tar", last modified: Wed Apr 12 14:29:02 2023, max compression
```

## Comparing `kedro-prefect-oliver-0.1.2.tar` & `kedro-prefect-oliver-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-03-29 21:57:47.467129 kedro-prefect-oliver-0.1.2/
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)     1140 2023-03-14 19:43:11.000000 kedro-prefect-oliver-0.1.2/LICENSE
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      577 2023-03-29 21:57:47.466982 kedro-prefect-oliver-0.1.2/PKG-INFO
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)     4582 2023-03-14 19:43:11.000000 kedro-prefect-oliver-0.1.2/README
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)     5684 2023-03-29 21:57:26.000000 kedro-prefect-oliver-0.1.2/pyproject.toml
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)       38 2023-03-29 21:57:47.467176 kedro-prefect-oliver-0.1.2/setup.cfg
-drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-03-29 21:57:47.464528 kedro-prefect-oliver-0.1.2/src/
-drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-03-29 21:57:47.465747 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver/
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      122 2023-03-24 12:46:02.000000 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver/__init__.py
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)     2068 2023-03-24 12:46:03.000000 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver/infrastructure.py
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)    13152 2023-03-29 21:57:26.000000 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver/register.py
-drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-03-29 21:57:47.466781 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver.egg-info/
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      577 2023-03-29 21:57:47.000000 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver.egg-info/PKG-INFO
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      385 2023-03-29 21:57:47.000000 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver.egg-info/SOURCES.txt
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)        1 2023-03-29 21:57:47.000000 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver.egg-info/dependency_links.txt
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      366 2023-03-29 21:57:47.000000 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver.egg-info/requires.txt
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)       21 2023-03-29 21:57:47.000000 kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4582 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/README
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/infrastructure.py
+-rw-rw-rw-   0 root         (0) root         (0)    13601 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/register.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/top_level.txt
```

### Comparing `kedro-prefect-oliver-0.1.2/LICENSE` & `kedro-prefect-oliver-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.2/PKG-INFO` & `kedro-prefect-oliver-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kedro-prefect-oliver-0.1.2/README` & `kedro-prefect-oliver-0.1.3/README`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.2/pyproject.toml` & `kedro-prefect-oliver-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name =  "kedro-prefect-oliver"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Oliver OTL", email = "dev@olivetreeholdings.com"},
 ]
 description = "Kedro-Prefect integration library"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver/infrastructure.py` & `kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/infrastructure.py`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver/register.py` & `kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/register.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from prefect.filesystems import GCS
 import prefect
 
 import pendulum
 import click
 
 from prefect.utilities.hashing import file_hash
-from prefect.server.schemas.schedules import CronSchedule, IntervalSchedule, RRuleSchedule
+from prefect.server.schemas.schedules import (
+    CronSchedule,
+    IntervalSchedule,
+    RRuleSchedule,
+)
 
 
 class KedroInitTask(object):
     """Task to initialize KedroSession"""
 
     def __init__(
         self,
@@ -111,15 +115,16 @@
 
     # return tasks as it is mutated. We want to make this obvious to the user.
     return node_task, tasks  # type: ignore[return-value]
 
 
 @task
 def run_kedro_task(
-    kedro_task: Union[KedroInitTask, KedroTask], task_dict: Union[None, Dict[str, Union[DataCatalog, str]]] = None
+    kedro_task: Union[KedroInitTask, KedroTask],
+    task_dict: Union[None, Dict[str, Union[DataCatalog, str]]] = None,
 ) -> Union[Dict[str, Union[DataCatalog, str]], None]:
     """Run a Kedro node as a Prefect task."""
     if task_dict is None:
         get_run_logger().info("Initializing Kedro session")
         task_dict = kedro_task.run()
         return task_dict
     else:
@@ -128,15 +133,20 @@
         kedro_task.run(task_dict)
         return None
 
 
 def init_kedro_nodes(
     pipeline_name: str, env: str
 ) -> Dict[
-    str, Union[KedroInitTask, Dict[str, List[KedroTask]], Dict[str, Dict[str, Union[KedroTask, List[KedroTask]]]]]
+    str,
+    Union[
+        KedroInitTask,
+        Dict[str, List[KedroTask]],
+        Dict[str, Dict[str, Union[KedroTask, List[KedroTask]]]],
+    ],
 ]:
     """Register a Kedro pipeline as a Prefect flow."""
     logger = get_run_logger()
     logger.info("Initializing Kedro nodes")
     project_path = Path.cwd()
     logger.info("Project path: %s", project_path)
     metadata = bootstrap_project(project_path)
@@ -175,24 +185,32 @@
 
     kedro_tasks = init_kedro_nodes(pipeline_name, env)
     init_task = kedro_tasks["init_task"]
     tasks = kedro_tasks["tasks"]
 
     run_kedro_init_task = run_kedro_task.with_options(name=init_task.name)
     task_dict = run_kedro_init_task.submit(init_task)
-    task_dependencies = {kedro_task["task"]: kedro_task["parent_tasks"] for kedro_task in tasks.values()}
+    task_dependencies = {
+        kedro_task["task"]: kedro_task["parent_tasks"] for kedro_task in tasks.values()
+    }
     todo_nodes = set([kedro_task["task"] for kedro_task in tasks.values()])
     submitted_tasks: Dict[KedroTask, prefect.Task] = {}
     while True:
-        ready = {node for node in todo_nodes if set(task_dependencies[node]) <= submitted_tasks.keys()}
+        ready = {
+            node
+            for node in todo_nodes
+            if set(task_dependencies[node]) <= submitted_tasks.keys()
+        }
         todo_nodes -= ready
         for node in ready:
             run_kedro_node_task = run_kedro_task.with_options(name=node.name)
             future = run_kedro_node_task.submit(
-                node, task_dict, wait_for=[submitted_tasks[t] for t in task_dependencies[node]]
+                node,
+                task_dict,
+                wait_for=[submitted_tasks[t] for t in task_dependencies[node]],
             )
             submitted_tasks[node] = future
 
         if not todo_nodes:
             break
 
 
@@ -203,45 +221,55 @@
     cron_string: str = None,
     day_or: bool = True,
     timezone: str = "America/New_York",
 ) -> Union[IntervalSchedule, CronSchedule, RRuleSchedule, None]:
     """Create a Prefect schedule for a Kedro pipeline."""
 
     if sum(option is not None for option in [interval, rrule_string, cron_string]) > 1:
-        raise ValueError("Exactly one of interval, rrule_string, or cron_string must be provided.")
+        raise ValueError(
+            "Exactly one of interval, rrule_string, or cron_string must be provided."
+        )
 
     if anchor_date and not interval:
-        raise ValueError("An anchor date can only be provided with an interval schedule.")
+        raise ValueError(
+            "An anchor date can only be provided with an interval schedule."
+        )
 
     schedule = None
     if interval is not None:
         if anchor_date:
             try:
                 pendulum.parse(anchor_date)
             except ValueError:
                 raise ValueError("The anchor date must be a valid date string.")
         interval_schedule = {
             "interval": interval,
             "anchor_date": anchor_date,
             "timezone": timezone,
         }
-        schedule = IntervalSchedule(**{k: v for k, v in interval_schedule.items() if v is not None})
+        schedule = IntervalSchedule(
+            **{k: v for k, v in interval_schedule.items() if v is not None}
+        )
 
     if cron_string is not None:
         cron_schedule = {
             "cron": cron_string,
             "day_or": day_or,
             "timezone": timezone,
         }
-        schedule = CronSchedule(**{k: v for k, v in cron_schedule.items() if v is not None})
+        schedule = CronSchedule(
+            **{k: v for k, v in cron_schedule.items() if v is not None}
+        )
 
     if rrule_string is not None:
         # a timezone in the `rrule_string` gets ignored by the RRuleSchedule constructor
         if "TZID" in rrule_string and not timezone:
-            raise ValueError("A timezone must be provided if the rrule string contains a timezone.")
+            raise ValueError(
+                "A timezone must be provided if the rrule string contains a timezone."
+            )
         schedule = RRuleSchedule(rrule=rrule_string, timezone=timezone)
 
     return schedule
 
 
 def deploy_flow(
     project: str,
@@ -274,61 +302,99 @@
                 req = line.split("#", 1)[0].strip()
                 if req and not req.startswith("--"):
                     requires.append(req)
         requires = " ".join([f"{req}" for req in requires])
 
     version = file_hash(str(Path(__file__).resolve()))
 
-    gcs_path = (kedro_package.replace("_", "-") + "/" + kedro_pipeline.replace("_", "-")).replace(" ", "")
+    gcs_path = (
+        kedro_package.replace("_", "-") + "/" + kedro_pipeline.replace("_", "-")
+    ).replace(" ", "")
     gcs_block_name = gcs_path.replace("/", "-")
     gcs_block = GCS(bucket_path=bucket + "/" + gcs_path, project=project)
     gcs_block.save(gcs_block_name, overwrite=True)
 
     job_name = f"{kedro_package.replace('_', '-')}-kubernetes-job"
     kubernetes_job = KubernetesJob.load(job_name)
 
     parameters = {"pipeline_name": kedro_pipeline, "env": env}
 
     deployment = Deployment.build_from_flow(
         entrypoint=entrypoint,
-        flow=create_pipeline.with_options(name=f"{kedro_package}.{kedro_pipeline}", version=version),
+        flow=create_pipeline.with_options(
+            name=f"{kedro_package}.{kedro_pipeline}", version=version
+        ),
         name="kubernetes-job",
         work_queue_name="kubernetes",
         tags=["kubernetes", "kedro"] + tags or [],
         storage=gcs_block,
         infrastructure=kubernetes_job,
         parameters=parameters,
         infra_overrides={
             "env": {"EXTRA_PIP_PACKAGES": requires},
         }
         if requires
         else {},
-        schedule=create_prefect_schedule(interval, anchor_date, rrule_string, cron_string, day_or, timezone),
+        schedule=create_prefect_schedule(
+            interval, anchor_date, rrule_string, cron_string, day_or, timezone
+        ),
     )
     dep_id = deployment.apply()
     print("Deployment ID: {}".format(dep_id))
 
 
 @click.command()
 @click.option("--project", type=str, required=True)
 @click.option("--entrypoint", type=str, required=True)
 @click.option("--bucket", type=str, required=True)
 @click.option("--kedro_package", type=str, required=True)
 @click.option("--kedro_pipeline", default=None)
 @click.option("--tags", multiple=True, type=str, default=None)
-@click.option("--env", "-e", type=str, default=None, help="Kedro environment to use (e.g. local, dev, prod, etc.")
 @click.option(
-    "--dev", "-d", type=bool, default=False, help="When True, use project dependencies from requirements.lock"
+    "--env",
+    "-e",
+    type=str,
+    default=None,
+    help="Kedro environment to use (e.g. local, dev, prod, etc.",
+)
+@click.option(
+    "--dev",
+    "-d",
+    type=bool,
+    default=False,
+    help="When True, use project dependencies from requirements.lock",
+)
+@click.option(
+    "--interval",
+    type=float,
+    default=None,
+    help="An interval to schedule on, specified in seconds",
+)
+@click.option(
+    "--anchor_date",
+    type=str,
+    default=None,
+    help="The anchor date for an interval schedule",
+)
+@click.option(
+    "--rrule", type=str, default=None, help="Deployment schedule rrule string"
 )
-@click.option("--interval", type=float, default=None, help="An interval to schedule on, specified in seconds")
-@click.option("--anchor_date", type=str, default=None, help="The anchor date for an interval schedule")
-@click.option("--rrule", type=str, default=None, help="Deployment schedule rrule string")
 @click.option("--cron", type=str, default=None, help="Deployment schedule cron string")
-@click.option("--day_or", type=bool, default=True, help="Control how croniter handles `day` and `day_of_week` entries")
-@click.option("--timezone", type=str, default="America/New_York", help="Deployment schedule timezone")
+@click.option(
+    "--day_or",
+    type=bool,
+    default=True,
+    help="Control how croniter handles `day` and `day_of_week` entries",
+)
+@click.option(
+    "--timezone",
+    type=str,
+    default="America/New_York",
+    help="Deployment schedule timezone",
+)
 def deploy_prefect_flow(
     project: str,
     entrypoint: str,
     bucket: str,
     kedro_package: str,
     kedro_pipeline: str,
     tags: List[str],
```

### Comparing `kedro-prefect-oliver-0.1.2/src/kedro_prefect_oliver.egg-info/PKG-INFO` & `kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

