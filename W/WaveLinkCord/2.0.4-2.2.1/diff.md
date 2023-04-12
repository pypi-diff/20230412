# Comparing `tmp/WaveLinkCord-2.0.4.tar.gz` & `tmp/WaveLinkCord-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveLinkCord-2.0.4.tar", last modified: Wed Mar 15 17:41:27 2023, max compression
+gzip compressed data, was "WaveLinkCord-2.2.1.tar", last modified: Wed Apr 12 16:08:20 2023, max compression
```

## Comparing `WaveLinkCord-2.0.4.tar` & `WaveLinkCord-2.2.1.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 17:41:27.125969 WaveLinkCord-2.0.4/
--rw-rw-rw-   0        0        0     1108 2023-03-11 18:03:30.000000 WaveLinkCord-2.0.4/LICENSE
--rw-rw-rw-   0        0        0     6010 2023-03-15 17:41:27.125969 WaveLinkCord-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5123 2023-03-11 18:11:18.000000 WaveLinkCord-2.0.4/README.rst
--rw-rw-rw-   0        0        0     1015 2023-03-15 17:40:14.000000 WaveLinkCord-2.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       30 2023-03-11 18:15:49.000000 WaveLinkCord-2.0.4/requirements.txt
--rw-rw-rw-   0        0        0      672 2023-03-15 17:41:27.132971 WaveLinkCord-2.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-15 17:41:27.025968 WaveLinkCord-2.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-15 17:41:27.079959 WaveLinkCord-2.0.4/src/WaveLinkCord.egg-info/
--rw-rw-rw-   0        0        0     6010 2023-03-15 17:41:26.000000 WaveLinkCord-2.0.4/src/WaveLinkCord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2023-03-15 17:41:27.000000 WaveLinkCord-2.0.4/src/WaveLinkCord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 17:41:26.000000 WaveLinkCord-2.0.4/src/WaveLinkCord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-03-15 17:41:26.000000 WaveLinkCord-2.0.4/src/WaveLinkCord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-15 17:41:26.000000 WaveLinkCord-2.0.4/src/WaveLinkCord.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-15 17:41:27.109964 WaveLinkCord-2.0.4/src/wavelinkcord/
--rw-rw-rw-   0        0        0     1495 2023-03-15 17:39:04.000000 WaveLinkCord-2.0.4/src/wavelinkcord/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-03-11 18:03:30.000000 WaveLinkCord-2.0.4/src/wavelinkcord/backoff.py
--rw-rw-rw-   0        0        0     1731 2023-03-11 18:03:30.000000 WaveLinkCord-2.0.4/src/wavelinkcord/enums.py
--rw-rw-rw-   0        0        0     1995 2023-03-11 18:03:30.000000 WaveLinkCord-2.0.4/src/wavelinkcord/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-15 17:41:27.111967 WaveLinkCord-2.0.4/src/wavelinkcord/ext/
--rw-rw-rw-   0        0        0        0 2023-03-11 18:08:25.000000 WaveLinkCord-2.0.4/src/wavelinkcord/ext/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-15 17:41:27.113966 WaveLinkCord-2.0.4/src/wavelinkcord/ext/spotify/
--rw-rw-rw-   0        0        0    16241 2023-03-11 19:02:30.000000 WaveLinkCord-2.0.4/src/wavelinkcord/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20287 2023-03-14 18:37:51.000000 WaveLinkCord-2.0.4/src/wavelinkcord/filters.py
--rw-rw-rw-   0        0        0    17637 2023-03-15 17:35:09.000000 WaveLinkCord-2.0.4/src/wavelinkcord/node.py
--rw-rw-rw-   0        0        0     2312 2023-03-14 19:07:24.000000 WaveLinkCord-2.0.4/src/wavelinkcord/payloads.py
--rw-rw-rw-   0        0        0    20386 2023-03-15 17:37:55.000000 WaveLinkCord-2.0.4/src/wavelinkcord/player.py
--rw-rw-rw-   0        0        0    12381 2023-03-15 09:34:30.000000 WaveLinkCord-2.0.4/src/wavelinkcord/queue.py
--rw-rw-rw-   0        0        0    10112 2023-03-14 18:37:50.000000 WaveLinkCord-2.0.4/src/wavelinkcord/tracks.py
-drwxrwxrwx   0        0        0        0 2023-03-15 17:41:27.123968 WaveLinkCord-2.0.4/src/wavelinkcord/types/
--rw-rw-rw-   0        0        0        0 2023-03-11 18:08:32.000000 WaveLinkCord-2.0.4/src/wavelinkcord/types/__init__.py
--rw-rw-rw-   0        0        0      860 2023-03-11 18:03:30.000000 WaveLinkCord-2.0.4/src/wavelinkcord/types/events.py
--rw-rw-rw-   0        0        0      635 2023-03-11 18:03:30.000000 WaveLinkCord-2.0.4/src/wavelinkcord/types/request.py
--rw-rw-rw-   0        0        0      426 2023-03-11 18:05:17.000000 WaveLinkCord-2.0.4/src/wavelinkcord/types/state.py
--rw-rw-rw-   0        0        0      343 2023-03-14 18:37:50.000000 WaveLinkCord-2.0.4/src/wavelinkcord/types/track.py
--rw-rw-rw-   0        0        0     8980 2023-03-15 17:35:56.000000 WaveLinkCord-2.0.4/src/wavelinkcord/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:08:20.757155 WaveLinkCord-2.2.1/
+-rw-rw-rw-   0        0        0     1108 2023-03-11 18:03:30.000000 WaveLinkCord-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0     6010 2023-04-12 16:08:20.758155 WaveLinkCord-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5123 2023-03-11 18:11:18.000000 WaveLinkCord-2.2.1/README.rst
+-rw-rw-rw-   0        0        0     1015 2023-04-12 16:06:16.000000 WaveLinkCord-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       30 2023-03-11 18:15:49.000000 WaveLinkCord-2.2.1/requirements.txt
+-rw-rw-rw-   0        0        0      672 2023-04-12 16:08:20.766157 WaveLinkCord-2.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 16:08:20.567115 WaveLinkCord-2.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:08:20.658133 WaveLinkCord-2.2.1/src/WaveLinkCord.egg-info/
+-rw-rw-rw-   0        0        0     6010 2023-04-12 16:08:20.000000 WaveLinkCord-2.2.1/src/WaveLinkCord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-04-12 16:08:20.000000 WaveLinkCord-2.2.1/src/WaveLinkCord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 16:08:20.000000 WaveLinkCord-2.2.1/src/WaveLinkCord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-12 16:08:20.000000 WaveLinkCord-2.2.1/src/WaveLinkCord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 16:08:20.000000 WaveLinkCord-2.2.1/src/WaveLinkCord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 16:08:20.720146 WaveLinkCord-2.2.1/src/wavelinkcord/
+-rw-rw-rw-   0        0        0     1495 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.1/src/wavelinkcord/__init__.py
+-rw-rw-rw-   0        0        0     2701 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.1/src/wavelinkcord/backoff.py
+-rw-rw-rw-   0        0        0     1731 2023-04-12 15:43:17.000000 WaveLinkCord-2.2.1/src/wavelinkcord/enums.py
+-rw-rw-rw-   0        0        0     1995 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.1/src/wavelinkcord/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:08:20.574113 WaveLinkCord-2.2.1/src/wavelinkcord/ext/
+drwxrwxrwx   0        0        0        0 2023-04-12 16:08:20.723147 WaveLinkCord-2.2.1/src/wavelinkcord/ext/spotify/
+-rw-rw-rw-   0        0        0    16456 2023-04-12 15:52:43.000000 WaveLinkCord-2.2.1/src/wavelinkcord/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    20203 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.1/src/wavelinkcord/filters.py
+-rw-rw-rw-   0        0        0    17775 2023-04-12 15:46:29.000000 WaveLinkCord-2.2.1/src/wavelinkcord/node.py
+-rw-rw-rw-   0        0        0     2474 2023-04-12 15:46:28.000000 WaveLinkCord-2.2.1/src/wavelinkcord/payloads.py
+-rw-rw-rw-   0        0        0    20778 2023-04-12 15:44:18.000000 WaveLinkCord-2.2.1/src/wavelinkcord/player.py
+-rw-rw-rw-   0        0        0    12384 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.1/src/wavelinkcord/queue.py
+-rw-rw-rw-   0        0        0    10104 2023-04-12 15:44:29.000000 WaveLinkCord-2.2.1/src/wavelinkcord/tracks.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:08:20.741152 WaveLinkCord-2.2.1/src/wavelinkcord/types/
+-rw-rw-rw-   0        0        0      860 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.1/src/wavelinkcord/types/events.py
+-rw-rw-rw-   0        0        0      635 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.1/src/wavelinkcord/types/request.py
+-rw-rw-rw-   0        0        0      424 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.1/src/wavelinkcord/types/state.py
+-rw-rw-rw-   0        0        0      343 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.1/src/wavelinkcord/types/track.py
+-rw-rw-rw-   0        0        0     9094 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.1/src/wavelinkcord/websocket.py
```

### Comparing `WaveLinkCord-2.0.4/LICENSE` & `WaveLinkCord-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.0.4/PKG-INFO` & `WaveLinkCord-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaveLinkCord
-Version: 2.0.4
+Version: 2.2.1
 Summary: A robust and powerful Lavalink wrapper for Nextcord
 Home-page: https://github.com/Zyb3rWolfi/Wavelinkcord
 Author: Zyb3rWolfi
 Author-email: Zyb3rWolfi  <Zyb3rWolfi@proton.me>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `WaveLinkCord-2.0.4/README.rst` & `WaveLinkCord-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.0.4/pyproject.toml` & `WaveLinkCord-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WaveLinkCord"
-version = "2.0.4"
+version = "2.2.1"
 authors = [
   { name="Zyb3rWolfi ", email="Zyb3rWolfi@proton.me" },
 ]
 dynamic = ["dependencies"]
 description = "A robust and powerful Lavalink wrapper for Nextcord"
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `WaveLinkCord-2.0.4/setup.cfg` & `WaveLinkCord-2.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6176 656c 696e 6b63 6f72 640d   = wavelinkcord.
-00000020: 0a76 6572 7369 6f6e 203d 2032 2e30 2e34  .version = 2.0.4
+00000020: 0a76 6572 7369 6f6e 203d 2032 2e32 2e31  .version = 2.2.1
 00000030: 0d0a 6175 7468 6f72 203d 205a 7962 3372  ..author = Zyb3r
 00000040: 576f 6c66 690d 0a61 7574 686f 725f 656d  Wolfi..author_em
 00000050: 6169 6c20 3d20 7a79 6233 7277 6f6c 6669  ail = zyb3rwolfi
 00000060: 4070 726f 746f 6e2e 6d65 0d0a 6465 7363  @proton.me..desc
 00000070: 7269 7074 696f 6e20 3d20 4120 706f 7765  ription = A powe
 00000080: 7266 756c 204c 6176 616c 696e 6b20 6c69  rful Lavalink li
 00000090: 6272 6172 7920 666f 7220 4e65 7874 636f  brary for Nextco
```

### Comparing `WaveLinkCord-2.0.4/src/WaveLinkCord.egg-info/PKG-INFO` & `WaveLinkCord-2.2.1/src/WaveLinkCord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaveLinkCord
-Version: 2.0.4
+Version: 2.2.1
 Summary: A robust and powerful Lavalink wrapper for Nextcord
 Home-page: https://github.com/Zyb3rWolfi/Wavelinkcord
 Author: Zyb3rWolfi
 Author-email: Zyb3rWolfi  <Zyb3rWolfi@proton.me>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `WaveLinkCord-2.0.4/src/WaveLinkCord.egg-info/SOURCES.txt` & `WaveLinkCord-2.2.1/src/WaveLinkCord.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,12 @@
 src/wavelinkcord/filters.py
 src/wavelinkcord/node.py
 src/wavelinkcord/payloads.py
 src/wavelinkcord/player.py
 src/wavelinkcord/queue.py
 src/wavelinkcord/tracks.py
 src/wavelinkcord/websocket.py
-src/wavelinkcord/ext/__init__.py
 src/wavelinkcord/ext/spotify/__init__.py
-src/wavelinkcord/types/__init__.py
 src/wavelinkcord/types/events.py
 src/wavelinkcord/types/request.py
 src/wavelinkcord/types/state.py
 src/wavelinkcord/types/track.py
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/__init__.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __title__ = "WaveLink"
 __author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.0.4"
+__version__ = "2.2.1"
 
 from .enums import *
 from .exceptions import *
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .tracks import *
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/backoff.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/backoff.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/enums.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/enums.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/exceptions.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/exceptions.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/ext/spotify/__init__.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/ext/spotify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 import re
 import time
 from typing import Any, List, Optional, Type, TypeVar, Union, TYPE_CHECKING
 
 import aiohttp
 from nextcord.ext import commands
 
-import wavelinkcord
-from wavelinkcord import Node, NodePool
+import wavelink
+from wavelink import Node, NodePool
 
 if TYPE_CHECKING:
-    from wavelinkcord import Player, Playable
+    from wavelink import Player, Playable
 
 
 __all__ = ('SpotifySearchType',
            'SpotifyClient',
            'SpotifyTrack',
            'SpotifyRequestError',
            'decode_url')
@@ -75,15 +75,15 @@
         Could return None if the URL is invalid.
 
     Examples
     --------
 
     .. code:: python3
 
-        from wavelinkcord.ext import spotify
+        from wavelink.ext import spotify
 
         ...
 
         decoded = spotify.decode_url("https://open.spotify.com/track/6BDLcvvtyJD2vnXRDi1IjQ?si=e2e5bd7aaf3d4a2a")
 
         if decoded and decoded['type'] is spotify.SpotifySearchType.track:
             track = await spotify.SpotifyTrack.search(query=decoded["id"], type=decoded["type"])
@@ -202,14 +202,29 @@
         The International Standard Recording Code associated with this track if given.
     length: int
         The track length in milliseconds.
     duration: int
         Alias to length.
     """
 
+    __slots__ = (
+        'raw',
+        'album',
+        'images',
+        'artists',
+        'name',
+        'title',
+        'uri',
+        'id',
+        'length',
+        'duration',
+        'isrc',
+        '__dict__'
+    )
+
     def __init__(self, data: dict[str, Any]) -> None:
         self.raw: dict[str, Any] = data
 
         album = data['album']
         self.album: str = album['name']
         self.images: list[str] = [i['url'] for i in album['images']]
 
@@ -244,15 +259,15 @@
 
         Parameters
         ----------
         query: str
             The song to search for.
         type: Optional[:class:`spotify.SpotifySearchType`]
             An optional enum value to use when searching with Spotify. Defaults to track.
-        node: Optional[:class:`wavelinkcord.Node`]
+        node: Optional[:class:`wavelink.Node`]
             An optional Node to use to make the search with.
         return_first: Optional[bool]
             An optional bool which when set to True will return only the first track found. Defaults to False.
 
         Returns
         -------
         Union[Optional[Track], List[Track]]
@@ -306,35 +321,35 @@
 
         return SpotifyAsyncIterator(query=query, limit=limit, node=node, type=type)
 
     @classmethod
     async def convert(cls: Type[ST], ctx: commands.Context, argument: str) -> ST:
         """Converter which searches for and returns the first track.
 
-        Used as a type hint in a nextcord.py command.
+        Used as a type hint in a discord.py command.
         """
         results = await cls.search(argument)
 
         if not results:
             raise commands.BadArgument("Could not find any songs matching that query.")
 
         return results[0]
 
     async def fulfill(self, *, player: Player, cls: Playable, populate: bool) -> Playable:
         """
         Parameters
         ----------
-        player: :class:`wavelinkcord.player.Player`
+        player: :class:`wavelink.player.Player`
             If Player.autoplay is enabled, this search will fill the AutoPlay Queue.
         cls
             The class to convert this Spotify Track to.
         """
         try:
             tracks: list[cls] = await cls.search(f'"{self.isrc}"')
-        except wavelinkcord.NoTracksError:
+        except wavelink.NoTracksError:
             tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
 
         if not player.autoplay or not populate:
             return tracks[0]
 
         node: Node = player.current_node
         sc: SpotifyClient | None = node._spotify
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/filters.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 class BaseFilter(abc.ABC):
 
     def __init__(self, name: str | None = None) -> None:
         self.name: str = name or "Unknown"
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.BaseFilter name={self.name}>"
+        return f"<wavelink.BaseFilter name={self.name}>"
 
     @property
     @abc.abstractmethod
     def _payload(self) -> Any:
         raise NotImplementedError
 
 
@@ -81,15 +81,15 @@
 
         _dict = collections.defaultdict(float)
         _dict.update(bands)
 
         self.bands = [{"band": band, "gain": _dict[band]} for band in range(15)]
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Equalizer name={self.name}>"
+        return f"<wavelink.Equalizer name={self.name}>"
 
     @property
     def _payload(self) -> list[dict[str, float]]:
         return self.bands
 
     @classmethod
     def flat(cls) -> Equalizer:
@@ -167,15 +167,15 @@
 
         self.level: float = level
         self.mono_level: float = mono_level
         self.filter_band: float = filter_band
         self.filter_width: float = filter_width
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Karaoke level={self.level}, mono_level={self.mono_level}, " \
+        return f"<wavelink.Karaoke level={self.level}, mono_level={self.mono_level}, " \
                f"filter_band={self.filter_band}, filter_width={self.filter_width}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "level":       self.level,
             "monoLevel":   self.mono_level,
@@ -219,15 +219,15 @@
         super().__init__(name="Timescale")
 
         self.speed: float = speed
         self.pitch: float = pitch
         self.rate: float = rate
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Timescale speed={self.speed}, pitch={self.pitch}, rate={self.rate}>"
+        return f"<wavelink.Timescale speed={self.speed}, pitch={self.pitch}, rate={self.rate}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "speed": self.speed,
             "pitch": self.pitch,
             "rate":  self.rate,
@@ -263,15 +263,15 @@
 
         super().__init__(name="Tremolo")
 
         self.frequency: float = frequency
         self.depth: float = depth
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Tremolo frequency={self.frequency}, depth={self.depth}>"
+        return f"<wavelink.Tremolo frequency={self.frequency}, depth={self.depth}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "frequency": self.frequency,
             "depth":     self.depth
         }
@@ -306,15 +306,15 @@
 
         super().__init__(name="Vibrato")
 
         self.frequency: float = frequency
         self.depth: float = depth
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Vibrato frequency={self.frequency}, depth={self.depth}>"
+        return f"<wavelink.Vibrato frequency={self.frequency}, depth={self.depth}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "frequency": self.frequency,
             "depth":     self.depth
         }
@@ -335,15 +335,15 @@
 
     def __init__(self, speed: float = 5) -> None:
         super().__init__(name="Rotation")
 
         self.speed: float = speed
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Rotation speed={self.speed}>"
+        return f"<wavelink.Rotation speed={self.speed}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "rotationHz": self.speed,
         }
 
@@ -371,15 +371,15 @@
         self.cos_scale: float = cos_scale
         self.tan_offset: float = tan_offset
         self.tan_scale: float = tan_scale
         self.offset: float = offset
         self.scale: float = scale
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Distortion " \
+        return f"<wavelink.Distortion " \
                f"sin_offset={self.sin_offset}, " \
                f"sin_scale={self.sin_scale}, cos_offset={self.cos_offset}, " \
                f"cos_scale={self.cos_scale}, tan_offset={self.tan_offset}, " \
                f"tan_scale={self.tan_scale}, offset={self.offset}, " \
                f"scale={self.scale}>"
 
     @property
@@ -440,15 +440,15 @@
 
         self.left_to_left: float = left_to_left
         self.right_to_right: float = right_to_right
         self.left_to_right: float = left_to_right
         self.right_to_left: float = right_to_left
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.ChannelMix " \
+        return f"<wavelink.ChannelMix " \
                f"left_to_left={self.left_to_left}, " \
                f"right_to_right{self.right_to_right}, " \
                f"left_to_right={self.left_to_right}, " \
                f"right_to_left={self.right_to_left}>"
 
     @property
     def _payload(self) -> dict[str, float]:
@@ -513,15 +513,15 @@
         smoothing: float = 20
     ) -> None:
         super().__init__(name="Low Pass")
 
         self.smoothing: float = smoothing
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.LowPass smoothing={self.smoothing}>"
+        return f"<wavelink.LowPass smoothing={self.smoothing}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "smoothing": self.smoothing,
         }
 
@@ -530,33 +530,33 @@
     """A filter that can be applied to a track.
 
     This filter accepts an instance of itself as a parameter which allows
     you to keep previous filters while also applying new ones or overwriting old ones.
 
     Parameters
     ----------
-    filter: wavelinkcord.Filter
+    filter: wavelink.Filter
         An instance of this filter class.
-    equalizer: wavelinkcord.Equalizer
+    equalizer: wavelink.Equalizer
         An equalizer to apply to the track.
-    karaoke: wavelinkcord.Karaoke
+    karaoke: wavelink.Karaoke
         A karaoke filter to apply to the track.
-    timescale: wavelinkcord.Timescale
+    timescale: wavelink.Timescale
         A timescale filter to apply to the track.
-    tremolo: wavelinkcord.Tremolo
+    tremolo: wavelink.Tremolo
         A tremolo filter to apply to the track.
-    vibrato: wavelinkcord.Vibrato
+    vibrato: wavelink.Vibrato
         A vibrato filter to apply to the track.
-    rotation: wavelinkcord.Rotation
+    rotation: wavelink.Rotation
         A rotation filter to apply to the track.
-    distortion: wavelinkcord.Distortion
+    distortion: wavelink.Distortion
         A distortion filter to apply to the track.
-    channel_mix: wavelinkcord.ChannelMix
+    channel_mix: wavelink.ChannelMix
         A channel mix filter to apply to the track.
-    low_pass: wavelinkcord.LowPass
+    low_pass: wavelink.LowPass
         A low pass filter to apply to the track.
 
     """
 
     def __init__(
         self,
         _filter: Filter | None = None,
@@ -581,15 +581,15 @@
         self.vibrato: Vibrato | None = vibrato
         self.rotation: Rotation | None = rotation
         self.distortion: Distortion | None = distortion
         self.channel_mix: ChannelMix | None = channel_mix
         self.low_pass: LowPass | None = low_pass
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Filter equalizer={self.equalizer}, " \
+        return f"<wavelink.Filter equalizer={self.equalizer}, " \
                f"karaoke={self.karaoke}, timescale={self.timescale}, tremolo={self.tremolo}, " \
                f"vibrato={self.vibrato}, rotation={self.rotation}, distortion={self.distortion}, " \
                f"channel_mix={self.channel_mix}, low_pass={self.low_pass}>"
 
     @property
     def _payload(self) -> dict[str, Any]:
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/node.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,14 +344,20 @@
         return cls(data=data)
 
 
 # noinspection PyShadowingBuiltins
 class NodePool:
     """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
 
+    Attributes
+    ----------
+    nodes: dict[str, :class:`Node`]
+        A mapping of :class:`Node` identifier to :class:`Node`.
+
+
     .. warning::
 
         This class should never be initialised. All methods are class methods.
     """
 
     __nodes: dict[str, Node] = {}
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/payloads.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/payloads.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,33 +34,35 @@
     from .tracks import Playable
     from .types.events import EventOp
 
 __all__ = ('TrackEventPayload', )
 
 
 class TrackEventPayload:
-    """The wavelinkcord Track Event Payload.
+    """The Wavelink Track Event Payload.
 
     .. warning::
 
         This class should not be created manually, instead you will receive it from the
-        various wavelinkcord track events.
+        various wavelink track events.
 
     Attributes
     ----------
     event: :class:`TrackEventType`
         An enum of the type of event.
     track: :class:`Playable`
         The track associated with this event.
+    original: Optional[:class:`Playable`]
+        The original requested track before conversion. Could be None.
     player: :class:`player.Player`
         The player associated with this event.
     reason: Optional[str]
         The reason this event was fired.
     """
 
-    def __init__(self, *, data: EventOp, track: Playable, player: Player) -> None:
+    def __init__(self, *, data: EventOp, track: Playable, original: Playable | None, player: Player) -> None:
         self.event: TrackEventType = try_enum(TrackEventType, data['type'])
         self.track: Playable = track
+        self.original: Playable | None = original
         self.player: Player = player
-        print(player)
 
         self.reason: str = data.get('reason')
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/player.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,30 +27,30 @@
 import logging
 from typing import TYPE_CHECKING, Any, Union
 
 import nextcord
 from nextcord.utils import MISSING
 
 from .enums import *
-from .exceptions import QueueEmpty
+from .exceptions import InvalidLavalinkResponse, QueueEmpty
 from .ext import spotify
 from .filters import Filter
 from .node import Node, NodePool
 from .payloads import TrackEventPayload
 from .queue import Queue
 from .tracks import *
 
 
 if TYPE_CHECKING:
     from nextcord.types.voice import GuildVoiceState, VoiceServerUpdate
     from typing_extensions import Self
 
     from .types.events import PlayerState, PlayerUpdateOp
     from .types.request import EncodedTrackRequest, Request
-    from .types.state import nextcordVoiceState
+    from .types.state import DiscordVoiceState
 
 __all__ = ("Player",)
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
@@ -130,26 +130,27 @@
 
         if not self.client:
             if self.current_node.client is None:
                 raise RuntimeError('')
             self.client = self.current_node.client
 
         self._guild: nextcord.Guild | None = None
-        self._voice_state: nextcordVoiceState = {}
+        self._voice_state: DiscordVoiceState = {}
         self._player_state: dict[str, Any] = {}
 
         self.swap_on_disconnect: bool = swap_node_on_disconnect
 
         self.last_update: datetime.datetime | None = None
         self.last_position: int = 0
 
         self._ping: int = 0
 
         self.queue: Queue = Queue()
         self._current: Playable | None = None
+        self._original: Playable | None = None
 
         self._volume: int = 50
         self._paused: bool = False
 
         self._track_seeds: list[str] = []
         self._autoplay: bool = False
         self.auto_queue: Queue = Queue()
@@ -158,24 +159,24 @@
 
     async def _auto_play_event(self, payload: TrackEventPayload) -> None:
         if not self.autoplay:
             return
 
         if payload.reason == 'REPLACED':
             return
-        
+
         if self.queue.loop:
             try:
                 track = self.queue.get()
             except QueueEmpty:
                 return
-            
+
             await self.play(track)
             return
-        
+
         if self.queue:
             populate = len(self.auto_queue) < self._auto_threshold
             await self.play(self.queue.get(), populate=populate)
 
             return
 
         if not self.auto_queue:
@@ -221,15 +222,15 @@
     def position(self) -> float:
         """The position of the currently playing track in milliseconds."""
 
         if not self.is_playing():
             return 0
 
         if self.is_paused():
-            return min(self.last_position, self.source.duration)  # type: ignore
+            return min(self.last_position, self.current.duration)  # type: ignore
 
         delta = (datetime.datetime.now(datetime.timezone.utc) - self.last_update).total_seconds() * 1000
         position = self.last_position + delta
 
         return min(position, self.current.duration)
 
     @property
@@ -299,15 +300,15 @@
         self.channel = self.client.get_channel(int(channel_id))  # type: ignore
 
         if not self._guild:
             self._guild = self.channel.guild  # type: ignore
             assert self._guild is not None
             self.current_node._players[self._guild.id] = self
 
-    async def _dispatch_voice_update(self, data: nextcordVoiceState | None = None) -> None:
+    async def _dispatch_voice_update(self, data: DiscordVoiceState | None = None) -> None:
         assert self._guild is not None
 
         data = data or self._voice_state
 
         try:
             session_id: str = data['session_id']
             token: str = data['token']
@@ -384,33 +385,52 @@
         -------
         :class:`tracks.Playable`
             The track that is now playing.
         """
         assert self._guild is not None
 
         if isinstance(track, spotify.SpotifyTrack):
+            original = track
             track = await track.fulfill(player=self, cls=YouTubeTrack, populate=populate)
 
+            for attr, value in original.__dict__.items():
+                if hasattr(track, attr):
+                    logger.warning(f'Unable to set attribute "{attr}" as it conflicts with new track type.')
+                    continue
+
+                setattr(track, attr, value)
+
         data = {
             'encodedTrack': track.encoded,
             'position': start or 0,
             'volume': volume or self._volume
         }
 
         if end:
             data['endTime'] = end
 
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data=data,
-                                                             query=f'noReplace={not replace}')
+        self._current = track
+        self._original = track
+
+        try:
+
+            resp: dict[str, Any] = await self.current_node._send(
+                method='PATCH',
+                path=f'sessions/{self.current_node._session_id}/players',
+                guild_id=self._guild.id,
+                data=data,
+                query=f'noReplace={not replace}'
+            )
+
+        except InvalidLavalinkResponse as e:
+            self._current = None
+            self._original = None
+            raise e
 
         self._player_state['track'] = resp['track']['encoded']
-        self._current = track
         self.queue._loaded = track
 
         return track
 
     async def set_volume(self, value: int) -> None:
         """|coro|
 
@@ -491,15 +511,15 @@
 
         resp: dict[str, Any] = await self.current_node._send(method='PATCH',
                                                              path=f'sessions/{self.current_node._session_id}/players',
                                                              guild_id=self._guild.id,
                                                              data={'encodedTrack': None})
 
         self.queue._loaded = None
-        
+
         self._player_state['track'] = None
         logger.debug(f'Player {self.guild.id} was stopped.')
 
     async def set_filter(
         self,
         _filter: Filter,
         /, *,
@@ -525,15 +545,15 @@
 
         resp: dict[str, Any] = await self.current_node._send(method='PATCH',
                                                              path=f'sessions/{self.current_node._session_id}/players',
                                                              guild_id=self._guild.id,
                                                              data=data)        
 
         if self.is_playing() and seek:
-            await self.seek(int(self.position * 1000))
+            await self.seek(int(self.position))
         logger.debug(f"Set filter:: {self._filter} ({self.channel.id})")
 
     async def _destroy(self) -> None:
         self.autoplay = False
         self._voice_state = {}
         self._player_state = {}
         self.cleanup()
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/queue.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,16 @@
             self.extend(other)
             return self
 
         raise TypeError(f"Adding '{type(other)}' type to the queue is not supported.")
 
     def _get(self) -> Playable | spotify.SpotifyTrack:
         if self.is_empty:
-            raise QueueEmpty("No items currently in the queue")
+            raise QueueEmpty("No items currently in the queue.")
+
         return self._queue.popleft()
 
     def _drop(self) -> Playable | spotify.SpotifyTrack:
         return self._queue.pop()
 
     def _index(self, item: Playable | spotify.SpotifyTrack) -> int:
         return self._queue.index(item)
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/tracks.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/tracks.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """
 
     def __init__(self, data: dict[str, Any]):
         self.data: dict[str, Any] = data
 
 
 class Playable(metaclass=abc.ABCMeta):
-    """Base ABC Track used in all the wavelinkcord Track types.
+    """Base ABC Track used in all the Wavelink Track types.
 
     Attributes
     ----------
     data: dict[str, Any]
         The raw data received via Lavalink.
     encoded: str
         The encoded Track string.
@@ -231,15 +231,15 @@
         if issubclass(cls, YouTubePlaylist):
             return results  # type: ignore
 
         return results[0]
 
 
 class GenericTrack(Playable):
-    """Generic wavelinkcord Track.
+    """Generic Wavelink Track.
 
     Use this track for searching for Local songs or direct URLs.
     """
     ...
 
 
 class YouTubeTrack(Playable):
```

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/types/events.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/types/events.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/types/request.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/types/request.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.0.4/src/wavelinkcord/websocket.py` & `WaveLinkCord-2.2.1/src/wavelinkcord/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 import asyncio
 import logging
 from typing import TYPE_CHECKING, Any, Optional
 
 import aiohttp
 
-import wavelinkcord
+import wavelink
 
 from . import __version__
 from .backoff import Backoff
 from .enums import NodeStatus, TrackEventType
 from .exceptions import *
 from .payloads import TrackEventPayload
 
@@ -92,15 +92,15 @@
 
         try:
             self._listener_task.cancel()
         except Exception as e:
             logger.debug(f'An error was raised while cancelling the websocket listener. {e}')
 
         uri: str = self.node._host.removeprefix('https://').removeprefix('http://')
-        
+
         if self.node._use_http:
             uri: str = f'{"https://" if self.node._secure else "http://"}{uri}'
         else:
             uri: str = f'{"wss://" if self.node._secure else "ws://"}{uri}'
 
         heartbeat: float = self.node.heartbeat
 
@@ -191,16 +191,21 @@
                     logger.debug('Received payload from Lavalink without an attached player. Disregarding.')
                     continue
 
                 if data['type'] == 'WebSocketClosedEvent':
                     if data['code'] == 4014:
                         continue
 
-                track = await self.node.build_track(cls=wavelinkcord.GenericTrack, encoded=data['encodedTrack'])
-                payload: TrackEventPayload = TrackEventPayload(data=data, track=track, player=player)
+                track = await self.node.build_track(cls=wavelink.GenericTrack, encoded=data['encodedTrack'])
+                payload: TrackEventPayload = TrackEventPayload(
+                    data=data,
+                    track=track,
+                    player=player,
+                    original=player._original
+                )
 
                 if payload.event is TrackEventType.END and payload.reason != 'REPLACED':
                     player._current = None
 
                 self.dispatch('track_event', payload)
 
                 if payload.event is TrackEventType.END:
```

