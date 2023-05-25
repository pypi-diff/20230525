# Comparing `tmp/pymodaq-4.0.1.tar.gz` & `tmp/pymodaq-4.0.2.tar.gz`

## Comparing `pymodaq-4.0.1.tar` & `pymodaq-4.0.2.tar`

### file list

```diff
@@ -1,413 +1,418 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/__init__.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/daq_utils.py
--rw-r--r--   0        0        0    61748 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/dashboard.py
--rw-r--r--   0        0        0    74359 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/icon.ico
--rw-r--r--   0        0        0    53114 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/splash.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/__init__.py
--rw-r--r--   0        0        0    39848 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/daq_move.py
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/daq_move_ui.py
--rw-r--r--   0        0        0    64099 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/daq_viewer.py
--rw-r--r--   0        0        0    15462 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/daq_viewer_ui.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/mocks.py
--rw-r--r--   0        0        0    30500 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/move_utility_classes.py
--rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/utils.py
--rw-r--r--   0        0        0    26665 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/control_modules/viewer_utility_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/__init__.py
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/custom_app.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/custom_viewer.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/function_plotter.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/nonlinearscanner.py
--rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/parameter_ex.py
--rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/preset_MockCamera.xml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.aliases
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvlps
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj
--rw-r--r--   0        0        0    69358 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi
--rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi
--rw-r--r--   0        0        0    29785 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi
--rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi
--rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi
--rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi
--rw-r--r--   0        0        0    19039 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi
--rw-r--r--   0        0        0    19791 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/console.py
--rw-r--r--   0        0        0    19481 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/daq_logger.py
--rw-r--r--   0        0        0    56107 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/daq_scan.py
--rw-r--r--   0        0        0    10123 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/daq_scan_ui.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/h5browser.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/utils.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/pid/__init__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/pid/daq_move_PID.py
--rw-r--r--   0        0        0    29797 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/pid/pid_controller.py
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/extensions/pid/utils.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/__init__.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/load_and_plot.py
--rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/process_to_scalar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/daq_analysis/__init__.py
--rw-r--r--   0        0        0    24346 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/daq_analysis/daq_analysis_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/daq_measurement/__init__.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui
--rw-r--r--   0        0        0    17093 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/post_treatment/daq_measurement/process_from_QtDesigner_DAQ_Measurement_GUI.bat
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/VERSION
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/__init__.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/config_template.toml
--rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/preset_default.xml
--rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/triangulation_data.npy
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.bat
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc
--rw-r--r--   0        0        0  8225442 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/__init__.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/icons.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/1d.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/2d.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/3d.png
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add2.png
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve.png
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve_All.png
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png
--rw-r--r--   0        0        0    47401 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnGroup.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnNum.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnText.png
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnTime.png
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnWave.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Close3.png
--rw-r--r--   0        0        0    47830 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png
--rw-r--r--   0        0        0    48054 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png
--rw-r--r--   0        0        0    48959 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Contract.png
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Create.png
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png
--rw-r--r--   0        0        0    49034 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png
--rw-r--r--   0        0        0    48413 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ErrorMessage.png
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png
--rw-r--r--   0        0        0    48491 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Expand.png
--rw-r--r--   0        0        0    47692 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png
--rw-r--r--   0        0        0    48102 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/FFT.png
--rw-r--r--   0        0        0    89487 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Histogram.png
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/LUT_LookUpTable.png
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Marker.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Math.png
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png
--rw-r--r--   0        0        0    48221 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png
--rw-r--r--   0        0        0    47229 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png
--rw-r--r--   0        0        0    47258 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Multiply.png
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png
--rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_File.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_Folder.png
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File.png
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png
--rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope_16.png
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Pass.png
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RGB.png
--rw-r--r--   0        0        0    47228 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png
--rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh2.png
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Region.png
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rendezvous.png
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SELECT.png
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save.png
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll.png
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png
--rw-r--r--   0        0        0    49529 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Search.png
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png
--rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png
--rw-r--r--   0        0        0    49414 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png
--rw-r--r--   0        0        0    49581 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png
--rw-r--r--   0        0        0    52734 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Spreadsheet.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics.png
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics2.png
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Status.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Subtract.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Vision.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Volts.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Wait2.png
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_1_1.png
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_in.png
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_out.png
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_to_Selection.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/abort.png
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/advanced2.png
--rw-r--r--   0        0        0    47292 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/b_icon.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/back.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/bg_icon.png
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera.png
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cartesian.png
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/close2.png
--rw-r--r--   0        0        0    47742 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color.png
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color2.png
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/continuous.png
--rw-r--r--   0        0        0    47210 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download.png
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download2.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/error2.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ethernet.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/fan.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/filter2.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/g_icon.png
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to.png
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grab.png
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/graph.png
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grey_icon.png
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greyscale.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1.png
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1_32.png
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/home2.png
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/integrator.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/joystick.png
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/limiter.png
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png
--rw-r--r--   0        0        0    50113 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png
--rw-r--r--   0        0        0    47361 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_straight_line.png
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/movie.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multi_point.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multiplexer.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/new.png
--rw-r--r--   0        0        0    48254 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png
--rw-r--r--   0        0        0    49028 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png
--rw-r--r--   0        0        0    48669 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/overlay.png
--rw-r--r--   0        0        0    24121 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pause.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/permute.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/phase.png
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/play.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/polar.png
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pole_zero.png
--rw-r--r--   0        0        0    47612 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/properties.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/r_icon.png
--rw-r--r--   0        0        0    47081 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/read2.png
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/remove.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/reset.png
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rgb_icon.png
--rw-r--r--   0        0        0    49951 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png
--rw-r--r--   0        0        0    47140 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run2.png
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saturation.png
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_horizontally.png
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_vertically.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/search2.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select2.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all.png
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_none.png
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence2.png
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/snap.png
--rw-r--r--   0        0        0    47434 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/start.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/status_cancelled.png
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop.png
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop3.png
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sum.png
--rw-r--r--   0        0        0    50597 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/tree.png
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/vector.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/verify.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/video.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/wait.png
--rw-r--r--   0        0        0    50127 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/watershed.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomAuto.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomReset.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/__init__.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/array_manipulation.py
--rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/calibration_camera.py
--rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/chrono_timer.py
--rw-r--r--   0        0        0    15404 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/config.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/conftests.py
--rw-r--r--   0        0        0    26941 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/daq_utils.py
--rw-r--r--   0        0        0    69686 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/data.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/enums.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/exceptions.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/factory.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/logger.py
--rw-r--r--   0        0        0    17513 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/math_utils.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/messenger.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/qvariant.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/slicing.py
--rw-r--r--   0        0        0    39074 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/tcp_server_client.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/units.py
--rw-r--r--   0        0        0   418388 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.odt
--rw-r--r--   0        0        0   361273 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.pdf
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/Tuto innosetup/script_full_setup.iss
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/abstract/__init__.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/abstract/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/db/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/db/db_logger/__init__.py
--rw-r--r--   0        0        0    12416 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/db/db_logger/db_logger.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/db/db_logger/db_logger_models.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/__init__.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/custom_app.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/dock.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/file_io.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/layout.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/list_picker.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/utils.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/label.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/lcd.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/push.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/qled.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/spinbox.py
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/table.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/h5modules/__init__.py
--rw-r--r--   0        0        0    31651 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/h5modules/backends.py
--rw-r--r--   0        0        0    26370 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/h5modules/browsing.py
--rw-r--r--   0        0        0    31499 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/h5modules/data_saving.py
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/h5modules/h5logging.py
--rw-r--r--   0        0        0    12061 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/h5modules/module_saving.py
--rw-r--r--   0        0        0    36566 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/h5modules/saving.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/h5modules/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/__init__.py
--rw-r--r--   0        0        0    16788 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/action_manager.py
--rw-r--r--   0        0        0    13905 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/batchscan_manager.py
--rw-r--r--   0        0        0    20277 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/modules_manager.py
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/overshoot_manager.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/parameter_manager.py
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/preset_manager.py
--rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/preset_manager_utils.py
--rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/remote_manager.py
--rw-r--r--   0        0        0    28454 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/managers/roi_manager.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/__init__.py
--rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/ioxml.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/utils.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/gant_chart.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/image_viewer.py
--rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/navigator.py
--rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/scan_selector.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/widgets.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/__init__.py
--rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer.py
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer0D.py
--rw-r--r--   0        0        0    19969 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer1D.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py
--rw-r--r--   0        0        0    41922 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer2D.py
--rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py
--rw-r--r--   0        0        0    34930 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewerND.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/items/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/items/axis_scaled.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/items/crosshair.py
--rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/items/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/axes_viewer.py
--rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/filter.py
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/lineout.py
--rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/plot_utils.py
--rw-r--r--   0        0        0    44892 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/signalND.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/__init__.py
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/scan_factory.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/scanner.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/utils.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/_1d_scanners.py
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/_2d_scanners.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/__init__.py
--rw-r--r--   0        0        0     7646 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/sequential.py
--rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/tabular.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/svg/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/svg/svg_renderer.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/svg/svg_view.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/svg/svg_viewer2D.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/tree_layout/__init__.py
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 pymodaq-4.0.1/src/pymodaq/utils/tree_layout/tree_layout_main.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pymodaq-4.0.1/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pymodaq-4.0.1/LICENSE
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 pymodaq-4.0.1/README.rst
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 pymodaq-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 pymodaq-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/__init__.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/daq_utils.py
+-rw-r--r--   0        0        0    61748 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/dashboard.py
+-rw-r--r--   0        0        0    74359 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/icon.ico
+-rw-r--r--   0        0        0    53114 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/splash.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/__init__.py
+-rw-r--r--   0        0        0    41489 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/daq_move.py
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/daq_move_ui.py
+-rw-r--r--   0        0        0    64322 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/daq_viewer.py
+-rw-r--r--   0        0        0    15462 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/daq_viewer_ui.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/mocks.py
+-rw-r--r--   0        0        0    30500 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/move_utility_classes.py
+-rw-r--r--   0        0        0     8250 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/utils.py
+-rw-r--r--   0        0        0    26665 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/viewer_utility_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/__init__.py
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/custom_app.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/custom_viewer.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/function_plotter.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/nonlinearscanner.py
+-rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/parameter_ex.py
+-rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/preset_MockCamera.xml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.aliases
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvlps
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj
+-rw-r--r--   0        0        0    69358 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi
+-rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi
+-rw-r--r--   0        0        0    29785 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi
+-rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi
+-rw-r--r--   0        0        0    19039 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi
+-rw-r--r--   0        0        0    19791 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/console.py
+-rw-r--r--   0        0        0    19346 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/daq_logger.py
+-rw-r--r--   0        0        0    56107 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/daq_scan.py
+-rw-r--r--   0        0        0    10123 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/daq_scan_ui.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/h5browser.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/utils.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/pid/__init__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/pid/daq_move_PID.py
+-rw-r--r--   0        0        0    29797 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/pid/pid_controller.py
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/pid/utils.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/__init__.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/load_and_plot.py
+-rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/process_to_scalar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_analysis/__init__.py
+-rw-r--r--   0        0        0    24346 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_analysis/daq_analysis_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/__init__.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui
+-rw-r--r--   0        0        0    17093 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/process_from_QtDesigner_DAQ_Measurement_GUI.bat
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/VERSION
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/__init__.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/config_template.toml
+-rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/preset_default.xml
+-rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/triangulation_data.npy
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.bat
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc
+-rw-r--r--   0        0        0  8225442 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/__init__.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/icons.svg
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/1d.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/2d.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/3d.png
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add2.png
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve.png
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve_All.png
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png
+-rw-r--r--   0        0        0    47401 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnGroup.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnNum.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnText.png
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnTime.png
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnWave.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Close3.png
+-rw-r--r--   0        0        0    47830 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png
+-rw-r--r--   0        0        0    48054 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png
+-rw-r--r--   0        0        0    48959 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Contract.png
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Create.png
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png
+-rw-r--r--   0        0        0    49034 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png
+-rw-r--r--   0        0        0    48413 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ErrorMessage.png
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png
+-rw-r--r--   0        0        0    48491 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Expand.png
+-rw-r--r--   0        0        0    47692 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png
+-rw-r--r--   0        0        0    48102 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/FFT.png
+-rw-r--r--   0        0        0    89487 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Histogram.png
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/LUT_LookUpTable.png
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Marker.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Math.png
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png
+-rw-r--r--   0        0        0    48221 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png
+-rw-r--r--   0        0        0    47229 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png
+-rw-r--r--   0        0        0    47258 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Multiply.png
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png
+-rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_File.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_Folder.png
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File.png
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png
+-rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope_16.png
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Pass.png
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RGB.png
+-rw-r--r--   0        0        0    47228 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png
+-rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh2.png
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Region.png
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rendezvous.png
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SELECT.png
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save.png
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll.png
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png
+-rw-r--r--   0        0        0    49529 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Search.png
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png
+-rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png
+-rw-r--r--   0        0        0    49414 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png
+-rw-r--r--   0        0        0    49581 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png
+-rw-r--r--   0        0        0    52734 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Spreadsheet.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics.png
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics2.png
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Status.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Subtract.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Vision.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Volts.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Wait2.png
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_1_1.png
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_in.png
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_out.png
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_to_Selection.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/abort.png
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/advanced2.png
+-rw-r--r--   0        0        0    47292 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/b_icon.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/back.png
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/bg_icon.png
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera.png
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cartesian.png
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/close2.png
+-rw-r--r--   0        0        0    47742 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color.png
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color2.png
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/continuous.png
+-rw-r--r--   0        0        0    47210 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download.png
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download2.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/error2.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ethernet.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/fan.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/filter2.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/g_icon.png
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to.png
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grab.png
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/graph.png
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grey_icon.png
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greyscale.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1.png
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1_32.png
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/home2.png
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/integrator.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/joystick.png
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/limiter.png
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png
+-rw-r--r--   0        0        0    50113 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png
+-rw-r--r--   0        0        0    47361 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_straight_line.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/movie.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multi_point.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multiplexer.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/new.png
+-rw-r--r--   0        0        0    48254 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png
+-rw-r--r--   0        0        0    49028 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png
+-rw-r--r--   0        0        0    48669 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/overlay.png
+-rw-r--r--   0        0        0    24121 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pause.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/permute.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/phase.png
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/play.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/polar.png
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pole_zero.png
+-rw-r--r--   0        0        0    47612 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/properties.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/r_icon.png
+-rw-r--r--   0        0        0    47081 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/read2.png
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/remove.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/reset.png
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rgb_icon.png
+-rw-r--r--   0        0        0    49951 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png
+-rw-r--r--   0        0        0    47140 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run2.png
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saturation.png
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_horizontally.png
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_vertically.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/search2.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select2.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all.png
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_none.png
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence2.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/snap.png
+-rw-r--r--   0        0        0    47434 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/start.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/status_cancelled.png
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop.png
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop3.png
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sum.png
+-rw-r--r--   0        0        0    50597 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/tree.png
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/vector.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/verify.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/video.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/wait.png
+-rw-r--r--   0        0        0    50127 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/watershed.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomAuto.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomReset.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/__init__.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/array_manipulation.py
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/calibration_camera.py
+-rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/chrono_timer.py
+-rw-r--r--   0        0        0    15404 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/config.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/conftests.py
+-rw-r--r--   0        0        0    26941 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/daq_utils.py
+-rw-r--r--   0        0        0    69686 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/data.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/enums.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/exceptions.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/factory.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/logger.py
+-rw-r--r--   0        0        0    17513 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/math_utils.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/messenger.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/qvariant.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/slicing.py
+-rw-r--r--   0        0        0    39074 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/tcp_server_client.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/units.py
+-rw-r--r--   0        0        0   418388 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.odt
+-rw-r--r--   0        0        0   361273 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.pdf
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/script_full_setup.iss
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/abstract/__init__.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/abstract/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/db/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/__init__.py
+-rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/db_logger.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/db_logger_models.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/__init__.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/custom_app.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/dock.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/file_io.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/layout.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/list_picker.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/utils.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/label.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/lcd.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/push.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/qled.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/spinbox.py
+-rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/table.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/__init__.py
+-rw-r--r--   0        0        0    32012 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/backends.py
+-rw-r--r--   0        0        0    22457 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/browsing.py
+-rw-r--r--   0        0        0    31654 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/data_saving.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporter.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/h5logging.py
+-rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/module_saving.py
+-rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/saving.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/__init__.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/base.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/flimj.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/hyperspy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/__init__.py
+-rw-r--r--   0        0        0    16788 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/action_manager.py
+-rw-r--r--   0        0        0    13905 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/batchscan_manager.py
+-rw-r--r--   0        0        0    20283 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/modules_manager.py
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/overshoot_manager.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/parameter_manager.py
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/preset_manager.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/preset_manager_utils.py
+-rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/remote_manager.py
+-rw-r--r--   0        0        0    28454 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/roi_manager.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/__init__.py
+-rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/ioxml.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/utils.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/__init__.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/gant_chart.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/image_viewer.py
+-rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/navigator.py
+-rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/scan_selector.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/widgets.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/__init__.py
+-rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer.py
+-rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer0D.py
+-rw-r--r--   0        0        0    19969 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer1D.py
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py
+-rw-r--r--   0        0        0    41922 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer2D.py
+-rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py
+-rw-r--r--   0        0        0    34930 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewerND.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/items/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/items/axis_scaled.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/items/crosshair.py
+-rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/items/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/axes_viewer.py
+-rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/filter.py
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/lineout.py
+-rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/plot_utils.py
+-rw-r--r--   0        0        0    44892 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/signalND.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/__init__.py
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scan_factory.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanner.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/utils.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/_1d_scanners.py
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/_2d_scanners.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/__init__.py
+-rw-r--r--   0        0        0     7646 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/sequential.py
+-rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/tabular.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/svg/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/svg/svg_renderer.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/svg/svg_view.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/svg/svg_viewer2D.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/tree_layout/__init__.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/tree_layout/tree_layout_main.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pymodaq-4.0.2/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pymodaq-4.0.2/LICENSE
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pymodaq-4.0.2/README.rst
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 pymodaq-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 pymodaq-4.0.2/PKG-INFO
```

### Comparing `pymodaq-4.0.1/src/pymodaq/__init__.py` & `pymodaq-4.0.2/src/pymodaq/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/daq_utils.py` & `pymodaq-4.0.2/src/pymodaq/daq_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/dashboard.py` & `pymodaq-4.0.2/src/pymodaq/dashboard.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/icon.ico` & `pymodaq-4.0.2/src/pymodaq/icon.ico`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/splash.png` & `pymodaq-4.0.2/src/pymodaq/splash.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/control_modules/daq_move.py` & `pymodaq-4.0.2/src/pymodaq/control_modules/daq_move.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Created the 29/07/2022
 
 @author: Sebastien Weber
 """
+
+from __future__ import annotations
+
 import sys
+from typing import List, Tuple, Union
+import numpy as np
 
 from qtpy.QtCore import QObject, Signal, QThread, Slot, Qt, QTimer
 from qtpy import QtWidgets
 
 from easydict import EasyDict as edict
 
 from pymodaq.utils.logger import set_logger, get_module_name, get_module_name
@@ -22,14 +27,16 @@
 from pymodaq.utils import daq_utils as utils
 from pymodaq.utils.parameter import utils as putils
 from pymodaq.utils.gui_utils import get_splash_sc
 from pymodaq.utils import config
 from pymodaq.utils.exceptions import ActuatorError
 from pymodaq.utils.messenger import deprecation_msg
 from pymodaq.utils.h5modules import module_saving
+from pymodaq.utils.data import DataRaw, DataFromPlugins, DataToExport, Axis, DataDistribution
+from pymodaq.utils.h5modules.backends import Node
 
 
 local_path = config.get_set_local_dir()
 sys.path.append(local_path)
 logger = set_logger(get_module_name(__file__))
 DAQ_Move_Actuators = utils.get_plugins('daq_move')
 ACTUATOR_TYPES = [mov['name'] for mov in DAQ_Move_Actuators]
@@ -55,15 +62,15 @@
     See Also
     --------
     :class:`ControlModule`, :class:`ParameterManager`
     """
     settings_name = 'daq_move_settings'
 
     move_done_signal = Signal(str, float)
-    _current_value_signal = Signal(str, float)
+    current_value_signal = Signal(str, float)
     # to be used in external program to make sure the move has been done,
     # export the current position. str refer to the unique title given to the module
     _update_settings_signal = Signal(edict)
     bounds_signal = Signal(bool)
 
     
     params = daq_move_params
@@ -152,14 +159,52 @@
         elif cmd.command == 'show_log':
             self.show_log()
         elif cmd.command == 'actuator_changed':
             self.actuator = cmd.attribute
         elif cmd.command == 'rel_value':
             self._relative_value = cmd.attribute
 
+    def append_data(self, data: DataToExport = None, where: Union[Node, str] = None):
+        """Appends current DataToExport to an ActuatorEnlargeableSaver
+
+        Parameters
+        ----------
+        data
+        where: Node or str
+        See Also
+        --------
+        ActuatorEnlargeableSaver
+        """
+        if data is None:
+            data = DataToExport(name=self.title, data=[DataRaw(name=self.title, dim='Data0D',
+                                                               data=[np.array([self._current_value])])])
+        self._add_data_to_saver(data, where=where)
+        # todo: test this for logging
+
+    def _add_data_to_saver(self, data: DataToExport, where=None, **kwargs):
+        """Adds DataToExport data to the current node using the declared module_and_data_saver
+
+        Filters the data to be saved by DataSource as specified in the current H5Saver (see self.module_and_data_saver)
+
+        Parameters
+        ----------
+        data: DataToExport
+            The data to be saved
+        kwargs: dict
+            Other named parameters to be passed as is to the module_and_data_saver
+
+        See Also
+        --------
+        DetectorSaver, DetectorEnlargeableSaver, DetectorExtendedSaver
+
+        """
+        #todo: test this for logging
+
+        node = self.module_and_data_saver.get_set_node(where)
+        self.module_and_data_saver.add_data(node, data, **kwargs)
 
     def stop_motion(self):
         """Stop any motion
         """
         try:
             self.command_hardware.emit(ThreadCommand(command="stop_motion"))
         except Exception as e:
@@ -459,15 +504,15 @@
             self._initialized_state = False
             self.init_signal.emit(self._initialized_state)
 
         elif status.command == "get_actuator_value" or status.command == 'check_position':
             if self.ui is not None:
                 self.ui.display_value(status.attribute[0])
             self._current_value = status.attribute[0]
-            self._current_value_signal.emit(self.title, self._current_value)
+            self.current_value_signal.emit(self.title, self._current_value)
             if self.settings.child('main_settings', 'tcpip', 'tcp_connected').value() and self._send_to_tcpip:
                 self._command_tcpip.emit(ThreadCommand('position_is', status.attribute))
 
         elif status.command == "move_done":
             if self.ui is not None:
                 self.ui.display_value(status.attribute[0])
                 self.ui.move_done = True
@@ -555,24 +600,24 @@
             self.command_hardware.emit(ThreadCommand(command="get_actuator_value"))
 
         except Exception as e:
             self.logger.exception(str(e))
 
     def grab(self):
         if self.ui is not None:
-            self.manage_ui_actions('refresh_value', 'setChecked', 'False')
+            self.manage_ui_actions('refresh_value', 'setChecked', False)
         self.get_continuous_actuator_value(False)
 
     def stop_grab(self):
         """Stop value polling. Mandatory
 
         First uncheck the ui action if ui is not None, then stop the polling
         """
         if self.ui is not None:
-            self.manage_ui_actions('refresh_value', 'setChecked', 'False')
+            self.manage_ui_actions('refresh_value', 'setChecked', False)
         self.get_continuous_actuator_value(False)
 
     def get_continuous_actuator_value(self, get_value=True):
         """Start the continuous getting of the actuator's value
 
         Parameters
         ----------
```

### Comparing `pymodaq-4.0.1/src/pymodaq/control_modules/daq_move_ui.py` & `pymodaq-4.0.2/src/pymodaq/control_modules/daq_move_ui.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/control_modules/daq_viewer.py` & `pymodaq-4.0.2/src/pymodaq/control_modules/daq_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jan 10 16:54:14 2018
 
 @author: Weber Sébastien
 """
-
+from __future__ import annotations
 from collections import OrderedDict
 import copy
 import datetime
 import os
 from pathlib import Path
 import sys
 from typing import List, Tuple, Union
@@ -27,14 +27,15 @@
 import pymodaq.utils.scanner
 from pymodaq.utils.tcp_server_client import TCPClient
 from pymodaq.utils.gui_utils.widgets.lcd import LCD
 from pymodaq.utils.config import Config, get_set_local_dir
 from pymodaq.utils.h5modules.browsing import browse_data
 from pymodaq.utils.h5modules.saving import H5Saver
 from pymodaq.utils.h5modules import module_saving
+from pymodaq.utils.h5modules.backends import Node
 from pymodaq.utils.daq_utils import ThreadCommand
 from pymodaq.utils.parameter import ioxml
 from pymodaq.utils.parameter import utils as putils
 from pymodaq.control_modules.viewer_utility_classes import params as daq_viewer_params
 from pymodaq.utils import daq_utils as utils
 from pymodaq.utils.messenger import deprecation_msg
 from pymodaq.utils.gui_utils import DockArea, get_splash_sc, Dock
@@ -569,31 +570,34 @@
             self.grab_done_signal.disconnect(self.append_data)
 
             try:
                 self._h5saver_continuous.close()
             except Exception as e:
                 self.logger.exception(str(e))
 
-    def append_data(self, where=None):
-        """Appends DataToExport to a DetectorEnlargeableSaver
+    def append_data(self, data: DataToExport = None, where: Union[Node, str] = None):
+        """Appends current DataToExport to a DetectorEnlargeableSaver
 
         Parameters
         ----------
         data: DataToExport
-            The data to be added to an enlargeable h5 array
-
+            not really used
+        where: Node or str
         See Also
         --------
         DetectorEnlargeableSaver
         """
-        self._add_data_to_saver(self._data_to_save_export, init_step=self._h5saver_continuous.settings['N_saved'] == 0,
-                                where=None)
+        if data is None:
+            data = self._data_to_save_export
+        self._add_data_to_saver(data, init_step=self._h5saver_continuous.settings['N_saved'] == 0,
+                                where=where)
         self._h5saver_continuous.settings.child('N_saved').setValue(self._h5saver_continuous.settings['N_saved'] + 1)
 
-    def insert_data(self, indexes: Tuple[int], where=None, distribution=DataDistribution['uniform']):
+    def insert_data(self, indexes: Tuple[int], where: Union[Node, str] = None,
+                    distribution=DataDistribution['uniform']):
         """Insert DataToExport to a DetectorExtendedSaver at specified indexes
 
         Parameters
         ----------
         indexes: tuple(int)
             The indexes within the extended array where to place these data
         where: Node or str
```

### Comparing `pymodaq-4.0.1/src/pymodaq/control_modules/daq_viewer_ui.py` & `pymodaq-4.0.2/src/pymodaq/control_modules/daq_viewer_ui.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/control_modules/mocks.py` & `pymodaq-4.0.2/src/pymodaq/control_modules/mocks.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/control_modules/move_utility_classes.py` & `pymodaq-4.0.2/src/pymodaq/control_modules/move_utility_classes.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/control_modules/utils.py` & `pymodaq-4.0.2/src/pymodaq/control_modules/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,14 +133,23 @@
         """Programmatic entry to grab data from detectors or current value from actuator"""
         raise NotImplementedError
 
     def stop_grab(self):
         """Programmatic entry to stop data grabbing from detectors or current value polling from actuator"""
         raise NotImplementedError
 
+    def _add_data_to_saver(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def append_data(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def insert_data(self, *args, **kwargs):
+        raise NotImplementedError
+
     def quit_fun(self):
         """Programmatic entry to quit the controle module"""
         raise NotImplementedError
 
     def init_hardware(self, do_init=True):
         """Programmatic entry to initialize/deinitialize the control module
```

### Comparing `pymodaq-4.0.1/src/pymodaq/control_modules/viewer_utility_classes.py` & `pymodaq-4.0.2/src/pymodaq/control_modules/viewer_utility_classes.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/custom_app.py` & `pymodaq-4.0.2/src/pymodaq/examples/custom_app.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/custom_viewer.py` & `pymodaq-4.0.2/src/pymodaq/examples/custom_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/function_plotter.py` & `pymodaq-4.0.2/src/pymodaq/examples/function_plotter.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/nonlinearscanner.py` & `pymodaq-4.0.2/src/pymodaq/examples/nonlinearscanner.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/parameter_ex.py` & `pymodaq-4.0.2/src/pymodaq/examples/parameter_ex.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/preset_MockCamera.xml` & `pymodaq-4.0.2/src/pymodaq/examples/preset_MockCamera.xml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl` & `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/console.py` & `pymodaq-4.0.2/src/pymodaq/extensions/console.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/daq_logger.py` & `pymodaq-4.0.2/src/pymodaq/extensions/daq_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
     def set_logger(self, logger_interface):
         if self.logger is not None:
             self.logger.close()
             self.docks['logger_settings'].removeWidgets()
 
         if logger_interface == 'H5 File':
-            self.logger = H5Logger()
+            self.logger = H5Logger(self.modules_manager)
         elif logger_interface == 'SQL DataBase':
             self.logger = DataBaseLogger(self.dashboard.preset_file.stem)
         else:
             return
 
         self.docks['logger_settings'].addWidget(self.logger.settings_tree)
 
@@ -430,18 +430,16 @@
         """
         try:
             self.data_logger.add_data(data)
         except Exception as e:
             logger.exception(str(e))
 
     def format_actuators_data(self, act_name, act_value):
-        acq_time = datetime.datetime.now().timestamp()
-        data = OrderedDict(name=act_name, acq_time_s=acq_time, control_module='DAQ_Move',
-                           data0D=OrderedDict(data=data_mod.DataToExport(name=act_name, dim='Data0D', source='raw',
-                                                                           data=np.array([act_value]))))
+        data = data_mod.DataToExport(name=act_name, data=[data_mod.DataRaw(name=act_name, dim='Data0D',
+                                                                           data=[np.array([act_value])])])
         self.do_save_continuous(data)
 
     def connect_actuators(self, connect=True):
         """Connect actuators to DAQ_Logging do_save_continuous method
 
         Parameters
         ----------
```

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/daq_scan.py` & `pymodaq-4.0.2/src/pymodaq/extensions/daq_scan.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/daq_scan_ui.py` & `pymodaq-4.0.2/src/pymodaq/extensions/daq_scan_ui.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/h5browser.py` & `pymodaq-4.0.2/src/pymodaq/extensions/h5browser.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/utils.py` & `pymodaq-4.0.2/src/pymodaq/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/pid/__init__.py` & `pymodaq-4.0.2/src/pymodaq/extensions/pid/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/pid/daq_move_PID.py` & `pymodaq-4.0.2/src/pymodaq/extensions/pid/daq_move_PID.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/pid/pid_controller.py` & `pymodaq-4.0.2/src/pymodaq/extensions/pid/pid_controller.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/extensions/pid/utils.py` & `pymodaq-4.0.2/src/pymodaq/extensions/pid/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/post_treatment/load_and_plot.py` & `pymodaq-4.0.2/src/pymodaq/post_treatment/load_and_plot.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/post_treatment/process_to_scalar.py` & `pymodaq-4.0.2/src/pymodaq/post_treatment/process_to_scalar.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/post_treatment/daq_analysis/daq_analysis_main.py` & `pymodaq-4.0.2/src/pymodaq/post_treatment/daq_analysis/daq_analysis_main.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py` & `pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui` & `pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py` & `pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/config_template.toml` & `pymodaq-4.0.2/src/pymodaq/resources/config_template.toml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/preset_default.xml` & `pymodaq-4.0.2/src/pymodaq/resources/preset_default.xml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/triangulation_data.npy` & `pymodaq-4.0.2/src/pymodaq/resources/triangulation_data.npy`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/icons.svg` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/icons.svg`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png` & `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/array_manipulation.py` & `pymodaq-4.0.2/src/pymodaq/utils/array_manipulation.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/calibration_camera.py` & `pymodaq-4.0.2/src/pymodaq/utils/calibration_camera.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/chrono_timer.py` & `pymodaq-4.0.2/src/pymodaq/utils/chrono_timer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/config.py` & `pymodaq-4.0.2/src/pymodaq/utils/config.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/daq_utils.py` & `pymodaq-4.0.2/src/pymodaq/utils/daq_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/data.py` & `pymodaq-4.0.2/src/pymodaq/utils/data.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/enums.py` & `pymodaq-4.0.2/src/pymodaq/utils/enums.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/exceptions.py` & `pymodaq-4.0.2/src/pymodaq/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/factory.py` & `pymodaq-4.0.2/src/pymodaq/utils/factory.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/logger.py` & `pymodaq-4.0.2/src/pymodaq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/math_utils.py` & `pymodaq-4.0.2/src/pymodaq/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/messenger.py` & `pymodaq-4.0.2/src/pymodaq/utils/messenger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/slicing.py` & `pymodaq-4.0.2/src/pymodaq/utils/slicing.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/tcp_server_client.py` & `pymodaq-4.0.2/src/pymodaq/utils/tcp_server_client.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/units.py` & `pymodaq-4.0.2/src/pymodaq/utils/units.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.odt` & `pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.odt`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.pdf` & `pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.pdf`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/Tuto innosetup/script_full_setup.iss` & `pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/script_full_setup.iss`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/abstract/__init__.py` & `pymodaq-4.0.2/src/pymodaq/utils/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/abstract/logger.py` & `pymodaq-4.0.2/src/pymodaq/utils/abstract/logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/db/db_logger/db_logger.py` & `pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/db_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 import datetime
 from typing import List
 
 from pymodaq.utils.logger import set_logger, get_module_name, get_module_name
 from pymodaq.utils.config import Config
 from qtpy import QtCore
 from contextlib import contextmanager
-from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker
-from sqlalchemy_utils import database_exists, create_database
+
 from pymodaq.utils.db.db_logger.db_logger_models import Base, Data0D, Data1D, Data2D, LogInfo,\
     Configuration, ControlModule
 from pymodaq.utils import daq_utils as utils
 from pymodaq.utils.gui_utils.utils import dashboard_submodules_params
 from pymodaq.utils.messenger import messagebox, deprecation_msg
 from pymodaq.utils.abstract.logger import AbstractLogger
 from pyqtgraph.parametertree import Parameter, ParameterTree
 
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker
+from sqlalchemy_utils import database_exists, create_database
 
 logger = set_logger(get_module_name(__file__))
 config = Config()
 
 
 class DBLogHandler(logging.StreamHandler):
     def __init__(self, dblogger):
@@ -210,16 +211,14 @@
                     session.add(Data2D(timestamp=time_stamp, control_module_id=module_id,
                                        channel=f"{data['data2D'][channel]['name']}:{channel}",
                                        value=data['data2D'][channel]['data'].tolist()))
 
             # not yet dataND as db should not know where to save these datas
 
 
-
-
 class DbLoggerGUI(DbLogger, QtCore.QObject):
     params = [
         {'title': 'Database:', 'name': 'database_type', 'type': 'list', 'value': 'PostgreSQL',
             'limits': ['PostgreSQL', ]},
         {'title': 'Server IP:', 'name': 'server_ip', 'type': 'str',
             'value': config('network', 'logging', 'sql', 'ip'),
          'tip':'Either localhost if the database server is on the same computer or the IP address of the server'},
@@ -232,15 +231,15 @@
     def __init__(self, database_name):
         DbLogger.__init__(self, database_name, ip_address=config('network', 'logging', 'sql', 'ip'),
                           port=config('network', 'logging', 'sql', 'port'), save2D=False)
         QtCore.QObject.__init__(self)
 
         self.settings = Parameter.create(title='DB settings', name='db_settings', type='group',
                                          children=self.params)
-        self.settings.child(('do_save')).hide()
+        self.settings.child('do_save').hide()
         self.settings_tree = ParameterTree()
         self.settings_tree.setMinimumHeight(310)
         self.settings_tree.setParameters(self.settings, showTop=False)
         self.settings.sigTreeStateChanged.connect(self.parameter_tree_changed)
 
     def parameter_tree_changed(self, param, changes):
         """
```

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/db/db_logger/db_logger_models.py` & `pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/db_logger_models.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/custom_app.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/custom_app.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/dock.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/dock.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/file_io.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/file_io.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/layout.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/layout.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/list_picker.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/list_picker.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/utils.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/label.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/label.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/lcd.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/lcd.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/push.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/push.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/qled.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/qled.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/spinbox.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/gui_utils/widgets/table.py` & `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/table.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/h5modules/backends.py` & `pymodaq-4.0.2/src/pymodaq/utils/h5modules/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,24 +53,26 @@
 
 
 class SaveType(BaseEnum):
     scan = 0
     detector = 1
     logger = 2
     custom = 3
+    actuator = 4
 
 
 class GroupType(BaseEnum):
     detector = 0
     actuator = 1
     data = 2
     ch = 3
     scan = 4
     external_h5 = 5
     data_dim = 6
+    data_logger = 7
 
 
 class InvalidExport(Exception):
     pass
 
 
 def check_mandatory_attrs(attr_name, attr):
@@ -186,14 +188,26 @@
             p = self.node._v_parent
         else:
             p = self.node.parent
         klass = get_attr(p, 'CLASS', self.backend)
         _cls = getattr(mod, klass)
         return _cls(p, self.backend)
 
+    @property
+    def h5file(self):
+        if self.backend == 'tables':
+            return self.node._v_file
+        else:
+            return self.node.file
+
+    def to_h5_backend(self) -> 'H5Backend':
+        h5_backend = H5Backend(self.backend)
+        h5_backend.h5file = self.h5file
+        return h5_backend
+
     def set_attr(self, key, value):
         self.attrs[key] = value
 
     def get_attr(self, item):
         return self.attrs[item]
 
     @property
@@ -255,16 +269,14 @@
             '%r (%s)' % (childname, child.__class__.__name__)
             for (childname, child) in self.children().items()
         ]
         childlist = '[%s]' % (', '.join(rep))
 
         return "%s\n  children := %s" % (str(self), childlist)
 
-
-
     def children(self) -> Dict[str, Node]:
         """Get a dict containing all children node hanging from self whith their name as keys
 
         Returns
         -------
         dict: keys are children node names, values are the children nodes
 
@@ -944,15 +956,15 @@
             array.array.attrs['EXTDIM'] = 0
         array.attrs['shape'] = (0,)
         array.attrs['dtype'] = dtype.name
         array.attrs['subdtype'] = subdtype
         array.attrs['backend'] = self.backend
         return array
 
-    def add_group(self, group_name, group_type, where, title='', metadata=dict([])) -> GROUP:
+    def add_group(self, group_name, group_type: GroupType, where, title='', metadata=dict([])) -> GROUP:
         """
         Add a node in the h5 file tree of the group type
         Parameters
         ----------
         group_name: (str) a custom name for this group
         group_type: str or GroupType enum
             one of the possible values of GroupType
```

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/h5modules/browsing.py` & `pymodaq-4.0.2/src/pymodaq/utils/h5modules/browsing.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 from pymodaq.utils import daq_utils as utils
 from pymodaq.utils.managers.action_manager import ActionManager
 from pymodaq.utils.managers.parameter_manager import ParameterManager
 from pymodaq.utils.messenger import messagebox
 from .backends import H5Backend
 from .saving import H5Saver
 from . import data_saving
-from .utils import find_scan_node
+from .utils import find_scan_node, get_h5_attributes
+from .exporter import ExporterFactory
 
 config = Config()
 logger = set_logger(get_module_name(__file__))
 
 
 class H5BrowserUtil(H5Backend):
     """Utility object to interact and get info and data from a hdf5 file
@@ -51,78 +52,26 @@
     ----------
     backend: str
         The used hdf5 backend: either tables, h5py or h5pyd
     """
     def __init__(self, backend='tables'):
         super().__init__(backend=backend)
 
-    def export_data(self, node_path='/', filesavename='datafile.h5'):
-        """Export data in nodes in another file format
+    def export_data(self, node_path='/', filesavename: str = 'datafile.h5'):
+        """Initialize the correct exporter and export the node"""
 
-        Parameters
-        ----------
-        node_path: str
-            the path in the file
-        filesavename:
-            the exported file name with a particular extension
-            Accepted extensions are:
-            * txt: to save node content in a tab delimited text file
-            * ascii: to save node content in a tab delimited ascii file
-            * h5
-        """
-        if filesavename != '':
-            file = Path(filesavename)
-            node = self.get_node(node_path)
-            if file.suffix == '.txt' or file.suffix == '.ascii':
-                if 'ARRAY' in node.attrs['CLASS']:
-                    data = node.read()
-                    if not isinstance(data, np.ndarray):
-                        # in case one has a list of same objects (array of strings for instance, logger or other)
-                        data = np.array(data)
-                        np.savetxt(filesavename,
-                                   data if file.suffix == '.txt' else data.T if len(data.shape) > 1 else [data],
-                                   '%s', '\t')
-                    else:
-                        np.savetxt(filesavename,
-                                   data if file.suffix == '.txt' else data.T if len(data.shape) > 1 else [data],
-                                   '%.6e', '\t')
-
-                elif 'GROUP' in node.attrs['CLASS']:
-                    data_tot = []
-                    header = []
-                    dtypes = []
-                    fmts = []
-                    for subnode_name, subnode in node.children().items():
-                        if 'ARRAY' in subnode.attrs['CLASS']:
-                            if len(subnode.attrs['shape']) == 1:
-                                data = subnode.read()
-                                if not isinstance(data, np.ndarray):
-                                    # in case one has a list of same objects (array of strings for instance, logger or other)
-                                    data = np.array(data)
-                                data_tot.append(data)
-                                dtypes.append((subnode_name, data.dtype))
-                                header.append(subnode_name)
-                                if data.dtype.char == 'U':
-                                    fmt = '%s'  # for strings
-                                elif data.dtype.char == 'l':
-                                    fmt = '%d'  # for integers
-                                else:
-                                    fmt = '%.6f'  # for decimal numbers
-                                fmts.append(fmt)
-
-                    data_trans = np.array(list(zip(*data_tot)), dtype=dtypes)
-                    np.savetxt(filesavename, data_trans, fmts, '\t', header='#' + '\t'.join(header))
-            elif file.suffix == '.h5':
-                self.save_file_as(str(file))
-                copied_file = H5Backend()
-                copied_file.open_file(str(file), 'a')
-
-                copied_file.h5file.move_node(self.get_node_path(node), newparent=copied_file.h5file.get_node('/'))
-                copied_file.h5file.remove_node('/Raw_datas', recursive=True)
-                copied_file.close_file()
+        # Format the node and file type
+        filepath = Path(filesavename)
+        node = self.get_node(node_path)
+        # Separate dot from extension
+        extension = filepath.suffix[1:]
+        # Obtain the suitable exporter object
+        exporter = ExporterFactory.create_exporter(extension)
+        # Export the data
+        exporter.export_data(node, filepath)
 
     def get_h5file_scans(self, where='/'):
         """Get the list of the scan nodes in the file
 
         Parameters
         ----------
         where: str
@@ -140,55 +89,17 @@
             if 'pixmap2D' in node.attrs:
                 scan_list.append(
                     dict(scan_name='{:s}_{:s}'.format(node.parent_node.name, node.name), path=node.path,
                          data=node.attrs['pixmap2D']))
 
         return scan_list
 
-    def get_h5_attributes(self, node_path):
-        """Get the list of attributes (metadata) of a given node
-
-        Parameters
-        ----------
-        node_path: str
-            the path in the file
-
-        Returns
-        -------
-        attr_dict: OrderedDict
-            attributes as a dict
-        settings: str
-            settings attribute
-        scan_settings: str
-            scan settings attribute
-        pixmaps: list of pixmap
-        """
-        node = self.get_node(node_path)
-        attrs_names = node.attrs.attrs_name
-        attr_dict = OrderedDict([])
-        for attr in attrs_names:
-            # if attr!='settings':
-            attr_dict[attr] = node.attrs[attr]
-
-        settings = None
-        scan_settings = None
-        if 'settings' in attrs_names:
-            if node.attrs['settings'] != '':
-                settings = node.attrs['settings']
-
-        if 'scan_settings' in attrs_names:
-            if node.attrs['scan_settings'] != '':
-                scan_settings = node.attrs['scan_settings']
-        pixmaps = []
-        for attr in attrs_names:
-            if 'pixmap' in attr:
-                pixmaps.append(node.attrs[attr])
-
-        return attr_dict, settings, scan_settings, pixmaps
-
+    @staticmethod
+    def get_h5_attributes(node_path):
+        return get_h5_attributes(node_path)
 
 class View(QObject):
     item_clicked_sig = Signal(object)
     item_double_clicked_sig = Signal(object)
     
     def __init__(self, widget: QtWidgets.QWidget, settings_tree, settings_attributes_tree):
         super().__init__()
@@ -470,15 +381,15 @@
         """Opens a dialog to export data
 
         See Also
         --------
         H5BrowserUtil.export_data
         """
         try:
-            file_filter = "Single node h5 file (*.h5);;Text files (*.txt);;Ascii file (*.ascii)"
+            file_filter = ExporterFactory.get_file_filters()
             file = select_file(save=True, filter=file_filter)
             self.current_node_path = self.get_tree_node_path()
             if file != '':
                 self.h5utils.export_data(self.current_node_path, str(file))
 
         except Exception as e:
             logger.exception(str(e))
```

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/h5modules/data_saving.py` & `pymodaq-4.0.2/src/pymodaq/utils/h5modules/data_saving.py`

 * *Files 2% similar despite different names*

```diff
@@ -681,15 +681,15 @@
     -----
     This object is made for continuous saving mode of DAQViewer and logging to h5file for DAQLogger
     """
     def __init__(self, h5saver: H5Saver):
         super().__init__(h5saver, 'time', 's')
 
     def add_data(self, where: Union[Node, str], data: DataToExport, settings_as_xml='', metadata={}):
-        super().add_data(where, data, axis_value=time(), settings_as_xml=settings_as_xml, metadata=metadata)
+        super().add_data(where, data, axis_value=data.timestamp, settings_as_xml=settings_as_xml, metadata=metadata)
 
 
 class DataToExportExtendedSaver(DataToExportSaver):
     """Object to save DataToExport at given indexes within arrays including extended shape
 
     Mostly used for data generated from the DAQScan
 
@@ -744,14 +744,17 @@
                 dwa_group = self._h5saver.get_set_group(dim_group, self.channel_formatter(ind), dwa.name)
                 self._data_saver.add_data(dwa_group, dwa, indexes=indexes, distribution=distribution)
 
 
 class DataLoader:
     """Specialized Object to load DataWithAxes object from a h5file
 
+    On the contrary to DataSaverLoader, does include navigation axes stored elsewhere in the h5file
+    (for instance if saved from the DAQ_Scan)
+
     Parameters
     ----------
     h5saver: H5Saver
     """
 
     def __init__(self, h5saver: H5Saver):
         self._axis_loader: AxisSaverLoader = None
```

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/h5modules/module_saving.py` & `pymodaq-4.0.2/src/pymodaq/utils/h5modules/module_saving.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .data_saving import DataToExportSaver, AxisSaverLoader, DataToExportTimedSaver, DataToExportExtendedSaver
 from pymodaq.utils.parameter import ioxml
 
 if TYPE_CHECKING:
     from pymodaq.extensions.daq_scan import DAQScan
     from pymodaq.control_modules.daq_viewer import DAQ_Viewer
     from pymodaq.control_modules.daq_move import DAQ_Move
+    from pymodaq.utils.h5modules.h5logging import H5Logger
 
 
 class ModuleSaver(metaclass=ABCMeta):
     """Abstract base class to save info and data from main modules (DAQScan, DAQViewer, DAQMove, ...)"""
     group_type: GroupType = abstract_attribute()
     _module = abstract_attribute()
     _h5saver: H5SaverLowLevel = abstract_attribute()
@@ -240,46 +241,49 @@
     ----------
     h5saver
     module
     """
     group_type = GroupType['actuator']
 
     def __init__(self, module: DAQ_Move):
-        self._axis_saver = None
+        self._datatoexport_saver: DataToExportTimedSaver = None
         self._module_group: GROUP = None
         self._module: DAQ_Move = module
         self._h5saver = None
 
-    def update_after_h5changed(self):
-        self._axis_saver = AxisSaverLoader(self.h5saver)
+    def update_after_h5changed(self, ):
+        self._datatoexport_saver = DataToExportTimedSaver(self.h5saver)
 
     def _add_module(self, where: Union[Node, str] = None, metadata={}):
         if where is None:
             where = self._h5saver.raw_group
 
         settings_xml = ET.Element('All_settings')
         settings_xml.append(ioxml.walk_parameters_to_xml(param=self._module.settings))
 
         return self._h5saver.add_act_group(where, title=self._module.title, settings_as_xml=ET.tostring(settings_xml),
                                            metadata=metadata)
 
+    def add_data(self, where: Union[Node, str], data: DataToExport):
+        self._datatoexport_saver.add_data(where, data)
+
 
 class ScanSaver(ModuleSaver):
     """Implementation of the ModuleSaver class dedicated to DAQScan module
 
     Parameters
     ----------
     h5saver
     module
     """
     group_type = GroupType['scan']
 
     def __init__(self, module):
         self._module_group: GROUP = None
-        self._module: 'DAQScan' = module
+        self._module: DAQScan = module
         self._h5saver = None
 
     def update_after_h5changed(self):
         for module in self._module.modules_manager.modules_all:
             if hasattr(module, 'module_and_data_saver'):
                 module.module_and_data_saver.h5saver = self.h5saver
 
@@ -344,7 +348,36 @@
         for detector in self._module.modules_manager.detectors:
             try:
                 detector.insert_data(indexes, where=self._module_group, distribution=distribution)
             except Exception as e:
                 pass
 
 
+class LoggerSaver(ScanSaver):
+    """Implementation of the ModuleSaver class dedicated to H5Logger module
+
+    H5Logger is the special logger to h5file of the DAQ_Logger extension
+
+    Parameters
+    ----------
+    h5saver
+    module
+    """
+    group_type = GroupType['data_logger']
+
+    def __init__(self, module):
+        self._module_group: GROUP = None
+        self._module: H5Logger = module
+        self._h5saver = None
+
+    def add_data(self):
+        for detector in self._module.modules_manager.detectors:
+            try:
+                detector.append_data(data=None, where=self._module_group)
+            except Exception as e:
+                pass
+
+        for actuator in self._module.modules_manager.actuators:
+            try:
+                actuator.append_data(data=None, where=self._module_group)
+            except Exception as e:
+                pass
```

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/h5modules/saving.py` & `pymodaq-4.0.2/src/pymodaq/utils/h5modules/saving.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,22 +379,24 @@
         -------
         add_incremental_group
         """
         group = self.add_incremental_group('detector', where, title, settings_as_xml, metadata)
         return group
 
     def add_scan_group(self, where='/RawData', title='', settings_as_xml='', metadata=dict([])):
-        """
-        Add a new group of type scan
+        """Add a new group of type scan
+
+        At creation adds the attributes description and scan_done to be used elsewhere
+
         See Also
         -------
         add_incremental_group
         """
         metadata.update(dict(description='', scan_done=False))
-        group = self.add_incremental_group('scan', where, title, settings_as_xml, metadata)
+        group = self.add_incremental_group(GroupType['scan'], where, title, settings_as_xml, metadata)
         return group
 
     def add_ch_group(self, where, title='', settings_as_xml='', metadata=dict([])):
         """
         Add a new group of type channel
         See Also
         -------
```

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/h5modules/utils.py` & `pymodaq-4.0.2/src/pymodaq/utils/h5modules/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/action_manager.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/action_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/batchscan_manager.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/batchscan_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/modules_manager.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/modules_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,16 +298,16 @@
         connect: bool
         slot: builtin_function_or_method
             method or function the chosen signal will be connected to
             if None, then the default move_done slot is used
         signal: str
             What kind of signal is to be used:
 
-            * 'move_done' will connect the `move_done signal` to the slot
-            * 'current_value' will connect the 'current_signal' to the slot
+            * 'move_done' will connect the `move_done_signal` to the slot
+            * 'current_value' will connect the 'current_value_signal' to the slot
 
         See Also
         --------
         :meth:`move_done`
         """
         if slot is None:
             slot = self.move_done
```

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/overshoot_manager.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/overshoot_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/parameter_manager.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/parameter_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/preset_manager.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/preset_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/preset_manager_utils.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/preset_manager_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/remote_manager.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/remote_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/managers/roi_manager.py` & `pymodaq-4.0.2/src/pymodaq/utils/managers/roi_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/ioxml.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/ioxml.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/utils.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py` & `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/gant_chart.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/gant_chart.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/image_viewer.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/image_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/navigator.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/navigator.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/scan_selector.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/scan_selector.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/widgets.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer0D.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer0D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer1D.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer1D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer2D.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer2D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/data_viewers/viewerND.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewerND.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/items/axis_scaled.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/items/axis_scaled.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/items/crosshair.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/items/crosshair.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/items/image.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/items/image.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/axes_viewer.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/axes_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/filter.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/lineout.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/lineout.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/plot_utils.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/plotting/utils/signalND.py` & `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/signalND.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/scanner/scan_factory.py` & `pymodaq-4.0.2/src/pymodaq/utils/scanner/scan_factory.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/scanner/scanner.py` & `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/scanner/utils.py` & `pymodaq-4.0.2/src/pymodaq/utils/scanner/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/_1d_scanners.py` & `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/_1d_scanners.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/_2d_scanners.py` & `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/_2d_scanners.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/sequential.py` & `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/sequential.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/scanner/scanners/tabular.py` & `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/tabular.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/svg/svg_view.py` & `pymodaq-4.0.2/src/pymodaq/utils/svg/svg_view.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/svg/svg_viewer2D.py` & `pymodaq-4.0.2/src/pymodaq/utils/svg/svg_viewer2D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/src/pymodaq/utils/tree_layout/tree_layout_main.py` & `pymodaq-4.0.2/src/pymodaq/utils/tree_layout/tree_layout_main.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/.gitignore` & `pymodaq-4.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/LICENSE` & `pymodaq-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/README.rst` & `pymodaq-4.0.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://codecov.io/gh/PyMoDAQ/PyMoDAQ/branch/pymodaq-dev/graph/badge.svg?token=IQNJRCQDM2
     :target: https://codecov.io/gh/PyMoDAQ/PyMoDAQ
 
-
-..  csv-table:: Tests:
-  :header: "Python", "Qt Backend", "OS", Passed
-  :widths: 15, 20, 15, 30
-
-  3.8, Qt5, Linux, |38Qt5|
-  3.9, Qt5, Linux, |39Qt5|
-  3.10, Qt5, Linux, |310Qt5|
-  3.11, Qt5, Linux, |311Qt5|
-  3.8, Qt5, Windows, |38Qt5win|
-  3.8, PySide2, Linux, |38pyside|
-  3.9, Qt6, Linux, |39Qt6|
+====== ========== ======= ======
+Python Qt Backend OS      Passed
+====== ========== ======= ======
+3.8    Qt5        Linux   |38Qt5|
+3.9    Qt5        Linux   |39Qt5|
+3.10   Qt5        Linux   |310Qt5|
+3.11   Qt5        Linux   |311Qt5|
+3.8    Qt5        Windows |38Qt5win|
+3.8    PySide2    Linux   |38pyside|
+3.9    Qt6        Linux   |39Qt6|
+====== ========== ======= ======
 
 
 .. |38Qt5| image:: https://github.com/PyMoDAQ/PyMoDAQ/actions/workflows/Testp38pyqt5.yml/badge.svg?branch=pymodaq-dev
     :target: https://github.com/PyMoDAQ/PyMoDAQ/actions/workflows/Testp38pyqt5.yml
 
 .. |39Qt5| image:: https://github.com/PyMoDAQ/PyMoDAQ/actions/workflows/Testp39pyqt5.yml/badge.svg?branch=pymodaq-dev
     :target: https://github.com/PyMoDAQ/PyMoDAQ/actions/workflows/Testp39pyqt5.yml
@@ -65,28 +64,33 @@
 It is organised a shown below:
 
 .. figure:: http://pymodaq.cnrs.fr/en/latest/_images/pymodaq_diagram.png
    :alt: overview
 
    PyMoDAQ's Dashboard and its extensions: DAQ_Scan for automated acquisitions, DAQ_Logger for data logging and many other.
 
+The main component is the **Dashboard** : This is a graphical component that will initialize actuators and detectors given
+the need of your particular experiment. You configure the dashboard using an interface for quick launch of various
+configurations (numbers and types of control modules).
+
+The detectors and the actuators are represented and manipulated using two control modules:
+
+* **DAQ_Move_module** : used to control/drive an actuator (stand alone and/or automated).
+  Any number of these modules can be instantiated in the Dashboard
+* **DAQ_Viewer_module** : used to control/drive a detector (stand alone and/or automated).
+
+Any number of these modules can be instantiated in the Dashboard.
+
+The Dashboard allows you to start dedicated extensions that will make use of the control modules:
 
-* **Dashboard_module** : This is the module that will initialize actuators and detectors given the need of your
-  particular experiment. You configure the dashboard using an interface for quick launch of various configurations.
 * **DAQ_Logger_module** : This module lets you log data from one or many detectors defined in the dashboard. You can log data
   in a binary hierarchical hdf5 file or towards a sql database
 * **DAQ_Scan_module** : This module lets you configure automated data acquisition from one or many detectors defined
   in the dashboard as a function or one or more actuators defined also in the dashboard.
 
-The detectors and the actuators are represented and manipulated using two control modules:
-
-* **DAQ_Move_module** : used to control/drive an actuator (stand alone and/or automated). Any number of these modules can be instantiated.
-* **DAQ_Viewer_module** : used to control/drive a detector (stand alone and/or automated). Any number of these modules can be instantiated.
-
 and many others to simplify any application development.
 
-
-Published under the CeCILL-B FREE SOFTWARE LICENSE
+Published under the MIT FREE SOFTWARE LICENSE
 
 GitHub repo: https://github.com/PyMoDAQ
 
 Documentation: http://pymodaq.cnrs.fr/
```

### Comparing `pymodaq-4.0.1/pyproject.toml` & `pymodaq-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.1/PKG-INFO` & `pymodaq-4.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq
-Version: 4.0.1
+Version: 4.0.2
 Summary: Modular Data Acquisition with Python
 Project-URL: Homepage, http://pymodaq.cnrs.fr
 Project-URL: Source, https://github.com/PyMoDAQ/PyMoDAQ
 Project-URL: Tracker, https://github.com/PyMoDAQ/PyMoDAQ/issues
 Author-email: Sébastien Weber <sebastien.weber@cemes.fr>
 License: The MIT License (MIT)
         
@@ -75,26 +75,25 @@
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://codecov.io/gh/PyMoDAQ/PyMoDAQ/branch/pymodaq-dev/graph/badge.svg?token=IQNJRCQDM2
     :target: https://codecov.io/gh/PyMoDAQ/PyMoDAQ
 
-
-..  csv-table:: Tests:
-  :header: "Python", "Qt Backend", "OS", Passed
-  :widths: 15, 20, 15, 30
-
-  3.8, Qt5, Linux, |38Qt5|
-  3.9, Qt5, Linux, |39Qt5|
-  3.10, Qt5, Linux, |310Qt5|
-  3.11, Qt5, Linux, |311Qt5|
-  3.8, Qt5, Windows, |38Qt5win|
-  3.8, PySide2, Linux, |38pyside|
-  3.9, Qt6, Linux, |39Qt6|
+====== ========== ======= ======
+Python Qt Backend OS      Passed
+====== ========== ======= ======
+3.8    Qt5        Linux   |38Qt5|
+3.9    Qt5        Linux   |39Qt5|
+3.10   Qt5        Linux   |310Qt5|
+3.11   Qt5        Linux   |311Qt5|
+3.8    Qt5        Windows |38Qt5win|
+3.8    PySide2    Linux   |38pyside|
+3.9    Qt6        Linux   |39Qt6|
+====== ========== ======= ======
 
 
 .. |38Qt5| image:: https://github.com/PyMoDAQ/PyMoDAQ/actions/workflows/Testp38pyqt5.yml/badge.svg?branch=pymodaq-dev
     :target: https://github.com/PyMoDAQ/PyMoDAQ/actions/workflows/Testp38pyqt5.yml
 
 .. |39Qt5| image:: https://github.com/PyMoDAQ/PyMoDAQ/actions/workflows/Testp39pyqt5.yml/badge.svg?branch=pymodaq-dev
     :target: https://github.com/PyMoDAQ/PyMoDAQ/actions/workflows/Testp39pyqt5.yml
@@ -132,28 +131,33 @@
 It is organised a shown below:
 
 .. figure:: http://pymodaq.cnrs.fr/en/latest/_images/pymodaq_diagram.png
    :alt: overview
 
    PyMoDAQ's Dashboard and its extensions: DAQ_Scan for automated acquisitions, DAQ_Logger for data logging and many other.
 
+The main component is the **Dashboard** : This is a graphical component that will initialize actuators and detectors given
+the need of your particular experiment. You configure the dashboard using an interface for quick launch of various
+configurations (numbers and types of control modules).
+
+The detectors and the actuators are represented and manipulated using two control modules:
+
+* **DAQ_Move_module** : used to control/drive an actuator (stand alone and/or automated).
+  Any number of these modules can be instantiated in the Dashboard
+* **DAQ_Viewer_module** : used to control/drive a detector (stand alone and/or automated).
+
+Any number of these modules can be instantiated in the Dashboard.
+
+The Dashboard allows you to start dedicated extensions that will make use of the control modules:
 
-* **Dashboard_module** : This is the module that will initialize actuators and detectors given the need of your
-  particular experiment. You configure the dashboard using an interface for quick launch of various configurations.
 * **DAQ_Logger_module** : This module lets you log data from one or many detectors defined in the dashboard. You can log data
   in a binary hierarchical hdf5 file or towards a sql database
 * **DAQ_Scan_module** : This module lets you configure automated data acquisition from one or many detectors defined
   in the dashboard as a function or one or more actuators defined also in the dashboard.
 
-The detectors and the actuators are represented and manipulated using two control modules:
-
-* **DAQ_Move_module** : used to control/drive an actuator (stand alone and/or automated). Any number of these modules can be instantiated.
-* **DAQ_Viewer_module** : used to control/drive a detector (stand alone and/or automated). Any number of these modules can be instantiated.
-
 and many others to simplify any application development.
 
-
-Published under the CeCILL-B FREE SOFTWARE LICENSE
+Published under the MIT FREE SOFTWARE LICENSE
 
 GitHub repo: https://github.com/PyMoDAQ
 
 Documentation: http://pymodaq.cnrs.fr/
```

