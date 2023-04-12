# Comparing `tmp/tegracli-0.1.3.tar.gz` & `tmp/tegracli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegracli-0.1.3.tar", max compression
+gzip compressed data, was "tegracli-0.2.0.tar", max compression
```

## Comparing `tegracli-0.1.3.tar` & `tegracli-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.1.3/LICENSE
--rw-r--r--   0        0        0     7852 2023-03-01 08:35:01.006655 tegracli-0.1.3/README.md
--rw-r--r--   0        0        0     1309 2023-03-01 08:56:32.138526 tegracli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       65 2023-02-03 16:03:39.614393 tegracli-0.1.3/tegracli/__init__.py
--rw-r--r--   0        0        0     4648 2023-02-03 16:37:42.757844 tegracli-0.1.3/tegracli/dispatch.py
--rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.1.3/tegracli/group.py
--rw-r--r--   0        0        0    11867 2023-03-01 08:39:51.277371 tegracli-0.1.3/tegracli/main.py
--rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.1.3/tegracli/types.py
--rw-r--r--   0        0        0     1578 2023-03-01 08:39:51.253372 tegracli-0.1.3/tegracli/utilities.py
--rw-r--r--   0        0        0     8937 2023-03-01 08:56:38.513936 tegracli-0.1.3/setup.py
--rw-r--r--   0        0        0     8826 2023-03-01 08:56:38.515033 tegracli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8456 2023-04-12 14:05:59.583449 tegracli-0.2.0/README.md
+-rw-r--r--   0        0        0     1322 2023-04-12 14:06:28.899428 tegracli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-04-11 13:51:38.330956 tegracli-0.2.0/tegracli/__init__.py
+-rw-r--r--   0        0        0     5026 2023-04-12 14:05:59.583449 tegracli-0.2.0/tegracli/dispatch.py
+-rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.0/tegracli/group.py
+-rw-r--r--   0        0        0    12827 2023-04-12 14:05:59.587449 tegracli-0.2.0/tegracli/main.py
+-rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.0/tegracli/types.py
+-rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.0/tegracli/utilities.py
+-rw-r--r--   0        0        0     9481 1970-01-01 00:00:00.000000 tegracli-0.2.0/PKG-INFO
```

### Comparing `tegracli-0.1.3/LICENSE` & `tegracli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tegracli-0.1.3/README.md` & `tegracli-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -115,14 +115,37 @@
 
   This function searches Telegram content that is available to your account for the specified search term(s).
 
 Options:
   --help  Show this message and exit.
 ```
 
+## HYDRATE
+
+To rehydrate messages from the API this command accepts a file with message IDs in the format of `$channel_name/$post_number`.
+Both input and output file are optional, if not given, `stdin` and `stdout` are used.
+
+Output data is JSONL, one message per line.
+
+```text
+Usage: tegracli hydrate [OPTIONS] [INPUT_FILE] [OUTPUT_FILE]
+
+  Hydrate a file with messages-ids.
+
+Options:
+  --help  Show this message and exit.
+```
+
+For example, to rehydrate message IDs:
+
+```bash
+echo test_channel/1234 | tegracli hydrate
+>> {"_":"Message","id": 1234, ... , "restriction_reason":[],"ttl_period":null}
+```
+
 ## GROUP INIT and GROUP RUN
 
 In order to support updatable  and long-running collections `tegracli` sports an *account group* feature which retrieves
 the history of a given set of accounts and is able to retrieve updates on each of these accounts.
 
 Groups are initialized by calling `teracli group init`, where accounts to track are stated by either stating them as arguments
 or by reading in a file.
```

### Comparing `tegracli-0.1.3/pyproject.toml` & `tegracli-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tegracli"
-version = "0.1.3"
+version = "0.2.0"
 description = "A research-focused Telegram CLI application"
 authors = ["Philipp Kessling <p.kessling@leibniz-hbi.de>", "Felix Münch <f.muench@lebniz-hbi.de>"]
 readme  = "README.md"
 license = "MIT"
 repository  = "https://github.com/Leibniz-HBI/tegracli"
 homepage = "https://pypi.org/project/tegracli/"
 classifiers = [
@@ -28,14 +28,15 @@
 pytest-socket = "^0.5.1"
 pytest-asyncio = "^0.18.3"
 black = "^22.6.0"
 isort = "^5.10.1"
 pytest-cov = "^3.0.0"
 coverage = "^6.4.2"
 pydocstyle = "^6.1.1"
+pylint = "*"
 
 [tool.pytest.ini_options]
 addopts = "--disable-socket --cov-report html:tests/coverage --cov=tegracli --capture=sys"
 asyncio_mode = "strict"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `tegracli-0.1.3/tegracli/dispatch.py` & `tegracli-0.2.0/tegracli/dispatch.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 from loguru import logger as log
 from telethon import TelegramClient
 from telethon.errors import FloodWaitError
 
 from .types import MessageHandler
 from .utilities import str_dict
 
+# pylint: disable=I1101  # c-extensions-no-member; we know it's there and that's why we don't
+# want to see it
+
 
 async def dispatch_iter_messages(
     client: TelegramClient, params: Dict, callback: MessageHandler
 ) -> None:
-    """Dispatch a a TG-method with callback.
+    """Dispatch a TG-method with callback.
 
-    Parameters:
-        client : TelegramClient
-        params : Dict
-        callback : MessageHandler
+    Args:
+        client: the client to use.
+        params: the parameters to pass to the method.
+        callback: the callback to pass data to.
     """
     async for message in client.iter_messages(wait_time=10, **params):
         await callback(message)
 
 
 async def dispatch_get(users, client: TelegramClient, params: Dict):
     """Get the message history of a specified set of users."""
-
     for user in users:
         done = False
         while done is False:
             try:
                 if str.isnumeric(user):
                     user = int(user)
                 other = await client.get_entity(user)  # see https://limits.tginfo.me/en
@@ -57,18 +59,32 @@
             except ValueError as err:
                 log.error(f"No dice for {user}, because {err}")
                 done = True
                 continue
             done = True
 
 
+async def dispatch_hydrate(
+    channel: str,
+    post_ids: List[str],
+    output_file: TextIOWrapper,
+    client: TelegramClient,
+):
+    """Dispatch a hydration by channel_id/post_id."""
+    await dispatch_iter_messages(
+        client,
+        {"entity": channel, "ids": post_ids},
+        partial(handle_message, file=output_file, injects=None),
+    )
+
+
 async def dispatch_search(queries: List[str], client: TelegramClient):
     """Dispatch a global search."""
     local_account = await client.get_me()
-    log.info(f"Using telegram accout of {local_account.username}")
+    log.info(f"Using telegram account of {local_account.username}")
     for query in queries:
         try:
             async for message in client.iter_messages(None, search=query, limit=15):
                 with Path(f"{query}.jsonl").open("a", encoding="utf8") as file:
                     m_dict = message.to_dict()
                     ujson.dump(  # pylint: disable=c-extension-no-member
                         str_dict(m_dict), file
@@ -80,63 +96,52 @@
 
 
 async def handle_message(
     message: telethon.types.Message, file: TextIOWrapper, injects: Optional[Dict]
 ):
     """Accept incoming messages and log them to disk.
 
-    Parameters
-    ----------
-
-    message : telethon.types.Message : incoming single message
-    file : TextIOWrapper : opened file to dump the message's json into
-
-    Returns
-    -------
-
-    None : nada, nothing
+    Args:
+        message: incoming single message.
+        file: opened file to dump the message's json into.
+        injects: additional data to inject into the message.
     """
-    # log.debug(f"Received {message.peer_id.channel_id}/{message.id}")
     m_dict = str_dict(message.to_dict())
     if injects is not None:
         for key, value in injects.items():
             m_dict[key] = value
     # print(str(m_dict))
     ujson.dump(m_dict, file, ensure_ascii=True)
     file.write("\n")
 
 
 async def get_input_entity(
     client: TelegramClient, member_id: int
 ) -> Optional[telethon.types.TypeInputPeer]:
     """Wraps the client.get_input_entity function.
 
-    Parameters
-    ----------
+    Args:
+        client: signed in TG client.
+        member_id: id/handle/URL of the entity to get.
 
-    client : TelegramClient : signed in TG client
-    member_id : int : id/handle/URL of the entity to get
-
-    Returns
-    -------
-    Optional[telethon.types.TypeInputPeer] : returns the requested entity or None
+    Returns:
+        Optional[telethon.types.TypeInputPeer] : returns the requested entity or None
     """
     return await client.get_input_entity(member_id)
 
 
 async def get_profile(
     client: TelegramClient, member: str, group_name: str
 ) -> Optional[Dict[str, str]]:
     """Returns a Dict from the requested entity.
 
-    Parameters
-    ----------
-
-    client : TelegramClient : signed in TG client
-    member : str : id/handle/URL of the entity to request
+    Args:
+        client: signed in TG client.
+        member: id/handle/URL of the entity to request.
+        group_name: name of the group to save the profile to.
     """
     _member = int(member) if str.isnumeric(member) else member
     profile = await client.get_entity(_member)
     p_dict: Dict[str, str] = str_dict(profile.to_dict())
     with (Path(group_name) / "profiles.jsonl").open("a") as profiles:
         ujson.dump(p_dict, profiles)
         profiles.write("\n")
```

### Comparing `tegracli-0.1.3/tegracli/group.py` & `tegracli-0.2.0/tegracli/group.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.1.3/tegracli/main.py` & `tegracli-0.2.0/tegracli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import telethon
 import yaml
 from loguru import logger as log
 from telethon import TelegramClient
 
 from .dispatch import (
     dispatch_get,
+    dispatch_hydrate,
     dispatch_iter_messages,
     dispatch_search,
     get_input_entity,
     get_profile,
     handle_message,
 )
 from .group import Group
@@ -76,14 +77,40 @@
 
     client = get_client(config_dict)
 
     client.loop.run_until_complete(ensure_authentication(client, _handle_auth))
 
 
 @cli.command()
+@click.argument("input_file", type=click.File("r", encoding="utf-8"), default="-")
+@click.argument("output_file", type=click.File("w", encoding="utf-8"), default="-")
+@click.pass_context
+def hydrate(ctx: click.Context, input_file: click.File, output_file: click.File):
+    """Hydrate a file with messages-ids."""
+    client = get_client(ctx.obj["credentials"])
+
+    channel_registry = {}
+    for message_id in input_file:
+        channel, post_id = message_id.split("/")
+
+        post_id = int(post_id)
+        if post_id is None:
+            continue
+        if channel not in channel_registry:
+            channel_registry[channel] = [post_id]
+        else:
+            channel_registry[channel].append(post_id)
+    with client:
+        for channel, post_ids in channel_registry.items():
+            client.loop.run_until_complete(
+                dispatch_hydrate(channel, post_ids, output_file, client)
+            )
+
+
+@cli.command()
 @click.option(
     "--limit", "-l", type=int, default=-1, help="Number of messages to retrieve."
 )
 @click.option(
     "--offset_date",
     "-O",
     type=click.DateTime(["%Y-%m-%d"]),
```

### Comparing `tegracli-0.1.3/tegracli/utilities.py` & `tegracli-0.2.0/tegracli/utilities.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.1.3/setup.py` & `tegracli-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,240 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tegracli
+Version: 0.2.0
+Summary: A research-focused Telegram CLI application
+Home-page: https://pypi.org/project/tegracli/
+License: MIT
+Author: Philipp Kessling
+Author-email: p.kessling@leibniz-hbi.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: Telethon (>=1.24.0,<2.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: ujson (>=5.4.0,<6.0.0)
+Project-URL: Repository, https://github.com/Leibniz-HBI/tegracli
+Description-Content-Type: text/markdown
 
-packages = \
-['tegracli']
+# tegracli
 
-package_data = \
-{'': ['*']}
+![The TEGRACLI logo](https://github.com/Leibniz-HBI/tegracli/blob/trunk/tegracli.png?raw=true)
 
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'Telethon>=1.24.0,<2.0.0',
- 'click>=8.1.3,<9.0.0',
- 'loguru>=0.6.0,<0.7.0',
- 'pandas>=1.4.3,<2.0.0',
- 'ujson>=5.4.0,<6.0.0']
-
-entry_points = \
-{'console_scripts': ['tegracli = tegracli.main:cli']}
-
-setup_kwargs = {
-    'name': 'tegracli',
-    'version': '0.1.3',
-    'description': 'A research-focused Telegram CLI application',
-    'long_description': "# tegracli\n\n![The TEGRACLI logo](https://github.com/Leibniz-HBI/tegracli/blob/trunk/tegracli.png?raw=true)\n\nA convenience wrapper around Telethon and the Telegram Client API for research purposes.\n\n# Installation Instructions\n\n`tegracli` uses Poetry and python >= 3.9 and < 4.0 for building and installing.\n\nTo install using pipx, run the following command `pipx install tegracli`.\n\n## How to get API keys\n\nIf you don't have API keys for Telegram, head over to [my.telegram.org](https://my.telegram.org).\nClick on [API development tools](https://my.telegram.org/apps), fill the form to create yourself an app and pluck the keys into `tegracli.conf.yml`. The session name can be arbitrary.\n\n```yaml\napi_id: 1234567\napi_hash : some12321hashthatmustbehere123\nsession_name: somesessionyo\n```\n\nThis template file is provided with the repository.\n\n# Usage\n\n`tegracli` is a terminal application to access the Telegram API for research purposes.\nIn order to retrieve messages the configuration-file from the section before must be present in the directory you start `tegracli`.\n\nThe following commands are available:\n\n## CONFIGURE\n\nOpens an interactive prompt for configuring API-access. Aks you to input your API id, API hash and session name and requests\na 2FA code from Telegram.\n\n```text\nUsage: tegracli configure [OPTIONS]\n\n  Configure tegracli.\n\nOptions:\n  --help  Show this message and exit.\n```\n\n## GET\n\nTo _get_ messages from a number of channels, use this command.\n\n```text\nUsage: tegracli get [OPTIONS] [CHANNELS]...\n\n  Get messages for the specified channels by either ID or username.\n\nOptions:\n  -l, --limit INTEGER           Number of messages to retrieve.\n  -O, --offset_date [%Y-%m-%d]  Offset retrieval to specific date in YYYY-MM-\n                                DD format.\n  -o, --offset_id INTEGER       Offset retrieval to a specific post number.\n  -m, --min_id INTEGER          Minimal post number.\n  -M, --max_id INTEGER          Maximal post number\n  -a, --add_offset INTEGER      Add an offset to the post numbers to be\n                                retrieved.\n  -f, --from_user TEXT          Only messages from this user.\n  --reverse / --forward         Should post numbers count upward or downward.\n                                Defaults to forward.\n  -r, --reply_to TEXT           Only messages replied to specific post id.\n  --help                        Show this message and exit.\n```\n\n| **parameter**       | **description**                                                                                                              |\n|---------------------|------------------------------------------------------------------------------------------------------------------------------|\n| **channels**        | a list of of either telegram usernames, channel or group URLs or user IDs.                                                   |\n| **limit**           | number of messages to retrieve, positive integer. If set to `-1` , retrieves all messages in the channel. defaults to `-1`.  |\n| **offset_date**     | specify start point of retrieval by date, retrieval direction is controlled by `reverse/forward`. Format must be YYYY-MM-DD. |\n| **offset_id**       | specify start point of retrieval by post number, retrieval direction is controlled by `reverse/forward`.                     |\n| **min_id**          | sets the minimum post number                                                                                                 |\n| **max_id**          | sets the maximum post number                                                                                                 |\n| **add_offset**      | add a offset to the post numbers to be retrieved                                                                             |\n| **from_user**       | limit messages to posts *from* a specific user                                                                               |\n| **reply_to**        | limit messages to replies *to* a specific user                                                                               |\n| **reverse/forward** | flag to indicate whether messages should be retrieved in chronological or reverse chronological order.                       |\n\n### Basic Examples\n\nTo retrieve the last fifty messages from a Telegram channel:\n\n```bash\ntegracli get --limit 50 corona_infokanal_bmg\n```\n\nTo retrieve the entire history starting with post #1 of a channel, set `limit` to `-1`.\n\n```bash\ntegracli get --reverse --limit -1 corona_infokanal_bmg\n```\nTo retrieve messages sent after January, 1st 2022:\n\n```bash\ntegracli get --offset_date 2022-01-01 corona_infokanal_bmg\n```\n\nTo retrieve message sent before January, 1st 2022:\n\n```bash\ntegracli get --reverse --offset_date 2022-01-01 corona_infokanal_bmg\n```\n## SEARCH\n\nTo _search_ messages of your chats and groups and channels you are subscribed to, use this command.\n\n```text\nUsage: tegracli search [OPTIONS] [QUERIES]...\n\n  This function searches Telegram content that is available to your account for the specified search term(s).\n\nOptions:\n  --help  Show this message and exit.\n```\n\n## GROUP INIT and GROUP RUN\n\nIn order to support updatable  and long-running collections `tegracli` sports an *account group* feature which retrieves\nthe history of a given set of accounts and is able to retrieve updates on each of these accounts.\n\nGroups are initialized by calling `teracli group init`, where accounts to track are stated by either stating them as arguments\nor by reading in a file.\n\n### Account Group File Format\n\nAccount files are expected to follow these requirements:\n\n- UTF8 text document,\n- per line one account, given as either username, channel-URL or ID,\n- there shall be no header and  no additional columns\n\n```text\nUsage: tegracli group init [OPTIONS] NAME [ACCOUNTS]...\n\n  initialize a new account group\n\nOptions:\n  -f, --read_file PATH         read an account list from a file, one\n                               handle/id/url per line.\n  -s, --start_date [%Y-%m-%d]  Start date for the collection. Must be in YYYY-\n                               MM-DD format.\n  -l, --limit INTEGER          number of posts fo retrieve in one run\n  --help                       Show this message and exit.\n```\n\nA group is essentially a directory in your tegracli project folder which holdes\na group configuration file, a `profiles.jsonl` file which will collect all user objects returned\nby Telegram (these will be recycled to save API requests), as well as the jsonl-files containing the messages.\nThe messages-files are structured in a way that one file holds the messages of one account and is named by the\naccount's ID.\n\nAn exemplary project could look this:\n\n```text\ntegracli-project/\n |- tegracli.conf.yml\n |- mysession.session\n |- my_group/\n    |- tegracli_group.conf.yml\n    |- profiles.jsonl\n    |- 10000001.jsonl\n    |- 10000002.jsonl\n```\nTo run the project command your terminal to `tegracli group run my_group` to collect the latest post of the accounts you want to track.\n\n```text\nUsage: tegracli group run [OPTIONS] [GROUPS]...\n\n  load a group configuration and run the groups operations\n```\n\n## Result File Format\n\nMessages are stored in `jsonl`-files per channel or query. For channels filename is the channel's or user's id, for searches the query.\n**BEWARE:** how directories and files are structured is subject to active development and prone to changes in the near future.\n\n# Developer Installation\n\n1. Install [poetry](https://python-poetry.org/docs/#installation),\n2. Clone repository and unzip, if necessary,\n3. In the directory run `poetry install`,\n4. Run `poetry shell` to start the development virtualenv,\n5. Run `pytest` to run tests, run `pytest --run_api` to include tests against the Telegram API (**these do require a valid configuration**), coverage report can be found under `tests/coverage`.\n",
-    'author': 'Philipp Kessling',
-    'author_email': 'p.kessling@leibniz-hbi.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://pypi.org/project/tegracli/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+A convenience wrapper around Telethon and the Telegram Client API for research purposes.
 
+# Installation Instructions
+
+`tegracli` uses Poetry and python >= 3.9 and < 4.0 for building and installing.
+
+To install using pipx, run the following command `pipx install tegracli`.
+
+## How to get API keys
+
+If you don't have API keys for Telegram, head over to [my.telegram.org](https://my.telegram.org).
+Click on [API development tools](https://my.telegram.org/apps), fill the form to create yourself an app and pluck the keys into `tegracli.conf.yml`. The session name can be arbitrary.
+
+```yaml
+api_id: 1234567
+api_hash : some12321hashthatmustbehere123
+session_name: somesessionyo
+```
+
+This template file is provided with the repository.
+
+# Usage
+
+`tegracli` is a terminal application to access the Telegram API for research purposes.
+In order to retrieve messages the configuration-file from the section before must be present in the directory you start `tegracli`.
+
+The following commands are available:
+
+## CONFIGURE
+
+Opens an interactive prompt for configuring API-access. Aks you to input your API id, API hash and session name and requests
+a 2FA code from Telegram.
+
+```text
+Usage: tegracli configure [OPTIONS]
+
+  Configure tegracli.
+
+Options:
+  --help  Show this message and exit.
+```
+
+## GET
+
+To _get_ messages from a number of channels, use this command.
+
+```text
+Usage: tegracli get [OPTIONS] [CHANNELS]...
+
+  Get messages for the specified channels by either ID or username.
+
+Options:
+  -l, --limit INTEGER           Number of messages to retrieve.
+  -O, --offset_date [%Y-%m-%d]  Offset retrieval to specific date in YYYY-MM-
+                                DD format.
+  -o, --offset_id INTEGER       Offset retrieval to a specific post number.
+  -m, --min_id INTEGER          Minimal post number.
+  -M, --max_id INTEGER          Maximal post number
+  -a, --add_offset INTEGER      Add an offset to the post numbers to be
+                                retrieved.
+  -f, --from_user TEXT          Only messages from this user.
+  --reverse / --forward         Should post numbers count upward or downward.
+                                Defaults to forward.
+  -r, --reply_to TEXT           Only messages replied to specific post id.
+  --help                        Show this message and exit.
+```
+
+| **parameter**       | **description**                                                                                                              |
+|---------------------|------------------------------------------------------------------------------------------------------------------------------|
+| **channels**        | a list of of either telegram usernames, channel or group URLs or user IDs.                                                   |
+| **limit**           | number of messages to retrieve, positive integer. If set to `-1` , retrieves all messages in the channel. defaults to `-1`.  |
+| **offset_date**     | specify start point of retrieval by date, retrieval direction is controlled by `reverse/forward`. Format must be YYYY-MM-DD. |
+| **offset_id**       | specify start point of retrieval by post number, retrieval direction is controlled by `reverse/forward`.                     |
+| **min_id**          | sets the minimum post number                                                                                                 |
+| **max_id**          | sets the maximum post number                                                                                                 |
+| **add_offset**      | add a offset to the post numbers to be retrieved                                                                             |
+| **from_user**       | limit messages to posts *from* a specific user                                                                               |
+| **reply_to**        | limit messages to replies *to* a specific user                                                                               |
+| **reverse/forward** | flag to indicate whether messages should be retrieved in chronological or reverse chronological order.                       |
+
+### Basic Examples
+
+To retrieve the last fifty messages from a Telegram channel:
+
+```bash
+tegracli get --limit 50 corona_infokanal_bmg
+```
+
+To retrieve the entire history starting with post #1 of a channel, set `limit` to `-1`.
+
+```bash
+tegracli get --reverse --limit -1 corona_infokanal_bmg
+```
+To retrieve messages sent after January, 1st 2022:
+
+```bash
+tegracli get --offset_date 2022-01-01 corona_infokanal_bmg
+```
+
+To retrieve message sent before January, 1st 2022:
+
+```bash
+tegracli get --reverse --offset_date 2022-01-01 corona_infokanal_bmg
+```
+## SEARCH
+
+To _search_ messages of your chats and groups and channels you are subscribed to, use this command.
+
+```text
+Usage: tegracli search [OPTIONS] [QUERIES]...
+
+  This function searches Telegram content that is available to your account for the specified search term(s).
+
+Options:
+  --help  Show this message and exit.
+```
+
+## HYDRATE
+
+To rehydrate messages from the API this command accepts a file with message IDs in the format of `$channel_name/$post_number`.
+Both input and output file are optional, if not given, `stdin` and `stdout` are used.
+
+Output data is JSONL, one message per line.
+
+```text
+Usage: tegracli hydrate [OPTIONS] [INPUT_FILE] [OUTPUT_FILE]
+
+  Hydrate a file with messages-ids.
+
+Options:
+  --help  Show this message and exit.
+```
+
+For example, to rehydrate message IDs:
+
+```bash
+echo test_channel/1234 | tegracli hydrate
+>> {"_":"Message","id": 1234, ... , "restriction_reason":[],"ttl_period":null}
+```
+
+## GROUP INIT and GROUP RUN
+
+In order to support updatable  and long-running collections `tegracli` sports an *account group* feature which retrieves
+the history of a given set of accounts and is able to retrieve updates on each of these accounts.
+
+Groups are initialized by calling `teracli group init`, where accounts to track are stated by either stating them as arguments
+or by reading in a file.
+
+### Account Group File Format
+
+Account files are expected to follow these requirements:
+
+- UTF8 text document,
+- per line one account, given as either username, channel-URL or ID,
+- there shall be no header and  no additional columns
+
+```text
+Usage: tegracli group init [OPTIONS] NAME [ACCOUNTS]...
+
+  initialize a new account group
+
+Options:
+  -f, --read_file PATH         read an account list from a file, one
+                               handle/id/url per line.
+  -s, --start_date [%Y-%m-%d]  Start date for the collection. Must be in YYYY-
+                               MM-DD format.
+  -l, --limit INTEGER          number of posts fo retrieve in one run
+  --help                       Show this message and exit.
+```
+
+A group is essentially a directory in your tegracli project folder which holdes
+a group configuration file, a `profiles.jsonl` file which will collect all user objects returned
+by Telegram (these will be recycled to save API requests), as well as the jsonl-files containing the messages.
+The messages-files are structured in a way that one file holds the messages of one account and is named by the
+account's ID.
+
+An exemplary project could look this:
+
+```text
+tegracli-project/
+ |- tegracli.conf.yml
+ |- mysession.session
+ |- my_group/
+    |- tegracli_group.conf.yml
+    |- profiles.jsonl
+    |- 10000001.jsonl
+    |- 10000002.jsonl
+```
+To run the project command your terminal to `tegracli group run my_group` to collect the latest post of the accounts you want to track.
+
+```text
+Usage: tegracli group run [OPTIONS] [GROUPS]...
+
+  load a group configuration and run the groups operations
+```
+
+## Result File Format
+
+Messages are stored in `jsonl`-files per channel or query. For channels filename is the channel's or user's id, for searches the query.
+**BEWARE:** how directories and files are structured is subject to active development and prone to changes in the near future.
+
+# Developer Installation
+
+1. Install [poetry](https://python-poetry.org/docs/#installation),
+2. Clone repository and unzip, if necessary,
+3. In the directory run `poetry install`,
+4. Run `poetry shell` to start the development virtualenv,
+5. Run `pytest` to run tests, run `pytest --run_api` to include tests against the Telegram API (**these do require a valid configuration**), coverage report can be found under `tests/coverage`.
 
-setup(**setup_kwargs)
```

