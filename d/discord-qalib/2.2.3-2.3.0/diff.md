# Comparing `tmp/discord-qalib-2.2.3.tar.gz` & `tmp/discord-qalib-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.2.3.tar", last modified: Sun May  7 14:12:19 2023, max compression
+gzip compressed data, was "discord-qalib-2.3.0.tar", last modified: Sat May 20 18:43:58 2023, max compression
```

## Comparing `discord-qalib-2.2.3.tar` & `discord-qalib-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.407762 discord-qalib-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-07 14:12:19.407762 discord-qalib-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.403762 discord-qalib-2.2.3/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-07 14:12:09.000000 discord-qalib-2.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.403762 discord-qalib-2.2.3/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-07 14:12:09.000000 discord-qalib-2.2.3/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.403762 discord-qalib-2.2.3/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.407762 discord-qalib-2.2.3/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/templater.py
--rw-r--r--   0 runner    (1001) docker     (123)    30812 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 14:12:19.407762 discord-qalib-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-07 14:12:09.000000 discord-qalib-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-20 18:43:48.000000 discord-qalib-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-20 18:43:48.000000 discord-qalib-2.3.0/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28623 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/templater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-20 18:43:48.000000 discord-qalib-2.3.0/setup.py
```

### Comparing `discord-qalib-2.2.3/LICENSE` & `discord-qalib-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.3/PKG-INFO` & `discord-qalib-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.2.3
+Version: 2.3.0
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.3 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.3.0 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.2.3/README.md` & `discord-qalib-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.3/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.3.0/discord_qalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.2.3
+Version: 2.3.0
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.3 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.3.0 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.2.3/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.3.0/discord_qalib.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 qalib/template_engines/formatter.py
 qalib/template_engines/jinja2.py
 qalib/template_engines/template_engine.py
 qalib/translators/__init__.py
 qalib/translators/deserializer.py
 qalib/translators/factory.py
 qalib/translators/json.py
+qalib/translators/menu.py
 qalib/translators/message_parsing.py
 qalib/translators/templater.py
 qalib/translators/xml.py
```

### Comparing `discord-qalib-2.2.3/pyproject.toml` & `discord-qalib-2.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.2.3"
+version = "2.3.0"
 authors = [
     { name = "YousefEZ", email = "syberprojects@gmail.com" },
 ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.poetry]
 name = "discord-qalib"
-version = "2.2.3"
+version = "2.3.0"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
```

### Comparing `discord-qalib-2.2.3/qalib/__init__.py` & `discord-qalib-2.3.0/qalib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .renderer import Renderer, RenderingOptions
 from .template_engines.template_engine import TemplateEngine
 
 __title__ = "qalib"
 __author__ = "YousefEZ"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present YousefEZ"
-__version__ = "2.2.3"
+__version__ = "2.3.0"
 
 T = TypeVar("T")
 Coro = Coroutine[Any, Any, T]
 
 
 def qalib_context(
         template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
```

### Comparing `discord-qalib-2.2.3/qalib/context.py` & `discord-qalib-2.3.0/qalib/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import discord.ext.commands
 import discord.message
 from deprecated import deprecated
 
 from qalib.renderer import Renderer
 from qalib.translators import Callback, Message
-from qalib.translators.deserializer import K_contra
+from qalib.translators.deserializer import K_contra, EventCallback
+from qalib.translators.menu import Menu
 
 
 class QalibContext(discord.ext.commands.context.Context, Generic[K_contra]):
     """QalibContext object is responsible for handling messages that are to be sent to the client."""
 
     def __init__(self, ctx: discord.ext.commands.context.Context, renderer: Renderer[K_contra]):
         """Constructor for the QalibContext object
@@ -57,50 +58,63 @@
         return confirm.content if confirm is not None else None
 
     async def rendered_send(
             self,
             identifier: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
+            events: Optional[EventCallback] = None,
             **kwargs,
     ) -> discord.message.Message:
         """Methods that is fires a message to the client and returns the message object. Doesn't save/keep track of the
         message.
 
         Args:
             identifier (str): identifies the embed in the route file
             callables (Optional[Dict[str, Callback]]) : functions that are hooked to components
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
+            events (Optional[EventCallback]): callbacks that are called on the event
             **kwargs: kwargs that are passed to the context's send method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        message = self._renderer.render(identifier, callables, keywords)
+        message = self._renderer.render(identifier, callables, keywords, events)
+
+        if isinstance(message, Menu):
+            message.front = 0 if "page" not in kwargs else kwargs["page"]
+            message = message.front
+
         assert isinstance(message, Message)
         return await self.send(**{**message.convert_to_context_message().dict(), **kwargs})
 
     async def display(
             self,
             key: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
+            events: Optional[EventCallback] = None,
             **kwargs,
     ) -> None:
         """this is the main function that we use to send one message, and one message only. However, edits to that
         message can take place.
 
         Args:
             key (str): identifies the embed in the route file
-            callables: callable coroutines that are called when the user interacts with the message
-            keywords: keywords that are passed to the embed renderer to format the text
+            callables (Optional[Dict[str, Callback]]): callable coroutines that are called when the user interacts
+            keywords (Optional[Dict[str, Any]]: keywords that are passed to the embed renderer to format the text
+            events (Optional[EventCallback]): callbacks that are called on the event
             **kwargs: kwargs that are passed to the context send method or the message edit method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        message = self._renderer.render(key, callables, keywords)
+        message = self._renderer.render(key, callables, keywords, events)
+        if isinstance(message, Menu):
+            message.front = 0 if "page" not in kwargs else kwargs["page"]
+            message = message.front
+
         assert isinstance(message, Message)
         if self._displayed:
             await self._display(**{**message.convert_to_context_message().as_edit().dict(), **kwargs})
             return
         await self._display(**{**message.convert_to_context_message().dict(), **kwargs})
 
     async def _display(self, **kwargs: Any) -> None:
@@ -116,21 +130,21 @@
 
     @deprecated(version="2.1.2", reason="Use rendered_send method instead")
     async def menu(
             self,
             key: K_contra,
             callbacks: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
+            events: Optional[EventCallback] = None,
             **kwargs,
     ) -> None:
         """This method is used to create a menu for the user to select from.
 
         Args:
             key (K): identifies the menu in the template file
             callbacks (Dict[str, Callback]): callbacks that are called when the user interacts with the menu
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
+            events (Optional[EventCallback]): callbacks that are called on the event
             **kwargs: kwargs that are passed to the context's send method
         """
         warnings.warn("use rendered_send method instead", DeprecationWarning)
-        display = self._renderer.render(key, callbacks=callbacks, keywords=keywords)
-        assert isinstance(display, Message)
-        await self._display(**{**display.convert_to_context_message().dict(), **kwargs})
+        await self.rendered_send(key, callbacks, keywords, events, **kwargs)
```

### Comparing `discord-qalib-2.2.3/qalib/interaction.py` & `discord-qalib-2.3.0/qalib/interaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import discord
 from deprecated import deprecated
 from discord.interactions import InteractionResponse
 from discord.ui import Modal
 
 from qalib.renderer import Renderer
 from qalib.translators import Callback, Message
-from qalib.translators.deserializer import K_contra
+from qalib.translators.deserializer import K_contra, EventCallback
+from qalib.translators.menu import Menu
 
 if TYPE_CHECKING:
     from discord.types.interactions import Interaction as InteractionPayload
 
 
 def create_interaction_payload(interaction: discord.Interaction) -> Dict[str, Any]:
     # pylint: disable=protected-access
@@ -56,28 +57,35 @@
         self._displayed = False
 
     async def rendered_send(
             self,
             identifier: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
+            events: Optional[EventCallback] = None,
             **kwargs,
     ) -> None:
         """Methods that is fires a message to the client and returns the message object. Doesn't save/keep track of the
         message.
 
         Args:
             identifier (str): identifies the embed in the route file
             callables (Optional[Dict[str, Callback]]) : functions that are hooked to components
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
+            events (Optional[EventCallback]): callbacks that are hooked to the event.
             **kwargs: kwargs that are passed to the context's send method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        message = self._renderer.render(identifier, callables, keywords)
+        message = self._renderer.render(identifier, callables, keywords, events)
+
+        if isinstance(message, Menu):
+            message.front = 0 if "page" not in kwargs else kwargs["page"]
+            message = message.front
+
         if isinstance(message, Message):
             assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
             # pylint: disable= no-member
             message_info = {**message.convert_to_interaction_message().dict(), **kwargs}
             return await self.response.send_message(**message_info)  # pyright: ignore [reportGeneralTypeIssues]
         if isinstance(message, Modal):
             assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
@@ -85,28 +93,35 @@
             return await self.response.send_modal(message)  # pyright: ignore [reportGeneralTypeIssues]
 
     async def display(
             self,
             key: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
+            events: Optional[EventCallback] = None,
             **kwargs,
     ) -> None:
         """this is the main function that we use to send one message, and one message only. However, edits to that
         message can take place.
 
         Args:
             key (K): identifies the message in the template file
             callables: callable coroutines that are called when the user interacts with the message
             keywords: keywords that are passed to the embed renderer to format the text
+            events (Optional[EventCallback]): callbacks that are called on the event.
             **kwargs: kwargs that are passed to the context send method or the message edit method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        message = self._renderer.render(key, callables, keywords)
+        message = self._renderer.render(key, callables, keywords, events)
+
+        if isinstance(message, Menu):
+            message.front = 0 if "page" not in kwargs else kwargs["page"]
+            message = message.front
+
         assert isinstance(message, Message)
         if self._displayed:
             await self._display(**{**message.convert_to_interaction_message().as_edit().dict(), **kwargs})
             return
         await self._display(**{**message.convert_to_interaction_message().dict(), **kwargs})
 
     async def _display(self, **kwargs: Any) -> None:
```

### Comparing `discord-qalib-2.2.3/qalib/renderer.py` & `discord-qalib-2.3.0/qalib/renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from enum import Enum, auto
 from typing import Any, Dict, Generic, Optional, cast
 
 from qalib.template_engines.template_engine import TemplateEngine
 from qalib.translators import Callback
-from qalib.translators.deserializer import ReturnType, K_contra, Deserializer
+from qalib.translators.deserializer import ReturnType, K_contra, Deserializer, EventCallbacks
 from qalib.translators.factory import DeserializerFactory, TemplaterFactory
 from qalib.translators.templater import Templater
 
 
 class RenderingOptions(Enum):
     """Options for the renderer."""
 
@@ -49,25 +49,30 @@
         return self._parser
 
     def render(
             self,
             key: K_contra,
             callbacks: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
+            events: Optional[EventCallbacks] = None
     ) -> ReturnType:
         """This method is used to render an embed and a view, and places it in a NamedTuple
 
         Args:
             key (K): key of the embed,
             callbacks (Optional[Dict[str, Callable]]): callbacks that are attached to the components of the view,
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text,
+            events (Optional[EventCallbacks]): callbacks that are called on events
 
         Returns (ReturnType): All possible deserialized types
         """
         if callbacks is None:
             callbacks = {}
 
         if keywords is None:
             keywords = {}
 
+        if events is None:
+            events = {}
+
         source = self._pre_template(keywords).template(self._template_engine, keywords)
-        return self._deserializer.deserialize(source, key, callbacks)
+        return self._deserializer.deserialize(source, key, callbacks, events)
```

### Comparing `discord-qalib-2.2.3/qalib/template_engines/formatter.py` & `discord-qalib-2.3.0/qalib/template_engines/formatter.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.3/qalib/template_engines/jinja2.py` & `discord-qalib-2.3.0/qalib/template_engines/jinja2.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.3/qalib/translators/__init__.py` & `discord-qalib-2.3.0/qalib/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.3/qalib/translators/deserializer.py` & `discord-qalib-2.3.0/qalib/translators/deserializer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Dict, Protocol, Optional, Literal, TypeVar, Union
+from typing import Dict, Protocol, Optional, Literal, TypeVar, Union, Callable
 
 from discord.ui import Modal
 
 from qalib.translators import Callback, Message
+from qalib.translators.menu import Menu, MenuEvents
 
 Types = Literal["message", "menu", "modal", "expansive"]
 
-ReturnType = Union[Message, Modal]
+ReturnType = Union[Message, Modal, Menu]
 
 K_contra = TypeVar("K_contra", bound=str, contravariant=True)
+Events = MenuEvents
+EventCallback = Callable[[Menu], None]
+EventCallbacks = Dict[Events, EventCallback]
 
 
 class ElementTypes(Enum):
     """Enum that represents the types of elements that can be deserialized."""
 
     MESSAGE = "message"
     MENU = "menu"
@@ -30,18 +34,25 @@
         return None
 
 
 class Deserializer(Protocol[K_contra]):
     """Protocol that represents the deserializer. It is meant to be placed into a Renderer, and is responsible for
     deserializing the document into embeds and views."""
 
-    def deserialize(self, source: str, key: K_contra, callables: Dict[str, Callback]) -> ReturnType:
+    def deserialize(
+            self,
+            source: str,
+            key: K_contra,
+            callables: Dict[str, Callback],
+            events: EventCallbacks
+    ) -> ReturnType:
         """This method is used to deserialize a document into an embed and a view.
 
         Parameters:
             source (str): document that is deserialized
-            key:
+            key (K_contra): key that is used to deserialize the document
             callables (Dict[str, Callback]): callables that are used to deserialize the document
+            events (EventCallbacks): hooks that are called on events
 
         Returns (ReturnType): All possible deserialized types
         """
         raise NotImplementedError
```

### Comparing `discord-qalib-2.2.3/qalib/translators/factory.py` & `discord-qalib-2.3.0/qalib/translators/factory.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.3/qalib/translators/json.py` & `discord-qalib-2.3.0/qalib/translators/json.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import discord.types.embed
 from discord import ui
 from discord.abc import Snowflake
 from typing_extensions import NotRequired
 
 from qalib.template_engines.template_engine import TemplateEngine
 from qalib.translators import Callback, DiscordIdentifier, Message
-from qalib.translators.deserializer import Deserializer, ElementTypes, Types, ReturnType, K_contra
+from qalib.translators.deserializer import Deserializer, ElementTypes, Types, ReturnType, K_contra, EventCallbacks
+from qalib.translators.menu import MenuActions, Menu
 from qalib.translators.message_parsing import (
     ButtonComponent,
     ButtonStyle,
     ChannelType,
     CustomSelects,
     Emoji,
     create_button,
@@ -30,15 +31,15 @@
     make_colour,
     make_emoji,
     Field,
     Footer,
     Author,
     TextInputRaw,
     TextInputComponent,
-    make_expansive_embeds, apply, bind_menu, attach_views
+    make_expansive_embeds, apply
 )
 from qalib.translators.templater import Templater
 
 OBJ = TypeVar("OBJ")
 
 ComponentTypes = Literal[
     "button",
@@ -65,14 +66,15 @@
     type: ComponentTypes
 
 
 class Button(Component):
     """This class is used to represent the blueprint of a button."""
 
     custom_id: NotRequired[str]
+    id: NotRequired[str]
     label: NotRequired[str]
     style: NotRequired[ButtonStyle]
     emoji: NotRequired[Emoji]
     url: NotRequired[str]
     disabled: NotRequired[bool]
     row: NotRequired[int]
 
@@ -198,33 +200,40 @@
 
 
 class RegularMessage(BaseMessage):
     """This class is used to represent the blueprint of a message."""
     embed: NotRequired[Embed]
 
 
+class Arrows(TypedDict):
+    previous: ButtonComponent
+    next: ButtonComponent
+
+
 class ExpansiveMessage(BaseMessage):
     page_number_key: NotRequired[str]
     embed: ExpansiveEmbed
+    arrows: NotRequired[Arrows]
 
 
 Page = Union[RegularMessage, ExpansiveMessage]
 
 
-class Menu(Element):
+class MenuMessage(Element):
     timeout: NotRequired[Optional[float]]
     pages: List[Union[str, Page]]
+    arrows: NotRequired[Arrows]
 
 
 class Modal(Element):
     title: str
     components: Components
 
 
-Elements = Union[RegularMessage, ExpansiveMessage, Menu, Modal]
+Elements = Union[RegularMessage, ExpansiveMessage, MenuMessage, Modal]
 Document = Dict[str, Elements]
 
 
 class JSONTemplater(Templater):
     """This method is used to parse the document into a menu and a list of callables for .json files"""
 
     __slots__ = ("_data",)
@@ -269,47 +278,62 @@
         Returns (str): templated element in the form of string.
         """
         return json.dumps(self.recursive_template(deepcopy(self._data), template_engine, keywords))
 
 
 class JSONDeserializer(Deserializer[K_contra]):
 
-    def deserialize(self, source: str, key: K_contra, callables: Dict[str, Callback]) -> ReturnType:
+    def deserialize(
+            self,
+            source: str,
+            key: K_contra,
+            callables: Dict[str, Callback],
+            events: EventCallbacks
+    ) -> ReturnType:
         """Method to deserialize a source into a Display object
 
         Args:
             source (str): The source text to deserialize
             key (K): The key of the element to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            events (EventCallbacks): A dictionary containing the event callbacks.
 
         Returns (ReturnType): All possible deserialized objects.
         """
         document: Document = json.loads(source)
         element: Elements = document[key]
-        return self.deserialize_element(document, element, callables)
+        return self.deserialize_element(document, element, callables, events)
 
-    def deserialize_element(self, document: Document, element: Elements, callables: Dict[str, Callback]) -> ReturnType:
+    def deserialize_element(
+            self,
+            document: Document,
+            element: Elements,
+            callables: Dict[str, Callback],
+            events: EventCallbacks
+    ) -> ReturnType:
         """Method to deserialize an element into a Display object
 
         Args:
             document (Document): The document to deserialize
             element (Elements): The element to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            events (EventCallbacks): A dictionary containing the event callbacks.
 
         Returns (ReturnType): All possible deserialized objects.
         """
         element_type: Optional[ElementTypes] = ElementTypes.from_str(element["type"])
 
-        deserializers: Dict[ElementTypes, Callable[..., ReturnType]] = {
+        deserializers: Dict[ElementTypes, Callable[[Elements, Dict[str, Callback]], ReturnType]] = {
             ElementTypes.MESSAGE: self.deserialize_message,
-            ElementTypes.EXPANSIVE: bind_menu(self.deserialize_expansive),
-            ElementTypes.MENU: bind_menu(partial(self.deserialize_menu, document=document)),
+            ElementTypes.EXPANSIVE: partial(self.deserialize_expansive_into_menu, events=events),
+            ElementTypes.MENU: partial(self.deserialize_menu, document=document, events=events),
             ElementTypes.MODAL: self.deserialize_modal,
         }
-        assert element_type is not None, f"Invalid element type: {element['type']}"
+        if element_type is None:
+            raise KeyError(f"Element type {element['type']} not found")
         return deserializers[element_type](element, callables)
 
     # pylint: disable= too-many-locals
     def deserialize_message(
             self,
             message_tree: Union[RegularMessage, ExpansiveMessage],
             callables: Dict[str, Callback],
@@ -352,75 +376,120 @@
         )
 
         for key, value in overrides.items():
             setattr(message, key, value)
 
         return message
 
-    def deserialize_expansive(self, message_tree: ExpansiveMessage, callbacks: Dict[str, Callback]) -> List[Message]:
+    def deserialize_expansive_into_menu(
+            self,
+            message_tree: ExpansiveMessage,
+            callbacks: Dict[str, Callback],
+            events: EventCallbacks
+    ) -> Menu:
+        """Method to deserialize an expansive message into a Menu
+
+        Args:
+            message_tree (ExpansiveMessage): The ExpansiveMessage of the message_tree
+            callbacks (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            events (EventCallbacks): A dictionary containing the event callbacks.
+
+        Returns (Menu): A Menu object
+        """
+        pages = self.deserialize_expansive(message_tree, callbacks)
+        timeout = message_tree.get("timeout", 180.0)
+        if "arrows" not in message_tree:
+            return Menu(pages, timeout, events=events)
+
+        arrows: Dict[MenuActions, ButtonComponent] = self._deserialize_menu_arrows(message_tree["arrows"])
+        return Menu(pages, timeout, arrows, events)
+
+    @staticmethod
+    def _deserialize_menu_arrows(arrows: Arrows) -> Dict[MenuActions, ButtonComponent]:
+        """Method to deserialize the arrows of a menu
+
+        Args:
+            arrows (Arrows): The view of the menu
+
+        Returns (Dict[MenuActions, ButtonComponent]): A dictionary containing the arrows of the menu
+        """
+        return {
+            MenuActions.PREVIOUS: cast(ButtonComponent, arrows["previous"]),
+            MenuActions.NEXT: cast(ButtonComponent, arrows["next"]),
+        }
+
+    def deserialize_expansive(
+            self,
+            message_tree: ExpansiveMessage,
+            callbacks: Dict[str, Callback],
+    ) -> List[Message]:
         """Method to deserialize a source into a list of Display objects
 
         Args:
             message_tree (ExpansiveMessage): The ExpansiveMessage of the message_tree
             callbacks (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
 
         Returns (List[Display]): A list of Display objects
         """
-        timeout = 180.0
-        if "timeout" in message_tree:
-            timeout = message_tree["timeout"]
-        messages = [self.deserialize_message(message_tree, callbacks, embed=embed)
-                    for embed in self._separate_embed(message_tree["embed"], message_tree.get("page_number_key"))]
-
-        attach_views(messages, timeout)
-        return messages
+        return [self.deserialize_message(message_tree, callbacks, embed=embed)
+                for embed in self._separate_embed(message_tree["embed"], message_tree.get("page_number_key"))]
 
     def deserialize_page(
             self,
             document: Document,
             raw_page: Union[str, Page],
             callables: Dict[str, Callback]
     ) -> List[Message]:
         """Method to deserialize a page into a Display object
 
         Args:
             document (Document): the original document containing all the keys.
             raw_page (Page): The page to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
 
-        Returns (Display): A Display object
+        Returns (List[Message]): List of pages
         """
         page = document[raw_page] if isinstance(raw_page, str) else raw_page
         element_type = ElementTypes.from_str(page["type"])
-        if element_type == ElementTypes.MESSAGE:
-            return [self.deserialize_message(cast(RegularMessage, page), callables)]
-        if element_type == ElementTypes.EXPANSIVE:
-            return self.deserialize_expansive(cast(ExpansiveMessage, page), callables)
-        raise TypeError(f"Invalid type {element_type} for page")
 
-    def deserialize_menu(self, menu: Menu, callables: Dict[str, Callback], *, document: Document) -> List[Message]:
+        page_deserializers: Dict[
+            ElementTypes, Callable[[BaseMessage, Dict[str, Callback]], List[Message]]] = {
+            ElementTypes.MESSAGE: lambda msg, callback: [self.deserialize_message(msg, callback)],
+            ElementTypes.EXPANSIVE: self.deserialize_expansive,
+        }
+        if element_type is None:
+            raise TypeError(f"Unknown Element type {page['type']}")
+        return page_deserializers[element_type](page, callables)
+
+    def deserialize_menu(
+            self,
+            menu: MenuMessage,
+            callables: Dict[str, Callback],
+            events: EventCallbacks,
+            *,
+            document: Document
+    ) -> Menu:
         """Method to deserialize a menu into a list of Display objects
 
         Args:
-            menu (Menu): The Menu Dictionary to deserialize into a List of Messages
+            menu (MenuMessage): The Menu Dictionary to deserialize into a List of Messages
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            events (EventCallbacks): A dictionary containing the event callbacks.
             document (Document): the original document containing all the keys.
 
         Returns (List[Message]): A list of Display objects
         """
         pages: List[Message] = sum((self.deserialize_page(document, page, callables) for page in menu["pages"]), [])
-
         timeout: Optional[float] = menu.get("timeout", 180.0)
 
-        for page in pages:
-            if page.view is None:
-                page.view = ui.View(timeout=timeout)
-            else:
-                page.view.timeout = timeout
-        return pages
+        if "arrows" not in menu:
+            return Menu(pages, timeout, events=events)
+
+        arrows: Dict[MenuActions, ButtonComponent] = self._deserialize_menu_arrows(menu["arrows"])
+        return Menu(pages, timeout, arrows, events)
 
     def deserialize_modal(self, tree: Modal, methods: Dict[str, Callback]) -> discord.ui.Modal:
         """Method to deserialize a modal into a discord.ui.Modal object
 
         Args:
             tree (Modal): The Modal Dictionary to deserialize into a discord.ui.Modal object
             methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
@@ -444,15 +513,15 @@
             replacement_key (str): the key to replace with the page number.
 
         Returns (List[discord.Embed]): A list of embeds.
         """
         return make_expansive_embeds(raw_embed["expansive_field"]["name"],
                                      raw_embed["expansive_field"]["value"],
                                      replacement_key,
-                                     raw_embed,
+                                     cast(Embed, raw_embed),
                                      self._render_embed)
 
     @staticmethod
     def _render_allowed_mentions(
             allowed_mentions: AllowedMentions,
     ) -> discord.AllowedMentions:
         def parse_mentions(mentions: Union[bool, List[int]]) -> Union[bool, List[Snowflake]]:
```

### Comparing `discord-qalib-2.2.3/qalib/translators/message_parsing.py` & `discord-qalib-2.3.0/qalib/translators/message_parsing.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,18 +22,14 @@
     "apply",
     "create_button",
     "create_select",
     "create_channel_select",
     "create_type_select",
     "create_text_input",
     "make_expansive_embeds",
-    "create_arrows",
-    "attach_views",
-    "bind_menu",
-    "make_menu",
     "TextStyle",
     "ButtonStyle",
     "ChannelType",
     "Emoji",
     "ButtonComponent",
     "TextInputRaw",
     "TextInputComponent",
@@ -402,74 +398,14 @@
         raw_embed: T,
         embed_renderer: Callable[Concatenate[T, P], discord.Embed]
 ) -> List[discord.Embed]:
     return [make_expansive_embed(name, value, str(i + 1), replacement_key, raw_embed, embed_renderer)
             for i, value in enumerate(split_text(text))]
 
 
-def attach_views(messages: List[Message], timeout: Optional[float]) -> None:
-    for message in messages:
-        if message.view is None:
-            message.view = ui.View()
-        message.view.timeout = timeout
-
-
-def create_arrows(left: Optional[Message] = None, right: Optional[Message] = None) -> List[discord.ui.Button]:
-    """This function creates the arrow buttons that are used to navigate between the pages.
-
-    Args:
-        left (Optional[Message]): embed and view of the left page
-        right (Optional[Display]): embed and view of the right page
-
-    Returns (List[discord.ui.Button]): list of the arrow buttons
-    """
-
-    def view(message: Message) -> Callback:
-        async def callback(interaction: discord.Interaction):
-            await interaction.response.edit_message(**message.convert_to_interaction_message().as_edit().dict())
-
-        return callback
-
-    buttons: List[discord.ui.Button] = []
-
-    def construct_button(display: Optional[Message], emoji_string: str):
-        if display is None:
-            return
-        button: ButtonComponent = {"emoji": emoji_string, "style": "primary", "callback": view(display)}
-        buttons.append(create_button(button))
-
-    construct_button(left, "⬅️")
-    construct_button(right, "➡️")
-
-    return buttons
-
-
-def make_menu(messages: List[Message]) -> Message:
-    for i, message in enumerate(messages):
-        arrow_up = messages[i - 1] if i > 0 else None
-        arrow_down = messages[i + 1] if i + 1 < len(messages) else None
-
-        if message.view is None:
-            message.view = ui.View()
-
-        for arrow in create_arrows(arrow_up, arrow_down):
-            message.view.add_item(arrow)
-
-    return messages[0]
-
-
-def bind_menu(
-        method: Callable[[T, Dict[str, Callback]], List[Message]]
-) -> Callable[[T, Dict[str, Callback]], Message]:
-    def wrapper(message: T, callbacks: Dict[str, Callback]) -> Message:
-        return make_menu(method(message, callbacks))
-
-    return wrapper
-
-
 def apply(
         element: Optional[M],
         func: Callable[Concatenate[M, P], N],
         *args: P.args,
         **keyword_args: P.kwargs,
 ) -> Optional[N]:
     if element is None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `discord-qalib-2.2.3/qalib/translators/templater.py` & `discord-qalib-2.3.0/qalib/translators/templater.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.3/qalib/translators/xml.py` & `discord-qalib-2.3.0/qalib/translators/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import discord
 import discord.types.embed as embed_types
 from discord import ui
 from discord.abc import Snowflake
 
 from qalib.template_engines.template_engine import TemplateEngine
 from qalib.translators import Callback, DiscordIdentifier, Message
-from qalib.translators.deserializer import Deserializer, ElementTypes, ReturnType, K_contra
+from qalib.translators.deserializer import Deserializer, ElementTypes, ReturnType, K_contra, EventCallbacks
+from qalib.translators.menu import MenuActions, Menu
 from qalib.translators.message_parsing import (
     ButtonComponent,
     ChannelType,
     Emoji,
     create_button,
     create_channel_select,
     create_select,
@@ -25,16 +26,15 @@
     make_channel_types,
     make_colour,
     make_emoji,
     Field,
     Footer,
     Author,
     TextInputComponent,
-    make_expansive_embeds, attach_views, apply, bind_menu,
-)
+    make_expansive_embeds, apply, )
 from qalib.translators.templater import Templater
 
 
 def get_text(element_tree: ElementTree.Element, child: str) -> Optional[str]:
     element = element_tree.find(child)
     if element is None:
         return None
@@ -49,15 +49,14 @@
     def __init__(self, source: str):
         """Initialisation of the XML Parser
 
         Args:
             source (str): the text of the XML file
         """
         self.source = source
-        self.root = ElementTree.fromstring(source)
 
     def template(self, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """This method is used to template an element, by identifying it by its key and using the template engine to
         template it.
 
         Args:
             template_engine (TemplateEngine): template engine that is used to template the embed
@@ -73,74 +72,115 @@
 
     def _get_element(self, document: ElementTree.Element, key: str) -> ElementTree.Element:
         for element in document:
             if key == self.get_attribute(element, "key"):
                 return element
         raise KeyError("Key not found")
 
-    def deserialize(self, source: str, key: K_contra, callables: Dict[str, Callback]) -> ReturnType:
+    def deserialize(
+            self,
+            source: str,
+            key: K_contra,
+            callables: Dict[str, Callback],
+            events: EventCallbacks
+    ) -> ReturnType:
         """This method is used to deserialize the embed from the XML file.
 
         Args:
             source (str): raw string containing the element
             key (K): key of the element
             callables (Dict[str, Callback]): dictionary containing the callables to use for the components
+            events (EventCallbacks): dictionary containing the events to use for the components
 
         Returns (Message): message containing the embed and its view
         """
         document = ElementTree.fromstring(source)
         element = self._get_element(document, key)
-        return self.deserialize_element(document, element, callables)
+        return self.deserialize_element(document, element, callables, events)
 
     def deserialize_element(
             self,
             document: ElementTree.Element,
             element: ElementTree.Element,
-            callables: Dict[str, Callback]
+            callables: Dict[str, Callback],
+            events: EventCallbacks
     ) -> ReturnType:
         """This method is used to deserialize the embed from the XML file.
 
         Args:
             document (ElementTree.Element): document containing all the elements
             element (ElementTree.Element): element containing the embed
             callables (Dict[str, Callback]): dictionary containing the callables to use for the components
+            events (EventCallbacks): dictionary containing the events to use for the components
 
         Returns (ReturnType): all possible deserialized objects.
         """
         element_type = ElementTypes.from_str(element.tag)
 
         deserializers: Dict[ElementTypes, Callable[[ElementTree.Element, Dict[str, Callback]], ReturnType]] = {
             ElementTypes.MESSAGE: self.deserialize_message,
-            ElementTypes.EXPANSIVE: bind_menu(self.deserialize_expansive),
-            ElementTypes.MENU: bind_menu(partial(self.deserialize_menu, document=document)),
+            ElementTypes.EXPANSIVE: partial(self.deserialize_expansive_into_menu, events=events),
+            ElementTypes.MENU: partial(self.deserialize_menu, document=document, events=events),
             ElementTypes.MODAL: self.deserialize_modal,
         }
         assert element_type is not None, f"Element type {element.tag} not found"
         return deserializers[element_type](element, callables)
 
-    def deserialize_expansive(self, element: ElementTree.Element, callbacks: Dict[str, Callback]) -> List[Message]:
+    def deserialize_expansive_into_menu(
+            self,
+            element: ElementTree.Element,
+            callbacks: Dict[str, Callback],
+            events: EventCallbacks
+    ) -> Menu:
+        pages = self.deserialize_expansive(element, callbacks)
+        print(element)
+        timeout_element = element.find("timeout")
+        timeout: Optional[float] = 180.0
+        if timeout_element is not None:
+            timeout = None if timeout_element.text is None else float(timeout_element.text)
+
+        arrows: Dict[MenuActions, ButtonComponent] = self.deserialize_menu_arrows(element)
+        return Menu(pages, timeout, arrows, events)
+
+    def deserialize_expansive(
+            self,
+            element: ElementTree.Element,
+            callbacks: Dict[str, Callback],
+    ) -> List[Message]:
         """Deserializes an embed from an XML file, and returns it as a Display object.
 
         Args:
             element (ElementTree.Element): templated document contents to deserialize.
             callbacks (Dict[str, Callback]): A dictionary containing the callables to use for the components.
 
-        Returns (Display): A display object containing the embed and its view.
+        Returns (List[Message]): A list of messages containing the embed and its view.
         """
         raw_embed = element.find("embed")
         assert raw_embed is not None, "Embed not found"
-        timeout_element = element.find("timeout")
-        timeout: Optional[float] = 180.0
-        if timeout_element is not None:
-            timeout = None if timeout_element.text is None else float(timeout_element.text)
-        messages = [self.deserialize_message(element, callbacks, embed=embed)
-                    for embed in self._separate_embed(raw_embed, element.get("page_number_key"))]
-        attach_views(messages, timeout)
 
-        return messages
+        return [self.deserialize_message(element, callbacks, embed=embed)
+                for embed in self._separate_embed(raw_embed, element.get("page_number_key"))]
+
+    def deserialize_menu_arrows(self, arrows_view: ElementTree.Element) -> Dict[MenuActions, ButtonComponent]:
+        """Deserializes the arrows of a menu from an XML file, and returns it as a dictionary.
+
+        Args:
+            arrows_view (ElementTree.Element): templated document contents to deserialize.
+
+        Returns (Dict[MenuActions, ButtonComponent]): A dictionary containing the arrows.
+        """
+        arrows: Dict[MenuActions, ButtonComponent] = {}
+        previous_element = arrows_view.find("previous")
+        next_element = arrows_view.find("next")
+        if previous_element is not None:
+            arrows[MenuActions.PREVIOUS] = self._create_button_component(previous_element)
+        if next_element is not None:
+            arrows[MenuActions.NEXT] = self._create_button_component(next_element)
+
+        return arrows
 
     def deserialize_message(
             self,
             message_tree: ElementTree.Element,
             callables: Dict[str, Callback],
             **overrides: Any
     ) -> Message:
@@ -199,56 +239,55 @@
             element: ElementTree.Element,
             callables: Dict[str, Callback]
     ) -> List[Message]:
         if element.tag == "page":
             element = self._get_element(document, self.get_attribute(element, "key"))
         element_type = ElementTypes.from_str(element.tag)
 
-        def wrap_in_list(
-                method: Callable[[ElementTree.Element, Dict[str, Callback]], Message]
-        ) -> Callable[[ElementTree.Element, Dict[str, Callback]], List[Message]]:
-            def wrapper(page: ElementTree.Element, callback: Dict[str, Callback]) -> List[Message]:
-                return [method(page, callback)]
-
-            return wrapper
-
         page_deserializers: Dict[
             ElementTypes, Callable[[ElementTree.Element, Dict[str, Callback]], List[Message]]] = {
-            ElementTypes.MESSAGE: wrap_in_list(self.deserialize_message),
+            ElementTypes.MESSAGE: lambda page, callback: [self.deserialize_message(page, callback)],
             ElementTypes.EXPANSIVE: self.deserialize_expansive,
         }
         assert element_type is not None, f"Element type {element.tag} not found"
         return page_deserializers[element_type](element, callables)
 
     def deserialize_menu(
             self,
             element: ElementTree.Element,
             callables: Dict[str, Callback],
+            events: EventCallbacks,
             *,
             document: ElementTree.Element,
-    ) -> List[Message]:
+    ) -> Menu:
         """Deserializes a menu from an XML file, by generating a list of displays that are connected by buttons in their
         views to navigate between them.
 
         Args:
             element (ElementTree.Element): The XML Menu Element to deserialize.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
+            events (EventCallbacks): A dictionary containing the events to callback on.
             document (ElementTree.Element): The entire document
 
         Returns (List[Display]): List of displays that are connected by buttons in their views to navigate between them.
         """
         raw_pages = element.find("pages")
         assert raw_pages is not None, "pages is not present"
 
         pages: List[Message] = sum([self.deserialize_page(document, page, callables) for page in raw_pages], [])
 
-        timeout = element.find("timeout")
-        attach_views(pages, float(timeout.text) if timeout is not None and timeout.text is not None else None)
+        timeout_ele = element.find("timeout")
+        timeout = float(timeout_ele.text) if timeout_ele is not None and timeout_ele.text is not None else None
 
-        return pages
+        view = element.find("arrows")
+        if view is None:
+            return Menu(pages, timeout, events=events)
+
+        arrows: Dict[MenuActions, ButtonComponent] = self.deserialize_menu_arrows(view)
+        return Menu(pages, timeout, arrows, events)
 
     def deserialize_modal(
             self,
             element: ElementTree.Element,
             methods: Dict[str, Callback],
             **kwargs: Any
     ) -> discord.ui.Modal:
@@ -370,15 +409,14 @@
 
         Args:
             raw_view (ElementTree.Element): The element to render the view from.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
 
         Returns (ui.View): A view object containing the components.
         """
-
         view = ui.View()
 
         timeout = raw_view.find("timeout")
         if timeout is not None:
             view.timeout = None if timeout.text is None else float(timeout.text)
         for component in self.render_components(raw_view, callables):
             view.add_item(component)
@@ -513,31 +551,42 @@
         Args:
             tree (ElementTree.Element): The element to extract the elements from.
 
         Returns (Dict[str, Any]): A dictionary containing the extracted elements.
         """
         return {element.tag: self.get_element_text(element) for element in tree}
 
-    def _render_button(self, component: ElementTree.Element, callback: Optional[Callback]) -> ui.Button:
-        """Renders a button based on the template in the element, and formatted values given by the keywords.
+    def _create_button_component(self, component: ElementTree.Element) -> ButtonComponent:
+        """Creates a button component from the given element.
 
         Args:
-            component (ElementTree.Element): The button to render, contains the template.
-            callback (Optional[Callback]): The callback to use if the user interacts with this button.
+            component (ElementTree.Element): The element to create the button component from.
 
-        Returns (ui.Button): The rendered button.
+        Returns (ButtonComponent): The created button component.
         """
         emoji_component = self.pop_component(component, "emoji")
         attributes = self._extract_elements(component)
         attributes["emoji"] = self._render_emoji(emoji_component)
-        attributes["callback"] = callback
         attributes["disabled"] = attributes["disabled"].lower() == "true" if "disabled" in attributes else False
 
-        button: ui.Button = create_button(cast(ButtonComponent, attributes))
-        return button
+        return attributes
+
+    def _render_button(self, component: ElementTree.Element, callback: Optional[Callback] = None) -> ui.Button:
+        """Renders a button based on the template in the element, and formatted values given by the keywords.
+
+        Args:
+            component (ElementTree.Element): The button to render, contains the template.
+            callback (Optional[Callback]): The callback to use if the user interacts with this button.
+
+        Returns (ui.Button): The rendered button.
+        """
+        button: ButtonComponent = self._create_button_component(component)
+        button["callback"] = callback
+
+        return create_button(button)
 
     def _render_options(self, raw_options: Optional[ElementTree.Element]) -> List[discord.SelectOption]:
         """Renders a list of options based on the template in the element, and formatted values given by the keywords.
 
         Args:
             raw_options (ElementTree.Element): The options to render, contains the template.
```

### Comparing `discord-qalib-2.2.3/setup.py` & `discord-qalib-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 setup(
     name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.2.3",
+    version="2.3.0",
     description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
     license="MIT",
     python_requires=">=3.8.0",
     install_requires=requirements,
     package_data={"qalib": ["py.typed"]},
 )
```

