# Comparing `tmp/osgiservicebridge-1.5.1.tar.gz` & `tmp/osgiservicebridge-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\osgiservicebridge-1.5.1.tar", last modified: Wed Apr  3 04:22:44 2019, max compression
+gzip compressed data, was "osgiservicebridge-1.5.2.tar", last modified: Sat May 20 00:03:47 2023, max compression
```

## Comparing `osgiservicebridge-1.5.1.tar` & `osgiservicebridge-1.5.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2019-04-03 04:22:44.000000 osgiservicebridge-1.5.1/
-drwxrwxrwx   0        0        0        0 2019-04-03 04:22:44.000000 osgiservicebridge-1.5.1/java/
--rw-rw-rw-   0        0        0  1866128 2019-04-02 02:56:24.000000 osgiservicebridge-1.5.1/java/py4j-remoteservicesprovider_2.9.0.zip
--rw-rw-rw-   0        0        0     1222 2019-04-03 04:22:44.000000 osgiservicebridge-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      283 2019-03-24 04:27:07.000000 osgiservicebridge-1.5.1/README.rst
--rw-rw-rw-   0        0        0       74 2019-04-03 04:22:44.000000 osgiservicebridge-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     4696 2019-04-03 04:16:43.000000 osgiservicebridge-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2019-04-03 04:22:44.000000 osgiservicebridge-1.5.1/src/
-drwxrwxrwx   0        0        0        0 2019-04-03 04:22:44.000000 osgiservicebridge-1.5.1/src/osgiservicebridge/
--rw-rw-rw-   0        0        0    48312 2019-03-24 05:57:28.000000 osgiservicebridge-1.5.1/src/osgiservicebridge/bridge.py
--rw-rw-rw-   0        0        0    13213 2019-03-24 04:27:08.000000 osgiservicebridge-1.5.1/src/osgiservicebridge/exporter_pb2.py
--rw-rw-rw-   0        0        0    11085 2019-03-24 04:27:07.000000 osgiservicebridge-1.5.1/src/osgiservicebridge/flatbuf.py
--rw-rw-rw-   0        0        0    31586 2019-04-03 01:23:28.000000 osgiservicebridge-1.5.1/src/osgiservicebridge/protobuf.py
--rw-rw-rw-   0        0        0       20 2019-04-03 04:02:40.000000 osgiservicebridge-1.5.1/src/osgiservicebridge/version.py
--rw-rw-rw-   0        0        0    17269 2019-03-24 04:27:08.000000 osgiservicebridge-1.5.1/src/osgiservicebridge/__init__.py
-drwxrwxrwx   0        0        0        0 2019-04-03 04:22:44.000000 osgiservicebridge-1.5.1/src/osgiservicebridge.egg-info/
--rw-rw-rw-   0        0        0        1 2019-04-03 04:22:43.000000 osgiservicebridge-1.5.1/src/osgiservicebridge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1222 2019-04-03 04:22:43.000000 osgiservicebridge-1.5.1/src/osgiservicebridge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       29 2019-04-03 04:22:43.000000 osgiservicebridge-1.5.1/src/osgiservicebridge.egg-info/requires.txt
--rw-rw-rw-   0        0        0      500 2019-04-03 04:22:43.000000 osgiservicebridge-1.5.1/src/osgiservicebridge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       18 2019-04-03 04:22:43.000000 osgiservicebridge-1.5.1/src/osgiservicebridge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.536032 osgiservicebridge-1.5.2/
+-rw-rw-rw-   0        0        0    11558 2019-03-24 04:27:06.000000 osgiservicebridge-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-05-20 00:03:47.536032 osgiservicebridge-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-19 20:02:04.000000 osgiservicebridge-1.5.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.499713 osgiservicebridge-1.5.2/java/
+-rw-rw-rw-   0        0        0  2778718 2023-05-19 19:42:54.000000 osgiservicebridge-1.5.2/java/py4j-remoteservicesprovider_2.11.0.zip
+-rw-rw-rw-   0        0        0       99 2023-05-19 23:48:27.000000 osgiservicebridge-1.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       74 2023-05-20 00:03:47.538037 osgiservicebridge-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     4751 2023-05-19 23:53:23.000000 osgiservicebridge-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.491421 osgiservicebridge-1.5.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.511026 osgiservicebridge-1.5.2/src/osgiservicebridge/
+-rw-rw-rw-   0        0        0    17269 2023-05-17 22:26:05.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/__init__.py
+-rw-rw-rw-   0        0        0    49609 2023-05-18 23:34:21.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/bridge.py
+-rw-rw-rw-   0        0        0     2475 2023-05-17 22:27:56.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/exporter_pb2.py
+-rw-rw-rw-   0        0        0    11085 2023-05-17 22:26:05.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/flatbuf.py
+-rw-rw-rw-   0        0        0    31593 2023-05-17 22:30:57.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/protobuf.py
+-rw-rw-rw-   0        0        0       20 2023-05-20 00:03:06.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/version.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.535035 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `osgiservicebridge-1.5.1/PKG-INFO` & `osgiservicebridge-1.5.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: osgiservicebridge
-Version: 1.5.1
+Version: 1.5.2
 Summary: OSGi services implemented in Python
 Home-page: https://github.com/ECF/Py4j-RemoteServicesProvider
 Author: Scott Lewis
 Author-email: scottslewis@gmail.com
 License: Apache Software License
-Description: osgiservicebridge provides the Python library for OSGi R7 remote services between Java and Python.  See the github project at https://github.com/ECF/Py4j-RemoteServicesProvider for detailed information about OSGi remote services and for examples
 Keywords: Java Python OSGi development
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Java
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Object Brokering
+License-File: LICENSE
+
+osgiservicebridge provides the Python library for OSGi R7 remote services between Java and Python.  See the github project at https://github.com/ECF/Py4j-RemoteServicesProvider for detailed information about OSGi remote services and for examples
```

### Comparing `osgiservicebridge-1.5.1/setup.py` & `osgiservicebridge-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 VERSION_PATH = os.path.join("src", "osgiservicebridge", "version.py")
 # For Python 3 compatibility, we can't use execfile; this is 2to3's conversion:
 exec(compile(open(VERSION_PATH).read(),
      VERSION_PATH, "exec"))
 VERSION = __version__  # noqa
 
-JAVA_FILE='java/py4j-remoteservicesprovider_2.9.0.zip'
+JAVA_FILE='java/py4j-remoteservicesprovider_2.11.0.zip'
 
 setup(
     name='osgiservicebridge',
     packages=find_packages(where='src'),
     package_dir={"": "src"},
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
@@ -61,19 +61,20 @@
         'Topic :: Software Development :: Build Tools',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: Apache Software License',
 
         # Specify the Python versions you support here. In particular, ensure
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        "Programming Language :: Java",
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+       "Programming Language :: Java",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Object Brokering",
     ],
 
     # What does your project relate to?
     keywords='Java Python OSGi development',
 
@@ -85,15 +86,15 @@
     # this:
     #   py_modules=["my_module"],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['py4j>=0.10.7','protobuf>=3.7.0'],
+    install_requires=['py4j>=0.10.9.7','protobuf==3.22.2'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     #extras_require={
     #    'dev': ['check-manifest'],
```

### Comparing `osgiservicebridge-1.5.1/src/osgiservicebridge/bridge.py` & `osgiservicebridge-1.5.2/src/osgiservicebridge/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,51 @@
         Remove a single path (string) from the sys.path
         '''
         pass
         
     class Java:
         implements = [JAVA_PATH_PROVIDER]
                 
+from py4j.java_collections import JavaMap, JavaMember, JavaIterator, register_output_converter
+from py4j import protocol as proto
+
+class BridgeJavaIterator(JavaIterator):
+    def __init__(self, target_id, gateway_client):
+        JavaIterator.__init__(self, target_id, gateway_client)
+
+    def next(self):
+        if self._next_name not in self._methods:
+            self._methods[self._next_name] = JavaMember(
+                self._next_name, self,
+                self._target_id, self._gateway_client)
+        if self.hasNext():
+            return self._methods[self._next_name]()
+        else:
+            raise StopIteration()
+        
+    __next__ = next
+    
+class BridgeJavaMap(JavaMap):
+    
+    def __init__(self, target_id, gateway_client):
+        JavaMap.__init__(self, target_id, gateway_client)
+        
+    def __repr__(self):
+        items = (
+            "{0}: {1}".format(repr(k), repr(self.get(k)))
+            for k in self.keySet())
+        return "{{{0}}}".format(", ".join(items))
+    
+register_output_converter(
+proto.MAP_TYPE, lambda target_id, gateway_client:
+BridgeJavaMap(target_id, gateway_client))
+register_output_converter(
+proto.ITERATOR_TYPE, lambda target_id, gateway_client:
+BridgeJavaIterator(target_id, gateway_client))
+
 class Py4jServiceBridge(object):
     '''Py4jServiceBridge class
     This class provides and API for consumers to use the Py4jServiceBridge.  This 
     allows a bridge between Python and the OSGi service registry.
     '''
     def __init__(self,service_listener=None,connection_listener=None,gateway_parameters=None,callback_server_parameters=None):
         self._gateway = None
```

### Comparing `osgiservicebridge-1.5.1/src/osgiservicebridge/flatbuf.py` & `osgiservicebridge-1.5.2/src/osgiservicebridge/flatbuf.py`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.1/src/osgiservicebridge/protobuf.py` & `osgiservicebridge-1.5.2/src/osgiservicebridge/protobuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,34 +25,34 @@
 import osgiservicebridge
 from osgiservicebridge import ENDPOINT_PACKAGE_VERSION_
 
 import time
 
 from google.protobuf.message import Message
 from google.protobuf.descriptor import EnumDescriptor, EnumValueDescriptor, Descriptor, FieldDescriptor, _OptionsOrNone
-from google.protobuf.descriptor_pb2 import DescriptorProto
 from osgiservicebridge.bridge import JavaRemoteServiceRegistry, Py4jServiceBridgeEventListener,\
     JavaServiceMethod, JavaServiceProxy, JAVA_OBJECT_METHODS,\
     ServiceMethod, get_interfaces,\
     get_return_methtype, Py4jService, PythonServiceMethod
 
 from osgiservicebridge import ECF_SERVICE_EXPORTED_ASYNC_INTERFACES
 
 from osgiservicebridge.exporter_pb2 import ExportRequest,ExportResponse,UnexportRequest,UnexportResponse
 from concurrent.futures._base import Future
 from concurrent.futures.thread import ThreadPoolExecutor
 from google.protobuf import symbol_database, descriptor_pool
-from _thread import RLock
+from threading import RLock
 from google.protobuf.internal import api_implementation
+from google.protobuf.descriptor_pb2 import _DESCRIPTORPROTO
 
 _USE_C_DESCRIPTORS = False
 if api_implementation.Type() == 'cpp':  
     # Used by MakeDescriptor in cpp mode
     import binascii
-    from google.protobuf.pyext import _message
+    from google.protobuf import message as _message
     _USE_C_DESCRIPTORS = getattr(_message, '_USE_C_DESCRIPTORS', False)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 from osgiservicebridge.version import __version__ as __v__
 # Version
@@ -470,15 +470,15 @@
 def MakeClassDescriptor(descriptor_pool, desc_proto, package='', build_file_if_cpp=True, syntax=None):
     if api_implementation.Type() == 'cpp' and build_file_if_cpp:
         # The C++ implementation requires all descriptors to be backed by the same
         # definition in the C++ descriptor pool. To do this, we build a
         # FileDescriptorProto with the same definition as this descriptor and build
         # it into the pool.
         from google.protobuf import descriptor_pb2
-        file_descriptor_proto = descriptor_pb2.FileDescriptorProto()
+        file_descriptor_proto = descriptor_pb2._FIELDDESCRIPTORPROTO
         file_descriptor_proto.message_type.add().MergeFrom(desc_proto)
 
         # Generate a random name for this proto file to prevent conflicts with any
         # imported ones. We need to specify a file name so the descriptor pool
         # accepts our FileDescriptorProto, but it is not important what that file
         # name is actually set to.
         proto_name = binascii.hexlify(os.urandom(16)).decode('ascii')
@@ -561,15 +561,15 @@
     
     def __init__(self, java_class, pool = _default_descriptor_pool):
         self._descriptor_pool = pool
         self._java_class = java_class
         jdesc_bytes = java_class.getMethod("getDescriptor",None).invoke(None,None).toProto().toByteArray()
         if PY2:
             jdesc_bytes = str(jdesc_bytes)
-        pdesc_proto = DescriptorProto()
+        pdesc_proto = _DESCRIPTORPROTO
         pdesc_proto.MergeFromString(jdesc_bytes)
         try:
             pdesc_proto_desc = self._descriptor_pool.FindFileContainingSymbol(pdesc_proto.name).message_types_by_name[pdesc_proto.name]
         except KeyError:
             pdesc_proto_desc = MakeClassDescriptor(self._descriptor_pool, pdesc_proto)
         self._python_class = _default_symbol_db.GetPrototype(pdesc_proto_desc)
```

### Comparing `osgiservicebridge-1.5.1/src/osgiservicebridge/__init__.py` & `osgiservicebridge-1.5.2/src/osgiservicebridge/__init__.py`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.1/src/osgiservicebridge.egg-info/PKG-INFO` & `osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: osgiservicebridge
-Version: 1.5.1
+Version: 1.5.2
 Summary: OSGi services implemented in Python
 Home-page: https://github.com/ECF/Py4j-RemoteServicesProvider
 Author: Scott Lewis
 Author-email: scottslewis@gmail.com
 License: Apache Software License
-Description: osgiservicebridge provides the Python library for OSGi R7 remote services between Java and Python.  See the github project at https://github.com/ECF/Py4j-RemoteServicesProvider for detailed information about OSGi remote services and for examples
 Keywords: Java Python OSGi development
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Java
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Object Brokering
+License-File: LICENSE
+
+osgiservicebridge provides the Python library for OSGi R7 remote services between Java and Python.  See the github project at https://github.com/ECF/Py4j-RemoteServicesProvider for detailed information about OSGi remote services and for examples
```

