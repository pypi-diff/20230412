# Comparing `tmp/async_sqs_consumer-0.3.6.tar.gz` & `tmp/async_sqs_consumer-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_sqs_consumer-0.3.6.tar", max compression
+gzip compressed data, was "async_sqs_consumer-0.3.7.tar", max compression
```

## Comparing `async_sqs_consumer-0.3.6.tar` & `async_sqs_consumer-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2410 2023-03-31 13:48:41.692048 async_sqs_consumer-0.3.6/README.md
--rw-r--r--   0        0        0        0 2023-03-31 14:08:47.294687 async_sqs_consumer-0.3.6/async_sqs_consumer/__init__.py
--rw-r--r--   0        0        0     4682 2023-04-11 18:06:55.645770 async_sqs_consumer-0.3.6/async_sqs_consumer/queue.py
--rw-r--r--   0        0        0     2254 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.6/async_sqs_consumer/resources.py
--rw-r--r--   0        0        0        0 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.6/async_sqs_consumer/test/__init__.py
--rw-r--r--   0        0        0      542 2023-04-02 17:24:04.634142 async_sqs_consumer-0.3.6/async_sqs_consumer/test/send_message.py
--rw-r--r--   0        0        0      543 2023-04-11 18:44:09.667026 async_sqs_consumer-0.3.6/async_sqs_consumer/test/server.py
--rw-r--r--   0        0        0      753 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.6/async_sqs_consumer/types.py
--rw-r--r--   0        0        0      486 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.6/async_sqs_consumer/utils/__init__.py
--rw-r--r--   0        0        0     1365 2023-03-31 15:12:56.460833 async_sqs_consumer-0.3.6/async_sqs_consumer/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5522 2023-04-11 14:12:54.911336 async_sqs_consumer-0.3.6/async_sqs_consumer/utils/__pycache__/retry.cpython-311.pyc
--rw-r--r--   0        0        0     3803 2023-04-11 12:49:23.872046 async_sqs_consumer-0.3.6/async_sqs_consumer/utils/retry.py
--rw-r--r--   0        0        0    10106 2023-04-11 18:43:37.009724 async_sqs_consumer-0.3.6/async_sqs_consumer/worker.py
--rw-r--r--   0        0        0      647 2023-04-11 19:40:19.723405 async_sqs_consumer-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.6/setup.py
--rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     2410 2023-03-31 13:48:41.692048 async_sqs_consumer-0.3.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-31 14:08:47.294687 async_sqs_consumer-0.3.7/async_sqs_consumer/__init__.py
+-rw-r--r--   0        0        0     4682 2023-04-11 18:06:55.645770 async_sqs_consumer-0.3.7/async_sqs_consumer/queue.py
+-rw-r--r--   0        0        0     2254 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.7/async_sqs_consumer/resources.py
+-rw-r--r--   0        0        0        0 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.7/async_sqs_consumer/test/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-02 17:24:04.634142 async_sqs_consumer-0.3.7/async_sqs_consumer/test/send_message.py
+-rw-r--r--   0        0        0      543 2023-04-11 18:44:09.667026 async_sqs_consumer-0.3.7/async_sqs_consumer/test/server.py
+-rw-r--r--   0        0        0      753 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.7/async_sqs_consumer/types.py
+-rw-r--r--   0        0        0      486 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.7/async_sqs_consumer/utils/__init__.py
+-rw-r--r--   0        0        0     1365 2023-03-31 15:12:56.460833 async_sqs_consumer-0.3.7/async_sqs_consumer/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5522 2023-04-11 14:12:54.911336 async_sqs_consumer-0.3.7/async_sqs_consumer/utils/__pycache__/retry.cpython-311.pyc
+-rw-r--r--   0        0        0     3803 2023-04-11 12:49:23.872046 async_sqs_consumer-0.3.7/async_sqs_consumer/utils/retry.py
+-rw-r--r--   0        0        0    10098 2023-04-11 22:05:33.291753 async_sqs_consumer-0.3.7/async_sqs_consumer/worker.py
+-rw-r--r--   0        0        0      647 2023-04-11 22:06:08.746182 async_sqs_consumer-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.7/setup.py
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.7/PKG-INFO
```

### Comparing `async_sqs_consumer-0.3.6/README.md` & `async_sqs_consumer-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/queue.py` & `async_sqs_consumer-0.3.7/async_sqs_consumer/queue.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/resources.py` & `async_sqs_consumer-0.3.7/async_sqs_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/test/send_message.py` & `async_sqs_consumer-0.3.7/async_sqs_consumer/test/send_message.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/test/server.py` & `async_sqs_consumer-0.3.7/async_sqs_consumer/test/server.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/types.py` & `async_sqs_consumer-0.3.7/async_sqs_consumer/types.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/utils/__pycache__/__init__.cpython-311.pyc` & `async_sqs_consumer-0.3.7/async_sqs_consumer/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/utils/__pycache__/retry.cpython-311.pyc` & `async_sqs_consumer-0.3.7/async_sqs_consumer/utils/__pycache__/retry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/utils/retry.py` & `async_sqs_consumer-0.3.7/async_sqs_consumer/utils/retry.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.6/async_sqs_consumer/worker.py` & `async_sqs_consumer-0.3.7/async_sqs_consumer/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
                 if len(
                     [
                         task
                         for task in asyncio.all_tasks(asyncio.get_event_loop())
                         if task.get_name().startswith(TASK_NAME_PREFIX)
                     ]
                 ) > (self._max_workers):
-                    await sleep(1)  # type: ignore
+                    await asyncio.sleep(1)
                     continue
 
                 for queue_alias, queue in queues:
                     messages = await queue.get_messages(sqs_client)
                     await asyncio.gather(
                         *[
                             self._consumer_callback(message, queue_alias)
```

### Comparing `async_sqs_consumer-0.3.6/pyproject.toml` & `async_sqs_consumer-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_sqs_consumer"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["Diego Restrepo <drestrepo@fluidattacks.com>"]
 repository = 'https://github.com/drestrepom/async_sqs_consumer'
 readme = "README.md"
 keywords = ["AWS", "AWS", "SQS", "sqs", "consumer", "async", "worker"]
 
 [tool.poetry.dependencies]
```

### Comparing `async_sqs_consumer-0.3.6/setup.py` & `async_sqs_consumer-0.3.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'aiohttp>=3.8.4,<4.0.0',
  'jsonschema>=4.17.3,<5.0.0',
  'pyrate-limiter>=2.10.0,<3.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'async-sqs-consumer',
-    'version': '0.3.6',
+    'version': '0.3.7',
     'description': '',
     'long_description': '# Async SQS consumer\n\nPython asynchronous (**async** / **await**) worker for consuming messages\nfrom AWS SQS.\n\nThis is a hobby project, if you find the project interesting\nany contribution is welcome.\n\n## Usage\n\nYou must create an instance of the worker with the url of the queue.\n\nAws credentials are taken from environment variables, you must set the\nfollowing environment variables. Or you can provide a Context object with the\naws credentials `async_sqs_consumer.types.Context`\n\n- `AWS_ACCESS_KEY_ID`\n- `AWS_SECRET_ACCESS_KEY`\n\nExample:\n\nYou can get the queue url with the follow aws cli command\n`aws sqs get-queue-url --queue-name xxxxxx`\n\n```python\n# test_worker.py\n\nfrom async_sqs_consumer.worker import (\n    Worker,\n)\n\nworker = Worker(\n    queue_url="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name"\n)\n\n\n@worker.task("report")\nasync def report(text: str) -> None:\n    print(text)\n\nif __name__: "__main__":\n    worker.start()\n```\n\nNow you can initialize the worker `python test_worker.py`\n\nNow you need to post a message for the worker to process\n\n```python\nimport json\nimport boto3\nimport uuid\n\nclient = boto3.client("sqs")\n\nclient.send_message(\n    QueueUrl="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name",\n    MessageBody=json.dumps(\n        {\n            "task": "report",\n            "id": uuid.uuid4().hex,\n            "args": ["hello world"],\n        }\n    ),\n)\n```\n\nOr you can use aioboto3\n\n```python\nimport asyncio\nimport json\nimport aioboto3\nimport uuid\n\n\nasync def main() -> None:\n    session = aioboto3.Session()\n    async with session.client("sqs") as client:\n        await client.send_message(\n            QueueUrl="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name",\n            MessageBody=json.dumps(\n                {\n                    "task": "report",\n                    "id": uuid.uuid4().hex,\n                    "args": ["hello world"],\n                }\n            ),\n        )\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo publish the messages they must have the following structure\n\n```json\n{\n    "type": "object",\n    "properties": {\n        "task": {"type": "string"},\n        "id": {"type": "string"},\n        "args": {"type": "array"},\n        "kwargs": {"type": "object"},\n        "retries": {"type": "number"},\n        "eta": {"type": "string"},\n        "expires": {"type": "string"},\n    },\n    "required": ["task", "id"],\n}\n```\n',
     'author': 'Diego Restrepo',
     'author_email': 'drestrepo@fluidattacks.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/drestrepom/async_sqs_consumer',
```

### Comparing `async_sqs_consumer-0.3.6/PKG-INFO` & `async_sqs_consumer-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-sqs-consumer
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Home-page: https://github.com/drestrepom/async_sqs_consumer
 Keywords: AWS,AWS,SQS,sqs,consumer,async,worker
 Author: Diego Restrepo
 Author-email: drestrepo@fluidattacks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

