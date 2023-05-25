# Comparing `tmp/multirotor-0.3.1.tar.gz` & `tmp/multirotor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multirotor-0.3.1.tar", last modified: Thu Apr 20 20:46:32 2023, max compression
+gzip compressed data, was "multirotor-0.4.0.tar", last modified: Thu May 25 19:18:48 2023, max compression
```

## Comparing `multirotor-0.3.1.tar` & `multirotor-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-04-20 20:46:32.349427 multirotor-0.3.1/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2023-04-20 20:46:32.349427 multirotor-0.3.1/PKG-INFO
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      823 2022-09-06 21:25:06.000000 multirotor-0.3.1/README.md
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-04-20 20:46:32.349427 multirotor-0.3.1/multirotor/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-06 21:25:06.000000 multirotor-0.3.1/multirotor/__init__.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     2484 2022-12-12 19:19:30.000000 multirotor-0.3.1/multirotor/coords.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     5515 2022-10-31 21:18:20.000000 multirotor-0.3.1/multirotor/env.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    16306 2023-04-11 13:43:29.000000 multirotor-0.3.1/multirotor/helpers.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     6548 2022-12-08 18:45:12.000000 multirotor-0.3.1/multirotor/physics.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    22647 2023-04-20 20:03:48.000000 multirotor-0.3.1/multirotor/simulation.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     9247 2023-03-18 19:01:32.000000 multirotor-0.3.1/multirotor/trajectories.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     5418 2023-04-11 13:45:56.000000 multirotor-0.3.1/multirotor/vehicle.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    12609 2023-04-07 17:31:02.000000 multirotor-0.3.1/multirotor/visualize.py
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-04-20 20:46:32.349427 multirotor-0.3.1/multirotor.egg-info/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/PKG-INFO
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      407 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/SOURCES.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        1 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/dependency_links.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      102 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/requires.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       11 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/top_level.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       81 2022-09-06 21:25:06.000000 multirotor-0.3.1/pyproject.toml
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      486 2023-04-20 20:46:32.353427 multirotor-0.3.1/setup.cfg
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-05-25 19:18:48.300461 multirotor-0.4.0/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2023-05-25 19:18:48.300461 multirotor-0.4.0/PKG-INFO
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      823 2022-09-06 21:25:06.000000 multirotor-0.4.0/README.md
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-05-25 19:18:48.300461 multirotor-0.4.0/multirotor/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-06 21:25:06.000000 multirotor-0.4.0/multirotor/__init__.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     2484 2022-12-12 19:19:30.000000 multirotor-0.4.0/multirotor/coords.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     8813 2023-05-25 18:30:50.000000 multirotor-0.4.0/multirotor/env.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    16660 2023-05-25 17:45:38.000000 multirotor-0.4.0/multirotor/helpers.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    15815 2023-05-25 18:01:00.000000 multirotor-0.4.0/multirotor/optimize.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     6604 2023-04-21 20:33:09.000000 multirotor-0.4.0/multirotor/physics.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    22940 2023-05-04 21:54:19.000000 multirotor-0.4.0/multirotor/simulation.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     9821 2023-05-03 15:46:07.000000 multirotor-0.4.0/multirotor/trajectories.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     5418 2023-04-11 13:45:56.000000 multirotor-0.4.0/multirotor/vehicle.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    14409 2023-05-04 15:21:26.000000 multirotor-0.4.0/multirotor/visualize.py
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-05-25 19:18:48.300461 multirotor-0.4.0/multirotor.egg-info/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/PKG-INFO
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      430 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        1 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      109 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/requires.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       11 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/top_level.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       81 2022-09-06 21:25:06.000000 multirotor-0.4.0/pyproject.toml
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      494 2023-05-25 19:18:48.304461 multirotor-0.4.0/setup.cfg
```

### Comparing `multirotor-0.3.1/PKG-INFO` & `multirotor-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multirotor
-Version: 0.3.1
+Version: 0.4.0
 Summary: Simulation testbed for multirotor vehicles.
 Keywords: multirotor,simulation,gym,uav
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
 Provides-Extra: CONTROL
```

### Comparing `multirotor-0.3.1/README.md` & `multirotor-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `multirotor-0.3.1/multirotor/coords.py` & `multirotor-0.4.0/multirotor/coords.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.3.1/multirotor/helpers.py` & `multirotor-0.4.0/multirotor/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,17 @@
         prop_angular_velocity=max_rads
     )
     torques = (torques * (torques > 0)).sum(axis=1)
     I = vp.inertia_matrix.diagonal()
     # t = i a
     ang_acc = torques / I
 
+    # TODO: max angular velocity such that can accelerate to and decelerate from it
+    # to 0
+
     res = dict(
         max_acc_xy=max_acc_xy,
         max_acc_z=max_acc_z,
         max_ang_acc=max(ang_acc)
     )
     return res
 
@@ -333,14 +336,21 @@
             setattr(self, '_' + str(arg), [])
         self._target = dict(
             position=[], velocity=[], orientation=[], rate=[]
         )
         self.vehicle = vehicle
         self.controller = controller
 
+
+    def __getitem__(self, item):
+        if isinstance(item, slice):
+            d = DataLog(other_vars=self._args)
+            pass
+        # TODO: Finish. Return a DataLog with the requested slice
+
         
     def log(self, **kwargs):
         """
         Add the state and action variables from the Multirotor and Controller.
         Any keyword arguments should already have been registered in `track()`
         and their values are now appended to the list.
 
@@ -413,21 +423,22 @@
                 a1 = getattr(self.target, k)
                 a2 = getattr(log.target, k)
                 a = np.concatenate((a1, a2), dtype=self.vehicle.dtype)
                 d[k] = a
             self.target = SimpleNamespace(**d)
 
         if relative:
-            last_time = self.times[old_len - 1]
             # last_pos = self.position[old_len - 1]
             if not self._arrayed:
+                last_time = self._times[old_len - 1]
                 for i in range(old_len, len(self)):
                         # self._states[i][:3] += last_pos
                         self._times[i] += last_time
             elif self._arrayed:
+                last_time = self.times[old_len - 1]
                 # self.states[old_len:,:3] += last_pos
                 self.times[old_len:] += last_time
 
             
     def _make_arrays(self, relative_to=None):
         """
         Convert python list to array and put up a flag that all arrays are up
```

### Comparing `multirotor-0.3.1/multirotor/physics.py` & `multirotor-0.4.0/multirotor/physics.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,16 @@
     # then undoing it for result:
     tau = np.cross(position_vector.T, force.T).T
     tau[2] = tau[2] + tau_rot
     return tau
 
 
 
-@njit
-def apply_forces_torques(
+# @njit
+def _apply_forces_torques(
     forces: np.ndarray, torques: np.ndarray, x: np.ndarray, g: float, mass: float,
     inertia_matrix: np.matrix, inertia_matrix_inverse: np.matrix
 ) -> np.ndarray:
     """
     Given forces and torqes, return the rate of change of state.
 
     Parameters
@@ -181,7 +181,10 @@
     xdot[8] = (q * sphi + r * cphi) / cthe  # = psidot
 
     # Angular rate
     gyro = np.cross(x[9:12], I @ x[9:12])
     xdot[9:12] = I_inv @ (torques - gyro)
     
     return xdot
+
+
+apply_forces_torques = njit(_apply_forces_torques)
```

### Comparing `multirotor-0.3.1/multirotor/simulation.py` & `multirotor-0.4.0/multirotor/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,15 @@
         for params in self.params.propellers:
             self.propellers.append(Propeller(params, self.simulation))
 
         if self.params.battery is not None:
             self.battery = Battery(self.params.battery, self.simulation)
         else:
             self.battery = Battery(BatteryParams(max_voltage=np.inf), self.simulation)
+        self.alloc, self.alloc_inverse = control_allocation_matrix(self.params)
         self.reset()
 
 
     def reset(self) -> np.ndarray:
         """
         Reset the state of the vehicle. This includes resetting each propeller
         and re-calculating inertia and allocation matrices.
@@ -292,18 +293,17 @@
         """
         self.t = 0.
         for p in self.propellers:
             p.reset()
         if self.battery is not None:
             self.battery.reset()
 
-        self.alloc, self.alloc_inverse = control_allocation_matrix(self.params)
         self.alloc = self.alloc.astype(self.dtype)
-        self.params.propeller_vectors = self.params.propeller_vectors.astype(self.dtype)
         self.alloc_inverse = self.alloc_inverse.astype(self.dtype)
+        self.params.propeller_vectors = self.params.propeller_vectors.astype(self.dtype)
         self.params.inertia_matrix = self.params.inertia_matrix.astype(self.dtype)
         self.params.inertia_matrix_inverse = self.params.inertia_matrix_inverse.astype(self.dtype)
         self.state = np.zeros(12, dtype=self.dtype)
         self._dxdt = np.zeros_like(self.state)
         return self.state
 
 
@@ -371,14 +371,23 @@
         peak_voltage = self.battery.params.max_voltage
         currents = np.asarray([p.motor.current for p in self.propellers])
         voltages = np.asarray([p.motor.voltage for p in self.propellers])
         duty_cycle = voltages / peak_voltage
         return np.sum(duty_cycle * currents)
 
 
+    @property
+    def speeds(self) -> np.ndarray:
+        return np.asarray([p.speed for p in self.propellers], self.dtype)
+    @speeds.setter
+    def speeds(self, speeds: np.ndarray):
+        for s, p in zip(speeds, self.propellers):
+            p.step(s, max_voltage=self.battery.voltage)
+
+
     def get_forces_torques(self, speeds: np.ndarray, state: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         """
         Calculate the forces and torques acting on the vehicle's center of gravity
         given its current state and speed of propellers.
 
         Parameters
         ----------
```

### Comparing `multirotor-0.3.1/multirotor/trajectories.py` & `multirotor-0.4.0/multirotor/trajectories.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             points = self.points
         points = np.asarray([p[:3] for p in points])
         if self.resolution is not None:
             _points = []
             for i, (p1, p2) in enumerate(zip(points[:-1], points[1:])):
                 pos_vec = p2 - p1
                 dist = np.linalg.norm(pos_vec)
-                unit_vec = pos_vec / dist
+                unit_vec = pos_vec / (dist + 1e-6)
                 # num = int(dist / self.resolution) + 1
                 number = dist // self.resolution
                 remainder  = dist % self.resolution
                 pts = p1 + unit_vec * self.resolution * np.arange(0, number+1, step=1).reshape(-1,1)
                 if remainder > 0 and i==len(points)-2: # if leftover distance and last point
                     pts = np.concatenate((pts, (p2,)))
                 # pts = p1 + unit_vec * np.arange(0, dist + self.resolution, step=self.resolution).reshape(-1,1)
@@ -223,7 +223,32 @@
                     i += 1 # steps since beginning of trajectory
                     j += 1 # steps since last trajectory replan
                     yield self._ref, velocity
 
 
     def reached(self, wp: np.ndarray) -> bool:
         return np.linalg.norm(self.vehicle.position - wp) <= self.proximity
+
+
+
+def eight_curve(a: float=10, N:int=20) -> np.ndarray:
+    """
+    Generate a list of points following the Eight curve pattern.
+
+    Parameters
+    ----------
+    a : int, optional
+        The scale of the curve, by default 50
+    N : int, optional
+        Number of points to generate, by default 20
+
+    Returns
+    -------
+    np.ndarray
+        A Nx3 array of points.
+    """
+    wp = np.zeros((N, 3), np.float32)
+    t = np.linspace(0, 2 * np.pi, N)
+    wp[:,0] = a * np.sin(t)
+    wp[:,1] = a * np.sin(t) * np.cos(t)
+    wp[:,2] = np.zeros(N)
+    return wp
```

### Comparing `multirotor-0.3.1/multirotor/vehicle.py` & `multirotor-0.4.0/multirotor/vehicle.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.3.1/multirotor/visualize.py` & `multirotor-0.4.0/multirotor/visualize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from typing import Tuple, Union
+from typing import Tuple, Union, Dict
 import threading as th
 import multiprocessing as mp
 import queue
 from dataclasses import dataclass
 import time
 
 import numpy as np
 import matplotlib.pyplot as plt
-from tqdm.autonotebook import tqdm
 from matplotlib.animation import FuncAnimation
 from mpl_toolkits.mplot3d import Axes3D
 from mpl_toolkits.mplot3d.art3d import Line3D
+from matplotlib.lines import Line2D
 
 from .coords import body_to_inertial, direction_cosine_matrix
 from .simulation import Multirotor
-from .trajectories import Trajectory, GuidedTrajectory
-from .controller import Controller
+from .vehicle import VehicleParams
 from .helpers import DataLog
 
 
 
 def plot_datalog(log: DataLog, figsize=(21,10.5),
     plots=('pos', 'vel', 'ctrl', 'traj'),
-    nrows=2, ncols=None):
+    nrows=2, ncols=None) -> Dict[str, plt.Axes]:
     """
     Plot recorded values from a Multirotor's flight. Including:
 
     1. Position and orientation,
     2. Motor speeds,
     3. Velocity in world frame,
     4. Control allocation,
@@ -35,27 +34,33 @@
 
     Parameters
     ----------
     log : DataLog
         The datalog, where `datalog.done_logging()` has been called.
     figsize : tuple, optional
         The x/y dimensions of the figure, by default (21,10.5)
+    
+    Returns
+    -------
+    Dict : Dict[str, plt.Axes]
+        A dictionary of plot names mapping to Axes
     """
     nplots = len(plots)
     if nrows is None and ncols is not None:
         nrows = nplots // ncols + (nplots % ncols !=0)
     elif nrows is not None and ncols is None:
         ncols = nplots // nrows + (nplots % nrows !=0)
 
     plt.figure(figsize=figsize)
     plot_grid = (nrows, ncols)
 
     n = len(log)
     hasctrl = log.controller is not None
     plot_number = 1
+    axes = {}
 
     # Positions
     if 'pos' in plots:
         plt.subplot(*plot_grid,plot_number)
         plt.plot(log.t, log.x, label='x', c='r')
         plt.plot(log.t, log.y, label='y', c='g')
         plt.plot(log.t, log.z, label='z', c='b')
@@ -72,14 +77,15 @@
             plt.plot(log.t, log.target.orientation[:,0] * (180 / np.pi), c='c', ls=':')
             plt.plot(log.t, log.target.orientation[:,1] * (180 / np.pi), c='m', ls=':')
             plt.plot(log.t, log.target.orientation[:,2] * (180 / np.pi), c='y', ls=':')
         plt.ylabel('Orientation /deg')
         plt.legend(handles=plt.gca().lines[:3] + lines, ncol=2)
         plt.title('Position and Orientation')
         plot_number += 1
+        axes['pos'] = plt.gca()
 
     if 'vel' in plots:
         plt.subplot(*plot_grid, plot_number)
         v_world, v_ref = np.zeros_like(log.velocity), np.zeros_like(log.velocity)
         for i, (v, o) in enumerate(zip(log.velocity, log.orientation)):
             dcm = direction_cosine_matrix(*o)
             v_world[i] = body_to_inertial(v, dcm)
@@ -90,39 +96,83 @@
             l, = plt.plot(log.t, v_world[:,i], label='Velocity %s' % a, c=c)
             if hasctrl:
                 plt.plot(log.t, v_ref[:,i], ls=':', c=l.get_c())
         #     plt.plot(velocities[:,i], label='Velocity %s' % a, c=c)
         plt.legend()
         plt.title('Velocities')
         plot_number += 1
+        axes['vel'] = plt.gca()
 
     if 'ctrl' in plots:
         plt.subplot(*plot_grid, plot_number)
         plt.title('Controller allocated dynamics')
         l = plt.plot(log.t, log.actions[:,0], label='Ctrl Thrust')
         plt.ylabel('Force /N')
         plt.twinx()
         for i, c, a in zip(range(3), 'rgb', 'xyz'):
             plt.plot(log.t, log.actions[:,1+i], label='Ctrl Torque %s' % a, c=c)
         plt.ylabel('Torque /Nm')
         plt.legend(handles=plt.gca().lines + l, ncol=2)
         plot_number += 1
+        axes['ctrl'] = plt.gca()
 
     if 'traj' in plots:
         plt.subplot(*plot_grid, plot_number)
         plt.plot(log.target.position[:,0], log.target.position[:,1], label='Prescribed traj', ls=':')
         plt.plot(log.x, log.y, label='Actual traj', ls='-')
         plt.gca().set_aspect('equal', 'box')
         plt.title('XY positions /m')
         plt.xlabel('X /m')
         plt.ylabel('Y /m')
         plt.legend()
         plot_number += 1
+        axes['traj'] = plt.gca()
 
     plt.tight_layout()
+    return axes
+
+
+
+def get_wind_quiver(heading: str, ax: plt.Axes, n=5, dim=2):
+    """
+    Create arrays of x,y,z coordinates for a quiver plot of wind.
+
+    Parameters
+    ----------
+    heading : str
+        The heading of the wind, e.g. '5@45' for 5N wind from 45 degrees.
+    ax : plt.Axes
+        The axes on which to plot the quiver.
+    n : int, optional
+        Size of arrays, by default 5
+    dim : int, optional
+        Dimension of quiver (2 or 3), by default 2
+
+    Returns
+    -------
+    Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]
+        x,y,[z],dx,dy,[dz] coordinates for quiver plot.
+    """
+    magnitude, angle = heading.split('@')
+    magnitude = float(magnitude)
+    if magnitude==0:
+        return (0,0,0,0) if dim==2 else (0,0,0,0,0,0)
+    angle = float(angle) * np.pi / 180
+    dx, dy = -np.cos(angle), -np.sin(angle)
+    xlim, ylim = ax.get_xlim(), ax.get_ylim()
+    if dim==3:
+        zlim = ax.get_zlim()
+        dz = 0
+        x,y,z = np.meshgrid(np.linspace(*xlim, num=n), np.linspace(*ylim, num=n), np.linspace(*zlim, num=n),
+                      indexing='xy')
+        return x,y,z,dx,dy,dz
+    else:
+        x,y = np.meshgrid(np.linspace(*xlim, num=n), np.linspace(*ylim, num=n),
+                      indexing='xy')
+        return x,y,dx,dy
 
 
 
 @dataclass
 class VehicleDrawing:
     vehicle: Multirotor
     axis: Axes3D = None
@@ -134,15 +184,15 @@
         self.t = self.vehicle.t
         self.params = self.vehicle.params
         self.interval = 1 / self.max_frames_per_second
         self.is_terminal = is_terminal()
         self.arm_lines, self.arm_lines_points, \
         self.trajectory_line, \
         self.axis_lines, self.axis_lines_points = \
-            make_drawing(self, self.body_axes)
+            make_drawing(self.params, self.body_axes)
         self.trajectory = [[], [], []] # [[X,..], [Y,...], [Z,...]]
 
 
     def connect(self, via: str ='animation') -> Union[FuncAnimation, th.Thread]:
         self.connection_via = via
         self.ev_cancel = mp.Event()
         self.queue = mp.Queue(maxsize=1)
@@ -256,47 +306,50 @@
                 pass
             end = time.time()
             self.ev_cancel.wait(max(0, self.interval - (end - start)))
         self.queue.close()
         
 
 
-def make_drawing(drawing: VehicleDrawing, body_axes: bool=False):
-    params = drawing.params
-    arm_lines_points = np.zeros((len(params.propellers) * 2, 3)) # [2 points/ propeller, axis]
+def make_drawing(params: VehicleParams, body_axes: bool=False, make_2d: bool=False, scale_arms=1.):
+    Line = Line3D if not make_2d else Line2D
+    arm_lines_points = np.zeros((len(params.propellers) * 2, 2 if make_2d else 3)) # [2 points/ propeller, axis]
     x = params.distances * np.cos(params.angles)
     y = params.distances * np.sin(params.angles)
     arm_lines_points[1::2,0] = x
     arm_lines_points[1::2,1] = y
+    arm_lines_points *=  scale_arms
     arm_lines = []
     for i in range(len(params.propellers)):
         arm_lines.append(
-            Line3D(
+            Line(
                 arm_lines_points[2*i:2*i+2,0],
                 arm_lines_points[2*i:2*i+2,1],
-                arm_lines_points[2*i:2*i+2,2],
-                antialiased=False))
+                antialiased=False),
+                **({'zs':arm_lines_points[2*i:2*i+2,2]} if not make_2d else {}),
+            )
 
-    trajectory_line = Line3D([], [], [], linewidth=0.5, color='black', linestyle=':')
+    trajectory_line = Line([], [], linewidth=0.5, color='black', linestyle=':',
+                           **({'zs':[]} if not make_2d else {}))
 
     axis_lines_points = np.zeros((6, 3)) # [2 points/ axis, axis]
     axis_lines_points[1::2] = np.eye(3)
     axis_lines = []
     for i, c in enumerate(['r', 'g', 'b']):
         if body_axes:
-            axis_lines.append(Line3D(
+            axis_lines.append(Line(
                 axis_lines_points[2*i:2*i+2,0],
                 axis_lines_points[2*i:2*i+2,1],
-                axis_lines_points[2*i:2*i+2,2],
                 antialiased=False,
                 linewidth=0.5,
-                color=c
+                color=c,
+                **({'zs':axis_lines_points[2*i:2*i+2,2]} if not make_2d else {}),
             )) 
         else:
-            axis_lines.append(Line3D([], [], []))
+            axis_lines.append(Line([], [], **({'zs':[]} if not make_2d else {})))
 
     return arm_lines, arm_lines_points, trajectory_line, axis_lines, axis_lines_points
 
 
 
 def update_drawing(drawing: VehicleDrawing, position: np.ndarray, orientation: np.ndarray):
     dcm = direction_cosine_matrix(orientation[0], orientation[1], orientation[2])
```

### Comparing `multirotor-0.3.1/multirotor.egg-info/PKG-INFO` & `multirotor-0.4.0/multirotor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multirotor
-Version: 0.3.1
+Version: 0.4.0
 Summary: Simulation testbed for multirotor vehicles.
 Keywords: multirotor,simulation,gym,uav
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
 Provides-Extra: CONTROL
```

