# Comparing `tmp/pose3d-2.1.0.tar.gz` & `tmp/pose3d-2.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pose3d-2.1.0.tar", last modified: Mon Feb 20 08:48:08 2023, max compression
+gzip compressed data, was "pose3d-2.1.1a0.tar", max compression
```

## Comparing `pose3d-2.1.0.tar` & `pose3d-2.1.1a0.tar`

### file list

```diff
@@ -1,24 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 08:48:08.000000 pose3d-2.1.0/
--rw-rw-rw-   0        0        0     1094 2023-02-17 12:41:19.000000 pose3d-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1075 2023-02-20 08:48:08.000000 pose3d-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-02-17 12:41:19.000000 pose3d-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-20 08:48:08.000000 pose3d-2.1.0/demo/
--rw-rw-rw-   0        0        0      117 2023-02-17 12:41:19.000000 pose3d-2.1.0/demo/__init__.py
--rw-rw-rw-   0        0        0      487 2023-02-17 12:41:19.000000 pose3d-2.1.0/demo/rotate_stuff.py
--rw-rw-rw-   0        0        0      162 2023-02-17 12:41:19.000000 pose3d-2.1.0/demo/transform_stuff.py
-drwxrwxrwx   0        0        0        0 2023-02-20 08:48:08.000000 pose3d-2.1.0/pose3d/
--rw-rw-rw-   0        0        0      139 2023-02-20 08:44:05.000000 pose3d-2.1.0/pose3d/__init__.py
--rw-rw-rw-   0        0        0    11227 2023-02-20 08:44:10.000000 pose3d-2.1.0/pose3d/er.py
--rw-rw-rw-   0        0        0     6765 2023-02-20 08:44:10.000000 pose3d-2.1.0/pose3d/et.py
--rw-rw-rw-   0        0        0     2416 2023-02-20 08:44:10.000000 pose3d-2.1.0/pose3d/pose.py
--rw-rw-rw-   0        0        0     5064 2023-02-20 08:44:10.000000 pose3d-2.1.0/pose3d/transform.py
--rw-rw-rw-   0        0        0     7000 2023-02-20 08:44:10.000000 pose3d-2.1.0/pose3d/transform_set.py
--rw-rw-rw-   0        0        0      620 2023-02-20 08:44:10.000000 pose3d-2.1.0/pose3d/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-20 08:48:08.000000 pose3d-2.1.0/pose3d.egg-info/
--rw-rw-rw-   0        0        0     1075 2023-02-20 08:48:07.000000 pose3d-2.1.0/pose3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-02-20 08:48:08.000000 pose3d-2.1.0/pose3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 08:48:07.000000 pose3d-2.1.0/pose3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-02-20 08:48:07.000000 pose3d-2.1.0/pose3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-20 08:48:07.000000 pose3d-2.1.0/pose3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-20 08:48:08.000000 pose3d-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1264 2023-02-20 08:44:10.000000 pose3d-2.1.0/setup.py
+-rw-r--r--   0        0        0     1073 2023-03-04 10:32:55.657329 pose3d-2.1.1a0/LICENSE
+-rw-r--r--   0        0        0      412 2023-03-04 10:32:55.657393 pose3d-2.1.1a0/README.md
+-rw-r--r--   0        0        0      134 2023-03-04 10:32:55.658906 pose3d-2.1.1a0/pose3d/__init__.py
+-rw-r--r--   0        0        0    11316 2023-05-25 17:18:42.326499 pose3d-2.1.1a0/pose3d/er.py
+-rw-r--r--   0        0        0     6589 2023-05-25 17:16:20.866753 pose3d-2.1.1a0/pose3d/et.py
+-rw-r--r--   0        0        0     2344 2023-05-25 17:15:18.316495 pose3d-2.1.1a0/pose3d/pose.py
+-rw-r--r--   0        0        0     4921 2023-05-25 17:12:54.769996 pose3d-2.1.1a0/pose3d/transform.py
+-rw-r--r--   0        0        0     6810 2023-05-25 17:13:54.121857 pose3d-2.1.1a0/pose3d/transform_set.py
+-rw-r--r--   0        0        0      597 2023-05-25 17:12:44.209814 pose3d-2.1.1a0/pose3d/utils.py
+-rw-r--r--   0        0        0      555 2023-05-25 17:49:03.895610 pose3d-2.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 pose3d-2.1.1a0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pose3d-2.1.0/LICENSE` & `pose3d-2.1.1a0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 John Halazonetis
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 John Halazonetis
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pose3d-2.1.0/pose3d/er.py` & `pose3d-2.1.1a0/pose3d/er.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,324 +1,353 @@
-import numpy as np
-from scipy.spatial.transform import Rotation
-from .utils import ER_TOLERANCE, valid_dim
-
-from typing import Union
-
-class ER:
-    def __init__(self, name: str = '', dim: int = 3) -> None:
-        '''
-        The `__init__` function is called when a new instance of the `RE` class is created.
-        It initializes all of the variables in the class and sets them to their default values.
-
-        By default, the `self.__rotation` member value is set to an identity value.
-
-        Parameters
-        ----------
-        - `name` (`str`): Set the name of the object (default: '')
-        - `dim` (`int`): Set the dimension of the vector (default: 3)
-        '''
-        self.name = name
-        self.__rotation = Rotation(quat=[0, 0, 0, 1])
-        self.identity()
-
-        if valid_dim(dim):
-            self.__dim = dim
-
-    # Setter functions
-    def identity(self) -> None:
-        '''
-        The `identity` function sets the `self.__rotation` member to
-        the equivalent of an identity matrix.
-        '''
-        self.__rotation = Rotation.identity()
-
-    def inv(self) -> None:
-        '''
-        The `inv` function sets the `self.__rotation` member to its inverse.
-        '''
-        self.__rotation = self.__rotation.inv()
-
-    def random(self) -> None:
-        '''
-        The `random` function sets the `self.__rotation` member to a random value.
-        '''
-        if self.dim == 2:
-            self.__rotation.from_euler('z', np.random.uniform(0, 360))
-
-        else:
-            self.__rotation = Rotation.random()
-
-    def from_quat(self, quat: Union[np.ndarray, list]) -> None:
-        '''
-        The `from_quat` function set the `self.__rotation` member from the value of
-        the input `quat`.
-
-        Note: This function will not work for `RE` objects that are defined in 2D space.
-
-        Parameters
-        ----------
-        - `quat` (`Union[np.ndarray, list]`): Input quaternion
-        '''
-        if self.__dim == 2:
-            raise AttributeError('Unable to set 2D rotation from quaternion input.')
-
-        if len(quat) != 4:
-            raise ValueError(f'Input vector shape must be equal to 4 (input shape: {len(quat)}).')
-
-        self.__rotation = Rotation.from_quat(np.array(quat))
-
-    def from_matrix(self, matrix: np.ndarray) -> None:
-        '''
-        The `from_matrix` function set the `self.__rotation` member from the value of
-        the input `matrix`. The function will first check whether the input matrix dimensions
-        are suitable for the number of dimensions set for the `RE` object.
-
-        Parameters
-        ----------
-        - `matrix` (`np.ndarray`): Input matrix
-        '''
-        if matrix.shape != (self.dim, self.dim):
-            raise ValueError(f'Input matrix shape must be ({self.dim}, {self.dim}) when rotation dimension is {self.dim}. Current input matrix shape: {matrix.shape}.')
-
-        if self.dim == 2:
-            matrix = np.hstack((np.array(matrix), np.zeros(shape=(2,1))))
-            matrix = np.vstack((np.array(matrix), [0, 0, 1]))
-
-        self.__rotation = Rotation.from_matrix(matrix)
-
-    def from_angle_axis(self, angle_axis: np.ndarray) -> None:
-        '''
-        The `from_angle_axis` function set the `self.__rotation` member from the value of
-        the input `angle_axis`.
-
-        Note: This function will not work for `RE` objects that are defined in 2D space.
-
-        Parameters
-        ----------
-        - `angle_axis` (`np.ndarray`): Input angle-axis vector
-        '''
-        if self.dim == 2:
-            raise AttributeError('Unable to set 2D rotation from angle-axis input.')
-
-        if len(angle_axis) != 3:
-            raise ValueError(f'Input vector shape must be equal to 3 (input shape: {len(angle_axis)}).')
-
-        self.__rotation = Rotation.from_rotvec(np.array(angle_axis) / np.linalg.norm(angle_axis))
-
-    def from_euler(self, sequence: str = None, angles: Union[np.ndarray, list] = None, degrees: bool = True) -> None:
-        '''
-        The `from_euler` function set the `self.__rotation` member from the value(s) of
-        the inputs `sequence` and `angles`. The angle will be converted from degrees to
-        radians if `degrees` is `True`.
-
-        Parameters
-        ----------
-        - `sequence` (`str`): Sequence of euler angles (e.g. 'xyz', 'xy', 'zyx')
-        - `angles` (`Union[np.ndarray, list]`): List of euler angles
-        - `degrees` (`bool`): Set to true if input angles are in degrees (default: `True`)
-        '''
-        if angles is None:
-            raise ValueError('Input angles cannot be None.')
-
-        if self.dim == 3:
-            if sequence is None:
-                raise ValueError('Input sequence cannot be None.')
-
-            self.__rotation = Rotation.from_euler(sequence, np.array(angles), degrees)
-
-        elif self.dim == 2:
-            self.__rotation = Rotation.from_euler('z', np.array(angles), degrees)
-
-    # Getter functions
-    @property
-    def dim(self) -> int:
-        '''
-        Return the number of dimensions.
-
-        Returns
-        -------
-        - `int`: Value of `self.__dim` member
-        '''
-        return self.__dim
-
-    def as_quat(self) -> np.ndarray:
-        '''
-        Return the stored `self.__rotation` member in quaternion form.
-
-        Returns
-        -------
-        - `np.ndarray`: Quaternion vector
-        '''
-        return self.__rotation.as_quat()
-
-    def as_matrix(self) -> np.ndarray:
-        '''
-        Return the stored `self.__rotation` member in matrix form.
-
-        Returns
-        -------
-        - `np.ndarray`: Rotation matrix
-        '''
-        return self.__rotation.as_matrix()[:self.dim, :self.dim]
-
-    def as_angle_axis(self, normalized: bool = True) -> np.ndarray:
-        '''
-        Return the stored `self.__rotation` member in angle-axis form.
-
-        Parameters
-        ----------
-        - `normalized` (`bool`): Return a normalized vector (Defaults to `True`)
-
-        Returns
-        -------
-        - `np.ndarray`: Angle-axis vector
-        '''
-        rotvec = self.__rotation.as_rotvec()
-        norm = np.linalg.norm(rotvec)
-
-        if norm == 0.0:
-            return rotvec
-
-        if normalized:
-            return rotvec/norm
-
-        return rotvec
-
-    def as_euler(self, sequence: str = None, degrees: bool = True) -> Union[np.ndarray, float]:
-        '''
-        Return the stored `self.__rotation` member in euler angles.
-
-        Parameters
-        ----------
-        - `sequence` (`str`): Sequence in which the euler angle will be returned
-        - `degrees` (`bool`): Option to return euler angles in degrees or not
-
-        Returns
-        -------
-        - `Union[np.ndarray, float]`: Euler angle(s) (if `RE` is in 2D then only a float will be returned)
-        '''
-        if self.dim == 2:
-            return self.__rotation.as_euler('zyx', degrees)[0]
-
-        if sequence is None:
-            raise ValueError('Input sequence cannot be None.')
-
-        return self.__rotation.as_euler(sequence, degrees)
-
-    def yaw(self, degrees: bool = True) -> float:
-        '''
-        Return rotation angle around the z axis.
-
-        Note: This function will not work for 2D rotations. It is recommended to use `as_euler()` instead.
-
-        Parameters
-        ----------
-        - `degrees` (`bool`): Option to return value in degrees or radians (default: `True`)
-
-        Returns
-        -------
-        - `float`: Yaw angle (in specified units)
-        '''
-        if self.dim == 2:
-            raise AttributeError('Unable to return yaw angle of 2D rotation (Call as_euler() instead).')
-
-        return self.__rotation.as_euler('xyz', degrees)[2]
-
-    def pitch(self, degrees: bool = True) -> float:
-        '''
-        Return rotation angle around the y axis.
-
-        Note: This function will not work for 2D rotations. It is recommended to use `as_euler()` instead.
-
-        Parameters
-        ----------
-        - `degrees` (`bool`): Option to return value in degrees or radians (default: `True`)
-
-        Returns
-        -------
-        - `float`: Pitch angle (in specified units)
-        '''
-        if self.dim == 2:
-            raise AttributeError('Unable to return pitch angle of 2D rotation (Call as_euler() instead).')
-
-        return self.__rotation.as_euler('xyz', degrees)[1]
-
-    def roll(self, degrees: bool = True) -> float:
-        '''
-        Return rotation angle around the x axis.
-
-        Note: This function will not work for 2D rotations. It is recommended to use `as_euler()` instead.
-
-        Parameters
-        ----------
-        - `degrees` (`bool`): Option to return value in degrees or radians (default: `True`)
-
-        Returns
-        -------
-        - `float`: Roll angle (in specified units)
-        '''
-        if self.dim == 2:
-            raise AttributeError('Unable to return roll angle of 2D rotation (Call as_euler() instead).')
-
-        return self.__rotation.as_euler('xyz', degrees)[0]
-
-    # Computation functions
-    def apply(self, input_element: Union[np.ndarray, list]) -> np.ndarray:
-        '''
-        The `apply` function applies this rotation to `input` vector.
-
-        Note: The dimension of the input vector must match the set dimension of the `RE` object.
-
-        Parameters
-        ----------
-        - `input` (`Union[np.ndarray, list]`): Input vector to be rotated
-
-        Returns
-        -------
-        - `np.ndarray`: Rotated vector
-        '''
-        input_element = np.array(input_element)
-
-        # Check shape of input
-        if input_element.shape[0] != self.dim:
-            raise ValueError(f'Input shape mismatch: self.dim ({self.dim}) != input.shape ({input_element.shape[0]})')
-
-        if self.dim == 2:
-            input_element = np.hstack((input_element, [0]))
-
-        result = self.__rotation.apply(input_element)
-
-        if self.dim == 2:
-            return result[:2]
-
-        return result
-
-    # Operator overloading
-    def __str__(self) -> str:
-        return f'ER{self.dim} - {self.name}: {self.__repr__()} degrees'
-
-    def __repr__(self) -> str:
-        if self.dim == 3:
-            sequence = 'xyz'
-        if self.dim == 2:
-            sequence = 'z'
-
-        return f'{self.as_euler(sequence, degrees=True)}'
-
-    def __eq__(self, other):
-        if isinstance(other, ER):
-            return np.allclose(self.as_quat(),
-                               other.as_quat(),
-                               rtol=ER_TOLERANCE,
-                               atol=ER_TOLERANCE)
-
-        raise TypeError(f'Input parameter is {type(other)}, not RE as expected.')
-
-    def __ne__(self, other):
-        if isinstance(other, ER):
-            return not np.allclose(self.as_quat(),
-                                   other.as_quat(),
-                                   rtol=ER_TOLERANCE,
-                                   atol=ER_TOLERANCE)
-
-        raise TypeError(f'Input parameter is {type(other)}, not RE as expected.')
+from typing import Union
+
+import numpy as np
+from scipy.spatial.transform import Rotation
+from .utils import ER_TOLERANCE, valid_dim
+
+
+class ER:
+    def __init__(self, name: str = '', dim: int = 3) -> None:
+        '''
+        The `__init__` function is called when a new instance of the `RE` class is created.
+        It initializes all of the variables in the class and sets them to their default values.
+
+        By default, the `self.__rotation` member value is set to an identity value.
+
+        Parameters
+        ----------
+        - `name` (`str`): Set the name of the object (default: '')
+        - `dim` (`int`): Set the dimension of the vector (default: 3)
+        '''
+        self.name = name
+        self.__rotation = Rotation(quat=[0, 0, 0, 1])
+        self.identity()
+
+        if valid_dim(dim):
+            self.__dim = dim
+
+    # Setter functions
+    def identity(self) -> None:
+        '''
+        The `identity` function sets the `self.__rotation` member to
+        the equivalent of an identity matrix.
+        '''
+        self.__rotation = Rotation.identity()
+
+    def inv(self) -> None:
+        '''
+        The `inv` function sets the `self.__rotation` member to its inverse.
+        '''
+        self.__rotation = self.__rotation.inv()
+
+    def random(self) -> None:
+        '''
+        The `random` function sets the `self.__rotation` member to a random value.
+        '''
+        if self.dim == 2:
+            self.__rotation.from_euler('z', np.random.uniform(0, 360))
+
+        else:
+            self.__rotation = Rotation.random()
+
+    def from_quat(self, quat: Union[np.ndarray, list]) -> None:
+        '''
+        The `from_quat` function set the `self.__rotation` member from the value of
+        the input `quat`.
+
+        Note: This function will not work for `RE` objects that are defined in 2D space.
+
+        Parameters
+        ----------
+        - `quat` (`Union[np.ndarray, list]`): Input quaternion
+        '''
+        if self.__dim == 2:
+            raise AttributeError(
+                'Unable to set 2D rotation from quaternion input.'
+            )
+
+        if len(quat) != 4:
+            raise ValueError(
+                f'Input vector shape must be equal to 4 (input shape: {len(quat)}).'
+            )
+
+        self.__rotation = Rotation.from_quat(np.array(quat))
+
+    def from_matrix(self, matrix: np.ndarray) -> None:
+        '''
+        The `from_matrix` function set the `self.__rotation` member from the value of
+        the input `matrix`. The function will first check whether the input matrix dimensions
+        are suitable for the number of dimensions set for the `RE` object.
+
+        Parameters
+        ----------
+        - `matrix` (`np.ndarray`): Input matrix
+        '''
+        if matrix.shape != (self.dim, self.dim):
+            raise ValueError(
+                f'Input matrix shape must be ({self.dim}, {self.dim}) when rotation dimension is {self.dim}. Current input matrix shape: {matrix.shape}.'
+            )
+
+        if self.dim == 2:
+            matrix = np.hstack((np.array(matrix), np.zeros(shape=(2,1))))
+            matrix = np.vstack((np.array(matrix), [0, 0, 1]))
+
+        self.__rotation = Rotation.from_matrix(matrix)
+
+    def from_angle_axis(self, angle_axis: np.ndarray) -> None:
+        '''
+        The `from_angle_axis` function set the `self.__rotation` member from the value of
+        the input `angle_axis`.
+
+        Note: This function will not work for `RE` objects that are defined in 2D space.
+
+        Parameters
+        ----------
+        - `angle_axis` (`np.ndarray`): Input angle-axis vector
+        '''
+        if self.dim == 2:
+            raise AttributeError(
+                'Unable to set 2D rotation from angle-axis input.'
+            )
+
+        if len(angle_axis) != 3:
+            raise ValueError(
+                f'Input vector shape must be equal to 3 (input shape: {len(angle_axis)}).'
+            )
+
+        self.__rotation = Rotation.from_rotvec(np.array(angle_axis) / np.linalg.norm(angle_axis))
+
+    def from_euler(self, sequence: str = None, angles: Union[np.ndarray, list] = None, degrees: bool = True) -> None:
+        '''
+        The `from_euler` function set the `self.__rotation` member from the value(s) of
+        the inputs `sequence` and `angles`. The angle will be converted from degrees to
+        radians if `degrees` is `True`.
+
+        Parameters
+        ----------
+        - `sequence` (`str`): Sequence of euler angles (e.g. 'xyz', 'xy', 'zyx')
+        - `angles` (`Union[np.ndarray, list]`): List of euler angles
+        - `degrees` (`bool`): Set to true if input angles are in degrees (default: `True`)
+        '''
+        if angles is None:
+            raise ValueError(
+                'Input angles cannot be None.'
+            )
+
+        if self.dim == 3:
+            if sequence is None:
+                raise ValueError(
+                    'Input sequence cannot be None.'
+                )
+
+            self.__rotation = Rotation.from_euler(sequence, np.array(angles), degrees)
+
+        elif self.dim == 2:
+            self.__rotation = Rotation.from_euler('z', np.array(angles), degrees)
+
+    # Getter functions
+    @property
+    def dim(self) -> int:
+        '''
+        Return the number of dimensions.
+
+        Returns
+        -------
+        - `int`: Value of `self.__dim` member
+        '''
+        return self.__dim
+
+    def as_quat(self) -> np.ndarray:
+        '''
+        Return the stored `self.__rotation` member in quaternion form.
+
+        Returns
+        -------
+        - `np.ndarray`: Quaternion vector
+        '''
+        return self.__rotation.as_quat()
+
+    def as_matrix(self) -> np.ndarray:
+        '''
+        Return the stored `self.__rotation` member in matrix form.
+
+        Returns
+        -------
+        - `np.ndarray`: Rotation matrix
+        '''
+        return self.__rotation.as_matrix()[:self.dim, :self.dim]
+
+    def as_angle_axis(self, normalized: bool = True) -> np.ndarray:
+        '''
+        Return the stored `self.__rotation` member in angle-axis form.
+
+        Parameters
+        ----------
+        - `normalized` (`bool`): Return a normalized vector (Defaults to `True`)
+
+        Returns
+        -------
+        - `np.ndarray`: Angle-axis vector
+        '''
+        rotvec = self.__rotation.as_rotvec()
+        norm = np.linalg.norm(rotvec)
+
+        if norm == 0.0:
+            return rotvec
+
+        if normalized:
+            return rotvec/norm
+
+        return rotvec
+
+    def as_euler(self, sequence: str = None, degrees: bool = True) -> Union[np.ndarray, float]:
+        '''
+        Return the stored `self.__rotation` member in euler angles.
+
+        Parameters
+        ----------
+        - `sequence` (`str`): Sequence in which the euler angle will be returned
+        - `degrees` (`bool`): Option to return euler angles in degrees or not
+
+        Returns
+        -------
+        - `Union[np.ndarray, float]`: Euler angle(s) (if `RE` is in 2D then only a float will be returned)
+        '''
+        if self.dim == 2:
+            return self.__rotation.as_euler('zyx', degrees)[0]
+
+        if sequence is None:
+            raise ValueError(
+                'Input sequence cannot be None.'
+            )
+
+        return self.__rotation.as_euler(sequence, degrees)
+
+    def yaw(self, degrees: bool = True) -> float:
+        '''
+        Return rotation angle around the z axis.
+
+        Note: This function will not work for 2D rotations. It is recommended to use `as_euler()` instead.
+
+        Parameters
+        ----------
+        - `degrees` (`bool`): Option to return value in degrees or radians (default: `True`)
+
+        Returns
+        -------
+        - `float`: Yaw angle (in specified units)
+        '''
+        if self.dim == 2:
+            raise AttributeError(
+                'Unable to return yaw angle of 2D rotation (Call as_euler() instead).'
+            )
+
+        return self.__rotation.as_euler('xyz', degrees)[2]
+
+    def pitch(self, degrees: bool = True) -> float:
+        '''
+        Return rotation angle around the y axis.
+
+        Note: This function will not work for 2D rotations. It is recommended to use `as_euler()` instead.
+
+        Parameters
+        ----------
+        - `degrees` (`bool`): Option to return value in degrees or radians (default: `True`)
+
+        Returns
+        -------
+        - `float`: Pitch angle (in specified units)
+        '''
+        if self.dim == 2:
+            raise AttributeError(
+                'Unable to return pitch angle of 2D rotation (Call as_euler() instead).'
+            )
+
+        return self.__rotation.as_euler('xyz', degrees)[1]
+
+    def roll(self, degrees: bool = True) -> float:
+        '''
+        Return rotation angle around the x axis.
+
+        Note: This function will not work for 2D rotations. It is recommended to use `as_euler()` instead.
+
+        Parameters
+        ----------
+        - `degrees` (`bool`): Option to return value in degrees or radians (default: `True`)
+
+        Returns
+        -------
+        - `float`: Roll angle (in specified units)
+        '''
+        if self.dim == 2:
+            raise AttributeError(
+                'Unable to return roll angle of 2D rotation (Call as_euler() instead).'
+            )
+
+        return self.__rotation.as_euler('xyz', degrees)[0]
+
+    # Computation functions
+    def apply(self, input_element: Union[np.ndarray, list]) -> np.ndarray:
+        '''
+        The `apply` function applies this rotation to `input` vector.
+
+        Note: The dimension of the input vector must match the set dimension of the `RE` object.
+
+        Parameters
+        ----------
+        - `input` (`Union[np.ndarray, list]`): Input vector to be rotated
+
+        Returns
+        -------
+        - `np.ndarray`: Rotated vector
+        '''
+        input_element = np.array(input_element)
+
+        # Check shape of input
+        if input_element.shape[0] != self.dim:
+            raise ValueError(
+                f'Input shape mismatch: self.dim ({self.dim}) != input.shape ({input_element.shape[0]})'
+            )
+
+        if self.dim == 2:
+            input_element = np.hstack((input_element, [0]))
+
+        result = self.__rotation.apply(input_element)
+
+        if self.dim == 2:
+            return result[:2]
+
+        return result
+
+    # Operator overloading
+    def __str__(self) -> str:
+        return f'ER{self.dim} - {self.name}: {self.__repr__()} degrees'
+
+    def __repr__(self) -> str:
+        if self.dim == 3:
+            sequence = 'xyz'
+        if self.dim == 2:
+            sequence = 'z'
+
+        return f'{self.as_euler(sequence, degrees=True)}'
+
+    def __eq__(self, other):
+        if isinstance(other, ER):
+            return np.allclose(self.as_quat(),
+                               other.as_quat(),
+                               rtol=ER_TOLERANCE,
+                               atol=ER_TOLERANCE)
+
+        raise TypeError(
+            f'Input parameter is {type(other)}, not RE as expected.'
+        )
+
+    def __ne__(self, other):
+        if isinstance(other, ER):
+            return not np.allclose(self.as_quat(),
+                                   other.as_quat(),
+                                   rtol=ER_TOLERANCE,
+                                   atol=ER_TOLERANCE)
+
+        raise TypeError(
+            f'Input parameter is {type(other)}, not RE as expected.'
+        )
```

### Comparing `pose3d-2.1.0/pose3d/et.py` & `pose3d-2.1.1a0/pose3d/et.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,206 +1,208 @@
-import numpy as np
-from typing import Union
-
-from .utils import valid_dim
-
-class ET:
-    def __init__(self, name: str = '', dim: int = 3, vector: Union[np.ndarray, list] = None) -> None:
-        '''
-        The `__init__` function is called when a new instance of the `ET` class is created.
-        It initializes all of the variables in the class and sets them to their default values.
-
-        By default, the `self.__vector` member value is set to zero.
-
-        Parameters
-        ----------
-        - `name` (`str`): Set the name of the object (default: '')
-        - `dim` (`int`): Set the dimension of the vector (default: 3)
-        - `vector` (`np.ndarray|list`): Set value of vector at `__init__` (default: `None`)
-        '''
-        self.name = name
-
-        if valid_dim(dim):
-            self.__dim = dim
-
-        if vector is None:
-            self.__vector = np.zeros(self.__dim)
-        else:
-            if valid_dim(len(vector)):
-                self.__dim = len(vector)
-                self.__vector = np.array(vector)
-
-    # Getter functions
-    @property
-    def dim(self) -> int:
-        '''
-        Return the number of dimensions.
-
-        Returns
-        -------
-        - `int`: Value of `self.__dim` member
-        '''
-        return self.__dim
-
-    @property
-    def vector(self) -> np.ndarray:
-        '''
-        Return the value of the `self.__vector` member.
-
-        Returns
-        -------
-        - `np.ndarray`: Value of `self.__vector` member
-        '''
-        return self.__vector
-
-    @property
-    def x(self) -> float:
-        '''
-        Return the first element of the `self.__vector` member.
-
-        Returns
-        -------
-        - `float`: First element of the `self.__vector` member
-        '''
-        return float(self.vector[0])
-
-    @property
-    def y(self) -> float:
-        '''
-        Return the second element of the `self.__vector` member.
-
-        Returns
-        -------
-        - `float`: Second element of the `self.__vector` member
-        '''
-        return float(self.vector[1])
-
-    @property
-    def z(self) -> float:
-        '''
-        Return the third element of the `self.__vector` member.
-
-        Note: This function will only work for `ET` classes set to 3 dimensions.
-
-        Returns
-        -------
-        - `float`: Third element of the `self.__vector` member
-        '''
-        return float(self.vector[2])
-
-    # Setter functions
-    def random(self) -> None:
-        '''
-        The `random` function sets the `self.__vector` member to a random state.
-        '''
-        self.vector = np.random.uniform(0, 1, size=self.vector.shape)
-
-    @vector.setter
-    def vector(self, vector: Union[np.ndarray, list]) -> None:
-        '''
-        The `vector` function sets the `self.__vector` to the input vector.
-
-        The function also checks whether the input dimension matches the class dimension.
-
-        Parameters
-        ----------
-        - `vector` (`Union[np.ndarray, list]`): Input vector
-        '''
-        if isinstance(vector, list):
-            vector = np.array(vector)
-
-        if vector.shape != self.__vector.shape:
-            raise ValueError(f'Input vector dimension ({vector.shape[0]}) does not match the set dimension ({self.__vector.shape[0]}).')
-
-        self.__vector = vector
-
-    def zero(self) -> None:
-        '''
-        The `zero` function sets the `self.__vector` to zero.
-        '''
-        self.vector = np.zeros(self.dim)
-
-    def inv(self) -> None:
-        '''
-        The `inv` function sets the `self.__vector` member to its inverse (negative value).
-        '''
-        self.vector = -self.vector
-
-    # Operator overloads
-    def __str__(self) -> str:
-        return f'ET{self.__dim} - {self.name}: {self.vector}'
-
-    def __repr__(self) -> str:
-        return f'{self.vector}'
-
-    def __add__(self, other):
-        if isinstance(other, ET):
-            if other.vector.shape == self.vector.shape:
-                return ET(name=f'Sum of {self.name} and {other.name}',
-                          vector=self.vector + other.vector)
-
-        elif isinstance(other, np.ndarray):
-            if other.shape == self.vector.shape:
-                return ET(name=self.name,
-                           vector=self.vector + other)
-
-        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
-
-    def __sub__(self, other):
-        if isinstance(other, ET):
-            if other.vector().shape == self.vector.shape:
-                return ET(name=f'Sum of {self.name} and {other.name}',
-                          vector=self.vector - other.vector)
-
-        elif isinstance(other, np.ndarray):
-            if other.shape == self.vector.shape:
-                return ET(name=self.name,
-                           vector=self.vector - other)
-
-        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
-
-    def __iadd__(self, other):
-        if not isinstance(other, (ET, np.ndarray)):
-            raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
-
-        if isinstance(other, ET):
-            if other.vector.shape == self.vector.shape:
-                self.vector = self.vector + other.vector
-
-        elif isinstance(other, np.ndarray):
-            if other.shape == self.vector.shape:
-                self.vector = self.vector + other
-
-    def __isub__(self, other):
-        if isinstance(other, ET):
-            if other.vector().shape == self.vector.shape:
-                self.vector = self.vector - other.vector
-
-        elif isinstance(other, np.ndarray):
-            if other.shape == self.vector.shape:
-                self.vector = self.vector - other
-
-        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
-
-    def __eq__(self, other):
-        if isinstance(other, ET):
-            return np.array_equal(self.vector, other.vector)
-
-        elif isinstance(other, np.ndarray):
-            return np.array_equal(self.vector, other)
-
-        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
-
-    def __ne__(self, other):
-        if isinstance(other, ET):
-            return not np.array_equal(self.vector, other.vector)
-
-        elif isinstance(other, np.ndarray):
-            return not np.array_equal(self.vector, other)
-
-        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
-
-    def __neg__(self):
-        self.vector = -self.vector
-
-    def __abs__(self):
-        self.vector = abs(self.vector)
+import numpy as np
+from typing import Union
+
+from .utils import valid_dim
+
+class ET:
+    def __init__(self, name: str = '', dim: int = 3, vector: Union[np.ndarray, list] = None) -> None:
+        '''
+        The `__init__` function is called when a new instance of the `ET` class is created.
+        It initializes all of the variables in the class and sets them to their default values.
+
+        By default, the `self.__vector` member value is set to zero.
+
+        Parameters
+        ----------
+        - `name` (`str`): Set the name of the object (default: '')
+        - `dim` (`int`): Set the dimension of the vector (default: 3)
+        - `vector` (`np.ndarray|list`): Set value of vector at `__init__` (default: `None`)
+        '''
+        self.name = name
+
+        if valid_dim(dim):
+            self.__dim = dim
+
+        if vector is None:
+            self.__vector = np.zeros(self.__dim)
+        else:
+            if valid_dim(len(vector)):
+                self.__dim = len(vector)
+                self.__vector = np.array(vector)
+
+    # Getter functions
+    @property
+    def dim(self) -> int:
+        '''
+        Return the number of dimensions.
+
+        Returns
+        -------
+        - `int`: Value of `self.__dim` member
+        '''
+        return self.__dim
+
+    @property
+    def vector(self) -> np.ndarray:
+        '''
+        Return the value of the `self.__vector` member.
+
+        Returns
+        -------
+        - `np.ndarray`: Value of `self.__vector` member
+        '''
+        return self.__vector
+
+    @property
+    def x(self) -> float:
+        '''
+        Return the first element of the `self.__vector` member.
+
+        Returns
+        -------
+        - `float`: First element of the `self.__vector` member
+        '''
+        return float(self.vector[0])
+
+    @property
+    def y(self) -> float:
+        '''
+        Return the second element of the `self.__vector` member.
+
+        Returns
+        -------
+        - `float`: Second element of the `self.__vector` member
+        '''
+        return float(self.vector[1])
+
+    @property
+    def z(self) -> float:
+        '''
+        Return the third element of the `self.__vector` member.
+
+        Note: This function will only work for `ET` classes set to 3 dimensions.
+
+        Returns
+        -------
+        - `float`: Third element of the `self.__vector` member
+        '''
+        return float(self.vector[2])
+
+    # Setter functions
+    def random(self) -> None:
+        '''
+        The `random` function sets the `self.__vector` member to a random state.
+        '''
+        self.vector = np.random.uniform(0, 1, size=self.vector.shape)
+
+    @vector.setter
+    def vector(self, vector: Union[np.ndarray, list]) -> None:
+        '''
+        The `vector` function sets the `self.__vector` to the input vector.
+
+        The function also checks whether the input dimension matches the class dimension.
+
+        Parameters
+        ----------
+        - `vector` (`Union[np.ndarray, list]`): Input vector
+        '''
+        if isinstance(vector, list):
+            vector = np.array(vector)
+
+        if vector.shape != self.__vector.shape:
+            raise ValueError(
+                f'Input vector dimension ({vector.shape[0]}) does not match the set dimension ({self.__vector.shape[0]}).'
+            )
+
+        self.__vector = vector
+
+    def zero(self) -> None:
+        '''
+        The `zero` function sets the `self.__vector` to zero.
+        '''
+        self.vector = np.zeros(self.dim)
+
+    def inv(self) -> None:
+        '''
+        The `inv` function sets the `self.__vector` member to its inverse (negative value).
+        '''
+        self.vector = -self.vector
+
+    # Operator overloads
+    def __str__(self) -> str:
+        return f'ET{self.__dim} - {self.name}: {self.vector}'
+
+    def __repr__(self) -> str:
+        return f'{self.vector}'
+
+    def __add__(self, other):
+        if isinstance(other, ET):
+            if other.vector.shape == self.vector.shape:
+                return ET(name=f'Sum of {self.name} and {other.name}',
+                          vector=self.vector + other.vector)
+
+        elif isinstance(other, np.ndarray):
+            if other.shape == self.vector.shape:
+                return ET(name=self.name,
+                           vector=self.vector + other)
+
+        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
+
+    def __sub__(self, other):
+        if isinstance(other, ET):
+            if other.vector().shape == self.vector.shape:
+                return ET(name=f'Sum of {self.name} and {other.name}',
+                          vector=self.vector - other.vector)
+
+        elif isinstance(other, np.ndarray):
+            if other.shape == self.vector.shape:
+                return ET(name=self.name,
+                           vector=self.vector - other)
+
+        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
+
+    def __iadd__(self, other):
+        if not isinstance(other, (ET, np.ndarray)):
+            raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
+
+        if isinstance(other, ET):
+            if other.vector.shape == self.vector.shape:
+                self.vector = self.vector + other.vector
+
+        elif isinstance(other, np.ndarray):
+            if other.shape == self.vector.shape:
+                self.vector = self.vector + other
+
+    def __isub__(self, other):
+        if isinstance(other, ET):
+            if other.vector().shape == self.vector.shape:
+                self.vector = self.vector - other.vector
+
+        elif isinstance(other, np.ndarray):
+            if other.shape == self.vector.shape:
+                self.vector = self.vector - other
+
+        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
+
+    def __eq__(self, other):
+        if isinstance(other, ET):
+            return np.array_equal(self.vector, other.vector)
+
+        elif isinstance(other, np.ndarray):
+            return np.array_equal(self.vector, other)
+
+        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
+
+    def __ne__(self, other):
+        if isinstance(other, ET):
+            return not np.array_equal(self.vector, other.vector)
+
+        elif isinstance(other, np.ndarray):
+            return not np.array_equal(self.vector, other)
+
+        raise TypeError(f'Input parameter is {type(other)}, not ET or np.ndarray as expected.')
+
+    def __neg__(self):
+        self.vector = -self.vector
+
+    def __abs__(self):
+        self.vector = abs(self.vector)
```

### Comparing `pose3d-2.1.0/pose3d/pose.py` & `pose3d-2.1.1a0/pose3d/pose.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from .et import ET
-from .er import ER
-from typing import Tuple
-
-from .utils import valid_dim
-
-class Pose:
-    def __init__(self, name: str = '', et_dim: int = 3, er_dim: int = 3) -> None:
-        '''
-        The `__init__` function is called when a new instance of the `Pose` class is created.
-        It initializes all of the variables in the class and sets them to their default values.
-
-        Parameters
-        ----------
-        - `name` (`str`): Set the name of the object (default: '')
-        - `et_dim` (`int`): Set the dimension of the position member (default: 3)
-        - `er_dim` (`int`): Set the dimension of the orientation member (default: 3)
-        '''
-        self.name = name
-
-        if valid_dim(et_dim):
-            self.position = ET(dim=et_dim)
-
-        if valid_dim(er_dim):
-            self.orientation = ER(dim=er_dim)
-
-    # Setter functions
-    def random(self) -> None:
-        '''
-        Sets the position and orientation to random values.
-        '''
-        self.orientation.random()
-        self.position.random()
-
-    def zero(self) -> None:
-        '''
-        Sets the position vector to zero and orientation to identity.
-        '''
-        self.orientation.identity()
-        self.position.zero()
-
-    # Getter functions
-    def dims(self) -> Tuple[int, int]:
-        '''
-        Returns the dimensions of the position and orientation (in that order).
-
-        Returns
-        -------
-        - `tuple[int, int]`: Dimension of position and orientation (in that order)
-        '''
-        return self.position.dim, self.orientation.dim
-
-    # Operator overloads
-    def __str__(self) -> str:
-        return f'''Pose - {self.name}:
-        Position:    {self.position.__repr__}
-        Orientation: {self.orientation.__repr__}'''
-
-    def __repr__(self) -> str:
-        return f'Position:    {self.position.__repr__}\nOrientation: {self.orientation.__repr__}'
-
-    def __eq__(self, other) -> bool:
-        if isinstance(other, Pose) and other.dims() == self.dims():
-            return self.orientation == other.orientation and self.position == other.position
-
-        return False
-
-    def __ne__(self, other) -> bool:
-        if isinstance(other, Pose) and other.dims() == self.dims():
-            return self.orientation != other.orientation or self.position != other.position
-
-        return False
+from .et import ET
+from .er import ER
+from typing import Tuple
+
+from .utils import valid_dim
+
+class Pose:
+    def __init__(self, name: str = '', et_dim: int = 3, er_dim: int = 3) -> None:
+        '''
+        The `__init__` function is called when a new instance of the `Pose` class is created.
+        It initializes all of the variables in the class and sets them to their default values.
+
+        Parameters
+        ----------
+        - `name` (`str`): Set the name of the object (default: '')
+        - `et_dim` (`int`): Set the dimension of the position member (default: 3)
+        - `er_dim` (`int`): Set the dimension of the orientation member (default: 3)
+        '''
+        self.name = name
+
+        if valid_dim(et_dim):
+            self.position = ET(dim=et_dim)
+
+        if valid_dim(er_dim):
+            self.orientation = ER(dim=er_dim)
+
+    # Setter functions
+    def random(self) -> None:
+        '''
+        Sets the position and orientation to random values.
+        '''
+        self.orientation.random()
+        self.position.random()
+
+    def zero(self) -> None:
+        '''
+        Sets the position vector to zero and orientation to identity.
+        '''
+        self.orientation.identity()
+        self.position.zero()
+
+    # Getter functions
+    def dims(self) -> Tuple[int, int]:
+        '''
+        Returns the dimensions of the position and orientation (in that order).
+
+        Returns
+        -------
+        - `tuple[int, int]`: Dimension of position and orientation (in that order)
+        '''
+        return self.position.dim, self.orientation.dim
+
+    # Operator overloads
+    def __str__(self) -> str:
+        return f'''Pose - {self.name}:
+        Position:    {self.position.__repr__}
+        Orientation: {self.orientation.__repr__}'''
+
+    def __repr__(self) -> str:
+        return f'Position:    {self.position.__repr__}\nOrientation: {self.orientation.__repr__}'
+
+    def __eq__(self, other) -> bool:
+        if isinstance(other, Pose) and other.dims() == self.dims():
+            return self.orientation == other.orientation and self.position == other.position
+
+        return False
+
+    def __ne__(self, other) -> bool:
+        if isinstance(other, Pose) and other.dims() == self.dims():
+            return self.orientation != other.orientation or self.position != other.position
+
+        return False
```

### Comparing `pose3d-2.1.0/pose3d/transform.py` & `pose3d-2.1.1a0/pose3d/transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-import numpy as np
-from typing import Tuple, Union
-
-from .et import ET
-from .er import ER
-
-from .pose import Pose
-
-from .utils import valid_dim
-
-class Transform:
-    def __init__(self, name: str, orig: str = 'origin', dest: str = 'destination', te_dim: int = 3, re_dim: int = 3) -> None:
-        # Set strings
-        self.name = name
-        self.origin = orig
-        self.destination = dest
-
-        # Init translation and rotation memebers
-        if valid_dim(te_dim):
-            self.translation = ET(dim = te_dim)
-
-        if valid_dim(re_dim):
-            self.rotation = ER(dim = re_dim)
-
-    # Setter functions
-    def between_poses(self, pose_1: Pose, pose_2: Pose) -> None:
-        '''
-        Compute transform between 2 3D poses. This instance of Transform
-        will be modifed to compute the transform from pose_1 to pose_2.
-
-        Parameters
-        ----------
-        - `pose_1` (`Pose`): Origin pose.
-        - `pose_2` (`Pose`): Destination pose.
-        '''
-        if pose_1.dims() != pose_2.dims():
-            raise AttributeError(f'Number of dimensions between both poses do not match: pose_1.dims() = {pose_1.dims()} and pose_2.dims = {pose_2.dims()}.')
-
-        # Modify dimension of transformation depending on pose_1 and pose_2
-        if pose_1.position.dim != self.translation.dim:
-            self.translation = ET(dim=pose_1.position.dim)
-
-        if pose_1.orientation.dim != self.rotation.dim:
-            self.rotation = ER(dim=pose_1.orientation.dim)
-
-        # Compute rotation from pose_1 to pose_2
-        self.rotation.from_matrix(np.dot(np.linalg.inv(pose_2.orientation.as_matrix()), pose_1.orientation.as_matrix()))
-        self.translation.vector = pose_2.position.vector - pose_1.position.vector
-
-    def identity(self) -> None:
-        '''
-        Set the transformation to zero and the rotation to identity.
-        '''
-        self.translation.zero()
-        self.rotation.identity()
-
-    def inv(self) -> None:
-        '''
-        Set the transformation it's inverse.
-        '''
-        self.rotation.inv()
-        self.translation.vector = -self.rotation.apply(self.translation.vector)
-
-    def random(self) -> None:
-        '''
-        Set a random transformation.
-        '''
-        self.translation.random()
-        self.rotation.random()
-
-    # Getter functions
-    def dims(self) -> Tuple[int, int]:
-        '''
-        Returns the dimensions of the translation and rotation (in that order).
-
-        Returns
-        -------
-        - `tuple[int, int]`: Dimension of translation and rotation (in that order)
-        '''
-        return self.translation.dim, self.rotation.dim
-
-    def matrix(self, homogeneous: bool = True) -> np.ndarray:
-        '''
-        Return the transformation matrix.
-
-        Returns
-        -------
-        - `np.ndarray`: Transformation matrix
-        '''
-        matrix = np.eye(max(self.dims()) + 1)
-
-        if self.origin != self.destination:
-            matrix[:self.rotation.dim, :self.rotation.dim] = self.rotation.as_matrix()
-            matrix[:self.translation.dim, -1] = self.translation.vector
-
-        if not homogeneous:
-            return matrix[:-1, :]
-
-        return matrix
-
-    # Computation functions
-    def apply(self, io_element: Union[Pose, np.ndarray]) -> Union[Pose, np.ndarray]:
-        '''
-        Apply transformation to `io`.
-
-        Parameters
-        ----------
-        - `io_element` (`Union[Pose, np.ndarray]`): Element to apply transformation to
-
-        Returns
-        -------
-        - `Union[Pose, np.ndarray]`: Output pose/vector
-        '''
-        # If io_element is a Pose
-        if isinstance(io_element, Pose):
-            output = Pose(et_dim=io_element.position.dim, er_dim=io_element.orientation.dim)
-            output.position.vector = io_element.position.vector
-            output.orientation.from_quat(io_element.orientation.as_quat())
-
-            output.orientation.from_matrix(np.dot(self.rotation.as_matrix(), output.orientation.as_matrix()))
-            output.position.vector = self.rotation.apply(output.position.vector) + self.translation.vector
-
-        # If io_element is a numpy vector
-        if isinstance(io_element, np.ndarray):
-            output = io_element.copy()
-            output = self.rotation.apply(output) + self.translation.vector
-
-        return output
-
-    # Operator overloads
-    def __repr__(self) -> str:
-        return f'''Transform - {self.name}:
-        Translation: {self.translation.__repr__}
-        Rotation:    {self.rotation.__repr__}'''
-
-    def __str__(self) -> str:
-        return f'Translation: {self.translation.__repr__}\nRotation:    {self.rotation.__repr__}'
-
-    def __eq__(self, other: object) -> bool:
-        return self.translation == other.translation and self.rotation == other.rotation
-
-    def __ne__(self, other: object) -> bool:
-        return self.translation != other.translation or self.rotation != other.rotation
+import numpy as np
+from typing import Tuple, Union
+
+from .et import ET
+from .er import ER
+
+from .pose import Pose
+
+from .utils import valid_dim
+
+class Transform:
+    def __init__(self, name: str, orig: str = 'origin', dest: str = 'destination', te_dim: int = 3, re_dim: int = 3) -> None:
+        # Set strings
+        self.name = name
+        self.origin = orig
+        self.destination = dest
+
+        # Init translation and rotation members
+        if valid_dim(te_dim):
+            self.translation = ET(dim = te_dim)
+
+        if valid_dim(re_dim):
+            self.rotation = ER(dim = re_dim)
+
+    # Setter functions
+    def between_poses(self, pose_1: Pose, pose_2: Pose) -> None:
+        '''
+        Compute transform between 2 3D poses. This instance of Transform
+        will be modified to compute the transform from pose_1 to pose_2.
+
+        Parameters
+        ----------
+        - `pose_1` (`Pose`): Origin pose.
+        - `pose_2` (`Pose`): Destination pose.
+        '''
+        if pose_1.dims() != pose_2.dims():
+            raise AttributeError(f'Number of dimensions between both poses do not match: pose_1.dims() = {pose_1.dims()} and pose_2.dims = {pose_2.dims()}.')
+
+        # Modify dimension of transformation depending on pose_1 and pose_2
+        if pose_1.position.dim != self.translation.dim:
+            self.translation = ET(dim=pose_1.position.dim)
+
+        if pose_1.orientation.dim != self.rotation.dim:
+            self.rotation = ER(dim=pose_1.orientation.dim)
+
+        # Compute rotation from pose_1 to pose_2
+        self.rotation.from_matrix(np.dot(np.linalg.inv(pose_2.orientation.as_matrix()), pose_1.orientation.as_matrix()))
+        self.translation.vector = pose_2.position.vector - pose_1.position.vector
+
+    def identity(self) -> None:
+        '''
+        Set the transformation to zero and the rotation to identity.
+        '''
+        self.translation.zero()
+        self.rotation.identity()
+
+    def inv(self) -> None:
+        '''
+        Set the transformation it's inverse.
+        '''
+        self.rotation.inv()
+        self.translation.vector = -self.rotation.apply(self.translation.vector)
+
+    def random(self) -> None:
+        '''
+        Set a random transformation.
+        '''
+        self.translation.random()
+        self.rotation.random()
+
+    # Getter functions
+    def dims(self) -> Tuple[int, int]:
+        '''
+        Returns the dimensions of the translation and rotation (in that order).
+
+        Returns
+        -------
+        - `tuple[int, int]`: Dimension of translation and rotation (in that order)
+        '''
+        return self.translation.dim, self.rotation.dim
+
+    def matrix(self, homogeneous: bool = True) -> np.ndarray:
+        '''
+        Return the transformation matrix.
+
+        Returns
+        -------
+        - `np.ndarray`: Transformation matrix
+        '''
+        matrix = np.eye(max(self.dims()) + 1)
+
+        if self.origin != self.destination:
+            matrix[:self.rotation.dim, :self.rotation.dim] = self.rotation.as_matrix()
+            matrix[:self.translation.dim, -1] = self.translation.vector
+
+        if not homogeneous:
+            return matrix[:-1, :]
+
+        return matrix
+
+    # Computation functions
+    def apply(self, io_element: Union[Pose, np.ndarray]) -> Union[Pose, np.ndarray]:
+        '''
+        Apply transformation to `io`.
+
+        Parameters
+        ----------
+        - `io_element` (`Union[Pose, np.ndarray]`): Element to apply transformation to
+
+        Returns
+        -------
+        - `Union[Pose, np.ndarray]`: Output pose/vector
+        '''
+        # If io_element is a Pose
+        if isinstance(io_element, Pose):
+            output = Pose(et_dim=io_element.position.dim, er_dim=io_element.orientation.dim)
+            output.position.vector = io_element.position.vector
+            output.orientation.from_quat(io_element.orientation.as_quat())
+
+            output.orientation.from_matrix(np.dot(self.rotation.as_matrix(), output.orientation.as_matrix()))
+            output.position.vector = self.rotation.apply(output.position.vector) + self.translation.vector
+
+        # If io_element is a numpy vector
+        if isinstance(io_element, np.ndarray):
+            output = io_element.copy()
+            output = self.rotation.apply(output) + self.translation.vector
+
+        return output
+
+    # Operator overloads
+    def __repr__(self) -> str:
+        return f'''Transform - {self.name}:
+        Translation: {self.translation.__repr__}
+        Rotation:    {self.rotation.__repr__}'''
+
+    def __str__(self) -> str:
+        return f'Translation: {self.translation.__repr__}\nRotation:    {self.rotation.__repr__}'
+
+    def __eq__(self, other: object) -> bool:
+        return self.translation == other.translation and self.rotation == other.rotation
+
+    def __ne__(self, other: object) -> bool:
+        return self.translation != other.translation or self.rotation != other.rotation
```

### Comparing `pose3d-2.1.0/pose3d/transform_set.py` & `pose3d-2.1.1a0/pose3d/transform_set.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-import toml
-import numpy as np
-from pathlib import Path
-
-from typing import Union
-
-from .utils import VALID_ROTATION_TYPES
-from .pose import Pose
-from .transform import Transform
-
-
-class TransformSet:
-    def __init__(self, transf_set: Union[str, Path, dict]) -> None:
-
-        self.frames = {}
-        if isinstance(transf_set, str) or isinstance(transf_set, Path):
-            path = Path(transf_set)
-            if not path.exists():
-                raise ValueError(f'Input path ({path.as_posix()}) not found or does not exist.')
-
-            self.__frame_data = toml.load(transf_set)
-        elif isinstance(transf_set, dict):
-            self.__frame_data = transf_set
-
-        # Create dictionary of frames (from which we can create transformations)
-        for frame_name, frame_data in self.__frame_data.items():
-            self.add_frame(frame_name=frame_name, frame_data=frame_data)
-
-        # Add base frame if not present
-        if 'base' not in self.frame_names():
-            base_frame = Pose(name='base')
-            base_frame.position.zero()
-            base_frame.orientation.identity()
-            self.frames['base'] = base_frame
-
-
-    # Setter methods
-    def add_frame(self, frame_name: str, frame_data: Union[dict, Pose]) -> None:
-        '''
-        Add frame to transform set.
-
-        Parameters
-        ----------
-        - `frame_name` (`str`): Name of new frame
-        - `frame_data` (`dict | Pose`): Data of frame
-        '''
-        if frame_name == '' or frame_name in self.frame_names():
-            raise ValueError(f"Invalid pose name {frame_name}. Please use a different name.")
-
-        if isinstance(frame_data, Pose):
-            new_frame = frame_data
-            new_frame.name = frame_name
-
-        elif isinstance(frame_data, dict):
-            new_frame = Pose(name=frame_name)
-
-            # Extract position
-            new_frame.position.vector = frame_data['position']
-
-            # Extract orientation
-            orientation_value = frame_data['orientation']
-            orientation_type = frame_data['orientation_type'].lower()
-            degrees = 'degree' in frame_data['orientation_units'].lower()
-
-            if orientation_type == 'euler':
-                new_frame.orientation.from_euler('xyz', orientation_value, degrees=degrees)
-            elif orientation_type == 'quaternion':
-                new_frame.orientation.from_quat(orientation_value)
-            elif orientation_type == 'angle-axis':
-                new_frame.orientation.from_angle_axis(orientation_value)
-            elif orientation_type == 'matrix':
-                new_frame.orientation.from_matrix(orientation_value)
-            else:
-                raise ValueError(f'TransformSet - Invalid rotation type: {orientation_type}. Rotation type must be: {VALID_ROTATION_TYPES}')
-
-        # Save new frame to self.frames
-        self.frames[frame_name] = new_frame
-
-
-    # Getter methods
-    def frame_names(self) -> list:
-        '''
-        Return list of frame names.
-
-        Returns
-        -------
-        - `list`: List of saved frame names
-        '''
-        return self.frames.keys()
-
-
-    def change_frame(self, input_element, from_frame: str, to_frame: str) -> np.ndarray:
-        '''
-        Coordinate transformation of a pose (6D vector) from origin frame to target frame.
-
-        A compund transformation from origin frame (defined in `from_frame` argument) to
-        the target frame (defined in `to_frame` argument) is computed and applied to the
-        input pose.
-
-        Parameters
-        ----------
-        - `input` (`np.ndarray`): Input pose
-        - `from_frame` (`str`): Name of origin frame
-        - `to_frame` (`str`): Name of target frame
-
-        Returns
-        -------
-        - `np.ndarray`: Transformed pose in target frame
-        '''
-        # Create compound transformation
-        transformation = self.__create_compound_transf(from_frame=from_frame, to_frame=to_frame)
-
-        return transformation.apply(input_element)
-
-
-    def wrench_change_frame(self, wrench: np.ndarray, from_frame: str, to_frame: str) -> np.ndarray:
-        '''
-        Method to change frame of wrench vector.
-
-        Method will perform simple rotation on forces (first three elements), and
-        will rotate the total moments on the origin frame.
-
-        Parameters
-        ----------
-        - `wrench` (`np.ndarray`): Input wrench array
-        - `from_frame` (`str`): Name of origin frame
-        - `to_frame` (`str`): Name of target frame
-
-        Returns
-        -------
-        - `np.ndarray`: Transformed wrench array
-        '''
-        # Verify input
-        if np.array(wrench).shape != (6,):
-            raise ValueError('TransformSet - Invalid wrench input. Shape must be (6,)')
-
-        # Create compound transformation
-        transformation = self.__create_compound_transf(from_frame=from_frame, to_frame=to_frame)
-
-        # Transform wrench
-        force_at_orig = wrench[:3]
-        torque_at_orig = wrench[3:]
-
-        torque_at_dest = transformation.rotation.apply(np.cross(force_at_orig, transformation.translation) + torque_at_orig)
-        force_at_dest = transformation.rotation.apply(force_at_orig)
-
-        return np.hstack([force_at_dest, torque_at_dest])
-
-
-    def transform_matrix(self, from_frame: str, to_frame: str, homogeneous: bool = True) -> np.ndarray:
-        '''
-        Return the transformation matrix to transform poses from origin
-        frame to destination frame.
-
-        Method will call the `__create_compound_transf()` method. Note that such a matrix
-        can only be directly used for poses. Other calculations are required for wrench
-        transformations.
-
-        Parameters
-        ----------
-        - `from_frame` (`str`): Name of origin frame
-        - `to_frame` (`str`): Name of target frame
-        - `homogeneous` (`bool`): Option if matrix should be homogenous or not (3x4 or 4x4) (default: `True`)
-
-        Returns
-        -------
-        - `np.ndarray`: Numpy matrix
-        '''
-        # Create compound transformation
-        full_transf = self.__create_compound_transf(from_frame, to_frame)
-
-        return full_transf.matrix(homogeneous=homogeneous)
-
-
-    def __create_compound_transf(self, from_frame: str, to_frame: str) -> Transform:
-        '''
-        Method to create compound transform between two frames.
-
-        Parameters
-        ----------
-        - `from_frame` (`str`): Name of origin frame
-        - `to_frame` (`str`): Name of destination frame
-
-        Returns
-        -------
-        - `Transform`: Transform object
-        '''
-        transformation = Transform(name=f'{from_frame}2{to_frame}', orig=from_frame, dest=to_frame)
-        transformation.between_poses(pose_1=self.frames[from_frame], pose_2=self.frames[to_frame])
-
-        return transformation
+import toml
+import numpy as np
+from pathlib import Path
+
+from typing import Union
+
+from .utils import VALID_ROTATION_TYPES
+from .pose import Pose
+from .transform import Transform
+
+
+class TransformSet:
+    def __init__(self, transf_set: Union[str, Path, dict]) -> None:
+
+        self.frames = {}
+        if isinstance(transf_set, str) or isinstance(transf_set, Path):
+            path = Path(transf_set)
+            if not path.exists():
+                raise ValueError(f'Input path ({path.as_posix()}) not found or does not exist.')
+
+            self.__frame_data = toml.load(transf_set)
+        elif isinstance(transf_set, dict):
+            self.__frame_data = transf_set
+
+        # Create dictionary of frames (from which we can create transformations)
+        for frame_name, frame_data in self.__frame_data.items():
+            self.add_frame(frame_name=frame_name, frame_data=frame_data)
+
+        # Add base frame if not present
+        if 'base' not in self.frame_names():
+            base_frame = Pose(name='base')
+            base_frame.position.zero()
+            base_frame.orientation.identity()
+            self.frames['base'] = base_frame
+
+
+    # Setter methods
+    def add_frame(self, frame_name: str, frame_data: Union[dict, Pose]) -> None:
+        '''
+        Add frame to transform set.
+
+        Parameters
+        ----------
+        - `frame_name` (`str`): Name of new frame
+        - `frame_data` (`dict | Pose`): Data of frame
+        '''
+        if frame_name == '' or frame_name in self.frame_names():
+            raise ValueError(f"Invalid pose name {frame_name}. Please use a different name.")
+
+        if isinstance(frame_data, Pose):
+            new_frame = frame_data
+            new_frame.name = frame_name
+
+        elif isinstance(frame_data, dict):
+            new_frame = Pose(name=frame_name)
+
+            # Extract position
+            new_frame.position.vector = frame_data['position']
+
+            # Extract orientation
+            orientation_value = frame_data['orientation']
+            orientation_type = frame_data['orientation_type'].lower()
+            degrees = 'degree' in frame_data['orientation_units'].lower()
+
+            if orientation_type == 'euler':
+                new_frame.orientation.from_euler('xyz', orientation_value, degrees=degrees)
+            elif orientation_type == 'quaternion':
+                new_frame.orientation.from_quat(orientation_value)
+            elif orientation_type == 'angle-axis':
+                new_frame.orientation.from_angle_axis(orientation_value)
+            elif orientation_type == 'matrix':
+                new_frame.orientation.from_matrix(orientation_value)
+            else:
+                raise ValueError(f'TransformSet - Invalid rotation type: {orientation_type}. Rotation type must be: {VALID_ROTATION_TYPES}')
+
+        # Save new frame to self.frames
+        self.frames[frame_name] = new_frame
+
+
+    # Getter methods
+    def frame_names(self) -> list:
+        '''
+        Return list of frame names.
+
+        Returns
+        -------
+        - `list`: List of saved frame names
+        '''
+        return self.frames.keys()
+
+
+    def change_frame(self, input_element, from_frame: str, to_frame: str) -> np.ndarray:
+        '''
+        Coordinate transformation of a pose (6D vector) from origin frame to target frame.
+
+        A compound transformation from origin frame (defined in `from_frame` argument) to
+        the target frame (defined in `to_frame` argument) is computed and applied to the
+        input pose.
+
+        Parameters
+        ----------
+        - `input` (`np.ndarray`): Input pose
+        - `from_frame` (`str`): Name of origin frame
+        - `to_frame` (`str`): Name of target frame
+
+        Returns
+        -------
+        - `np.ndarray`: Transformed pose in target frame
+        '''
+        # Create compound transformation
+        transformation = self.__create_compound_transf(from_frame=from_frame, to_frame=to_frame)
+
+        return transformation.apply(input_element)
+
+
+    def wrench_change_frame(self, wrench: np.ndarray, from_frame: str, to_frame: str) -> np.ndarray:
+        '''
+        Method to change frame of wrench vector.
+
+        Method will perform simple rotation on forces (first three elements), and
+        will rotate the total moments on the origin frame.
+
+        Parameters
+        ----------
+        - `wrench` (`np.ndarray`): Input wrench array
+        - `from_frame` (`str`): Name of origin frame
+        - `to_frame` (`str`): Name of target frame
+
+        Returns
+        -------
+        - `np.ndarray`: Transformed wrench array
+        '''
+        # Verify input
+        if np.array(wrench).shape != (6,):
+            raise ValueError('TransformSet - Invalid wrench input. Shape must be (6,)')
+
+        # Create compound transformation
+        transformation = self.__create_compound_transf(from_frame=from_frame, to_frame=to_frame)
+
+        # Transform wrench
+        force_at_orig = wrench[:3]
+        torque_at_orig = wrench[3:]
+
+        torque_at_dest = transformation.rotation.apply(np.cross(force_at_orig, transformation.translation) + torque_at_orig)
+        force_at_dest = transformation.rotation.apply(force_at_orig)
+
+        return np.hstack([force_at_dest, torque_at_dest])
+
+
+    def transform_matrix(self, from_frame: str, to_frame: str, homogeneous: bool = True) -> np.ndarray:
+        '''
+        Return the transformation matrix to transform poses from origin
+        frame to destination frame.
+
+        Method will call the `__create_compound_transf()` method. Note that such a matrix
+        can only be directly used for poses. Other calculations are required for wrench
+        transformations.
+
+        Parameters
+        ----------
+        - `from_frame` (`str`): Name of origin frame
+        - `to_frame` (`str`): Name of target frame
+        - `homogeneous` (`bool`): Option if matrix should be homogenous or not (3x4 or 4x4) (default: `True`)
+
+        Returns
+        -------
+        - `np.ndarray`: Numpy matrix
+        '''
+        # Create compound transformation
+        full_transf = self.__create_compound_transf(from_frame, to_frame)
+
+        return full_transf.matrix(homogeneous=homogeneous)
+
+
+    def __create_compound_transf(self, from_frame: str, to_frame: str) -> Transform:
+        '''
+        Method to create compound transform between two frames.
+
+        Parameters
+        ----------
+        - `from_frame` (`str`): Name of origin frame
+        - `to_frame` (`str`): Name of destination frame
+
+        Returns
+        -------
+        - `Transform`: Transform object
+        '''
+        transformation = Transform(name=f'{from_frame}2{to_frame}', orig=from_frame, dest=to_frame)
+        transformation.between_poses(pose_1=self.frames[from_frame], pose_2=self.frames[to_frame])
+
+        return transformation
```

### Comparing `pose3d-2.1.0/pose3d/utils.py` & `pose3d-2.1.1a0/pose3d/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-ER_TOLERANCE = 1e-10
-ET_TOLERANCE = 1e-10
-
-def valid_dim(input_dim: int) -> bool:
-    '''
-    Check if an imput dimension value is valid for `pose3d` application
-
-    Parameters
-    ----------
-    - `input_dim` (`int`): Input dimension
-
-    Returns
-    -------
-    - `bool`: True if valid dimension.
-    '''
-    valid_dims = [2, 3]
-
-    if input_dim not in valid_dims:
-        raise ValueError(f'Input value for dim argument ({input_dim}) is not valid. Use one of the following: {valid_dims}.')
-
-    return True
-
-VALID_ROTATION_TYPES = ['euler', 'quaternion', 'angle-axis', 'matrix', 'rodrigues']
+ER_TOLERANCE = 1e-10
+ET_TOLERANCE = 1e-10
+
+def valid_dim(input_dim: int) -> bool:
+    '''
+    Check if an input dimension value is valid for `pose3d` application
+
+    Parameters
+    ----------
+    - `input_dim` (`int`): Input dimension
+
+    Returns
+    -------
+    - `bool`: True if valid dimension.
+    '''
+    valid_dims = [2, 3]
+
+    if input_dim not in valid_dims:
+        raise ValueError(f'Input value for dim argument ({input_dim}) is not valid. Use one of the following: {valid_dims}.')
+
+    return True
+
+VALID_ROTATION_TYPES = ['euler', 'quaternion', 'angle-axis', 'matrix', 'rodrigues']
```

