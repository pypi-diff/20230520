# Comparing `tmp/python-openapi-0.1.8.tar.gz` & `tmp/python-openapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-openapi-0.1.8.tar", last modified: Sat Nov 19 00:30:18 2022, max compression
+gzip compressed data, was "python-openapi-0.1.9.tar", last modified: Sat May 20 08:00:01 2023, max compression
```

## Comparing `python-openapi-0.1.8.tar` & `python-openapi-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-11-19 00:30:18.015862 python-openapi-0.1.8/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1118 2022-07-22 10:59:25.000000 python-openapi-0.1.8/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10109 2022-11-19 00:30:18.016064 python-openapi-0.1.8/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9187 2022-11-15 20:10:18.000000 python-openapi-0.1.8/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-11-19 00:30:18.013445 python-openapi-0.1.8/pyopenapi/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2026 2022-11-19 00:29:44.000000 python-openapi-0.1.8/pyopenapi/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2022-07-22 10:59:25.000000 python-openapi-0.1.8/pyopenapi/__main__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    21569 2022-11-18 23:36:15.000000 python-openapi-0.1.8/pyopenapi/generator.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      766 2022-09-13 18:14:14.000000 python-openapi-0.1.8/pyopenapi/metadata.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13441 2022-08-05 10:45:08.000000 python-openapi-0.1.8/pyopenapi/operations.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2437 2022-11-15 13:43:11.000000 python-openapi-0.1.8/pyopenapi/options.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4107 2022-07-30 20:07:21.000000 python-openapi-0.1.8/pyopenapi/proxy.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5853 2022-10-03 07:00:52.000000 python-openapi-0.1.8/pyopenapi/specification.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1234 2022-07-30 21:24:42.000000 python-openapi-0.1.8/pyopenapi/template.html
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3474 2022-11-18 23:46:46.000000 python-openapi-0.1.8/pyopenapi/utility.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-07-22 10:59:25.000000 python-openapi-0.1.8/pyproject.toml
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-11-19 00:30:18.015526 python-openapi-0.1.8/python_openapi.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10109 2022-11-19 00:30:17.000000 python-openapi-0.1.8/python_openapi.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      498 2022-11-19 00:30:18.000000 python-openapi-0.1.8/python_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2022-11-19 00:30:17.000000 python-openapi-0.1.8/python_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       39 2022-11-19 00:30:17.000000 python-openapi-0.1.8/python_openapi.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       10 2022-11-19 00:30:17.000000 python-openapi-0.1.8/python_openapi.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2022-11-19 00:30:17.000000 python-openapi-0.1.8/python_openapi.egg-info/zip-safe
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1102 2022-11-19 00:30:18.016845 python-openapi-0.1.8/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-07-22 10:59:25.000000 python-openapi-0.1.8/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-20 08:00:01.392980 python-openapi-0.1.9/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1118 2023-01-04 12:08:59.000000 python-openapi-0.1.9/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10132 2023-05-20 08:00:01.393313 python-openapi-0.1.9/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9187 2023-01-04 12:08:59.000000 python-openapi-0.1.9/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-20 08:00:01.385547 python-openapi-0.1.9/pyopenapi/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2026 2023-05-20 07:58:06.000000 python-openapi-0.1.9/pyopenapi/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-01-04 12:08:59.000000 python-openapi-0.1.9/pyopenapi/__main__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    24134 2023-05-19 20:05:17.000000 python-openapi-0.1.9/pyopenapi/generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      766 2023-05-19 19:47:30.000000 python-openapi-0.1.9/pyopenapi/metadata.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13646 2023-05-19 19:47:34.000000 python-openapi-0.1.9/pyopenapi/operations.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2674 2023-05-19 19:47:37.000000 python-openapi-0.1.9/pyopenapi/options.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4206 2023-05-19 19:47:41.000000 python-openapi-0.1.9/pyopenapi/proxy.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-05-19 18:36:48.000000 python-openapi-0.1.9/pyopenapi/py.typed
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5918 2023-05-19 19:47:45.000000 python-openapi-0.1.9/pyopenapi/specification.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1234 2023-01-04 12:08:59.000000 python-openapi-0.1.9/pyopenapi/template.html
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3707 2023-05-19 19:47:50.000000 python-openapi-0.1.9/pyopenapi/utility.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-01-04 12:08:59.000000 python-openapi-0.1.9/pyproject.toml
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-20 08:00:01.390321 python-openapi-0.1.9/python_openapi.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10132 2023-05-20 08:00:01.000000 python-openapi-0.1.9/python_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      559 2023-05-20 08:00:01.000000 python-openapi-0.1.9/python_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-05-20 08:00:01.000000 python-openapi-0.1.9/python_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       39 2023-05-20 08:00:01.000000 python-openapi-0.1.9/python_openapi.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       10 2023-05-20 08:00:01.000000 python-openapi-0.1.9/python_openapi.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-05-20 08:00:01.000000 python-openapi-0.1.9/python_openapi.egg-info/zip-safe
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1138 2023-05-20 08:00:01.394585 python-openapi-0.1.9/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2023-01-04 12:08:59.000000 python-openapi-0.1.9/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-20 08:00:01.392118 python-openapi-0.1.9/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5636 2023-05-19 19:47:58.000000 python-openapi-0.1.9/tests/test_openapi.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1850 2023-05-19 19:48:02.000000 python-openapi-0.1.9/tests/test_proxy.py
```

### Comparing `python-openapi-0.1.8/LICENSE` & `python-openapi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-openapi-0.1.8/PKG-INFO` & `python-openapi-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-openapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate an OpenAPI specification from a Python class definition
 Home-page: https://github.com/hunyadi/pyopenapi
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Generate an OpenAPI specification from a Python class
 
 *PyOpenAPI* produces an OpenAPI specification in JSON, YAML or HTML format with endpoint definitions extracted from member functions of a strongly-typed Python class.
```

### Comparing `python-openapi-0.1.8/README.md` & `python-openapi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python-openapi-0.1.8/pyopenapi/__init__.py` & `python-openapi-0.1.9/pyopenapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Callable, Optional, TypeVar
 
 from .metadata import WebMethod
 from .options import *
 from .utility import Specification
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 T = TypeVar("T")
 
 
 def webmethod(
     route: Optional[str] = None,
     public: Optional[bool] = False,
```

### Comparing `python-openapi-0.1.8/pyopenapi/generator.py` & `python-openapi-0.1.9/pyopenapi/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+import hashlib
+import ipaddress
+import typing
 from typing import Any, Dict, Set, Union
 
 from strong_typing.core import JsonType
-from strong_typing.docstring import parse_type
+from strong_typing.docstring import Docstring, parse_type
 from strong_typing.inspection import (
     is_generic_list,
     is_type_optional,
     is_type_union,
     unwrap_generic_list,
     unwrap_optional_type,
     unwrap_union_types,
 )
 from strong_typing.name import python_type_to_name
 from strong_typing.schema import (
     JsonSchemaGenerator,
     Schema,
     SchemaOptions,
     get_schema_identifier,
+    register_schema,
 )
-from strong_typing.serialization import object_to_json
+from strong_typing.serialization import json_dump_string, object_to_json
 
 from .operations import (
     EndpointOperation,
     HTTPMethod,
     get_endpoint_events,
     get_endpoint_operations,
 )
@@ -35,21 +39,47 @@
     Operation,
     Parameter,
     ParameterLocation,
     PathItem,
     RequestBody,
     Response,
     ResponseRef,
+    SchemaOrRef,
     SchemaRef,
     Tag,
     TagGroup,
 )
 
+register_schema(
+    ipaddress.IPv4Address,
+    schema={
+        "type": "string",
+        "format": "ipv4",
+        "title": "IPv4 address",
+        "description": "IPv4 address, according to dotted-quad ABNF syntax as defined in RFC 2673, section 3.2.",
+    },
+    examples=["192.0.2.0", "198.51.100.1", "203.0.113.255"],
+)
 
-SchemaOrRef = Union[Schema, SchemaRef]
+register_schema(
+    ipaddress.IPv6Address,
+    schema={
+        "type": "string",
+        "format": "ipv6",
+        "title": "IPv6 address",
+        "description": "IPv6 address, as defined in RFC 2373, section 2.2.",
+    },
+    examples=[
+        "FEDC:BA98:7654:3210:FEDC:BA98:7654:3210",
+        "1080:0:0:0:8:800:200C:417A",
+        "1080::8:800:200C:417A",
+        "FF01::101",
+        "::1",
+    ],
+)
 
 
 def http_status_to_string(status_code: HTTPStatusCode) -> str:
     "Converts an HTTP status code to a string."
 
     if isinstance(status_code, HTTPStatus):
         return str(status_code.value)
@@ -148,40 +178,62 @@
             item_type = payload_type
 
         return {media_type: self.build_media_type(item_type, examples)}
 
     def build_media_type(
         self, item_type: type, examples: Optional[List[Any]] = None
     ) -> MediaType:
-
         schema = self.schema_builder.classdef_to_ref(item_type)
         if self.schema_transformer:
             schema_transformer: Callable[[SchemaOrRef], SchemaOrRef] = self.schema_transformer  # type: ignore
             schema = schema_transformer(schema)
+
+        if not examples:
+            return MediaType(schema=schema)
+
+        if len(examples) == 1:
+            return MediaType(schema=schema, example=self._build_example(examples[0]))
+
         return MediaType(
             schema=schema,
             examples=self._build_examples(examples),
         )
 
     def _build_examples(
-        self, examples: Optional[List[Any]] = None
-    ) -> Optional[Dict[str, Union[Example, ExampleRef]]]:
+        self, examples: List[Any]
+    ) -> Dict[str, Union[Example, ExampleRef]]:
+        "Creates a set of several examples for a media type."
+
+        if self.sample_transformer:
+            sample_transformer: Callable[[JsonType], JsonType] = self.sample_transformer  # type: ignore
+        else:
+            sample_transformer = lambda sample: sample
+
+        results: Dict[str, Union[Example, ExampleRef]] = {}
+        for example in examples:
+            value = sample_transformer(object_to_json(example))
+
+            hash_string = (
+                hashlib.md5(json_dump_string(value).encode("utf-8")).digest().hex()
+            )
+            name = f"ex-{hash_string}"
 
-        if examples is None:
-            return None
+            results[name] = Example(value=value)
+
+        return results
+
+    def _build_example(self, example: Any) -> Any:
+        "Creates a single example for a media type."
 
         if self.sample_transformer:
             sample_transformer: Callable[[JsonType], JsonType] = self.sample_transformer  # type: ignore
         else:
             sample_transformer = lambda sample: sample
 
-        return {
-            str(example): Example(value=sample_transformer(object_to_json(example)))
-            for example in examples
-        }
+        return sample_transformer(object_to_json(example))
 
 
 @dataclass
 class ResponseOptions:
     """
     Configuration options for building a response for an operation.
 
@@ -232,15 +284,15 @@
             if options.examples:
                 status_response.examples.extend(
                     example
                     for example in options.examples
                     if isinstance(example, response_type)
                 )
 
-        return status_responses
+        return dict(sorted(status_responses.items()))
 
     def build_response(
         self, options: ResponseOptions
     ) -> Dict[str, Union[Response, ResponseRef]]:
         """
         Groups responses that have the same status code.
         """
@@ -286,36 +338,58 @@
                 description=description,
                 content=self.content_builder.build_content(response_type, examples),
             )
         else:
             return Response(description=description)
 
 
+def schema_error_wrapper(schema: SchemaOrRef) -> Schema:
+    "Wraps an error output schema into a top-level error schema."
+
+    return {
+        "type": "object",
+        "properties": {
+            "error": schema,  # type: ignore
+        },
+        "additionalProperties": False,
+        "required": [
+            "error",
+        ],
+    }
+
+
+def sample_error_wrapper(error: JsonType) -> JsonType:
+    "Wraps an error output sample into a top-level error sample."
+
+    return {"error": error}
+
+
 class Generator:
     endpoint: type
     options: Options
     schema_builder: SchemaBuilder
     responses: Dict[str, Response]
 
     def __init__(self, endpoint: type, options: Options) -> None:
         self.endpoint = endpoint
         self.options = options
         schema_generator = JsonSchemaGenerator(
             SchemaOptions(
                 definitions_path="#/components/schemas/",
+                use_examples=self.options.use_examples,
                 property_description_fun=options.property_description_fun,
             )
         )
         self.schema_builder = SchemaBuilder(schema_generator)
         self.responses = {}
 
     def _build_type_tag(self, ref: str, schema: Schema) -> Tag:
         definition = f'<SchemaDefinition schemaRef="#/components/schemas/{ref}" />'
-        title = schema.get("title")
-        description = schema.get("description")
+        title = typing.cast(str, schema.get("title"))
+        description = typing.cast(str, schema.get("description"))
         return Tag(
             name=ref,
             description="\n\n".join(
                 s for s in (title, description, definition) if s is not None
             ),
         )
 
@@ -334,15 +408,16 @@
             tag_list: List[Tag] = []
 
             for extra_type in category_items:
                 name = python_type_to_name(extra_type)
                 schema = self.schema_builder.classdef_to_named_schema(name, extra_type)
                 tag_list.append(self._build_type_tag(name, schema))
 
-            extra_tags[category_name] = tag_list
+            if tag_list:
+                extra_tags[category_name] = tag_list
 
         return extra_tags
 
     def _build_operation(self, op: EndpointOperation) -> Operation:
         doc_string = parse_type(op.func_ref)
         doc_params = dict(
             (param.name, param.description) for param in doc_string.params.values()
@@ -360,15 +435,15 @@
             for param_name, param_type in op.path_params
         ]
 
         # parameters passed in URL component query string
         query_parameters = []
         for param_name, param_type in op.query_params:
             if is_type_optional(param_type):
-                inner_type = unwrap_optional_type(param_type)
+                inner_type: type = unwrap_optional_type(param_type)
                 required = False
             else:
                 inner_type = param_type
                 required = True
 
             query_parameter = Parameter(
                 name=param_name,
@@ -397,18 +472,23 @@
             )
         else:
             requestBody = None
 
         # success response types
         if doc_string.returns is None and is_type_union(op.response_type):
             # split union of return types into a list of response types
-            success_type_descriptions = {
-                item: parse_type(item).short_description
+            success_type_docstring: Dict[type, Docstring] = {
+                typing.cast(type, item): parse_type(item)
                 for item in unwrap_union_types(op.response_type)
             }
+            success_type_descriptions = {
+                item: doc_string.short_description
+                for item, doc_string in success_type_docstring.items()
+                if doc_string.short_description
+            }
         else:
             # use return type as a single response type
             success_type_descriptions = {
                 op.response_type: (
                     doc_string.returns.description if doc_string.returns else "OK"
                 )
             }
@@ -420,15 +500,15 @@
             if not isinstance(example, Exception)
         ]
 
         content_builder = ContentBuilder(self.schema_builder)
         response_builder = ResponseBuilder(content_builder)
         response_options = ResponseOptions(
             success_type_descriptions,
-            success_examples,
+            success_examples if self.options.use_examples else None,
             self.options.success_responses,
             "200",
         )
         responses = response_builder.build_response(response_options)
 
         # failure response types
         if doc_string.raises:
@@ -438,38 +518,29 @@
             exception_examples = [
                 example
                 for example in response_examples
                 if isinstance(example, Exception)
             ]
 
             if self.options.error_wrapper:
-                schema_transformer = lambda schema: {
-                    "type": "object",
-                    "properties": {
-                        "error": schema,
-                    },
-                    "additionalProperties": False,
-                    "required": [
-                        "error",
-                    ],
-                }
-                sample_transformer = lambda error: {"error": error}
+                schema_transformer = schema_error_wrapper
+                sample_transformer = sample_error_wrapper
             else:
                 schema_transformer = None
                 sample_transformer = None
 
             content_builder = ContentBuilder(
                 self.schema_builder,
                 schema_transformer=schema_transformer,
                 sample_transformer=sample_transformer,
             )
             response_builder = ResponseBuilder(content_builder)
             response_options = ResponseOptions(
                 exception_types,
-                exception_examples,
+                exception_examples if self.options.use_examples else None,
                 self.options.error_responses,
                 "500",
             )
             responses.update(response_builder.build_response(response_options))
 
         if op.event_type is not None:
             builder = ContentBuilder(self.schema_builder)
@@ -499,15 +570,17 @@
             callbacks=callbacks,
             security=[] if op.public else None,
         )
 
     def generate(self) -> Document:
         paths: Dict[str, PathItem] = {}
         endpoint_classes: Set[type] = set()
-        for op in get_endpoint_operations(self.endpoint):
+        for op in get_endpoint_operations(
+            self.endpoint, use_examples=self.options.use_examples
+        ):
             endpoint_classes.add(op.defining_class)
 
             operation = self._build_operation(op)
 
             if op.http_method is HTTPMethod.GET:
                 pathItem = PathItem(get=operation)
             elif op.http_method is HTTPMethod.PUT:
@@ -607,16 +680,21 @@
 
         if self.options.default_security_scheme:
             securitySchemes = {"Default": self.options.default_security_scheme}
         else:
             securitySchemes = None
 
         return Document(
-            openapi="3.1.0",
+            openapi=".".join(str(item) for item in self.options.version),
             info=self.options.info,
+            jsonSchemaDialect=(
+                "https://json-schema.org/draft/2020-12/schema"
+                if self.options.version >= (3, 1, 0)
+                else None
+            ),
             servers=[self.options.server],
             paths=paths,
             components=Components(
                 schemas=self.schema_builder.schemas,
                 responses=self.responses,
                 securitySchemes=securitySchemes,
             ),
```

### Comparing `python-openapi-0.1.8/pyopenapi/metadata.py` & `python-openapi-0.1.9/pyopenapi/metadata.py`

 * *Files identical despite different names*

### Comparing `python-openapi-0.1.8/pyopenapi/operations.py` & `python-openapi-0.1.9/pyopenapi/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,16 @@
     path_params: List[OperationParameter]
     query_params: List[OperationParameter]
     request_param: Optional[OperationParameter]
     event_type: Optional[type]
     response_type: type
     http_method: HTTPMethod
     public: bool
-    request_examples: Optional[List[Any]]
-    response_examples: Optional[List[Any]]
+    request_examples: Optional[List[Any]] = None
+    response_examples: Optional[List[Any]] = None
 
     def get_route(self) -> str:
         if self.route is not None:
             return self.route
 
         route_parts = ["", self.name]
         for param_name, _ in self.path_params:
@@ -114,32 +114,31 @@
 
 
 class _FormatParameterExtractor:
     "A visitor to exract parameters in a format string."
 
     keys: List[str]
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.keys = []
 
-    def __getitem__(self, key: str):
+    def __getitem__(self, key: str) -> None:
         self.keys.append(key)
         return None
 
 
 def _get_route_parameters(route: str) -> List[str]:
     extractor = _FormatParameterExtractor()
     route.format_map(extractor)
     return extractor.keys
 
 
 def _get_endpoint_functions(
     endpoint: type, prefixes: List[str]
 ) -> Iterator[Tuple[str, str, str, Callable]]:
-
     if not inspect.isclass(endpoint):
         raise ValidationError(f"object is not a class type: {endpoint}")
 
     functions = inspect.getmembers(endpoint, inspect.isfunction)
     for func_name, func_ref in functions:
         prefix, operation_name = split_prefix(func_name, "_", prefixes)
         if not prefix:
@@ -158,15 +157,17 @@
                 return cls
 
     raise ValidationError(
         f"cannot find defining class for {member_fn} in {derived_cls}"
     )
 
 
-def get_endpoint_operations(endpoint: type) -> List[EndpointOperation]:
+def get_endpoint_operations(
+    endpoint: type, use_examples: bool = True
+) -> List[EndpointOperation]:
     """
     Extracts a list of member functions in a class eligible for HTTP interface binding.
 
     These member functions are expected to have a signature like
     ```
     async def get_object(self, uuid: str, version: int) -> Object:
         ...
@@ -175,14 +176,15 @@
     `uuid` and `version` are mapped to route path elements in "/object/{uuid}/{version}", and `Object` becomes
     the response payload type, transmitted as an object serialized to JSON.
 
     If the member function has a composite class type in the argument list, it becomes the request payload type,
     and the caller is expected to provide the data as serialized JSON in an HTTP POST request.
 
     :param endpoint: A class with member functions that can be mapped to an HTTP endpoint.
+    :param use_examples: Whether to return examples associated with member functions.
     """
 
     result = []
 
     for prefix, operation_name, func_name, func_ref in _get_endpoint_functions(
         endpoint,
         [
@@ -193,15 +195,14 @@
             "post",
             "put",
             "remove",
             "set",
             "update",
         ],
     ):
-
         # extract routing information from function metadata
         webmethod: Optional[WebMethod] = getattr(func_ref, "__webmethod__", None)
         if webmethod is not None:
             route = webmethod.route
             route_params = _get_route_parameters(route) if route is not None else None
             public = webmethod.public
             request_examples = webmethod.request_examples
@@ -230,15 +231,15 @@
             # check if all parameters have explicit type
             if parameter.annotation is inspect.Parameter.empty:
                 raise ValidationError(
                     f"parameter '{param_name}' in function '{func_name}' has no type annotation"
                 )
 
             if is_type_optional(param_type):
-                inner_type = unwrap_optional_type(param_type)
+                inner_type: type = unwrap_optional_type(param_type)
             else:
                 inner_type = param_type
 
             if (
                 inner_type is bool
                 or inner_type is int
                 or inner_type is float
@@ -321,16 +322,16 @@
                 path_params=path_params,
                 query_params=query_params,
                 request_param=request_param,
                 event_type=event_type,
                 response_type=response_type,
                 http_method=http_method,
                 public=public,
-                request_examples=request_examples,
-                response_examples=response_examples,
+                request_examples=request_examples if use_examples else None,
+                response_examples=response_examples if use_examples else None,
             )
         )
 
     if not result:
         raise ValidationError(f"no eligible endpoint operations in type {endpoint}")
 
     return result
```

### Comparing `python-openapi-0.1.8/pyopenapi/options.py` & `python-openapi-0.1.9/pyopenapi/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dataclasses
 from dataclasses import dataclass
 from http import HTTPStatus
-from typing import Callable, ClassVar, Dict, List, Optional, Union
+from typing import Callable, ClassVar, Dict, List, Optional, Tuple, Union
 
 from .specification import (
     Info,
     SecurityScheme,
     SecuritySchemeAPI,
     SecuritySchemeHTTP,
     SecuritySchemeOpenIDConnect,
@@ -16,27 +16,31 @@
 
 
 @dataclass
 class Options:
     """
     :param server: Base URL for the API endpoint.
     :param info: Meta-information for the endpoint specification.
+    :param version: OpenAPI specification version as a tuple of major, minor, revision.
     :param default_security_scheme: Security scheme to apply to endpoints, unless overridden on a per-endpoint basis.
     :param extra_types: Extra types in addition to those found in operation signatures. Use a dictionary to group related types.
+    :param use_examples: Whether to emit examples for operations.
     :param success_responses: Associates operation response types with HTTP status codes.
     :param error_responses: Associates error response types with HTTP status codes.
     :param error_wrapper: True if errors are encapsulated in an error object wrapper.
     :param property_description_fun: Custom transformation function to apply to class property documentation strings.
     :param captions: User-defined captions for sections such as "Operations" or "Types", and (if applicable) groups of extra types.
     """
 
     server: Server
     info: Info
+    version: Tuple[int, int, int] = (3, 1, 0)
     default_security_scheme: Optional[SecurityScheme] = None
     extra_types: Union[List[type], Dict[str, List[type]], None] = None
+    use_examples: bool = True
     success_responses: Dict[type, HTTPStatusCode] = dataclasses.field(
         default_factory=dict
     )
     error_responses: Dict[type, HTTPStatusCode] = dataclasses.field(
         default_factory=dict
     )
     error_wrapper: bool = False
```

### Comparing `python-openapi-0.1.8/pyopenapi/proxy.py` & `python-openapi-0.1.9/pyopenapi/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Dict, Optional, Tuple, Type, TypeVar
+from typing import Any, Callable, Dict, Optional, Tuple, Type, TypeVar
 
 import aiohttp
 from strong_typing.serialization import json_to_object, object_to_json
 
 from .operations import (
     EndpointOperation,
     HTTPMethod,
@@ -65,15 +65,17 @@
     payload, builds an HTTP request, and processes the HTTP response.
     """
 
     def __init__(self, op: EndpointOperation):
         self.op = op
         self.sig = get_signature(op.func_ref)
 
-    async def __call__(self, endpoint_proxy: EndpointProxy, *args, **kwargs):
+    async def __call__(
+        self, endpoint_proxy: EndpointProxy, *args: Any, **kwargs: Any
+    ) -> Any:
         "Invokes an API operation via HTTP REST."
 
         ba = self.sig.bind(self, *args, **kwargs)
 
         # substitute parameters in URL path
         route = self.op.get_route()
         path = route.format_map(
@@ -111,20 +113,22 @@
                 )
 
             return json_to_object(self.op.response_type, s)
         else:
             return None
 
 
-def _get_operation_proxy(op: EndpointOperation):
+def _get_operation_proxy(op: EndpointOperation) -> Callable[..., Any]:
     "Wraps an operation into a function that calls the corresponding HTTP REST API operation."
 
     operation_proxy = OperationProxy(op)
 
-    async def _operation_proxy_fn(self: EndpointProxy, *args, **kwargs):
+    async def _operation_proxy_fn(
+        self: EndpointProxy, *args: Any, **kwargs: Any
+    ) -> Any:
         return await operation_proxy(self, *args, **kwargs)
 
     return _operation_proxy_fn
 
 
 T = TypeVar("T")
```

### Comparing `python-openapi-0.1.8/pyopenapi/specification.py` & `python-openapi-0.1.9/pyopenapi/specification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from __future__ import annotations
-
 import dataclasses
 import enum
 from dataclasses import dataclass
 from typing import Any, ClassVar, Dict, List, Optional, Union
 
-from strong_typing.schema import JsonType, StrictJsonType, Schema
+from strong_typing.schema import JsonType, Schema, StrictJsonType
 
 URL = str
 
 
 @dataclass
 class Ref:
     ref_type: ClassVar[str]
@@ -20,14 +18,17 @@
 
 
 @dataclass
 class SchemaRef(Ref):
     ref_type: ClassVar[str] = "schemas"
 
 
+SchemaOrRef = Union[Schema, SchemaRef]
+
+
 @dataclass
 class ResponseRef(Ref):
     ref_type: ClassVar[str] = "responses"
 
 
 @dataclass
 class ParameterRef(Ref):
@@ -60,17 +61,17 @@
     termsOfService: Optional[str] = None
     contact: Optional[Contact] = None
     license: Optional[License] = None
 
 
 @dataclass
 class MediaType:
-    schema: Optional[Schema] = None
+    schema: Optional[SchemaOrRef] = None
     example: Optional[Any] = None
-    examples: Optional[Dict[str, Union[Example, ExampleRef]]] = None
+    examples: Optional[Dict[str, Union["Example", ExampleRef]]] = None
 
 
 @dataclass
 class RequestBody:
     content: Dict[str, MediaType]
     description: Optional[str] = None
     required: Optional[bool] = None
@@ -91,29 +92,29 @@
 
 @dataclass
 class Parameter:
     name: str
     in_: ParameterLocation
     description: Optional[str] = None
     required: Optional[bool] = None
-    schema: Optional[Schema] = None
+    schema: Optional[SchemaOrRef] = None
     example: Optional[Any] = None
 
 
 @dataclass
 class Operation:
     responses: Dict[str, Union[Response, ResponseRef]]
     tags: Optional[List[str]] = None
     summary: Optional[str] = None
     description: Optional[str] = None
     operationId: Optional[str] = None
     parameters: Optional[List[Parameter]] = None
     requestBody: Optional[RequestBody] = None
     callbacks: Optional[Dict[str, "Callback"]] = None
-    security: Optional[List[SecurityRequirement]] = None
+    security: Optional[List["SecurityRequirement"]] = None
 
 
 @dataclass
 class PathItem:
     summary: Optional[str] = None
     description: Optional[str] = None
     get: Optional[Operation] = None
@@ -121,15 +122,15 @@
     post: Optional[Operation] = None
     delete: Optional[Operation] = None
     options: Optional[Operation] = None
     head: Optional[Operation] = None
     patch: Optional[Operation] = None
     trace: Optional[Operation] = None
 
-    def update(self, other: PathItem) -> None:
+    def update(self, other: "PathItem") -> None:
         "Merges another instance of this class into this object."
 
         for field in dataclasses.fields(self.__class__):
             value = getattr(other, field.name)
             if value is not None:
                 setattr(self, field.name, value)
 
@@ -240,11 +241,12 @@
     For details, see <https://swagger.io/specification/>
     """
 
     openapi: str
     info: Info
     servers: List[Server]
     paths: Dict[str, PathItem]
+    jsonSchemaDialect: Optional[str] = None
     components: Optional[Components] = None
     security: Optional[List[SecurityRequirement]] = None
     tags: Optional[List[Tag]] = None
     tagGroups: Optional[List[TagGroup]] = None
```

### Comparing `python-openapi-0.1.8/pyopenapi/template.html` & `python-openapi-0.1.9/pyopenapi/template.html`

 * *Files identical despite different names*

### Comparing `python-openapi-0.1.8/pyopenapi/utility.py` & `python-openapi-0.1.9/pyopenapi/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import importlib.resources
 import json
 import sys
+import typing
 from typing import TextIO
 
 from strong_typing.schema import StrictJsonType, object_to_json
 
 from .generator import Generator
-from .specification import Document
 from .options import Options
+from .specification import Document
 
 
 class Specification:
     document: Document
 
     def __init__(self, endpoint: type, options: Options):
         generator = Generator(endpoint, options)
@@ -20,26 +21,30 @@
     def get_json(self) -> StrictJsonType:
         """
         Returns the OpenAPI specification as a Python data type (e.g. `dict` for an object, `list` for an array).
 
         The result can be serialized to a JSON string with `json.dump` or `json.dumps`.
         """
 
-        json_doc = object_to_json(self.document)
+        json_doc = typing.cast(StrictJsonType, object_to_json(self.document))
 
-        # rename vendor-specific properties
-        tag_groups = json_doc.pop("tagGroups", None)
-        if tag_groups:
-            json_doc["x-tagGroups"] = tag_groups
-        tags = json_doc.get("tags")
-        if tags:
-            for tag in tags:
-                display_name = tag.pop("displayName", None)
-                if display_name:
-                    tag["x-displayName"] = display_name
+        if isinstance(json_doc, dict):
+            # rename vendor-specific properties
+            tag_groups = json_doc.pop("tagGroups", None)
+            if tag_groups:
+                json_doc["x-tagGroups"] = tag_groups
+            tags = json_doc.get("tags")
+            if tags and isinstance(tags, list):
+                for tag in tags:
+                    if not isinstance(tag, dict):
+                        continue
+
+                    display_name = tag.pop("displayName", None)
+                    if display_name:
+                        tag["x-displayName"] = display_name
 
         return json_doc
 
     def get_json_string(self, pretty_print: bool = False) -> str:
         """
         Returns the OpenAPI specification as a JSON string.
```

### Comparing `python-openapi-0.1.8/python_openapi.egg-info/PKG-INFO` & `python-openapi-0.1.9/python_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-openapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate an OpenAPI specification from a Python class definition
 Home-page: https://github.com/hunyadi/pyopenapi
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Generate an OpenAPI specification from a Python class
 
 *PyOpenAPI* produces an OpenAPI specification in JSON, YAML or HTML format with endpoint definitions extracted from member functions of a strongly-typed Python class.
```

### Comparing `python-openapi-0.1.8/setup.cfg` & `python-openapi-0.1.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 	Typing :: Typed
 
 [options]
 zip_safe = True
 include_package_data = True
 packages = find:
+python_requires = >=3.8
 install_requires = 
 	aiohttp >= 3.8
-	json_strong_typing >= 0.2.4
+	json_strong_typing >= 0.2.7
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [options.package_data]
-pyopenapi = *.html
+pyopenapi = 
+	*.html
+	py.typed
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

