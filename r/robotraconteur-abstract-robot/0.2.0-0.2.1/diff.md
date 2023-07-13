# Comparing `tmp/robotraconteur_abstract_robot-0.2.0-py3-none-any.whl.zip` & `tmp/robotraconteur_abstract_robot-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 25784 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       72 b- defN 22-Dec-29 07:57 robotraconteur_abstract_robot/__init__.py
--rw-rw-rw-  2.0 fat    85300 b- defN 22-Dec-29 23:06 robotraconteur_abstract_robot/abstract_robot.py
--rw-rw-rw-  2.0 fat     4997 b- defN 22-Dec-29 23:06 robotraconteur_abstract_robot/joint_trajectory_interpolator.py
--rw-rw-rw-  2.0 fat    14151 b- defN 22-Dec-29 23:06 robotraconteur_abstract_robot/trapezoidal_joint_trajectory_generator.py
--rw-rw-rw-  2.0 fat    11349 b- defN 22-Dec-30 02:31 robotraconteur_abstract_robot-0.2.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      614 b- defN 22-Dec-30 02:31 robotraconteur_abstract_robot-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Dec-30 02:31 robotraconteur_abstract_robot-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 22-Dec-30 02:31 robotraconteur_abstract_robot-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      949 b- defN 22-Dec-30 02:31 robotraconteur_abstract_robot-0.2.0.dist-info/RECORD
-9 files, 117554 bytes uncompressed, 24090 bytes compressed:  79.5%
+Zip file size: 25916 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       72 b- defN 23-Jul-05 06:37 robotraconteur_abstract_robot/__init__.py
+-rw-rw-rw-  2.0 fat    87139 b- defN 23-Jul-13 02:54 robotraconteur_abstract_robot/abstract_robot.py
+-rw-rw-rw-  2.0 fat     5118 b- defN 23-Jul-05 06:37 robotraconteur_abstract_robot/joint_trajectory_interpolator.py
+-rw-rw-rw-  2.0 fat    14613 b- defN 23-Jul-05 06:37 robotraconteur_abstract_robot/trapezoidal_joint_trajectory_generator.py
+-rw-rw-rw-  2.0 fat    11549 b- defN 23-Jul-13 16:03 robotraconteur_abstract_robot-0.2.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      614 b- defN 23-Jul-13 16:03 robotraconteur_abstract_robot-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 16:03 robotraconteur_abstract_robot-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 23-Jul-13 16:03 robotraconteur_abstract_robot-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      949 b- defN 23-Jul-13 16:03 robotraconteur_abstract_robot-0.2.1.dist-info/RECORD
+9 files, 120176 bytes uncompressed, 24222 bytes compressed:  79.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: robotraconteur_abstract_robot/joint_trajectory_interpolator.py
 Comment: 
 
 Filename: robotraconteur_abstract_robot/trapezoidal_joint_trajectory_generator.py
 Comment: 
 
-Filename: robotraconteur_abstract_robot-0.2.0.dist-info/LICENSE.txt
+Filename: robotraconteur_abstract_robot-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: robotraconteur_abstract_robot-0.2.0.dist-info/METADATA
+Filename: robotraconteur_abstract_robot-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: robotraconteur_abstract_robot-0.2.0.dist-info/WHEEL
+Filename: robotraconteur_abstract_robot-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: robotraconteur_abstract_robot-0.2.0.dist-info/top_level.txt
+Filename: robotraconteur_abstract_robot-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: robotraconteur_abstract_robot-0.2.0.dist-info/RECORD
+Filename: robotraconteur_abstract_robot-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## robotraconteur_abstract_robot/abstract_robot.py

```diff
@@ -1,1849 +1,1849 @@
-# Copyright 2022 Wason Technology, LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""
-Module containing ``AbstractRobot`` class. Robot Raconteur types are shortened for brevity. See 
-``com.robotraconteur.robotics.robot`` robdef ``using`` statements for fully qualified types.
-"""
-
-from enum import Enum
-import traceback
-from turtle import down
-import RobotRaconteur as RR
-RRN = RR.RobotRaconteurNode.s
-from RobotRaconteurCompanion.Util.RobotUtil import RobotUtil
-from RobotRaconteurCompanion.Util.DateTimeUtil import DateTimeUtil
-from RobotRaconteurCompanion.Util.GeometryUtil import GeometryUtil
-from RobotRaconteurCompanion.Util.SensorDataUtil import SensorDataUtil
-import time
-import threading
-import numpy as np
-from abc import ABC, abstractmethod
-
-from .joint_trajectory_interpolator import JointTrajectoryInterpolator
-from .trapezoidal_joint_trajectory_generator import JointTrajectoryLimits, JointTrajectoryPositionRequest, \
-    JointTrajectoryVelocityRequest, JointTrajectoryPositionCommand, TrapezoidalJointTrajectoryGenerator
-
-class AbstractRobot(ABC):
-    """
-    Abstact base class for standard Robot Raconteur robot device drivers. Subclasses implement specific functionality
-    for each robot controller type. Typically, these drivers communicate with the vendor controller. The vender
-    controller may provide the communication method natively, or the vendor controller may need to execute
-    special programs provided by the driver.
-
-    The driver uses a ``RobotInfo`` structure to initialize information about kinematics etc. The __init__
-    function should also be overridden to initialize various instance variables. The ``robot_info`` parameter
-    is typically loaded from a YAML file.
-
-    AbstractRobot uses a real-time loop that periodically calls ``_run_timestep()``, with the period set by 
-    ``_update_period``. ``_run_timestep()`` does the following, some of which the subclass must implement:
-
-    #. Read feedback from driver (must be implemented by subclass).
-         Update ``_joint_position``, ``_joint_velocity`` (optional), ``_joint_effort`` (optional), ``_endpoint_pose``, 
-        ``_endpoint_vel`` (optional), ``_ready``, ``_enabled``, ``_stopped``, ``_error``, ``_estop_source``,
-        ``_last_robot_state``, ``_last_joint_state``, and ``_last_endpoint_state``. These updates may happen
-        outside the loop, when the data is received from the robot. Hold ``_lock`` when updating data if not
-        inside the loop.
-    #. Verify communication by calling ``_verify_communication()``. If ``_last_robot_state``, ``_last_joint_state``,
-        or ``_last_endpoint_state`` exceed ``_communication_timeout`` relative to stopwatch time, set communication
-        failure.
-    #. Verify the current robot state by calling ``_verify_robot_state()
-    #. Fill a joint position or joint velocity command by calling ``_fill_robot_command()``. This will check the
-        current operational mode and commands from the client to generate the next command.
-    #. Fill the robot state structures to return to clients. Calls ``_fill_states()``, ``_fill_state_flags()``,
-        ``_calc_endpoint_poses()``, and ``_calc_endpoint_vels()``
-    #. If a valid command is available, send to the robot using ``_send_robot_command()``. Subclass must implement
-        this function.
-    
-    At a minimum, a driver subclass must fill feedback data from the robot as shown in step 1 above, and must
-    implement ``_send_robot_command()``, ``_send_disable()``, ``_send_enable()``, and ``_send_reset_errors()``.
-    See the example minimal ABB robot driver. Also see abb_robotraconteur_driver_hmp for a more sophisticated driver.    
-
-    :ivar _robot_info: The ``RobotInfo`` structure, initialized from __init__ parameter
-    :ivar _joint_names: The names of the robot joints. Initialized from ``robot_info`` or ``default_joint_count``
-    :ivar _joint_count: The number of robot joints. Initialized from ``robot_info`` or ``default_joint_count``
-    :ivar _robot_uuid: The UUID of the robot. Initialized from the ``robot_info`` structure
-    :ivar _robot_caps: The capability flags of the robot taken from ``RobotCapabilities`` enum. By default initialized
-                       from ``robot_info`, but it is recommended the driver override this value in __init__
-    :ivar _robot_util: Companion ``RobotUtil`` utility class instance
-    :ivar _datetime_util: Companion ``DateTimeUtil`` utility class instance
-    :ivar _geometry_util: Companion ``GeometryUtil`` utility class instance
-    :ivar _sensor_data_util: Companion ``SensorDataUtil`` utility class instance
-    :ivar _pose_dtype: ``com.robotraconteur.geometry.Pose`` numpy dtype
-    :ivar _spatial_velocity_dtype: ``com.robotraconteur.geometry.SpatialVelocity`` numpy dtype
-    :ivar _robot_state_type: ``RobotState`` structure type
-    :ivar _advanced_robot_state_type: ``AdvancedRobotState`` structure type
-    :ivar _robot_state_sensor_data_type: ``RobotStateSensorData`` structure type
-    :ivar _robot_joint_command_type: ``RobotJointCommand`` structure type
-    :ivar _isoch_info_type: ``IsochInfo`` structure type
-    :ivar _robot_consts: Constants from ``com.robotraconteur.robotics.robot``
-    :ivar _robot_capabilities: ``RobotCapabilities`` enum
-    :ivar _robot_command_mode: ``RobotCommandMode`` enum
-    :ivar _robot_operational_mode: ``RobotOperationalMode`` enum
-    :ivar _robot_controller_state: ``RobotControllerState`` enum
-    :ivar _robot_state_flags: ``RobotStateFlags`` enum
-    :ivar _joint_consts: Constants from ``com.robotraconteur.robotics.joints``
-    :ivar _joint_position_units: ``JointPositionUnits`` enum
-    :ivar _joint_effort_units: ``JointEffortUnits`` enum
-    :ivar _uses_homing: Robot uses homing command. Initialized from capabilities flags in ``robot_info``. 
-            Recommended to override in __init__
-    :ivar _has_position_command: Robot has streaming position command. Initialized from capabilities flags in 
-            ``robot_info``. Recommended to override in __init__
-    :ivar _has_velocity_command: Robot has streaming velocity command. Initialized from capabilities flags in 
-            ``robot_info``. Recommended to override in __init__
-    :ivar _has_jog_command: Robot has jog command. Initialized from capabilities flags in 
-            ``robot_info``. Recommended to override in __init__
-    :ivar _current_tool: Currently attached robot tool. Array, one entry per chain. Initialized from ``robot_info``,
-                            updated using ``tool_attached()`` and ``tool_detached()``
-    :ivar _current_payload: Currently attached payload. Array, one entry per chain. Initialized from ``robot_info``,
-                            updated using ``payload_attached()`` and ``payload_detached()``
-    :ivar _current_payload_pose: Pose of currently attached payload relative to tool TCP. Array, one entry per chain. 
-                                    Initialized from ``robot_info``, updated using ``payload_attached()`` 
-                                    and ``payload_detached()``
-    :ivar _keep_going: Boolean flag to stop loop
-    :ivar _update_period: The update period of the loop (aka timestep). Should be set in __init__
-    :ivar _speed_ratio: The current speed ratio. Set using ``speed_ratio`` property
-    :ivar _jog_joint_limit: The maximum joint distance allowed during a jog command
-    :ivar _trajectory_error_tol: The maximum error allowed between command and robot position during trajectory 
-                                    execution
-    :ivar _command_mode: The current command mode. Set using ``command_mode`` property, and updated during operation
-                            due to errors or other events.
-    :ivar _operational_mode: The operational mode of the vendor robot controller, using values from 
-                                ``RobotOperationalMode`` enum. Should be
-                                updated every timestep if available. Set ``_base_set_operational_mode`` to False
-                                if used.
-    :ivar _controller_state: The controller state of the vendor robot controller, using values from 
-                                ``RobotOperationalMode`` enum. Should be
-                                updated every timestep if available. Set ``_base_set_controller_state`` to False
-                                if used.
-    :ivar _joint_position: Current joint position based on feedback in radians (or meters). This value should be
-                            updated every timestep using robot feedback.
-    :ivar _joint_velocity: Current joint velocity based on feedback in radians/s (or meters/s). This value should be
-                            updated every timestep using robot feedback. Leave as empty array if velocity feedback
-                            not available.
-    :ivar _joint_effort: Current joint effort based on feedback in Nm (or N). This value should be
-                            updated every timestep using robot feedback. Leave as empty array if effort feedback
-                            not available.
-    :ivar _position_command: Current position command. Set by the subclass after issuing command to robot. This
-                                value is used for client state information.
-    :ivar _velocity_command: Current velocity command. Set by the subclass after issuing command to robot. This
-                                value is used for client state information.
-    :ivar _endpoint_pose: Array of endpoint poses, one entry per chain. Update every timestep. Units should be in 
-                            meters, quaternions, relative to world or base of robot.
-    :ivar _endpoint_vel: Array of endpoint velocities, one entry per chain. Update every timestep. Units should be in 
-                            meters/s, radians/s, relative to world or base of robot.
-    :ivar _last_robot_state: The stopwatch time in seconds of the last state update received from the robot. 
-                                Must be updated to avoid communication timeout.
-    :ivar _last_joint_state: The stopwatch time in seconds of the last joint position update received from the robot. 
-                                Must be updated to avoid communication timeout.
-    :ivar _last_endpoint_state: The stopwatch time in seconds of the last endpoint update received from the robot. 
-                                Must be updated to avoid communication timeout.
-    :ivar _state_seqno: Counter of number of loop iterations executed (sequence number)
-    :ivar _homed: Set to True if robot is homed. Only valid if robot has homing capability
-    :ivar _ready: Set to True if robot is ready to move. Should be updated every timestep
-    :ivar _enabled: Set to True if robot is enabled with motors on. Should be updated every timestep. Robot may
-                    be enabled but not ready
-    :ivar _stopped: Set to True if robot is stopped due to an estop. Should be updated every timestep
-    :ivar _error: Set to True if robot is in an error state. Should be updated every timestep. Errors are reset by
-                    switching to halt more, calling ``reset_errors()``, and/or clearing the error on the vendor
-                    controller, in escalating levels of severity.
-    :ivar _estop_source: The source of the estop, using values from ``RobotStateFlags``
-    :ivar _communication_failure: Set by ``_verify_communication`` based on ``_communication_timeout``
-    :ivar _communication_timeout: Communication timeout in seconds. If no updates are received from the controller
-                                  within the communication timeout, an error condition is set
-    :ivar _broadcast_downsampler: Broadcast downsampler used by all wires and pipes to control data rate sent to client
-    :ivar position_command: Wire populated by Robot Raconteur to receive streaming position commands. Only used 
-                            in ``position_command`` command mode
-    :ivar velocity_command: Wire populated by Robot Raconteur to receive streaming position commands. Only used 
-                            in ``velocity_command`` command mode
-    :ivar _wires_ready: Set to True when wires and pipes have been initialized by Robot Raconteur
-    :ivar _config_seqno: The sequence number returned as part of ``RobotInfo``. Incremented as tools and payloads
-                            are attached/detached.
-    :ivar _base_set_operational_mode: If True, abstract robot will set ``_operational_mode`` to a default value.
-                                        Set to False if driver will update ``_operational_mode``
-    :ivar _base_set_controller_state: If True, abstract robot will set ``_controller_state`` to a default value.
-                                        Set to False if driver will update ``_controller_state``
-    :ivar _lock: Lock to hold when updating data to prevent race conditions
-
-    :param robot_info: The ``RobotInfo`` structure for the robot
-    :param default_joint_count: The default number of joints for the robot
-    :param node: The Robot Raconteur node for the driver
-    """
-    def __init__(self, robot_info, default_joint_count, node = None ):
-        super().__init__()
-
-        if node is None:
-            self._node = RRN
-        else:
-            self._node = node
-
-        self._robot_info = robot_info
-        if robot_info.joint_info is not None:
-            j_names = []
-            for j_info in robot_info.joint_info:
-                j_names.append(j_info.joint_identifier.name)
-            self._joint_names = j_names
-        else:
-            assert default_joint_count > 0, "Joints must be specified in RobotInfo structure"
-            self._joint_names = [f"joint_{x}" for x in range(default_joint_count)]
-        
-        self._joint_count = len(self._joint_names)
-
-        self._robot_uuid = robot_info.device_info.device.uuid
-
-        self._robot_caps = robot_info.robot_capabilities
-
-        self._robot_util = RobotUtil(self._node)
-        self._datetime_util = DateTimeUtil(self._node)
-        self._geometry_util = GeometryUtil(self._node)
-        self._sensor_data_util = SensorDataUtil(self._node)
-
-        self._pose_dtype = self._node.GetNamedArrayDType("com.robotraconteur.geometry.Pose")
-        self._spatial_velocity_dtype = self._node.GetNamedArrayDType("com.robotraconteur.geometry.SpatialVelocity")
-        self._robot_state_type = self._node.GetStructureType("com.robotraconteur.robotics.robot.RobotState")
-        self._advanced_robot_state_type = self._node.GetStructureType("com.robotraconteur.robotics.robot.AdvancedRobotState")
-        self._robot_state_sensor_data_type = self._node.GetStructureType("com.robotraconteur.robotics.robot.RobotStateSensorData")
-        self._robot_joint_command_type = self._node.GetStructureType("com.robotraconteur.robotics.robot.RobotJointCommand")
-        self._isoch_info_type = self._node.GetStructureType("com.robotraconteur.device.isoch.IsochInfo")
-
-        self._robot_consts = self._node.GetConstants("com.robotraconteur.robotics.robot")
-        self._robot_capabilities = self._robot_consts["RobotCapabilities"]
-        self._robot_command_mode = self._robot_consts["RobotCommandMode"]
-        self._robot_operational_mode = self._robot_consts["RobotOperationalMode"]
-        self._robot_controller_state = self._robot_consts["RobotControllerState"]
-        self._robot_state_flags = self._robot_consts["RobotStateFlags"]
-
-        self._joint_consts = self._node.GetConstants("com.robotraconteur.robotics.joints")
-        self._joint_position_units = self._joint_consts["JointPositionUnits"]
-        self._joint_effort_units = self._joint_consts["JointEffortUnits"]
-
-        self._uses_homing = (self._robot_caps & self._robot_capabilities["homing_command"]) != 0
-        self._has_position_command = (self._robot_caps & self._robot_capabilities["position_command"]) != 0
-        self._has_velocity_command = (self._robot_caps & self._robot_capabilities["velocity_command"]) != 0
-        self._has_jog_command = (self._robot_caps & self._robot_capabilities["jog_command"]) != 0
-
-        try:
-            self._rox_robots = []
-            for chain_i in range(len(self._robot_info.chains)):
-                self._rox_robots.append(self._robot_util.robot_info_to_rox_robot(self._robot_info,chain_i))
-        except:
-            traceback.print_exc()
-            raise ValueError("invalid robot_info, could not populate GeneralRoboticsToolbox.Robot")
-
-        self._current_tool = [None]*len(self._robot_info.chains)
-        self._current_payload = [None]*len(self._robot_info.chains)
-        self._current_payload_pose = [None]*len(self._robot_info.chains)
-
-        for i in range(len(self._robot_info.chains)):
-            if self._robot_info.chains[i].current_tool is not None:
-                self._current_tool[i] = self._robot_info.chains[i].current_tool
-
-            if self._robot_info.chains[i].current_payload is not None:
-                self._current_payload[i] = self._robot_info.chains[i].current_payload
-
-        for i in range(self._joint_count):
-            limits = robot_info.joint_info[i].joint_limits
-            assert limits.velocity > 0, f"Invalid joint velocity for joint {i}"
-            if limits.reduced_velocity <= 0:
-                limits.reduced_velocity = limits.velocity
-
-            assert limits.acceleration > 0, f"Invalid joint acceleration for joint {i}"
-            if limits.reduced_acceleration <= 0:
-                limits.reduced_acceleration = limits.acceleration
-
-        self._keep_going = False
-
-        self._stopwatch_epoch = None
-        self._stopwatch_start = None
-
-        self._loop_thread = None
-        self._update_period = 0.01
-
-        self._wait_event = threading.Event()
-
-        self._last_robot_state = 0
-        self._last_joint_state = 0
-        self._last_endpoint_state = 0
-
-        self._state_seqno = 0
-
-        self._speed_ratio = 1.0
-
-        self._jog_joint_limit = np.deg2rad(1000.)
-        self._trajectory_error_tol = np.deg2rad(5.)
-
-        self._command_mode = self._robot_command_mode["halt"]
-        self._operational_mode = self._robot_operational_mode["manual_reduced_speed"]
-        self._controller_state = self._robot_operational_mode["undefined"]
-
-        self._joint_position = np.zeros((0,))
-        self._joint_velocity = np.zeros((0,))
-        self._joint_effort = np.zeros((0,))
-
-        self._position_command = None
-        self._velocity_command = None
-
-        self._endpoint_pose = []
-        self._endpoint_vel = []
-
-        self._homed = False
-        self._ready = False
-        self._enabled = False
-        self._stopped = False
-        self._error = False
-        self._estop_source = 0
-
-        self._communication_failure = True
-        self._communication_timeout = 0.25
-
-        self._broadcast_downsampler = None
-
-        self._wire_position_command_sent = False
-        self._wire_velocity_command_sent = False
-        self._wire_position_command_last_seqno = 0
-        self._wire_velocity_command_last_seqno = 0
-        self._wire_position_command_last_ep = 0
-        self._wire_velocity_command_last_ep = 0
-
-        self._trajectory_valid = False
-        self._trajectory_current_time = 0
-        self._trajectory_max_time = 0
-        self._trajectory_waypoint = 0
-
-        self._lock = threading.Lock()
-
-        self._wires_ready = False
-
-        self._active_trajectory = None
-        self._queued_trajectories = []
-
-        self._jog_start_time = 0.
-        self._jog_trajectory_generator = None
-        self._jog_completion_handler = None
-
-        self._config_seqno = 1
-
-        self._base_set_operational_mode = True
-        self._base_set_controller_state = True
-
-    def RRServiceObjectInit(self, context, service_path):
-        self.robot_state_sensor_data.MaxBacklog = 3
-
-        self._broadcast_downsampler = RR.BroadcastDownsampler(context, 0)
-        self._broadcast_downsampler.AddPipeBroadcaster(self.robot_state_sensor_data)
-        self._broadcast_downsampler.AddWireBroadcaster(self.robot_state)
-        self._broadcast_downsampler.AddWireBroadcaster(self.advanced_robot_state)
-        self._broadcast_downsampler.AddWireBroadcaster(self.device_clock_now)
-
-        self._wires_ready = True
-
-    def _perf_counter(self) -> float:
-        """
-        System performance counter in seconds. This counter is not relative to real time clock.
-
-        :return: Performance counter time in seconds
-        """
-        return time.perf_counter()
-
-    def _stopwatch_ellapsed_s(self) -> float:
-        """
-        Stopwatch time in seconds. Relative to start of driver loop.
-
-        :return: Stopwatch time in seconds
-        """
-        return self._perf_counter() - self._stopwatch_start
-
-    def _start_robot(self):
-        """
-        Start the robot driver loop
-        """
-
-        self._stopwatch_epoch = self._datetime_util.TimeSpec2Now()
-        self._stopwatch_start = self._perf_counter()
-
-        self._keep_going = True
-        self._loop_thread = threading.Thread(target = self._loop_thread_func)
-        self._loop_thread.daemon = True
-        self._loop_thread.start()
-
-    def _stop_robot(self):
-        """
-        Stop the robot driver loop
-        """
-        self._keep_going = False
-        self._loop_thread.join()
-
-    def _loop_thread_func(self):
-        """
-        Loop thread entry function. This function runs the loop, and calls ``run_timestep()`` periodically at
-        ``_update_period`` specified in seconds.
-        """
-
-        next_wait = self._stopwatch_ellapsed_s()
-        now = next_wait
-
-        while self._keep_going:
-
-            self._run_timestep(now)
-
-            now = self._stopwatch_ellapsed_s()
-
-            while True:
-                next_wait += self._update_period
-                if next_wait > now:
-                    break
-
-            while True:
-                now = self._stopwatch_ellapsed_s()
-                if now >= next_wait:
-                    break
-                self._wait_event.wait(timeout=(next_wait-now))
-
-            
-    def _close(self):
-        """
-        Close the driver, stop the loop
-        """
-        self._keep_going = False
-        try:
-            self._loop_thread.join(timeout=1)
-        except:
-            pass
-
-    
-
-    def _run_timestep(self, now):
-        """
-        Called by loop each timestep at ``_update_timestep`` period in seconds
-
-        :param now: stopwatch time in seconds
-        """
-        res = False
-        joint_pos_cmd = None
-        joint_vel_cmd = None
-
-        rr_robot_state = None
-        rr_advanced_robot_state = None
-        rr_state_sensor_data = None
-        downsampler_step = None
-
-        with self._lock:
-            if self._wires_ready:
-                downsampler_step = RR.BroadcastDownsamplerStep(self._broadcast_downsampler)
-
-            self._state_seqno += 1
-
-            res = self._verify_communication(now)
-            res = res and self._verify_robot_state(now)
-            res_fill, joint_pos_cmd, joint_vel_cmd = self._fill_robot_command(now)
-            res = res and res_fill
-
-            rr_robot_state, rr_advanced_robot_state, rr_state_sensor_data = self._fill_states(now)
-
-        if res:
-            self._send_robot_command(now, joint_pos_cmd, joint_vel_cmd)
-
-        if downsampler_step:
-            with downsampler_step:
-                self._send_states(now, rr_robot_state, rr_advanced_robot_state, rr_state_sensor_data)
-
-    def _fill_state_flags(self, now):
-        """
-        Fill ``_robot_state_flags`` based on current state of driver. Called by the loop each timestep to update 
-        driver state
-
-        :param now: stopwatch time in seconds
-        """
-
-        f = 0
-        if self._communication_failure:
-            f |= self._robot_state_flags["communication_failure"]
-            return f
-
-        if self._error:
-            f |= self._robot_state_flags["error"]
-
-        if self._stopped:
-            f |= self._robot_state_flags["estop"]
-
-            if self._estop_source == 0:
-                pass
-            elif self._estop_source == 1:
-                f |= self._robot_state_flags["estop_button1"]
-            elif self._estop_source == 2:
-                f |= self._robot_state_flags["estop_other"]
-            elif self._estop_source == 3:
-                f |= self._robot_state_flags["estop_fault"]
-            elif self._estop_source == 4:
-                f |= self._robot_state_flags["estop_internal"]
-        
-        if self._enabled:
-            f |= self._robot_state_flags["enabled"]
-
-        if self._ready:
-            f |= self._robot_state_flags["ready"]
-
-        if self._uses_homing:
-            if self._homed:
-                f |= self._robot_state_flags["homed"]
-            else:
-                f |= self._robot_state_flags["homing_required"]
-
-        if self._wire_position_command_sent:
-            f |= self._robot_state_flags["valid_position_command"]
-
-        if self._wire_velocity_command_sent:
-            f |= self._robot_state_flags["valid_velocity_command"]
-
-        if self._trajectory_valid:
-            f |= self._robot_state_flags["trajectory_running"]
-
-        return f
-
-    def _calc_endpoint_pose(self, chain):
-        """
-        Compute endpoint pose for specified chain. By default uses ``_endpoint_pose[chain]`` and transforms
-        to the TCP of ``self._current_tool[chain]``. If the robot reports the endpoint position with the tool
-        transform applied, this should return ``self._endpoint_pose[chain]``
-
-        Called by the loop each timestep to update driver state.
-
-        :param chain: The chain index, always 0 for single arm driver
-        :rtype: com.robotraconteur.geometry.Pose
-        :return: The pose of the end effector
-        """
-
-        # CALL LOCKED!
-        if self._current_tool[chain] is None:
-            return self._endpoint_pose[chain]
-
-        endpoint_transform = self._geometry_util.pose_to_rox_transform(self._endpoint_pose[chain])
-        tool_transform = self._geometry_util.transform_to_rox_transform(self._current_tool[chain].tcp)
-        res = endpoint_transform * tool_transform
-        return self._geometry_util.rox_transform_to_pose(res)
-
-    def _calc_endpoint_poses(self):
-        """
-        Compute the endpoints of all chains. Calls ``_calc_endpoint_pose()`` for each chain.
-
-        Called by the loop each timestep to update driver state.
-
-        :rtype: com.robotraconteur.geometry.Pose[]
-        :return: Array of all chain poses. Single element array for single arm drivers
-        """
-        if self._endpoint_pose is None:
-            return np.zeros((0,), dtype=self._pose_dtype)
-        n = len(self._endpoint_pose)
-        o = np.zeros((n,), dtype=self._pose_dtype)
-        for i in range(n):
-            o[i] = self._calc_endpoint_pose(i)
-        return o
-
-    def _calc_endpoint_vel(self, chain):
-        """
-        Compute spatial velocity for specified chain. By default uses ``_endpoint_vel[chain]`` and applies TCP
-        transform of ``self._current_tool[chain]``. If the robot reports the endpoint position with the tool
-        transform applied, this should return ``self._endpoint_vel[chain]``
-
-        Called by the loop each timestep to update driver state.
-
-        :param chain: The chain index, always 0 for single arm driver
-        :rtype: com.robotraconteur.geometry.SpatialVelocity
-        :return: The spatial velocity (6x1) of the end effector
-        """
-        # CALL LOCKED!
-
-        if self._current_tool[chain] is None:
-            return self._endpoint_vel[chain]
-
-        endpoint_vel = self._geometry_util.spatial_velocity_to_array(self._endpoint_vel).flatten()
-        endpoint_vel_ang = endpoint_vel[0:3]
-        endpoint_vel_lin = endpoint_vel[3:7]
-        current_tool_p = self._geometry_util.point_to_xyz(self._current_tool[chain].tcp["translation"])
-
-        endpoint_transform = self._geometry_util.pose_to_rox_transform(self._endpoint_pose[chain])
-
-        
-        vel = endpoint_vel_lin + np.cross(endpoint_vel_ang, np.matmul(endpoint_transform.R, current_tool_p))
-
-        return self._geometry_util.array_to_spatial_acceleration(np.concatenate((endpoint_vel_ang, vel)))
-
-    def _calc_endpoint_vels(self):
-        """
-        Compute the spatial velocity of all chains. Calls ``_calc_endpoint_vel()`` for each chain.
-
-        Called by the loop each timestep to update driver state.
-
-        :rtype: com.robotraconteur.geometry.SpatialVelocity[]
-        :return: Array of all chain spatial velocities. Single element array for single arm drivers
-        """
-
-        if self._endpoint_vel is None:
-            return np.zeros((0,),dtype=self._spatial_velocity_dtype)
-
-        n = len(self._endpoint_vel)
-        o = np.zeros((n,),dtype=self._spatial_velocity_dtype)
-        for i in range(n):
-            o[i] = self._calc_endpoint_vel(i)
-        
-        return o
-
-    def _fill_states(self, now):
-        """
-        Fill the ``RobotState``, ``AdvancedRobotState``, and ``RobotStateSensorData`` structures based on
-        current driver state.
-
-        Called by the loop each timestep to fill data to send to clients.
-
-        :param now: stopwatch time in seconds
-        :rtype: Tuple[RobotState,AdvancedRobotState,RobotStateSensorData]
-        """
-        ts = self._datetime_util.TimeSpec3Now()
-
-        rob_state = self._robot_state_type()               
-        rob_state.ts = ts
-        rob_state.seqno = self._state_seqno
-        rob_state.command_mode = self._command_mode
-        rob_state.operational_mode = self._operational_mode
-        rob_state.controller_state = self._controller_state
-
-        flags = self._fill_state_flags(now)
-
-        rob_state.robot_state_flags = flags
-
-        rob_state.joint_position = np.copy(self._joint_position)
-        rob_state.joint_velocity = np.copy(self._joint_velocity)
-        rob_state.joint_effort = np.copy(self._joint_effort)
-        rob_state.joint_position_command = self._position_command if self._position_command is not None \
-                else np.zeros((0,))
-        rob_state.joint_velocity_command = self._velocity_command if self._velocity_command is not None \
-                else np.zeros((0,))
-        rob_state.kin_chain_tcp = self._calc_endpoint_poses()
-        rob_state.kin_chain_tcp_vel = self._calc_endpoint_vels()
-        rob_state.trajectory_running = self._trajectory_valid
-
-        a_rob_state = self._advanced_robot_state_type()
-        a_rob_state.ts = ts
-        a_rob_state.seqno = rob_state.seqno
-        a_rob_state.command_mode = rob_state.command_mode
-        a_rob_state.operational_mode = rob_state.operational_mode
-        a_rob_state.controller_state = rob_state.controller_state
-        a_rob_state.robot_state_flags = rob_state.robot_state_flags
-        a_rob_state.joint_position = rob_state.joint_position
-        a_rob_state.joint_velocity = rob_state.joint_velocity
-        a_rob_state.joint_effort = rob_state.joint_effort
-        a_rob_state.joint_position_command = rob_state.joint_position_command
-        a_rob_state.joint_velocity_command = rob_state.joint_velocity_command
-        a_rob_state.kin_chain_tcp = rob_state.kin_chain_tcp
-        a_rob_state.kin_chain_tcp_vel = rob_state.kin_chain_tcp_vel
-        a_rob_state.trajectory_running = rob_state.trajectory_running
-        a_rob_state.joint_position_units = [self._joint_position_units["radian"]]*self._joint_count
-        a_rob_state.joint_effort_units = [self._joint_effort_units["newton_meter"]]*self._joint_count
-        a_rob_state.trajectory_running = self._trajectory_valid
-        a_rob_state.trajectory_time = self._trajectory_current_time
-        a_rob_state.trajectory_max_time = self._trajectory_max_time
-        a_rob_state.trajectory_current_waypoint = self._trajectory_waypoint
-        a_rob_state.config_seqno = self._config_seqno
-
-        sensor_data_header = self._sensor_data_util.FillSensorDataHeader(self._robot_info.device_info, self._state_seqno)
-
-        sensor_data = self._robot_state_sensor_data_type()
-        sensor_data.data_header = sensor_data_header
-        sensor_data.robot_state = a_rob_state
-
-        return rob_state, a_rob_state, sensor_data
-
-
-    def _send_states(self, now, rr_robot_state, rr_advanced_robot_state, rr_state_sensor_data):
-        """
-        Sends the states to the Robot Raconteur clients using broadcast wires
-
-        Called by the loop each timestep to send data to clients.
-
-        :param now: stopwatch time in seconds
-        :param rr_robot_state: populated RobotState instance
-        :param rr_advanced_robot_state: populated AdvancedRobotState instance
-        :param rr_state_sensor_data: populated RobotStateSensorData instance
-        """
-        if not self._wires_ready:
-            return
-             
-        self.robot_state.OutValue = rr_robot_state
-        self.advanced_robot_state.OutValue = rr_advanced_robot_state
-        self.robot_state_sensor_data.AsyncSendPacket(rr_state_sensor_data, lambda: None)
-        self.device_clock_now.OutValue = self._datetime_util.FillDeviceTime(self._robot_info.device_info, self._state_seqno)
-
-    @abstractmethod
-    def _send_disable(self, handler):
-        """
-        Called to send a disable command to the robot. Only valid if driver has ``software_enable`` capability.
-        Implementing class must override if used. ``handler`` must be called to complete the asynchronous request.
-        """
-        pass
-
-    def async_disable(self, handler):
-        """Called by client to request robot disable. Calls ``_send_disable()``"""
-        self._send_disable(handler)
-
-    @abstractmethod
-    def _send_enable(self, handler):
-        """
-        Called to send an enable command to the robot. Only valid if driver has ``software_enable`` capability.
-        Implementing class must override if used. ``handler`` must be called to complete the asynchronous request.
-        """
-        pass
-
-    def async_enable(self, handler):
-        """Called by client to request robot enable. Calls ``_send_enable()``"""
-        self._send_enable(handler)
-
-    @abstractmethod
-    def _send_reset_errors(self, handler):
-        """
-        Called to send an reset errors command to the robot. Only valid if driver has ``software_reset_errors`` 
-        capability. Implementing class must override if used. ``handler`` must be called to complete the asynchronous 
-        request.
-        """
-        pass
-
-    def async_reset_errors(self, handler):
-        """Called by client to request software reset errors. Calls ``_send_reset_errors()``"""
-        self._send_reset_errors(handler)
-
-    def _verify_communication(self, now):
-        """
-        Verify that the driver is communicating with robot. Compares last communication tomi te 
-        ``_communication_timeout`` to determine when communication has been lost.
-
-        Called by the loop each timestep to check if robot is still communicating.
-
-        :param now: stopwatch time in seconds
-        """
-        if (now - self._last_joint_state) > self._communication_timeout \
-            or (now - self._last_robot_state) > self._communication_timeout \
-            or (now - self._last_endpoint_state) > self._communication_timeout :
-
-            self._communication_failure = True
-
-            self._command_mode = self._robot_command_mode["invalid_state"]
-            if self._base_set_operational_mode:
-                self._operational_mode = self._robot_operational_mode["undefined"]
-                self._controller_state = self._robot_controller_state["undefined"]
-
-            self._joint_position = np.zeros((0,))
-            self._joint_velocity = np.zeros((0,))
-            self._joint_effort = np.zeros((0,))
-
-            self._endpoint_pose = None
-            self._endpoint_vel = None
-
-            return False
-
-        if self._base_set_operational_mode:
-            self._operational_mode = self._robot_operational_mode["cobot"]
-        self._communication_failure = False
-
-        return True
-
-    def _verify_robot_state(self, now):
-        """
-        Verify that the robot is ready to operate, or if an error has occurred. Drops to ``halt`` command mode
-        if robot is not ready. Drops to ``error`` command mode if error has occurred.
-
-        :param now: stopwatch time in seconds
-        """
-
-        if self._command_mode == self._robot_command_mode["homing"]:
-            if self._enabled and not self._error and not self._communication_failure:
-                if self._base_set_controller_state:
-                    self._controller_state = self._robot_controller_state["motor_off"]
-                return True
-
-        if not self._ready or self._error or self._communication_failure:
-            if self._base_set_controller_state:
-                if self._stopped:
-                    self._controller_state = self._robot_controller_state["emergency_stop"]
-                elif self._error:
-                    self._controller_state = self._robot_controller_state["guard_stop"]
-                else:
-                    self._controller_state = self._robot_controller_state["motor_off"]
-            if self._error or self._command_mode != self._robot_command_mode["halt"]:
-                self._command_mode = self._robot_command_mode["invalid_state"]
-            return False
-
-        if not self._enabled:
-            if self._base_set_controller_state:
-                self._controller_state = self._robot_controller_state["motor_off"]
-            if self._command_mode != self._robot_command_mode["halt"]:
-                self._command_mode = self._robot_command_mode["invalid_state"]
-            return False
-
-        if self._command_mode == self._robot_command_mode["invalid_state"] and not self._error:
-             self._command_mode = self._robot_command_mode["halt"]
-
-        if self._base_set_controller_state:
-            self._controller_state = self._robot_controller_state["motor_on"]
-
-        return True
-
-    def _fill_robot_command(self, now):
-        """
-        Fill robot command to send to robot based on current state and commands sent by the client. Returns a
-        tuple containing three elements: ``success``, ``joint_position_command``, ``joint_velocity_command``.
-        If success is False, the driver cannot generate a command in its current state. If ``success`` is True,
-        either ``joint_position_command`` will be non-Null, or ``joint_velocity_command`` will be non-Null.
-        ``joint_velocity_command`` is only valid if the driver has the ``velocity_command`` driver capability.
-        ``joint_position_command`` is in radians (or meters), while ``joint_velocity_command`` is in radians/s 
-        (or meters/s)
-
-        This function is called by the loop every timestep, and the return is passed to ``_send_joint_command()``.
-        It is not typically called by the implementing class.
-
-        :param now: stopwatch time in seconds
-        :rtype: Tuple[bool,np.array,np.array]
-        :return: ``success``, ``joint_position_command``, ``joint_velocity_command``
-        """
-
-        self._wire_position_command_sent = False
-        self._wire_velocity_command_sent = False
-
-        self._trajectory_valid = False
-        self._trajectory_current_time = 0.
-        self._trajectory_max_time = 0.
-        self._trajectory_waypoint = 0
-
-        if self._command_mode != self._robot_command_mode["trajectory"]:
-            if self._active_trajectory is not None:
-                self._active_trajectory._invalid_mode()
-                self._active_trajectory = None
-
-            if len(self._queued_trajectories) > 0:
-                for t in self._queued_trajectories:
-                    t._cancelled_in_queue()
-                self._queued_trajectories.clear()
-
-        if self._command_mode != self._robot_command_mode["jog"]:
-            if self._jog_trajectory_generator is not None:
-                self._jog_trajectory_generator = None
-            if self._jog_completion_handler is not None:
-                h = self._jog_completion_handler
-                self._jog_completion_handler = None
-                self._node.PostToThreadPool(lambda: h(None))
-            
-        if self._command_mode != self._robot_command_mode["velocity_command"]:
-            # self._velocity_command = None
-            pass
-        
-        if self._command_mode == self._robot_command_mode["jog"]:
-            if self._jog_trajectory_generator is not None:
-                jog_time = now - self._jog_start_time
-
-                if jog_time > self._jog_trajectory_generator.t_final:
-                    if self._jog_completion_handler is not None:
-                        h = self._jog_completion_handler
-                        self._jog_completion_handler = None
-                        self._node.PostToThreadPool(lambda: h(None))
-                    self._jog_trajectory_generator = None
-                    return False, None, None
-                
-                res, jog_command = self._jog_trajectory_generator.get_command(jog_time)
-                if not res:
-                    return False, None, None
-
-                joint_pos_cmd = jog_command.command_position
-                return True, joint_pos_cmd, None
-
-            else:
-                if self._jog_completion_handler is not None:
-                    h = self._jog_completion_handler
-                    self._jog_completion_handler = None
-                    self._node.PostToThreadPool(lambda: h(None))
-        
-                return True, None, None
-
-        elif self._command_mode == self._robot_command_mode["position_command"]:
-            
-            res, pos_cmd, ts, ep = self.position_command.TryGetInValue()
-            if not res:
-                return True, None, None
-
-            if self._wire_position_command_last_ep != ep:
-                self._wire_position_command_last_ep = ep
-                self._wire_position_command_last_seqno = 0
-
-            if pos_cmd is None \
-                or pos_cmd.seqno < self._wire_position_command_last_seqno \
-                or abs(pos_cmd.state_seqno - self._state_seqno) > 10 \
-                or len(pos_cmd.command) != self._joint_count \
-                or len(pos_cmd.units) != 0 and len(pos_cmd.units) != self._joint_count:
-                    return True, None, None
-            
-            pos_cmd_j = None
-            if len(pos_cmd.units) == 0:
-                pos_cmd_j = pos_cmd.command
-            else:
-                pos_cmd_j = np.zeros((self._joint_count,))
-                for i in range(self._joint_count):
-                    if pos_cmd.units[i] == self._joint_position_units["implicit"] \
-                        or pos_cmd.units[i] == self._joint_position_units["radian"]:
-                        pos_cmd_j[i] = pos_cmd.command[i]
-                    elif pos_cmd.units[i] == self._joint_position_units["degree"]:
-                        pos_cmd_j[i] = np.deg2rad(pos_cmd.command[i])
-                    elif pos_cmd.units[i] == self._joint_position_units["ticks_rot"]:
-                        pos_cmd_j[i] = pos_cmd.command[i]*(2.*np.pi)/(pow(2.,20.))
-                    elif pos_cmd.units[i] == self._joint_position_units["nanoticks_rot"]:
-                        pos_cmd_j[i] = pos_cmd.command[i]*(2.*np.pi)/(pow(2.,20.)*1.e9)
-                    else:
-                        return True, None, None
-
-            self._wire_position_command_last_seqno = pos_cmd.seqno
-            self._wire_position_command_sent = True
-            return True, pos_cmd_j, None
-
-        elif self._command_mode == self._robot_command_mode["velocity_command"]:
-            
-            res, vel_cmd, ts, ep = self.velocity_command.TryGetInValue()
-            if not res:
-                return True, None, None
-
-            if self._wire_velocity_command_last_ep != ep:
-                self._wire_velocity_command_last_ep = ep
-                self._wire_velocity_command_last_seqno = 0
-
-            if vel_cmd is None \
-                or vel_cmd.seqno < self._wire_velocity_command_last_seqno \
-                or abs(vel_cmd.stat_seqno - self._state_seqno) > 10 \
-                or len(vel_cmd.command) != self._joint_count \
-                or len(vel_cmd.units) != 0 and len(vel_cmd.units) != self._joint_count:
-                    return True, None, None
-            
-            vel_cmd_j = None
-            if len(vel_cmd.units) == 0:
-                vel_cmd_j = vel_cmd.command
-            else:
-                vel_cmd_j = np.zeros((self._joint_count,))
-                for i in range(self._joint_count):
-                    if vel_cmd.units[i] == self._joint_position_units["implicit"] \
-                        or vel_cmd.units[i] == self._joint_position_units["radian_second"]:
-                        vel_cmd_j[i] = vel_cmd.command[i]
-                    elif vel_cmd.units[i] == self._joint_position_units["degree_second"]:
-                        vel_cmd_j[i] = np.deg2rad(vel_cmd.command[i])
-                    elif vel_cmd.units[i] == self._joint_position_units["ticks_rot_second"]:
-                        vel_cmd_j[i] = vel_cmd.command[i]*(2.*np.pi)/(pow(2.,20.))
-                    elif vel_cmd.units[i] == self._joint_position_units["nanoticks_rot_second"]:
-                        vel_cmd_j[i] = vel_cmd.command[i]*(2.*np.pi)/(pow(2.,20.)*1.e9)
-                    else:
-                        return True, None, None
-
-            self._wire_position_command_last_seqno = vel_cmd.seqno
-
-            if self._speed_ratio != 1.0:
-                vel_cmd_j *= self._speed_ratio
-
-            self._wire_position_command_sent = True
-            return True, None, vel_cmd_j
-
-        elif self._command_mode == self._robot_command_mode["trajectory"]:
-
-            if self._active_trajectory is not None:
-                send_traj_cmd = False
-
-                interp_res, traj_pos, traj_vel, traj_t, traj_max_time, traj_waypoint = self._active_trajectory._get_setpoint(now, self._joint_position)
-
-                if interp_res == TrajectoryTaskRes.ready:
-                    self._trajectory_valid = True
-                    send_traj_cmd = False
-                elif interp_res == TrajectoryTaskRes.first_valid_setpoint or \
-                     interp_res == TrajectoryTaskRes.valid_setpoint:
-
-                     self._trajectory_valid = True
-                     send_traj_cmd = True
-                elif interp_res == TrajectoryTaskRes.trajectory_complete:
-                    self._trajectory_valid = True
-                    send_traj_comd = True
-                    self._active_trajectory = None
-                    if len(self._queued_trajectories) > 0:
-                        self._active_trajectory = self._queued_trajectories.pop(0)
-                else:
-                    self._trajectory_valid = False
-                    send_traj_cmd = False
-                    self._active_trajectory = None
-                    for w in self._queued_trajectories:
-                        w._cancelled_in_queue()
-                    self._queued_trajectories.clear()
-                
-                if self._trajectory_valid:
-                    self._trajectory_current_time = traj_t
-                    self._trajectory_max_time = traj_max_time
-                    self._trajectory_waypoint = traj_waypoint
-
-                if send_traj_cmd:
-                    joint_pos_cmd = traj_pos
-                else:
-                    joint_pos_cmd = None
-
-            else:
-                joint_pos_cmd = None
-            return True, joint_pos_cmd, None
-        
-        else:
-            return True, None, None
-
-    @abstractmethod
-    def _send_robot_command(self, now, joint_pos_cmd, joint_vel_cmd):
-        """
-        Called each timestep to send robot command. Must be implemented by subclass.
-
-        Both ``joint_pos_cmd`` and ``joint_vel_cmd`` may be None if there is no valid command available.
-        If ``joint_pos_cmd`` is non-Null, a joint position command must be sent. All drivers must support
-        position command. ``joint_vel_cmd`` is only used for ``velocity_command`` mode, and is only supported
-        if the driver has ``velocity_command`` capability.
-
-        :param now: stopwatch time in seconds
-        :param joint_pos_cmd: Joint position command in radians (or meters)
-        :param joint_vel_cmd: Joint velocity command in radians/s (or meters/s)
-        """
-        pass
-                        
-    @property
-    def command_mode(self):
-        """
-        Get or set the current command mode. Command mode must always be set to ``halt`` (0) before changing to another 
-        mode. If there is an error, the mode will change to ``error`` (-1), and must be set to ``halt`` to clear the 
-        error. If the error cannot be cleared, it may be possible to call the robot a "reset_errors()" function, if the 
-        driver has the ``software_reset_errors`` capability.
-
-        ``jog`` mode (1) requires the robot be in manual operational mode, if the robot supports reading the
-        operational mode and is not a cobot. The ``jog_command`` capability is required.
-
-        ``trajectory`` mode (2) can run in auto or manual operational mode and requires the ``trajectory_command`` 
-        capability.
-
-        ``position_command`` mode (3) can run in auto or manual operational mode and requires the 
-        ``position_command`` capability.
-
-        ``velocity_command`` mode (4) can run in auto or manual operational mode and requires the 
-        ``velocity_command`` capability.
-
-        ``homing_command`` mode (5) requires the ``homing_command`` capability. The implementation is device specific
-
-        """
-        with self._lock:
-            return self._command_mode
-
-    @command_mode.setter
-    def command_mode(self, value):
-        with self._lock:
-            if self._command_mode == self._robot_command_mode["invalid_state"] \
-                and value == self._robot_command_mode["homing"]:
-
-                if not self._enabled or self._communication_failure:
-                    raise RR.InvalidOperationException("Cannot set homing command mode in current state")
-
-                self._command_mode = self._robot_command_mode["homing"]
-                return
-
-            if self._command_mode == self._robot_command_mode["invalid_state"] \
-                and value == self._robot_command_mode["halt"] and self._enabled and not self._error \
-                and not self._communication_failure:
-
-                self._command_mode = value
-                return
-
-            if self._communication_failure:
-                raise RR.InvalidOperationException("Cannot set robot command mode in current state")
-
-            if not self._ready and value != self._robot_command_mode["halt"]:
-                raise RR.InvalidOperationException("Cannot set robot command mode in current state")
-
-            if self._command_mode != self._robot_command_mode["halt"] and value != self._robot_command_mode["halt"]:
-                raise RR.InvalidOperationException("Must switch to \"halt\" before selecting new mode")
-
-            if value == self._robot_command_mode["jog"]:
-                if not self._has_jog_command:
-                    raise RR.InvalidOperationException("Robot does not support jog command mode")
-                self._jog_trajectory_generator = None
-                self._command_mode = self._robot_command_mode["jog"]
-            elif value == self._robot_command_mode["halt"]:
-                self._command_mode = value
-            elif value == self._robot_command_mode["homing"]:
-                if not self._uses_homing:
-                    raise RR.InvalidOperationException("Robot does not support homing command mode")
-                self._command_mode = value
-            elif value == self._robot_command_mode["position_command"]:
-                if not self._has_position_command:
-                    raise RR.InvalidOperationException("Robot does not support position command mode")
-                self._command_mode = value
-            elif value == self._robot_command_mode["velocity_command"]:
-                if not self._has_velocity_command:
-                    raise RR.InvalidOperationException("Robot does not support velocity command mode")
-                self._command_mode = value
-            elif value == self._robot_command_mode["trajectory"]:
-                self._command_mode = value
-            else:
-                raise RR.InvalidOperationException("Invalid command mode specified")
-    
-    def async_jog_freespace(self, joint_position, max_velocity, wait, handler):
-        """
-        Called by client to jog the robot to a specified joint position with specified maximum joint velocity. If wait
-        is True, the function will not return to the client until the move is complete. Otherwise will return
-        immediately.
-
-        This function is typically used to jog the robot to a specific position.
-
-        Robot must be in ``jog`` command mode to call this function.
-
-        This is an asynchronous function, and handler must be called to return result to the client.
-
-        :param joint_position: The desired joint position in radians
-        :type joint_position: np.ndarray
-        :param max_velocity: The maximum joint velocity in radians/s
-        :type max_velocity: np.ndarray
-        :param wait: Wait for completion or return immediately
-        :type wait: bool
-        :param handler: Handler to call when function is complete
-        :type handler: Callable[[],Exception]
-        """
-        with self._lock:
-
-            if self._command_mode != self._robot_command_mode["jog"]:
-                raise RR.InvalidOperationException("Robot not in jog mode")
-
-            if not self._ready:
-                raise RR.InvalidOperationException("Robot not ready")
-
-            if len(joint_position) != self._joint_count:
-                raise RR.InvalidArgumentException(f"joint_position array must have {self._joint_count} elements")
-
-            if len(max_velocity) != self._joint_count:
-                raise RR.InvalidArgumentException(f"max_velocity array must have {self._joint_count} elements")
-
-            
-            if np.any(np.abs(self._joint_position - joint_position) > self._jog_joint_limit):
-                raise RR.InvalidArgumentException("Position command must be within 15 degrees from current")
-
-            if np.any(max_velocity <= 0):
-                raise RR.InvalidArgumentException("max_velocity must be greater than zero")
-
-            if self._jog_completion_handler is not None:
-                h = self._jog_completion_handler
-                self._jog_completion_handler = None
-                self._node.PostToThreadPool(
-                    lambda: h(RR.OperationAbortedException("Operation interrupted by new jog command")))
-            
-            now = self._stopwatch_ellapsed_s()
-            if self._jog_trajectory_generator is None:
-                if self._operational_mode == self._robot_operational_mode["manual_reduced_speed"]:
-                    limits_a_max = np.array([j.joint_limits.reduced_acceleration for j in self._robot_info.joint_info],dtype=np.float64)
-                    limits_v_max = np.array([j.joint_limits.reduced_velocity for j in self._robot_info.joint_info],dtype=np.float64)
-                elif self._operational_mode == self._robot_operational_mode["manual_full_speed"] or \
-                     self._operational_mode == self._robot_operational_mode["cobot"]:
-
-                    limits_a_max = np.array([j.joint_limits.acceleration for j in self._robot_info.joint_info],dtype=np.float64)
-                    limits_v_max = np.array([j.joint_limits.velocity for j in self._robot_info.joint_info],dtype=np.float64)
-                else:
-                    raise RR.InvalidOperationException("Invalid operation mode for jog")
-
-                limits_x_min = np.array([j.joint_limits.lower for j in self._robot_info.joint_info],dtype=np.float64)
-                limits_x_max = np.array([j.joint_limits.upper for j in self._robot_info.joint_info],dtype=np.float64)
-
-                limits = JointTrajectoryLimits(
-                    x_min = limits_x_min,
-                    x_max = limits_x_max,
-                    v_max = limits_v_max,
-                    a_max = limits_a_max,
-                    j_max = None
-                    )
-
-                for i in range(self._joint_count):
-                    if np.abs(max_velocity[i]) > limits.v_max[i]:
-                        raise RR.InvalidArgumentException(
-                            f"max_velocity[{i}] is greater than joint limits ({limits.v_max[i]})")
-                
-                self._jog_trajectory_generator = TrapezoidalJointTrajectoryGenerator(self._joint_count, limits)
-
-                new_req = JointTrajectoryPositionRequest(
-                    current_position = (self._position_command if self._position_command is not None else np.copy(self._joint_position)),
-                    current_velocity = (self._velocity_command if self._velocity_command is not None else np.zeros((self._joint_count,))),
-                    desired_position = joint_position,
-                    desired_velocity = np.zeros((self._joint_count,)),
-                    max_velocity = max_velocity,
-                    speed_ratio = self._speed_ratio
-                )
-
-                self._jog_trajectory_generator.update_desired_position(new_req)
-                self._jog_start_time = now
-            else:
-                jog_trajectory_t = now - self._jog_start_time
-                res, cmd = self._jog_trajectory_generator.get_command(jog_trajectory_t)
-                if not res:
-                    raise RR.InvalidOperationException("Cannot update jog command")
-
-                new_req = JointTrajectoryPositionRequest(
-                    current_position = cmd.command_position,
-                    current_velocity = cmd.command_velocity,
-                    desired_position = joint_position,
-                    desired_velocity = np.zeros((self._joint_count,)),
-                    max_velocity = max_velocity,
-                    speed_ratio = self._speed_ratio
-                )
-
-                self._jog_trajectory_generator.update_desired_position(new_req)
-                self._jog_start_time = now
-
-            if not wait:
-                self._jog_completion_source = None
-                self._node.PostToThreadPool(lambda: handler(None))
-            else:
-                self._jog_completion_handler = handler
-
-    
-    def async_jog_joint(self, joint_velocity, timeout, wait, handler):
-        """
-        Called by client to jog the robot at a specified joint velocity for a specified time. If wait
-        is True, the function will not return to the client until the move is complete. Otherwise will return
-        immediately.
-
-        This function is typically called repeatedly by the client (with wait=False) to drive the robot in response to
-        user input such as a panel button or joystick.
-
-        Robot must be in ``jog`` command mode to call this function.
-
-        This is an asynchronous function, and handler must be called to return result to the client.
-
-        :param joint_velocity: The desired joint velocity position in radians/s
-        :type joint_position: np.ndarray
-        :param timeout: The timeout to run at the specified velocity
-        :type timeout: float
-        :param wait: Wait for completion or return immediately
-        :type wait: bool
-        :param handler: Handler to call when function is complete
-        :type handler: Callable[[],Exception]
-        """
-        with self._lock:
-
-            if self._command_mode != self._robot_command_mode["jog"]:
-                raise RR.InvalidOperationException("Robot not in jog mode")
-
-            if not self._ready:
-                raise RR.OperationAbortedException("Robot not ready")
-
-            if len(joint_velocity) != self._joint_count:
-                raise RR.InvalidArgumentException(f"joint_velocity array must have {self._joint_count} elements")
-
-            if timeout <= 0:
-                raise RR.InvalidArgumentException("Invalid jog timeout specified")
-
-            for i in range(self._joint_count):
-                if abs(joint_velocity[i] > self._robot_info.joint_info[i].joint_limits.reduced_velocity):
-                    raise RR.InvalidArgumentException("Joint velocity exceeds joint limits")
-
-            if self._jog_completion_handler is not None:
-                h = self._jog_completion_handler
-                self._jog_completion_handler = None
-                self._node.PostToThreadPool(
-                    lambda: h(RR.OperationAbortedException("Operation interrupted by new jog command")))
-
-            now = self._stopwatch_ellapsed_s()
-            if self._jog_trajectory_generator is None:
-                if self._operational_mode == self._robot_operational_mode["manual_reduced_speed"]:
-                    limits_a_max = np.array([j.joint_limits.reduced_acceleration for j in self._robot_info.joint_info],dtype=np.float64)
-                    limits_v_max = np.array([j.joint_limits.reduced_velocity for j in self._robot_info.joint_info],dtype=np.float64)
-                elif self._operational_mode == self._robot_operational_mode["manual_full_speed"] or \
-                     self._operational_mode == self._robot_operational_mode["cobot"]:
-                    limits_a_max = np.array([j.joint_limits.acceleration for j in self._robot_info.joint_info],dtype=np.float64)
-                    limits_v_max = np.array([j.joint_limits.velocity for j in self._robot_info.joint_info],dtype=np.float64)
-                else:
-                    raise RR.InvalidOperationException("Invalid operation mode for jog")
-
-                limits_x_min = np.array([j.joint_limits.lower for j in self._robot_info.joint_info],dtype=np.float64)
-                limits_x_max = np.array([j.joint_limits.upper for j in self._robot_info.joint_info],dtype=np.float64)
-                                
-                limits = JointTrajectoryLimits(
-                    x_min = limits_x_min,
-                    x_max = limits_x_max,
-                    v_max = limits_v_max,
-                    a_max = limits_a_max,
-                    j_max = None
-                )
-
-                self._jog_trajectory_generator = TrapezoidalJointTrajectoryGenerator(self._joint_count, limits)
-
-                new_req = JointTrajectoryVelocityRequest(
-                    current_position = (self._position_command if self._position_command is not None else np.copy(self._joint_position)),
-                    current_velocity = (self._velocity_command if self._velocity_command is not None else np.zeros((self._joint_count,))),
-                    desired_velocity = joint_velocity,
-                    speed_ratio = self._speed_ratio,
-                    timeout = timeout
-                )
-
-                self._jog_trajectory_generator.update_desired_velocity(new_req)
-                self._jog_start_time = now
-            else:
-                jog_trajectory_t = now - self._jog_start_time
-                res, cmd = self._jog_trajectory_generator.get_command(jog_trajectory_t)
-                if not res:
-                    raise RR.InvalidOperationException("Cannot update jog command")
-
-                new_req = JointTrajectoryVelocityRequest(
-                    current_position = cmd.command_position,
-                    current_velocity = cmd.command_velocity,
-                    desired_velocity = joint_velocity,
-                    timeout = timeout,
-                    speed_ratio = self._speed_ratio
-                )
-
-                self._jog_trajectory_generator.update_desired_velocity(new_req)
-                self._jog_start_time = now
-
-            if not wait:
-                self._jog_completion_source = None
-                self._node.PostToThreadPool(lambda: handler(None))
-            else:
-                self._jog_completion_handler = handler
-
-    @property
-    def robot_info(self):
-        """
-        Returns the current ``RobotInfo`` structure. The ``RobotInfo`` structure will be updated with tool
-        and payload information as it changes.
-
-        :return: The populated RobotInfo structure
-        :rtype: RobotInfo
-        """
-        with self._lock:
-            
-            for i in range(len(self._robot_info.chains)):
-                self._robot_info.chains[i].current_tool = self._current_tool[i]
-                self._robot_info.chains[i].current_payload = self._current_payload[i]
-                if self._robot_info.chains[i].extended is None:
-                    self._robot_info.chains[i].extended = dict()
-                self._robot_info.chains[i].extended["current_payload_pose"] = \
-                    RR.VarValue(self._current_payload_pose[i], "com.robotraconteur.geometry.Pose") \
-                    if self._current_payload_pose[i] is not None else None
-                
-            return self._robot_info
-
-    def execute_trajectory(self, trajectory):
-        """
-        Called by the client to execute a trajectory. Must be in ``trajectory`` command mode.
-
-        This function returns a generator. The client must call ``Next()`` repeatedly on the generator
-        until the trajectory is complete.
-
-        The first waypoint on the trajectory must be reasonably close to the current robot position.
-
-        :param trajectory: The trajectory to execute
-        :type trajectory: JointTrajectory
-        :return: The trajectory generator, that must have ``Next()`` called repeatedly to execute trajectory
-        :rtype: TrajectoryStatus{generator}
-        """
-        owner_ep = RR.ServerEndpoint.GetCurrentEndpoint()
-
-        with self._lock:
-            speed_ratio = self._speed_ratio
-            current_joint_pos = np.copy(self._joint_position)
-
-        interp = JointTrajectoryInterpolator(self._robot_info)
-        interp.load_trajectory(trajectory, speed_ratio)
-
-        res, joint_pos1, _ = interp.interpolate(0)
-        assert res
-
-        if np.any(np.abs(current_joint_pos - joint_pos1) > self._trajectory_error_tol):
-            raise RR.InvalidArgumentException("Starting waypoint too far from current joint positions")
-
-        with self._lock:
-            if self._command_mode != self._robot_command_mode["trajectory"]:
-                raise RR.InvalidOperationException("Robot must be in trajectory mode to execut trajectory")
-
-            traj_task = None
-
-            if self._active_trajectory is None:
-                traj_task = TrajectoryTask(self, interp, False, owner_ep)
-                self._active_trajectory = traj_task
-            else:
-                traj_task = TrajectoryTask(self, interp, True, owner_ep)
-                self._queued_trajectories.append(traj_task)
-
-            return traj_task
-
-    def _cancel_trajectory(self, trajectory):
-        """
-        Cancel a trajectory that is in the queue. Called from the trajectory generator if ``Close()`` is called.
-        """
-
-        with self._lock:
-            if trajectory is self._active_trajectory:
-                self._active_trajectory = None
-                for t in self._queued_trajectories:
-                    t._cancelled_in_queue()
-                self._queued_trajectories.clear()
-            else:
-                for i in range(len(self._queued_trajectories)):
-                    if trajectory is self._queued_trajectories[i]:
-                        t_index = i
-                        break
-                
-                if t_index >= 0:
-                    for i in range(len(self._queued_trajectories)-1, t_index, -1):
-                        self._queued_trajectories[i]._cancelled_in_queue()
-                        self._queued_trajectories.pop(i)
-                    self._queued_trajectories.pop(t_index)
-
-    def _abort_trajectory(self, trajectory):
-        """
-        Aborts trajectory and all trajectories by dropping to ``halt`` command made. Called by trajectory
-        generater if ``Abort()`` is called.
-        """
-        self._command_mode = self._robot_command_mode["halt"]
-
-    @property
-    def speed_ratio(self):
-        """
-        Get or set the speed ratio. Can be used to reduce or increase speed of trajectory and other operations.
-        :param value: New speed ratio. Must be between 0.1 and 10
-        :type value: float
-        """
-        return self._speed_ratio
-
-    @speed_ratio.setter
-    def speed_ratio(self, value):
-        if value < 0.1 or value > 10:
-            raise RR.InvalidArgumentException("Invalid speed_ratio")
-
-        self._speed_ratio = value
-
-    @property
-    def operational_mode(self):
-        """Return the current operational mode of the controller, if available"""
-        return self._operation_mode
-
-    def controller_state(self):
-        """Return the current state of the vendor robot controller, if available"""
-        return self._controller_state
-
-    def current_errors(self):
-        """Returns currently reported errors, if available"""
-        return []
-
-    def jog_cartesian(self, velocity, timeout, wait):
-        """
-        Called by client to jog the robot at a specified cartesian velocity for a specified time. If wait
-        is True, the function will not return to the client until the move is complete. Otherwise will return
-        immediately.
-
-        This function is typically called repeatedly by the client (with wait=False) to drive the robot in response to
-        user input such as a panel button or joystick.
-
-        Robot must be in ``jog`` command mode to call this function.
-
-        This is an asynchronous function, and handler must be called to return result to the client.
-
-        :param velocity: The desired end effector spatial velocity position in meters/s,radians/s
-        :type joint_position: SpatialVelocity
-        :param timeout: The timeout to run at the specified velocity
-        :type timeout: float
-        :param wait: Wait for completion or return immediately
-        :type wait: bool
-        :param handler: Handler to call when function is complete
-        :type handler: Callable[[],Exception]
-        """
-        raise RR.NotImplementedException("Not implemented")
-
-    def async_home(self, handler):
-        """
-        Called by client to home the robot. Behavior is device specific.
-
-        Robot must be in ``homing`` command mode to call this function.
-
-        :param handler: Handler to call when function is complete
-        :type handler: Callable[[],Exception]
-        """
-        raise RR.NotImplementedException()
-
-    def async_getf_signal(self, signal_name, handler):
-        """Get the value of a signal. Optionally implemented by subclass"""
-        raise RR.NotImplementedException()
-
-    def async_setf_signal(self, signal_name, value, handler):
-        """Set the value of a signal. Optionally implemented by subclass"""
-        raise RR.NotImplementedException()
-
-    def tool_attached(self, chain, tool):
-        """
-        Called by client to notify the driver that a tool has been attached. TCP is used to compute endpoint position
-        and velocity. Implementing class may also update the vendor robot controller if necessary.
-
-        :param chain: The kinematic chain the tool has been attached
-        :type chain: int
-        :param tool: The ToolInfo structure of the tool, specified by the client
-        :type tool: ToolInfo
-        """
-        if tool is None:
-            raise RR.NullValueException("Tool cannot be null")
-
-        if chain > 0 or not (chain < len(self._current_tool)):
-            raise RR.InvalidArgumentException(f"Invalid kinematic chain {chain} for tool")
-
-        with self._lock:
-            if self._current_tool[chain] is not None:
-                raise RR.InvalidArgumentException(f"Tool already attached to kinematic chain {chain}")
-
-            self._current_tool[chain] = tool
-
-            try:
-                device_name = tool.device_info.device.name
-            except:
-                traceback.print_exc()
-                device_name = ""
-
-            self.tool_changed.fire(chain, device_name)
-            self._config_seqno+=1
-
-    def tool_detached(self, chain, tool_name):
-        """
-        Called by client to notify the driver that a tool has been detached. Payloads must be detached before
-        the tool can be detached.
-
-        :param payload_name: The name of the tool that was detached
-        :type payload_name: str
-        """
-
-        if chain > 0 or not (chain < len(self._current_tool)):
-            raise RR.InvalidArgumentException(f"Invalid kinematic chain {chain} for tool")
-
-        with self._lock:
-            if self._current_tool[chain] is None:
-                raise RR.InvalidArgumentException(f"Tool not attached to kinematic chain {chain}")
-
-            if self._current_payload[chain] is not None:
-                raise RR.InvalidArgumentException(f"Cannot remove tool while payload attached")
-
-            if len(tool_name) > 0:                
-                try:
-                    device_name = self._current_tool.device_info.device.name
-                except:
-                    traceback.print_exc()
-                    device_name = ""
-                
-                if device_name != tool_name:
-                    raise RR.InvalidArgumentException(f"Invalid tool name to detach from kinematic chain {chain}")
-            
-            self._current_tool[chain] = None
-
-            self.tool_changed.fire(chain, "")
-            self._config_seqno+=1
-
-    def payload_attached(self, chain, payload, pose):
-        """
-        Called by client to notify the driver that a payload has been attached to the tool. A tool must be attached
-        to attach a payload. The pose between the payload and tool is also specified.
-        
-        Implementing class may also update the vendor robot controller if necessary.
-
-        :param chain: The kinematic chain the tool has been attached
-        :type chain: int
-        :param payload: The PayloadInfo structure of the tool, specified by the client
-        :type tool: PayloadInfo
-        :param pose: The pose of the payload relative to the tool TCP
-        :type pose: com.geometry.Pose
-        """
-        if payload is None:
-            raise RR.NullValueException("Payload cannot be null")
-
-        if chain > 0 or not (chain < len(self._current_payload)):
-            raise RR.InvalidArgumentException(f"Invalid kinematic chain {chain} for payload")
-
-        with self._lock:
-            if self._current_tool[chain] is None:
-                raise RR.InvalidArgumentException(f"No tool attached to kinematic chain {chain}, cannot attach payload")
-
-            if self._current_payload[chain] is not None:
-                raise RR.InvalidArgumentException(f"Payload already attached to kinematic chain {chain}")
-
-            self._current_payload[chain] = payload
-            self._current_payload_pose[chain] = pose
-
-            try:
-                device_name = payload.device_info.device.name
-            except:
-                traceback.print_exc()
-                device_name = ""
-
-            self.payload_changed.fire(chain, device_name)
-            self._config_seqno+=1
-    
-    def payload_detached(self, chain, payload_name):
-        """
-        Called by client to notify the driver that a payload has been detached
-
-        :param payload_name: The name of the payload that was detached
-        :type payload_name: str
-        """
-        
-        if chain > 0 or not (chain < len(self._current_payload)):
-            raise RR.InvalidArgumentException(f"Invalid kinematic chain {chain} for payload")
-
-        with self._lock:
-            
-            if self._current_payload[chain] is None:
-                raise RR.InvalidArgumentException(f"Payload not attached to kinematic chain {chain}")
-
-            if len(payload_name) != 0:
-                try:
-                    device_name = self._current_payload[chain].device_info.device.name
-                except:
-                    traceback.print_exc()
-                    device_name = ""
-            
-                if device_name != payload_name:
-                    raise RR.InvalidArgumentException(f"Invalid payload name to detach from kinematic chain {chain}")
-            
-            self._current_payload[chain] = None
-            self.payload_changed.fire(chain, "")
-            self._config_seqno+=1
-
-    def getf_param(self, param_name):
-        """Get the value of a parameter. Optionally implemented by subclass"""
-        raise RR.InvalidArgumentException("Invalid parameter")
-
-    def setf_param(self, param_name, value):
-        """Set the value of a parameter. Optionally implemented by subclass"""
-        raise RR.InvalidArgumentException("Invalid parameter")
-
-    @property
-    def device_info(self):
-        """Returns the DeviceInfo structure contained in RobotInfo"""
-        return self._robot_info.device_info
-
-    @property
-    def isoch_info(self):
-        """Returns the IsochInfo structure"""
-        iso_info = self._isoch_info_type()
-        iso_info.update_rate = 1.0/self._update_period
-        iso_info.max_downsample = 1000
-
-        iso_info.isoch_epoch = self._stopwatch_epoch
-
-        return iso_info
-
-    @property
-    def isoch_downsample(self):
-        """
-        Get or set the current client isoch_downsample level. By default, the wires and pipes will transmit
-        every timestep. The ``isoch_downsample`` property allows the client to request every ``n`` samples be dropped.
-        For instance, if ``isoch_downsample`` is set to 2, the driver will skip two timesteps, and only transmit on every
-        third timestep. Check ``isoch_info` to determine the native loop update rate in Hz.
-
-        :param value: The downsample level
-        :type value: int
-        
-        """
-        with self._lock:
-            return self._broadcast_downsampler.GetClientDownsample(RR.ServerEndpoint.GetCurrentEndpoint())
-
-    @isoch_downsample.setter
-    def isoch_downsample(self, value):
-        with self._lock:
-            self._broadcast_downsampler.SetClientDownsample(RR.ServerEndpoint.GetCurrentEndpoint(), value)
-
-
-class TrajectoryTaskRes(Enum):
-    unknown = 0
-    ready = 1
-    first_valid_setpoint = 2
-    valid_setpoint = 3
-    trajectory_complete = 4
-    invalid_state = 5
-    joint_tol_error = 6
-    failed = 7
-
-
-class TrajectoryTask:
-
-    def __init__(self, parent, path, queued, owner_ep):
-        self._parent = parent
-        self._path = path
-        self._queued = queued
-        self._owner_ep = owner_ep
-
-        self._next_called = False
-        self._started = False
-        self._start_time = 0
-        self._aborted = False
-        self._cancelled = False
-        self._joint_tol_error = False
-        self._finished = False
-        self._next_wait_handler = []
-        self._queue_wait_handler = []
-        self._success_sent = False
-
-        self._node = parent._node
-        self._trajectory_status_type = \
-            self._node.GetStructureType("com.robotraconteur.robotics.trajectory.TrajectoryStatus")
-
-        self._action_consts = self._node.GetConstants("com.robotraconteur.action")
-        self._action_status_code = self._action_consts["ActionStatusCode"]
-
-        self._traj_t = 0.0
-        self._traj_waypoint = 0
-
-        self._lock = threading.Lock()
-
-    def _call_next_wait_handler(self, err):
-        with self._lock:
-            for c in self._next_wait_handler:
-                self._node.PostToThreadPool(lambda c=c, err=err: c(err))
-            self._next_wait_handler.clear()
-
-    def _call_queue_wait_handler(self,err):
-        with self._lock:
-            for c in self._queue_wait_handler:
-                self._node.PostToThreadPool(lambda c=c, err=err: c(err))
-            self._next_wait_handler.clear()
-
-    def Abort(self):
-        self._aborted = True
-        self._parent._abort_trajectory(self)
-        self._call_next_wait_handler(RR.OperationAbortedException("Trajectory execution aborted"))
-
-    def Close(self):
-        self._cancelled = True
-        self._parent._cancel_trajectory(self)
-        self._call_next_wait_handler(RR.OperationAbortedException("Trajectory execution cancelled"))
-
-    def AsyncNext(self,handler):
-        if self._success_sent:
-            raise RR.StopIterationException("")
-
-        with self._lock:            
-            first_call = not self._next_called
-            self._next_called = True
-
-            if first_call and self._queued:
-                # Report back that we are queued immediately
-
-                ret = self._trajectory_status_type()
-                ret.action_status = self._action_status_code["queued"]
-                ret.trajectory_time = 0
-                ret.current_waypoint = 0
-                ret.seqno = self._parent._state_seqno
-                handler(ret, None)
-                return
-
-            complete_called = [False]
-
-            def complete(err):
-                with self._lock:
-                    if complete_called[0]:
-                        return
-                    complete_called[0] = True
-                if err:
-                    handler(None, err)
-                
-                if not self._started:
-                    # Still queued...
-
-                    ret = self._trajectory_status_type()
-                    ret.action_status = self._action_status_code["queued"]
-                    ret.trajectory_time = 0
-                    ret.current_waypoint = 0
-                    ret.seqno = self._parent._state_seqno
-                    handler(ret, None)
-                    return
-
-                if self._finished:
-                    self._success_sent = True
-                    ret = self._trajectory_status_type()
-                    ret.action_status = self._action_status_code["complete"]
-                    ret.trajectory_time = self._traj_t
-                    ret.current_waypoint = int(self._traj_waypoint)
-                    ret.seqno = self._parent._state_seqno
-                    handler(ret, None)
-                    return
-
-                else:
-                    ret = self._trajectory_status_type()
-                    ret.action_status = self._action_status_code["running"]
-                    ret.trajectory_time = self._traj_t
-                    ret.current_waypoint = int(self._traj_waypoint)
-                    ret.seqno = self._parent._state_seqno
-                    handler(ret,None)
-                    return
-
-            if self._queued:
-                self._next_wait_handler.append(complete)
-                self._queue_wait_handler.append(complete)
-            else:
-                self._next_wait_handler.append(complete)
-
-            timer = self._node.CreateTimer(5, lambda _: complete(None), True)
-            timer.Start()
-
-    def _cancelled_in_queue(self):
-        self._cancelled = True
-        self._call_next_wait_handler(RR.OperationAbortedException("Trajectory cancelled by controller before start"))
-
-    def _invalid_mode(self):
-        self._aborted = True
-        self._call_next_wait_handler(RR.OperationAbortedException("Invalid mode for trajectory execution"))
-
-    
-    def _get_setpoint(self, now, current_joint_pos):
-        if self._cancelled or self._aborted:
-            return TrajectoryTaskRes.failed, None, None, 0.0, 0.0, 0
-
-        first_call = False
-
-        t = 0.0
-
-        if self._next_called:
-            if not self._started:
-                self._start_time = now
-                self._started = True
-                first_call = True
-
-            t = now - self._start_time
-
-        res, joint_pos1, current_waypoint1 = self._path.interpolate(t)
-        if not res:
-            self._call_next_wait_handler(Exception("Trajectory execution failed"))
-            return TrajectoryTaskRes.failed, None, None, 0.0, 0.0, 0
-
-        if np.any(np.abs(current_joint_pos - joint_pos1) > self._parent._trajectory_error_tol):
-            self._call_next_wait_handler(RR.OperationFailedException("Trajectory tolerance failure"))
-            return TrajectoryTaskRes.ready, None, None, 0.0, 0.0, 0
-
-        if not self._next_called:
-            return TrajectoryTaskRes.ready, None, None, 0.0, self._path.max_time, 0
-        
-        if t > self._path.max_time:
-            self._traj_t = t
-            self._traj_waypoint = current_waypoint1
-            self._finished = True
-            self._call_next_wait_handler(None)
-            return TrajectoryTaskRes.trajectory_complete, joint_pos1, None, t, self._path.max_time, current_waypoint1
-
-        if first_call:
-            if self._queued:
-                self._queued = False
-                self._call_queue_wait_handler(None)
-            return TrajectoryTaskRes.first_valid_setpoint, joint_pos1, None, t, self._path.max_time, current_waypoint1
-        else:
-            return TrajectoryTaskRes.valid_setpoint, joint_pos1, None, t, self._path.max_time, current_waypoint1
-
-    #TODO: Add connection test?
-
+# Copyright 2022 Wason Technology, LLC
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""
+Module containing ``AbstractRobot`` class. Robot Raconteur types are shortened for brevity. See 
+``com.robotraconteur.robotics.robot`` robdef ``using`` statements for fully qualified types.
+"""
+
+from enum import Enum
+import traceback
+from turtle import down
+import RobotRaconteur as RR
+RRN = RR.RobotRaconteurNode.s
+from RobotRaconteurCompanion.Util.RobotUtil import RobotUtil
+from RobotRaconteurCompanion.Util.DateTimeUtil import DateTimeUtil
+from RobotRaconteurCompanion.Util.GeometryUtil import GeometryUtil
+from RobotRaconteurCompanion.Util.SensorDataUtil import SensorDataUtil
+import time
+import threading
+import numpy as np
+from abc import ABC, abstractmethod
+
+from .joint_trajectory_interpolator import JointTrajectoryInterpolator
+from .trapezoidal_joint_trajectory_generator import JointTrajectoryLimits, JointTrajectoryPositionRequest, \
+    JointTrajectoryVelocityRequest, JointTrajectoryPositionCommand, TrapezoidalJointTrajectoryGenerator
+
+class AbstractRobot(ABC):
+    """
+    Abstact base class for standard Robot Raconteur robot device drivers. Subclasses implement specific functionality
+    for each robot controller type. Typically, these drivers communicate with the vendor controller. The vender
+    controller may provide the communication method natively, or the vendor controller may need to execute
+    special programs provided by the driver.
+
+    The driver uses a ``RobotInfo`` structure to initialize information about kinematics etc. The __init__
+    function should also be overridden to initialize various instance variables. The ``robot_info`` parameter
+    is typically loaded from a YAML file.
+
+    AbstractRobot uses a real-time loop that periodically calls ``_run_timestep()``, with the period set by 
+    ``_update_period``. ``_run_timestep()`` does the following, some of which the subclass must implement:
+
+    #. Read feedback from driver (must be implemented by subclass).
+         Update ``_joint_position``, ``_joint_velocity`` (optional), ``_joint_effort`` (optional), ``_endpoint_pose``, 
+        ``_endpoint_vel`` (optional), ``_ready``, ``_enabled``, ``_stopped``, ``_error``, ``_estop_source``,
+        ``_last_robot_state``, ``_last_joint_state``, and ``_last_endpoint_state``. These updates may happen
+        outside the loop, when the data is received from the robot. Hold ``_lock`` when updating data if not
+        inside the loop.
+    #. Verify communication by calling ``_verify_communication()``. If ``_last_robot_state``, ``_last_joint_state``,
+        or ``_last_endpoint_state`` exceed ``_communication_timeout`` relative to stopwatch time, set communication
+        failure.
+    #. Verify the current robot state by calling ``_verify_robot_state()
+    #. Fill a joint position or joint velocity command by calling ``_fill_robot_command()``. This will check the
+        current operational mode and commands from the client to generate the next command.
+    #. Fill the robot state structures to return to clients. Calls ``_fill_states()``, ``_fill_state_flags()``,
+        ``_calc_endpoint_poses()``, and ``_calc_endpoint_vels()``
+    #. If a valid command is available, send to the robot using ``_send_robot_command()``. Subclass must implement
+        this function.
+    
+    At a minimum, a driver subclass must fill feedback data from the robot as shown in step 1 above, and must
+    implement ``_send_robot_command()``, ``_send_disable()``, ``_send_enable()``, and ``_send_reset_errors()``.
+    See the example minimal ABB robot driver. Also see abb_robotraconteur_driver_hmp for a more sophisticated driver.    
+
+    :ivar _robot_info: The ``RobotInfo`` structure, initialized from __init__ parameter
+    :ivar _joint_names: The names of the robot joints. Initialized from ``robot_info`` or ``default_joint_count``
+    :ivar _joint_count: The number of robot joints. Initialized from ``robot_info`` or ``default_joint_count``
+    :ivar _robot_uuid: The UUID of the robot. Initialized from the ``robot_info`` structure
+    :ivar _robot_caps: The capability flags of the robot taken from ``RobotCapabilities`` enum. By default initialized
+                       from ``robot_info`, but it is recommended the driver override this value in __init__
+    :ivar _robot_util: Companion ``RobotUtil`` utility class instance
+    :ivar _datetime_util: Companion ``DateTimeUtil`` utility class instance
+    :ivar _geometry_util: Companion ``GeometryUtil`` utility class instance
+    :ivar _sensor_data_util: Companion ``SensorDataUtil`` utility class instance
+    :ivar _pose_dtype: ``com.robotraconteur.geometry.Pose`` numpy dtype
+    :ivar _spatial_velocity_dtype: ``com.robotraconteur.geometry.SpatialVelocity`` numpy dtype
+    :ivar _robot_state_type: ``RobotState`` structure type
+    :ivar _advanced_robot_state_type: ``AdvancedRobotState`` structure type
+    :ivar _robot_state_sensor_data_type: ``RobotStateSensorData`` structure type
+    :ivar _robot_joint_command_type: ``RobotJointCommand`` structure type
+    :ivar _isoch_info_type: ``IsochInfo`` structure type
+    :ivar _robot_consts: Constants from ``com.robotraconteur.robotics.robot``
+    :ivar _robot_capabilities: ``RobotCapabilities`` enum
+    :ivar _robot_command_mode: ``RobotCommandMode`` enum
+    :ivar _robot_operational_mode: ``RobotOperationalMode`` enum
+    :ivar _robot_controller_state: ``RobotControllerState`` enum
+    :ivar _robot_state_flags: ``RobotStateFlags`` enum
+    :ivar _joint_consts: Constants from ``com.robotraconteur.robotics.joints``
+    :ivar _joint_position_units: ``JointPositionUnits`` enum
+    :ivar _joint_effort_units: ``JointEffortUnits`` enum
+    :ivar _uses_homing: Robot uses homing command. Initialized from capabilities flags in ``robot_info``. 
+            Recommended to override in __init__
+    :ivar _has_position_command: Robot has streaming position command. Initialized from capabilities flags in 
+            ``robot_info``. Recommended to override in __init__
+    :ivar _has_velocity_command: Robot has streaming velocity command. Initialized from capabilities flags in 
+            ``robot_info``. Recommended to override in __init__
+    :ivar _has_jog_command: Robot has jog command. Initialized from capabilities flags in 
+            ``robot_info``. Recommended to override in __init__
+    :ivar _current_tool: Currently attached robot tool. Array, one entry per chain. Initialized from ``robot_info``,
+                            updated using ``tool_attached()`` and ``tool_detached()``
+    :ivar _current_payload: Currently attached payload. Array, one entry per chain. Initialized from ``robot_info``,
+                            updated using ``payload_attached()`` and ``payload_detached()``
+    :ivar _current_payload_pose: Pose of currently attached payload relative to tool TCP. Array, one entry per chain. 
+                                    Initialized from ``robot_info``, updated using ``payload_attached()`` 
+                                    and ``payload_detached()``
+    :ivar _keep_going: Boolean flag to stop loop
+    :ivar _update_period: The update period of the loop (aka timestep). Should be set in __init__
+    :ivar _speed_ratio: The current speed ratio. Set using ``speed_ratio`` property
+    :ivar _jog_joint_limit: The maximum joint distance allowed during a jog command
+    :ivar _trajectory_error_tol: The maximum error allowed between command and robot position during trajectory 
+                                    execution
+    :ivar _command_mode: The current command mode. Set using ``command_mode`` property, and updated during operation
+                            due to errors or other events.
+    :ivar _operational_mode: The operational mode of the vendor robot controller, using values from 
+                                ``RobotOperationalMode`` enum. Should be
+                                updated every timestep if available. Set ``_base_set_operational_mode`` to False
+                                if used.
+    :ivar _controller_state: The controller state of the vendor robot controller, using values from 
+                                ``RobotOperationalMode`` enum. Should be
+                                updated every timestep if available. Set ``_base_set_controller_state`` to False
+                                if used.
+    :ivar _joint_position: Current joint position based on feedback in radians (or meters). This value should be
+                            updated every timestep using robot feedback.
+    :ivar _joint_velocity: Current joint velocity based on feedback in radians/s (or meters/s). This value should be
+                            updated every timestep using robot feedback. Leave as empty array if velocity feedback
+                            not available.
+    :ivar _joint_effort: Current joint effort based on feedback in Nm (or N). This value should be
+                            updated every timestep using robot feedback. Leave as empty array if effort feedback
+                            not available.
+    :ivar _position_command: Current position command. Set by the subclass after issuing command to robot. This
+                                value is used for client state information.
+    :ivar _velocity_command: Current velocity command. Set by the subclass after issuing command to robot. This
+                                value is used for client state information.
+    :ivar _endpoint_pose: Array of endpoint poses, one entry per chain. Update every timestep. Units should be in 
+                            meters, quaternions, relative to world or base of robot.
+    :ivar _endpoint_vel: Array of endpoint velocities, one entry per chain. Update every timestep. Units should be in 
+                            meters/s, radians/s, relative to world or base of robot.
+    :ivar _last_robot_state: The stopwatch time in seconds of the last state update received from the robot. 
+                                Must be updated to avoid communication timeout.
+    :ivar _last_joint_state: The stopwatch time in seconds of the last joint position update received from the robot. 
+                                Must be updated to avoid communication timeout.
+    :ivar _last_endpoint_state: The stopwatch time in seconds of the last endpoint update received from the robot. 
+                                Must be updated to avoid communication timeout.
+    :ivar _state_seqno: Counter of number of loop iterations executed (sequence number)
+    :ivar _homed: Set to True if robot is homed. Only valid if robot has homing capability
+    :ivar _ready: Set to True if robot is ready to move. Should be updated every timestep
+    :ivar _enabled: Set to True if robot is enabled with motors on. Should be updated every timestep. Robot may
+                    be enabled but not ready
+    :ivar _stopped: Set to True if robot is stopped due to an estop. Should be updated every timestep
+    :ivar _error: Set to True if robot is in an error state. Should be updated every timestep. Errors are reset by
+                    switching to halt more, calling ``reset_errors()``, and/or clearing the error on the vendor
+                    controller, in escalating levels of severity.
+    :ivar _estop_source: The source of the estop, using values from ``RobotStateFlags``
+    :ivar _communication_failure: Set by ``_verify_communication`` based on ``_communication_timeout``
+    :ivar _communication_timeout: Communication timeout in seconds. If no updates are received from the controller
+                                  within the communication timeout, an error condition is set
+    :ivar _broadcast_downsampler: Broadcast downsampler used by all wires and pipes to control data rate sent to client
+    :ivar position_command: Wire populated by Robot Raconteur to receive streaming position commands. Only used 
+                            in ``position_command`` command mode
+    :ivar velocity_command: Wire populated by Robot Raconteur to receive streaming position commands. Only used 
+                            in ``velocity_command`` command mode
+    :ivar _wires_ready: Set to True when wires and pipes have been initialized by Robot Raconteur
+    :ivar _config_seqno: The sequence number returned as part of ``RobotInfo``. Incremented as tools and payloads
+                            are attached/detached.
+    :ivar _base_set_operational_mode: If True, abstract robot will set ``_operational_mode`` to a default value.
+                                        Set to False if driver will update ``_operational_mode``
+    :ivar _base_set_controller_state: If True, abstract robot will set ``_controller_state`` to a default value.
+                                        Set to False if driver will update ``_controller_state``
+    :ivar _lock: Lock to hold when updating data to prevent race conditions
+
+    :param robot_info: The ``RobotInfo`` structure for the robot
+    :param default_joint_count: The default number of joints for the robot
+    :param node: The Robot Raconteur node for the driver
+    """
+    def __init__(self, robot_info, default_joint_count, node = None ):
+        super().__init__()
+
+        if node is None:
+            self._node = RRN
+        else:
+            self._node = node
+
+        self._robot_info = robot_info
+        if robot_info.joint_info is not None:
+            j_names = []
+            for j_info in robot_info.joint_info:
+                j_names.append(j_info.joint_identifier.name)
+            self._joint_names = j_names
+        else:
+            assert default_joint_count > 0, "Joints must be specified in RobotInfo structure"
+            self._joint_names = [f"joint_{x}" for x in range(default_joint_count)]
+        
+        self._joint_count = len(self._joint_names)
+
+        self._robot_uuid = robot_info.device_info.device.uuid
+
+        self._robot_caps = robot_info.robot_capabilities
+
+        self._robot_util = RobotUtil(self._node)
+        self._datetime_util = DateTimeUtil(self._node)
+        self._geometry_util = GeometryUtil(self._node)
+        self._sensor_data_util = SensorDataUtil(self._node)
+
+        self._pose_dtype = self._node.GetNamedArrayDType("com.robotraconteur.geometry.Pose")
+        self._spatial_velocity_dtype = self._node.GetNamedArrayDType("com.robotraconteur.geometry.SpatialVelocity")
+        self._robot_state_type = self._node.GetStructureType("com.robotraconteur.robotics.robot.RobotState")
+        self._advanced_robot_state_type = self._node.GetStructureType("com.robotraconteur.robotics.robot.AdvancedRobotState")
+        self._robot_state_sensor_data_type = self._node.GetStructureType("com.robotraconteur.robotics.robot.RobotStateSensorData")
+        self._robot_joint_command_type = self._node.GetStructureType("com.robotraconteur.robotics.robot.RobotJointCommand")
+        self._isoch_info_type = self._node.GetStructureType("com.robotraconteur.device.isoch.IsochInfo")
+
+        self._robot_consts = self._node.GetConstants("com.robotraconteur.robotics.robot")
+        self._robot_capabilities = self._robot_consts["RobotCapabilities"]
+        self._robot_command_mode = self._robot_consts["RobotCommandMode"]
+        self._robot_operational_mode = self._robot_consts["RobotOperationalMode"]
+        self._robot_controller_state = self._robot_consts["RobotControllerState"]
+        self._robot_state_flags = self._robot_consts["RobotStateFlags"]
+
+        self._joint_consts = self._node.GetConstants("com.robotraconteur.robotics.joints")
+        self._joint_position_units = self._joint_consts["JointPositionUnits"]
+        self._joint_effort_units = self._joint_consts["JointEffortUnits"]
+
+        self._uses_homing = (self._robot_caps & self._robot_capabilities["homing_command"]) != 0
+        self._has_position_command = (self._robot_caps & self._robot_capabilities["position_command"]) != 0
+        self._has_velocity_command = (self._robot_caps & self._robot_capabilities["velocity_command"]) != 0
+        self._has_jog_command = (self._robot_caps & self._robot_capabilities["jog_command"]) != 0
+
+        try:
+            self._rox_robots = []
+            for chain_i in range(len(self._robot_info.chains)):
+                self._rox_robots.append(self._robot_util.robot_info_to_rox_robot(self._robot_info,chain_i))
+        except:
+            traceback.print_exc()
+            raise ValueError("invalid robot_info, could not populate GeneralRoboticsToolbox.Robot")
+
+        self._current_tool = [None]*len(self._robot_info.chains)
+        self._current_payload = [None]*len(self._robot_info.chains)
+        self._current_payload_pose = [None]*len(self._robot_info.chains)
+
+        for i in range(len(self._robot_info.chains)):
+            if self._robot_info.chains[i].current_tool is not None:
+                self._current_tool[i] = self._robot_info.chains[i].current_tool
+
+            if self._robot_info.chains[i].current_payload is not None:
+                self._current_payload[i] = self._robot_info.chains[i].current_payload
+
+        for i in range(self._joint_count):
+            limits = robot_info.joint_info[i].joint_limits
+            assert limits.velocity > 0, f"Invalid joint velocity for joint {i}"
+            if limits.reduced_velocity <= 0:
+                limits.reduced_velocity = limits.velocity
+
+            assert limits.acceleration > 0, f"Invalid joint acceleration for joint {i}"
+            if limits.reduced_acceleration <= 0:
+                limits.reduced_acceleration = limits.acceleration
+
+        self._keep_going = False
+
+        self._stopwatch_epoch = None
+        self._stopwatch_start = None
+
+        self._loop_thread = None
+        self._update_period = 0.01
+
+        self._wait_event = threading.Event()
+
+        self._last_robot_state = 0
+        self._last_joint_state = 0
+        self._last_endpoint_state = 0
+
+        self._state_seqno = 0
+
+        self._speed_ratio = 1.0
+
+        self._jog_joint_limit = np.deg2rad(1000.)
+        self._trajectory_error_tol = np.deg2rad(5.)
+
+        self._command_mode = self._robot_command_mode["halt"]
+        self._operational_mode = self._robot_operational_mode["manual_reduced_speed"]
+        self._controller_state = self._robot_operational_mode["undefined"]
+
+        self._joint_position = np.zeros((0,))
+        self._joint_velocity = np.zeros((0,))
+        self._joint_effort = np.zeros((0,))
+
+        self._position_command = None
+        self._velocity_command = None
+
+        self._endpoint_pose = []
+        self._endpoint_vel = []
+
+        self._homed = False
+        self._ready = False
+        self._enabled = False
+        self._stopped = False
+        self._error = False
+        self._estop_source = 0
+
+        self._communication_failure = True
+        self._communication_timeout = 0.25
+
+        self._broadcast_downsampler = None
+
+        self._wire_position_command_sent = False
+        self._wire_velocity_command_sent = False
+        self._wire_position_command_last_seqno = 0
+        self._wire_velocity_command_last_seqno = 0
+        self._wire_position_command_last_ep = 0
+        self._wire_velocity_command_last_ep = 0
+
+        self._trajectory_valid = False
+        self._trajectory_current_time = 0
+        self._trajectory_max_time = 0
+        self._trajectory_waypoint = 0
+
+        self._lock = threading.Lock()
+
+        self._wires_ready = False
+
+        self._active_trajectory = None
+        self._queued_trajectories = []
+
+        self._jog_start_time = 0.
+        self._jog_trajectory_generator = None
+        self._jog_completion_handler = None
+
+        self._config_seqno = 1
+
+        self._base_set_operational_mode = True
+        self._base_set_controller_state = True
+
+    def RRServiceObjectInit(self, context, service_path):
+        self.robot_state_sensor_data.MaxBacklog = 3
+
+        self._broadcast_downsampler = RR.BroadcastDownsampler(context, 0)
+        self._broadcast_downsampler.AddPipeBroadcaster(self.robot_state_sensor_data)
+        self._broadcast_downsampler.AddWireBroadcaster(self.robot_state)
+        self._broadcast_downsampler.AddWireBroadcaster(self.advanced_robot_state)
+        self._broadcast_downsampler.AddWireBroadcaster(self.device_clock_now)
+
+        self._wires_ready = True
+
+    def _perf_counter(self) -> float:
+        """
+        System performance counter in seconds. This counter is not relative to real time clock.
+
+        :return: Performance counter time in seconds
+        """
+        return time.perf_counter()
+
+    def _stopwatch_ellapsed_s(self) -> float:
+        """
+        Stopwatch time in seconds. Relative to start of driver loop.
+
+        :return: Stopwatch time in seconds
+        """
+        return self._perf_counter() - self._stopwatch_start
+
+    def _start_robot(self):
+        """
+        Start the robot driver loop
+        """
+
+        self._stopwatch_epoch = self._datetime_util.TimeSpec2Now()
+        self._stopwatch_start = self._perf_counter()
+
+        self._keep_going = True
+        self._loop_thread = threading.Thread(target = self._loop_thread_func)
+        self._loop_thread.daemon = True
+        self._loop_thread.start()
+
+    def _stop_robot(self):
+        """
+        Stop the robot driver loop
+        """
+        self._keep_going = False
+        self._loop_thread.join()
+
+    def _loop_thread_func(self):
+        """
+        Loop thread entry function. This function runs the loop, and calls ``run_timestep()`` periodically at
+        ``_update_period`` specified in seconds.
+        """
+
+        next_wait = self._stopwatch_ellapsed_s()
+        now = next_wait
+
+        while self._keep_going:
+            
+            now = self._stopwatch_ellapsed_s()
+            self._run_timestep(now)
+
+
+            while True:
+                next_wait += self._update_period
+                if next_wait > now:
+                    break
+
+            while True:
+                now = self._stopwatch_ellapsed_s()
+                if now >= next_wait:
+                    break
+                time.sleep(next_wait-now)
+
+            
+    def _close(self):
+        """
+        Close the driver, stop the loop
+        """
+        self._keep_going = False
+        try:
+            self._loop_thread.join(timeout=1)
+        except:
+            pass
+
+    
+
+    def _run_timestep(self, now):
+        """
+        Called by loop each timestep at ``_update_timestep`` period in seconds
+
+        :param now: stopwatch time in seconds
+        """
+        res = False
+        joint_pos_cmd = None
+        joint_vel_cmd = None
+
+        rr_robot_state = None
+        rr_advanced_robot_state = None
+        rr_state_sensor_data = None
+        downsampler_step = None
+
+        with self._lock:
+            if self._wires_ready:
+                downsampler_step = RR.BroadcastDownsamplerStep(self._broadcast_downsampler)
+
+            self._state_seqno += 1
+
+            res = self._verify_communication(now)
+            res = res and self._verify_robot_state(now)
+            res_fill, joint_pos_cmd, joint_vel_cmd = self._fill_robot_command(now)
+            res = res and res_fill
+
+            rr_robot_state, rr_advanced_robot_state, rr_state_sensor_data = self._fill_states(now)
+
+        if res:
+            self._send_robot_command(now, joint_pos_cmd, joint_vel_cmd)
+
+        if downsampler_step:
+            with downsampler_step:
+                self._send_states(now, rr_robot_state, rr_advanced_robot_state, rr_state_sensor_data)
+
+    def _fill_state_flags(self, now):
+        """
+        Fill ``_robot_state_flags`` based on current state of driver. Called by the loop each timestep to update 
+        driver state
+
+        :param now: stopwatch time in seconds
+        """
+
+        f = 0
+        if self._communication_failure:
+            f |= self._robot_state_flags["communication_failure"]
+            return f
+
+        if self._error:
+            f |= self._robot_state_flags["error"]
+
+        if self._stopped:
+            f |= self._robot_state_flags["estop"]
+
+            if self._estop_source == 0:
+                pass
+            elif self._estop_source == 1:
+                f |= self._robot_state_flags["estop_button1"]
+            elif self._estop_source == 2:
+                f |= self._robot_state_flags["estop_other"]
+            elif self._estop_source == 3:
+                f |= self._robot_state_flags["estop_fault"]
+            elif self._estop_source == 4:
+                f |= self._robot_state_flags["estop_internal"]
+        
+        if self._enabled:
+            f |= self._robot_state_flags["enabled"]
+
+        if self._ready:
+            f |= self._robot_state_flags["ready"]
+
+        if self._uses_homing:
+            if self._homed:
+                f |= self._robot_state_flags["homed"]
+            else:
+                f |= self._robot_state_flags["homing_required"]
+
+        if self._wire_position_command_sent:
+            f |= self._robot_state_flags["valid_position_command"]
+
+        if self._wire_velocity_command_sent:
+            f |= self._robot_state_flags["valid_velocity_command"]
+
+        if self._trajectory_valid:
+            f |= self._robot_state_flags["trajectory_running"]
+
+        return f
+
+    def _calc_endpoint_pose(self, chain):
+        """
+        Compute endpoint pose for specified chain. By default uses ``_endpoint_pose[chain]`` and transforms
+        to the TCP of ``self._current_tool[chain]``. If the robot reports the endpoint position with the tool
+        transform applied, this should return ``self._endpoint_pose[chain]``
+
+        Called by the loop each timestep to update driver state.
+
+        :param chain: The chain index, always 0 for single arm driver
+        :rtype: com.robotraconteur.geometry.Pose
+        :return: The pose of the end effector
+        """
+
+        # CALL LOCKED!
+        if self._current_tool[chain] is None:
+            return self._endpoint_pose[chain]
+
+        endpoint_transform = self._geometry_util.pose_to_rox_transform(self._endpoint_pose[chain])
+        tool_transform = self._geometry_util.transform_to_rox_transform(self._current_tool[chain].tcp)
+        res = endpoint_transform * tool_transform
+        return self._geometry_util.rox_transform_to_pose(res)
+
+    def _calc_endpoint_poses(self):
+        """
+        Compute the endpoints of all chains. Calls ``_calc_endpoint_pose()`` for each chain.
+
+        Called by the loop each timestep to update driver state.
+
+        :rtype: com.robotraconteur.geometry.Pose[]
+        :return: Array of all chain poses. Single element array for single arm drivers
+        """
+        if self._endpoint_pose is None:
+            return np.zeros((0,), dtype=self._pose_dtype)
+        n = len(self._endpoint_pose)
+        o = np.zeros((n,), dtype=self._pose_dtype)
+        for i in range(n):
+            o[i] = self._calc_endpoint_pose(i)
+        return o
+
+    def _calc_endpoint_vel(self, chain):
+        """
+        Compute spatial velocity for specified chain. By default uses ``_endpoint_vel[chain]`` and applies TCP
+        transform of ``self._current_tool[chain]``. If the robot reports the endpoint position with the tool
+        transform applied, this should return ``self._endpoint_vel[chain]``
+
+        Called by the loop each timestep to update driver state.
+
+        :param chain: The chain index, always 0 for single arm driver
+        :rtype: com.robotraconteur.geometry.SpatialVelocity
+        :return: The spatial velocity (6x1) of the end effector
+        """
+        # CALL LOCKED!
+
+        if self._current_tool[chain] is None:
+            return self._endpoint_vel[chain]
+
+        endpoint_vel = self._geometry_util.spatial_velocity_to_array(self._endpoint_vel).flatten()
+        endpoint_vel_ang = endpoint_vel[0:3]
+        endpoint_vel_lin = endpoint_vel[3:7]
+        current_tool_p = self._geometry_util.point_to_xyz(self._current_tool[chain].tcp["translation"])
+
+        endpoint_transform = self._geometry_util.pose_to_rox_transform(self._endpoint_pose[chain])
+
+        
+        vel = endpoint_vel_lin + np.cross(endpoint_vel_ang, np.matmul(endpoint_transform.R, current_tool_p))
+
+        return self._geometry_util.array_to_spatial_acceleration(np.concatenate((endpoint_vel_ang, vel)))
+
+    def _calc_endpoint_vels(self):
+        """
+        Compute the spatial velocity of all chains. Calls ``_calc_endpoint_vel()`` for each chain.
+
+        Called by the loop each timestep to update driver state.
+
+        :rtype: com.robotraconteur.geometry.SpatialVelocity[]
+        :return: Array of all chain spatial velocities. Single element array for single arm drivers
+        """
+
+        if self._endpoint_vel is None:
+            return np.zeros((0,),dtype=self._spatial_velocity_dtype)
+
+        n = len(self._endpoint_vel)
+        o = np.zeros((n,),dtype=self._spatial_velocity_dtype)
+        for i in range(n):
+            o[i] = self._calc_endpoint_vel(i)
+        
+        return o
+
+    def _fill_states(self, now):
+        """
+        Fill the ``RobotState``, ``AdvancedRobotState``, and ``RobotStateSensorData`` structures based on
+        current driver state.
+
+        Called by the loop each timestep to fill data to send to clients.
+
+        :param now: stopwatch time in seconds
+        :rtype: Tuple[RobotState,AdvancedRobotState,RobotStateSensorData]
+        """
+        ts = self._datetime_util.TimeSpec3Now()
+
+        rob_state = self._robot_state_type()               
+        rob_state.ts = ts
+        rob_state.seqno = self._state_seqno
+        rob_state.command_mode = self._command_mode
+        rob_state.operational_mode = self._operational_mode
+        rob_state.controller_state = self._controller_state
+
+        flags = self._fill_state_flags(now)
+
+        rob_state.robot_state_flags = flags
+
+        rob_state.joint_position = np.copy(self._joint_position)
+        rob_state.joint_velocity = np.copy(self._joint_velocity)
+        rob_state.joint_effort = np.copy(self._joint_effort)
+        rob_state.joint_position_command = self._position_command if self._position_command is not None \
+                else np.zeros((0,))
+        rob_state.joint_velocity_command = self._velocity_command if self._velocity_command is not None \
+                else np.zeros((0,))
+        rob_state.kin_chain_tcp = self._calc_endpoint_poses()
+        rob_state.kin_chain_tcp_vel = self._calc_endpoint_vels()
+        rob_state.trajectory_running = self._trajectory_valid
+
+        a_rob_state = self._advanced_robot_state_type()
+        a_rob_state.ts = ts
+        a_rob_state.seqno = rob_state.seqno
+        a_rob_state.command_mode = rob_state.command_mode
+        a_rob_state.operational_mode = rob_state.operational_mode
+        a_rob_state.controller_state = rob_state.controller_state
+        a_rob_state.robot_state_flags = rob_state.robot_state_flags
+        a_rob_state.joint_position = rob_state.joint_position
+        a_rob_state.joint_velocity = rob_state.joint_velocity
+        a_rob_state.joint_effort = rob_state.joint_effort
+        a_rob_state.joint_position_command = rob_state.joint_position_command
+        a_rob_state.joint_velocity_command = rob_state.joint_velocity_command
+        a_rob_state.kin_chain_tcp = rob_state.kin_chain_tcp
+        a_rob_state.kin_chain_tcp_vel = rob_state.kin_chain_tcp_vel
+        a_rob_state.trajectory_running = rob_state.trajectory_running
+        a_rob_state.joint_position_units = [self._joint_position_units["radian"]]*self._joint_count
+        a_rob_state.joint_effort_units = [self._joint_effort_units["newton_meter"]]*self._joint_count
+        a_rob_state.trajectory_running = self._trajectory_valid
+        a_rob_state.trajectory_time = self._trajectory_current_time
+        a_rob_state.trajectory_max_time = self._trajectory_max_time
+        a_rob_state.trajectory_current_waypoint = self._trajectory_waypoint
+        a_rob_state.config_seqno = self._config_seqno
+
+        sensor_data_header = self._sensor_data_util.FillSensorDataHeader(self._robot_info.device_info, self._state_seqno)
+
+        sensor_data = self._robot_state_sensor_data_type()
+        sensor_data.data_header = sensor_data_header
+        sensor_data.robot_state = a_rob_state
+
+        return rob_state, a_rob_state, sensor_data
+
+
+    def _send_states(self, now, rr_robot_state, rr_advanced_robot_state, rr_state_sensor_data):
+        """
+        Sends the states to the Robot Raconteur clients using broadcast wires
+
+        Called by the loop each timestep to send data to clients.
+
+        :param now: stopwatch time in seconds
+        :param rr_robot_state: populated RobotState instance
+        :param rr_advanced_robot_state: populated AdvancedRobotState instance
+        :param rr_state_sensor_data: populated RobotStateSensorData instance
+        """
+        if not self._wires_ready:
+            return
+             
+        self.robot_state.OutValue = rr_robot_state
+        self.advanced_robot_state.OutValue = rr_advanced_robot_state
+        self.robot_state_sensor_data.AsyncSendPacket(rr_state_sensor_data, lambda: None)
+        self.device_clock_now.OutValue = self._datetime_util.FillDeviceTime(self._robot_info.device_info, self._state_seqno)
+
+    @abstractmethod
+    def _send_disable(self, handler):
+        """
+        Called to send a disable command to the robot. Only valid if driver has ``software_enable`` capability.
+        Implementing class must override if used. ``handler`` must be called to complete the asynchronous request.
+        """
+        pass
+
+    def async_disable(self, handler):
+        """Called by client to request robot disable. Calls ``_send_disable()``"""
+        self._send_disable(handler)
+
+    @abstractmethod
+    def _send_enable(self, handler):
+        """
+        Called to send an enable command to the robot. Only valid if driver has ``software_enable`` capability.
+        Implementing class must override if used. ``handler`` must be called to complete the asynchronous request.
+        """
+        pass
+
+    def async_enable(self, handler):
+        """Called by client to request robot enable. Calls ``_send_enable()``"""
+        self._send_enable(handler)
+
+    @abstractmethod
+    def _send_reset_errors(self, handler):
+        """
+        Called to send an reset errors command to the robot. Only valid if driver has ``software_reset_errors`` 
+        capability. Implementing class must override if used. ``handler`` must be called to complete the asynchronous 
+        request.
+        """
+        pass
+
+    def async_reset_errors(self, handler):
+        """Called by client to request software reset errors. Calls ``_send_reset_errors()``"""
+        self._send_reset_errors(handler)
+
+    def _verify_communication(self, now):
+        """
+        Verify that the driver is communicating with robot. Compares last communication tomi te 
+        ``_communication_timeout`` to determine when communication has been lost.
+
+        Called by the loop each timestep to check if robot is still communicating.
+
+        :param now: stopwatch time in seconds
+        """
+        if (now - self._last_joint_state) > self._communication_timeout \
+            or (now - self._last_robot_state) > self._communication_timeout \
+            or (now - self._last_endpoint_state) > self._communication_timeout :
+
+            self._communication_failure = True
+
+            self._command_mode = self._robot_command_mode["invalid_state"]
+            if self._base_set_operational_mode:
+                self._operational_mode = self._robot_operational_mode["undefined"]
+                self._controller_state = self._robot_controller_state["undefined"]
+
+            self._joint_position = np.zeros((0,))
+            self._joint_velocity = np.zeros((0,))
+            self._joint_effort = np.zeros((0,))
+
+            self._endpoint_pose = None
+            self._endpoint_vel = None
+
+            return False
+
+        if self._base_set_operational_mode:
+            self._operational_mode = self._robot_operational_mode["cobot"]
+        self._communication_failure = False
+
+        return True
+
+    def _verify_robot_state(self, now):
+        """
+        Verify that the robot is ready to operate, or if an error has occurred. Drops to ``halt`` command mode
+        if robot is not ready. Drops to ``error`` command mode if error has occurred.
+
+        :param now: stopwatch time in seconds
+        """
+
+        if self._command_mode == self._robot_command_mode["homing"]:
+            if self._enabled and not self._error and not self._communication_failure:
+                if self._base_set_controller_state:
+                    self._controller_state = self._robot_controller_state["motor_off"]
+                return True
+
+        if not self._ready or self._error or self._communication_failure:
+            if self._base_set_controller_state:
+                if self._stopped:
+                    self._controller_state = self._robot_controller_state["emergency_stop"]
+                elif self._error:
+                    self._controller_state = self._robot_controller_state["guard_stop"]
+                else:
+                    self._controller_state = self._robot_controller_state["motor_off"]
+            if self._error or self._command_mode != self._robot_command_mode["halt"]:
+                self._command_mode = self._robot_command_mode["invalid_state"]
+            return False
+
+        if not self._enabled:
+            if self._base_set_controller_state:
+                self._controller_state = self._robot_controller_state["motor_off"]
+            if self._command_mode != self._robot_command_mode["halt"]:
+                self._command_mode = self._robot_command_mode["invalid_state"]
+            return False
+
+        if self._command_mode == self._robot_command_mode["invalid_state"] and not self._error:
+             self._command_mode = self._robot_command_mode["halt"]
+
+        if self._base_set_controller_state:
+            self._controller_state = self._robot_controller_state["motor_on"]
+
+        return True
+
+    def _fill_robot_command(self, now):
+        """
+        Fill robot command to send to robot based on current state and commands sent by the client. Returns a
+        tuple containing three elements: ``success``, ``joint_position_command``, ``joint_velocity_command``.
+        If success is False, the driver cannot generate a command in its current state. If ``success`` is True,
+        either ``joint_position_command`` will be non-Null, or ``joint_velocity_command`` will be non-Null.
+        ``joint_velocity_command`` is only valid if the driver has the ``velocity_command`` driver capability.
+        ``joint_position_command`` is in radians (or meters), while ``joint_velocity_command`` is in radians/s 
+        (or meters/s)
+
+        This function is called by the loop every timestep, and the return is passed to ``_send_joint_command()``.
+        It is not typically called by the implementing class.
+
+        :param now: stopwatch time in seconds
+        :rtype: Tuple[bool,np.array,np.array]
+        :return: ``success``, ``joint_position_command``, ``joint_velocity_command``
+        """
+
+        self._wire_position_command_sent = False
+        self._wire_velocity_command_sent = False
+
+        self._trajectory_valid = False
+        self._trajectory_current_time = 0.
+        self._trajectory_max_time = 0.
+        self._trajectory_waypoint = 0
+
+        if self._command_mode != self._robot_command_mode["trajectory"]:
+            if self._active_trajectory is not None:
+                self._active_trajectory._invalid_mode()
+                self._active_trajectory = None
+
+            if len(self._queued_trajectories) > 0:
+                for t in self._queued_trajectories:
+                    t._cancelled_in_queue()
+                self._queued_trajectories.clear()
+
+        if self._command_mode != self._robot_command_mode["jog"]:
+            if self._jog_trajectory_generator is not None:
+                self._jog_trajectory_generator = None
+            if self._jog_completion_handler is not None:
+                h = self._jog_completion_handler
+                self._jog_completion_handler = None
+                self._node.PostToThreadPool(lambda: h(None))
+            
+        if self._command_mode != self._robot_command_mode["velocity_command"]:
+            # self._velocity_command = None
+            pass
+        
+        if self._command_mode == self._robot_command_mode["jog"]:
+            if self._jog_trajectory_generator is not None:
+                jog_time = now - self._jog_start_time
+
+                if jog_time > self._jog_trajectory_generator.t_final:
+                    if self._jog_completion_handler is not None:
+                        h = self._jog_completion_handler
+                        self._jog_completion_handler = None
+                        self._node.PostToThreadPool(lambda: h(None))
+                    self._jog_trajectory_generator = None
+                    return False, None, None
+                
+                res, jog_command = self._jog_trajectory_generator.get_command(jog_time)
+                if not res:
+                    return False, None, None
+
+                joint_pos_cmd = jog_command.command_position
+                return True, joint_pos_cmd, None
+
+            else:
+                if self._jog_completion_handler is not None:
+                    h = self._jog_completion_handler
+                    self._jog_completion_handler = None
+                    self._node.PostToThreadPool(lambda: h(None))
+        
+                return True, None, None
+
+        elif self._command_mode == self._robot_command_mode["position_command"]:
+            
+            res, pos_cmd, ts, ep = self.position_command.TryGetInValue()
+            if not res:
+                return True, None, None
+
+            if self._wire_position_command_last_ep != ep:
+                self._wire_position_command_last_ep = ep
+                self._wire_position_command_last_seqno = 0
+
+            if pos_cmd is None \
+                or pos_cmd.seqno < self._wire_position_command_last_seqno \
+                or abs(pos_cmd.state_seqno - self._state_seqno) > 10 \
+                or len(pos_cmd.command) != self._joint_count \
+                or len(pos_cmd.units) != 0 and len(pos_cmd.units) != self._joint_count:
+                    return True, None, None
+            
+            pos_cmd_j = None
+            if len(pos_cmd.units) == 0:
+                pos_cmd_j = pos_cmd.command
+            else:
+                pos_cmd_j = np.zeros((self._joint_count,))
+                for i in range(self._joint_count):
+                    if pos_cmd.units[i] == self._joint_position_units["implicit"] \
+                        or pos_cmd.units[i] == self._joint_position_units["radian"]:
+                        pos_cmd_j[i] = pos_cmd.command[i]
+                    elif pos_cmd.units[i] == self._joint_position_units["degree"]:
+                        pos_cmd_j[i] = np.deg2rad(pos_cmd.command[i])
+                    elif pos_cmd.units[i] == self._joint_position_units["ticks_rot"]:
+                        pos_cmd_j[i] = pos_cmd.command[i]*(2.*np.pi)/(pow(2.,20.))
+                    elif pos_cmd.units[i] == self._joint_position_units["nanoticks_rot"]:
+                        pos_cmd_j[i] = pos_cmd.command[i]*(2.*np.pi)/(pow(2.,20.)*1.e9)
+                    else:
+                        return True, None, None
+
+            self._wire_position_command_last_seqno = pos_cmd.seqno
+            self._wire_position_command_sent = True
+            return True, pos_cmd_j, None
+
+        elif self._command_mode == self._robot_command_mode["velocity_command"]:
+            
+            res, vel_cmd, ts, ep = self.velocity_command.TryGetInValue()
+            if not res:
+                return True, None, None
+
+            if self._wire_velocity_command_last_ep != ep:
+                self._wire_velocity_command_last_ep = ep
+                self._wire_velocity_command_last_seqno = 0
+
+            if vel_cmd is None \
+                or vel_cmd.seqno < self._wire_velocity_command_last_seqno \
+                or abs(vel_cmd.stat_seqno - self._state_seqno) > 10 \
+                or len(vel_cmd.command) != self._joint_count \
+                or len(vel_cmd.units) != 0 and len(vel_cmd.units) != self._joint_count:
+                    return True, None, None
+            
+            vel_cmd_j = None
+            if len(vel_cmd.units) == 0:
+                vel_cmd_j = vel_cmd.command
+            else:
+                vel_cmd_j = np.zeros((self._joint_count,))
+                for i in range(self._joint_count):
+                    if vel_cmd.units[i] == self._joint_position_units["implicit"] \
+                        or vel_cmd.units[i] == self._joint_position_units["radian_second"]:
+                        vel_cmd_j[i] = vel_cmd.command[i]
+                    elif vel_cmd.units[i] == self._joint_position_units["degree_second"]:
+                        vel_cmd_j[i] = np.deg2rad(vel_cmd.command[i])
+                    elif vel_cmd.units[i] == self._joint_position_units["ticks_rot_second"]:
+                        vel_cmd_j[i] = vel_cmd.command[i]*(2.*np.pi)/(pow(2.,20.))
+                    elif vel_cmd.units[i] == self._joint_position_units["nanoticks_rot_second"]:
+                        vel_cmd_j[i] = vel_cmd.command[i]*(2.*np.pi)/(pow(2.,20.)*1.e9)
+                    else:
+                        return True, None, None
+
+            self._wire_position_command_last_seqno = vel_cmd.seqno
+
+            if self._speed_ratio != 1.0:
+                vel_cmd_j *= self._speed_ratio
+
+            self._wire_position_command_sent = True
+            return True, None, vel_cmd_j
+
+        elif self._command_mode == self._robot_command_mode["trajectory"]:
+
+            if self._active_trajectory is not None:
+                send_traj_cmd = False
+
+                interp_res, traj_pos, traj_vel, traj_t, traj_max_time, traj_waypoint = self._active_trajectory._get_setpoint(now, self._joint_position)
+
+                if interp_res == TrajectoryTaskRes.ready:
+                    self._trajectory_valid = True
+                    send_traj_cmd = False
+                elif interp_res == TrajectoryTaskRes.first_valid_setpoint or \
+                     interp_res == TrajectoryTaskRes.valid_setpoint:
+
+                     self._trajectory_valid = True
+                     send_traj_cmd = True
+                elif interp_res == TrajectoryTaskRes.trajectory_complete:
+                    self._trajectory_valid = True
+                    send_traj_comd = True
+                    self._active_trajectory = None
+                    if len(self._queued_trajectories) > 0:
+                        self._active_trajectory = self._queued_trajectories.pop(0)
+                else:
+                    self._trajectory_valid = False
+                    send_traj_cmd = False
+                    self._active_trajectory = None
+                    for w in self._queued_trajectories:
+                        w._cancelled_in_queue()
+                    self._queued_trajectories.clear()
+                
+                if self._trajectory_valid:
+                    self._trajectory_current_time = traj_t
+                    self._trajectory_max_time = traj_max_time
+                    self._trajectory_waypoint = traj_waypoint
+
+                if send_traj_cmd:
+                    joint_pos_cmd = traj_pos
+                else:
+                    joint_pos_cmd = None
+
+            else:
+                joint_pos_cmd = None
+            return True, joint_pos_cmd, None
+        
+        else:
+            return True, None, None
+
+    @abstractmethod
+    def _send_robot_command(self, now, joint_pos_cmd, joint_vel_cmd):
+        """
+        Called each timestep to send robot command. Must be implemented by subclass.
+
+        Both ``joint_pos_cmd`` and ``joint_vel_cmd`` may be None if there is no valid command available.
+        If ``joint_pos_cmd`` is non-Null, a joint position command must be sent. All drivers must support
+        position command. ``joint_vel_cmd`` is only used for ``velocity_command`` mode, and is only supported
+        if the driver has ``velocity_command`` capability.
+
+        :param now: stopwatch time in seconds
+        :param joint_pos_cmd: Joint position command in radians (or meters)
+        :param joint_vel_cmd: Joint velocity command in radians/s (or meters/s)
+        """
+        pass
+                        
+    @property
+    def command_mode(self):
+        """
+        Get or set the current command mode. Command mode must always be set to ``halt`` (0) before changing to another 
+        mode. If there is an error, the mode will change to ``error`` (-1), and must be set to ``halt`` to clear the 
+        error. If the error cannot be cleared, it may be possible to call the robot a "reset_errors()" function, if the 
+        driver has the ``software_reset_errors`` capability.
+
+        ``jog`` mode (1) requires the robot be in manual operational mode, if the robot supports reading the
+        operational mode and is not a cobot. The ``jog_command`` capability is required.
+
+        ``trajectory`` mode (2) can run in auto or manual operational mode and requires the ``trajectory_command`` 
+        capability.
+
+        ``position_command`` mode (3) can run in auto or manual operational mode and requires the 
+        ``position_command`` capability.
+
+        ``velocity_command`` mode (4) can run in auto or manual operational mode and requires the 
+        ``velocity_command`` capability.
+
+        ``homing_command`` mode (5) requires the ``homing_command`` capability. The implementation is device specific
+
+        """
+        with self._lock:
+            return self._command_mode
+
+    @command_mode.setter
+    def command_mode(self, value):
+        with self._lock:
+            if self._command_mode == self._robot_command_mode["invalid_state"] \
+                and value == self._robot_command_mode["homing"]:
+
+                if not self._enabled or self._communication_failure:
+                    raise RR.InvalidOperationException("Cannot set homing command mode in current state")
+
+                self._command_mode = self._robot_command_mode["homing"]
+                return
+
+            if self._command_mode == self._robot_command_mode["invalid_state"] \
+                and value == self._robot_command_mode["halt"] and self._enabled and not self._error \
+                and not self._communication_failure:
+
+                self._command_mode = value
+                return
+
+            if self._communication_failure:
+                raise RR.InvalidOperationException("Cannot set robot command mode in current state")
+
+            if not self._ready and value != self._robot_command_mode["halt"]:
+                raise RR.InvalidOperationException("Cannot set robot command mode in current state")
+
+            if self._command_mode != self._robot_command_mode["halt"] and value != self._robot_command_mode["halt"]:
+                raise RR.InvalidOperationException("Must switch to \"halt\" before selecting new mode")
+
+            if value == self._robot_command_mode["jog"]:
+                if not self._has_jog_command:
+                    raise RR.InvalidOperationException("Robot does not support jog command mode")
+                self._jog_trajectory_generator = None
+                self._command_mode = self._robot_command_mode["jog"]
+            elif value == self._robot_command_mode["halt"]:
+                self._command_mode = value
+            elif value == self._robot_command_mode["homing"]:
+                if not self._uses_homing:
+                    raise RR.InvalidOperationException("Robot does not support homing command mode")
+                self._command_mode = value
+            elif value == self._robot_command_mode["position_command"]:
+                if not self._has_position_command:
+                    raise RR.InvalidOperationException("Robot does not support position command mode")
+                self._command_mode = value
+            elif value == self._robot_command_mode["velocity_command"]:
+                if not self._has_velocity_command:
+                    raise RR.InvalidOperationException("Robot does not support velocity command mode")
+                self._command_mode = value
+            elif value == self._robot_command_mode["trajectory"]:
+                self._command_mode = value
+            else:
+                raise RR.InvalidOperationException("Invalid command mode specified")
+    
+    def async_jog_freespace(self, joint_position, max_velocity, wait, handler):
+        """
+        Called by client to jog the robot to a specified joint position with specified maximum joint velocity. If wait
+        is True, the function will not return to the client until the move is complete. Otherwise will return
+        immediately.
+
+        This function is typically used to jog the robot to a specific position.
+
+        Robot must be in ``jog`` command mode to call this function.
+
+        This is an asynchronous function, and handler must be called to return result to the client.
+
+        :param joint_position: The desired joint position in radians
+        :type joint_position: np.ndarray
+        :param max_velocity: The maximum joint velocity in radians/s
+        :type max_velocity: np.ndarray
+        :param wait: Wait for completion or return immediately
+        :type wait: bool
+        :param handler: Handler to call when function is complete
+        :type handler: Callable[[],Exception]
+        """
+        with self._lock:
+
+            if self._command_mode != self._robot_command_mode["jog"]:
+                raise RR.InvalidOperationException("Robot not in jog mode")
+
+            if not self._ready:
+                raise RR.InvalidOperationException("Robot not ready")
+
+            if len(joint_position) != self._joint_count:
+                raise RR.InvalidArgumentException(f"joint_position array must have {self._joint_count} elements")
+
+            if len(max_velocity) != self._joint_count:
+                raise RR.InvalidArgumentException(f"max_velocity array must have {self._joint_count} elements")
+
+            
+            if np.any(np.abs(self._joint_position - joint_position) > self._jog_joint_limit):
+                raise RR.InvalidArgumentException("Position command must be within 15 degrees from current")
+
+            if np.any(max_velocity <= 0):
+                raise RR.InvalidArgumentException("max_velocity must be greater than zero")
+
+            if self._jog_completion_handler is not None:
+                h = self._jog_completion_handler
+                self._jog_completion_handler = None
+                self._node.PostToThreadPool(
+                    lambda: h(RR.OperationAbortedException("Operation interrupted by new jog command")))
+            
+            now = self._stopwatch_ellapsed_s()
+            if self._jog_trajectory_generator is None:
+                if self._operational_mode == self._robot_operational_mode["manual_reduced_speed"]:
+                    limits_a_max = np.array([j.joint_limits.reduced_acceleration for j in self._robot_info.joint_info],dtype=np.float64)
+                    limits_v_max = np.array([j.joint_limits.reduced_velocity for j in self._robot_info.joint_info],dtype=np.float64)
+                elif self._operational_mode == self._robot_operational_mode["manual_full_speed"] or \
+                     self._operational_mode == self._robot_operational_mode["cobot"]:
+
+                    limits_a_max = np.array([j.joint_limits.acceleration for j in self._robot_info.joint_info],dtype=np.float64)
+                    limits_v_max = np.array([j.joint_limits.velocity for j in self._robot_info.joint_info],dtype=np.float64)
+                else:
+                    raise RR.InvalidOperationException("Invalid operation mode for jog")
+
+                limits_x_min = np.array([j.joint_limits.lower for j in self._robot_info.joint_info],dtype=np.float64)
+                limits_x_max = np.array([j.joint_limits.upper for j in self._robot_info.joint_info],dtype=np.float64)
+
+                limits = JointTrajectoryLimits(
+                    x_min = limits_x_min,
+                    x_max = limits_x_max,
+                    v_max = limits_v_max,
+                    a_max = limits_a_max,
+                    j_max = None
+                    )
+
+                for i in range(self._joint_count):
+                    if np.abs(max_velocity[i]) > limits.v_max[i]:
+                        raise RR.InvalidArgumentException(
+                            f"max_velocity[{i}] is greater than joint limits ({limits.v_max[i]})")
+                
+                self._jog_trajectory_generator = TrapezoidalJointTrajectoryGenerator(self._joint_count, limits)
+
+                new_req = JointTrajectoryPositionRequest(
+                    current_position = (self._position_command if self._position_command is not None else np.copy(self._joint_position)),
+                    current_velocity = (self._velocity_command if self._velocity_command is not None else np.zeros((self._joint_count,))),
+                    desired_position = joint_position,
+                    desired_velocity = np.zeros((self._joint_count,)),
+                    max_velocity = max_velocity,
+                    speed_ratio = self._speed_ratio
+                )
+
+                self._jog_trajectory_generator.update_desired_position(new_req)
+                self._jog_start_time = now
+            else:
+                jog_trajectory_t = now - self._jog_start_time
+                res, cmd = self._jog_trajectory_generator.get_command(jog_trajectory_t)
+                if not res:
+                    raise RR.InvalidOperationException("Cannot update jog command")
+
+                new_req = JointTrajectoryPositionRequest(
+                    current_position = cmd.command_position,
+                    current_velocity = cmd.command_velocity,
+                    desired_position = joint_position,
+                    desired_velocity = np.zeros((self._joint_count,)),
+                    max_velocity = max_velocity,
+                    speed_ratio = self._speed_ratio
+                )
+
+                self._jog_trajectory_generator.update_desired_position(new_req)
+                self._jog_start_time = now
+
+            if not wait:
+                self._jog_completion_source = None
+                self._node.PostToThreadPool(lambda: handler(None))
+            else:
+                self._jog_completion_handler = handler
+
+    
+    def async_jog_joint(self, joint_velocity, timeout, wait, handler):
+        """
+        Called by client to jog the robot at a specified joint velocity for a specified time. If wait
+        is True, the function will not return to the client until the move is complete. Otherwise will return
+        immediately.
+
+        This function is typically called repeatedly by the client (with wait=False) to drive the robot in response to
+        user input such as a panel button or joystick.
+
+        Robot must be in ``jog`` command mode to call this function.
+
+        This is an asynchronous function, and handler must be called to return result to the client.
+
+        :param joint_velocity: The desired joint velocity position in radians/s
+        :type joint_position: np.ndarray
+        :param timeout: The timeout to run at the specified velocity
+        :type timeout: float
+        :param wait: Wait for completion or return immediately
+        :type wait: bool
+        :param handler: Handler to call when function is complete
+        :type handler: Callable[[],Exception]
+        """
+        with self._lock:
+
+            if self._command_mode != self._robot_command_mode["jog"]:
+                raise RR.InvalidOperationException("Robot not in jog mode")
+
+            if not self._ready:
+                raise RR.OperationAbortedException("Robot not ready")
+
+            if len(joint_velocity) != self._joint_count:
+                raise RR.InvalidArgumentException(f"joint_velocity array must have {self._joint_count} elements")
+
+            if timeout <= 0:
+                raise RR.InvalidArgumentException("Invalid jog timeout specified")
+
+            for i in range(self._joint_count):
+                if abs(joint_velocity[i] > self._robot_info.joint_info[i].joint_limits.reduced_velocity):
+                    raise RR.InvalidArgumentException("Joint velocity exceeds joint limits")
+
+            if self._jog_completion_handler is not None:
+                h = self._jog_completion_handler
+                self._jog_completion_handler = None
+                self._node.PostToThreadPool(
+                    lambda: h(RR.OperationAbortedException("Operation interrupted by new jog command")))
+
+            now = self._stopwatch_ellapsed_s()
+            if self._jog_trajectory_generator is None:
+                if self._operational_mode == self._robot_operational_mode["manual_reduced_speed"]:
+                    limits_a_max = np.array([j.joint_limits.reduced_acceleration for j in self._robot_info.joint_info],dtype=np.float64)
+                    limits_v_max = np.array([j.joint_limits.reduced_velocity for j in self._robot_info.joint_info],dtype=np.float64)
+                elif self._operational_mode == self._robot_operational_mode["manual_full_speed"] or \
+                     self._operational_mode == self._robot_operational_mode["cobot"]:
+                    limits_a_max = np.array([j.joint_limits.acceleration for j in self._robot_info.joint_info],dtype=np.float64)
+                    limits_v_max = np.array([j.joint_limits.velocity for j in self._robot_info.joint_info],dtype=np.float64)
+                else:
+                    raise RR.InvalidOperationException("Invalid operation mode for jog")
+
+                limits_x_min = np.array([j.joint_limits.lower for j in self._robot_info.joint_info],dtype=np.float64)
+                limits_x_max = np.array([j.joint_limits.upper for j in self._robot_info.joint_info],dtype=np.float64)
+                                
+                limits = JointTrajectoryLimits(
+                    x_min = limits_x_min,
+                    x_max = limits_x_max,
+                    v_max = limits_v_max,
+                    a_max = limits_a_max,
+                    j_max = None
+                )
+
+                self._jog_trajectory_generator = TrapezoidalJointTrajectoryGenerator(self._joint_count, limits)
+
+                new_req = JointTrajectoryVelocityRequest(
+                    current_position = (self._position_command if self._position_command is not None else np.copy(self._joint_position)),
+                    current_velocity = (self._velocity_command if self._velocity_command is not None else np.zeros((self._joint_count,))),
+                    desired_velocity = joint_velocity,
+                    speed_ratio = self._speed_ratio,
+                    timeout = timeout
+                )
+
+                self._jog_trajectory_generator.update_desired_velocity(new_req)
+                self._jog_start_time = now
+            else:
+                jog_trajectory_t = now - self._jog_start_time
+                res, cmd = self._jog_trajectory_generator.get_command(jog_trajectory_t)
+                if not res:
+                    raise RR.InvalidOperationException("Cannot update jog command")
+
+                new_req = JointTrajectoryVelocityRequest(
+                    current_position = cmd.command_position,
+                    current_velocity = cmd.command_velocity,
+                    desired_velocity = joint_velocity,
+                    timeout = timeout,
+                    speed_ratio = self._speed_ratio
+                )
+
+                self._jog_trajectory_generator.update_desired_velocity(new_req)
+                self._jog_start_time = now
+
+            if not wait:
+                self._jog_completion_source = None
+                self._node.PostToThreadPool(lambda: handler(None))
+            else:
+                self._jog_completion_handler = handler
+
+    @property
+    def robot_info(self):
+        """
+        Returns the current ``RobotInfo`` structure. The ``RobotInfo`` structure will be updated with tool
+        and payload information as it changes.
+
+        :return: The populated RobotInfo structure
+        :rtype: RobotInfo
+        """
+        with self._lock:
+            
+            for i in range(len(self._robot_info.chains)):
+                self._robot_info.chains[i].current_tool = self._current_tool[i]
+                self._robot_info.chains[i].current_payload = self._current_payload[i]
+                if self._robot_info.chains[i].extended is None:
+                    self._robot_info.chains[i].extended = dict()
+                self._robot_info.chains[i].extended["current_payload_pose"] = \
+                    RR.VarValue(self._current_payload_pose[i], "com.robotraconteur.geometry.Pose") \
+                    if self._current_payload_pose[i] is not None else None
+                
+            return self._robot_info
+
+    def execute_trajectory(self, trajectory):
+        """
+        Called by the client to execute a trajectory. Must be in ``trajectory`` command mode.
+
+        This function returns a generator. The client must call ``Next()`` repeatedly on the generator
+        until the trajectory is complete.
+
+        The first waypoint on the trajectory must be reasonably close to the current robot position.
+
+        :param trajectory: The trajectory to execute
+        :type trajectory: JointTrajectory
+        :return: The trajectory generator, that must have ``Next()`` called repeatedly to execute trajectory
+        :rtype: TrajectoryStatus{generator}
+        """
+        owner_ep = RR.ServerEndpoint.GetCurrentEndpoint()
+
+        with self._lock:
+            speed_ratio = self._speed_ratio
+            current_joint_pos = np.copy(self._joint_position)
+
+        interp = JointTrajectoryInterpolator(self._robot_info)
+        interp.load_trajectory(trajectory, speed_ratio)
+
+        res, joint_pos1, _ = interp.interpolate(0)
+        assert res
+
+        if np.any(np.abs(current_joint_pos - joint_pos1) > self._trajectory_error_tol):
+            raise RR.InvalidArgumentException("Starting waypoint too far from current joint positions")
+
+        with self._lock:
+            if self._command_mode != self._robot_command_mode["trajectory"]:
+                raise RR.InvalidOperationException("Robot must be in trajectory mode to execut trajectory")
+
+            traj_task = None
+
+            if self._active_trajectory is None:
+                traj_task = TrajectoryTask(self, interp, False, owner_ep)
+                self._active_trajectory = traj_task
+            else:
+                traj_task = TrajectoryTask(self, interp, True, owner_ep)
+                self._queued_trajectories.append(traj_task)
+
+            return traj_task
+
+    def _cancel_trajectory(self, trajectory):
+        """
+        Cancel a trajectory that is in the queue. Called from the trajectory generator if ``Close()`` is called.
+        """
+
+        with self._lock:
+            if trajectory is self._active_trajectory:
+                self._active_trajectory = None
+                for t in self._queued_trajectories:
+                    t._cancelled_in_queue()
+                self._queued_trajectories.clear()
+            else:
+                for i in range(len(self._queued_trajectories)):
+                    if trajectory is self._queued_trajectories[i]:
+                        t_index = i
+                        break
+                
+                if t_index >= 0:
+                    for i in range(len(self._queued_trajectories)-1, t_index, -1):
+                        self._queued_trajectories[i]._cancelled_in_queue()
+                        self._queued_trajectories.pop(i)
+                    self._queued_trajectories.pop(t_index)
+
+    def _abort_trajectory(self, trajectory):
+        """
+        Aborts trajectory and all trajectories by dropping to ``halt`` command made. Called by trajectory
+        generater if ``Abort()`` is called.
+        """
+        self._command_mode = self._robot_command_mode["halt"]
+
+    @property
+    def speed_ratio(self):
+        """
+        Get or set the speed ratio. Can be used to reduce or increase speed of trajectory and other operations.
+        :param value: New speed ratio. Must be between 0.1 and 10
+        :type value: float
+        """
+        return self._speed_ratio
+
+    @speed_ratio.setter
+    def speed_ratio(self, value):
+        if value < 0.1 or value > 10:
+            raise RR.InvalidArgumentException("Invalid speed_ratio")
+
+        self._speed_ratio = value
+
+    @property
+    def operational_mode(self):
+        """Return the current operational mode of the controller, if available"""
+        return self._operation_mode
+
+    def controller_state(self):
+        """Return the current state of the vendor robot controller, if available"""
+        return self._controller_state
+
+    def current_errors(self):
+        """Returns currently reported errors, if available"""
+        return []
+
+    def jog_cartesian(self, velocity, timeout, wait):
+        """
+        Called by client to jog the robot at a specified cartesian velocity for a specified time. If wait
+        is True, the function will not return to the client until the move is complete. Otherwise will return
+        immediately.
+
+        This function is typically called repeatedly by the client (with wait=False) to drive the robot in response to
+        user input such as a panel button or joystick.
+
+        Robot must be in ``jog`` command mode to call this function.
+
+        This is an asynchronous function, and handler must be called to return result to the client.
+
+        :param velocity: The desired end effector spatial velocity position in meters/s,radians/s
+        :type joint_position: SpatialVelocity
+        :param timeout: The timeout to run at the specified velocity
+        :type timeout: float
+        :param wait: Wait for completion or return immediately
+        :type wait: bool
+        :param handler: Handler to call when function is complete
+        :type handler: Callable[[],Exception]
+        """
+        raise RR.NotImplementedException("Not implemented")
+
+    def async_home(self, handler):
+        """
+        Called by client to home the robot. Behavior is device specific.
+
+        Robot must be in ``homing`` command mode to call this function.
+
+        :param handler: Handler to call when function is complete
+        :type handler: Callable[[],Exception]
+        """
+        raise RR.NotImplementedException()
+
+    def async_getf_signal(self, signal_name, handler):
+        """Get the value of a signal. Optionally implemented by subclass"""
+        raise RR.NotImplementedException()
+
+    def async_setf_signal(self, signal_name, value, handler):
+        """Set the value of a signal. Optionally implemented by subclass"""
+        raise RR.NotImplementedException()
+
+    def tool_attached(self, chain, tool):
+        """
+        Called by client to notify the driver that a tool has been attached. TCP is used to compute endpoint position
+        and velocity. Implementing class may also update the vendor robot controller if necessary.
+
+        :param chain: The kinematic chain the tool has been attached
+        :type chain: int
+        :param tool: The ToolInfo structure of the tool, specified by the client
+        :type tool: ToolInfo
+        """
+        if tool is None:
+            raise RR.NullValueException("Tool cannot be null")
+
+        if chain > 0 or not (chain < len(self._current_tool)):
+            raise RR.InvalidArgumentException(f"Invalid kinematic chain {chain} for tool")
+
+        with self._lock:
+            if self._current_tool[chain] is not None:
+                raise RR.InvalidArgumentException(f"Tool already attached to kinematic chain {chain}")
+
+            self._current_tool[chain] = tool
+
+            try:
+                device_name = tool.device_info.device.name
+            except:
+                traceback.print_exc()
+                device_name = ""
+
+            self.tool_changed.fire(chain, device_name)
+            self._config_seqno+=1
+
+    def tool_detached(self, chain, tool_name):
+        """
+        Called by client to notify the driver that a tool has been detached. Payloads must be detached before
+        the tool can be detached.
+
+        :param payload_name: The name of the tool that was detached
+        :type payload_name: str
+        """
+
+        if chain > 0 or not (chain < len(self._current_tool)):
+            raise RR.InvalidArgumentException(f"Invalid kinematic chain {chain} for tool")
+
+        with self._lock:
+            if self._current_tool[chain] is None:
+                raise RR.InvalidArgumentException(f"Tool not attached to kinematic chain {chain}")
+
+            if self._current_payload[chain] is not None:
+                raise RR.InvalidArgumentException(f"Cannot remove tool while payload attached")
+
+            if len(tool_name) > 0:                
+                try:
+                    device_name = self._current_tool.device_info.device.name
+                except:
+                    traceback.print_exc()
+                    device_name = ""
+                
+                if device_name != tool_name:
+                    raise RR.InvalidArgumentException(f"Invalid tool name to detach from kinematic chain {chain}")
+            
+            self._current_tool[chain] = None
+
+            self.tool_changed.fire(chain, "")
+            self._config_seqno+=1
+
+    def payload_attached(self, chain, payload, pose):
+        """
+        Called by client to notify the driver that a payload has been attached to the tool. A tool must be attached
+        to attach a payload. The pose between the payload and tool is also specified.
+        
+        Implementing class may also update the vendor robot controller if necessary.
+
+        :param chain: The kinematic chain the tool has been attached
+        :type chain: int
+        :param payload: The PayloadInfo structure of the tool, specified by the client
+        :type tool: PayloadInfo
+        :param pose: The pose of the payload relative to the tool TCP
+        :type pose: com.geometry.Pose
+        """
+        if payload is None:
+            raise RR.NullValueException("Payload cannot be null")
+
+        if chain > 0 or not (chain < len(self._current_payload)):
+            raise RR.InvalidArgumentException(f"Invalid kinematic chain {chain} for payload")
+
+        with self._lock:
+            if self._current_tool[chain] is None:
+                raise RR.InvalidArgumentException(f"No tool attached to kinematic chain {chain}, cannot attach payload")
+
+            if self._current_payload[chain] is not None:
+                raise RR.InvalidArgumentException(f"Payload already attached to kinematic chain {chain}")
+
+            self._current_payload[chain] = payload
+            self._current_payload_pose[chain] = pose
+
+            try:
+                device_name = payload.device_info.device.name
+            except:
+                traceback.print_exc()
+                device_name = ""
+
+            self.payload_changed.fire(chain, device_name)
+            self._config_seqno+=1
+    
+    def payload_detached(self, chain, payload_name):
+        """
+        Called by client to notify the driver that a payload has been detached
+
+        :param payload_name: The name of the payload that was detached
+        :type payload_name: str
+        """
+        
+        if chain > 0 or not (chain < len(self._current_payload)):
+            raise RR.InvalidArgumentException(f"Invalid kinematic chain {chain} for payload")
+
+        with self._lock:
+            
+            if self._current_payload[chain] is None:
+                raise RR.InvalidArgumentException(f"Payload not attached to kinematic chain {chain}")
+
+            if len(payload_name) != 0:
+                try:
+                    device_name = self._current_payload[chain].device_info.device.name
+                except:
+                    traceback.print_exc()
+                    device_name = ""
+            
+                if device_name != payload_name:
+                    raise RR.InvalidArgumentException(f"Invalid payload name to detach from kinematic chain {chain}")
+            
+            self._current_payload[chain] = None
+            self.payload_changed.fire(chain, "")
+            self._config_seqno+=1
+
+    def getf_param(self, param_name):
+        """Get the value of a parameter. Optionally implemented by subclass"""
+        raise RR.InvalidArgumentException("Invalid parameter")
+
+    def setf_param(self, param_name, value):
+        """Set the value of a parameter. Optionally implemented by subclass"""
+        raise RR.InvalidArgumentException("Invalid parameter")
+
+    @property
+    def device_info(self):
+        """Returns the DeviceInfo structure contained in RobotInfo"""
+        return self._robot_info.device_info
+
+    @property
+    def isoch_info(self):
+        """Returns the IsochInfo structure"""
+        iso_info = self._isoch_info_type()
+        iso_info.update_rate = 1.0/self._update_period
+        iso_info.max_downsample = 1000
+
+        iso_info.isoch_epoch = self._stopwatch_epoch
+
+        return iso_info
+
+    @property
+    def isoch_downsample(self):
+        """
+        Get or set the current client isoch_downsample level. By default, the wires and pipes will transmit
+        every timestep. The ``isoch_downsample`` property allows the client to request every ``n`` samples be dropped.
+        For instance, if ``isoch_downsample`` is set to 2, the driver will skip two timesteps, and only transmit on every
+        third timestep. Check ``isoch_info` to determine the native loop update rate in Hz.
+
+        :param value: The downsample level
+        :type value: int
+        
+        """
+        with self._lock:
+            return self._broadcast_downsampler.GetClientDownsample(RR.ServerEndpoint.GetCurrentEndpoint())
+
+    @isoch_downsample.setter
+    def isoch_downsample(self, value):
+        with self._lock:
+            self._broadcast_downsampler.SetClientDownsample(RR.ServerEndpoint.GetCurrentEndpoint(), value)
+
+
+class TrajectoryTaskRes(Enum):
+    unknown = 0
+    ready = 1
+    first_valid_setpoint = 2
+    valid_setpoint = 3
+    trajectory_complete = 4
+    invalid_state = 5
+    joint_tol_error = 6
+    failed = 7
+
+
+class TrajectoryTask:
+
+    def __init__(self, parent, path, queued, owner_ep):
+        self._parent = parent
+        self._path = path
+        self._queued = queued
+        self._owner_ep = owner_ep
+
+        self._next_called = False
+        self._started = False
+        self._start_time = 0
+        self._aborted = False
+        self._cancelled = False
+        self._joint_tol_error = False
+        self._finished = False
+        self._next_wait_handler = []
+        self._queue_wait_handler = []
+        self._success_sent = False
+
+        self._node = parent._node
+        self._trajectory_status_type = \
+            self._node.GetStructureType("com.robotraconteur.robotics.trajectory.TrajectoryStatus")
+
+        self._action_consts = self._node.GetConstants("com.robotraconteur.action")
+        self._action_status_code = self._action_consts["ActionStatusCode"]
+
+        self._traj_t = 0.0
+        self._traj_waypoint = 0
+
+        self._lock = threading.Lock()
+
+    def _call_next_wait_handler(self, err):
+        with self._lock:
+            for c in self._next_wait_handler:
+                self._node.PostToThreadPool(lambda c=c, err=err: c(err))
+            self._next_wait_handler.clear()
+
+    def _call_queue_wait_handler(self,err):
+        with self._lock:
+            for c in self._queue_wait_handler:
+                self._node.PostToThreadPool(lambda c=c, err=err: c(err))
+            self._next_wait_handler.clear()
+
+    def Abort(self):
+        self._aborted = True
+        self._parent._abort_trajectory(self)
+        self._call_next_wait_handler(RR.OperationAbortedException("Trajectory execution aborted"))
+
+    def Close(self):
+        self._cancelled = True
+        self._parent._cancel_trajectory(self)
+        self._call_next_wait_handler(RR.OperationAbortedException("Trajectory execution cancelled"))
+
+    def AsyncNext(self,handler):
+        if self._success_sent:
+            raise RR.StopIterationException("")
+
+        with self._lock:            
+            first_call = not self._next_called
+            self._next_called = True
+
+            if first_call and self._queued:
+                # Report back that we are queued immediately
+
+                ret = self._trajectory_status_type()
+                ret.action_status = self._action_status_code["queued"]
+                ret.trajectory_time = 0
+                ret.current_waypoint = 0
+                ret.seqno = self._parent._state_seqno
+                handler(ret, None)
+                return
+
+            complete_called = [False]
+
+            def complete(err):
+                with self._lock:
+                    if complete_called[0]:
+                        return
+                    complete_called[0] = True
+                if err:
+                    handler(None, err)
+                
+                if not self._started:
+                    # Still queued...
+
+                    ret = self._trajectory_status_type()
+                    ret.action_status = self._action_status_code["queued"]
+                    ret.trajectory_time = 0
+                    ret.current_waypoint = 0
+                    ret.seqno = self._parent._state_seqno
+                    handler(ret, None)
+                    return
+
+                if self._finished:
+                    self._success_sent = True
+                    ret = self._trajectory_status_type()
+                    ret.action_status = self._action_status_code["complete"]
+                    ret.trajectory_time = self._traj_t
+                    ret.current_waypoint = int(self._traj_waypoint)
+                    ret.seqno = self._parent._state_seqno
+                    handler(ret, None)
+                    return
+
+                else:
+                    ret = self._trajectory_status_type()
+                    ret.action_status = self._action_status_code["running"]
+                    ret.trajectory_time = self._traj_t
+                    ret.current_waypoint = int(self._traj_waypoint)
+                    ret.seqno = self._parent._state_seqno
+                    handler(ret,None)
+                    return
+
+            if self._queued:
+                self._next_wait_handler.append(complete)
+                self._queue_wait_handler.append(complete)
+            else:
+                self._next_wait_handler.append(complete)
+
+            timer = self._node.CreateTimer(5, lambda _: complete(None), True)
+            timer.Start()
+
+    def _cancelled_in_queue(self):
+        self._cancelled = True
+        self._call_next_wait_handler(RR.OperationAbortedException("Trajectory cancelled by controller before start"))
+
+    def _invalid_mode(self):
+        self._aborted = True
+        self._call_next_wait_handler(RR.OperationAbortedException("Invalid mode for trajectory execution"))
+
+    
+    def _get_setpoint(self, now, current_joint_pos):
+        if self._cancelled or self._aborted:
+            return TrajectoryTaskRes.failed, None, None, 0.0, 0.0, 0
+
+        first_call = False
+
+        t = 0.0
+
+        if self._next_called:
+            if not self._started:
+                self._start_time = now
+                self._started = True
+                first_call = True
+
+            t = now - self._start_time
+
+        res, joint_pos1, current_waypoint1 = self._path.interpolate(t)
+        if not res:
+            self._call_next_wait_handler(Exception("Trajectory execution failed"))
+            return TrajectoryTaskRes.failed, None, None, 0.0, 0.0, 0
+
+        if np.any(np.abs(current_joint_pos - joint_pos1) > self._parent._trajectory_error_tol):
+            self._call_next_wait_handler(RR.OperationFailedException("Trajectory tolerance failure"))
+            return TrajectoryTaskRes.ready, None, None, 0.0, 0.0, 0
+
+        if not self._next_called:
+            return TrajectoryTaskRes.ready, None, None, 0.0, self._path.max_time, 0
+        
+        if t > self._path.max_time:
+            self._traj_t = t
+            self._traj_waypoint = current_waypoint1
+            self._finished = True
+            self._call_next_wait_handler(None)
+            return TrajectoryTaskRes.trajectory_complete, joint_pos1, None, t, self._path.max_time, current_waypoint1
+
+        if first_call:
+            if self._queued:
+                self._queued = False
+                self._call_queue_wait_handler(None)
+            return TrajectoryTaskRes.first_valid_setpoint, joint_pos1, None, t, self._path.max_time, current_waypoint1
+        else:
+            return TrajectoryTaskRes.valid_setpoint, joint_pos1, None, t, self._path.max_time, current_waypoint1
+
+    #TODO: Add connection test?
+
```

## robotraconteur_abstract_robot/joint_trajectory_interpolator.py

 * *Ordering differences only*

```diff
@@ -1,122 +1,122 @@
-# Copyright 2022 Wason Technology, LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import numpy as np
-from scipy.interpolate import CubicSpline
-import RobotRaconteur as RR
-
-class JointTrajectoryInterpolator:
-
-    def __init__(self, info):
-        self._joint_names = [j.joint_identifier.name for j in info.joint_info]
-        self._joint_min = np.array([j.joint_limits.lower for j in info.joint_info])
-        self._joint_max = np.array([j.joint_limits.upper for j in info.joint_info])
-        self._joint_vel_max = np.array([j.joint_limits.velocity for j in info.joint_info])
-        self._joint_splines = None
-        self._max_t = 0
-        self._joint_start = None
-        self._joint_end = None
-        self._waypoint_times = None
-
-    def load_trajectory(self, traj, speed_ratio):
-
-        if len(traj.joint_names) > 0:
-            if traj.joint_names != self._joint_names:
-                raise RR.InvalidArgumentException("Joint names in trajectory must match robot joint names")
-
-        if traj.waypoints is None:
-            raise RR.InvalidArgumentException("Waypoint list must not be null")
-
-        if len(traj.waypoints) < 5:
-            raise RR.InvalidArgumentException("Waypoint list must contain five or more waypoints")
-
-        if traj.waypoints[0].time_from_start != 0:
-            raise RR.InvalidArgumentException("Trajectory time_from_start must equal zero for first waypoint")
-
-        n_waypoints = len(traj.waypoints)
-        n_joints = len(self._joint_names)
-
-        traj_t = np.zeros((n_waypoints,))
-        traj_j = np.zeros((n_waypoints, n_joints))
-
-        last_t = 0
-
-        for i in range(n_waypoints):
-
-            w = traj.waypoints[i]
-
-            if (len(w.joint_position) != n_joints):
-                raise RR.InvalidArgumentException(f"Waypoint {i} invalid joint array length")
-
-            if len(w.joint_velocity) != n_joints and len(w.joint_velocity) != 0:
-                raise RR.InvalidArgumentException(f"Waypoint {i} invalid joint velocity array length")
-
-            if len(w.position_tolerance) != n_joints and len(w.position_tolerance) != 0:
-                raise RR.InvalidArgumentException(f"Waypoint {i} invalid tolerance array length")
-
-            if len(w.velocity_tolerance) != n_joints and len(w.velocity_tolerance) != 0:
-                raise RR.InvalidArgumentException(f"Waypoint {i} invalid tolerance array length")
-
-            if i > 0:
-                if w.time_from_start/speed_ratio <= last_t:
-                    raise RR.InvalidArgumentException(f"Waypoint {i} time_from_start must be increasing")
-
-                if w.time_from_start/speed_ratio - last_t > 0.1:
-                    raise RR.InvalidArgumentException("Waypoint {i} more than 100 ms from previous waypoint")
-
-            if np.any(w.joint_position > self._joint_max) or np.any(w.joint_position < self._joint_min):
-                raise RR.InvalidArgumentException(f"Waypoint {i} exceeds joint limits")
-
-            if len(w.joint_velocity) > 0:
-                if np.any(np.abs(w.joint_velocity*speed_ratio) > self._joint_vel_max):
-                    raise RR.InvalidArgumentException(f"Waypoint {i} exceeds joint velocity limits")
-
-            if i > 0:
-                last_w = traj.waypoints[i-1]
-                dt = w.time_from_start/speed_ratio - last_w.time_from_start/speed_ratio
-                dj = np.abs(w.joint_position - last_w.joint_position)
-                if np.any (dj/dt > self._joint_vel_max):
-                    raise RR.InvalidArgumentException(f"Waypoint {i} exceeds joint velocity limits")
-
-            traj_t[i] = w.time_from_start/speed_ratio
-            traj_j[i,:] = w.joint_position
-            last_t = w.time_from_start / speed_ratio 
-
-        self._joint_splines = CubicSpline(traj_t, traj_j)
-        self._max_t = last_t
-
-        self._joint_start = traj.waypoints[0].joint_position
-        self._joint_end = traj.waypoints[-1].joint_position
-        self._waypoint_times = traj_t
-
-    @property
-    def max_time(self):
-        return self._max_t
-
-    def interpolate(self, time):
-        if time <= 0:
-            return True, self._joint_start, 0
-
-        if time >= self._max_t:
-            return True, self._joint_end, len(self._waypoint_times) -1
-
-        joint_pos = self._joint_splines(time)
-
-        a = np.where(self._waypoint_times <= time)[0]
-        if len(a) > 0:
-            current_waypoint = a[-1]
-        else:
-            current_waypoint = 0
-        
+# Copyright 2022 Wason Technology, LLC
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import numpy as np
+from scipy.interpolate import CubicSpline
+import RobotRaconteur as RR
+
+class JointTrajectoryInterpolator:
+
+    def __init__(self, info):
+        self._joint_names = [j.joint_identifier.name for j in info.joint_info]
+        self._joint_min = np.array([j.joint_limits.lower for j in info.joint_info])
+        self._joint_max = np.array([j.joint_limits.upper for j in info.joint_info])
+        self._joint_vel_max = np.array([j.joint_limits.velocity for j in info.joint_info])
+        self._joint_splines = None
+        self._max_t = 0
+        self._joint_start = None
+        self._joint_end = None
+        self._waypoint_times = None
+
+    def load_trajectory(self, traj, speed_ratio):
+
+        if len(traj.joint_names) > 0:
+            if traj.joint_names != self._joint_names:
+                raise RR.InvalidArgumentException("Joint names in trajectory must match robot joint names")
+
+        if traj.waypoints is None:
+            raise RR.InvalidArgumentException("Waypoint list must not be null")
+
+        if len(traj.waypoints) < 5:
+            raise RR.InvalidArgumentException("Waypoint list must contain five or more waypoints")
+
+        if traj.waypoints[0].time_from_start != 0:
+            raise RR.InvalidArgumentException("Trajectory time_from_start must equal zero for first waypoint")
+
+        n_waypoints = len(traj.waypoints)
+        n_joints = len(self._joint_names)
+
+        traj_t = np.zeros((n_waypoints,))
+        traj_j = np.zeros((n_waypoints, n_joints))
+
+        last_t = 0
+
+        for i in range(n_waypoints):
+
+            w = traj.waypoints[i]
+
+            if (len(w.joint_position) != n_joints):
+                raise RR.InvalidArgumentException(f"Waypoint {i} invalid joint array length")
+
+            if len(w.joint_velocity) != n_joints and len(w.joint_velocity) != 0:
+                raise RR.InvalidArgumentException(f"Waypoint {i} invalid joint velocity array length")
+
+            if len(w.position_tolerance) != n_joints and len(w.position_tolerance) != 0:
+                raise RR.InvalidArgumentException(f"Waypoint {i} invalid tolerance array length")
+
+            if len(w.velocity_tolerance) != n_joints and len(w.velocity_tolerance) != 0:
+                raise RR.InvalidArgumentException(f"Waypoint {i} invalid tolerance array length")
+
+            if i > 0:
+                if w.time_from_start/speed_ratio <= last_t:
+                    raise RR.InvalidArgumentException(f"Waypoint {i} time_from_start must be increasing")
+
+                if w.time_from_start/speed_ratio - last_t > 0.1:
+                    raise RR.InvalidArgumentException("Waypoint {i} more than 100 ms from previous waypoint")
+
+            if np.any(w.joint_position > self._joint_max) or np.any(w.joint_position < self._joint_min):
+                raise RR.InvalidArgumentException(f"Waypoint {i} exceeds joint limits")
+
+            if len(w.joint_velocity) > 0:
+                if np.any(np.abs(w.joint_velocity*speed_ratio) > self._joint_vel_max):
+                    raise RR.InvalidArgumentException(f"Waypoint {i} exceeds joint velocity limits")
+
+            if i > 0:
+                last_w = traj.waypoints[i-1]
+                dt = w.time_from_start/speed_ratio - last_w.time_from_start/speed_ratio
+                dj = np.abs(w.joint_position - last_w.joint_position)
+                if np.any (dj/dt > self._joint_vel_max):
+                    raise RR.InvalidArgumentException(f"Waypoint {i} exceeds joint velocity limits")
+
+            traj_t[i] = w.time_from_start/speed_ratio
+            traj_j[i,:] = w.joint_position
+            last_t = w.time_from_start / speed_ratio 
+
+        self._joint_splines = CubicSpline(traj_t, traj_j)
+        self._max_t = last_t
+
+        self._joint_start = traj.waypoints[0].joint_position
+        self._joint_end = traj.waypoints[-1].joint_position
+        self._waypoint_times = traj_t
+
+    @property
+    def max_time(self):
+        return self._max_t
+
+    def interpolate(self, time):
+        if time <= 0:
+            return True, self._joint_start, 0
+
+        if time >= self._max_t:
+            return True, self._joint_end, len(self._waypoint_times) -1
+
+        joint_pos = self._joint_splines(time)
+
+        a = np.where(self._waypoint_times <= time)[0]
+        if len(a) > 0:
+            current_waypoint = a[-1]
+        else:
+            current_waypoint = 0
+        
         return True, joint_pos, current_waypoint
```

## robotraconteur_abstract_robot/trapezoidal_joint_trajectory_generator.py

 * *Ordering differences only*

```diff
@@ -1,463 +1,463 @@
-# Copyright 2022 Wason Technology, LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import numpy as np
-import RobotRaconteur as RR
-from typing import NamedTuple
-
-class JointTrajectoryLimits(NamedTuple):
-    j_max: np.array
-    a_max: np.array
-    v_max: np.array
-    x_min: np.array
-    x_max: np.array
-
-class JointTrajectoryPositionRequest(NamedTuple):
-    current_position: np.array
-    current_velocity: np.array
-    desired_position: np.array
-    desired_velocity: np.array
-    max_velocity: np.array
-    desired_time: float = None
-    speed_ratio: float = 1.
-    splice_time: float = None
-
-class JointTrajectoryVelocityRequest(NamedTuple):
-    current_position: np.array
-    current_velocity: np.array
-    desired_velocity: np.array
-    timeout: float
-    speed_ratio: float
-    desired_time: float = None
-
-class JointTrajectoryPositionCommand(NamedTuple):
-    command_position: np.array
-    command_velocity: np.array
-
-
-class TrapezoidalJointTrajectoryGenerator:
-
-    def __init__(self, joint_count, limits):
-        self._joint_count=joint_count
-        self._limits=limits
-
-        self._speed_ratio = 1.0
-        self._t_des = 0.0
-        self._exec = None
-
-    @property
-    def t_des(self):
-        return self._t_des
-
-    @property
-    def speed_ratio(self):
-        return self._speed_ratio
-
-    @property
-    def t_final(self):
-        if self._exec is not None:
-            return self._exec.t_final
-        else:
-            return 0.
-
-    @property
-    def is_valid(self):
-        return self._exec is not None
-
-    @property
-    def target_position(self):
-        return self._exec.xf
-
-    @property
-    def target_velocity(self):
-        return self._exec.v3
-
-    def get_command(self, t):
-        if self._exec is None:
-            return False, None
-
-        res, command_position, command_velocity = self._exec.calc_at_time(t)
-        if not res:
-            return False, None
-        command = JointTrajectoryPositionCommand(
-            command_position = command_position,
-            command_velocity = command_velocity
-        )
-
-        return True, command
-
-    def update_desired_position(self, request):
-        assert request.desired_time is None, "desired time not supported"
-        self._exec = TrapezoidalJointTrajectoryGeneratorCalc.initialize_pos_exec(self._joint_count, self._limits, request)
-        return True
-
-    def update_desired_velocity(self, request):
-        self._exec = TrapezoidalJointTrajectoryGeneratorCalc.initialize_vel_exec(self._joint_count, self._limits, request)
-        return True
-
-class TrapezoidalJointTrajectoryGeneratorCalc:
-    
-    @classmethod
-    def initialize_pos_exec(cls, joint_count, limits, request):
-        assert request.desired_time is None
-
-        a_max = np.copy(limits.a_max)
-        v_max = np.copy(limits.v_max)
-
-        if request.speed_ratio != 0.0:
-            a_max *= request.speed_ratio
-            v_max *= request.speed_ratio
-
-            if request.max_velocity is not None:
-                req_vel = request.max_velocity * request.speed_ratio
-                assert np.all(req_vel <= v_max), "req_vel must be less than or equal to v_max"
-                v_max = np.minimum(req_vel,v_max)
-
-        else:            
-            assert np.all(request.max_velocity <= v_max), "req_vel must be less than or equal to v_max"
-            v_max = np.minimum(request.max_velocity,v_max)
-
-        dx = request.desired_position - request.current_position
-
-        t1 = np.zeros((joint_count,))
-        t2 = np.zeros((joint_count,))
-        t3 = np.zeros((joint_count,))
-
-        v1 = np.zeros((joint_count,))
-        a1 = np.zeros((joint_count,))
-        a3 = np.zeros((joint_count,))
-
-        for i in range(joint_count):
-            if dx[i] == 0 and request.desired_velocity[i] == 0 and request.current_velocity[i] == 0:
-                continue
-
-            case2_success, v1[i], a1[i], a3[i], t1[i], t2[i], t3[i] = \
-                cls.solve_case2(
-                request.current_position[i], request.desired_position[i], request.current_velocity[i],
-                request.desired_velocity[i], v_max[i], a_max[i]
-            )
-
-            if not case2_success:
-                case3_success, a1[i], a3[i], t1[i], t3[i] = \
-                    cls.solve_case3(
-                    request.current_position[i], request.desired_position[i], request.current_velocity[i],
-                    request.desired_velocity[i], a_max[i]
-                )
-                t2[i] = 0
-                v1[i] = 0
-
-                assert case3_success, "Invalid trajectory request"
-
-        t1_4 = np.max(t1)
-        t2_4 = np.max(t2)
-        t3_4 = np.max(t3)
-
-        a1_4 = np.zeros((joint_count,))
-        a3_4 = np.zeros((joint_count,))
-        v1_4 = np.zeros((joint_count,))
-
-        for i in range(joint_count):
-            v1_4[i], a1_4[i], a3_4[i] = cls.solve_case4(
-                request.current_position[i], request.desired_position[i], request.current_velocity[i], 
-                request.desired_velocity[i], t1_4, t2_4, t3_4)
-
-        return TrapezoidalJointTrajectoryGeneratorExec(
-            joint_count = joint_count,
-            t1 = t1_4,
-            t2 = t2_4,
-            t3 = t3_4,
-            x1 = request.current_position,
-            v1 = request.current_velocity,
-            v2 = v1_4,
-            v3 = request.desired_velocity,
-            a1 = a1_4,
-            a3 = a3_4,
-            xf = request.desired_position
-        )
-
-    @staticmethod
-    def pos_1(a, v, x, t):
-        return (0.5 * a * pow(t, 2) if a != 0 else 0.0) + v*t + x
-
-    @staticmethod
-    def vel_1(a, v, t):
-        return (a *t if a != 0 else 0.0) + v
-
-    @classmethod
-    def pos(cls,a1, a3, x0, v0, t1, t2, t3):
-        v1_p = cls.vel_1(a1, v0, t1)
-        v3_p = cls.vel_1(a3, v1_p, t3)
-
-        x1_p = cls.pos_1(a1, v0, x0, t1)
-        x2_p = cls.pos_1(0, v1_p, x1_p, t2)
-        x3_p = cls.pos_1(a3, v1_p, x2_p, t3)
-
-        return x3_p, v3_p
-
-    @classmethod
-    def solve_case2_sub(cls, x0, xf, v0, v1, vf, a_max):
-        t1 = 0
-        a1 = 0
-        if v1 != v0:
-            a1 = a_max * np.sign(v1 - v0)
-            t1 = (v1-v0) / a1
-        
-        t3 = 0
-        a3 = 0
-        if vf != v1:
-            a3 = a_max * np.sign(vf-v1)
-            t3 = (vf - v1) / a3
-
-        xf_1, vf_1 = cls.pos(a1, a3, x0, v0, t1, 0.0, t3)
-
-        dx2 = xf - xf_1
-
-        t2 = dx2/v1
-
-        return t2 >= 0, a1, a3, t1, t2, t3
-
-    @classmethod
-    def solve_case2(cls, x0, xf, v0, vf, v_max, a_max):
-        case2_res, a1, a3, t1, t2, t3 = cls.solve_case2_sub(x0, xf, v0, v_max, vf, a_max)
-        if case2_res:
-            return True, v_max, a1, a3, t1, t2, t3
-
-        case2_res, a1, a3, t1, t2, t3 = cls.solve_case2_sub(x0, xf, v0, -v_max, vf, a_max)
-        if case2_res:
-            return True, -v_max, a1, a3, t1, t2, t3
-
-        return False, None, None, None, None, None, None
-
-
-    @staticmethod
-    def solve_case3_sub1(x0, xf, v0, vf, a1):
-        return a1 * (xf - x0) + 0.5 * pow(v0, 2.0) + 0.5 * pow(vf, 2.0)
-
-    @classmethod
-    def solve_case3(cls, x0, xf, v0, vf, a_max):
-        sub1 = cls.solve_case3_sub1(x0, xf, v0, vf, a_max)
-        if sub1 >= 0:
-            a1 = a_max
-            a3 = -a_max
-            t1 = (-v0 + np.sqrt(sub1)) / a1
-            t3 = (a1*t1 + v0-vf) / a1
-            if t1 > 0 and t3 > 0:
-                return True, a1, a3, t1, t3
-            t1 = (-v0 - np.sqrt(sub1))/ a1
-            t3 = a1 * (a1 * t1 + v0 - vf) / a1
-            if t1 > 0 and t3 > 0:
-                return True, a1, a3, t1, t3
-
-        sub1 = cls.solve_case3_sub1(x0, xf, v0, vf, -a_max)
-
-        if sub1 >= 0:
-            a1 = -a_max
-            a3 = a_max
-            t1 = (-v0 + np.sqrt(sub1)) / a1
-            t3 = (a1 * t1 + v0 - vf) / a1
-            if t1 > 0 and t3 > 0:
-                return True, a1, a3, t1, t3
-
-            t1 = (-v0 - np.sqrt(sub1)) / a1
-            t3 = (a1 * t1 + v0 - vf) / a1
-            if (t1 > 0 and t3 > 0):
-                return True, a1, a3, t1, t3
-
-        return False, None, None, None, None
-
-    @classmethod
-    def solve_case4(cls, x0, xf, v0, vf, t1, t2, t3):
-        a1_den = t1 * (t1 + 2*t2 + t3)
-        a1 = (-2 * t1 * v0 - 2 * t2 * v0 - t3 * v0 - t3 * vf - 2 * x0 + 2 * xf) / a1_den if a1_den !=0 else 0.0
-        v1 = a1 * t1 + v0
-        a3 = 0.0
-        if t3 != 0:
-            a3 = (-a1 * t1 - v0 + vf) / t3
-
-        return v1, a1, a3
-    
-    @classmethod
-    def initialize_vel_exec(cls, joint_count, limits, request):
-        a_max = np.copy(limits.a_max)
-        v_max = np.copy(limits.v_max)
-        if request.speed_ratio != 0.0:
-            a_max *= request.speed_ratio
-            v_max *= request.speed_ratio
-
-            req_vel = request.desired_velocity * request.speed_ratio
-            assert np.all(req_vel <= v_max), "req_vel must be less than or equal to v_max"
-            v_max = np.minimum(v_max, req_vel)
-
-        else:
-            assert np.all(request.max_velocity <= v_max), "req_vel must be less than or equal to v_max"
-            v_max = np.minimum(request.max_velocity,v_max)
-
-        t1 = np.zeros((joint_count,))
-        t2 = np.zeros((joint_count,))
-        t3 = np.zeros((joint_count,))
-
-        v1 = np.zeros((joint_count,))
-        a1 = np.zeros((joint_count,))
-        a3 = np.zeros((joint_count,))
-
-        for i in range(joint_count):
-            if request.desired_velocity[i] == 0 and request.current_velocity[i] == 0:
-                continue
-
-            a_max[i], v1[i], a1[i], a3[i], t1[i], t2[i], t3[i] = cls.solve_case5(request.current_velocity[i], 
-                request.desired_velocity[i], 0, request.timeout, a_max[i])
-
-        t1_4 = np.max(t1)
-        t2_4 = np.max(t2)
-        t3_4 = np.max(t3)
-
-        a1_4 = np.zeros((joint_count,))
-        a3_4 = np.zeros((joint_count,))
-
-        for i in range(joint_count):
-            a1_4[i], a3_4[i] = cls.solve_case6(request.current_velocity[i], v1[i], 0, t1_4, t2_4, t3_4)
-
-        ret = TrapezoidalJointTrajectoryGeneratorExec(
-            joint_count = joint_count,
-            t1 = t1_4,
-            t2 = t2_4,
-            t3 = t3_4,
-            x1 = request.current_position,
-            v1 = request.current_velocity,
-            v2 = v1,
-            v3 =np.zeros((joint_count,)),
-            a1 = a1_4,
-            a3 = a3_4,
-            xf = None
-        )
-
-        return ret
-            
-
-    
-    @staticmethod
-    def solve_case5(v0, v1, vf, timeout, a_max):
-        t1 = 0.0
-        a1 = 0.0
-        if (v1 != v0):        
-            a1 = a_max * np.sign(v1 - v0)
-            t1 = (v1 - v0) / a1
-        
-        if (t1 > timeout):        
-            v1 = a1 * timeout
-            t1 = timeout        
-
-        t3 = 0
-        a3 = 0
-        if (vf != v1):        
-            a3 = a_max * np.sign(vf - v1)
-            t3 = (vf - v1) / a3        
-
-        t2 = timeout - t1
-
-        v1_res = v1
-
-        return True, v1_res, a1, a3, t1, t2, t3
-
-    @staticmethod
-    def solve_case6(v0, v1, vf, t1, t2, t3):
-        a1_den = t1
-        a1 = (v1-v0) / a1_den  if (a1_den != 0) else 0.0
-        a3 = 0
-        if (t3 != 0):        
-            a3 = (-a1 * t1 - v0 + vf) / t3
-
-        return a1, a3
-        
-
-
-class TrapezoidalJointTrajectoryGeneratorExec:
-    def __init__(self, joint_count, t1, t2, t3, x1, v1, v2, v3, a1, a3, xf):
-        self.joint_count = joint_count
-        self.t1 = t1
-        self.t2 = t2
-        self.t3 = t3
-        self.x1 = x1
-        self.v1 = v1
-        self.v2 = v2
-        self.v3 = v3
-        self.a1 = a1
-        self.a3 = a3
-        self.xf = xf
-        self.t_final = t1 + t2 +t3
-        self.x2 = None
-        self.x3 = None
-
-    @staticmethod
-    def pos_1(a, v, x, t):
-        return (0.5 * a * pow(t, 2) if a != 0 else 0.0) + v*t + x
-
-    @staticmethod
-    def vel_1(a, v, t):
-        return (a *t if a != 0 else 0.0) + v
-
-    @classmethod
-    def pos(cls, n, a, v, x, t):
-        o = np.zeros((n,))
-        for i in range(n):
-            if a is not None:
-                o[i] = cls.pos_1(a[i], v[i], x[i], t)
-            else:
-                o[i] = cls.pos_1(0.0, v[i], x[i], t)
-        
-        return o
-
-    @classmethod
-    def vel(cls, n, a, v, t):
-        o = np.zeros((n,))
-        for i in range(n):
-            if a is not None:
-                o[i] = cls.vel_1(a[i], v[i], t)
-            else:
-                o[i] = cls.vel_1(0.0, v[i], t)
-
-        return o
-
-    def calc_at_time(self, t):
-        if self.x2 is None:
-            self.x2 = self.pos(self.joint_count, self.a1, self.v1, self.x1, self.t1)
-
-        if self.x3 is None:
-            self.x3 = self.pos(self.joint_count, None, self.v2, self.x2, self.t2)
-
-        if self.xf is None:
-            self.xf = self.pos(self.joint_count, self.a3, self.v2, self.x3, self.t3)
-
-        if t < 0:
-            return False, None, None
-
-        if (t < self.t1):
-            x = self.pos(self.joint_count, self.a1, self.v1, self.x1, t)
-            v = self.vel(self.joint_count, self.a1, self.v1, t)
-            return True, x, v
-
-        if (t < self.t2 + self.t1):
-            x = self.pos(self.joint_count, None, self.v2, self.x2, t - self.t1)
-            v = self.vel(self.joint_count, None, self.v2, t - self.t1)
-            return True, x, v
-
-        if (t < self.t_final):
-            x = self.pos(self.joint_count, self.a3, self.v2, self.x3, t - self.t1 -self.t2)
-            v = self.vel(self.joint_count, self.a3, self.v2, t - self.t1 - self.t2)
-            return True, x, v
-
-        x = self.pos(self.joint_count, None, self.v3, self.xf, t - self.t_final)
-        v = self.vel(self.joint_count, None, self.v3, t - self.t_final)
-        return True, x, v
+# Copyright 2022 Wason Technology, LLC
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import numpy as np
+import RobotRaconteur as RR
+from typing import NamedTuple
+
+class JointTrajectoryLimits(NamedTuple):
+    j_max: np.array
+    a_max: np.array
+    v_max: np.array
+    x_min: np.array
+    x_max: np.array
+
+class JointTrajectoryPositionRequest(NamedTuple):
+    current_position: np.array
+    current_velocity: np.array
+    desired_position: np.array
+    desired_velocity: np.array
+    max_velocity: np.array
+    desired_time: float = None
+    speed_ratio: float = 1.
+    splice_time: float = None
+
+class JointTrajectoryVelocityRequest(NamedTuple):
+    current_position: np.array
+    current_velocity: np.array
+    desired_velocity: np.array
+    timeout: float
+    speed_ratio: float
+    desired_time: float = None
+
+class JointTrajectoryPositionCommand(NamedTuple):
+    command_position: np.array
+    command_velocity: np.array
+
+
+class TrapezoidalJointTrajectoryGenerator:
+
+    def __init__(self, joint_count, limits):
+        self._joint_count=joint_count
+        self._limits=limits
+
+        self._speed_ratio = 1.0
+        self._t_des = 0.0
+        self._exec = None
+
+    @property
+    def t_des(self):
+        return self._t_des
+
+    @property
+    def speed_ratio(self):
+        return self._speed_ratio
+
+    @property
+    def t_final(self):
+        if self._exec is not None:
+            return self._exec.t_final
+        else:
+            return 0.
+
+    @property
+    def is_valid(self):
+        return self._exec is not None
+
+    @property
+    def target_position(self):
+        return self._exec.xf
+
+    @property
+    def target_velocity(self):
+        return self._exec.v3
+
+    def get_command(self, t):
+        if self._exec is None:
+            return False, None
+
+        res, command_position, command_velocity = self._exec.calc_at_time(t)
+        if not res:
+            return False, None
+        command = JointTrajectoryPositionCommand(
+            command_position = command_position,
+            command_velocity = command_velocity
+        )
+
+        return True, command
+
+    def update_desired_position(self, request):
+        assert request.desired_time is None, "desired time not supported"
+        self._exec = TrapezoidalJointTrajectoryGeneratorCalc.initialize_pos_exec(self._joint_count, self._limits, request)
+        return True
+
+    def update_desired_velocity(self, request):
+        self._exec = TrapezoidalJointTrajectoryGeneratorCalc.initialize_vel_exec(self._joint_count, self._limits, request)
+        return True
+
+class TrapezoidalJointTrajectoryGeneratorCalc:
+    
+    @classmethod
+    def initialize_pos_exec(cls, joint_count, limits, request):
+        assert request.desired_time is None
+
+        a_max = np.copy(limits.a_max)
+        v_max = np.copy(limits.v_max)
+
+        if request.speed_ratio != 0.0:
+            a_max *= request.speed_ratio
+            v_max *= request.speed_ratio
+
+            if request.max_velocity is not None:
+                req_vel = request.max_velocity * request.speed_ratio
+                assert np.all(req_vel <= v_max), "req_vel must be less than or equal to v_max"
+                v_max = np.minimum(req_vel,v_max)
+
+        else:            
+            assert np.all(request.max_velocity <= v_max), "req_vel must be less than or equal to v_max"
+            v_max = np.minimum(request.max_velocity,v_max)
+
+        dx = request.desired_position - request.current_position
+
+        t1 = np.zeros((joint_count,))
+        t2 = np.zeros((joint_count,))
+        t3 = np.zeros((joint_count,))
+
+        v1 = np.zeros((joint_count,))
+        a1 = np.zeros((joint_count,))
+        a3 = np.zeros((joint_count,))
+
+        for i in range(joint_count):
+            if dx[i] == 0 and request.desired_velocity[i] == 0 and request.current_velocity[i] == 0:
+                continue
+
+            case2_success, v1[i], a1[i], a3[i], t1[i], t2[i], t3[i] = \
+                cls.solve_case2(
+                request.current_position[i], request.desired_position[i], request.current_velocity[i],
+                request.desired_velocity[i], v_max[i], a_max[i]
+            )
+
+            if not case2_success:
+                case3_success, a1[i], a3[i], t1[i], t3[i] = \
+                    cls.solve_case3(
+                    request.current_position[i], request.desired_position[i], request.current_velocity[i],
+                    request.desired_velocity[i], a_max[i]
+                )
+                t2[i] = 0
+                v1[i] = 0
+
+                assert case3_success, "Invalid trajectory request"
+
+        t1_4 = np.max(t1)
+        t2_4 = np.max(t2)
+        t3_4 = np.max(t3)
+
+        a1_4 = np.zeros((joint_count,))
+        a3_4 = np.zeros((joint_count,))
+        v1_4 = np.zeros((joint_count,))
+
+        for i in range(joint_count):
+            v1_4[i], a1_4[i], a3_4[i] = cls.solve_case4(
+                request.current_position[i], request.desired_position[i], request.current_velocity[i], 
+                request.desired_velocity[i], t1_4, t2_4, t3_4)
+
+        return TrapezoidalJointTrajectoryGeneratorExec(
+            joint_count = joint_count,
+            t1 = t1_4,
+            t2 = t2_4,
+            t3 = t3_4,
+            x1 = request.current_position,
+            v1 = request.current_velocity,
+            v2 = v1_4,
+            v3 = request.desired_velocity,
+            a1 = a1_4,
+            a3 = a3_4,
+            xf = request.desired_position
+        )
+
+    @staticmethod
+    def pos_1(a, v, x, t):
+        return (0.5 * a * pow(t, 2) if a != 0 else 0.0) + v*t + x
+
+    @staticmethod
+    def vel_1(a, v, t):
+        return (a *t if a != 0 else 0.0) + v
+
+    @classmethod
+    def pos(cls,a1, a3, x0, v0, t1, t2, t3):
+        v1_p = cls.vel_1(a1, v0, t1)
+        v3_p = cls.vel_1(a3, v1_p, t3)
+
+        x1_p = cls.pos_1(a1, v0, x0, t1)
+        x2_p = cls.pos_1(0, v1_p, x1_p, t2)
+        x3_p = cls.pos_1(a3, v1_p, x2_p, t3)
+
+        return x3_p, v3_p
+
+    @classmethod
+    def solve_case2_sub(cls, x0, xf, v0, v1, vf, a_max):
+        t1 = 0
+        a1 = 0
+        if v1 != v0:
+            a1 = a_max * np.sign(v1 - v0)
+            t1 = (v1-v0) / a1
+        
+        t3 = 0
+        a3 = 0
+        if vf != v1:
+            a3 = a_max * np.sign(vf-v1)
+            t3 = (vf - v1) / a3
+
+        xf_1, vf_1 = cls.pos(a1, a3, x0, v0, t1, 0.0, t3)
+
+        dx2 = xf - xf_1
+
+        t2 = dx2/v1
+
+        return t2 >= 0, a1, a3, t1, t2, t3
+
+    @classmethod
+    def solve_case2(cls, x0, xf, v0, vf, v_max, a_max):
+        case2_res, a1, a3, t1, t2, t3 = cls.solve_case2_sub(x0, xf, v0, v_max, vf, a_max)
+        if case2_res:
+            return True, v_max, a1, a3, t1, t2, t3
+
+        case2_res, a1, a3, t1, t2, t3 = cls.solve_case2_sub(x0, xf, v0, -v_max, vf, a_max)
+        if case2_res:
+            return True, -v_max, a1, a3, t1, t2, t3
+
+        return False, None, None, None, None, None, None
+
+
+    @staticmethod
+    def solve_case3_sub1(x0, xf, v0, vf, a1):
+        return a1 * (xf - x0) + 0.5 * pow(v0, 2.0) + 0.5 * pow(vf, 2.0)
+
+    @classmethod
+    def solve_case3(cls, x0, xf, v0, vf, a_max):
+        sub1 = cls.solve_case3_sub1(x0, xf, v0, vf, a_max)
+        if sub1 >= 0:
+            a1 = a_max
+            a3 = -a_max
+            t1 = (-v0 + np.sqrt(sub1)) / a1
+            t3 = (a1*t1 + v0-vf) / a1
+            if t1 > 0 and t3 > 0:
+                return True, a1, a3, t1, t3
+            t1 = (-v0 - np.sqrt(sub1))/ a1
+            t3 = a1 * (a1 * t1 + v0 - vf) / a1
+            if t1 > 0 and t3 > 0:
+                return True, a1, a3, t1, t3
+
+        sub1 = cls.solve_case3_sub1(x0, xf, v0, vf, -a_max)
+
+        if sub1 >= 0:
+            a1 = -a_max
+            a3 = a_max
+            t1 = (-v0 + np.sqrt(sub1)) / a1
+            t3 = (a1 * t1 + v0 - vf) / a1
+            if t1 > 0 and t3 > 0:
+                return True, a1, a3, t1, t3
+
+            t1 = (-v0 - np.sqrt(sub1)) / a1
+            t3 = (a1 * t1 + v0 - vf) / a1
+            if (t1 > 0 and t3 > 0):
+                return True, a1, a3, t1, t3
+
+        return False, None, None, None, None
+
+    @classmethod
+    def solve_case4(cls, x0, xf, v0, vf, t1, t2, t3):
+        a1_den = t1 * (t1 + 2*t2 + t3)
+        a1 = (-2 * t1 * v0 - 2 * t2 * v0 - t3 * v0 - t3 * vf - 2 * x0 + 2 * xf) / a1_den if a1_den !=0 else 0.0
+        v1 = a1 * t1 + v0
+        a3 = 0.0
+        if t3 != 0:
+            a3 = (-a1 * t1 - v0 + vf) / t3
+
+        return v1, a1, a3
+    
+    @classmethod
+    def initialize_vel_exec(cls, joint_count, limits, request):
+        a_max = np.copy(limits.a_max)
+        v_max = np.copy(limits.v_max)
+        if request.speed_ratio != 0.0:
+            a_max *= request.speed_ratio
+            v_max *= request.speed_ratio
+
+            req_vel = request.desired_velocity * request.speed_ratio
+            assert np.all(req_vel <= v_max), "req_vel must be less than or equal to v_max"
+            v_max = np.minimum(v_max, req_vel)
+
+        else:
+            assert np.all(request.max_velocity <= v_max), "req_vel must be less than or equal to v_max"
+            v_max = np.minimum(request.max_velocity,v_max)
+
+        t1 = np.zeros((joint_count,))
+        t2 = np.zeros((joint_count,))
+        t3 = np.zeros((joint_count,))
+
+        v1 = np.zeros((joint_count,))
+        a1 = np.zeros((joint_count,))
+        a3 = np.zeros((joint_count,))
+
+        for i in range(joint_count):
+            if request.desired_velocity[i] == 0 and request.current_velocity[i] == 0:
+                continue
+
+            a_max[i], v1[i], a1[i], a3[i], t1[i], t2[i], t3[i] = cls.solve_case5(request.current_velocity[i], 
+                request.desired_velocity[i], 0, request.timeout, a_max[i])
+
+        t1_4 = np.max(t1)
+        t2_4 = np.max(t2)
+        t3_4 = np.max(t3)
+
+        a1_4 = np.zeros((joint_count,))
+        a3_4 = np.zeros((joint_count,))
+
+        for i in range(joint_count):
+            a1_4[i], a3_4[i] = cls.solve_case6(request.current_velocity[i], v1[i], 0, t1_4, t2_4, t3_4)
+
+        ret = TrapezoidalJointTrajectoryGeneratorExec(
+            joint_count = joint_count,
+            t1 = t1_4,
+            t2 = t2_4,
+            t3 = t3_4,
+            x1 = request.current_position,
+            v1 = request.current_velocity,
+            v2 = v1,
+            v3 =np.zeros((joint_count,)),
+            a1 = a1_4,
+            a3 = a3_4,
+            xf = None
+        )
+
+        return ret
+            
+
+    
+    @staticmethod
+    def solve_case5(v0, v1, vf, timeout, a_max):
+        t1 = 0.0
+        a1 = 0.0
+        if (v1 != v0):        
+            a1 = a_max * np.sign(v1 - v0)
+            t1 = (v1 - v0) / a1
+        
+        if (t1 > timeout):        
+            v1 = a1 * timeout
+            t1 = timeout        
+
+        t3 = 0
+        a3 = 0
+        if (vf != v1):        
+            a3 = a_max * np.sign(vf - v1)
+            t3 = (vf - v1) / a3        
+
+        t2 = timeout - t1
+
+        v1_res = v1
+
+        return True, v1_res, a1, a3, t1, t2, t3
+
+    @staticmethod
+    def solve_case6(v0, v1, vf, t1, t2, t3):
+        a1_den = t1
+        a1 = (v1-v0) / a1_den  if (a1_den != 0) else 0.0
+        a3 = 0
+        if (t3 != 0):        
+            a3 = (-a1 * t1 - v0 + vf) / t3
+
+        return a1, a3
+        
+
+
+class TrapezoidalJointTrajectoryGeneratorExec:
+    def __init__(self, joint_count, t1, t2, t3, x1, v1, v2, v3, a1, a3, xf):
+        self.joint_count = joint_count
+        self.t1 = t1
+        self.t2 = t2
+        self.t3 = t3
+        self.x1 = x1
+        self.v1 = v1
+        self.v2 = v2
+        self.v3 = v3
+        self.a1 = a1
+        self.a3 = a3
+        self.xf = xf
+        self.t_final = t1 + t2 +t3
+        self.x2 = None
+        self.x3 = None
+
+    @staticmethod
+    def pos_1(a, v, x, t):
+        return (0.5 * a * pow(t, 2) if a != 0 else 0.0) + v*t + x
+
+    @staticmethod
+    def vel_1(a, v, t):
+        return (a *t if a != 0 else 0.0) + v
+
+    @classmethod
+    def pos(cls, n, a, v, x, t):
+        o = np.zeros((n,))
+        for i in range(n):
+            if a is not None:
+                o[i] = cls.pos_1(a[i], v[i], x[i], t)
+            else:
+                o[i] = cls.pos_1(0.0, v[i], x[i], t)
+        
+        return o
+
+    @classmethod
+    def vel(cls, n, a, v, t):
+        o = np.zeros((n,))
+        for i in range(n):
+            if a is not None:
+                o[i] = cls.vel_1(a[i], v[i], t)
+            else:
+                o[i] = cls.vel_1(0.0, v[i], t)
+
+        return o
+
+    def calc_at_time(self, t):
+        if self.x2 is None:
+            self.x2 = self.pos(self.joint_count, self.a1, self.v1, self.x1, self.t1)
+
+        if self.x3 is None:
+            self.x3 = self.pos(self.joint_count, None, self.v2, self.x2, self.t2)
+
+        if self.xf is None:
+            self.xf = self.pos(self.joint_count, self.a3, self.v2, self.x3, self.t3)
+
+        if t < 0:
+            return False, None, None
+
+        if (t < self.t1):
+            x = self.pos(self.joint_count, self.a1, self.v1, self.x1, t)
+            v = self.vel(self.joint_count, self.a1, self.v1, t)
+            return True, x, v
+
+        if (t < self.t2 + self.t1):
+            x = self.pos(self.joint_count, None, self.v2, self.x2, t - self.t1)
+            v = self.vel(self.joint_count, None, self.v2, t - self.t1)
+            return True, x, v
+
+        if (t < self.t_final):
+            x = self.pos(self.joint_count, self.a3, self.v2, self.x3, t - self.t1 -self.t2)
+            v = self.vel(self.joint_count, self.a3, self.v2, t - self.t1 - self.t2)
+            return True, x, v
+
+        x = self.pos(self.joint_count, None, self.v3, self.xf, t - self.t_final)
+        v = self.vel(self.joint_count, None, self.v3, t - self.t_final)
+        return True, x, v
```

## Comparing `robotraconteur_abstract_robot-0.2.0.dist-info/LICENSE.txt` & `robotraconteur_abstract_robot-0.2.1.dist-info/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022 Wason Technology, LLC
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+                                Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 Wason Technology, LLC
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

## Comparing `robotraconteur_abstract_robot-0.2.0.dist-info/METADATA` & `robotraconteur_abstract_robot-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotraconteur-abstract-robot
-Version: 0.2.0
+Version: 0.2.1
 Summary: Robot Raconteur Python Abstract Robot and Abstract Tool
 Home-page: https://github.com/robotraconteur/robotraconteur_abstract_robot_python
 Author: John Wason
 Author-email: wason@wasontech.com
 License-File: LICENSE.txt
 Requires-Dist: RobotRaconteur
 Requires-Dist: RobotRaconteurCompanion
```

