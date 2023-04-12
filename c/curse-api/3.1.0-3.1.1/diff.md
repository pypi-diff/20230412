# Comparing `tmp/curse_api-3.1.0.tar.gz` & `tmp/curse_api-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curse_api-3.1.0.tar", max compression
+gzip compressed data, was "curse_api-3.1.1.tar", max compression
```

## Comparing `curse_api-3.1.0.tar` & `curse_api-3.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      432 2023-04-05 04:40:26.517410 curse_api-3.1.0/curse_api/__init__.py
--rw-r--r--   0        0        0      693 2023-03-29 19:10:20.991380 curse_api-3.1.0/curse_api/abc.py
--rw-r--r--   0        0        0     9944 2023-04-05 04:49:25.478376 curse_api-3.1.0/curse_api/api.py
--rw-r--r--   0        0        0    19682 2023-04-05 04:27:56.559430 curse_api-3.1.0/curse_api/categories.py
--rw-r--r--   0        0        0     2613 2023-03-31 19:47:09.453755 curse_api-3.1.0/curse_api/clients/aiohttp.py
--rw-r--r--   0        0        0     2545 2023-03-31 19:41:25.587365 curse_api-3.1.0/curse_api/clients/httpx.py
--rw-r--r--   0        0        0     2547 2023-04-05 04:23:15.949888 curse_api-3.1.0/curse_api/enums.py
--rw-r--r--   0        0        0      352 2023-03-29 19:05:09.167372 curse_api-3.1.0/curse_api/errors.py
--rw-r--r--   0        0        0       71 2023-03-29 20:55:33.376025 curse_api-3.1.0/curse_api/ext/__init__.py
--rw-r--r--   0        0        0     1267 2023-03-29 21:18:53.091488 curse_api-3.1.0/curse_api/ext/manifest.py
--rw-r--r--   0        0        0     8890 2023-04-05 04:36:52.833259 curse_api-3.1.0/curse_api/models.py
--rw-r--r--   0        0        0     1438 2023-04-05 04:38:53.111050 curse_api-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     4205 2023-03-28 23:23:05.412678 curse_api-3.1.0/README.md
--rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 curse_api-3.1.0/setup.py
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 curse_api-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      432 2023-04-05 04:40:26.517410 curse_api-3.1.1/curse_api/__init__.py
+-rw-r--r--   0        0        0      693 2023-04-12 21:13:06.372593 curse_api-3.1.1/curse_api/abc.py
+-rw-r--r--   0        0        0     9944 2023-04-05 04:49:25.478376 curse_api-3.1.1/curse_api/api.py
+-rw-r--r--   0        0        0    19682 2023-04-05 04:27:56.559430 curse_api-3.1.1/curse_api/categories.py
+-rw-r--r--   0        0        0     2613 2023-04-10 01:35:20.792577 curse_api-3.1.1/curse_api/clients/aiohttp.py
+-rw-r--r--   0        0        0     2545 2023-03-31 19:41:25.587365 curse_api-3.1.1/curse_api/clients/httpx.py
+-rw-r--r--   0        0        0     2547 2023-04-05 04:23:15.949888 curse_api-3.1.1/curse_api/enums.py
+-rw-r--r--   0        0        0      352 2023-03-29 19:05:09.167372 curse_api-3.1.1/curse_api/errors.py
+-rw-r--r--   0        0        0       71 2023-03-29 20:55:33.376025 curse_api-3.1.1/curse_api/ext/__init__.py
+-rw-r--r--   0        0        0     1564 2023-04-12 21:19:25.640878 curse_api-3.1.1/curse_api/ext/manifest.py
+-rw-r--r--   0        0        0     8890 2023-04-12 21:13:06.374593 curse_api-3.1.1/curse_api/models.py
+-rw-r--r--   0        0        0     1438 2023-04-12 21:24:34.338454 curse_api-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4205 2023-03-28 23:23:05.412678 curse_api-3.1.1/README.md
+-rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 curse_api-3.1.1/setup.py
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 curse_api-3.1.1/PKG-INFO
```

### Comparing `curse_api-3.1.0/curse_api/abc.py` & `curse_api-3.1.1/curse_api/abc.py`

 * *Files identical despite different names*

### Comparing `curse_api-3.1.0/curse_api/api.py` & `curse_api-3.1.1/curse_api/api.py`

 * *Files identical despite different names*

### Comparing `curse_api-3.1.0/curse_api/categories.py` & `curse_api-3.1.1/curse_api/categories.py`

 * *Files identical despite different names*

### Comparing `curse_api-3.1.0/curse_api/clients/aiohttp.py` & `curse_api-3.1.1/curse_api/clients/aiohttp.py`

 * *Files identical despite different names*

### Comparing `curse_api-3.1.0/curse_api/clients/httpx.py` & `curse_api-3.1.1/curse_api/clients/httpx.py`

 * *Files identical despite different names*

### Comparing `curse_api-3.1.0/curse_api/enums.py` & `curse_api-3.1.1/curse_api/enums.py`

 * *Files identical despite different names*

### Comparing `curse_api-3.1.0/curse_api/ext/manifest.py` & `curse_api-3.1.1/curse_api/ext/manifest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from __future__ import annotations
 from typing import Dict, Any, TYPE_CHECKING, List
-from ..models import File, ManifestMetadata
+from ..models import File, ManifestMetadata, Mod
 
 if TYPE_CHECKING:
     from ..api import CurseAPI
 
 AnyDict = Dict[Any, Any]
 
+
 # TODO: custom manifest creator
 class ManifestParser:
     def __init__(self, api: "CurseAPI") -> None:
         self.api = api
 
     async def load_files(self, data: AnyDict) -> List[File]:
         files = data.get("files", None)
         if not isinstance(files, list):
             raise TypeError("Files is not list")
 
         fids = [i["fileID"] for i in files]
         return await self.api.get_files(fids)
 
+    async def load_mods(self, data: AnyDict) -> List[Mod]:
+        files = data.get("files", None)
+        if not isinstance(files, list):
+            raise TypeError("Files is not list")
+
+        fids = [i["projectID"] for i in files]
+        return await self.api.get_mods(fids)
+
     async def load_modloader(self, data: AnyDict):  # TODO: type better
         minecraft = data.get("minecraft")
         if not isinstance(minecraft, dict):
             raise TypeError("Manifest is invalid")
         modls: List[Dict] = minecraft.get("modLoaders")  # type: ignore
 
         modls = [i["id"] for i in modls if i["primary"]]
```

### Comparing `curse_api-3.1.0/curse_api/models.py` & `curse_api-3.1.1/curse_api/models.py`

 * *Files identical despite different names*

### Comparing `curse_api-3.1.0/pyproject.toml` & `curse_api-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "curse-api"
 repository = "https://github.com/Stinky-c/curse-api"
 homepage = "https://github.com/Stinky-c/curse-api"
 readme = "README.md"
-version = "3.1.0"
+version = "3.1.1"
 description = "A simple curseforge api wrapper"
 authors = ["Stinky-c <60587749+Stinky-c@users.noreply.github.com>"]
 license = "MIT"
 keywords = ["curseforge", "api wrapper"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.8",
```

### Comparing `curse_api-3.1.0/README.md` & `curse_api-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `curse_api-3.1.0/setup.py` & `curse_api-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 extras_require = \
 {'aiohttp': ['aiohttp>=3.8.4,<4.0.0'],
  'httpx': ['httpx>=0.23.1,<0.24.0'],
  'quick': ['httpx>=0.23.1,<0.24.0']}
 
 setup_kwargs = {
     'name': 'curse-api',
-    'version': '3.1.0',
+    'version': '3.1.1',
     'description': 'A simple curseforge api wrapper',
     'long_description': '# curse-api\n\n----\n\n## A simple async python Curseforge api wrapper using pydantic\n\nBuilt to serve CF endpoints while providing methods and functions to assist in finding the right mod.\n\n- Quick Install: `pip install curse-api[quick]`\n- [Features](#features)\n- [Quick Start](#quick-start)\n- [Examples](#examples)\n\n----\n\n## Some backstory\n\nA while back when I was starting to learn python further then the basics I created a small tool to download Minecraft mods from a pack manifest.\nSoon after I wrote it the new API changes came and broke it. Now once more I want to return to that project idea and expand further. After first rewriting the project using [chili](https://pypi.org/project/chili/) it felt off, so returned to rewrite once more using [pydantic](https://pypi.org/project/pydantic/) for data validation and ease of access. This is mostly a pet project to learn further python.\n\n----\n\n## Features\n\nMain Dependency:\n\n- [Pydantic](https://pypi.org/project/pydantic/)\n\nNative async library support:\n\n- [Aiohttp](https://pypi.org/project/aiohttp/) - `pip install curse-api[aiohttp]`\n- [Httpx](https://pypi.org/project/httpx/) - `pip install curse-api[httpx]`\n\nCurrently implemented:\n\n- Important endpoint support\n- Full CurseForge model\n- Mediocre error handling\n- Pluggable API factories\n- Serialization and deserialization of models\n- Python 3.7, 3.8 & 3.9 support\n- Async\n\nTo Do:\n\n- Fix to be usable with pydantic based ORM\'s\n- Address all TODO\'s\n- Test other games too\n- Add more\n- Write docs\n- Update and fix error handling\n- Shortcuts to import clients\n\nCI/CD:\n\n- Type checking\n- Version testing\n- Tests\n\n----\n\n## Examples\n\n### Quick start\n\nRequires an api from CF to use the API. You can get one [here](https://docs.curseforge.com/#authentication).\nThis example runs through most of the basics\n\n```python\nfrom curse_api import CurseAPI\nfrom curse_api.clients.httpx import HttpxFactory\nimport os\nimport asyncio\n\n\nasync def main():\n    async with CurseAPI(os.environ["CF_API_KEY"], factory=HttpxFactory) as api:\n\n        "Mods"\n        a = await api.search_mods(searchFilter="JEI", slug="jei")\n        # applies the search filters to the standard of CF docs\n\n        mod = await api.get_mod(250398)  # returns a singular Mod\n        mod_list = await api.get_mods([285109, 238222])  # returns a list of Mods\n\n        "files"\n        "See examples/download.py"\n        # TODO finish file support\n        files = await api.get_files([3940240])  # returns a list of Files matching their id\n        mod_files = await api.get_mod_files(238222)  # returns all the Files of on a give Mod\n\n        "Version details - large data"\n        "See examples/modloader.py"\n        mc = await api.minecraft_versions()  # returns all of minecraft version data\n        ml = await api.modloader_versions()  # returns **ALL** modloader versions on curseforge\n\n        mc_112 = await api.get_specific_minecraft_version("1.12.2")  # returns minecraft version related information\n        forge = await api.get_specific_minecraft_modloader("forge-36.2.39")  # returns forge related version information\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n### Downloading to a file\n\nThis example opens a properly named file in the current working directory and writes to it.\n\n```python\nfrom curse_api import CurseAPI\nfrom curse_api.clients.httpx import HttpxFactory\nimport os\nimport asyncio\n\n\nasync def main():\n    async with CurseAPI(os.environ["CF_API_KEY"], factory=HttpxFactory) as api:\n\n        # fetch the latest file from project with slug \'jei\'\n        mod_l, page_data = await api.search_mods(slug="jei")\n        latest = mod_l[0].latestFiles[0]\n\n        with open(latest.fileName, "wb") as f:\n            down = await api.download(latest.downloadUrl)  # type: ignore\n            async for b in down:\n                f.write(b)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n\n```\n\n----\n\n### Sub project / extension ideas\n\n- Modloader download and installation\n- Minecraft Version type / parser\n- MC pack installation\n- DB cache extension\n- Manifest parsing\n',
     'author': 'Stinky-c',
     'author_email': '60587749+Stinky-c@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Stinky-c/curse-api',
```

### Comparing `curse_api-3.1.0/PKG-INFO` & `curse_api-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curse-api
-Version: 3.1.0
+Version: 3.1.1
 Summary: A simple curseforge api wrapper
 Home-page: https://github.com/Stinky-c/curse-api
 License: MIT
 Keywords: curseforge,api wrapper
 Author: Stinky-c
 Author-email: 60587749+Stinky-c@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
```

