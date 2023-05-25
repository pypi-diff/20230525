# Comparing `tmp/streamlitopencvplayer-1.0.0.tar.gz` & `tmp/streamlitopencvplayer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.0.0.tar", last modified: Mon May 22 22:21:20 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.1.0.tar", last modified: Thu May 25 21:45:59 2023, max compression
```

## Comparing `streamlitopencvplayer-1.0.0.tar` & `streamlitopencvplayer-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 22:21:20.811699 streamlitopencvplayer-1.0.0/
--rw-rw-rw-   0        0        0      324 2023-05-22 22:21:20.810703 streamlitopencvplayer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      985 2023-05-10 09:24:37.000000 streamlitopencvplayer-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 22:21:20.812701 streamlitopencvplayer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-05-22 22:20:23.000000 streamlitopencvplayer-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 22:21:20.785699 streamlitopencvplayer-1.0.0/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.0.0/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     7131 2023-05-22 22:10:29.000000 streamlitopencvplayer-1.0.0/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-05-22 22:21:20.799699 streamlitopencvplayer-1.0.0/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      324 2023-05-22 22:21:20.000000 streamlitopencvplayer-1.0.0/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-22 22:21:20.000000 streamlitopencvplayer-1.0.0/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 22:21:20.000000 streamlitopencvplayer-1.0.0/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-22 22:21:20.000000 streamlitopencvplayer-1.0.0/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 22:21:20.806699 streamlitopencvplayer-1.0.0/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.0.0/test/__init__.py
--rw-rw-rw-   0        0        0      797 2023-05-22 15:32:01.000000 streamlitopencvplayer-1.0.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:45:59.585264 streamlitopencvplayer-1.1.0/
+-rw-rw-rw-   0        0        0      324 2023-05-25 21:45:59.583263 streamlitopencvplayer-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-05-10 09:24:37.000000 streamlitopencvplayer-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 21:45:59.586263 streamlitopencvplayer-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-05-25 21:45:30.000000 streamlitopencvplayer-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:45:59.555587 streamlitopencvplayer-1.1.0/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     7352 2023-05-25 21:45:15.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:45:59.571777 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-05-25 21:45:59.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-25 21:45:59.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 21:45:59.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-25 21:45:59.000000 streamlitopencvplayer-1.1.0/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 21:45:59.578264 streamlitopencvplayer-1.1.0/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.1.0/test/__init__.py
+-rw-rw-rw-   0        0        0      818 2023-05-25 21:34:02.000000 streamlitopencvplayer-1.1.0/test/test.py
```

### Comparing `streamlitopencvplayer-1.0.0/README.md` & `streamlitopencvplayer-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.0.0/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.1.0/streamlitopencvplayer/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import time
+
 import cv2
 import pandas as pd
 import streamlit as st
 from st_aggrid import AgGrid, GridOptionsBuilder
-import time
 
 # Initiate all session states used
 if 'counter' not in st.session_state:
     st.session_state['counter'] = 0
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
 
@@ -15,15 +16,15 @@
 
 def display_value():
     st.session_state['counter'] = st.session_state.myslider
 
 # Function to display video in the Streamlit app
 
 
-def display_video(video_path, alerts_dict, data,alerts):
+def display_video(video_path, alerts_dict, alerts, data):
     # Open the video file
     cap = cv2.VideoCapture(video_path)
     fps = cap.get(cv2.CAP_PROP_FPS)
     i = 0
 
     resume = False
     column1, column2, column3 = st.columns([1, 1.5, 1])
@@ -35,17 +36,16 @@
         df = pd.DataFrame(alerts_dict)
         options_builder = GridOptionsBuilder.from_dataframe(df)
         options_builder.configure_selection(
             selection_mode="single", use_checkbox=True)
         grid_options = options_builder.build()
         grid_return = AgGrid(df, grid_options)
         selected_rows = grid_return["selected_rows"]
-        # Buttons and zone of display
-    col1, col2, col3, col4, col5 = st.columns(
-        [1, 4, 1, 1.5, 0.5])
+    # Buttons and zone of display
+    col1, col2, col3, col4, col5 = st.columns(5)
     with col1:
         st.write('')
         st.write('')
         container_2 = st.empty()
         pause = container_2.button('⏸')
 
     with col2:
@@ -73,16 +73,19 @@
         st.session_state['counter'] = 0
         st.session_state['frames'] = []
     if selected_rows:
         selected_rows = grid_return["selected_rows"][0]["Alerts"]
 
         if plus:
             st.session_state['counter'] = st.session_state['counter']+1
+        elif minus:
+            st.session_state['counter'] = st.session_state['counter']-1
         else:
             st.session_state['counter'] = selected_rows
+
         widget.slider("", min_value=0, max_value=int(
             cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
         container_2.empty()
         pause = container_2.button('▶')
         resume = True
         # get all the frames from video when the list is empty
     if not st.session_state['frames']:
@@ -93,50 +96,51 @@
                 st.session_state['frames'].append(frames)
             else:
                 break
         cap.release()
     # back to the first frame if the video is finished
     if st.session_state['counter'] == len(st.session_state['frames']):
         st.session_state['counter'] = 0
+        del st.session_state.myslider
     stframe.image(st.session_state['frames']
                   [st.session_state['counter']], caption='', width=450)
     try:
         while st.session_state['counter'] < len(st.session_state['frames']):
             if not resume:
                 if i < len(data):
-                            if st.session_state['counter'] == int(alerts[i]*fps):
-                                # draw all detections on the frame
-                                for j in range(len(data[i])):
-                                    output = cv2.rectangle(st.session_state['frames'][st.session_state['counter']], (data[i][j][0][0], data[i][j][0][1]), (
-                                        data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
-                                    output = cv2.putText(
-                                        st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
-                                # update image zone with detections
-                                stframe.image(output, caption='', width=500)
-                                time.sleep(0.08)
-                                # the detection is drawn, to the next one
-                                i += 1
-                                st.session_state['counter'] += 1
-                                # frame_number.slider_changed(st.session_state['counter'])
-
-                                # update slider value
-                                widget.slider("", min_value=0, max_value=int(
-                    cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
+                    if st.session_state['counter'] == int(alerts[i]*fps):
+                        # draw all detections on the frame
+                        for j in range(len(data[i])):
+                            output = cv2.rectangle(st.session_state['frames'][st.session_state['counter']], (data[i][j][0][0], data[i][j][0][1]), (
+                                data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
+                            output = cv2.putText(
+                                st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
+                        # update image zone with detections
+                        stframe.image(output, caption='', width=500)
+                        time.sleep(0.08)
+                        # the detection is drawn, to the next one
+                        i += 1
+                        st.session_state['counter'] += 1
+                        # frame_number.slider_changed(st.session_state['counter'])
+
+                        # update slider value
+                        widget.slider("", min_value=0, max_value=int(
+                            cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
                 stframe.image(
                     st.session_state['frames'][st.session_state['counter']], caption='', width=500)
                 time.sleep(0.08)
                 st.session_state['counter'] += 1
                 # update slider value
 
                 frame_num = widget.slider("", min_value=0, max_value=int(
                     cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
 
                 if st.session_state.myslider > frame_num:
                     del st.session_state.myslider
-                    #st.session_state.clear()
+                    # st.session_state.clear()
                     st.session_state['counter'] = frame_num
                     #st.session_state['counter'] = 0
                     resume = True
                     # st.experimental_rerun() #remove cache
                     break
 
                 if pause:
@@ -145,31 +149,33 @@
                 if plus:
                     resume = True
                     break
                 if minus:
                     st.session_state['counter'] -= 1
                     resume = True
                     break
+                    # back to the first frame if the video is finished
+                if st.session_state['counter'] == len(st.session_state['frames']):
+                    st.session_state['counter'] = 0
+                    del st.session_state.myslider
                 st.session_state['counter'] = frame_num
     except Exception as e:
         st.write('')
     if resume:
         container_2.empty()
         pause = container_2.button('▶')
         resume = False
 
-# Run the Streamlit app
-
 
 def main():
 
-    alerts_dict = {"Alerts": [43, 64]}
+    my_dict = {"Alerts": [43, 64]}
     alerts = [43, 64]
     data = [[[10, 100, 290, 200], 0.82, 0, "Class 0"],
             [[55, 22, 100, 120], 0.9, 1, "Class 1"]]
-    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-22T23%3A01%3A56Z&sp=r&sv=2021-08-06&sr=b&sig=UmdnieQArm9s2rnsMytmEOUel8R5Wu7ZtThDf6sL8nY%3D"
+    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-25T22%3A37%3A17Z&sp=r&sv=2021-08-06&sr=b&sig=Ev%2BgYuVoa00p82rLRBm%2ByqwN3ubvk%2Bb%2BI57Zp7zpWSU%3D"
     if video_path is not None:
-        display_video(video_path, alerts_dict, data,alerts)
+        display_video(video_path, my_dict, alerts, data)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `streamlitopencvplayer-1.0.0/test/test.py` & `streamlitopencvplayer-1.1.0/test/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-import streamlitopencvplayer
-from streamlitopencvplayer.app import display_video
 import streamlit as st
+
+from streamlitopencvplayer.app import display_video
+
 # Initiate all session states used
 if 'counter' not in st.session_state:
     st.session_state['counter'] = 0
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
+
+
 def main():
 
-    alerts = {"Alerts": [43, 64]}
+    alerts_dict = {"Alerts": [43, 64]}
+    alerts = [43, 64]
     data = [[[10, 100, 290, 200], 0.82, 0, "Class 0"],
             [[55, 22, 100, 120], 0.9, 1, "Class 1"]]
-    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-22T15%3A52%3A24Z&sp=r&sv=2021-08-06&sr=b&sig=wUTiwlgqE9cWJrAWELquNAimEahYFcd0cdGhIiFZ4ko%3D"
+    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-25T14%3A31%3A49Z&sp=r&sv=2021-08-06&sr=b&sig=358A3taHXFqd86m7CRCk9tbGW6V5K73nBD8H%2Bsu9QWk%3D"
     if video_path is not None:
-        display_video(video_path, alerts, data)
+        display_video(video_path, alerts_dict, alerts, data)
 
 
 if __name__ == "__main__":
     main()
```

