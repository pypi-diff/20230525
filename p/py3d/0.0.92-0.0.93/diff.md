# Comparing `tmp/py3d-0.0.92.tar.gz` & `tmp/py3d-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.92.tar", last modified: Wed May 24 01:03:14 2023, max compression
+gzip compressed data, was "py3d-0.0.93.tar", last modified: Thu May 25 16:42:26 2023, max compression
```

## Comparing `py3d-0.0.92.tar` & `py3d-0.0.93.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 01:03:14.742548 py3d-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-24 01:03:14.742548 py3d-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-24 01:03:04.000000 py3d-0.0.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 01:03:14.742548 py3d-0.0.92/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-24 01:03:04.000000 py3d-0.0.92/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26933 2023-05-24 01:03:04.000000 py3d-0.0.92/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22243 2023-05-24 01:03:04.000000 py3d-0.0.92/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 01:03:14.742548 py3d-0.0.92/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 01:03:14.742548 py3d-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-24 01:03:04.000000 py3d-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 16:42:26.209101 py3d-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-25 16:42:26.209101 py3d-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-25 16:42:15.000000 py3d-0.0.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 16:42:26.205101 py3d-0.0.93/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-25 16:42:15.000000 py3d-0.0.93/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27651 2023-05-25 16:42:15.000000 py3d-0.0.93/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22603 2023-05-25 16:42:15.000000 py3d-0.0.93/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 16:42:26.209101 py3d-0.0.93/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-25 16:42:26.000000 py3d-0.0.93/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 16:42:26.209101 py3d-0.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-25 16:42:15.000000 py3d-0.0.93/setup.py
```

### Comparing `py3d-0.0.92/PKG-INFO` & `py3d-0.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.92
+Version: 0.0.93
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.92/README.md` & `py3d-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.92/py3d/core.py` & `py3d-0.0.93/py3d/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -358,19 +358,27 @@
         return p0 + (self - p0).vector_projection(p1 - p0)
 
     def projection_on_plane(self, plane) -> numpy.ndarray:
         return self + (plane.position[:, numpy.newaxis] - self).vector_projection(
             plane.normal[:, numpy.newaxis]
         )
 
-    def interp(self, xp, x):
+    def interpolate(self, x, xp) -> Vector3:
+        '''
+        linear interpolation
+        x: 1-D array, the data to be interpolated.
+        xp: 1-D array, the data to interpolate into. For example, time series.
+        '''
+        x = numpy.array(x)
+        xp = numpy.array(xp)
+        assert x.ndim <= xp.ndim == 1
         i = numpy.searchsorted(xp, x).clip(1, len(xp)-1)
         x0 = xp[i-1]
         x1 = xp[i]
-        d = ((x-x0)/(x1-x0))[:, numpy.newaxis]
+        d = ((x-x0)/(x1-x0)).reshape(-1,1)
         f0 = self[i-1]
         f1 = self[i]
         return (1-d)*f0+d*f1
 
     def as_scaling(self) -> Transform:
         ret = Transform(n=self.n)
         ret[..., 0, 0] = self[..., 0]
@@ -388,20 +396,22 @@
     def as_point(self, color=None) -> Point:
         entity = Point(*self.n)
         entity.xyz = self
         if color is not None:
             entity.color = color
         return entity
 
-    def as_line(self) -> LineSegment:
+    def as_line(self, color=None) -> LineSegment:
         n = list(self.n)
         n[-1] = (n[-1] - 1) * 2
         entity = LineSegment(*n)
         entity.start.xyz = self[..., :-1, :]
         entity.end.xyz = self[..., 1:, :]
+        if color is not None:
+            entity.color = color
         return entity
 
     def as_lineloop(self) -> LineSegment:
         n = list(self.n)
         n[-1] = n[-1] * 2
         entity = LineSegment(*n)
         entity.start.xyz = self
@@ -409,20 +419,23 @@
         return entity
 
     def as_linesegment(self) -> LineSegment:
         entity = LineSegment(*self.n)
         entity.xyz = self
         return entity
 
-    def as_shape(self) -> Triangle:
+    def as_shape(self, color=None) -> Triangle:
         v = numpy.repeat(self, 3, axis=self.ndim-2)
         v = numpy.roll(v, 1, axis=v.ndim-2)
         c = self.M[..., numpy.newaxis, :]
         v[..., 1::3, :] = c
-        return v.view(Vector3).as_triangle()
+        entity = v.view(Vector3).as_triangle()
+        if color is not None:
+            entity.color = color
+        return entity
 
     def as_triangle(self) -> Triangle:
         entity = Triangle(*self.n)
         entity.xyz = self
         return entity
 
     def as_vector(self) -> LineSegment:
@@ -705,15 +718,21 @@
             [0, 0, -2 * near * far * range_inv, 0]
         ])
 
     @classmethod
     def from_orthographic(cls, l, r, t, b, n, f):
         pass
 
-    def interp(self, xp, x) -> Transform:
+    def interpolate(self, x, xp) -> Transform:
+        '''
+        Linear interpolation
+        x: 1-D array, the data to be interpolated.
+        xp: 1-D array, the data to interpolate into. For example, time series.
+        Only translation, rotation and scaling can be interpolated
+        '''
         xp = numpy.array(xp)
         x = numpy.array(x)
         i = numpy.searchsorted(xp, x).clip(1, len(xp)-1)
         x0 = xp[i-1]
         x1 = xp[i]
         d: numpy.ndarray = (x-x0)/(x1-x0)
         r0: Transform = self.rotation[i-1]
```

### Comparing `py3d-0.0.92/py3d/viewer.html` & `py3d-0.0.93/py3d/viewer.html`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,14 @@
             return [
                 x ** 2 + (1 - x ** 2) * cos, -x * y * cos + x * y + z * sin, -x * z * cos + x * z - y * sin, 0,
                 -x * y * cos + x * y - z * sin, y ** 2 + (1 - y ** 2) * cos, x * sin - y * z * cos + y * z, 0,
                 -x * z * cos + x * z + y * sin, -x * sin - y * z * cos + y * z, z ** 2 + (1 - z ** 2) * cos, 0,
                 0, 0, 0, 1
             ]
         }
-        static distance(v0, v1) {
-            return Math.sqrt(Math.pow(v0[0] - v1[0], 2) + Math.pow(v0[1] - v1[1], 2) + Math.pow(v0[2] - v1[2], 2))
-        }
         static vm(v, m) {
             console.assert(m.length == 16 && v.length >= 3, m, v)
             let ret = []
             for (let j of [0, 1, 2, 3]) {
                 ret.push(m[j] * v[0] + m[j + 4] * v[1] + m[j + 8] * v[2] + m[j + 12])
             }
             return ret
@@ -85,27 +82,35 @@
                 }
             }
             ret[12] = -m[12]
             ret[13] = -m[13]
             ret[14] = -m[14]
             return ret
         }
-        static vec3_range(array) {
-            let x = array.filter((v, i) => i % 3 == 0)
-            let y = array.filter((v, i) => i % 3 == 1)
-            let z = array.filter((v, i) => i % 3 == 2)
-            return [Math.min(...x), Math.max(...x), Math.min(...y), Math.max(...y), Math.min(...z), Math.max(...z)]
+        static rgb2hex(r, g, b, a) {
+            return "#" + ((1 << 24) + (r * 255 << 16) + (g * 255 << 8) + b * 255 ).toString(16).slice(1)
+        }
+        static fround(value, digits) {
+            let tmp = 10**digits
+            return Math.round(value * tmp) / tmp
+        }
+        static fceil(value, digits) {
+            let tmp = 10**digits
+            return Math.ceil(value * tmp) / tmp
         }
         static ticks(min, max, step) {
             if (max <= min) {
                 return [[min], min, max]
             }
-            let dig = Math.round(Math.log10(step))
-            let size = Math.ceil((max - min) / step) + 1
-            let ticks = Array.from({ length: size }, (v, i) => Number((min + step * i).toFixed(Math.max(-dig, 0))))
+            let dig = Math.max(0, -Math.round(Math.log10(step)))
+            let r_min = mat.fround(min, dig)
+            let r_max = mat.fround(max, dig)
+            let r_step = mat.fceil(step, dig)
+            let size = Math.ceil((r_max - r_min) / r_step) + 1
+            let ticks = Array.from({ length: size }, (v, i) => mat.fround(r_min + r_step * i, dig))
             return [ticks, ticks[0], ticks[ticks.length - 1]]
         }
     }
     class Camera {
         PERSPECTIVE = "P"
         ORTHOGRAPHIC = "O"
         constructor(type, fovy, aspect, near, far, min, max) {
@@ -423,15 +428,20 @@
             let ny = p[1] / p[3]
             let nz = p[2] / p[3]
             if (Math.abs(nx) <= 1 && Math.abs(ny) <= 1 && Math.abs(nz) <= 1) {
                 let x = 0.5 * (1 + nx) * this.canvas.width
                 let y = 0.5 * (1 - ny) * this.canvas.height
                 div.style.left = x + "px"
                 div.style.top = y + "px"
-                div.style.color = color
+                if (typeof(color) == "string") {
+                    div.style.color = color
+                } else {
+                    div.style.color = mat.rgb2hex(color)
+                    div.style.opacity = color[color.length - 1]
+                }
                 div.style.pointerEvents = "none"
                 this.labeldiv.append(div)
             }
         }
         render() {
             this.labeldiv.innerHTML = ""
             this.gl.clearColor(0, 0, 0, 0)
@@ -463,31 +473,32 @@
         }
         grid(min, max, modelview, resolution) {
             let step = 50 * resolution// meter per pixel
             const [x_ticks, x_tick_min, x_tick_max] = mat.ticks(min[0], max[0], step)
             const [y_ticks, y_tick_min, y_tick_max] = mat.ticks(min[1], max[1], step)
             const [z_ticks, z_tick_min, z_tick_max] = mat.ticks(min[2], max[2], step)
             let lines = []
+            let text_color = [0.3, 0.3, 0.3, 0.6]
             for (let x of x_ticks) {
                 lines.push(x, y_tick_min, z_tick_min, x, y_tick_max, z_tick_min)
                 lines.push(x, y_tick_min, z_tick_min, x, y_tick_min, z_tick_max)
-                this.drawText(x, [x, y_tick_min, z_tick_min], "grey", modelview)
+                this.drawText(x, [x, y_tick_min, z_tick_min], text_color, modelview)
             }
             for (let y of y_ticks) {
                 lines.push(x_tick_min, y, z_tick_min, x_tick_max, y, z_tick_min)
                 lines.push(x_tick_min, y, z_tick_min, x_tick_min, y, z_tick_max)
-                this.drawText(y, [x_tick_min, y, z_tick_min], "grey", modelview)
+                this.drawText(y, [x_tick_min, y, z_tick_min], text_color, modelview)
             }
             for (let z of z_ticks) {
                 lines.push(x_tick_min, y_tick_min, z, x_tick_max, y_tick_min, z)
                 lines.push(x_tick_min, y_tick_min, z, x_tick_min, y_tick_max, z)
-                this.drawText(z, [x_tick_min, y_tick_min, z], "grey", modelview)
+                this.drawText(z, [x_tick_min, y_tick_min, z], text_color, modelview)
             }
-            this.drawText("X", [x_tick_max + step, y_tick_min, z_tick_min], "grey", modelview)
-            this.drawText("Y", [x_tick_min, y_tick_max + step, z_tick_min], "grey", modelview)
-            this.drawText("Z", [x_tick_min, y_tick_min, z_tick_max + step], "grey", modelview)
+            this.drawText("X", [x_tick_max + step, y_tick_min, z_tick_min], text_color, modelview)
+            this.drawText("Y", [x_tick_min, y_tick_max + step, z_tick_min], text_color, modelview)
+            this.drawText("Z", [x_tick_min, y_tick_min, z_tick_max + step], text_color, modelview)
             this.set_attribute("position", lines, 3)
-            this.set_attribute("color", Array.from({ length: lines.length / 3 * 4 }, (v, i) => i % 4 == 3 ? 1 : 0.5), 4)
+            this.set_attribute("color", Array.from({ length: lines.length / 3 * 4 }, (v, i) => i % 4 == 3 ? 0.6 : 0.3), 4)
             this.gl.drawArrays(this.gl.LINES, 0, lines.length / 3)
         }
     }
 </script>
```

### Comparing `py3d-0.0.92/py3d.egg-info/PKG-INFO` & `py3d-0.0.93/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.92
+Version: 0.0.93
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.92/setup.py` & `py3d-0.0.93/setup.py`

 * *Files identical despite different names*

