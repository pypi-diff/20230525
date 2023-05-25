# Comparing `tmp/arena-py-0.2.1.tar.gz` & `tmp/arena-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arena-py-0.2.1.tar", last modified: Wed Mar 15 16:09:12 2023, max compression
+gzip compressed data, was "dist/arena-py-0.3.0.tar", last modified: Wed Apr 12 14:49:34 2023, max compression
```

## Comparing `arena-py-0.2.1.tar` & `arena-py-0.3.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.736290 arena-py-0.2.1/
--rw-r--r--   0 mwfarb     (501) staff       (20)     1533 2020-12-01 18:59:55.000000 arena-py-0.2.1/LICENSE
--rw-r--r--   0 mwfarb     (501) staff       (20)     4346 2023-03-15 16:09:12.736114 arena-py-0.2.1/PKG-INFO
--rw-r--r--   0 mwfarb     (501) staff       (20)     3842 2023-02-02 16:06:13.000000 arena-py-0.2.1/README.md
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.724875 arena-py-0.2.1/arena/
--rw-r--r--   0 mwfarb     (501) staff       (20)      280 2022-06-06 21:30:11.000000 arena-py-0.2.1/arena/__init__.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)     3142 2022-06-24 16:57:42.000000 arena-py-0.2.1/arena/__main__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)    12326 2023-02-01 20:31:43.000000 arena-py-0.2.1/arena/arena_mqtt.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.727723 arena-py-0.2.1/arena/attributes/
--rw-r--r--   0 mwfarb     (501) staff       (20)      918 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/attributes/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1031 2021-03-01 16:34:58.000000 arena-py-0.2.1/arena/attributes/animation.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      139 2021-03-01 16:34:58.000000 arena-py-0.2.1/arena/attributes/animation_mixer.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      175 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/attributes/attribute.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1135 2021-06-28 19:02:43.000000 arena-py-0.2.1/arena/attributes/color.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     4684 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/attributes/data.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      342 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/attributes/goto_url.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      744 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/attributes/impulse.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      503 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/attributes/jitsi_video.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      811 2022-03-22 01:57:06.000000 arena-py-0.2.1/arena/attributes/landmark.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      637 2021-03-01 16:34:58.000000 arena-py-0.2.1/arena/attributes/material.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      263 2021-03-01 16:34:58.000000 arena-py-0.2.1/arena/attributes/morph.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      368 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/attributes/physics.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      496 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/attributes/position.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1616 2023-03-15 15:58:06.000000 arena-py-0.2.1/arena/attributes/rotation.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      355 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/attributes/scale.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      273 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/attributes/sound.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      439 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/attributes/text_input.py
--rw-r--r--   0 mwfarb     (501) staff       (20)    16321 2023-03-10 20:19:34.000000 arena-py-0.2.1/arena/auth.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1127 2021-09-15 13:49:45.000000 arena-py-0.2.1/arena/base_object.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     2684 2022-06-06 21:22:44.000000 arena-py-0.2.1/arena/device.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.728858 arena-py-0.2.1/arena/event_loop/
--rw-r--r--   0 mwfarb     (501) staff       (20)      267 2021-03-08 20:18:41.000000 arena-py-0.2.1/arena/event_loop/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      419 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/event_loop/async_worker.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1690 2021-06-28 19:02:43.000000 arena-py-0.2.1/arena/event_loop/asyncio_mqtt.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1749 2023-03-15 15:59:58.000000 arena-py-0.2.1/arena/event_loop/event_loop.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      651 2021-06-28 19:02:43.000000 arena-py-0.2.1/arena/event_loop/lazy_worker.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      841 2021-06-28 19:02:43.000000 arena-py-0.2.1/arena/event_loop/persistent_worker.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      129 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/event_loop/single_worker.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1171 2021-06-28 19:02:43.000000 arena-py-0.2.1/arena/event_loop/worker.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.729198 arena-py-0.2.1/arena/events/
--rw-r--r--   0 mwfarb     (501) staff       (20)       25 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/events/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      984 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/events/event.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.734040 arena-py-0.2.1/arena/objects/
--rw-r--r--   0 mwfarb     (501) staff       (20)     1262 2021-06-28 19:02:43.000000 arena-py-0.2.1/arena/objects/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     6679 2023-02-02 18:07:17.000000 arena-py-0.2.1/arena/objects/arena_object.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      516 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/box.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1569 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/camera.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      236 2021-03-07 12:08:38.000000 arena-py-0.2.1/arena/objects/circle.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      228 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/cone.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      243 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/cylinder.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      260 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/dodecahedron.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1320 2021-09-15 13:49:45.000000 arena-py-0.2.1/arena/objects/gltf.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      256 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/icosahedron.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      249 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/image.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/light.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      332 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/line.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      252 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/octahedron.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      244 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/particle.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/plane.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      228 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/ring.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      236 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/sphere.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      256 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/tetrahedron.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      264 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/text.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      968 2021-04-07 22:02:00.000000 arena-py-0.2.1/arena/objects/thickline.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/torus.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      248 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/torus_knot.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      244 2021-03-03 22:16:46.000000 arena-py-0.2.1/arena/objects/triangle.py
--rw-r--r--   0 mwfarb     (501) staff       (20)    15709 2023-03-10 22:46:29.000000 arena-py-0.2.1/arena/scene.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.734806 arena-py-0.2.1/arena/scripts/
--rw-r--r--   0 mwfarb     (501) staff       (20)        0 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/scripts/__init__.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      122 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/scripts/arena_py_permissions.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      557 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/scripts/arena_py_pub.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      118 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/scripts/arena_py_signout.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      559 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/scripts/arena_py_sub.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      229 2021-10-12 18:10:25.000000 arena-py-0.2.1/arena/scripts/arena_py_token.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.735099 arena-py-0.2.1/arena/utils/
--rw-r--r--   0 mwfarb     (501) staff       (20)       25 2021-01-22 22:37:37.000000 arena-py-0.2.1/arena/utils/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      781 2021-03-01 16:34:58.000000 arena-py-0.2.1/arena/utils/utils.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-03-15 16:09:12.735887 arena-py-0.2.1/arena_py.egg-info/
--rw-r--r--   0 mwfarb     (501) staff       (20)     4346 2023-03-15 16:09:12.000000 arena-py-0.2.1/arena_py.egg-info/PKG-INFO
--rw-r--r--   0 mwfarb     (501) staff       (20)     1999 2023-03-15 16:09:12.000000 arena-py-0.2.1/arena_py.egg-info/SOURCES.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)        1 2023-03-15 16:09:12.000000 arena-py-0.2.1/arena_py.egg-info/dependency_links.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)      308 2023-03-15 16:09:12.000000 arena-py-0.2.1/arena_py.egg-info/entry_points.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)      150 2023-03-15 16:09:12.000000 arena-py-0.2.1/arena_py.egg-info/requires.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)        6 2023-03-15 16:09:12.000000 arena-py-0.2.1/arena_py.egg-info/top_level.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)       38 2023-03-15 16:09:12.736345 arena-py-0.2.1/setup.cfg
--rw-r--r--   0 mwfarb     (501) staff       (20)     1451 2023-03-15 16:08:58.000000 arena-py-0.2.1/setup.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.762743 arena-py-0.3.0/
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1533 2020-12-01 18:59:55.000000 arena-py-0.3.0/LICENSE
+-rw-r--r--   0 mwfarb     (501) staff       (20)     4346 2023-04-12 14:49:34.762540 arena-py-0.3.0/PKG-INFO
+-rw-r--r--   0 mwfarb     (501) staff       (20)     3842 2023-02-02 16:06:13.000000 arena-py-0.3.0/README.md
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.751923 arena-py-0.3.0/arena/
+-rw-r--r--   0 mwfarb     (501) staff       (20)      280 2022-06-06 21:30:11.000000 arena-py-0.3.0/arena/__init__.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)     3142 2022-06-24 16:57:42.000000 arena-py-0.3.0/arena/__main__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)    12326 2023-03-27 15:44:34.000000 arena-py-0.3.0/arena/arena_mqtt.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.755380 arena-py-0.3.0/arena/attributes/
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1022 2023-04-11 20:21:11.000000 arena-py-0.3.0/arena/attributes/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1031 2021-03-01 16:34:58.000000 arena-py-0.3.0/arena/attributes/animation.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      139 2021-03-01 16:34:58.000000 arena-py-0.3.0/arena/attributes/animation_mixer.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      175 2021-01-22 22:37:37.000000 arena-py-0.3.0/arena/attributes/attribute.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1135 2021-06-28 19:02:43.000000 arena-py-0.3.0/arena/attributes/color.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     4974 2023-04-11 16:20:00.000000 arena-py-0.3.0/arena/attributes/data.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      362 2023-04-11 17:08:06.000000 arena-py-0.3.0/arena/attributes/goto_url.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      764 2023-04-11 16:29:38.000000 arena-py-0.3.0/arena/attributes/impulse.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      503 2021-10-12 18:10:25.000000 arena-py-0.3.0/arena/attributes/jitsi_video.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      811 2022-03-22 01:57:06.000000 arena-py-0.3.0/arena/attributes/landmark.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      611 2023-04-11 20:36:06.000000 arena-py-0.3.0/arena/attributes/material.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      237 2023-04-12 12:33:13.000000 arena-py-0.3.0/arena/attributes/morph.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      357 2023-04-11 20:36:06.000000 arena-py-0.3.0/arena/attributes/physics.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      496 2021-01-22 22:37:37.000000 arena-py-0.3.0/arena/attributes/position.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1616 2023-03-15 15:58:06.000000 arena-py-0.3.0/arena/attributes/rotation.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      355 2021-01-22 22:37:37.000000 arena-py-0.3.0/arena/attributes/scale.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      247 2023-04-11 20:36:06.000000 arena-py-0.3.0/arena/attributes/sound.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      475 2023-04-11 20:22:33.000000 arena-py-0.3.0/arena/attributes/text_input.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      152 2023-04-11 20:33:16.000000 arena-py-0.3.0/arena/attributes/video_control.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)    16321 2023-03-17 13:54:42.000000 arena-py-0.3.0/arena/auth.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1127 2021-09-15 13:49:45.000000 arena-py-0.3.0/arena/base_object.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     2684 2022-06-06 21:22:44.000000 arena-py-0.3.0/arena/device.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.756654 arena-py-0.3.0/arena/event_loop/
+-rw-r--r--   0 mwfarb     (501) staff       (20)      267 2021-03-08 20:18:41.000000 arena-py-0.3.0/arena/event_loop/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      419 2021-01-22 22:37:37.000000 arena-py-0.3.0/arena/event_loop/async_worker.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1690 2021-06-28 19:02:43.000000 arena-py-0.3.0/arena/event_loop/asyncio_mqtt.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1749 2023-03-15 15:59:58.000000 arena-py-0.3.0/arena/event_loop/event_loop.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      651 2021-06-28 19:02:43.000000 arena-py-0.3.0/arena/event_loop/lazy_worker.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      841 2021-06-28 19:02:43.000000 arena-py-0.3.0/arena/event_loop/persistent_worker.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      129 2021-01-22 22:37:37.000000 arena-py-0.3.0/arena/event_loop/single_worker.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1171 2021-06-28 19:02:43.000000 arena-py-0.3.0/arena/event_loop/worker.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.756945 arena-py-0.3.0/arena/events/
+-rw-r--r--   0 mwfarb     (501) staff       (20)       25 2021-01-22 22:37:37.000000 arena-py-0.3.0/arena/events/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      984 2021-01-22 22:37:37.000000 arena-py-0.3.0/arena/events/event.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.760442 arena-py-0.3.0/arena/objects/
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1262 2021-06-28 19:02:43.000000 arena-py-0.3.0/arena/objects/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     6766 2023-04-11 16:20:00.000000 arena-py-0.3.0/arena/objects/arena_object.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      516 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/box.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1569 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/camera.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      236 2021-03-07 12:08:38.000000 arena-py-0.3.0/arena/objects/circle.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      228 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/cone.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      243 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/cylinder.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      260 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/dodecahedron.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1320 2021-09-15 13:49:45.000000 arena-py-0.3.0/arena/objects/gltf.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      256 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/icosahedron.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      249 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/image.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/light.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      332 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/line.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      252 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/octahedron.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      244 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/particle.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/plane.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      228 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/ring.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      236 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/sphere.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      256 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/tetrahedron.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      264 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/text.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      968 2021-04-07 22:02:00.000000 arena-py-0.3.0/arena/objects/thickline.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/torus.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      248 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/torus_knot.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      244 2021-03-03 22:16:46.000000 arena-py-0.3.0/arena/objects/triangle.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)    16199 2023-04-12 12:52:26.000000 arena-py-0.3.0/arena/scene.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.761279 arena-py-0.3.0/arena/scripts/
+-rw-r--r--   0 mwfarb     (501) staff       (20)        0 2021-10-12 18:10:25.000000 arena-py-0.3.0/arena/scripts/__init__.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      122 2021-10-12 18:10:25.000000 arena-py-0.3.0/arena/scripts/arena_py_permissions.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      557 2021-10-12 18:10:25.000000 arena-py-0.3.0/arena/scripts/arena_py_pub.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      118 2021-10-12 18:10:25.000000 arena-py-0.3.0/arena/scripts/arena_py_signout.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      559 2021-10-12 18:10:25.000000 arena-py-0.3.0/arena/scripts/arena_py_sub.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      229 2021-10-12 18:10:25.000000 arena-py-0.3.0/arena/scripts/arena_py_token.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.761544 arena-py-0.3.0/arena/utils/
+-rw-r--r--   0 mwfarb     (501) staff       (20)       25 2021-01-22 22:37:37.000000 arena-py-0.3.0/arena/utils/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      781 2021-03-01 16:34:58.000000 arena-py-0.3.0/arena/utils/utils.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-04-12 14:49:34.762317 arena-py-0.3.0/arena_py.egg-info/
+-rw-r--r--   0 mwfarb     (501) staff       (20)     4346 2023-04-12 14:49:34.000000 arena-py-0.3.0/arena_py.egg-info/PKG-INFO
+-rw-r--r--   0 mwfarb     (501) staff       (20)     2033 2023-04-12 14:49:34.000000 arena-py-0.3.0/arena_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)        1 2023-04-12 14:49:34.000000 arena-py-0.3.0/arena_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)      308 2023-04-12 14:49:34.000000 arena-py-0.3.0/arena_py.egg-info/entry_points.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)      150 2023-04-12 14:49:34.000000 arena-py-0.3.0/arena_py.egg-info/requires.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)        6 2023-04-12 14:49:34.000000 arena-py-0.3.0/arena_py.egg-info/top_level.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)       38 2023-04-12 14:49:34.762800 arena-py-0.3.0/setup.cfg
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1451 2023-04-12 14:46:41.000000 arena-py-0.3.0/setup.py
```

### Comparing `arena-py-0.2.1/LICENSE` & `arena-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/PKG-INFO` & `arena-py-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.2.1
+Version: 0.3.0
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `arena-py-0.2.1/README.md` & `arena-py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/__main__.py` & `arena-py-0.3.0/arena/__main__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/arena_mqtt.py` & `arena-py-0.3.0/arena/arena_mqtt.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/attributes/__init__.py` & `arena-py-0.3.0/arena/attributes/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .morph import Morph
 from .physics import Physics
 from .position import Position
 from .rotation import Rotation
 from .scale import Scale
 from .sound import Sound
 from .text_input import TextInput
+from .video_control import VideoControl
 
 # [TODO]: do something with this
 ATTRIBUTE_TYPE_MAP = {
     "animation-mixer": AnimationMixer,
     "animation": Animation,
     "attribute": Attribute,
     "color": Color,
@@ -28,8 +29,10 @@
     "material": Material,
     "morph": Morph,
     "physics": Physics,
     "position": Position,
     "rotation": Rotation,
     "scale": Scale,
     "sound": Sound,
+    "text_input": TextInput,
+    "video_control": VideoControl,
 }
```

### Comparing `arena-py-0.2.1/arena/attributes/animation.py` & `arena-py-0.3.0/arena/attributes/animation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/attributes/color.py` & `arena-py-0.3.0/arena/attributes/color.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/attributes/data.py` & `arena-py-0.3.0/arena/attributes/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .rotation import Rotation
 from .goto_url import GotoUrl
 from .jitsi_video import JitsiVideo
 from .physics import Physics
 from .scale import Scale
 from .material import Material
 from .color import Color
+from .video_control import VideoControl
 
 class Data(Attribute):
     """
     Data Attribute. Wraps all attributes in JSON.
     """
     def __init__(self, **kwargs):
         data = {}
@@ -36,14 +37,22 @@
                 dash_words += [k]
                 k = "jitsi_video"
                 if isinstance(v, dict):
                     data[k] = JitsiVideo(**v)
                 else:
                     data[k] = v
 
+            if k == "video-control":
+                dash_words += [k]
+                k = "video_control"
+                if isinstance(v, dict):
+                    data[k] = VideoControl(**v)
+                else:
+                    data[k] = v
+
             # this could be called "clickable"
             if k == "click-listener":
                 if "clickable" in data:
                     k = "clickable"
                 else:
                     dash_words += [k]
                     k = "click_listener"
```

### Comparing `arena-py-0.2.1/arena/attributes/impulse.py` & `arena-py-0.3.0/arena/attributes/impulse.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from .position import Position
 
 class Impulse(Attribute):
     """
     Impulse Attribute.
     Usage: impulse=Impulse(...)
     """
-    def __init__(self, on="mousedown", force=Position(0,0,0), position=Position(0,0,0)):
+    def __init__(self, on="mousedown", force=Position(0,0,0), position=Position(0,0,0), **kwargs):
         if isinstance(force, Position):
             force = force.to_str()
         elif isinstance(force, tuple) or isinstance(force, list):
             force = Utils.tuple_to_string(force)
 
         if isinstance(position, Position):
             position = position.to_str()
         elif isinstance(position, tuple) or isinstance(position, list):
             position = Utils.tuple_to_string(position)
 
-        super().__init__(on=on, force=force, position=position)
+        super().__init__(on=on, force=force, position=position, **kwargs)
```

### Comparing `arena-py-0.2.1/arena/attributes/landmark.py` & `arena-py-0.3.0/arena/attributes/landmark.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/attributes/rotation.py` & `arena-py-0.3.0/arena/attributes/rotation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/auth.py` & `arena-py-0.3.0/arena/auth.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/base_object.py` & `arena-py-0.3.0/arena/base_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/device.py` & `arena-py-0.3.0/arena/device.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/event_loop/asyncio_mqtt.py` & `arena-py-0.3.0/arena/event_loop/asyncio_mqtt.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/event_loop/event_loop.py` & `arena-py-0.3.0/arena/event_loop/event_loop.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/event_loop/lazy_worker.py` & `arena-py-0.3.0/arena/event_loop/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/event_loop/persistent_worker.py` & `arena-py-0.3.0/arena/event_loop/persistent_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/event_loop/worker.py` & `arena-py-0.3.0/arena/event_loop/worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/events/event.py` & `arena-py-0.3.0/arena/events/event.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/objects/__init__.py` & `arena-py-0.3.0/arena/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/objects/arena_object.py` & `arena-py-0.3.0/arena/objects/arena_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,17 @@
 
             elif "collision_listener" == k:
                 json_data["collision-listener"] = v
 
             elif "animation_mixer" == k:
                 json_data["animation-mixer"] = v
 
+            elif "video_control" == k:
+                json_data["video-control"] = v
+
             # for animation, replace "start" and "end" with "from" and "to"
             elif isinstance(k, str) and "animation" == k[:len("animation")]:
                 animation = vars(v).copy()
                 Utils.dict_key_replace(animation, "start", "from")
                 Utils.dict_key_replace(animation, "end", "to")
                 json_data[k] = animation
             else:
```

### Comparing `arena-py-0.2.1/arena/objects/box.py` & `arena-py-0.3.0/arena/objects/box.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/objects/camera.py` & `arena-py-0.3.0/arena/objects/camera.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/objects/gltf.py` & `arena-py-0.3.0/arena/objects/gltf.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/objects/thickline.py` & `arena-py-0.3.0/arena/objects/thickline.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/scene.py` & `arena-py-0.3.0/arena/scene.py`

 * *Files 3% similar despite different names*

```diff
@@ -280,15 +280,29 @@
 
     def delete_object(self, obj):
         """Public function to delete an object"""
         payload = {
             "object_id": obj.object_id
         }
         Object.remove(obj)
-        return self._publish(payload, "delete")
+        return self._publish(payload, "delete", custom_payload=True)
+
+    def delete_attributes(self, obj, attributes=None):
+        """Public function to delete a list of 'attributes' as a string[], updating each to null"""
+        updated_data = {}
+        for attr in attributes:
+            obj.data[attr] = None  # remove from large internal storage
+            updated_data[attr] = None # remove from small external publish
+        payload = {
+            "object_id": obj.object_id,
+            "type": obj.type,
+            "persist": obj.persist,
+            "data": updated_data  # dashes handled from string array
+        }
+        return self._publish(payload, "update", custom_payload=True)
 
     def run_animations(self, obj):
         """Runs all dispatched animations"""
         if obj.animations:
             payload = {
                 "object_id": obj.object_id,
                 "type": obj.type,
@@ -302,29 +316,24 @@
                     if i == 0:
                         payload["data"][f"animation"] = anim
                     else:
                         payload["data"][f"animation__{i}"] = anim
                     Utils.dict_key_replace(anim, "start", "from")
                     Utils.dict_key_replace(anim, "end", "to")
             obj.clear_animations()
-            return self._publish(payload, "dispatch_animation")
+            return self._publish(payload, "update", custom_payload=True)
 
-    def _publish(self, obj, action):
+    def _publish(self, obj, action, custom_payload=False):
         """Publishes to mqtt broker with "action":action"""
         topic = f"{self.root_topic}/{self.mqttc_id}/{obj['object_id']}"
         d = datetime.utcnow().isoformat()[:-3]+"Z"
 
-        if action == "delete":
-            payload = obj
-            payload["action"] = "delete"
-            payload["timestamp"] = d
-            payload = json.dumps(payload)
-        elif action == "dispatch_animation":
+        if custom_payload:
             payload = obj
-            payload["action"] = "update"
+            payload["action"] = action
             payload["timestamp"] = d
             payload = json.dumps(payload)
         else:
             payload = obj.json(action=action, timestamp=d)
 
         self.mqttc.publish(topic, payload, qos=0)
         if self.debug: print("[publish]", topic, payload)
```

### Comparing `arena-py-0.2.1/arena/scripts/arena_py_pub.py` & `arena-py-0.3.0/arena/scripts/arena_py_pub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/scripts/arena_py_sub.py` & `arena-py-0.3.0/arena/scripts/arena_py_sub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena/utils/utils.py` & `arena-py-0.3.0/arena/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.2.1/arena_py.egg-info/PKG-INFO` & `arena-py-0.3.0/arena_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.2.1
+Version: 0.3.0
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `arena-py-0.2.1/arena_py.egg-info/SOURCES.txt` & `arena-py-0.3.0/arena_py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 arena/attributes/morph.py
 arena/attributes/physics.py
 arena/attributes/position.py
 arena/attributes/rotation.py
 arena/attributes/scale.py
 arena/attributes/sound.py
 arena/attributes/text_input.py
+arena/attributes/video_control.py
 arena/event_loop/__init__.py
 arena/event_loop/async_worker.py
 arena/event_loop/asyncio_mqtt.py
 arena/event_loop/event_loop.py
 arena/event_loop/lazy_worker.py
 arena/event_loop/persistent_worker.py
 arena/event_loop/single_worker.py
```

### Comparing `arena-py-0.2.1/setup.py` & `arena-py-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="arena-py",
-    version="0.2.1",
+    version="0.3.0",
     author="Conix Research Center",
     author_email="info@conix.io",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     description="Draw objects and run programs in the ARENA using Python!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arenaxr/ARENA-py",
```

