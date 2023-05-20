# Comparing `tmp/Wavelink-2.1.0.tar.gz` & `tmp/Wavelink-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wavelink-2.1.0.tar", last modified: Sat Apr  1 01:44:42 2023, max compression
+gzip compressed data, was "Wavelink-2.3.0.tar", last modified: Sat May 20 08:58:01 2023, max compression
```

## Comparing `Wavelink-2.1.0.tar` & `Wavelink-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 01:44:42.079163 Wavelink-2.1.0/
--rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     5772 2023-04-01 01:44:42.078663 Wavelink-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-01 01:44:42.064346 Wavelink-2.1.0/Wavelink.egg-info/
--rw-rw-rw-   0        0        0     5772 2023-04-01 01:44:42.000000 Wavelink-2.1.0/Wavelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-04-01 01:44:42.000000 Wavelink-2.1.0/Wavelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 01:44:42.000000 Wavelink-2.1.0/Wavelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-01 01:44:42.000000 Wavelink-2.1.0/Wavelink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-01 01:44:42.000000 Wavelink-2.1.0/Wavelink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1006 2023-04-01 01:43:10.000000 Wavelink-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 01:44:42.079163 Wavelink-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-01 01:44:42.073366 Wavelink-2.1.0/wavelink/
--rw-rw-rw-   0        0        0     1495 2023-04-01 01:43:10.000000 Wavelink-2.1.0/wavelink/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/backoff.py
--rw-rw-rw-   0        0        0     1730 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/enums.py
--rw-rw-rw-   0        0        0     1995 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-01 01:44:42.039156 Wavelink-2.1.0/wavelink/ext/
-drwxrwxrwx   0        0        0        0 2023-04-01 01:44:42.074881 Wavelink-2.1.0/wavelink/ext/spotify/
--rw-rw-rw-   0        0        0    16455 2023-04-01 01:28:43.000000 Wavelink-2.1.0/wavelink/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/filters.py
--rw-rw-rw-   0        0        0    17758 2023-03-31 23:50:08.000000 Wavelink-2.1.0/wavelink/node.py
--rw-rw-rw-   0        0        0     2280 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/payloads.py
--rw-rw-rw-   0        0        0    20648 2023-04-01 01:28:43.000000 Wavelink-2.1.0/wavelink/player.py
--rw-rw-rw-   0        0        0    12384 2023-03-15 08:08:05.000000 Wavelink-2.1.0/wavelink/queue.py
--rw-rw-rw-   0        0        0    10102 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/tracks.py
-drwxrwxrwx   0        0        0        0 2023-04-01 01:44:42.077662 Wavelink-2.1.0/wavelink/types/
--rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/types/events.py
--rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/types/request.py
--rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/types/state.py
--rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.1.0/wavelink/types/track.py
--rw-rw-rw-   0        0        0     8964 2023-03-15 12:01:00.000000 Wavelink-2.1.0/wavelink/websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.231994 Wavelink-2.3.0/
+-rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5772 2023-05-20 08:58:01.231494 Wavelink-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.169060 Wavelink-2.3.0/Wavelink.egg-info/
+-rw-rw-rw-   0        0        0     5772 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1006 2023-05-20 08:48:03.000000 Wavelink-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 08:58:01.231994 Wavelink-2.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.207765 Wavelink-2.3.0/wavelink/
+-rw-rw-rw-   0        0        0     1495 2023-05-20 08:48:03.000000 Wavelink-2.3.0/wavelink/__init__.py
+-rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/backoff.py
+-rw-rw-rw-   0        0        0     2225 2023-05-20 08:30:58.000000 Wavelink-2.3.0/wavelink/enums.py
+-rw-rw-rw-   0        0        0     1995 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.141550 Wavelink-2.3.0/wavelink/ext/
+drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.214288 Wavelink-2.3.0/wavelink/ext/spotify/
+-rw-rw-rw-   0        0        0    16455 2023-04-01 01:28:43.000000 Wavelink-2.3.0/wavelink/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/filters.py
+-rw-rw-rw-   0        0        0    17765 2023-04-04 07:37:42.000000 Wavelink-2.3.0/wavelink/node.py
+-rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.3.0/wavelink/payloads.py
+-rw-rw-rw-   0        0        0    20759 2023-05-20 08:25:37.000000 Wavelink-2.3.0/wavelink/player.py
+-rw-rw-rw-   0        0        0    12384 2023-03-15 08:08:05.000000 Wavelink-2.3.0/wavelink/queue.py
+-rw-rw-rw-   0        0        0    10102 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/tracks.py
+drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.230357 Wavelink-2.3.0/wavelink/types/
+-rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/types/events.py
+-rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/types/request.py
+-rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/types/state.py
+-rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/types/track.py
+-rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.3.0/wavelink/websocket.py
```

### Comparing `Wavelink-2.1.0/LICENSE` & `Wavelink-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/PKG-INFO` & `Wavelink-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.1.0
+Version: 2.3.0
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.1.0/README.rst` & `Wavelink-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/Wavelink.egg-info/PKG-INFO` & `Wavelink-2.3.0/Wavelink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.1.0
+Version: 2.3.0
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.1.0/Wavelink.egg-info/SOURCES.txt` & `Wavelink-2.3.0/Wavelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/pyproject.toml` & `Wavelink-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Wavelink"
-version = "2.1.0"
+version = "2.3.0"
 authors = [
   { name="EvieePy", email="evieepy@gmail.com" },
 ]
 dynamic = ["dependencies"]
 description = "A robust and powerful Lavalink wrapper for discord.py"
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `Wavelink-2.1.0/wavelink/__init__.py` & `Wavelink-2.3.0/wavelink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __title__ = "WaveLink"
 __author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.1.0"
+__version__ = "2.3.0"
 
 from .enums import *
 from .exceptions import *
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .tracks import *
```

### Comparing `Wavelink-2.1.0/wavelink/backoff.py` & `Wavelink-2.3.0/wavelink/backoff.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/wavelink/enums.py` & `Wavelink-2.3.0/wavelink/enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from discord.enums import Enum
 
-__all__ = ('NodeStatus', 'TrackSource', 'LoadType', 'TrackEventType')
+__all__ = ('NodeStatus', 'TrackSource', 'LoadType', 'TrackEventType', 'DiscordVoiceCloseType')
 
 
 class NodeStatus(Enum):
 
     DISCONNECTED = 0
     CONNECTING = 1
     CONNECTED = 2
@@ -51,7 +51,23 @@
     load_failed = "LOAD_FAILED"
 
 
 class TrackEventType(Enum):
 
     START = 'TrackStartEvent'
     END = 'TrackEndEvent'
+
+
+class DiscordVoiceCloseType(Enum):
+    CLOSE_NORMAL = 1000  # Not Discord but standard websocket
+    UNKNOWN_OPCODE = 4001
+    FAILED_DECODE_PAYLOAD = 4002
+    NOT_AUTHENTICATED = 4003
+    AUTHENTICATION_FAILED = 4004
+    ALREADY_AUTHENTICATED = 4005
+    SESSION_INVALID = 4006
+    SESSION_TIMEOUT = 4009
+    SERVER_NOT_FOUND = 4011
+    UNKNOWN_PROTOCOL = 4012
+    DISCONNECTED = 4014
+    VOICE_SERVER_CRASHED = 4015
+    UNKNOWN_ENCRYPTION_MODE = 4016
```

### Comparing `Wavelink-2.1.0/wavelink/exceptions.py` & `Wavelink-2.3.0/wavelink/exceptions.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/wavelink/ext/spotify/__init__.py` & `Wavelink-2.3.0/wavelink/ext/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/wavelink/filters.py` & `Wavelink-2.3.0/wavelink/filters.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/wavelink/node.py` & `Wavelink-2.3.0/wavelink/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,17 +346,18 @@
 
 # noinspection PyShadowingBuiltins
 class NodePool:
     """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
 
     Attributes
     ----------
-    nodes: list[:class:`Node`]
+    nodes: dict[str, :class:`Node`]
         A mapping of :class:`Node` identifier to :class:`Node`.
 
+
     .. warning::
 
         This class should never be initialised. All methods are class methods.
     """
 
     __nodes: dict[str, Node] = {}
```

### Comparing `Wavelink-2.1.0/wavelink/payloads.py` & `Wavelink-2.3.0/wavelink/payloads.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from discord.enums import try_enum
 
-from .enums import TrackEventType
+from .enums import TrackEventType, DiscordVoiceCloseType
 
 if TYPE_CHECKING:
     from .player import Player
     from .tracks import Playable
     from .types.events import EventOp
 
-__all__ = ('TrackEventPayload', )
+__all__ = ('TrackEventPayload', 'WebsocketClosedPayload')
 
 
 class TrackEventPayload:
     """The Wavelink Track Event Payload.
 
     .. warning::
 
@@ -47,19 +47,49 @@
 
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
 
         self.reason: str = data.get('reason')
+
+
+class WebsocketClosedPayload:
+    """The Wavelink WebsocketClosed Event Payload.
+
+    .. warning::
+
+        This class should not be created manually, instead you will receive it from the
+        wavelink `on_wavelink_websocket_closed` event.
+
+    Attributes
+    ----------
+    code: :class:`DiscordVoiceCloseType`
+        An Enum representing the close code from Discord.
+    reason: Optional[str]
+        The reason the Websocket was closed.
+    by_discord: bool
+        Whether the websocket was closed by Discord.
+    player: :class:`player.Player`
+        The player associated with this event.
+    """
+
+    def __init__(self, *, data: dict[str, Any], player: Player) -> None:
+        self.code: DiscordVoiceCloseType = try_enum(DiscordVoiceCloseType, data['code'])
+        self.reason: str = data.get('reason')
+        self.by_discord: bool = data.get('byRemote')
+        self.player: Player = player
```

### Comparing `Wavelink-2.1.0/wavelink/player.py` & `Wavelink-2.3.0/wavelink/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import logging
 from typing import TYPE_CHECKING, Any, Union
 
 import discord
 from discord.utils import MISSING
 
 from .enums import *
-from .exceptions import QueueEmpty
+from .exceptions import InvalidLavalinkResponse, QueueEmpty
 from .ext import spotify
 from .filters import Filter
 from .node import Node, NodePool
 from .payloads import TrackEventPayload
 from .queue import Queue
 from .tracks import *
 
@@ -142,14 +142,15 @@
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
@@ -403,22 +404,33 @@
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
 
@@ -533,15 +545,15 @@
 
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

### Comparing `Wavelink-2.1.0/wavelink/queue.py` & `Wavelink-2.3.0/wavelink/queue.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/wavelink/tracks.py` & `Wavelink-2.3.0/wavelink/tracks.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/wavelink/types/events.py` & `Wavelink-2.3.0/wavelink/types/events.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/wavelink/types/request.py` & `Wavelink-2.3.0/wavelink/types/request.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.1.0/wavelink/websocket.py` & `Wavelink-2.3.0/wavelink/websocket.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 import wavelink
 
 from . import __version__
 from .backoff import Backoff
 from .enums import NodeStatus, TrackEventType
 from .exceptions import *
-from .payloads import TrackEventPayload
+from .payloads import TrackEventPayload, WebsocketClosedPayload
 
 if TYPE_CHECKING:
     from .node import Node
     from .player import Player
 
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -50,28 +50,30 @@
     __slots__ = (
         'node',
         'socket',
         'retries',
         'retry',
         '_original_attempts',
         'backoff',
-        '_listener_task'
+        '_listener_task',
+        '_reconnect_task'
     )
 
     def __init__(self, *, node: Node) -> None:
         self.node: Node = node
         self.socket: aiohttp.ClientWebSocketResponse | None = None
 
         self.retries: int | None = node._retries
         self.retry: float = 1
         self._original_attempts: int | None = node._retries
 
         self.backoff: Backoff = Backoff()
 
         self._listener_task: asyncio.Task | None = None
+        self._reconnect_task: asyncio.Task | None = None
 
     @property
     def headers(self) -> dict[str, str]:
         assert self.node.client is not None
         assert self.node.client.user is not None
 
         return {
@@ -110,14 +112,15 @@
             if isinstance(e, aiohttp.WSServerHandshakeError) and e.status == 401:
                 raise AuthorizationFailed from e
             else:
                 logger.error(f'An error occurred connecting to node: "{self.node}". {e}')
 
         if self.is_connected():
             self.retries = self._original_attempts
+            self._reconnect_task = None
             # TODO - Configure Resuming...
         else:
             await self._reconnect()
             return
 
         self._listener_task = asyncio.create_task(self._listen())
 
@@ -146,15 +149,15 @@
             message = await self.socket.receive()
 
             if message.type in (aiohttp.WSMsgType.CLOSED, aiohttp.WSMsgType.CLOSING):
 
                 for player in self.node.players.copy().values():
                     await player._update_event(data=None)
 
-                asyncio.create_task(self._reconnect())
+                self._reconnect_task = asyncio.create_task(self._reconnect())
                 return
 
             if message.data == 1011:
                 logger.error('Lavalink encountered an internal error which can not be resolved. '
                              'Make sure your Lavalink sever is up to date, and try restarting.')
 
                 await self.cleanup()
@@ -188,19 +191,29 @@
                 player = self.get_player(data)
 
                 if player is None:
                     logger.debug('Received payload from Lavalink without an attached player. Disregarding.')
                     continue
 
                 if data['type'] == 'WebSocketClosedEvent':
-                    if data['code'] == 4014:
-                        continue
+                    logger.debug(f'WebSocketClosed Event: '
+                                 f'<code: {data["code"]}, reason: {data["reason"]}, by_discord: {data["byRemote"]}>')
+
+                    payload: WebsocketClosedPayload = WebsocketClosedPayload(data=data, player=player)
+
+                    self.dispatch('websocket_closed', payload)
+                    continue
 
                 track = await self.node.build_track(cls=wavelink.GenericTrack, encoded=data['encodedTrack'])
-                payload: TrackEventPayload = TrackEventPayload(data=data, track=track, player=player)
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

