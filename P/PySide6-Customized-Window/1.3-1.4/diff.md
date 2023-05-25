# Comparing `tmp/PySide6_Customized_Window-1.3-py3-none-any.whl.zip` & `tmp/PySide6_Customized_Window-1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,7 @@
-Zip file size: 10713 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    48100 b- defN 23-May-04 15:07 PySide6_Customized_Window.py
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      619 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      486 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      672 b- defN 23-May-04 15:13 PySide6_Customized_Window-1.3.dist-info/RECORD
-7 files, 49985 bytes uncompressed, 9503 bytes compressed:  81.0%
+Zip file size: 10966 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    47011 b- defN 23-May-25 14:38 PySide6_Customized_Window.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-25 15:34 PySide6_Customized_Window-1.4.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-25 15:34 PySide6_Customized_Window-1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2518 b- defN 23-May-25 15:34 PySide6_Customized_Window-1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      452 b- defN 23-May-25 15:34 PySide6_Customized_Window-1.4.dist-info/RECORD
+5 files, 50079 bytes uncompressed, 10124 bytes compressed:  79.8%
```

## zipnote {}

```diff
@@ -1,22 +1,16 @@
 Filename: PySide6_Customized_Window.py
 Comment: 
 
-Filename: PySide6_Customized_Window-1.3.dist-info/DESCRIPTION.rst
+Filename: PySide6_Customized_Window-1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: PySide6_Customized_Window-1.3.dist-info/metadata.json
+Filename: PySide6_Customized_Window-1.4.dist-info/WHEEL
 Comment: 
 
-Filename: PySide6_Customized_Window-1.3.dist-info/top_level.txt
+Filename: PySide6_Customized_Window-1.4.dist-info/METADATA
 Comment: 
 
-Filename: PySide6_Customized_Window-1.3.dist-info/WHEEL
-Comment: 
-
-Filename: PySide6_Customized_Window-1.3.dist-info/METADATA
-Comment: 
-
-Filename: PySide6_Customized_Window-1.3.dist-info/RECORD
+Filename: PySide6_Customized_Window-1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PySide6_Customized_Window.py

```diff
@@ -87,66 +87,59 @@
 
 class Win10BlurEffect:
     def __init__(self):
         self.WCA_ACCENT_POLICY = 19
         self.ACCENT_ENABLE_BLURBEHIND = 3
         self.ACCENT_ENABLE_ACRYLICBLURBEHIND = 4
         self.SetWindowCompositionAttribute = ctypes.windll.user32.SetWindowCompositionAttribute
-
         self.accentPolicy = ACCENT_POLICY()
         self.winCompAttrData = WINDOWCOMPOSITIONATTRIBDATA()
         self.winCompAttrData.Attribute = self.WCA_ACCENT_POLICY
         self.winCompAttrData.SizeOfData = ctypes.sizeof(self.accentPolicy)
-        self.winCompAttrData.Data = ctypes.pointer(self.accentPolicy)
+        self.winCompAttrData.Data = ctypes.byref(self.accentPolicy)
 
     def setAeroEffect(self, hWnd, gradientColor='01000000', isEnableShadow=True, animationId=0):
         gradientColor = ctypes.c_ulong(int(gradientColor, base=16))
         animationId = ctypes.c_ulong(animationId)
         accentFlags = ctypes.c_ulong(0x20 | 0x40 | 0x80 | 0x100 | 0x200) if isEnableShadow else ctypes.c_ulong(0)
-
         self.accentPolicy.AccentState = self.ACCENT_ENABLE_BLURBEHIND
         self.accentPolicy.GradientColor = gradientColor
         self.accentPolicy.AccentFlags = accentFlags
         self.accentPolicy.AnimationId = animationId
-        code = self.SetWindowCompositionAttribute(hWnd, ctypes.pointer(self.winCompAttrData))
+        code = self.SetWindowCompositionAttribute(hWnd, ctypes.byref(self.winCompAttrData))
         return code
 
     def setAcrylicEffect(self, hWnd, gradientColor='01000000', isEnableShadow=True, animationId=0):
         gradientColor = ctypes.c_ulong(int(gradientColor, base=16))
         animationId = ctypes.c_ulong(animationId)
         accentFlags = ctypes.c_ulong(0x20 | 0x40 | 0x80 | 0x100) if isEnableShadow else ctypes.c_ulong(0)
-
         self.accentPolicy.AccentState = self.ACCENT_ENABLE_ACRYLICBLURBEHIND
         self.accentPolicy.GradientColor = gradientColor
         self.accentPolicy.AccentFlags = accentFlags
         self.accentPolicy.AnimationId = animationId
-        code = self.SetWindowCompositionAttribute(hWnd, ctypes.pointer(self.winCompAttrData))
+        code = self.SetWindowCompositionAttribute(hWnd, ctypes.byref(self.winCompAttrData))
         return code
 
 
 def isAeroEnabled():
     try:
         pfEnabled = ctypes.c_uint()
         ctypes.windll.dwmapi.DwmIsCompositionEnabled(ctypes.byref(pfEnabled))
         return pfEnabled.value
-    except:
-        return 0
+    except: return 0
 
 
 def isdarktheme():
     try:
         value = winreg.QueryValueEx(winreg.OpenKey(winreg.HKEY_CURRENT_USER,
-                                                   "Software\\Microsoft\\Windows\\CurrentVersion\\Themes\\Personalize"),
-                                    "AppsUseLightTheme")[0]
-    except:
-        return False
-    if value:
-        return False
-    else:
-        return True
+                                                   'Software\\Microsoft\\Windows\\CurrentVersion\\Themes\\Personalize'),
+                                    'AppsUseLightTheme')[0]
+    except: return False
+    if value: return False
+    else: return True
 
 
 def pyside1_hwnd(winId):
     try:
         ctypes.pythonapi.PyCapsule_GetPointer.restype = ctypes.c_void_p
         ctypes.pythonapi.PyCapsule_GetPointer.argtypes = [ctypes.py_object, ctypes.c_char_p]
         hwnd = ctypes.pythonapi.PyCapsule_GetPointer(winId, None)
@@ -156,18 +149,16 @@
         hwnd = ctypes.pythonapi.PyCObject_AsVoidPtr(winId)
     return hwnd
 
 
 def gethwnd(window):
     hwnd = window.winId()
     if type(hwnd) != int:
-        try:
-            hwnd = int(hwnd)
-        except:
-            hwnd = pyside1_hwnd(hwnd)
+        try: hwnd = int(hwnd)
+        except: hwnd = pyside1_hwnd(hwnd)
     return hwnd
 
 
 def getdpiforwindow_winapi(hwnd):
     try:
         dpi_x = ctypes.c_uint()
         dpi_y = ctypes.c_uint()
@@ -176,111 +167,85 @@
         dpi = dpi_x.value
     except:
         if hasattr(ctypes.windll.user32, 'IsProcessDPIAware'):
             if ctypes.windll.user32.IsProcessDPIAware():
                 hDC = ctypes.windll.user32.GetDC(None)
                 dpi = ctypes.windll.gdi32.GetDeviceCaps(hDC, 88)
                 ctypes.windll.user32.ReleaseDC(None, hDC)
-            else:
-                dpi = 96
-        else:
-            dpi = 96
+            else: dpi = 96
+        else: dpi = 96
     return dpi
 
 
 def getautohidetaskbarposition():
     SPI_GETWORKAREA = 0x30
     primaryscreenrect = RECT()
-    primaryscreenwidth = ctypes.windll.user32.GetSystemMetrics(0)
-    primaryscreenheight = ctypes.windll.user32.GetSystemMetrics(1)
+    GetSystemMetrics = ctypes.windll.user32.GetSystemMetrics
+    FindWindowA = ctypes.windll.user32.FindWindowA
+    GetWindowRect = ctypes.windll.user32.GetWindowRect
+    primaryscreenwidth = GetSystemMetrics(0)
+    primaryscreenheight = GetSystemMetrics(1)
     primaryscreenrect.left = 0
     primaryscreenrect.top = 0
     primaryscreenrect.right = primaryscreenwidth
     primaryscreenrect.bottom = primaryscreenheight
-    if primaryscreenwidth != primaryscreenrect.right - primaryscreenrect.left or primaryscreenheight != primaryscreenrect.bottom - primaryscreenrect.top:
-        return 4
-    taskbar_hwnd = ctypes.windll.user32.FindWindowA(b'Shell_TrayWnd', None)
-    if not taskbar_hwnd:
-        return 4
+    if primaryscreenwidth != primaryscreenrect.right - primaryscreenrect.left or primaryscreenheight != primaryscreenrect.bottom - primaryscreenrect.top: return 4
+    taskbar_hwnd = FindWindowA(b'Shell_TrayWnd', None)
+    if not taskbar_hwnd: return 4
     taskbar_rect = RECT()
-    ctypes.windll.user32.GetWindowRect(taskbar_hwnd, ctypes.byref(taskbar_rect))
-    if taskbar_rect.left < primaryscreenrect.left and taskbar_rect.top == primaryscreenrect.top and taskbar_rect.right != primaryscreenrect.right and taskbar_rect.bottom == primaryscreenrect.bottom:
-        return 0
-    elif taskbar_rect.left == primaryscreenrect.left and taskbar_rect.top < primaryscreenrect.top and taskbar_rect.right == primaryscreenrect.right and taskbar_rect.bottom != primaryscreenrect.bottom:
-        return 1
-    elif taskbar_rect.left != primaryscreenrect.left and taskbar_rect.top == primaryscreenrect.top and taskbar_rect.right > primaryscreenrect.right and taskbar_rect.bottom == primaryscreenrect.bottom:
-        return 2
-    elif taskbar_rect.left == primaryscreenrect.left and taskbar_rect.top != primaryscreenrect.top and taskbar_rect.right == primaryscreenrect.right and taskbar_rect.bottom > primaryscreenrect.bottom:
-        return 3
-    else:
-        return 4
+    GetWindowRect(taskbar_hwnd, ctypes.byref(taskbar_rect))
+    if taskbar_rect.left < primaryscreenrect.left and taskbar_rect.top == primaryscreenrect.top and taskbar_rect.right != primaryscreenrect.right and taskbar_rect.bottom == primaryscreenrect.bottom: return 0
+    elif taskbar_rect.left == primaryscreenrect.left and taskbar_rect.top < primaryscreenrect.top and taskbar_rect.right == primaryscreenrect.right and taskbar_rect.bottom != primaryscreenrect.bottom: return 1
+    elif taskbar_rect.left != primaryscreenrect.left and taskbar_rect.top == primaryscreenrect.top and taskbar_rect.right > primaryscreenrect.right and taskbar_rect.bottom == primaryscreenrect.bottom: return 2
+    elif taskbar_rect.left == primaryscreenrect.left and taskbar_rect.top != primaryscreenrect.top and taskbar_rect.right == primaryscreenrect.right and taskbar_rect.bottom > primaryscreenrect.bottom: return 3
+    else: return 4
     
 
 
 def getcaptionfont():
     result = NONCLIENTMETRICS()
     result.cbSize = ctypes.sizeof(NONCLIENTMETRICS)
-    ctypes.windll.user32.SystemParametersInfoW(0x29, ctypes.sizeof(NONCLIENTMETRICS), ctypes.pointer(result), 0)
+    ctypes.windll.user32.SystemParametersInfoW(0x29, ctypes.sizeof(NONCLIENTMETRICS), ctypes.byref(result), 0)
     captionfont = result.lfCaptionFont.lfFaceName
     return captionfont
 
 
 class CustomizedWindow(QWidget):
     '''A customized window based on PySideX.'''
     def __init__(self):
         super(CustomizedWindow, self).__init__()
+        user32 = ctypes.windll.user32
         self.hwnd = gethwnd(self)
         self.animation1 = QPropertyAnimation(self, b'windowOpacity')
         self.animation1.setDuration(250)
         self.animation1.setStartValue(0.0)
         self.animation1.setEndValue(1.0)
         self.animation2 = QPropertyAnimation(self, b'windowOpacity')
         self.animation2.setDuration(250)
         self.animation2.setStartValue(1.0)
         self.animation2.setEndValue(0.0)
-        self.nonclientareasizeinited = False
         self.isblurwindow = isinstance(self, BlurWindow)
-        WNDPROC = ctypes.WINFUNCTYPE(ctypes.c_long, ctypes.c_int, ctypes.c_uint, ctypes.c_int, ctypes.c_int)
-        BasicMessageHandlerAddress = ctypes.cast(WNDPROC(self.BasicMessageHandler), ctypes.c_void_p).value
-        if hasattr(ctypes.windll.user32, 'GetWindowLongPtrW'):
-            self.originalBasicMessageHandler = ctypes.windll.user32.GetWindowLongPtrW(self.hwnd, -4)
-        else:
-            self.originalBasicMessageHandler = ctypes.windll.user32.GetWindowLongW(self.hwnd, -4)
-        if ISPYSIDE1:
-            if hasattr(ctypes.windll.user32, 'SetWindowLongPtrW'):
-                ctypes.windll.user32.SetWindowLongPtrW(self.hwnd, -4, ctypes.c_int64(BasicMessageHandlerAddress))
-            else:
-                ctypes.windll.user32.SetWindowLongW(self.hwnd, -4, BasicMessageHandlerAddress)
-        self.setAttribute(Qt.WA_TranslucentBackground, True)
-        self.hwnd = gethwnd(self)
-        if ISPYSIDE1:
-            ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, 0x40000 | 0x20000 | 0x10000)
-        else:
-            ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, 0xc00000 | 0x40000 | 0x20000 | 0x10000)
         self.isaeroenabled = isAeroEnabled()
-        if self.isaeroenabled:
-            if self.isblurwindow:
-                self.setBlurEffect()
-            else:
-                self.setDWMShadowEffect()
+        self.setAttribute(Qt.WA_TranslucentBackground, True)
+        self.SetWindowLong = user32.SetWindowLongPtrW if hasattr(user32, 'SetWindowLongPtrW') else user32.SetWindowLongW 
+        WNDPROC = ctypes.WINFUNCTYPE(ctypes.c_long, ctypes.c_int, ctypes.c_uint, ctypes.c_int, ctypes.c_int)
+        self.BasicMessageHandlerAddress = ctypes.cast(WNDPROC(self.BasicMessageHandler), ctypes.c_void_p).value
+        if hasattr(user32, 'GetWindowLongPtrW'): self.originalBasicMessageHandler = user32.GetWindowLongPtrW(self.hwnd, -4)
+        else: self.originalBasicMessageHandler = user32.GetWindowLongW(self.hwnd, -4)
+        self.handle_setWindowFlags()
+        if self.isaeroenabled: self.setBlurEffect() if self.isblurwindow else self.setDWMShadowEffect()
         self.realdpi = getdpiforwindow_winapi(self.hwnd)
         self.highdpiscalingenabled = False
         self.highdpiscalefactorroundingpolicy = 3
         if hasattr(Qt, 'AA_EnableHighDpiScaling'):
-            if QApplication.testAttribute(Qt.AA_EnableHighDpiScaling):
-                self.highdpiscalingenabled = True
+            if QApplication.testAttribute(Qt.AA_EnableHighDpiScaling): self.highdpiscalingenabled = True
         if hasattr(Qt, 'HighDpiScaleFactorRoundingPolicy'):
             policy_dict = {Qt.HighDpiScaleFactorRoundingPolicy.Ceil: 1, Qt.HighDpiScaleFactorRoundingPolicy.Floor: 2, Qt.HighDpiScaleFactorRoundingPolicy.PassThrough: 3, Qt.HighDpiScaleFactorRoundingPolicy.Round: 4, Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor: 5}
-            if hasattr(Qt.HighDpiScaleFactorRoundingPolicy, 'Unset'):
-                if QApplication.highDpiScaleFactorRoundingPolicy() == Qt.HighDpiScaleFactorRoundingPolicy.Unset:
-                    self.highdpiscalefactorroundingpolicy = 3
-                else:
-                    self.highdpiscalefactorroundingpolicy = policy_dict[QApplication.highDpiScaleFactorRoundingPolicy()]
-            else:
-                self.highdpiscalefactorroundingpolicy = policy_dict[QApplication.highDpiScaleFactorRoundingPolicy()]
+            if hasattr(Qt.HighDpiScaleFactorRoundingPolicy, 'Unset'): self.highdpiscalefactorroundingpolicy = 3 if QApplication.highDpiScaleFactorRoundingPolicy() == Qt.HighDpiScaleFactorRoundingPolicy.Unset else policy_dict[QApplication.highDpiScaleFactorRoundingPolicy()]
+            else: self.highdpiscalefactorroundingpolicy = policy_dict[QApplication.highDpiScaleFactorRoundingPolicy()]
         self.dpi = self.getdpibyrealdpi(self.realdpi)
         dpi = self.dpi
         self.maximizedwindowborderwidth_list = self.getMaximizedWindowBorderWidth()
         self.themecolour = 0
         self.isdarktheme = isdarktheme()
         self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
         self.updateconstantsfordpi()
@@ -343,49 +308,66 @@
         self.closeButton.setFocusPolicy(Qt.NoFocus)
         self.titleBarLayout.addWidget(self.closeButton)
         self.paintTitleBarAndClientArea(self.isActiveWindow())
         self.originalSetWindowTitle = self.setWindowTitle
         self.setWindowTitle = self.setWindowTitle2
         self.originalSetWindowIcon = self.setWindowIcon
         self.setWindowIcon = self.setWindowIcon2
-        if not ISPYSIDE1:
-            self.windowHandle().screenChanged.connect(self.screenChangedHandler)
+        if not ISPYSIDE1: self.windowHandle().screenChanged.connect(self.screenChangedHandler)
     def setDarkTheme(self, themecolour=0):
         '''themecolour=0: Auto; themecolour=1: Light; themecolour=2: Dark'''
         self.themecolour = themecolour
-        if themecolour == 0:
-            self.isdarktheme = isdarktheme()
-        elif themecolour == 1:
-            self.isdarktheme = False
-        elif themecolour == 2:
-            self.isdarktheme = True
-        else:
-            raise Exception
+        if themecolour == 0: self.isdarktheme = isdarktheme()
+        elif themecolour == 1: self.isdarktheme = False
+        elif themecolour == 2: self.isdarktheme = True
+        else: raise Exception
     def setWindowTitle2(self, arg__1):
         self.originalSetWindowTitle(arg__1)
         self.paintTitleBarAndClientArea(self.isActiveWindow())
     def setWindowIcon2(self, icon):
         self.originalSetWindowIcon(icon)
         self.paintTitleBarAndClientArea(self.isActiveWindow())
+    def setWindowFlag(self, arg__1, on=True):
+        raise AttributeError('Function setWindowFlag has been deleted.')
+    def setWindowFlags(self, type):
+        raise AttributeError('Function setWindowFlags has been deleted.')
+    def handle_setWindowFlags(self):
+        user32 = ctypes.windll.user32
+        if ISPYSIDE1:
+            if hasattr(self, 'originalBasicMessageHandler'):
+                if hasattr(user32, 'SetWindowLongPtrW'): self.SetWindowLong(self.hwnd, -4, ctypes.c_int64(self.originalBasicMessageHandler))
+                else: self.SetWindowLong(self.hwnd, -4, self.originalBasicMessageHandler)
+        self.hwnd = gethwnd(self)
+        BasicMessageHandlerAddress = self.BasicMessageHandlerAddress
+        if hasattr(user32, 'GetWindowLongPtrW'): self.originalBasicMessageHandler = user32.GetWindowLongPtrW(self.hwnd, -4)
+        else: self.originalBasicMessageHandler = user32.GetWindowLongW(self.hwnd, -4)
+        self.nonclientareasizeinited = False
+        if ISPYSIDE1:
+            if hasattr(self, 'originalBasicMessageHandler'):
+                if hasattr(user32, 'SetWindowLongPtrW'): self.SetWindowLong(self.hwnd, -4, ctypes.c_int64(BasicMessageHandlerAddress))
+                else: self.SetWindowLong(self.hwnd, -4, BasicMessageHandlerAddress)
+            self.windowlong = self.SetWindowLong(self.hwnd, -16, 0x40000 | 0x20000 | 0x10000)
+        else:
+            self.windowlong = self.SetWindowLong(self.hwnd, -16, 0xc00000 | 0x40000 | 0x20000 | 0x10000)
+        if self.isaeroenabled: self.setBlurEffect() if self.isblurwindow else self.setDWMShadowEffect()
     def paintTitleBarAndClientArea(self, isactivewindow=0, ismaximized=-1):
         SWP_NOSIZE = 0x1
         SWP_NOMOVE = 0x2
         SWP_NOZORDER = 0x4
         hwnd = self.hwnd
         dpi = self.dpi
         title_height = self.title_height
         menubutton_width = self.menubutton_width
         title_font_size = self.title_font_size
         titleiconlayout_margin = self.titleiconlayout_margin
         captionfont = self.captionfont
         isblurwindow = self.isblurwindow
         isaeroenabled = self.isaeroenabled
         isdarktheme = self.isdarktheme
-        if ismaximized == -1:
-            ismaximized = self.isMaximized()
+        if ismaximized == -1: ismaximized = self.isMaximized()
         self.titleBar.setLayout(self.titleBarLayout)
         self.titleBar.setFixedHeight(self.title_height)
         self.titleIconContainerLabel.setFixedSize(title_height, title_height)
         titleiconsize = int(title_height - int(2.0 * titleiconlayout_margin))
         windowicon = self.windowIcon()
         windowiconpixmap = windowicon.pixmap(titleiconsize, titleiconsize)
         self.titleIconLabel.setPixmap(windowiconpixmap)
@@ -396,81 +378,53 @@
         self.minSizeButton.setFixedSize(menubutton_width, title_height)
         self.maxSizeButton.setFixedSize(menubutton_width, title_height)
         self.closeButton.setFixedSize(menubutton_width, title_height)
         self.minSizeButton.setStyleSheet('background:transparent; border-radius:0px')
         self.maxSizeButton.setStyleSheet('background:transparent; border-radius:0px')
         self.closeButton.setStyleSheet('background:transparent; border-radius:0px')
         titletextpalette = QPalette()
-        self.titleTextLabel.setStyleSheet('''QLabel{
-background:transparent;
-font-family:'%s';
-font-size:%dpx;
-}''' % (captionfont, title_font_size))
+        self.titleTextLabel.setStyleSheet('background:transparent; font-family:%s; font-size:%dpx' % (captionfont, title_font_size))
         if isdarktheme:
             try:
                 ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 19, ctypes.byref(ctypes.c_int(1)), ctypes.sizeof(ctypes.c_int(1)))
                 ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 20, ctypes.byref(ctypes.c_int(1)), ctypes.sizeof(ctypes.c_int(1)))
             except: pass
             ctypes.windll.user32.SetWindowPos(hwnd, None, 0, 0, 0, 0, SWP_NOSIZE | SWP_NOMOVE | SWP_NOZORDER)
             if isblurwindow:
                 if isaeroenabled:
-                    self.titleBar.setStyleSheet('''QLabel{
-background:qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1, stop: 0.0 rgba(0, 0, 0, 107) , stop: 1.0 rgba(0, 0, 0, 197));
-}''')
-                    self.clientArea.setStyleSheet('''QLabel{
-background:rgba(0, 0, 0, 127);
-}''')
+                    self.titleBar.setStyleSheet('background:qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1, stop: 0.0 rgba(0, 0, 0, 107) , stop: 1.0 rgba(0, 0, 0, 197))')
+                    self.clientArea.setStyleSheet('QLabel{background:rgba(0, 0, 0, 127)}')
                 else:
-                    self.titleBar.setStyleSheet('''QLabel{
-background:qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1, stop: 0.0 rgba(38, 38, 38, 255) , stop: 1.0 rgba(0, 0, 0, 255));
-}''')
-                    self.clientArea.setStyleSheet('''QLabel{
-background:rgba(20, 20, 20, 255);
-}''')
+                    self.titleBar.setStyleSheet('background:qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1, stop: 0.0 rgba(38, 38, 38, 255) , stop: 1.0 rgba(0, 0, 0, 255))')
+                    self.clientArea.setStyleSheet('QLabel{background:rgba(20, 20, 20, 255)}')
             else:
-                self.titleBar.setStyleSheet('''QLabel{
-background:#000000;
-}''')
-                self.clientArea.setStyleSheet('''QLabel{
-background:#000000;
-}''')
+                self.titleBar.setStyleSheet('background:#000000')
+                self.clientArea.setStyleSheet('QLabel{background:#000000}')
             if isactivewindow:
                 menuButtonPen = QPen(Qt.white)
                 titletextpalette.setColor(QPalette.WindowText, Qt.white)
             else:
                 menuButtonPen = QPen(QColor(155, 155, 155))
                 titletextpalette.setColor(QPalette.WindowText, QColor(155, 155, 155))
         else:
             try:
                 ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 19, ctypes.byref(ctypes.c_int(0)), ctypes.sizeof(ctypes.c_int(0)))
                 ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 20, ctypes.byref(ctypes.c_int(0)), ctypes.sizeof(ctypes.c_int(0)))
             except: pass
             ctypes.windll.user32.SetWindowPos(hwnd, None, 0, 0, 0, 0, SWP_NOSIZE | SWP_NOMOVE | SWP_NOZORDER)
             if isblurwindow:
                 if isaeroenabled:
-                    self.titleBar.setStyleSheet('''QLabel{
-background:qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1, stop: 0.0 rgba(255, 255, 255, 107) , stop: 1.0 rgba(255, 255, 255, 197));
-}''')
-                    self.clientArea.setStyleSheet('''QLabel{
-background:rgba(255, 255, 255, 127);
-}''')
+                    self.titleBar.setStyleSheet('background:qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1, stop: 0.0 rgba(255, 255, 255, 107) , stop: 1.0 rgba(255, 255, 255, 197))')
+                    self.clientArea.setStyleSheet('QLabel{background:rgba(255, 255, 255, 127)}')
                 else:
-                    self.titleBar.setStyleSheet('''QLabel{
-background:qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1, stop: 0.0 rgba(217, 217, 217, 255) , stop: 1.0 rgba(255, 255, 255, 255));
-}''')
-                    self.clientArea.setStyleSheet('''QLabel{
-background:rgba(235, 235, 235, 255);
-}''')
+                    self.titleBar.setStyleSheet('background:qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1, stop: 0.0 rgba(217, 217, 217, 255) , stop: 1.0 rgba(255, 255, 255, 255))')
+                    self.clientArea.setStyleSheet('QLabel{background:rgba(235, 235, 235, 255)}')
             else:
-                self.titleBar.setStyleSheet('''QLabel{
-background:#FFFFFF;
-}''')
-                self.clientArea.setStyleSheet('''QLabel{
-background:#FFFFFF;
-}''')
+                self.titleBar.setStyleSheet('background:#FFFFFF')
+                self.clientArea.setStyleSheet('QLabel{background:#FFFFFF}')
             if isactivewindow:
                 menuButtonPen = QPen(Qt.black)
                 titletextpalette.setColor(QPalette.WindowText, Qt.black)
             else:
                 menuButtonPen = QPen(QColor(99, 99, 99))
                 titletextpalette.setColor(QPalette.WindowText, QColor(99, 99, 99))
         self.titleTextLabel.setPalette(titletextpalette)
@@ -533,56 +487,50 @@
         self.closeButton.setIcon(closeIcon)
         self.closeButton.setIconSize(QSize(menubutton_width, title_height))
     def setMenuButtonStyle(self, button, state=1):
         stylesheet1 = 'background:transparent'
         stylesheet2 = 'background:transparent'
         stylesheet3 = 'background:transparent'
         if button == 1:
-            if state == 1:
-                stylesheet1 = self.minMaxSizeButtonHoverBackgroundStyleSheet_Dark if self.isdarktheme else self.minMaxSizeButtonHoverBackgroundStyleSheet_Light
-            elif state == 2:
-                stylesheet1 = self.minMaxSizeButtonPressedBackgroundStyleSheet_Dark if self.isdarktheme else self.minMaxSizeButtonPressedBackgroundStyleSheet_Light
+            if state == 1: stylesheet1 = self.minMaxSizeButtonHoverBackgroundStyleSheet_Dark if self.isdarktheme else self.minMaxSizeButtonHoverBackgroundStyleSheet_Light
+            elif state == 2: stylesheet1 = self.minMaxSizeButtonPressedBackgroundStyleSheet_Dark if self.isdarktheme else self.minMaxSizeButtonPressedBackgroundStyleSheet_Light
         elif button == 2:
-            if state == 1:
-                stylesheet2 = self.minMaxSizeButtonHoverBackgroundStyleSheet_Dark if self.isdarktheme else self.minMaxSizeButtonHoverBackgroundStyleSheet_Light
-            elif state == 2:
-                stylesheet2 = self.minMaxSizeButtonPressedBackgroundStyleSheet_Dark if self.isdarktheme else self.minMaxSizeButtonPressedBackgroundStyleSheet_Light
+            if state == 1: stylesheet2 = self.minMaxSizeButtonHoverBackgroundStyleSheet_Dark if self.isdarktheme else self.minMaxSizeButtonHoverBackgroundStyleSheet_Light
+            elif state == 2: stylesheet2 = self.minMaxSizeButtonPressedBackgroundStyleSheet_Dark if self.isdarktheme else self.minMaxSizeButtonPressedBackgroundStyleSheet_Light
         elif button == 3:
-            if state == 1:
-                stylesheet3 = self.closeButtonHoverBackgroundStyleSheet
-            elif state == 2:
-                stylesheet3 = self.closeButtonPressedBackgroundStyleSheet
-        elif button != 0:
-            raise Exception
+            if state == 1: stylesheet3 = self.closeButtonHoverBackgroundStyleSheet
+            elif state == 2: stylesheet3 = self.closeButtonPressedBackgroundStyleSheet
+        elif button != 0: raise Exception
         self.minSizeButton.setStyleSheet(stylesheet1)
         self.maxSizeButton.setStyleSheet(stylesheet2)
         self.closeButton.setStyleSheet(stylesheet3)
     def MessageHandler(self, hwnd, message, wParam, lParam):
         '''Example:
 class MyOwnWindow(self):
 |->|...
 |->|def MessageHandler(self, hwnd, message, wParam, lParam):
 |->||->|print(hwnd, message, wParam, lParam)
 |->||->|...'''
         pass
     def BasicMessageHandler(self, hwnd, message, wParam, lParam):
         '''For PySide1/2/6, you should define MessageHandler instead of BasicMessageHandler.'''
+        user32 = ctypes.windll.user32
         WM_ACTIVATE = 0x6
         WM_SHOWWINDOW = 0x18
         WM_SETTINGCHANGE = 0x1a
-        WM_GETMINMAXINFO = 0x24
-        WM_WINDOWPOSCHANGED = 0x47
+        WM_STYLECHANGED = 0x7d
         WM_NCCALCSIZE = 0x83
         WM_NCHITTEST = 0x84
         WM_NCLBUTTONDOWN = 0xa1
         WM_NCLBUTTONUP = 0xa2
         WM_LBUTTONUP = 0x2a2
         WM_DPICHANGED = 0x2e0
         WM_SYSCOMMAND = 0x112
         WM_DWMCOMPOSITIONCHANGED = 0x31e
+        WM_DWMNCRENDERINGCHANGED = 0x31f
         SW_PARENTOPENING = 0x3
         SC_SIZE = 0xf000
         SC_MOVE = 0xf010
         SC_MINIMIZE = 0xf020
         SC_MAXIMIZE = 0xf030
         SC_CLOSE = 0xf060
         SC_RESTORE = 0xf120
@@ -629,21 +577,21 @@
             windowrect = self.GetWindowRect()
         except:
             windowrect = RECT(0, 0, 0, 0)
         windowx = windowrect.left
         windowy = windowrect.top
         try:
             globalpos = POINT()
-            ctypes.windll.user32.GetPhysicalCursorPos(ctypes.byref(globalpos))
-            ctypes.windll.user32.PhysicalToLogicalPoint(self.hwnd, ctypes.byref(globalpos))
+            user32.GetPhysicalCursorPos(ctypes.byref(globalpos))
+            user32.PhysicalToLogicalPoint(self.hwnd, ctypes.byref(globalpos))
             x = globalpos.x - windowx
             y = globalpos.y - windowy
         except:
             globalpos = POINT()
-            ctypes.windll.user32.GetCursorPos(ctypes.byref(globalpos))
+            user32.GetCursorPos(ctypes.byref(globalpos))
             x = globalpos.x - windowx
             y = globalpos.y - windowy
         width = windowrect.right - windowx
         height = windowrect.bottom - windowy
         intitlebar = windowmargin_top <= y < real_title_height + windowmargin_top
         inminsizebutton = int(width - windowmargin_left - 3 * real_menubutton_width) <= x < int(width - windowmargin_left - 2 * real_menubutton_width) and intitlebar
         inmaxsizebutton = int(width - windowmargin_left - 2 * real_menubutton_width) <= x < int(width - windowmargin_left - real_menubutton_width) and intitlebar
@@ -660,196 +608,154 @@
         self.inleftborder = inleftborder
         self.inbottomborder = inbottomborder
         self.inrightborder = inrightborder
         if message == WM_NCCALCSIZE:
             return self.Handle_WM_NCCALCSIZE_Message(hwnd, message, wParam, lParam)
         if message == WM_NCHITTEST:
             VK_LBUTTON = 0x1
-            isleftbuttonpressed = ctypes.windll.user32.GetKeyState(VK_LBUTTON) not in [0, 1]
+            isleftbuttonpressed = user32.GetKeyState(VK_LBUTTON) not in [0, 1]
             if not self.isMaximized():
-                if intopborder and inleftborder:
-                    WM_NCHITTEST_result = HTTOPLEFT
-                elif intopborder and inrightborder:
-                    WM_NCHITTEST_result = HTTOPRIGHT
-                elif inbottomborder and inleftborder:
-                    WM_NCHITTEST_result = HTBOTTOMLEFT
-                elif inbottomborder and inrightborder:
-                    WM_NCHITTEST_result = HTBOTTOMRIGHT
-                elif inleftborder:
-                    WM_NCHITTEST_result = HTLEFT
-                elif intopborder:
-                    WM_NCHITTEST_result = HTTOP
-                elif inrightborder:
-                    WM_NCHITTEST_result = HTRIGHT
-                elif inbottomborder:
-                    WM_NCHITTEST_result = HTBOTTOM
+                if intopborder and inleftborder: WM_NCHITTEST_result = HTTOPLEFT
+                elif intopborder and inrightborder: WM_NCHITTEST_result = HTTOPRIGHT
+                elif inbottomborder and inleftborder: WM_NCHITTEST_result = HTBOTTOMLEFT
+                elif inbottomborder and inrightborder: WM_NCHITTEST_result = HTBOTTOMRIGHT
+                elif inleftborder: WM_NCHITTEST_result = HTLEFT
+                elif intopborder: WM_NCHITTEST_result = HTTOP
+                elif inrightborder: WM_NCHITTEST_result = HTRIGHT
+                elif inbottomborder: WM_NCHITTEST_result = HTBOTTOM
             if not 'WM_NCHITTEST_result' in dir():
                 if inminsizebutton:
-                    if not isleftbuttonpressed:
-                        self.setMenuButtonStyle(1, 1)
+                    if not isleftbuttonpressed: self.setMenuButtonStyle(1, 1)
                     WM_NCHITTEST_result = HTMINBUTTON
                 elif inmaxsizebutton:
-                    if not isleftbuttonpressed:
-                        self.setMenuButtonStyle(2, 1)
+                    if not isleftbuttonpressed: self.setMenuButtonStyle(2, 1)
                     WM_NCHITTEST_result = HTMAXBUTTON
                 elif inclosebutton:
-                    if not isleftbuttonpressed:
-                        self.setMenuButtonStyle(3, 1)
+                    if not isleftbuttonpressed: self.setMenuButtonStyle(3, 1)
                     WM_NCHITTEST_result = HTCLOSE
                 elif intitlebar:
                     WM_NCHITTEST_result = HTCAPTION
-                else:
-                    WM_NCHITTEST_result = HTCLIENT
+                else: WM_NCHITTEST_result = HTCLIENT
             if WM_NCHITTEST_result not in [HTMINBUTTON, HTMAXBUTTON, HTCLOSE]:
-                if not isleftbuttonpressed:
-                    self.setMenuButtonStyle(0)
+                if not isleftbuttonpressed: self.setMenuButtonStyle(0)
             return WM_NCHITTEST_result
         if message == WM_NCLBUTTONDOWN:
             if wParam in [HTMINBUTTON, HTMAXBUTTON, HTCLOSE]:
-                if wParam == HTMINBUTTON:
-                    self.setMenuButtonStyle(1, 2)
-                if wParam == HTMAXBUTTON:
-                    self.setMenuButtonStyle(2, 2)
-                if wParam == HTCLOSE:
-                    self.setMenuButtonStyle(3, 2)
+                if wParam == HTMINBUTTON: self.setMenuButtonStyle(1, 2)
+                if wParam == HTMAXBUTTON: self.setMenuButtonStyle(2, 2)
+                if wParam == HTCLOSE: self.setMenuButtonStyle(3, 2)
                 return 0
-            return ctypes.windll.user32.DefWindowProcW(hwnd, message, wParam, lParam)
+            return user32.DefWindowProcW(hwnd, message, wParam, lParam)
         if message == WM_NCLBUTTONUP:
             self.setMenuButtonStyle(0)
-            if wParam == HTMINBUTTON:
-                self.minSizeButtonClicked()
-            elif wParam == HTMAXBUTTON:
-                self.maxSizeButtonClicked()
-            elif wParam == HTCLOSE:
-                self.closeButtonClicked()
-            return ctypes.windll.user32.DefWindowProcW(hwnd, message, wParam, lParam)
+            if wParam == HTMINBUTTON: self.minSizeButtonClicked()
+            elif wParam == HTMAXBUTTON: self.maxSizeButtonClicked()
+            elif wParam == HTCLOSE: self.closeButtonClicked()
+            return user32.DefWindowProcW(hwnd, message, wParam, lParam)
         if message == WM_LBUTTONUP:
             self.setMenuButtonStyle(0)
         if message == WM_DPICHANGED:
             window_rect = RECT.from_address(lParam)
             realdpi = wParam >> 16
             self.realdpi = realdpi
             self.maximizedwindowborderwidth_list = self.getMaximizedWindowBorderWidth()
             x = window_rect.left
             y = window_rect.top
             width = int(window_rect.right - window_rect.left)
             height = int(window_rect.bottom - window_rect.top)
-            if not self.highdpiscalingenabled:
-                self.setGeometry(x, y, width, height)
+            if not self.highdpiscalingenabled: self.setGeometry(x, y, width, height)
             dpi = self.getdpibyrealdpi(realdpi)
             self.dpi = dpi
             self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
             self.updateconstantsfordpi()
             self.paintTitleBarAndClientArea(self.isActiveWindow())
         if message == WM_SETTINGCHANGE:
-            try:
-                lParam_string = str(ctypes.cast(lParam, ctypes.c_wchar_p).value)
-            except:
-                lParam_string = ''
+            try: lParam_string = str(ctypes.cast(lParam, ctypes.c_wchar_p).value)
+            except: lParam_string = ''
             if wParam == SPI_SETWORKAREA:
                 self.updateautohidetaskbarwidth()
-                ctypes.windll.user32.SetWindowPos(hwnd, None, 0, 0, 0, 0, SWP_NOSIZE | SWP_NOMOVE | SWP_NOZORDER | SWP_FRAMECHANGED)
+                user32.SetWindowPos(hwnd, None, 0, 0, 0, 0, SWP_NOSIZE | SWP_NOMOVE | SWP_NOZORDER | SWP_FRAMECHANGED)
             if wParam == SPI_SETNONCLIENTMETRICS:
                 self.maximizedwindowborderwidth_list = self.getMaximizedWindowBorderWidth()
                 self.captionfont = getcaptionfont()
             if self.themecolour == 0 and lParam_string == 'ImmersiveColorSet':
                 self.isdarktheme = isdarktheme()
                 self.paintTitleBarAndClientArea(self.isActiveWindow())
         if message == WM_DWMCOMPOSITIONCHANGED:
             self.isaeroenabled = isAeroEnabled()
-            if self.isaeroenabled:
-                if self.isblurwindow:
-                    self.setBlurEffect()
-                else:
-                    self.setDWMShadowEffect()
+            if self.isaeroenabled: self.setBlurEffect() if self.isblurwindow else self.setDWMShadowEffect()
             self.paintTitleBarAndClientArea(self.isActiveWindow())
+        if message == WM_DWMNCRENDERINGCHANGED:
+            if self.isaeroenabled: self.setBlurEffect() if self.isblurwindow else self.setDWMShadowEffect()
         if message == WM_ACTIVATE:
             isactivewindow = 0 if wParam == 0 else 1
-            if not isactivewindow:
-                self.setMenuButtonStyle(0)
+            if not isactivewindow: self.setMenuButtonStyle(0)
             self.paintTitleBarAndClientArea(isactivewindow)
         if message == WM_SHOWWINDOW:
             self.paintTitleBarAndClientArea(self.isActiveWindow())
+        if message == WM_STYLECHANGED:
+            if hasattr(self, 'nonclientareasizeinited'):
+                if self.nonclientareasizeinited: self.SetWindowLong(self.hwnd, -16, 0xc00000 | 0x40000 | 0x20000 | 0x10000)
         messagehandlerresult = self.MessageHandler(hwnd, message, wParam, lParam)
-        if messagehandlerresult != None:
-            return messagehandlerresult
-        if ISPYSIDE1:
-            return ctypes.windll.user32.CallWindowProcW(self.originalBasicMessageHandler, hwnd, message, wParam, lParam)
+        if messagehandlerresult != None: return messagehandlerresult
+        if ISPYSIDE1: return user32.CallWindowProcW(self.originalBasicMessageHandler, hwnd, message, wParam, lParam)
     def Handle_WM_NCCALCSIZE_Message(self, hwnd, message, wParam, lParam):
+        user32 = ctypes.windll.user32
         try:
-            nonclientareasizeinited = self.nonclientareasizeinited
             leftautohidetaskbarwidth = self.leftautohidetaskbarwidth
             topautohidetaskbarwidth = self.topautohidetaskbarwidth
             rightautohidetaskbarwidth = self.rightautohidetaskbarwidth
             bottomautohidetaskbarwidth = self.bottomautohidetaskbarwidth
         except:
-            nonclientareasizeinited = False
-            leftautohidetaskbarwidth = 0
-            topautohidetaskbarwidth = 0
-            rightautohidetaskbarwidth = 0
-            bottomautohidetaskbarwidth = 0
-        if not nonclientareasizeinited:
-            if ISPYSIDE1:
-                if hasattr(ctypes.windll.user32, 'GetWindowLongPtrW'):
-                    originalwindowlong = ctypes.windll.user32.GetWindowLongPtrW(self.hwnd, -16)
-                else:
-                    originalwindowlong = ctypes.windll.user32.GetWindowLongW(self.hwnd, -16)
-                if hasattr(ctypes.windll.user32, 'SetWindowLongPtrW'):
-                    ctypes.windll.user32.SetWindowLongPtrW(self.hwnd, -16, originalwindowlong | 0xc00000)
-                else:
-                    ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, originalwindowlong | 0xc00000)
-            self.nonclientareasizeinited = True
+            leftautohidetaskbarwidth, topautohidetaskbarwidth, rightautohidetaskbarwidth, bottomautohidetaskbarwidth = 0, 0, 0, 0
         if wParam:
             rect = ctypes.cast(lParam, ctypes.POINTER(NCCALCSIZE_PARAMS)).contents.rgrc[0]
         else:
             rect = ctypes.cast(lParam, ctypes.POINTER(RECT)).contents
-        ISMAXIMIZED = ctypes.windll.user32.IsZoomed(hwnd)
+        ISMAXIMIZED = user32.IsZoomed(hwnd)
         try:
             maximizedwindowborderwidth_list = self.maximizedwindowborderwidth_list
         except:
             maximizedwindowborderwidth_list = [0, 0]
         if ISMAXIMIZED:
             self.windowmargin_left = maximizedwindowborderwidth_list[0] + leftautohidetaskbarwidth
             self.windowmargin_right = maximizedwindowborderwidth_list[0] + rightautohidetaskbarwidth
             self.windowmargin_top = maximizedwindowborderwidth_list[1] + topautohidetaskbarwidth
             self.windowmargin_bottom = maximizedwindowborderwidth_list[1] + bottomautohidetaskbarwidth
-        else:
-            self.windowmargin_left = 0
-            self.windowmargin_right = 0
-            self.windowmargin_top = 0
-            self.windowmargin_bottom = 0
+        else: self.windowmargin_left, self.windowmargin_right, self.windowmargin_top, self.windowmargin_bottom = 0, 0, 0, 0
         windowmargin_left = self.windowmargin_left
         windowmargin_right = self.windowmargin_right
         windowmargin_top = self.windowmargin_top
         windowmargin_bottom = self.windowmargin_bottom
         rect.left += windowmargin_left
         rect.right -= windowmargin_right
         rect.top += windowmargin_top
         rect.bottom -= windowmargin_bottom
-        if nonclientareasizeinited:
-            self.paintTitleBarAndClientArea(self.isActiveWindow(), ISMAXIMIZED)
+        if hasattr(self, 'nonclientareasizeinited'):
+            nonclientareasizeinited = self.nonclientareasizeinited
+            if not nonclientareasizeinited:
+                if ISPYSIDE1: self.SetWindowLong(self.hwnd, -16, 0xc00000 | 0x40000 | 0x20000 | 0x10000)
+                self.nonclientareasizeinited = True
+            else: self.paintTitleBarAndClientArea(self.isActiveWindow(), ISMAXIMIZED)
         return 0
     def minSizeButtonClicked(self):
         WM_SYSCOMMAND = 0x112
         SC_MINIMIZE = 0xf020
-        ctypes.windll.user32.SendMessageW(self.hwnd, WM_SYSCOMMAND, SC_MINIMIZE, 0)
+        ctypes.windll.user32.PostMessageW(self.hwnd, WM_SYSCOMMAND, SC_MINIMIZE, 0)
     def maxSizeButtonClicked(self):
         WM_SYSCOMMAND = 0x112
         SC_MAXIMIZE = 0xf030
         SC_RESTORE = 0xf120
-        if self.isMaximized():
-            ctypes.windll.user32.SendMessageW(self.hwnd, WM_SYSCOMMAND, SC_RESTORE, 0)
-        elif self.isFullScreen():
-            pass
-        else:
-            ctypes.windll.user32.SendMessageW(self.hwnd, WM_SYSCOMMAND, SC_MAXIMIZE, 0)
+        if self.isMaximized(): ctypes.windll.user32.PostMessageW(self.hwnd, WM_SYSCOMMAND, SC_RESTORE, 0)
+        elif self.isFullScreen(): pass
+        else: ctypes.windll.user32.PostMessageW(self.hwnd, WM_SYSCOMMAND, SC_MAXIMIZE, 0)
     def closeButtonClicked(self):
         WM_SYSCOMMAND = 0x112
         SC_CLOSE = 0xf060
-        ctypes.windll.user32.SendMessageW(self.hwnd, WM_SYSCOMMAND, SC_CLOSE, 0)
+        ctypes.windll.user32.PostMessageW(self.hwnd, WM_SYSCOMMAND, SC_CLOSE, 0)
     def getMaximizedWindowBorderWidth(self):
         SM_CXSIZEFRAME = 32
         SM_CYSIZEFRAME = 33
         SM_CXPADDEDBORDER = 92
         realdpi = self.realdpi
         if hasattr(ctypes.windll.user32, 'GetSystemMetricsForDpi'):
             borderwidth_x = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXSIZEFRAME, realdpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, realdpi)
@@ -863,76 +769,58 @@
         WM_NCCALCSIZE = 0x83
         msg = MSG.from_address(msg.__int__())
         hwnd = msg.hWnd
         message = msg.message
         wParam = msg.wParam
         lParam = msg.lParam
         basicmessagehandlerresult = self.BasicMessageHandler(hwnd, message, wParam, lParam)
-        if basicmessagehandlerresult != None:
-            return True, basicmessagehandlerresult
+        if basicmessagehandlerresult != None: return True, basicmessagehandlerresult
         return super(CustomizedWindow, self).nativeEvent(eventType, msg)
     def setBlurEffect(self):
         hwnd = self.hwnd
         try:
+            dwmapi = ctypes.windll.dwmapi
+            dwmapi.DwmSetWindowAttribute(hwnd, 2, ctypes.byref(ctypes.c_int(2)), ctypes.sizeof(ctypes.c_int(2)))
             bb = DWM_BLURBEHIND()
             bb.dwFlags = 1
             bb.fEnable = 1
-            ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 2, ctypes.byref(ctypes.c_int(2)), ctypes.sizeof(ctypes.c_int(2)))
             win11_21h2_blur_code, win11_22h2_blur_code = self.setwin11blur(hwnd)
             if win11_22h2_blur_code:
-                ctypes.windll.dwmapi.DwmExtendFrameIntoClientArea(hwnd, ctypes.byref(MARGINS(1, 1, 0, 0)))
-                ctypes.windll.dwmapi.DwmEnableBlurBehindWindow(ctypes.c_int(hwnd), ctypes.byref(bb))
+                dwmapi.DwmExtendFrameIntoClientArea(hwnd, ctypes.byref(MARGINS(1, 1, 0, 0)))
+                dwmapi.DwmEnableBlurBehindWindow(ctypes.c_int(hwnd), ctypes.byref(bb))
             else:
-                ctypes.windll.dwmapi.DwmExtendFrameIntoClientArea(hwnd, ctypes.byref(MARGINS(-1, -1, -1, -1)))
+                dwmapi.DwmExtendFrameIntoClientArea(hwnd, ctypes.byref(MARGINS(-1, -1, -1, -1)))
                 return 3
             try:
                 AeroEffect = Win10BlurEffect()
                 win10_blur_code = AeroEffect.setAeroEffect(hwnd, isEnableShadow=True)
-                if win10_blur_code != 0:
-                    return 2
+                if win10_blur_code != 0: return 2
             except: pass
             return 1
-        except:
-            return 0
+        except: return 0
     def setDWMShadowEffect(self):
         hwnd = self.hwnd
         try:
+            ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 2, ctypes.byref(ctypes.c_int(2)), ctypes.sizeof(ctypes.c_int(2)))
             ctypes.windll.dwmapi.DwmExtendFrameIntoClientArea(hwnd, ctypes.byref(MARGINS(1, 1, 0, 0)))
             return 1
-        except:
-            return 0
+        except: return 0
     def getdpibyrealdpi(self, realdpi):
         realscalefactor = realdpi / 96.0
         if self.highdpiscalingenabled:
-            if self.highdpiscalefactorroundingpolicy == 1:
-                if realscalefactor - int(realscalefactor) > 0:
-                    scalefactor = int(realscalefactor + 1)
-                else:
-                    scalefactor = int(realscalefactor)
-            elif self.highdpiscalefactorroundingpolicy == 2:
-                scalefactor = int(realscalefactor)
-            elif self.highdpiscalefactorroundingpolicy == 3:
-                scalefactor = realscalefactor
-            elif self.highdpiscalefactorroundingpolicy == 4:
-                if realscalefactor - int(realscalefactor) >= 0.5:
-                    scalefactor = int(realscalefactor + 1)
-                else:
-                    scalefactor = int(realscalefactor)
-            elif self.highdpiscalefactorroundingpolicy == 5:
-                if realscalefactor - int(realscalefactor) > 0.5:
-                    scalefactor = int(realscalefactor + 1)
-                else:
-                    scalefactor = int(realscalefactor)
+            if self.highdpiscalefactorroundingpolicy == 1: scalefactor = int(realscalefactor + 1) if realscalefactor - int(realscalefactor) > 0 else int(realscalefactor)
+            elif self.highdpiscalefactorroundingpolicy == 2: scalefactor = int(realscalefactor)
+            elif self.highdpiscalefactorroundingpolicy == 3: scalefactor = realscalefactor
+            elif self.highdpiscalefactorroundingpolicy == 4: scalefactor = int(realscalefactor + 1) if realscalefactor - int(realscalefactor) >= 0.5 else int(realscalefactor)
+            elif self.highdpiscalefactorroundingpolicy == 5: scalefactor = int(realscalefactor + 1) if realscalefactor - int(realscalefactor) > 0.5 else int(realscalefactor)
             dpi = int(float(realdpi) / scalefactor)
-        else:
-            dpi = realdpi
+        else: dpi = realdpi
         return dpi
     def updateconstantsfordpi(self):
-        dpi = self.dpi
-        realdpi = self.realdpi
+        dpi, realdpi = self.dpi, self.realdpi
         self.border_width = int(5.0 * dpi / 96.0)
         self.title_height = int(30.0 * dpi / 96.0)
         self.menubutton_width = int(46.0 * dpi / 96.0)
         self.title_font_size = int(13.0 * dpi / 96.0)
         self.real_border_width = int(5.0 * realdpi / 96.0)
         self.real_title_height = int(30.0 * realdpi / 96.0)
         self.real_menubutton_width = int(46.0 * realdpi / 96.0)
@@ -940,24 +828,17 @@
     def updateautohidetaskbarwidth(self):
         autohidetaskbarposition = getautohidetaskbarposition()
         self.leftautohidetaskbarwidth = 2 if autohidetaskbarposition == 0 else 0
         self.topautohidetaskbarwidth = 2 if autohidetaskbarposition == 1 else 0
         self.rightautohidetaskbarwidth = 2 if autohidetaskbarposition == 2 else 0
         self.bottomautohidetaskbarwidth = 2 if autohidetaskbarposition == 3 else 0
     def setwin11blur(self, hWnd):
-        Win11_21H2_ENTRY = 1029
-        Win11_21H2_VALUE = 1
-        Win11_22H2_ENTRY = 38
-        Win11_22H2_VALUE = 3
-        Win11_21H2_COMMAND = ctypes.windll.dwmapi.DwmSetWindowAttribute(hWnd, Win11_21H2_ENTRY,
-                                                                        ctypes.byref(ctypes.c_int(Win11_21H2_VALUE)),
-                                                                        ctypes.sizeof(ctypes.c_int))
-        Win11_22H2_COMMAND = ctypes.windll.dwmapi.DwmSetWindowAttribute(hWnd, Win11_22H2_ENTRY,
-                                                                        ctypes.byref(ctypes.c_int(Win11_22H2_VALUE)),
-                                                                        ctypes.sizeof(ctypes.c_int))
+        Win11_21H2_ENTRY, Win11_22H2_ENTRY = 1029, 38
+        Win11_21H2_VALUE, Win11_22H2_VALUE = 1, 3
+        Win11_21H2_COMMAND, Win11_22H2_COMMAND = list(map(ctypes.windll.dwmapi.DwmSetWindowAttribute, [hWnd] * 2, [Win11_21H2_ENTRY, Win11_22H2_ENTRY], [ctypes.byref(ctypes.c_int(Win11_21H2_VALUE)), ctypes.byref(ctypes.c_int(Win11_22H2_VALUE))], [ctypes.sizeof(ctypes.c_int)] * 2))
         return (Win11_21H2_COMMAND, Win11_22H2_COMMAND)
     def GetWindowRect(self):
         lpRect = RECT()
         ctypes.windll.user32.GetWindowRect(self.hwnd, ctypes.byref(lpRect))
         return lpRect
     def screenChangedHandler(self):
         hwnd = gethwnd(self.windowHandle())
```

