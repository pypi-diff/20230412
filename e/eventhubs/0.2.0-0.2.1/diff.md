# Comparing `tmp/eventhubs-0.2.0.tar.gz` & `tmp/eventhubs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventhubs-0.2.0.tar", last modified: Sat Mar 18 08:29:42 2023, max compression
+gzip compressed data, was "eventhubs-0.2.1.tar", last modified: Wed Apr 12 14:44:24 2023, max compression
```

## Comparing `eventhubs-0.2.0.tar` & `eventhubs-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 08:29:42.913503 eventhubs-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-18 08:29:27.000000 eventhubs-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-18 08:29:42.913503 eventhubs-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-18 08:29:27.000000 eventhubs-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 08:29:42.913503 eventhubs-0.2.0/eventhubs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 08:29:27.000000 eventhubs-0.2.0/eventhubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-18 08:29:27.000000 eventhubs-0.2.0/eventhubs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-03-18 08:29:27.000000 eventhubs-0.2.0/eventhubs/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 08:29:42.913503 eventhubs-0.2.0/eventhubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-18 08:29:42.000000 eventhubs-0.2.0/eventhubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-18 08:29:42.000000 eventhubs-0.2.0/eventhubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 08:29:42.000000 eventhubs-0.2.0/eventhubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-18 08:29:42.000000 eventhubs-0.2.0/eventhubs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-18 08:29:42.000000 eventhubs-0.2.0/eventhubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-18 08:29:42.000000 eventhubs-0.2.0/eventhubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 08:29:42.913503 eventhubs-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-18 08:29:27.000000 eventhubs-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 08:29:42.913503 eventhubs-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-18 08:29:27.000000 eventhubs-0.2.0/tests/test_eventhubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:44:24.478672 eventhubs-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 14:44:09.000000 eventhubs-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-12 14:44:24.478672 eventhubs-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-12 14:44:09.000000 eventhubs-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:44:24.478672 eventhubs-0.2.1/eventhubs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:44:09.000000 eventhubs-0.2.1/eventhubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 14:44:09.000000 eventhubs-0.2.1/eventhubs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-12 14:44:09.000000 eventhubs-0.2.1/eventhubs/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:44:24.478672 eventhubs-0.2.1/eventhubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-12 14:44:24.000000 eventhubs-0.2.1/eventhubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-12 14:44:24.000000 eventhubs-0.2.1/eventhubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:44:24.000000 eventhubs-0.2.1/eventhubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 14:44:24.000000 eventhubs-0.2.1/eventhubs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 14:44:24.000000 eventhubs-0.2.1/eventhubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:44:24.000000 eventhubs-0.2.1/eventhubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:44:24.478672 eventhubs-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-12 14:44:09.000000 eventhubs-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:44:24.478672 eventhubs-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 14:44:09.000000 eventhubs-0.2.1/tests/test_eventhubs.py
```

### Comparing `eventhubs-0.2.0/LICENSE` & `eventhubs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eventhubs-0.2.0/PKG-INFO` & `eventhubs-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventhubs
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI tool to send and receive event data from Azure Event Hubs
 Home-page: https://github.com/zmoog/eventhubs
 Author: Maurizio Branca
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/zmoog/eventhubs/issues
 Project-URL: CI, https://github.com/zmoog/eventhubs/actions
 Project-URL: Changelog, https://github.com/zmoog/eventhubs/releases
@@ -65,14 +65,27 @@
     export EVENTHUB_CONNECTION_STRING="Endpoint=sb://...="
     export EVENTHUB_NAME="application-insights"
 
     eh eventdata receive
 
     eh eventdata receive --name "another-name"
 
+Defaults to printing the message payload only, so it is easier to combine output with other tools, like `jq`:
+
+    $ eh eventdata receive | jq '.records[].tenantId' 
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+
+But you can still turn on verbose and get more information about what's going on:
+
+    $ eh --verbose eventdata receive
+    Receiving events from mbranca
+    Received event from partition 0: {"records": [{....
+
 For help, run:
 
     eventhubs --help
 
 You can also use:
 
     python -m eventhubs --help
```

### Comparing `eventhubs-0.2.0/README.md` & `eventhubs-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,27 @@
     export EVENTHUB_CONNECTION_STRING="Endpoint=sb://...="
     export EVENTHUB_NAME="application-insights"
 
     eh eventdata receive
 
     eh eventdata receive --name "another-name"
 
+Defaults to printing the message payload only, so it is easier to combine output with other tools, like `jq`:
+
+    $ eh eventdata receive | jq '.records[].tenantId' 
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+
+But you can still turn on verbose and get more information about what's going on:
+
+    $ eh --verbose eventdata receive
+    Receiving events from mbranca
+    Received event from partition 0: {"records": [{....
+
 For help, run:
 
     eventhubs --help
 
 You can also use:
 
     python -m eventhubs --help
```

### Comparing `eventhubs-0.2.0/eventhubs/cli.py` & `eventhubs-0.2.1/eventhubs/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,22 @@
     envvar="EVENTHUB_CONSUMER_GROUP",
 )
 @click.option(
     "--name",
     required=True,
     envvar="EVENTHUB_NAME",
 )
-@click.option('--verbose', '-v', is_flag=True, help="Enable verbose mode", default=False)
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    help="Enables verbose mode",
+    default=False,
+    envvar="EVENTHUB_VERBOSE",
+)
 @click.pass_context
 def cli(ctx: click.Context, connection_string: str, consumer_group: str, name: str, verbose: bool):
     """CLI tool to send and receive event data from Azure Event Hubs"""
     ctx.ensure_object(dict)
     ctx.obj['connection_string'] = connection_string
     ctx.obj['consumer_group'] = consumer_group
     ctx.obj['name'] = name
@@ -52,19 +59,23 @@
     consumer = EventHubConsumerClient.from_connection_string(
         ctx.obj['connection_string'],
         ctx.obj['consumer_group'],
         eventhub_name=ctx.obj['name'],
     )
 
     def on_event(partition_context, event: EventData):
-        print(f"Received event from partition {partition_context.partition_id}: {event.body_as_str()}")
+        if ctx.obj['verbose']:
+            print(f"Received event from partition {partition_context.partition_id}: {event.body_as_str()}")
+        else:
+            print(event.body_as_str())
         partition_context.update_checkpoint(event)
 
     with consumer:
-        print(f"Receiving events from {ctx.obj['name']}")
+        if ctx.obj['verbose']:
+            print(f"Receiving events from {ctx.obj['name']}")
         consumer.receive(
             on_event=on_event,
             starting_position=starting_position,
         )    
 
 
 @eventdata.command(name="send")
@@ -116,14 +127,15 @@
                 print(f"adding {event}")
             try:
                 batch.add(EventData(event))
             except ValueError as e:
                 # if the batch is full, we send the
                 # current one and the create a brand
                 # new one for the remaining events
-                print("Event data batch is full ({} events).".format(len(batch)))
+                if ctx.obj['verbose']:
+                    print("Event data batch is full ({} events).".format(len(batch)))
                 producer.send_batch(batch)
                 batch = producer.create_batch()
                 batch.add(EventData(event))
 
         if len(batch) > 0:
             producer.send_batch(batch)
```

### Comparing `eventhubs-0.2.0/eventhubs.egg-info/PKG-INFO` & `eventhubs-0.2.1/eventhubs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventhubs
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI tool to send and receive event data from Azure Event Hubs
 Home-page: https://github.com/zmoog/eventhubs
 Author: Maurizio Branca
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/zmoog/eventhubs/issues
 Project-URL: CI, https://github.com/zmoog/eventhubs/actions
 Project-URL: Changelog, https://github.com/zmoog/eventhubs/releases
@@ -65,14 +65,27 @@
     export EVENTHUB_CONNECTION_STRING="Endpoint=sb://...="
     export EVENTHUB_NAME="application-insights"
 
     eh eventdata receive
 
     eh eventdata receive --name "another-name"
 
+Defaults to printing the message payload only, so it is easier to combine output with other tools, like `jq`:
+
+    $ eh eventdata receive | jq '.records[].tenantId' 
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+    "1de2b364-21e1-4866-bb46-7804f17c417d"
+
+But you can still turn on verbose and get more information about what's going on:
+
+    $ eh --verbose eventdata receive
+    Receiving events from mbranca
+    Received event from partition 0: {"records": [{....
+
 For help, run:
 
     eventhubs --help
 
 You can also use:
 
     python -m eventhubs --help
```

### Comparing `eventhubs-0.2.0/setup.py` & `eventhubs-0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

