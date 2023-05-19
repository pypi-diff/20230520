# Comparing `tmp/stablerandom-0.5.40.tar.gz` & `tmp/stablerandom-0.6.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stablerandom-0.5.40.tar", max compression
+gzip compressed data, was "stablerandom-0.6.44.tar", max compression
```

## Comparing `stablerandom-0.5.40.tar` & `stablerandom-0.6.44.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-03-02 19:28:51.060564 stablerandom-0.5.40/LICENSE.txt
--rw-r--r--   0        0        0     1526 2023-03-02 19:28:51.060564 stablerandom-0.5.40/README.md
--rw-r--r--   0        0        0      452 2023-03-02 19:29:15.092510 stablerandom-0.5.40/pyproject.toml
--rw-r--r--   0        0        0      145 2023-03-02 19:28:51.060564 stablerandom-0.5.40/stablerandom/__init__.py
--rw-r--r--   0        0        0     3404 2023-03-02 19:28:51.060564 stablerandom-0.5.40/stablerandom/stablerandom.py
--rw-r--r--   0        0        0     2507 2023-03-02 19:28:51.060564 stablerandom-0.5.40/stablerandom/stablerandom_test.py
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 stablerandom-0.5.40/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 22:47:15.852869 stablerandom-0.6.44/LICENSE.txt
+-rw-r--r--   0        0        0     2040 2023-05-19 22:47:15.852869 stablerandom-0.6.44/README.md
+-rw-r--r--   0        0        0      452 2023-05-19 22:47:31.529219 stablerandom-0.6.44/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-05-19 22:47:15.852869 stablerandom-0.6.44/stablerandom/__init__.py
+-rw-r--r--   0        0        0     3633 2023-05-19 22:47:15.852869 stablerandom-0.6.44/stablerandom/stablerandom.py
+-rw-r--r--   0        0        0     3060 2023-05-19 22:47:15.852869 stablerandom-0.6.44/stablerandom/stablerandom_test.py
+-rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 stablerandom-0.6.44/PKG-INFO
```

### Comparing `stablerandom-0.5.40/LICENSE.txt` & `stablerandom-0.6.44/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stablerandom-0.5.40/README.md` & `stablerandom-0.6.44/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,49 @@
 stablerandom provides a stable and repeatable implementation of 
 the NumPy random number generator (numpy.random). With this package, 
 you can generate the same sequence of random numbers across different 
 platforms and Python environments, ensuring reproducibility 
 in scientific computing, machine learning, and unit testing.
 
 stablerandom can decorate any function or method and provide a 
-call-stack scoped seeded random generator. It is thread safe and 
-supports nested scopes.
+call-stack scoped seeded random generator. stablerandom can also be used
+as a Context. It is thread safe and supports nested scopes.
 
-## Example
+## Example decorator
 Using the `@stablerandom` decorator to get a stable output for numpy.random.triangular
 
- ```
+ ```python
 import numpy.random
 from stablerandom import stablerandom
 
 @stablerandom
 def random_triangular(samples):
     return numpy.random.triangular(1, 5, 10, samples)
 
 print(random_triangular(3))
->>> [1.99882862 7.95097645 7.68974243]
+>>> [5.1017943  2.64970963 8.6996913 ]
 print(random_triangular(3))
->>> [1.99882862 7.95097645 7.68974243]
+>>> [5.1017943  2.64970963 8.6996913 ]
+```
+
+## Example context
+Using the `with stablerandom` context to get a stable output:
+```python
+import numpy.random
+from stablerandom import stablerandom
+
+with stablerandom:
+    print(numpy.random.triangular(1, 5, 10, 3))
+    print(numpy.random.triangular(1, 5, 10, 3))
+>>> [5.1017943  2.64970963 8.6996913 ]
+>>> [3.30538708 2.39427919 3.57653224]
+
+with stablerandom:
+    print(numpy.random.triangular(1, 5, 10, 3))
+>>> [5.1017943  2.64970963 8.6996913 ]
 ```
 
 ## Installing
 ```bash
 $ pip install stablerandom
 ```
 The source code is currently hosted on GitHub at
```

### Comparing `stablerandom-0.5.40/stablerandom/stablerandom.py` & `stablerandom-0.6.44/stablerandom/stablerandom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # Copyright (c) 2023 John Heintz, Gist Labs https://gistlabs.com
 # License Apache v2 http://www.apache.org/licenses/
 import numpy.random
 from numpy.random import Generator, PCG64
 import threading
+from contextlib import ContextDecorator
 
 
 class RandomLocal(threading.local):
     """
     A threadlocal to hold a stack of stable random generators
     """
     stack = []
 
     def push(self):
-        """Push a new Generator PCG64 SeedSequence to the stack"""
-        self.stack.append(Generator(PCG64(123456789)))
+        """Push a new Generator PCG64 SeedSequence to the stack
+
+        What’s better decimal jokes or integer ones?
+        Decimal jokes. Integer jokes just don’t have any point.
+        https://upjoke.com/integer-jokes
+
+        The largest prime number with 9 digits is 999999937"""
+        self.stack.append(Generator(PCG64(999999937)))
 
     def pop(self):
         """Removes the top element from the stack"""
         self.stack.pop(0)
 
     def top(self) -> numpy.random.Generator:
         """Lookup the top random generator, or return None
@@ -42,34 +49,36 @@
     Return a Generator,either the current stable one or else a (random) global Generator
 
     This can be used for all cases to get random numbers, whether inside a @stablerandom or not
 
     """
     return _randomLocalStack.top() or _globalRandomGenerator
 
-
-def stablerandom(func):
+class StableRandom(ContextDecorator):
     """A decorator indicating stable random
     @stablerandom provides stable random behavior for a function and call stack
 
     Usage:
-        @stable_random
+        @stablerandom
         def my_method():
             ...
-    """
-    def wrapper(*args, **kwargs):
-        _randomLocalStack.push() # push a new stable random Generator on to the stack
 
-        try:
-            return func(*args, **kwargs) # call the function and this might make random().function calls
-        finally:
-            _randomLocalStack.pop() # clear thread local
+    A context indicating stable random
+    Usage:
+        with stablerandom:
+            ...
+    """
+    def __enter__(self):
+        _randomLocalStack.push()
+        return self
 
-    return wrapper
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        _randomLocalStack.pop()
 
+stablerandom = StableRandom()
 
 # random functions to wrap for stable,
 # from https://numpy.org/doc/stable/reference/random/legacy.html#functions-in-numpy-random
 
 
 # List of all available numpy.random functions
 _random_functions = [x for x in dir(numpy.random) if not x.startswith('_')]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stablerandom-0.5.40/stablerandom/stablerandom_test.py` & `stablerandom-0.6.44/stablerandom/stablerandom_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,34 @@
 
     @stablerandom
     def stableIsNotGlobal():
         assert _globalRandomGenerator != random()
         assert random() == _randomLocalStack.top()
     stableIsNotGlobal()
 
+def test_context_global():
+    with stablerandom:
+        assert _globalRandomGenerator != random()
+        assert random() == _randomLocalStack.top()
+
+def test_decorator_equals_context():
+    s = stable()
+
+    with stablerandom:
+        assert s == numpy.random.triangular(1, 5, 10)
+
+def test_nested_context():
+    with stablerandom:
+        a = numpy.random.triangular(1, 5, 10)
+        b = numpy.random.triangular(1, 5, 10)
+        assert a != b
+
+        with stablerandom:
+            c = numpy.random.triangular(1, 5, 10)
+            assert a == c
 
 def test_stable_randint():
     @stablerandom
     def stable_randint():
         return numpy.random.randint(8, size=1)
 
     assert stable_randint() == stable_randint()
```

