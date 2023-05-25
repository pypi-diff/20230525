# Comparing `tmp/snake-opencv-0.1.1.tar.gz` & `tmp/snake_opencv-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake-opencv-0.1.1.tar", max compression
+gzip compressed data, was "snake_opencv-0.1.2.tar", max compression
```

## Comparing `snake-opencv-0.1.1.tar` & `snake_opencv-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11358 2023-05-05 19:37:45.899387 snake-opencv-0.1.1/LICENSE
--rw-r--r--   0        0        0      460 2023-05-05 22:17:27.044555 snake-opencv-0.1.1/README.md
--rw-r--r--   0        0        0      686 2023-05-05 22:01:43.402463 snake-opencv-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      161 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/__init__.py
--rw-r--r--   0        0        0       44 2023-05-05 22:47:28.939893 snake-opencv-0.1.1/snake_opencv/core/__init__.py
--rw-r--r--   0        0        0    12427 2023-05-06 23:46:48.811339 snake-opencv-0.1.1/snake_opencv/core/binding.py
--rw-r--r--   0        0        0    24344 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/core/const.py
--rw-r--r--   0        0        0       44 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/dnn/__init__.py
--rw-r--r--   0        0        0     3607 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/dnn/binding.py
--rw-r--r--   0        0        0     1379 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/dnn/const.py
--rw-r--r--   0        0        0       44 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/highgui/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/highgui/binding.py
--rw-r--r--   0        0        0     2912 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/highgui/const.py
--rw-r--r--   0        0        0       44 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/imgcodecs/__init__.py
--rw-r--r--   0        0        0     5211 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/imgcodecs/binding.py
--rw-r--r--   0        0        0     1496 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/imgcodecs/const.py
--rw-r--r--   0        0        0       44 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/imgproc/__init__.py
--rw-r--r--   0        0        0    34260 2023-05-06 23:14:06.167539 snake-opencv-0.1.1/snake_opencv/imgproc/binding.py
--rw-r--r--   0        0        0    35343 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/imgproc/const.py
--rw-r--r--   0        0        0       44 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/photo/__init__.py
--rw-r--r--   0        0        0     3620 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/photo/binding.py
--rw-r--r--   0        0        0      854 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/photo/const.py
--rw-r--r--   0        0        0       44 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/videoio/__init__.py
--rw-r--r--   0        0        0     7240 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/videoio/binding.py
--rw-r--r--   0        0        0    29523 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/videoio/const.py
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 snake-opencv-0.1.1/setup.py
--rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 snake-opencv-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.2/LICENSE
+-rw-r--r--   0        0        0      460 2023-05-25 16:59:10.585668 snake_opencv-0.1.2/README.md
+-rw-r--r--   0        0        0      686 2023-05-25 16:59:35.011367 snake_opencv-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.2/snake_opencv/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.2/snake_opencv/core/__init__.py
+-rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.2/snake_opencv/core/binding.py
+-rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.2/snake_opencv/core/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.2/snake_opencv/dnn/__init__.py
+-rw-r--r--   0        0        0     3607 2023-05-25 16:59:10.587684 snake_opencv-0.1.2/snake_opencv/dnn/binding.py
+-rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.2/snake_opencv/dnn/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.2/snake_opencv/highgui/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.2/snake_opencv/highgui/binding.py
+-rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.2/snake_opencv/highgui/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.2/snake_opencv/imgcodecs/__init__.py
+-rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.2/snake_opencv/imgcodecs/binding.py
+-rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.2/snake_opencv/imgcodecs/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.2/snake_opencv/imgproc/__init__.py
+-rw-r--r--   0        0        0    37011 2023-05-25 17:52:22.840887 snake_opencv-0.1.2/snake_opencv/imgproc/binding.py
+-rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.2/snake_opencv/imgproc/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.2/snake_opencv/photo/__init__.py
+-rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.2/snake_opencv/photo/binding.py
+-rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.2/snake_opencv/photo/const.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.2/snake_opencv/py.typed
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.2/snake_opencv/videoio/__init__.py
+-rw-r--r--   0        0        0     7240 2023-05-25 16:59:10.590449 snake_opencv-0.1.2/snake_opencv/videoio/binding.py
+-rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.2/snake_opencv/videoio/const.py
+-rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 snake_opencv-0.1.2/PKG-INFO
```

### Comparing `snake-opencv-0.1.1/LICENSE` & `snake_opencv-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/pyproject.toml` & `snake_opencv-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snake-opencv"
-version = "0.1.1"
+version = "0.1.2"
 repository = "https://github.com/cospectrum/snake-opencv"
 description = "Snake case opencv with type annotations"
 license = "Apache-2.0"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "snake_opencv"}]
```

### Comparing `snake-opencv-0.1.1/snake_opencv/core/binding.py` & `snake_opencv-0.1.2/snake_opencv/core/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/core/const.py` & `snake_opencv-0.1.2/snake_opencv/core/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/dnn/binding.py` & `snake_opencv-0.1.2/snake_opencv/dnn/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/dnn/const.py` & `snake_opencv-0.1.2/snake_opencv/dnn/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/highgui/binding.py` & `snake_opencv-0.1.2/snake_opencv/highgui/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/highgui/const.py` & `snake_opencv-0.1.2/snake_opencv/highgui/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/imgcodecs/binding.py` & `snake_opencv-0.1.2/snake_opencv/imgcodecs/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/imgcodecs/const.py` & `snake_opencv-0.1.2/snake_opencv/imgcodecs/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/imgproc/binding.py` & `snake_opencv-0.1.2/snake_opencv/imgproc/binding.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     'get_perspective_transform',
     'warp_perspective',
     'laplacian',
     'threshold',
     'connected_components_with_stats',
     'connected_components',
     'match_template',
+    'warp_affine',
+    'get_affine_transform',
 ]
 
 
 LineType = Literal[-1, 4, 8, 16]
 
 
 Width = int
@@ -90,15 +92,15 @@
             scale factor along the horizontal axis; when it equals 0, it is
             computed as dsize.width / src.cols
         fy:
             scale factor along the vertical axis; when it equals 0, it is
             computed as dsize.height / src.rows
         interpolation: interpolation method, see #InterpolationFlags
     """
-    return cv2.resize(
+    return cv2.resize(  # type: ignore
         src,
         dsize,
         dst,
         fx=fx,
         fy=fy,
         interpolation=interpolation,
     )
@@ -154,15 +156,15 @@
         code: color space conversion code (see #ColorConversionCodes).
         dst: output image of the same size and depth as src.
         dst_cn:
             number of channels in the destination image; if the parameter is
             0, the number of the channels is derived automatically from src
             and code.
     """
-    return cv2.cvtColor(src, code, dst, dst_cn)
+    return cv2.cvtColor(src, code, dst, dst_cn)  # type: ignore
 
 
 X = int
 Y = int
 Scalar = Union[Tuple[float, ...], float]
 
 
@@ -188,15 +190,15 @@
         thickness:
             Thickness of lines that make up the rectangle. Negative values,
             like #FILLED, mean that the function has to draw a filled
             rectangle.
         line_type: Type of the line. See #LineTypes
         shift: Number of fractional bits in the point coordinates.
     """
-    return cv2.rectangle(image, pt1, pt2, color, thickness, line_type, shift)
+    return cv2.rectangle(image, pt1, pt2, color, thickness, line_type, shift)  # type: ignore
 
 
 def circle(
     image: np.ndarray,
     center: Tuple[X, Y],
     radius: int,
     color: Scalar,
@@ -218,15 +220,15 @@
             Thickness of the circle outline, if positive. Negative values,
             like #FILLED, mean that a filled circle is to be drawn.
         line_type: Type of the circle boundary. See #LineTypes
         shift:
             Number of fractional bits in the coordinates of the center and in
             the radius value.
     """
-    return cv2.circle(
+    return cv2.circle(  # type: ignore
         image,
         center,
         radius,
         color,
         thickness,
         line_type,
         shift=shift,
@@ -255,15 +257,15 @@
         pt1: First point of the line segment.
         pt2: Second point of the line segment.
         color: Line color.
         thickness: Line thickness.
         line_type: Type of the line. See #LineTypes.
         shift: Number of fractional bits in the point coordinates.
     """
-    return cv2.line(image, pt1, pt2, color, thickness, line_type, shift)
+    return cv2.line(image, pt1, pt2, color, thickness, line_type, shift)  # type: ignore
 
 
 def fill_poly(
     image: np.ndarray,
     pts: List[np.ndarray],
     color: Scalar,
     line_type: LineType = 8,
@@ -283,15 +285,15 @@
             Array of polygons where each polygon is represented as an array of
             points.
         color: Polygon color.
         line_lype: Type of the polygon boundaries. See #LineTypes
         shift: Number of fractional bits in the vertex coordinates.
         offset: Optional offset of all points of the contours.
     """
-    return cv2.fillPoly(image, pts, color, line_type, shift, offset)
+    return cv2.fillPoly(image, pts, color, line_type, shift, offset)  # type: ignore
 
 
 def put_text(
     image: np.ndarray,
     text: str,
     org: Tuple[X, Y],
     font_face: int,
@@ -318,15 +320,15 @@
         color: Text color.
         thickness: Thickness of the lines used to draw a text.
         line_type: Line type. See #LineTypes
         bottom_left_origin:
             When true, the image data origin is at the bottom-left corner.
             Otherwise, it is at the top-left corner.
     """
-    return cv2.putText(
+    return cv2.putText(  # type: ignore
         image,
         text,
         org,
         font_face,
         font_scale,
         color,
         thickness,
@@ -361,15 +363,15 @@
         aperture_size: aperture size for the Sobel operator.
         l2gradient:
             a flag, indicating whether a more accurate
             l2-norm = sqrt((dI/dx)^2 + (dI/dy)^2) should be used to calculate
             the image gradient magnitude (l2gradient=true), or whether the
             default l1-norm = |dI/dx| + |dI/dy| is enough (l2gradient=false).
     """
-    return cv2.Canny(
+    return cv2.Canny(  # type: ignore
         image,
         threshold1,
         threshold2,
         edges=edges,
         apertureSize=aperture_size,
         L2gradient=l2gradient,
     )
@@ -404,15 +406,15 @@
         mode: Contour retrieval mode, see #RetrievalModes
         method: Contour approximation method, see #ContourApproximationModes
         offset:
             Optional offset by which every contour point is shifted. This is
             useful if the contours are extracted from the image ROI and then
             they should be analyzed in the whole image context.
     """
-    return cv2.findContours(image, mode=mode, method=method, offset=offset)
+    return cv2.findContours(image, mode=mode, method=method, offset=offset)  # type: ignore
 
 
 def draw_contours(
     image: np.ndarray,
     contours: Contours,
     contour_idx: int,
     color: Scalar,
@@ -451,15 +453,15 @@
             when there is hierarchy available.
         offset:
             Optional contour shift parameter.
             Shift all the drawn contours by the specified offset = (dx, dy).
 
     Returns: destination image.
     """
-    return cv2.drawContours(
+    return cv2.drawContours(  # type: ignore
         image,
         contours,
         contour_idx,
         color,
         thickness,
         line_type,
         hierarchy,
@@ -499,15 +501,15 @@
             (see #getGaussianKernel for details); to fully control the result
             regardless of possible future modifications of all this semantics,
             it is recommended to specify all of ksize, sigmaX, and sigmaY.
         border_type:
             pixel extrapolation method, see #BorderTypes.
             #BORDER_WRAP is not supported.
     """
-    return cv2.GaussianBlur(src, ksize, sigma_x, dst, sigma_y, border_type)
+    return cv2.GaussianBlur(src, ksize, sigma_x, dst, sigma_y, border_type)  # type: ignore
 
 
 def hough_lines(
     image: np.ndarray,
     rho: float,
     theta: float,
     threshold: int,
@@ -554,15 +556,15 @@
             check for lines. Must fall between 0 and max_theta.
         max_theta:
             For standard and multi-scale Hough transform, an upper bound for
             the angle. Must fall between min_theta and CV_PI. The actual
             maximum angle in the accumulator may be slightly less than
             max_theta, depending on the parameters min_theta and theta.
     """
-    return cv2.HoughLines(
+    return cv2.HoughLines(  # type: ignore
         image,
         rho=rho,
         theta=theta,
         threshold=threshold,
         lines=lines,
         srn=srn,
         stn=stn,
@@ -601,15 +603,15 @@
             vector (x1, y1, x2, y2), where (x1, y1) and (x2, y2) are the
             ending points of each detected line segment.
         min_line_length:
             Minimum line length. Line segments shorter than that are rejected.
         max_line_gap:
             Maximum allowed gap between points on the same line to link them.
     """
-    return cv2.HoughLinesP(
+    return cv2.HoughLinesP(  # type: ignore
         image,
         rho,
         theta,
         threshold,
         lines,
         min_line_length,
         max_line_gap,
@@ -629,15 +631,15 @@
     (possibly rotated) for a specified point set. Developer should keep in
     mind that the returned RotatedRect can contain negative indices when data
     is close to the containing Mat element boundary.
 
     Args:
         points: Input vector of 2D points.
     """
-    return cv2.minAreaRect(points)
+    return cv2.minAreaRect(points)  # type: ignore
 
 
 def box_points(
     box: RotatedRect,
     points: Optional[np.ndarray] = None,
 ) -> np.ndarray:
     """Finds the four vertices of a rotated rect. Useful to draw the rotated
@@ -649,15 +651,15 @@
     tutorial_bounding_rotated_ellipses “tutorial on Creating Bounding rotated
     boxes and ellipses for contours” for more information.
 
     Args:
         box: The input rotated rectangle. It may be the output of
         points: The output array of four vertices of rectangles.
     """
-    return cv2.boxPoints(box, points)
+    return cv2.boxPoints(box, points)  # type: ignore
 
 
 def get_perspective_transform(
     src: np.ndarray,
     dst: np.ndarray,
     solve_method: int = DECOMP_LU,
 ) -> np.ndarray:
@@ -667,15 +669,15 @@
     Args:
         src: Coordinates of quadrangle vertices in the source image.
         dst:
             Coordinates of the corresponding quadrangle vertices in the
             destination image.
         solve_method: method passed to cv::solve (#DecompTypes)
     """
-    return cv2.getPerspectiveTransform(src, dst, solve_method)
+    return cv2.getPerspectiveTransform(src, dst, solve_method)  # type: ignore
 
 
 def warp_perspective(
     src: np.ndarray,
     m: np.ndarray,
     dsize: Tuple[Width, Height],
     dst: Optional[np.ndarray] = None,
@@ -701,15 +703,15 @@
             pixel extrapolation method (#BORDER_CONSTANT or
             #BORDER_REPLICATE).
         border_value:
             value used in case of a constant border; by default, it equals 0.
 
     Returns: output image that has the size dsize and the same type as src
     """
-    return cv2.warpPerspective(
+    return cv2.warpPerspective(  # type: ignore
         src,
         m,
         dsize,
         dst,
         flag,
         border_mode,
         border_value,
@@ -753,15 +755,15 @@
         delta:
             Optional delta value that is added to the results prior to storing
             them in dst.
         border_type:
             Pixel extrapolation method, see #BorderTypes. #BORDER_WRAP is not
             supported.
     """
-    return cv2.Laplacian(
+    return cv2.Laplacian(  # type: ignore
         src,
         ddepth,
         dst,
         ksize=ksize,
         scale=scale,
         delta=delta,
         borderType=border_type,
@@ -801,15 +803,15 @@
         type: thresholding type (see #ThresholdTypes).
         dst:
             output array of the same size and type and the same number of
             channels as src.
 
     Returns: the computed threshold value if Otsu’s or Triangle methods used.
     """
-    return cv2.threshold(
+    return cv2.threshold(  # type: ignore
         src,
         thresh,
         maxval,
         type=type,
         dst=dst,
     )
 
@@ -855,15 +857,15 @@
             centroid output for each label, including the background label.
             Centroids are accessed via centroids(label, 0) for x and
             centroids(label, 1) for y. The data type CV_64F.
         connectivity: 8 or 4 for 8-way or 4-way connectivity respectively
         ltype:
             output image label type. Currently CV_32S and CV_16U are supported.
     """
-    return cv2.connectedComponentsWithStats(
+    return cv2.connectedComponentsWithStats(  # type: ignore
         image,
         labels=labels,
         stats=stats,
         centroids=centroids,
         connectivity=connectivity,
         ltype=ltype,
     )
@@ -893,15 +895,15 @@
     Args:
         image: the 8-bit single-channel image to be labeled
         labels: destination labeled image
         connectivity: 8 or 4 for 8-way or 4-way connectivity respectively
         ltype:
             output image label type. Currently CV_32S and CV_16U are supported.
     """
-    return cv2.connectedComponents(
+    return cv2.connectedComponents(  # type: ignore
         image,
         labels=labels,
         connectivity=connectivity,
         ltype=ltype,
     )
 
 
@@ -949,14 +951,80 @@
             which is then used for all template and image channels. If the data
             type is CV_8U, the mask is interpreted as a binary mask, meaning
             only elements where mask is nonzero are used and are kept unchanged
             independent of the actual mask value (weight equals 1). For data
             tpye CV_32F, the mask values are used as weights. The exact
             formulas are documented in TemplateMatchModes.
     """
-    return cv2.matchTemplate(
+    return cv2.matchTemplate(  # type: ignore
         image,
         templ=templ,
         method=method,
         result=result,
         mask=mask,
     )
+
+
+def warp_affine(
+    src: np.ndarray,
+    m: np.ndarray,
+    dsize: Tuple[Width, Height],
+    dst: Optional[np.ndarray] = None,
+    flags: int = INTER_LINEAR,
+    border_mode: int = BORDER_CONSTANT,
+    border_value: Optional[Scalar] = None,
+) -> np.ndarray:
+    """Applies an affine transformation to an image.
+
+    The function warpAffine transforms the source image using the specified
+    matrix:
+        𝚍𝚜𝚝(x,y) = 𝚜𝚛𝚌(𝙼11x + 𝙼12y + 𝙼13, 𝙼21x + 𝙼22y + 𝙼23)
+
+    when the flag WARP_INVERSE_MAP is set. Otherwise, the transformation is
+    first inverted with invertAffineTransform and then put in the formula
+    above instead of M. The function cannot operate in-place.
+
+    Args:
+        src: input image.
+        dst: output image that has the size dsize and the same type as src.
+        M: 2×3 transformation matrix.
+        dsize: size of the output image.
+        flags:
+            combination of interpolation methods (see InterpolationFlags) and
+            the optional flag WARP_INVERSE_MAP that means that M is the
+            inverse transformation ( 𝚍𝚜𝚝→𝚜𝚛𝚌 ).
+        border_mode:
+            pixel extrapolation method (see BorderTypes); when
+            borderMode=BORDER_TRANSPARENT, it means that the pixels in the
+            destination image corresponding to the "outliers" in the source
+            image are not modified by the function.
+        border_value:
+            value used in case of a constant border; by default, it is 0.
+    """
+    return cv2.warpAffine(  # type: ignore
+        src,
+        m,
+        dsize=dsize,
+        dst=dst,
+        flags=flags,
+        borderMode=border_mode,
+        borderValue=border_value,
+    )
+
+
+def get_affine_transform(src: np.ndarray, dst: np.ndarray) -> np.ndarray:
+    """Calculates an affine transform from three pairs of the corresponding
+    points.
+
+    The function calculates the 2×3 matrix of an affine transform so that:
+        [x', y'].T == map_matrix * [x, y, 1].T
+
+    where
+        dst(i) = (x'i, y'i), src(i) = (xi, yi),  i = 0, 1, 2
+
+    Args:
+        src: Coordinates of triangle vertices in the source image.
+        dst:
+            Coordinates of the corresponding triangle vertices in the
+            destination image.
+    """
+    return cv2.getAffineTransform(src, dst=dst)  # type: ignore
```

### Comparing `snake-opencv-0.1.1/snake_opencv/imgproc/const.py` & `snake_opencv-0.1.2/snake_opencv/imgproc/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/photo/binding.py` & `snake_opencv-0.1.2/snake_opencv/photo/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/photo/const.py` & `snake_opencv-0.1.2/snake_opencv/photo/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/videoio/binding.py` & `snake_opencv-0.1.2/snake_opencv/videoio/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/snake_opencv/videoio/const.py` & `snake_opencv-0.1.2/snake_opencv/videoio/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.1/PKG-INFO` & `snake_opencv-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: snake-opencv
-Version: 0.1.1
+Version: 0.1.2
 Summary: Snake case opencv with type annotations
 Home-page: https://github.com/cospectrum/snake-opencv
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: opencv-python (>=4.0,<5.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/cospectrum/snake-opencv
 Description-Content-Type: text/markdown
 
 # Snake-OpenCV
 Snake case OpenCV with type annotations for Python.
```

