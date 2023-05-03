# Comparing `tmp/eagerx-0.1.8.tar.gz` & `tmp/eagerx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagerx-0.1.8.tar", max compression
+gzip compressed data, was "eagerx-0.1.9.tar", max compression
```

## Comparing `eagerx-0.1.8.tar` & `eagerx-0.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      373 2022-03-14 13:34:21.107688 eagerx-0.1.8/eagerx/__init__.py
--rw-r--r--   0        0        0        0 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/__init__.py
--rw-r--r--   0        0        0      348 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/openai_gym/__init__.py
--rw-r--r--   0        0        0     2684 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/openai_gym/bridge.py
--rw-r--r--   0        0        0     1951 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/openai_gym/converters.py
--rw-r--r--   0        0        0    12912 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/openai_gym/enginenodes.py
--rw-r--r--   0        0        0     3966 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/openai_gym/env.py
--rw-r--r--   0        0        0     5037 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/openai_gym/objects.py
--rw-r--r--   0        0        0        0 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/openai_gym/simstates.py
--rw-r--r--   0        0        0      250 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/test/__init__.py
--rw-r--r--   0        0        0     3843 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/test/bridge.py
--rw-r--r--   0        0        0     3963 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/test/converters.py
--rw-r--r--   0        0        0      686 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/test/enginestates.py
--rw-r--r--   0        0        0    13479 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/test/nodes.py
--rw-r--r--   0        0        0    15332 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/bridges/test/objects.py
--rw-r--r--   0        0        0      113 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/converters/__init__.py
--rw-r--r--   0        0        0     1001 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/converters/ros_processor.py
--rw-r--r--   0        0        0     5203 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/converters/space_ros_converters.py
--rw-r--r--   0        0        0      350 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/__init__.py
--rw-r--r--   0        0        0     3001 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/constants.py
--rw-r--r--   0        0        0      563 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/converters.py
--rw-r--r--   0        0        0    43453 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/entities.py
--rw-r--r--   0        0        0    20031 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/env.py
--rwxr-xr-x   0        0        0     5597 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/executable_bridge.py
--rwxr-xr-x   0        0        0     5965 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/executable_node.py
--rw-r--r--   0        0        0    56678 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/graph.py
--rw-r--r--   0        0        0    40499 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/graph_engine.py
--rw-r--r--   0        0        0    10670 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/nodes.py
--rw-r--r--   0        0        0     9212 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/register.py
--rw-r--r--   0        0        0    22542 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/rx_message_broker.py
--rw-r--r--   0        0        0    45105 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/rx_operators.py
--rw-r--r--   0        0        0    34068 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/rx_pipelines.py
--rw-r--r--   0        0        0    31356 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/specs.py
--rw-r--r--   0        0        0     8753 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/supervisor.py
--rw-r--r--   0        0        0     9496 2022-03-14 13:34:11.799640 eagerx-0.1.8/eagerx/core/view.py
--rw-r--r--   0        0        0        0 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/enginestates/__init__.py
--rw-r--r--   0        0        0       46 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/enginestates/enginestates.py
--rw-r--r--   0        0        0       53 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/nodes/__init__.py
--rw-r--r--   0        0        0     3258 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/nodes/butterworth_filter.py
--rw-r--r--   0        0        0        0 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/utils/__init__.py
--rw-r--r--   0        0        0     6658 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/utils/network_utils.py
--rw-r--r--   0        0        0     5627 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/utils/node_utils.py
--rw-r--r--   0        0        0    15279 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/utils/utils.py
--rw-r--r--   0        0        0       58 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/wrappers/__init__.py
--rw-r--r--   0        0        0      809 2022-03-14 13:34:11.803640 eagerx-0.1.8/eagerx/wrappers/flatten.py
--rw-r--r--   0        0        0     1260 2022-03-14 13:34:21.107688 eagerx-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1287 2022-03-14 13:34:28.022013 eagerx-0.1.8/setup.py
--rw-r--r--   0        0        0     1370 2022-03-14 13:34:28.022321 eagerx-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      373 2022-03-16 13:23:00.371468 eagerx-0.1.9/eagerx/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/__init__.py
+-rw-r--r--   0        0        0      348 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/openai_gym/__init__.py
+-rw-r--r--   0        0        0     2684 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/openai_gym/bridge.py
+-rw-r--r--   0        0        0     1951 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/openai_gym/converters.py
+-rw-r--r--   0        0        0    12867 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/openai_gym/enginenodes.py
+-rw-r--r--   0        0        0     3966 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/openai_gym/env.py
+-rw-r--r--   0        0        0     4914 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/openai_gym/objects.py
+-rw-r--r--   0        0        0        0 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/openai_gym/simstates.py
+-rw-r--r--   0        0        0      250 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/test/__init__.py
+-rw-r--r--   0        0        0     3843 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/test/bridge.py
+-rw-r--r--   0        0        0     3963 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/test/converters.py
+-rw-r--r--   0        0        0      686 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/test/enginestates.py
+-rw-r--r--   0        0        0    13479 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/test/nodes.py
+-rw-r--r--   0        0        0    15332 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/bridges/test/objects.py
+-rw-r--r--   0        0        0      113 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/converters/__init__.py
+-rw-r--r--   0        0        0     1001 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/converters/ros_processor.py
+-rw-r--r--   0        0        0     5203 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/converters/space_ros_converters.py
+-rw-r--r--   0        0        0      350 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/__init__.py
+-rw-r--r--   0        0        0     3001 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/constants.py
+-rw-r--r--   0        0        0      563 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/converters.py
+-rw-r--r--   0        0        0    61323 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/entities.py
+-rw-r--r--   0        0        0    20031 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/env.py
+-rwxr-xr-x   0        0        0     5597 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/executable_bridge.py
+-rwxr-xr-x   0        0        0     5965 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/executable_node.py
+-rw-r--r--   0        0        0    56678 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/graph.py
+-rw-r--r--   0        0        0    40469 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/graph_engine.py
+-rw-r--r--   0        0        0    10670 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/nodes.py
+-rw-r--r--   0        0        0     9212 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/register.py
+-rw-r--r--   0        0        0    22542 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/rx_message_broker.py
+-rw-r--r--   0        0        0    45105 2022-03-16 13:22:50.743406 eagerx-0.1.9/eagerx/core/rx_operators.py
+-rw-r--r--   0        0        0    34068 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/core/rx_pipelines.py
+-rw-r--r--   0        0        0    30494 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/core/specs.py
+-rw-r--r--   0        0        0     8753 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/core/supervisor.py
+-rw-r--r--   0        0        0     9496 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/core/view.py
+-rw-r--r--   0        0        0        0 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/enginestates/__init__.py
+-rw-r--r--   0        0        0       46 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/enginestates/enginestates.py
+-rw-r--r--   0        0        0       53 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/nodes/__init__.py
+-rw-r--r--   0        0        0     3258 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/nodes/butterworth_filter.py
+-rw-r--r--   0        0        0        0 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/utils/__init__.py
+-rw-r--r--   0        0        0     6658 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/utils/network_utils.py
+-rw-r--r--   0        0        0     5627 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/utils/node_utils.py
+-rw-r--r--   0        0        0    15279 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/utils/utils.py
+-rw-r--r--   0        0        0       58 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/wrappers/__init__.py
+-rw-r--r--   0        0        0      809 2022-03-16 13:22:50.747406 eagerx-0.1.9/eagerx/wrappers/flatten.py
+-rw-r--r--   0        0        0     1276 2022-03-16 13:23:00.371468 eagerx-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1308 2022-03-16 13:23:07.875427 eagerx-0.1.9/setup.py
+-rw-r--r--   0        0        0     1405 2022-03-16 13:23:07.876113 eagerx-0.1.9/PKG-INFO
```

### Comparing `eagerx-0.1.8/eagerx/bridges/openai_gym/bridge.py` & `eagerx-0.1.9/eagerx/bridges/openai_gym/bridge.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/bridges/openai_gym/converters.py` & `eagerx-0.1.9/eagerx/bridges/openai_gym/converters.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/bridges/openai_gym/enginenodes.py` & `eagerx-0.1.9/eagerx/bridges/openai_gym/enginenodes.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         spec.config.outputs = outputs if outputs else ["observation"]
 
     def initialize(self):
         # We will probably use self.simulator[self.obj_name] in callback & reset.
         assert (
             self.process == process.BRIDGE
         ), "Simulation node requires a reference to the simulator, hence it must be launched in the Bridge process"
-        self.id = self.bridge_params["env_id"]
-        self.obj_name = self.agnostic_params["name"]
+        self.id = self.bridge_config["env_id"]
+        self.obj_name = self.config["name"]
         self.last_obs = None
 
     @register.states()
     def reset(self):
         self.last_obs = None
 
     @register.inputs(tick=UInt64)
@@ -93,16 +93,16 @@
         spec.config.outputs = outputs if outputs else ["reward"]
 
     def initialize(self):
         # We will probably use self.simulator[self.obj_name] in callback & reset.
         assert (
             self.process == process.BRIDGE
         ), "Simulation node requires a reference to the simulator, hence it must be launched in the Bridge process"
-        self.id = self.bridge_params["env_id"]
-        self.obj_name = self.agnostic_params["name"]
+        self.id = self.bridge_config["env_id"]
+        self.obj_name = self.config["name"]
         self.last_reward = None
 
     @register.states()
     def reset(self):
         self.last_reward = 0.0
 
     @register.inputs(tick=UInt64)
@@ -146,16 +146,16 @@
         spec.config.outputs = outputs if outputs else ["done"]
 
     def initialize(self):
         # We will probably use self.simulator[self.obj_name] in callback & reset.
         assert (
             self.process == process.BRIDGE
         ), "Simulation node requires a reference to the simulator, hence it must be launched in the Bridge process"
-        self.id = self.bridge_params["env_id"]
-        self.obj_name = self.agnostic_params["name"]
+        self.id = self.bridge_config["env_id"]
+        self.obj_name = self.config["name"]
         self.last_done = None
 
     @register.states()
     def reset(self):
         self.last_done = False
 
     @register.inputs(tick=UInt64)
@@ -203,15 +203,15 @@
         spec.config.zero_action = zero_action
 
     def initialize(self, zero_action):
         # We will probably use self.simulator[self.obj_name] in callback & reset.
         assert (
             self.process == process.BRIDGE
         ), "Simulation node requires a reference to the simulator, hence it must be launched in the Bridge process"
-        self.obj_name = self.agnostic_params["name"]
+        self.obj_name = self.config["name"]
         self.simulator[self.obj_name]["env"]: gym.Env
         self.is_discrete = (
             True if isinstance(self.simulator[self.obj_name]["env"].action_space, gym.spaces.Discrete) else False
         )
         if zero_action is None:
             self.zero_action = self.simulator[self.obj_name]["env"].action_space.sample()
         else:
@@ -290,16 +290,16 @@
         # We will probably use self.simulator[self.obj_name] in callback & reset.
         assert (
             self.process == process.BRIDGE
         ), "Simulation node requires a reference to the simulator, hence it must be launched in the Bridge process"
         self.shape = tuple(shape)
         self.always_render = always_render
         self.render_toggle = False
-        self.id = self.bridge_params["env_id"]
-        self.obj_name = self.agnostic_params["name"]
+        self.id = self.bridge_config["env_id"]
+        self.obj_name = self.config["name"]
         self.render_toggle_pub = rospy.Subscriber("%s/env/render/toggle" % self.ns, Bool, self._set_render_toggle)
 
     @register.states()
     def reset(self):
         # This sensor is stateless (in contrast to e.g. a Kalman filter).
         pass
```

### Comparing `eagerx-0.1.8/eagerx/bridges/openai_gym/env.py` & `eagerx-0.1.9/eagerx/bridges/openai_gym/env.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/bridges/openai_gym/objects.py` & `eagerx-0.1.9/eagerx/bridges/openai_gym/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,20 @@
     def agnostic(spec: ObjectSpec, rate):
         """Agnostic definition of the GymObject"""
         # Register standard converters, space_converters, and processors
         import eagerx.converters  # noqa # pylint: disable=unused-import
 
         # Set observation space_converters
         spec.sensors.observation.space_converter = SpaceConverter.make(
-            "GymSpace_Float32MultiArray",
-            gym_id=spec.config.env_id,
-            space="observation",
+            "GymSpace_Float32MultiArray", gym_id=spec.config.env_id, space="observation"
         )
         spec.sensors.reward.space_converter = SpaceConverter.make("Space_Float32", low=-99999, high=9999, dtype="float32")
         spec.sensors.done.space_converter = SpaceConverter.make("Space_Bool")
         spec.sensors.image.space_converter = SpaceConverter.make(
-            "Space_Image",
-            low=0,
-            high=1,
-            shape=spec.config.render_shape,
-            dtype="float32",
+            "Space_Image", low=0, high=1, shape=spec.config.render_shape, dtype="float32"
         )
         spec.actuators.action.space_converter = SpaceConverter.make(
             "GymSpace_Float32MultiArray", gym_id=spec.config.env_id, space="action"
         )
 
         # Set observation rates
         spec.sensors.observation.rate = rate
@@ -101,19 +95,15 @@
             rate=spec.sensors.image.rate,
             process=2,
         )
 
         # Create actuator engine nodes
         # Rate=None, because we will connect it to an actuator (thus uses the rate set in the agnostic specification)
         action = EngineNode.make(
-            "ActionActuator",
-            "action",
-            rate=spec.actuators.action.rate,
-            process=2,
-            zero_action=spec.config.default_action,
+            "ActionActuator", "action", rate=spec.actuators.action.rate, process=2, zero_action=spec.config.default_action
         )
 
         # Connect all engine nodes
         graph.add([obs, rwd, done, image, action])
         graph.connect(source=obs.outputs.observation, sensor="observation")
         graph.connect(source=rwd.outputs.reward, sensor="reward")
         graph.connect(source=done.outputs.done, sensor="done")
```

### Comparing `eagerx-0.1.8/eagerx/bridges/test/bridge.py` & `eagerx-0.1.9/eagerx/bridges/test/bridge.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/bridges/test/converters.py` & `eagerx-0.1.9/eagerx/bridges/test/converters.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/bridges/test/enginestates.py` & `eagerx-0.1.9/eagerx/bridges/test/enginestates.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/bridges/test/nodes.py` & `eagerx-0.1.9/eagerx/bridges/test/nodes.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/bridges/test/objects.py` & `eagerx-0.1.9/eagerx/bridges/test/objects.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/converters/ros_processor.py` & `eagerx-0.1.9/eagerx/converters/ros_processor.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/converters/space_ros_converters.py` & `eagerx-0.1.9/eagerx/converters/space_ros_converters.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/constants.py` & `eagerx-0.1.9/eagerx/core/constants.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/converters.py` & `eagerx-0.1.9/eagerx/core/converters.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/env.py` & `eagerx-0.1.9/eagerx/core/env.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/executable_bridge.py` & `eagerx-0.1.9/eagerx/core/executable_bridge.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/executable_node.py` & `eagerx-0.1.9/eagerx/core/executable_node.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/graph.py` & `eagerx-0.1.9/eagerx/core/graph.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/graph_engine.py` & `eagerx-0.1.9/eagerx/core/graph_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     episode_graph,
     plot_graph,
     color_nodes,
     color_edges,
     is_stale,
 )
 from eagerx.core.graph import merge
-from eagerx.core.specs import EngineNodeSpec, ConverterSpec, EntitySpec
+from eagerx.core.specs import NodeSpec, ConverterSpec, EntitySpec
 from eagerx.core.view import GraphView
 
 yaml.Dumper.ignore_aliases = lambda *args: True
 
 
 class EngineGraph:
     def __init__(self, state: Dict):
@@ -78,15 +78,15 @@
 
         # Create a state
         state = dict(nodes=dict(), connects=list(), backup=dict())
         graph = cls(state)
         graph.add(nodes)
         return graph
 
-    def add(self, nodes: Union[EngineNodeSpec, List[EngineNodeSpec]]):
+    def add(self, nodes: Union[NodeSpec, List[NodeSpec]]):
         """
         Add a node/object to the provided state.
         """
         if not isinstance(nodes, list):
             nodes = [nodes]
 
         for node in nodes:
@@ -600,25 +600,25 @@
                 # sensors[target_cname] = entry
                 sensors[target_cname].append(entry)
                 continue  # we continue here, because the address for actuators is determined by an output from the agnostic graph.
             state["nodes"][target_name][target_comp][target_cname]["address"] = address
 
         # Initialize param objects
         nodes = dict()
-        from eagerx.core.specs import EngineNodeSpec
+        from eagerx.core.specs import NodeSpec
 
         for name, params in state["nodes"].items():
             if "node_type" in params:
                 if name == "actuators":
                     pass
                 elif name == "sensors":
                     pass
                 else:
                     # Put node name into object namespace
-                    spec = EngineNodeSpec(params)
+                    spec = NodeSpec(params)
                     name = f"$(ns obj_name)/{spec.config.name}"
                     spec.config.name = name
                     params = spec.params
 
                     # Substitute placeholder args of simnode
                     context = {"ns": {"node_name": name}, "config": params["config"]}
                     substitute_args(params, context, only=["config", "ns"])
```

### Comparing `eagerx-0.1.8/eagerx/core/nodes.py` & `eagerx-0.1.9/eagerx/core/nodes.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/register.py` & `eagerx-0.1.9/eagerx/core/register.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/rx_message_broker.py` & `eagerx-0.1.9/eagerx/core/rx_message_broker.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/rx_operators.py` & `eagerx-0.1.9/eagerx/core/rx_operators.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/rx_pipelines.py` & `eagerx-0.1.9/eagerx/core/rx_pipelines.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/specs.py` & `eagerx-0.1.9/eagerx/core/specs.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,18 +366,14 @@
         return replace_None(node_params)
 
 
 class NodeSpec(BaseNodeSpec):
     pass
 
 
-class EngineNodeSpec(BaseNodeSpec):
-    pass
-
-
 class ResetNodeSpec(BaseNodeSpec):
     @property
     def targets(self):
         return self._lookup("targets")
 
     @property
     def feedthroughs(self):
@@ -650,55 +646,18 @@
             try:
                 obj_params.pop(component)
             except KeyError:
                 pass
 
         # Add states
         obj_params["states"] = [s.build(ns) for s in states]
-        nodes = [EngineNodeSpec(params) for name, params in nodes.items() if name in dependencies]
+        nodes = [NodeSpec(params) for name, params in nodes.items() if name in dependencies]
         return {name: replace_None(obj_params)}, nodes
 
 
-class AgnosticSpec(EntitySpec):
-    def __init__(self, params):
-        params["sensors"] = dict()
-        params["actuators"] = dict()
-        params["states"] = dict()
-        super().__init__(params)
-
-    def _lookup(self, depth):
-        return SpecView(self, depth=[depth])
-
-    @property
-    def sensors(self):
-        return self._lookup("sensors")
-
-    @property
-    def actuators(self):
-        return self._lookup("actuators")
-
-    @property
-    def states(self):
-        return self._lookup("states")
-
-
-class SpecificSpec(EntitySpec):
-    def __init__(self, params):
-        params["states"] = dict()
-        super().__init__(params)
-
-    @property
-    def config(self):
-        return SpecView(self, depth=[])
-
-    @property
-    def states(self):
-        return SpecView(self, depth=["states"])
-
-
 # REQUIRED FOR BUILDING SPECS
 
 
 class Component(object):
     def __init__(self, **kwargs):
         # Iterates over provided arguments and sets the provided arguments as class properties
         for key, value in kwargs.items():
```

### Comparing `eagerx-0.1.8/eagerx/core/supervisor.py` & `eagerx-0.1.9/eagerx/core/supervisor.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/core/view.py` & `eagerx-0.1.9/eagerx/core/view.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/nodes/butterworth_filter.py` & `eagerx-0.1.9/eagerx/nodes/butterworth_filter.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/utils/network_utils.py` & `eagerx-0.1.9/eagerx/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/utils/node_utils.py` & `eagerx-0.1.9/eagerx/utils/node_utils.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/utils/utils.py` & `eagerx-0.1.9/eagerx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/eagerx/wrappers/flatten.py` & `eagerx-0.1.9/eagerx/wrappers/flatten.py`

 * *Files identical despite different names*

### Comparing `eagerx-0.1.8/pyproject.toml` & `eagerx-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eagerx"
-version = "0.1.8"
+version = "0.1.9"
 description = "Engine Angostic Gym Environments for Robotics"
 authors = ["Bas van der Heijden <d.s.vanderheijden@tudelft.nl>", "Jelle Luijkx <j.d.luijkx@tudelft.nl>"]
 license = "Apache2.0"
 homepage = "https://github.com/eager-dev/eagerx"
 repository = "https://github.com/eager-dev/eagerx"
 documentation = "https://eagerx.readthedocs.io/en/master/"
 
@@ -22,14 +22,15 @@
 termcolor = "^1.1.0"
 defusedxml = "^0.7.1"
 netifaces = "^0.11.0"
 pyglet = "^1.5.21"
 sphinx-autodoc-typehints = "^1.0"
 Sphinx = "^4.0"
 sphinx-rtd-theme = "^1.0"
+typing = "^3.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pytest = "^5.2"
 pytest-cov = "^3.0.0"
 flake8 = "^4.0.1"
 flake8-bugbear = "^22.1.11"
```

### Comparing `eagerx-0.1.8/setup.py` & `eagerx-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,19 +28,20 @@
  'psutil>=5.9.0,<6.0.0',
  'pyglet>=1.5.21,<2.0.0',
  'rospkg>=1.3.0,<2.0.0',
  'scikit-image>=0.17.2,<0.18.0',
  'sphinx-autodoc-typehints>=1.0,<2.0',
  'sphinx-rtd-theme>=1.0,<2.0',
  'tabulate>=0.8.9,<0.9.0',
- 'termcolor>=1.1.0,<2.0.0']
+ 'termcolor>=1.1.0,<2.0.0',
+ 'typing>=3.0,<4.0']
 
 setup_kwargs = {
     'name': 'eagerx',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Engine Angostic Gym Environments for Robotics',
     'long_description': None,
     'author': 'Bas van der Heijden',
     'author_email': 'd.s.vanderheijden@tudelft.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/eager-dev/eagerx',
```

### Comparing `eagerx-0.1.8/PKG-INFO` & `eagerx-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eagerx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Engine Angostic Gym Environments for Robotics
 Home-page: https://github.com/eager-dev/eagerx
 License: Apache2.0
 Author: Bas van der Heijden
 Author-email: d.s.vanderheijden@tudelft.nl
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: Other/Proprietary License
@@ -25,9 +25,10 @@
 Requires-Dist: pyglet (>=1.5.21,<2.0.0)
 Requires-Dist: rospkg (>=1.3.0,<2.0.0)
 Requires-Dist: scikit-image (>=0.17.2,<0.18.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.0,<2.0)
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
+Requires-Dist: typing (>=3.0,<4.0)
 Project-URL: Documentation, https://eagerx.readthedocs.io/en/master/
 Project-URL: Repository, https://github.com/eager-dev/eagerx
```

