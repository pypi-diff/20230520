# Comparing `tmp/snapstream-0.0.4.tar.gz` & `tmp/snapstream-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.4.tar", max compression
+gzip compressed data, was "snapstream-0.0.5.tar", max compression
```

## Comparing `snapstream-0.0.4.tar` & `snapstream-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-05-12 20:12:28.224818 snapstream-0.0.4/LICENSE
--rw-r--r--   0        0        0     2536 2023-05-12 20:12:28.224818 snapstream-0.0.4/README.md
--rw-r--r--   0        0        0     1976 2023-05-12 20:12:40.461104 snapstream-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2277 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/__init__.py
--rw-r--r--   0        0        0     7763 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/__main__.py
--rw-r--r--   0        0        0     9781 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/caching.py
--rw-r--r--   0        0        0     2592 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/codecs.py
--rw-r--r--   0        0        0     9129 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/core.py
--rw-r--r--   0        0        0     3271 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/utils.py
--rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-20 14:25:54.488845 snapstream-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2536 2023-05-20 14:25:54.488845 snapstream-0.0.5/README.md
+-rw-r--r--   0        0        0     2034 2023-05-20 14:26:06.372835 snapstream-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2277 2023-05-20 14:25:54.492845 snapstream-0.0.5/snapstream/__init__.py
+-rw-r--r--   0        0        0     7897 2023-05-20 14:25:54.492845 snapstream-0.0.5/snapstream/__main__.py
+-rw-r--r--   0        0        0     9781 2023-05-20 14:25:54.492845 snapstream-0.0.5/snapstream/caching.py
+-rw-r--r--   0        0        0     2562 2023-05-20 14:25:54.492845 snapstream-0.0.5/snapstream/codecs.py
+-rw-r--r--   0        0        0    10542 2023-05-20 14:25:54.496845 snapstream-0.0.5/snapstream/core.py
+-rw-r--r--   0        0        0     3255 2023-05-20 14:25:54.496845 snapstream-0.0.5/snapstream/utils.py
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.5/PKG-INFO
```

### Comparing `snapstream-0.0.4/LICENSE` & `snapstream-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.4/README.md` & `snapstream-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.4/pyproject.toml` & `snapstream-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snapstream"
-version = "0.0.4"
+version = "0.0.5"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Menziess/snapstream"
 documentation = "https://snapstream.readthedocs.io"
 license = "MIT"
 keywords = ["kafka", "pubsub"]
@@ -37,21 +37,22 @@
 pydocstyle = "^6.3.0"
 autopep8 = "^2.0.2"
 pyright = "^1.1.300"
 flake8 = "^6.0.0"
 bandit = "^1.7.5"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
-pre-commit = "^3.2.1"
 pytest-mock = "^3.10.0"
+pre-commit = "^3.2.1"
 ipykernel = "^6.22.0"
 sphinx = "^6.2.1"
 sphinx-rtd-theme = "^1.2.0"
 sphinx-autoapi = "^2.1.0"
 sphinx-autobuild = "^2021.3.14"
+testcontainers = {extras = ["kafka"], version = "^3.7.1"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 include = ["snapstream"]
```

### Comparing `snapstream-0.0.4/snapstream/__init__.py` & `snapstream-0.0.5/snapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.4/snapstream/__main__.py` & `snapstream-0.0.5/snapstream/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 def replace_variable_references(entry: dict, args: Namespace) -> dict:
     """For every value starting with $, replace with env."""
     conf = entry['conf']
     for k, v in conf.items():
         if v.startswith('$'):
             conf[k] = get_variable(v[1:], args.secrets_base_path)
         if v.startswith(r'\$'):
-            conf[k] = v.replace()
+            conf[k] = v.replace(r'\$', '$')
     entry['conf'] = conf
     return entry
 
 
 def regex_filter(regex: str, key: Optional[str]) -> bool:
     """Check whether key matches regex filter."""
     if regex and key:
@@ -159,34 +159,36 @@
             .fromtimestamp(msg.timestamp()[-1] / 1000, tz=timezone.utc)
             .isoformat()
             if msg.timestamp() else ''
         )
         key = msg.key().decode() if msg.key() is not None else ''
         offset = msg.offset()
         val = msg.value()
-        if key_filter(str(key)) and val_filter(str(val)):
+        if key_filter(str(key)) and val_filter(str(val)):  # pyright: ignore
             print()
             print('>>> timestamp:', timestamp)
             print('>>> offset:', offset)
             print('>>> key:', key)
-            print(val.decode()) if not args.columns else print({
+            print(val) if not args.columns else print({
                 k: v for k, v in val.items() if k in args.columns.split(',')
             })
 
 
 def inspect_cache(conf: dict, args: Namespace):
     """Read records from cache."""
+    if not path.isdir(args.path):
+        raise OSError(f'Folder doesn\'t exist: {args.path}')
     cache = Cache(
         args.path,
         access_type=AccessType.read_only(),
     )
     key_filter = curry(regex_filter)(args.key_filter)
     val_filter = curry(regex_filter)(args.val_filter)
     for key, val in cache.items():
-        if key_filter(str(key)) and val_filter(str(val)):
+        if key_filter(str(key)) and val_filter(str(val)):  # pyright: ignore
             if args.columns and not isinstance(val, dict):
                 raise ValueError(f'Columns could not be extracted from {type(val)}: {val}')
             print()
             print('>>> key:', key)
             print(val) if not args.columns else print({
                 k: v for k, v in val.items() if k in args.columns.split(',')
             })
```

### Comparing `snapstream-0.0.4/snapstream/caching.py` & `snapstream-0.0.5/snapstream/caching.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.4/snapstream/codecs.py` & `snapstream-0.0.5/snapstream/codecs.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Any, cast
 
 from avro.io import BinaryDecoder, BinaryEncoder, DatumReader, DatumWriter
 from avro.schema import Schema, parse
 from toolz import curry
 
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
 
 
 def deserialize_json(msg: bytes) -> dict:
     """Deserialize json message."""
     return loads(msg.decode())
```

### Comparing `snapstream-0.0.4/snapstream/core.py` & `snapstream-0.0.5/snapstream/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from pubsub import pub
 from toolz import pipe
 
 from snapstream.codecs import ICodec
 from snapstream.utils import KafkaIgnoredPropertyFilter, Singleton
 
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
 logger.addFilter(KafkaIgnoredPropertyFilter())
 
 READ_FROM_START = -2
 READ_FROM_END = -1
 
 
 class Conf(metaclass=Singleton):
@@ -194,46 +193,47 @@
 
     try:
         yield consume()
     finally:
         c.close()
 
 
-def _producer_handler(err, msg):
-    if err is not None:
-        logger.error(f'Failed to deliver message: {err}.')
-        # Raise exception by default
-        raise KafkaException(err)
-    else:
-        logger.debug(f'Produced to topic: {msg.topic()}.')
+def _producer_handler(p, topic, dry, codec):
+    def callback(err, msg):
+        if err is not None:
+            logger.error(f'Failed to deliver message: {err}.')
+            # Raise exception by default
+            raise KafkaException(err)
+        else:
+            logger.debug(f'Produced to topic: {msg.topic()}.')
+
+    def produce(key, val, *args, **kwargs):
+        if codec:
+            logger.debug(f'Encoding using codec: {topic}.')
+            val = codec.encode(val)
+        if dry:
+            logger.warning(f'Skipped sending message to {topic} [dry=True].')
+            return
+        p.produce(topic=topic, key=key, value=val, *args, **kwargs, callback=callback)
+    return produce
 
 
 @contextmanager
 def get_producer(
     topic: str,
     conf: dict,
     dry=False,
     codec: Optional[ICodec] = None,
     flush_timeout: float = -1.0,
-    callback=_producer_handler
+    pusher=_producer_handler
 ) -> Iterator[Callable[[Any, Any], None]]:
     """Yield kafka produce method."""
     p = Producer(conf, logger=logger)
-
-    def produce(key, val, *args, **kwargs):
-        if codec:
-            logger.debug(f'Encoding using codec: {topic}.')
-            val = codec.encode(val)
-        if dry:
-            logger.warning(f'Skipped sending message to {topic} [dry=True].')
-            return
-        p.produce(topic=topic, key=key, value=val, *args, **kwargs, callback=callback)
-
-    yield produce
-
+    yield pusher(p, topic, dry, codec)
+    logger.debug(f'Flushing messages to kafka, flush_timeout={flush_timeout}.')
     p.flush(flush_timeout)
 
 
 class Topic(ITopic):
     """Act as a consumer and producer.
 
     >>> topic = Topic('emoji', {
@@ -256,27 +256,29 @@
         self,
         name: str,
         conf: dict = {},
         offset: Optional[int] = None,
         codec: Optional[ICodec] = None,
         flush_timeout: float = -1.0,
         poll_timeout: float = 1.0,
-        callback=_producer_handler,
+        pusher=_producer_handler,
         poller=_consumer_handler,
         dry: bool = False
     ) -> None:
         """Pass topic related configuration."""
         c = Conf()
         self.name = name
         self.conf = {**c.conf, **conf}
         self.starting_offset = offset
         self.flush_timeout = flush_timeout
         self.poll_timeout = poll_timeout
+        self.consumer = None
         self.producer = None
-        self.callback = callback
+        self._producer_ctx = None
+        self.pusher = pusher
         self.poller = poller
         self.codec = codec
         self.dry = dry
 
     def admin(self):
         """Get admin client."""
         return AdminClient(self.conf)
@@ -298,14 +300,50 @@
     def __iter__(self) -> Iterator[Any]:
         """Consume from topic."""
         c = get_consumer(self.name, self.conf, self.starting_offset, self.codec, self.poll_timeout, self.poller)
         with c as consumer:
             for msg in consumer:
                 yield msg
 
+    def __next__(self) -> Any:
+        """Consume next message from topic."""
+        self.consumer = self.consumer or self.__iter__()
+        return next(self.consumer)
+
+    def __getitem__(self, i) -> Any:
+        """Consume specific range of messages from topic."""
+        if not isinstance(i, (slice, int)):
+            raise TypeError('Expected slice or int.')
+        start, step, stop = (
+            i,
+            None,
+            i + 1 if i >= 0 else None
+        ) if isinstance(i, int) else (
+            i.start,
+            i.step,
+            i.stop
+        )
+        c = get_consumer(self.name, self.conf, start, self.codec, self.poll_timeout, self.poller)
+        with c as consumer:
+            for msg in consumer:
+                if stop and msg.offset() >= stop:
+                    return
+                if step and (msg.offset() - max(0, start)) % step != 0:
+                    continue
+                yield msg
+
     def __call__(self, val, key=None, *args, **kwargs) -> None:
         """Produce to topic."""
+        self._producer_ctx = (
+            self._producer_ctx
+            or get_producer(self.name, self.conf, self.dry, self.codec, self.flush_timeout, self.pusher)
+        )
         self.producer = (
             self.producer or
-            get_producer(self.name, self.conf, self.dry, self.codec, self.flush_timeout, self.callback).__enter__()
+            self._producer_ctx.__enter__()
         )
         self.producer(key, val, *args, **kwargs)
+
+    def __del__(self):
+        """Exit potential producer instance."""
+        if self._producer_ctx:
+            self._producer_ctx.__exit__(None, None, None)
```

### Comparing `snapstream-0.0.4/snapstream/utils.py` & `snapstream-0.0.5/snapstream/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pathlib import Path
 from re import match, sub
 from typing import Any, Dict, Optional
 
 from toolz.curried import compose, curry, last
 
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
 
 
 def get_variable(
     secret: str,
     secrets_base_path='',
     required=False
 ) -> Optional[str]:
@@ -106,10 +105,11 @@
 
 class KafkaIgnoredPropertyFilter(logging.Filter):
     """Filter out specific kafka logging."""
 
     def filter(self, record):
         """Suppress CONFWARN messages with specific config keys."""
         return not (
-            record.levelno == logging.WARNING
-            and 'property and will be ignored' in record.getMessage()
+            (record.levelno == logging.WARNING)
+            and
+            'property and will be ignored' in record.getMessage()
         )
```

### Comparing `snapstream-0.0.4/PKG-INFO` & `snapstream-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 0.0.4
+Version: 0.0.5
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

