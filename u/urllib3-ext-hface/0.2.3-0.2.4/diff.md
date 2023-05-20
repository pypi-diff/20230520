# Comparing `tmp/urllib3_ext_hface-0.2.3.tar.gz` & `tmp/urllib3_ext_hface-0.2.4.tar.gz`

## Comparing `urllib3_ext_hface-0.2.3.tar` & `urllib3_ext_hface-0.2.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/dev-requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/changelog.rst
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/cli.rst
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/common.rst
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/conf.py
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/connections.rst
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/facade.rst
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/index.rst
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/install.rst
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/intro.rst
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/license.rst
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/protocols.rst
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/_static/custom.css
--rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/_static/hface.png
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_factories.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_protocol.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/_factories.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/_protocol.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_factories.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_protocol.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_quic.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/tests/helpers.py
--rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/tests/test_http1.py
--rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/tests/test_http2.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/NOTICE
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/dev-requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/changelog.rst
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/cli.rst
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/common.rst
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/conf.py
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/connections.rst
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/facade.rst
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/index.rst
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/install.rst
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/intro.rst
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/license.rst
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/protocols.rst
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/_static/custom.css
+-rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/_static/hface.png
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_factories.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_protocol.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/_factories.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/_protocol.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_factories.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_protocol.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_quic.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/tests/helpers.py
+-rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/tests/test_http1.py
+-rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/tests/test_http2.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/NOTICE
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/README.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.2.3/CHANGELOG.rst` & `urllib3_ext_hface-0.2.4/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v0.2.4 (2023-05-20)
+--------
+
+* Enforce `bytes_to_send` and `bytes_received` for all abstract protocols.
+* Implement graceful close for ``HTTP2Protocol`` (GoAway packet).
+
 v0.2.3 (2023-05-14)
 --------
 
 * Remove ``ProtocolRegistry``.
 
 v0.2.2 (2023-05-13)
 --------
```

### Comparing `urllib3_ext_hface-0.2.3/docs/cli.rst` & `urllib3_ext_hface-0.2.4/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/common.rst` & `urllib3_ext_hface-0.2.4/docs/common.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/conf.py` & `urllib3_ext_hface-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/connections.rst` & `urllib3_ext_hface-0.2.4/docs/connections.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/facade.rst` & `urllib3_ext_hface-0.2.4/docs/facade.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/index.rst` & `urllib3_ext_hface-0.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/install.rst` & `urllib3_ext_hface-0.2.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/intro.rst` & `urllib3_ext_hface-0.2.4/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/protocols.rst` & `urllib3_ext_hface-0.2.4/docs/protocols.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/docs/_static/hface.png` & `urllib3_ext_hface-0.2.4/docs/_static/hface.png`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/__init__.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/_factories.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,48 +18,52 @@
 from typing import Sequence
 
 from .._error_codes import HTTPErrorCodes
 from .._typing import HeadersType
 from ..events import Event
 
 
-class OverTCPProtocol(metaclass=ABCMeta):
-    """
-    Interface for sans-IO protocols on top TCP.
-    """
-
-    # Receiving direction
+class BaseProtocol(metaclass=ABCMeta):
+    """Sans-IO common methods whenever it is TCP, UDP or QUIC."""
 
     @abstractmethod
-    def connection_lost(self) -> None:
+    def bytes_received(self, data: bytes) -> None:
         """
-        Called when the connection is lost or closed.
+        Called when some data is received.
         """
         raise NotImplementedError
 
+    # Sending direction
+
     @abstractmethod
-    def eof_received(self) -> None:
+    def bytes_to_send(self) -> bytes:
         """
-        Called when the other end signals it won’t send any more data.
+        Returns data for sending out of the internal data buffer.
         """
         raise NotImplementedError
 
+
+class OverTCPProtocol(BaseProtocol):
+    """
+    Interface for sans-IO protocols on top TCP.
+    """
+
+    # Receiving direction
+
     @abstractmethod
-    def bytes_received(self, data: bytes) -> None:
+    def connection_lost(self) -> None:
         """
-        Called when some data is received.
+        Called when the connection is lost or closed.
         """
         raise NotImplementedError
 
-    # Sending direction
-
     @abstractmethod
-    def bytes_to_send(self) -> bytes:
+    def eof_received(self) -> None:
         """
-        Returns data for sending out of the internal data buffer.
+        Called when the other end signals it won’t send any more data.
         """
         raise NotImplementedError
 
 
 class OverUDPProtocol(metaclass=ABCMeta):
     """
     Interface for sans-IO protocols on top UDP.
@@ -96,34 +100,14 @@
     @abstractmethod
     def connection_lost(self) -> None:
         """
         Called when the connection is lost or closed.
         """
         raise NotImplementedError
 
-    @abstractmethod
-    def bytes_received(self, data: bytes) -> None:
-        """
-        Called when some data is received.
-
-        :param data: the received UDP frame.
-        """
-        raise NotImplementedError
-
-    # Sending direction
-
-    @abstractmethod
-    def bytes_to_send(self) -> bytes:
-        """
-        Returns data for sending out of the internal data buffer.
-
-        :return: UDP frame to send
-        """
-        raise NotImplementedError
-
 
 class OverQUICProtocol(OverUDPProtocol):
     @property
     @abstractmethod
     def connection_ids(self) -> Sequence[bytes]:
         """
         QUIC connection IDs
```

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_factories.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_protocol.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_protocol.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/_factories.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/_protocol.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return self._terminated
 
     def get_available_stream_id(self) -> int:
         stream_id: int = self._connection.get_next_available_stream_id()
         return stream_id
 
     def submit_close(self, error_code: int = 0) -> None:
-        pass  # TODO: send GOAWAY?
+        self._connection.close_connection(error_code)
 
     def submit_headers(
         self, stream_id: int, headers: HeadersType, end_stream: bool = False
     ) -> None:
         self._connection.send_headers(stream_id, headers, end_stream)
 
     def submit_data(
```

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_factories.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_protocol.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_protocol.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_quic.py` & `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_quic.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/tests/helpers.py` & `urllib3_ext_hface-0.2.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/tests/test_http1.py` & `urllib3_ext_hface-0.2.4/tests/test_http1.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/tests/test_http2.py` & `urllib3_ext_hface-0.2.4/tests/test_http2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/tests/test_integration.py` & `urllib3_ext_hface-0.2.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/LICENSE` & `urllib3_ext_hface-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/NOTICE` & `urllib3_ext_hface-0.2.4/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/README.rst` & `urllib3_ext_hface-0.2.4/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ===================================================
 
 Documentation_ | GitHub_ | PyPI_
 
 This project is a fork of the akamai/hface project but highly slimmed.
 The purpose of that project is to enable basic support for HTTP/1.1, HTTP/2 and HTTP/3 in urllib3.
 
-* HTTP/1.1, HTTP/2, and HTTP/3 support
+* HTTP/1.1, HTTP/2, and HTTP/3 support through respectively h11, h2 and aioquic
 * Sans-IO_ core with pluggable protocol implementations
 * Layered design with well-defined APIs
 * Client-oriented only
 
 See online documentation_ for more info.
 
 .. _Documentation: https://urllib3.readthedocs.io/
```

### Comparing `urllib3_ext_hface-0.2.3/pyproject.toml` & `urllib3_ext_hface-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.3/PKG-INFO` & `urllib3_ext_hface-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3-ext-hface
-Version: 0.2.3
+Version: 0.2.4
 Summary: urllib3 extension to support HTTP/1.1, HTTP/2 and HTTP/3 independently of Python httplib
 Project-URL: Changelog, https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/Ousret/urllib3-ext-hface
 Project-URL: Issue tracker, https://github.com/Ousret/urllib3-ext-hface/issues
 Author-email: Miloslav Pojman <mpojman@akamai.com>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -44,15 +44,15 @@
 ===================================================
 
 Documentation_ | GitHub_ | PyPI_
 
 This project is a fork of the akamai/hface project but highly slimmed.
 The purpose of that project is to enable basic support for HTTP/1.1, HTTP/2 and HTTP/3 in urllib3.
 
-* HTTP/1.1, HTTP/2, and HTTP/3 support
+* HTTP/1.1, HTTP/2, and HTTP/3 support through respectively h11, h2 and aioquic
 * Sans-IO_ core with pluggable protocol implementations
 * Layered design with well-defined APIs
 * Client-oriented only
 
 See online documentation_ for more info.
 
 .. _Documentation: https://urllib3.readthedocs.io/
```

