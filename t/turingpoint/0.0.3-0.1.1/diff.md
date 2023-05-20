# Comparing `tmp/turingpoint-0.0.3.tar.gz` & `tmp/turingpoint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turingpoint-0.0.3.tar", last modified: Mon Apr 24 11:56:15 2023, max compression
+gzip compressed data, was "turingpoint-0.1.1.tar", last modified: Sat May 20 18:46:18 2023, max compression
```

## Comparing `turingpoint-0.0.3.tar` & `turingpoint-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-04-24 11:56:15.292458 turingpoint-0.0.3/
--rw-r--r--   0 oren      (1000) oren      (1000)     7023 2023-04-24 11:56:15.292458 turingpoint-0.0.3/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)     6233 2023-02-25 19:46:15.000000 turingpoint-0.0.3/README.md
--rw-r--r--   0 oren      (1000) oren      (1000)      103 2023-01-21 13:37:50.000000 turingpoint-0.0.3/pyproject.toml
--rw-r--r--   0 oren      (1000) oren      (1000)     1185 2023-04-24 11:56:15.292458 turingpoint-0.0.3/setup.cfg
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-04-24 11:56:15.292458 turingpoint-0.0.3/turingpoint/
--rw-r--r--   0 oren      (1000) oren      (1000)      136 2023-04-24 11:12:09.000000 turingpoint-0.0.3/turingpoint/__init__.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1448 2023-01-21 14:08:54.000000 turingpoint-0.0.3/turingpoint/assembly.py
--rw-r--r--   0 oren      (1000) oren      (1000)      476 2023-01-20 16:18:22.000000 turingpoint-0.0.3/turingpoint/definitions.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1433 2023-04-24 11:08:57.000000 turingpoint-0.0.3/turingpoint/gymnasium_utils.py
--rw-r--r--   0 oren      (1000) oren      (1000)      435 2023-04-24 11:09:05.000000 turingpoint-0.0.3/turingpoint/sb3_utils.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1778 2023-02-10 15:09:28.000000 turingpoint-0.0.3/turingpoint/self_play.py
--rw-r--r--   0 oren      (1000) oren      (1000)      862 2023-04-24 10:31:58.000000 turingpoint-0.0.3/turingpoint/utils.py
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-04-24 11:56:15.292458 turingpoint-0.0.3/turingpoint.egg-info/
--rw-r--r--   0 oren      (1000) oren      (1000)     7023 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)      415 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/SOURCES.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/dependency_links.txt
--rw-r--r--   0 oren      (1000) oren      (1000)      146 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/requires.txt
--rw-r--r--   0 oren      (1000) oren      (1000)       12 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/top_level.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-01-21 13:51:35.000000 turingpoint-0.0.3/turingpoint.egg-info/zip-safe
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-20 18:46:18.952157 turingpoint-0.1.1/
+-rw-r--r--   0 oren      (1000) oren      (1000)     7023 2023-05-20 18:46:18.952157 turingpoint-0.1.1/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)     6233 2023-02-25 19:46:15.000000 turingpoint-0.1.1/README.md
+-rw-r--r--   0 oren      (1000) oren      (1000)      103 2023-01-21 13:37:50.000000 turingpoint-0.1.1/pyproject.toml
+-rw-r--r--   0 oren      (1000) oren      (1000)     1185 2023-05-20 18:46:18.952157 turingpoint-0.1.1/setup.cfg
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-20 18:46:18.952157 turingpoint-0.1.1/turingpoint/
+-rw-r--r--   0 oren      (1000) oren      (1000)      177 2023-05-20 16:03:17.000000 turingpoint-0.1.1/turingpoint/__init__.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1458 2023-05-17 15:41:08.000000 turingpoint-0.1.1/turingpoint/assembly.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      476 2023-01-20 16:18:22.000000 turingpoint-0.1.1/turingpoint/definitions.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1407 2023-05-17 15:41:47.000000 turingpoint-0.1.1/turingpoint/gymnasium_utils.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     2637 2023-05-20 18:01:34.000000 turingpoint-0.1.1/turingpoint/pz_utils.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      431 2023-05-20 16:04:30.000000 turingpoint-0.1.1/turingpoint/sb3_utils.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1778 2023-02-10 15:09:28.000000 turingpoint-0.1.1/turingpoint/self_play.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1058 2023-05-20 18:08:59.000000 turingpoint-0.1.1/turingpoint/utils.py
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-20 18:46:18.952157 turingpoint-0.1.1/turingpoint.egg-info/
+-rw-r--r--   0 oren      (1000) oren      (1000)     7023 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)      439 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)      146 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/requires.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)       12 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/top_level.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-01-21 13:51:35.000000 turingpoint-0.1.1/turingpoint.egg-info/zip-safe
```

### Comparing `turingpoint-0.0.3/PKG-INFO` & `turingpoint-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turingpoint
-Version: 0.0.3
+Version: 0.1.1
 Summary: Reinforcement Learning (RL) library
 Home-page: https://github.com/zbenmo/turingpoint
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 Keywords: Reinforcement Learning,Framework,Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `turingpoint-0.0.3/README.md` & `turingpoint-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `turingpoint-0.0.3/setup.cfg` & `turingpoint-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `turingpoint-0.0.3/turingpoint/assembly.py` & `turingpoint-0.1.1/turingpoint/assembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,29 @@
     pass
 
   @abstractmethod
   def participants(self) -> Generator[Participant, None, None]:
     pass
 
   def launch(self) -> dict:
-    """
-    The 'launch' function is an episode (or main) loop of the evaluation / training / playing / deploying realm.
+    """The 'launch' function is an episode (or main) loop of the evaluation / training / playing / deploying realm.
     For example if you are running multiple episodes you'll probably be calling this function multiple times as needed.
     
     The initial parcel is created with a call to 'self.create_inital_parcel()',
     which in turn shall, for example, set the initial observations.
     Next this function (launch) calls the parcipitants each at its turn.
 
     The 'self.parcipitants' generator can be based for example on a list,
     where once the end of the list is reached, the generator goes back to the start of the list.
     
     Given that the 'participants' generator is potentially infinite,
     it is the responsibility of (one or more) of the participants to close the generator.
     Closing the generator from a participant can be achieved by raising a flag or by raising an event. See examples.
 
-    The return value is the parcel as is at the end of the loop's execution.
+    Returns:
+      The return value is the parcel as is at the end of the loop's execution.
     """
     
     parcel = self.create_initial_parcel()
     for participant in self.participants():
       participant(parcel)
     return parcel
```

### Comparing `turingpoint-0.0.3/turingpoint/gymnasium_utils.py` & `turingpoint-0.1.1/turingpoint/gymnasium_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Generator, List
 from turingpoint import Assembly, Participant
 import gymnasium as gym
 
 
-class EnvironmentParticipant(Participant):
+class EnvironmentParticipant:
   def __init__(self, env: gym.Env, save_obs_as="obs"):
     self._env = env
     self._save_obs_as = save_obs_as
 
   def __call__(self, parcel: dict) -> None:
     action = parcel['action']
     obs, reward, terminated, truncated, info = self._env.step(action)
     parcel[self._save_obs_as] = obs
     parcel['reward'] = reward
     parcel['terminated'] = terminated
     parcel['truncated'] = truncated
     parcel['info'] = info
 
 
-class RenderParticipant(Participant):
+class RenderParticipant:
   def __init__(self, env: gym.Env):
     self._env = env
 
   def __call__(self, _: dict):
     self._env.render()
```

### Comparing `turingpoint-0.0.3/turingpoint/self_play.py` & `turingpoint-0.1.1/turingpoint/self_play.py`

 * *Files identical despite different names*

### Comparing `turingpoint-0.0.3/turingpoint.egg-info/PKG-INFO` & `turingpoint-0.1.1/turingpoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turingpoint
-Version: 0.0.3
+Version: 0.1.1
 Summary: Reinforcement Learning (RL) library
 Home-page: https://github.com/zbenmo/turingpoint
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 Keywords: Reinforcement Learning,Framework,Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

