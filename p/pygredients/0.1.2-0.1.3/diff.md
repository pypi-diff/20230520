# Comparing `tmp/pygredients-0.1.2.tar.gz` & `tmp/pygredients-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygredients-0.1.2.tar", last modified: Tue May  2 00:38:01 2023, max compression
+gzip compressed data, was "pygredients-0.1.3.tar", last modified: Fri May 19 22:39:09 2023, max compression
```

## Comparing `pygredients-0.1.2.tar` & `pygredients-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,45 @@
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.099979 pygredients-0.1.2/
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.098113 pygredients-0.1.2/.idea/
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      176 2023-04-16 03:27:57.000000 pygredients-0.1.2/.idea/.gitignore
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.098538 pygredients-0.1.2/.idea/inspectionProfiles/
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4819 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      174 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      185 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/misc.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      296 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/modules.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      284 2023-04-16 03:29:34.000000 pygredients-0.1.2/.idea/python-design-patterns.iml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      180 2023-05-02 00:36:11.000000 pygredients-0.1.2/.idea/vcs.xml
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1082 2023-05-01 23:27:20.000000 pygredients-0.1.2/LICENSE.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2745 2023-05-02 00:38:01.099807 pygredients-0.1.2/PKG-INFO
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2011 2023-05-02 00:37:50.000000 pygredients-0.1.2/README.md
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-01 23:37:49.000000 pygredients-0.1.2/__init__.py
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.098768 pygredients-0.1.2/__pycache__/
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2873 2023-04-18 20:41:21.000000 pygredients-0.1.2/__pycache__/node.cpython-39.pyc
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.099017 pygredients-0.1.2/_trial_temp/
--rwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-04-18 20:33:46.000000 pygredients-0.1.2/_trial_temp/_trial_marker
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     5155 2023-04-18 20:37:26.000000 pygredients-0.1.2/adapter_linkedlist.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4650 2023-04-18 20:37:26.000000 pygredients-0.1.2/adapter_queue.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4432 2023-04-18 20:37:26.000000 pygredients-0.1.2/adapter_stack.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1872 2023-04-18 20:37:26.000000 pygredients-0.1.2/node.py
-drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-02 00:38:01.099610 pygredients-0.1.2/pygredients.egg-info/
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     2745 2023-05-02 00:38:00.000000 pygredients-0.1.2/pygredients.egg-info/PKG-INFO
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      611 2023-05-02 00:38:01.000000 pygredients-0.1.2/pygredients.egg-info/SOURCES.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        1 2023-05-02 00:38:00.000000 pygredients-0.1.2/pygredients.egg-info/dependency_links.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       13 2023-05-02 00:38:00.000000 pygredients-0.1.2/pygredients.egg-info/requires.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        1 2023-05-02 00:38:00.000000 pygredients-0.1.2/pygredients.egg-info/top_level.txt
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       38 2023-05-02 00:38:01.100022 pygredients-0.1.2/setup.cfg
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      966 2023-05-02 00:37:56.000000 pygredients-0.1.2/setup.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4259 2023-04-18 20:33:05.000000 pygredients-0.1.2/test_adapter_linkedlist.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3841 2023-04-18 20:37:26.000000 pygredients-0.1.2/test_adapter_queue.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3757 2023-04-18 20:33:11.000000 pygredients-0.1.2/test_adapter_stack.py
--rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1086 2023-04-18 20:42:06.000000 pygredients-0.1.2/test_node.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.981364 pygredients-0.1.3/
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.975936 pygredients-0.1.3/.idea/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      176 2023-04-16 03:27:57.000000 pygredients-0.1.3/.idea/.gitignore
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.976590 pygredients-0.1.3/.idea/inspectionProfiles/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4819 2023-04-16 03:29:34.000000 pygredients-0.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      174 2023-04-16 03:29:34.000000 pygredients-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      185 2023-04-16 03:29:34.000000 pygredients-0.1.3/.idea/misc.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      296 2023-04-16 03:29:34.000000 pygredients-0.1.3/.idea/modules.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      284 2023-04-16 03:29:34.000000 pygredients-0.1.3/.idea/python-design-patterns.iml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      180 2023-05-02 00:36:11.000000 pygredients-0.1.3/.idea/vcs.xml
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1082 2023-05-01 23:27:20.000000 pygredients-0.1.3/LICENSE.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4375 2023-05-19 22:39:09.981213 pygredients-0.1.3/PKG-INFO
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3608 2023-05-19 22:05:36.000000 pygredients-0.1.3/README.md
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.976822 pygredients-0.1.3/_trial_temp/
+-rwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 21:26:09.000000 pygredients-0.1.3/_trial_temp/_trial_marker
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.976939 pygredients-0.1.3/pygredients/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      138 2023-05-19 22:36:27.000000 pygredients-0.1.3/pygredients/__init__.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.978173 pygredients-0.1.3/pygredients/linkedlist/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       34 2023-05-19 22:36:09.000000 pygredients-0.1.3/pygredients/linkedlist/__init__.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     5727 2023-05-19 22:17:25.000000 pygredients-0.1.3/pygredients/linkedlist/linkedlist.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4302 2023-05-19 22:19:12.000000 pygredients-0.1.3/pygredients/linkedlist/test_linkedlist.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.978859 pygredients-0.1.3/pygredients/node/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       22 2023-05-19 22:35:56.000000 pygredients-0.1.3/pygredients/node/__init__.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1872 2023-04-18 20:37:26.000000 pygredients-0.1.3/pygredients/node/node.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1151 2023-05-19 22:19:12.000000 pygredients-0.1.3/pygredients/node/test_node.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.979687 pygredients-0.1.3/pygredients/observer/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       30 2023-05-19 22:35:56.000000 pygredients-0.1.3/pygredients/observer/__init__.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3439 2023-05-19 20:40:39.000000 pygredients-0.1.3/pygredients/observer/observer.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3122 2023-05-19 22:19:12.000000 pygredients-0.1.3/pygredients/observer/test_observer.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.980366 pygredients-0.1.3/pygredients/queue/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       24 2023-05-19 22:35:38.000000 pygredients-0.1.3/pygredients/queue/__init__.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     5294 2023-05-19 22:17:25.000000 pygredients-0.1.3/pygredients/queue/queue.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3884 2023-05-19 22:34:47.000000 pygredients-0.1.3/pygredients/queue/test_queue.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.980866 pygredients-0.1.3/pygredients/stack/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       24 2023-05-19 22:35:56.000000 pygredients-0.1.3/pygredients/stack/__init__.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     5070 2023-05-19 22:18:05.000000 pygredients-0.1.3/pygredients/stack/stack.py
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     3807 2023-05-19 22:19:12.000000 pygredients-0.1.3/pygredients/stack/test_stack.py
+drwxr-xr-x   0 francoisboulay-handfield   (501) staff       (20)        0 2023-05-19 22:39:09.977626 pygredients-0.1.3/pygredients.egg-info/
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     4375 2023-05-19 22:39:09.000000 pygredients-0.1.3/pygredients.egg-info/PKG-INFO
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)      923 2023-05-19 22:39:09.000000 pygredients-0.1.3/pygredients.egg-info/SOURCES.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)        1 2023-05-19 22:39:09.000000 pygredients-0.1.3/pygredients.egg-info/dependency_links.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       13 2023-05-19 22:39:09.000000 pygredients-0.1.3/pygredients.egg-info/requires.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       12 2023-05-19 22:39:09.000000 pygredients-0.1.3/pygredients.egg-info/top_level.txt
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)       38 2023-05-19 22:39:09.981425 pygredients-0.1.3/setup.cfg
+-rw-r--r--   0 francoisboulay-handfield   (501) staff       (20)     1029 2023-05-19 22:06:45.000000 pygredients-0.1.3/setup.py
```

### Comparing `pygredients-0.1.2/.idea/inspectionProfiles/Project_Default.xml` & `pygredients-0.1.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.2/LICENSE.txt` & `pygredients-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.2/PKG-INFO` & `pygredients-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,178 @@
-Metadata-Version: 2.1
-Name: pygredients
-Version: 0.1.2
-Summary: Pygredients is an open-source Python library for data structures and algorithms available on PyPi.
-Home-page: https://github.com/FBH514/pygredients
-Author: François Boulay-Handfield
-Author-email: fbhworks@icloud.com
-License: MIT
-Keywords: data structures algorithms
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Pygredients
 
-Version 0.1.2
+Version 0.1.3
 
-Pygredients is an open-source Python library for data structures and algorithms available on PyPi. 🍎🍊🍋🫐
+Pygredients is an open-source Python library for data structures, algorithms and design patterns available on PyPi. 🍎🍊🍋🫐
 
 ## Installation
-```pip install pygredients```
 
-```pip3 install pygredients``` for OSX users
+You can install Pygredients using pip:
+
+```
+pip install pygredients
+```
+
+For macOS users, please use the following command:
+
+```
+pip3 install pygredients
+```
 
 ## Usage
+
+To use Pygredients in your Python code, import it as follows:
+
 ```python
-from pygredients import *
+import pygredients
 ```
 
-## Data Structures
-### Linked List
+# Data Structures
+
+## Linked List
+
+You can create a linked list, add nodes to it, remove nodes from it, and perform other operations using the `LinkedList` class.
+
 ```python
 # Create a linked list
 ll = LinkedList()
 
 # Add a node to the linked list
 ll.append(1)
 ll.append(2)
 ll.append(3)
 
 # Remove a node from the linked list
-ll.remove(2) # 2
+ll.remove(2)  # 2
 
 # Check if a value is in the linked list
-ll.contains(1) # True
+ll.contains(1)  # True
 
 # Get the head of the linked list
-ll.peek() # 3
+ll.peek()  # 3
 
 # Get the length of the linked list
-ll.size() # 2
+ll.size()  # 2
 
 # Check if the linked list is empty
-ll.is_empty() # False
+ll.is_empty()  # False
 
 # Print the linked list
-print(ll) # [1, 3]
+print(ll)  # [1, 3]
 
 # Limit the length of the linked list
 ll.limit = 2
-ll.append(4) # ValueError: Cannot append 4 to Linked List as it is full.
+ll.append(4)  # ValueError: Cannot append 4 to Linked List as it is full.
 ```
 
-### Stack
+## Stack
+
+You can create a stack, push values onto it, pop values from it, and perform other operations using the `Stack` class.
+
 ```python
 # Create a stack
 stack = Stack()
 
 # Push a value to the stack
 stack.push(1)
 stack.push(2)
 stack.push(3)
 
 # Pop a value from the stack
-stack.pop() # 3
+stack.pop()  # 3
 
 # Peek the top of the stack
-stack.peek() # 2
+stack.peek()  # 2
 
 # Check if a value is in the stack
-stack.contains(1) # True
+stack.contains(1)  # True
 
 # Get the length of the stack
-stack.size() # 2
+stack.size()  # 2
 
 # Check if the stack is empty
-stack.is_empty() # False
+stack.is_empty()  # False
 
 # Print the stack
-print(stack) # [1, 2]
+print(stack)  # [1, 2]
 
 # Limit the length of the stack
 stack.limit = 2
-stack.push(4) # ValueError: Cannot push 4 to Stack as it is full.
+stack.push(4)  # ValueError: Cannot push 4 to Stack as it is full.
 ```
 
-### Queue
+## Queue
+
+You can create a queue, enqueue values into it, dequeue values from it, and perform other operations using the `Queue` class.
+
 ```python
 # Create a queue
 queue = Queue()
 
 # Enqueue a value to the queue
 queue.enqueue(1)
 queue.enqueue(2)
 queue.enqueue(3)
 
 # Dequeue a value from the queue
-queue.dequeue() # 1
+queue.dequeue()  # 1
 
 # Peek the front of the queue
-queue.peek() # 2
+queue.peek()  # 2
 
 # Check if a value is in the queue
-queue.contains(1) # True
+queue.contains(1)  # True
 
 # Get the length of the queue
-queue.size() # 2
+queue.size()  # 2
 
 # Check if the queue is empty
-queue.is_empty() # False
+queue.is_empty()  # False
 
 # Print the queue
-print(queue) # [2, 3]
+print(queue)  # [2, 3]
 
 # Limit the length of the queue
-queue.limit = 2 
-queue.enqueue(4) # ValueError: Cannot enqueue 4 to Queue as it is full.
+queue.limit = 2
+queue.enqueue(4)  # ValueError: Cannot enqueue 4 to Queue as it is full.
 ```
 
+# Design Patterns
+
+## Observer
+
+The Observer pattern is implemented in Pygredients using the`Observer` and `Observable` classes. Here's an example usage:
+
+```python
+from pygredients.observer.observer import Observer, Observable
+
+
+class WeatherStation(Observable):
+    pass
+
+
+class DisplayDevice(Observer):
+    def __init__(self, name):
+        super().__init__(name)
+        self.temperature = None
+
+    def notify(self, *args, **kwargs):
+        self.temperature = kwargs.get('temperature')
+        print(f'{self.name} now displays the temperature: {self.temperature}°C')
+
+
+# Initialize a WeatherStation and two DisplayDevices
+station = WeatherStation()
+device1 = DisplayDevice("Device1")
+device2 = DisplayDevice("Device2")
+
+# Register the DisplayDevices with the WeatherStation
+station.register_observers(device1)
+station.register_observers(device2)
+
+# Update the state of the WeatherStation
+station.state = {'temperature': 20}
+
+# Unsubscribe device1 and update the state again
+device1.unsubscribe()
+station.state = {'temperature': 22}
+```
```

### Comparing `pygredients-0.1.2/adapter_linkedlist.py` & `pygredients-0.1.3/pygredients/queue/queue.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,141 @@
-from node import Node
+from pygredients.node.node import Node
 from typing import Any
-from abc import abstractmethod, ABC
 
-
-class AdapterLinkedListInterface(ABC):
-    """Defines the interface for the Linked List data structure."""
-
-    @abstractmethod
-    def __init__(self, limit=None) -> None:
-        pass
-
-    @abstractmethod
-    def __str__(self) -> str:
-        pass
-
-    @abstractmethod
-    def __repr__(self) -> str:
-        pass
-
-    @abstractmethod
-    def append(self, data: Any) -> None:
-        pass
-
-    @abstractmethod
-    def remove(self, data: Any) -> Any:
-        pass
-
-    @abstractmethod
-    def peek(self) -> Any:
-        pass
-
-    @abstractmethod
-    def contains(self, data: Any) -> bool:
-        pass
-
-    @abstractmethod
-    def size(self) -> int:
-        pass
-
-    @abstractmethod
-    def is_empty(self) -> bool:
-        pass
-
-
-class AdapterLinkedList(AdapterLinkedListInterface):
+class Queue:
     """
-    Defines a Linked List data structure.
-    Contracted by the Linked List interface.
+    This class represents a Queue data structure, implemented as a singly linked list of Node objects.
+    The queue has a size property, which keeps track of the number of nodes in the list,
+    and a limit property, which sets the maximum number of nodes allowed in the list.
+    The queue supports standard queue operations like enqueue (i.e., add to the end),
+    dequeue (i.e., remove from the front), peeking, and checking whether a particular value exists in the list.
     """
 
     def __init__(self, limit=None) -> None:
         """
-        Constructor for the Linked List data structure.
-        :param limit: int
-        """
-        if not limit: self._limit = float("inf")
-        else: self._limit = limit
+        Constructs a new queue.
+        If a limit is not provided, the queue will have no fixed size limit.
+        :param limit: The maximum number of nodes allowed in the queue.
+                      Defaults to None, in which case the queue can grow indefinitely.
+        """
+        if not limit:
+            self._limit = float("inf")
+        else:
+            self._limit = limit
         self._size: int = 0
         self.head = None
 
     def __str__(self) -> str:
         """
-        Returns a string representation of the Linked List data structure to display.
+        Returns a string representation of the queue, detailing its size and the items it contains.
         :return: str
         """
         data = []
         current = self.head
         while current is not None:
             data.append(current.data)
             current = current.next
-        return "Linked List has a size of {} and contains the following items:\n{}".format(self._size, data)
-
-    def __repr__(self) -> str:
-        """
-        Returns a string representation of the Linked List data structure to debug.
-        :return: str
-        """
-        return "LinkedList({})".format(self._size)
+        return "Queue has a size of {} and contains the following items:\n{}".format(self._size, data)
 
     @property
     def limit(self) -> int:
         """
-        Returns the limit of the Linked List data structure.
-        :return: int
+        Getter for the limit of the queue.
+        The limit represents the maximum number of nodes that can be stored in the queue.
+        :return: The maximum number of nodes allowed in the queue.
         """
         return self._limit
 
     @limit.setter
     def limit(self, value: int) -> None:
         """
-        Sets the limit of the Linked List data structure.
-        :param value: int
-        :return: None
+        Setter for the limit of the queue.
+        The new limit must be a positive integer and greater than or equal to the current size of the queue.
+        :param value: The new maximum number of nodes allowed in the queue.
         """
         if not value > 0:
             raise ValueError("Cannot set the limit to {} as it is not a valid value.".format(value))
         elif value < self._size:
-            raise ValueError("Cannot set the limit to {} as it is smaller than the current size of the Linked List.".format(value))
+            raise ValueError(
+                "Cannot set the limit to {} as it is smaller than the current size of the queue.".format(value))
         self._limit = value
 
-    def append(self, data: Any) -> None:
+    def __repr__(self) -> str:
         """
-        Appends the data to the Linked List data structure.
-        :param data: Any
-        :return: None
+        Returns a technical string representation of the queue, useful for debugging.
+        :return: str
+        """
+        return "Queue({})".format(self._size)
+
+    def enqueue(self, data: Any) -> None:
+        """
+        Adds a new node with the provided data to the end of the queue.
+        If the queue has reached its size limit, an IndexError is raised.
+        :param data: The data to be stored in the new node. Must not be None.
         """
         if data is None:
-            raise ValueError("Cannot append {} to the Linked List.".format(data))
+            raise ValueError("Cannot enqueue {} in the Queue.".format(data))
         if self._size == self._limit:
-            raise IndexError("Cannot append {} to Linked List as it is full.".format(data))
-        self.head = Node(data, self.head)
+            raise IndexError("Cannot append {} to the Queue as it is full.".format(data))
+        if self.head is None:
+            self.head = Node(data)
+        else:
+            current = self.head
+            while current.next is not None:
+                current = current.next
+            current.next = Node(data)
         self._size += 1
 
-    def remove(self, data: Any) -> Any:
+    def dequeue(self) -> Any:
         """
-        Removes and returns the data from the Linked List data structure.
-        :param data: Any
-        :return: Any
+        Removes the node at the front of the queue and returns its data.
+        If the queue is empty, an IndexError is raised.
+        :return: The data of the dequeued node.
         """
         if self.is_empty():
-            raise IndexError("Cannot remove {} from an empty Linked List.".format(data))
-        if data is None:
-            raise ValueError("Cannot remove {} from the Linked List.".format(data))
+            raise IndexError("Cannot dequeue an empty Queue.")
         current = self.head
-        previous = None
-        while current is not None:
-            if data == current.data:
-                if previous is not None:
-                    previous.next = current.next
-                else:
-                    self.head = current.next
-                self._size -= 1
-                return current.data
-            previous = current
-            current = current.next
-        raise ValueError("Cannot remove {} from Linked List as it does not exist.".format(data))
+        self.head = current.next
+        self._size -= 1
+        return current.data
 
     def peek(self) -> Any:
         """
-        Returns the first item in the Linked List data structure.
-        :return: Any
+        Returns the data of the node at the front of the queue.
+        If the queue is empty, an IndexError is raised.
+        :return: The data of the front node.
         """
         if self.is_empty():
-            raise IndexError("Cannot peek an empty Linked List.")
+            raise IndexError("Cannot peek an empty Queue.")
         return self.head.data
 
     def contains(self, data: Any) -> bool:
         """
-        Returns whether the Linked List data structure contains the data.
-        :param data: Any
-        :return: bool
+        Checks if the provided data exists in any node in the queue.
+        If the queue is empty, an IndexError is raised.
+        :param data: The data to search for in the queue.
+        :return: True if the data exists in the queue, False otherwise.
         """
         if self.is_empty():
-            raise IndexError("Cannot search an empty Linked List.")
+            raise IndexError("Cannot search an empty Queue.")
         if data is None:
-            raise ValueError("Cannot search for {} in the Linked List.".format(data))
+            raise ValueError("Cannot search for {} in the Queue.".format(data))
         current = self.head
         while current is not None:
             if data == current.data:
                 return True
             current = current.next
         return False
 
     def size(self) -> int:
         """
-        Returns the size of the Linked List data structure.
-        :return: int
+        Returns the current number of nodes in the queue.
+        :return: the size of the queue.
         """
         return self._size
 
     def is_empty(self) -> bool:
         """
-        Returns whether the Linked List data structure is empty.
-        :return: bool
+        Checks if the queue is currently empty (i.e., contains no nodes).
+        :return: True if the queue is empty, False otherwise.
         """
         return self._size == 0
```

### Comparing `pygredients-0.1.2/node.py` & `pygredients-0.1.3/pygredients/node/node.py`

 * *Files identical despite different names*

### Comparing `pygredients-0.1.2/setup.py` & `pygredients-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pygredients',
-    version='0.1.2',
-    description='Pygredients is an open-source Python library for data structures and algorithms available on PyPi.',
+    version='0.1.3',
+    description='Pygredients is an open-source Python library for data structures, algorithms and design patterns available on PyPi.',
     long_description=f"{long_description}",
     long_description_content_type="text/markdown",
     author='François Boulay-Handfield',
     author_email="fbhworks@icloud.com",
     url="https://github.com/FBH514/pygredients",
     license="MIT",
+    packages=find_packages(),
     install_requires=[
         "twine>=4.0.0",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
     ],
-    keywords="data structures algorithms",
+    keywords="data structures algorithms design patterns",
     python_requires=">=3.9"
 )
```

### Comparing `pygredients-0.1.2/test_adapter_linkedlist.py` & `pygredients-0.1.3/pygredients/linkedlist/test_linkedlist.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import unittest
 from unittest import TestCase
-from adapter_linkedlist import AdapterLinkedList as LinkedList
+from linkedlist import LinkedList as LinkedList
 
 
-class TestAdapterLinkedList(TestCase):
+class TestLinkedList(TestCase):
     """Tests the Linked List data structure."""
 
     def setUp(self) -> None:
         """
         Sets up the test suite.
         :return: None
         """
@@ -110,7 +111,11 @@
         self.assertFalse(self.linked_list.is_empty())
         self.linked_list.remove(5)
         self.linked_list.remove(4)
         self.linked_list.remove(3)
         self.linked_list.remove(2)
         self.linked_list.remove(1)
         self.assertTrue(self.linked_list.is_empty())
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `pygredients-0.1.2/test_adapter_queue.py` & `pygredients-0.1.3/pygredients/queue/test_queue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import unittest
 from unittest import TestCase
-from adapter_queue import AdapterQueue as Queue
+from queue import Queue as Queue
 
 
-class TestAdapterQueue(TestCase):
+class TestQueue(TestCase):
     """Tests the Queue data structure."""
 
     def setUp(self) -> None:
         """
         Sets up the test suite.
         :return: None
         """
@@ -110,7 +111,11 @@
         self.assertFalse(self.queue.is_empty())
         self.queue.dequeue()
         self.queue.dequeue()
         self.queue.dequeue()
         self.queue.dequeue()
         self.queue.dequeue()
         self.assertTrue(self.queue.is_empty())
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `pygredients-0.1.2/test_adapter_stack.py` & `pygredients-0.1.3/pygredients/stack/test_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import unittest
 from unittest import TestCase
-from adapter_stack import AdapterStack as Stack
+from stack import Stack as Stack
 
 
 class TestStack(TestCase):
     """Tests the Stack data structure."""
 
     def setUp(self) -> None:
         """
@@ -109,7 +110,11 @@
         Tests the is_empty method of the Stack data structure.
         :return: None
         """
         self.assertFalse(self.stack.is_empty())
         for _ in range(5):
             self.stack.pop()
         self.assertTrue(self.stack.is_empty())
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `pygredients-0.1.2/test_node.py` & `pygredients-0.1.3/pygredients/node/test_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import unittest
 from unittest import TestCase
 from node import Node
 
 
 class TestNode(TestCase):
     """Tests the Node data structure."""
 
@@ -34,7 +35,11 @@
     def test_next(self) -> None:
         """
         Tests the next property of the Node data structure.
         :return: None
         """
         self.assertTrue(self.one.next is None)
         self.assertTrue(self.two.next is self.one)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

