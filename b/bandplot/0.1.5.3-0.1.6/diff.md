# Comparing `tmp/bandplot-0.1.5.3-py3-none-any.whl.zip` & `tmp/bandplot-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17596 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       26 b- defN 23-May-23 01:14 bandplot/__init__.py
--rw-rw-r--  2.0 unx     7096 b- defN 23-May-23 01:14 bandplot/mass.py
--rw-rw-r--  2.0 unx    25644 b- defN 23-May-23 01:14 bandplot/plots.py
--rw-rw-r--  2.0 unx    22446 b- defN 23-May-23 01:14 bandplot/pplots.py
--rw-rw-r--  2.0 unx     9321 b- defN 23-May-23 01:14 bandplot/projected.py
--rw-rw-r--  2.0 unx     6229 b- defN 23-May-23 01:14 bandplot/readdata.py
--rw-rw-r--  2.0 unx    23361 b- defN 23-May-23 01:14 bandplot/wrapper.py
--rw-rw-r--  2.0 unx     3084 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      938 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/RECORD
-12 files, 98332 bytes uncompressed, 16034 bytes compressed:  83.7%
+Zip file size: 17866 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       24 b- defN 23-May-25 02:09 bandplot/__init__.py
+-rw-rw-r--  2.0 unx     7327 b- defN 23-May-25 02:09 bandplot/mass.py
+-rw-rw-r--  2.0 unx    26503 b- defN 23-May-25 02:09 bandplot/plots.py
+-rw-rw-r--  2.0 unx    23084 b- defN 23-May-25 02:09 bandplot/pplots.py
+-rw-rw-r--  2.0 unx     9548 b- defN 23-May-25 02:09 bandplot/projected.py
+-rw-rw-r--  2.0 unx     6229 b- defN 23-May-25 02:09 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    23474 b- defN 23-May-25 02:09 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     3082 b- defN 23-May-25 02:09 bandplot-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-25 02:09 bandplot-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-25 02:09 bandplot-0.1.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-25 02:09 bandplot-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      928 b- defN 23-May-25 02:09 bandplot-0.1.6.dist-info/RECORD
+12 files, 100386 bytes uncompressed, 16324 bytes compressed:  83.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.5.3.dist-info/METADATA
+Filename: bandplot-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.5.3.dist-info/WHEEL
+Filename: bandplot-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.5.3.dist-info/entry_points.txt
+Filename: bandplot-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.5.3.dist-info/top_level.txt
+Filename: bandplot-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.5.3.dist-info/RECORD
+Filename: bandplot-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.5.3"
+__version__ = "0.1.6"
```

## bandplot/mass.py

```diff
@@ -89,57 +89,62 @@
     return pltlabel
 
 def plot(data, calM, pltlabel, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['red']
     linestyle = fig_p.linestyle or [':']
     linewidth = fig_p.linewidth or [0.8]
+    location  = fig_p.location or [1, 2]
+    if len(location) == 1:
+        location = [location[0], 2]
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = data[0,0],data[-1,0]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     plt.xticks(ticks,labels)
     plt.xlim(data[0,0],data[-1,0])
     plt.ylim(fig_p.vertical)
     plt.plot(data[:,0], data[:,1:], color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     for i in range(len(calM)):
         plt.plot(calM[i][0],calM[i][1], label='%7.3f'%pltlabel[i])
     plt.ylabel('Energy (eV)')
-    plt.legend(frameon=False, loc='upper left', alignment='left', title='$LUMO$ & $HOMO$', title_fontproperties={'size':'medium'})
+    plt.legend(frameon=False, loc=location[1], alignment='left', title='$LUMO$ & $HOMO$', title_fontproperties={'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def plot2(data, calM_u, pltlabel_u, calM_d, pltlabel_d, ticks, labels, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['darkred', 'red']
     linestyle = fig_p.linestyle or [':', ':']
     linewidth = fig_p.linewidth or [0.8, 0.8]
+    location  = fig_p.location or [1, 2, 2]
     if len(color) == 1:
         color = [color[0], 'red']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], ':']
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
+    if len(location) < 3:
+        location += [2] * (3 - len(location))
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
-    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     if len(ticks) > 2:
         ticks[0],ticks[-1] = data[0,0,0],data[0,-1,0]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     ax1.set_xlim(data[0,0,0], data[0,-1,0])
     ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(data[1,0,0], data[1,-1,0])
     ax2.set_ylim(fig_p.vertical)
     if len(labels) > 0:
         ax1.set_xticks(ticks,labels[:-1]+[''])
     else:
@@ -148,11 +153,11 @@
     ax1.set_ylabel('Energy (eV)')
     ax1.plot(data[0,:,0], data[0,:,1:], color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(data[1,:,0], data[1,:,1:], color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     for i in range(len(calM_u)):
         ax1.plot(calM_u[i,0], calM_u[i,1], label='%7.3f'%pltlabel_u[i])
     for i in range(len(calM_d)):
         ax2.plot(calM_d[i,0], calM_d[i,1], label='%7.3f'%pltlabel_d[i])
-    ax1.legend(frameon=False, loc='upper left', alignment='left', title='$LUMO$ & $HOMO$', title_fontproperties={'size':'small'})
-    ax2.legend(frameon=False, loc='upper left', alignment='left', title='$LUMO$ & $HOMO$', title_fontproperties={'size':'small'})
+    ax1.legend(frameon=False, loc=location[1], alignment='left', title='$LUMO$ & $HOMO$', title_fontproperties={'size':'small'})
+    ax2.legend(frameon=False, loc=location[2], alignment='left', title='$LUMO$ & $HOMO$', title_fontproperties={'size':'small'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## bandplot/plots.py

```diff
@@ -3,39 +3,39 @@
 # bandplot
 
 def Noneispin(arr, bands, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
+    location  = fig_p.location  or [0]
     plt.plot(arr, bands.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     plt.xticks(ticks,labels)
-    plt.legend([legend[0]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.legend([legend[0]], frameon=False, prop={'size':'medium'}, loc=location[0])
     plt.xlim(arr[0], arr[-1])
     plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Noneispin2(arr, bands, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
-    linewidth = fig_p.linewidth or [0.8, 0.8]
+    linewidth = fig_p.linewidth + [0.8] * (2 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 2 else fig_p.linewidth
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-    if len(linewidth) == 1:
-        linewidth = [linewidth[0], 0.8]
     f = plt.plot(arr[0], bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
@@ -44,30 +44,29 @@
     plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     ax = plt.axes()
     g = ax.plot(arr[1], bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax.set_xlim(arr[1][0], arr[1][-1])
     ax.set_ylim(fig_p.vertical)
     ax.axis('off')
-    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
-    plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=location[1])
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Noneispin3(arr, bands, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k', 'b']
     linestyle = fig_p.linestyle or ['-', '-.', ':']
-    linewidth = fig_p.linewidth or [0.8, 0.8, 0.8]
+    linewidth = fig_p.linewidth + [0.8] * (3 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 3 else fig_p.linewidth
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     if len(color) < 3:
-        color = color + [''] * (3 - len(color))
+        color += [''] * (3 - len(color))
     if len(linestyle) < 3:
-        linestyle = linestyle + ['-'] * (3 - len(linestyle))
-    if len(linewidth) < 3:
-        linewidth = linewidth + [0.8] * (3 - len(linewidth))
+        linestyle += ['-'] * (3 - len(linestyle))
     f = plt.plot(arr[0], bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
@@ -81,33 +80,32 @@
     ax.set_ylim(fig_p.vertical)
     ax.axis('off')
     af = plt.axes()
     h = ax.plot(arr[2], bands[2].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     af.set_xlim(arr[2][0], arr[2][-1])
     af.set_ylim(fig_p.vertical)
     af.axis('off')
-    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
-    plt.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=location[1])
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Ispin(arr, bands, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
-    linewidth = fig_p.linewidth or [0.8, 0.8]
+    linewidth = fig_p.linewidth + [0.8] * (2 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 2 else fig_p.linewidth
+    location  = fig_p.location  or [0]
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-    if len(linewidth) == 1:
-        linewidth = [linewidth[0], 0.8]
     p_up = plt.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     p_do = plt.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    plt.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=fig_p.location,
+    plt.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=location[0],
                 alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
@@ -119,39 +117,36 @@
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Dispin(arr, bands, ticks, labels, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
-    linewidth = fig_p.linewidth or [0.8, 0.8]
+    linewidth = fig_p.linewidth + [0.8] * (2 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 2 else fig_p.linewidth
+    location  = fig_p.location + [0] * (3 - len(fig_p.location)) if len(fig_p.location) < 3 else fig_p.location
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-    if len(linewidth) == 1:
-        linewidth = [linewidth[0], 0.8]
     ax1.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
-    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=fig_p.location)
-    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=fig_p.location)
+    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=location[1])
+    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=location[2])
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
-
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     ax1.set_xlim(arr[0], arr[-1])
     ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(arr[0], arr[-1])
     ax2.set_ylim(fig_p.vertical)
     if len(labels) > 0:
         ax1.set_xticks(ticks,labels[:-1]+[''])
     else:
@@ -161,174 +156,161 @@
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Dispin2(arr, bands, ticks, labels, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'r', 'k', 'k']
     linestyle = fig_p.linestyle or ['-', '-', '-.', '-.']
-    linewidth = fig_p.linewidth or [0.8, 0.8, 0.8, 0.8]
+    linewidth = fig_p.linewidth + [0.8] * (4 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 4 else fig_p.linewidth
+    location  = fig_p.location + [0] * (3 - len(fig_p.location)) if len(fig_p.location) < 3 else fig_p.location
     if len(color) < 4:
-        color = color + [''] * (4 - len(color))
+        color += [''] * (4 - len(color))
     if len(linestyle) < 4:
-        linestyle = linestyle + ['-'] * (4 - len(linestyle))
-    if len(linewidth) < 4:
-        linewidth = linewidth + [0.8] * (4 - len(linewidth))
+        linestyle += ['-'] * (4 - len(linestyle))
     f1 = ax1.plot(arr[0], bands[0][0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     f2 = ax2.plot(arr[0], bands[0][1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
-
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     ax1.set_xlim(arr[0][0], arr[0][-1])
     ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(arr[0][0], arr[0][-1])
     ax2.set_ylim(fig_p.vertical)
     if len(labels) > 0:
         ax1.set_xticks(ticks,labels[:-1]+[''])
     else:
         ax1.set_xticks(ticks,labels)
     ax2.set_xticks(ticks,labels)
     ax1.set_ylabel('Energy (eV)')
-
     ax1_f = fig.add_subplot(1,2,1)
     g1 = ax1_f.plot(arr[1], bands[1][0].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     ax1_f.set_xlim(arr[1][0], arr[1][-1])
     ax1_f.set_ylim(fig_p.vertical)
     ax1_f.axis('off')
     ax2_f = fig.add_subplot(1,2,2)
     g2 = ax2_f.plot(arr[1], bands[1][1].T, color=color[3], linewidth=linewidth[3], linestyle=linestyle[3])
     ax2_f.set_xlim(arr[1][0], arr[1][-1])
     ax2_f.set_ylim(fig_p.vertical)
     ax2_f.axis('off')
-
-    ax1.legend([f1[0], g1[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+    ax1.legend([f1[0], g1[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=location[1],
                 alignment='left', title='up', title_fontproperties={'style':'italic', 'size':'medium'})
-    ax2.legend([f2[0], g2[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+    ax2.legend([f2[0], g2[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=location[2],
                 alignment='left', title='down', title_fontproperties={'style':'italic', 'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Dispin3(arr, bands, ticks, labels, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'r', 'k', 'k', 'b', 'b']
     linestyle = fig_p.linestyle or ['-', '-', '-.', '-.', ':', ':']
-    linewidth = fig_p.linewidth or [0.8] * 6
+    linewidth = fig_p.linewidth + [0.8] * (6 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 6 else fig_p.linewidth
+    location  = fig_p.location + [0] * (3 - len(fig_p.location)) if len(fig_p.location) < 3 else fig_p.location
     if len(color) < 6:
-        color = color + [''] * (6 - len(color))
+        color += [''] * (6 - len(color))
     if len(linestyle) < 6:
-        linestyle = linestyle + ['-'] * (6 - len(linestyle))
-    if len(linewidth) < 6:
-        linewidth = linewidth + [0.8] * (6 - len(linewidth))
+        linestyle += ['-'] * (6 - len(linestyle))
     f1 = ax1.plot(arr[0], bands[0][0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     f2 = ax2.plot(arr[0], bands[0][1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
 
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     ax1.set_xlim(arr[0][0], arr[0][-1])
     ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(arr[0][0], arr[0][-1])
     ax2.set_ylim(fig_p.vertical)
     if len(labels) > 0:
         ax1.set_xticks(ticks,labels[:-1]+[''])
     else:
         ax1.set_xticks(ticks,labels)
     ax2.set_xticks(ticks,labels)
     ax1.set_ylabel('Energy (eV)')
-
     ax1_f = fig.add_subplot(1,2,1)
     g1 = ax1_f.plot(arr[1], bands[1][0].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     ax1_f.set_xlim(arr[1][0], arr[1][-1])
     ax1_f.set_ylim(fig_p.vertical)
     ax1_f.axis('off')
     ax2_f = fig.add_subplot(1,2,2)
     g2 = ax2_f.plot(arr[1], bands[1][1].T, color=color[3], linewidth=linewidth[3], linestyle=linestyle[3])
     ax2_f.set_xlim(arr[1][0], arr[1][-1])
     ax2_f.set_ylim(fig_p.vertical)
     ax2_f.axis('off')
-
     ax1_g = fig.add_subplot(1,2,1)
     h1 = ax1_f.plot(arr[2], bands[2][0].T, color=color[4], linewidth=linewidth[4], linestyle=linestyle[4])
     ax1_g.set_xlim(arr[2][0], arr[2][-1])
     ax1_g.set_ylim(fig_p.vertical)
     ax1_g.axis('off')
     ax2_g = fig.add_subplot(1,2,2)
     h2 = ax2_f.plot(arr[2], bands[2][1].T, color=color[5], linewidth=linewidth[5], linestyle=linestyle[5])
     ax2_g.set_xlim(arr[2][0], arr[2][-1])
     ax2_g.set_ylim(fig_p.vertical)
     ax2_g.axis('off')
-    ax1.legend([f1[0], g1[0], h1[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+    ax1.legend([f1[0], g1[0], h1[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=location[1],
                 alignment='left', title='up', title_fontproperties={'style':'italic', 'size':'medium'})
-    ax2.legend([f2[0], g2[0], h2[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+    ax2.legend([f2[0], g2[0], h2[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=location[2],
                 alignment='left', title='down', title_fontproperties={'style':'italic', 'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-fig_p.width_ratios, fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
-
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     ax1.plot(arr, bands.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = len(index_f)
     p_dos = []
     if num + 1 > len(color):
         color = color + [''] * (num + 1 - len(color))
-
     if num + 1 > len(linestyle):
         linestyle = linestyle + ['-'] * (num + 1 - len(linestyle))
-
     if num + 1 > len(linewidth):
         linewidth = linewidth + [0.8] * (num + 1 - len(linewidth))
-
     for i in range(num):
         if color[i+1]:
             p_dos += ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+1], alpha=fig_p.fill)
         else:
             p_dos += ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
-
-    ax1.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=fig_p.location)
+    ax1.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=location[0])
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.set_yticklabels([])
-    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Density of states", title_fontproperties={'size':'small'})
+    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=location[1],
+               alignment='left', title="Density of states", title_fontproperties={'size':'small'})
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axvline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i,linewidth=0.4,linestyle='-.',c='gray')
-
     ax1.set_xlim(arr[0], arr[-1])
     ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(fig_p.horizontal)
     ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels)
     ax2.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
@@ -336,57 +318,53 @@
 
 def IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-fig_p.width_ratios, fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
     linewidth = fig_p.linewidth or [0.8, 0.8]
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
     p_up = ax1.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     p_do = ax1.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    ax1.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'small'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'small'})
+    ax1.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'small'}, loc=location[0], alignment='left', title=legend[0], title_fontproperties={'size':'small'})
     num = len(index_f)
     p_dos = []
     if num + 2 > len(color):
-        color = color + [''] * (num + 2 - len(color))
-
+        color += [''] * (num + 2 - len(color))
     if num + 2 > len(linestyle):
-        linestyle = linestyle + ['-'] * (num + 2 - len(linestyle))
-
+        linestyle += ['-'] * (num + 2 - len(linestyle))
     if num + 2 > len(linewidth):
-        linewidth = linewidth + [0.8] * (num + 2 - len(linewidth))
-
+        linewidth += [0.8] * (num + 2 - len(linewidth))
     for i in range(num):
         if color[i+2]:
             p_dos += ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2], color=color[i+2])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
         else:
             p_dos += ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
-
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.axvline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
-    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Density of states", title_fontproperties={'size':'small'})
+    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=location[1], alignment='left', title="Density of states", title_fontproperties={'size':'small'})
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i,linewidth=0.4, linestyle='-.', c='gray')
-
     ax1.set_xlim(arr[0], arr[-1])
     ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(fig_p.horizontal)
     ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels)
     ax2.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
@@ -394,65 +372,60 @@
 
 def DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p):
     fig, (ax1, ax2, ax3) = plt.subplots(1, 3, width_ratios=[0.5*(1-fig_p.width_ratios), 0.5*(1-fig_p.width_ratios), fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
     linewidth = fig_p.linewidth or [0.8, 0.8]
+    location  = fig_p.location + [0] * (4 - len(fig_p.location)) if len(fig_p.location) < 4 else fig_p.location
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
     ax1.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'small'})
+    L = ax1.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'small'})
     ax1.add_artist(L)
-    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'small'}, loc=fig_p.location)
-    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'small'}, loc=fig_p.location)
+    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'small'}, loc=location[1])
+    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'small'}, loc=location[2])
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax3.minorticks_on()
     ax3.tick_params(axis='both', which='minor', color='gray')
     num = len(index_f)
     p_dos = []
     if num + 2 > len(color):
-        color = color + [''] * (num + 2 - len(color))
-
+        color += [''] * (num + 2 - len(color))
     if num + 2 > len(linestyle):
-        linestyle = linestyle + ['-'] * (num + 2 - len(linestyle))
-
+        linestyle += ['-'] * (num + 2 - len(linestyle))
     if num + 2 > len(linewidth):
-        linewidth = linewidth + [0.8] * (num + 2 - len(linewidth))
-
+        linewidth += [0.8] * (num + 2 - len(linewidth))
     for i in range(num):
         if color[i+2]:
             p_dos += ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2], color=color[i+2])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
         else:
             p_dos += ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
-
     ax3.axvline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     ax3.set_yticklabels([])
-    ax3.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Density of states", title_fontproperties={'size':'small'})
-
+    ax3.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=location[3], alignment='left', title="Density of states", title_fontproperties={'size':'small'})
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax3.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i,linewidth=0.4,linestyle='-.',c='gray')
             ax2.axvline(i,linewidth=0.4,linestyle='-.',c='gray')
-
     ax1.set_xlim(arr[0], arr[-1])
     ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(arr[0], arr[-1])
     ax2.set_ylim(fig_p.vertical)
     ax3.set_xlim(fig_p.horizontal)
     ax3.set_ylim(fig_p.vertical)
     if len(labels) > 0:
@@ -469,34 +442,31 @@
     plt.minorticks_on()
     plt.tick_params(axis='both', which='minor', color='gray')
     num = len(index_f)
     p_dos = []
     color = fig_p.color
     linestyle = fig_p.linestyle
     linewidth = fig_p.linewidth
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     if num > len(color):
-        color = color + [''] * (num - len(color))
-
+        color += [''] * (num - len(color))
     if num > len(linestyle):
-        linestyle = linestyle + ['-'] * (num - len(linestyle))
-
+        linestyle += ['-'] * (num - len(linestyle))
     if num > len(linewidth):
-        linewidth = linewidth + [0.8] * (num - len(linewidth))
-
+        linewidth += [0.8] * (num - len(linewidth))
     if fig_p.exchange:
         for i in range(num):
             if color[i]:
                 p_dos += plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
                 if fig_p.fill:
                     plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, color=color[i], alpha=fig_p.fill)
             else:
                 p_dos += plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i])
                 if fig_p.fill:
                     plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, alpha=fig_p.fill)
-
         plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
         plt.xlim(fig_p.vertical)
         plt.ylim(fig_p.horizontal)
         plt.xlabel('Energy (eV)')
         plt.ylabel('Density of states, electrons/eV')
     else:
         for i in range(num):
@@ -504,21 +474,19 @@
                 p_dos += plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i], color=color[i])
                 if fig_p.fill:
                     plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i], alpha=fig_p.fill)
             else:
                 p_dos += plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i])
                 if fig_p.fill:
                     plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
-
         plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
         plt.ylim(fig_p.vertical)
         plt.xlim(fig_p.horizontal)
         plt.ylabel('Energy (eV)')
         plt.xlabel('Density of states, electrons/eV')
-
-    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=location[1])
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## bandplot/pplots.py

```diff
@@ -4,14 +4,15 @@
 
 def Broken(arr, fre, ticks, labels, broken, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[fig_p.height_ratio, 1-fig_p.height_ratio], figsize=fig_p.size)
     fig.subplots_adjust(hspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
+    location  = fig_p.location  or [0]
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.xlim(arr[0], arr[-1])
     vertical = fig_p.vertical or plt.ylim()
     ax1.set_ylim(broken[1], vertical[1])
     ax2.set_ylim(vertical[0], broken[0])
     ax1.spines['bottom'].set_visible(False)
@@ -23,35 +24,34 @@
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
-    ax2.legend([legend[0]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    ax2.legend([legend[0]], frameon=False, prop={'size':'medium'}, loc=location[0])
     plt.xticks(ticks,labels)
     plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
     kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
                   linestyle='', color='k', mec='k', mew=1, clip_on=False)
     ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
     ax2.plot([0, 1], [0.98, 0.98], transform=ax2.transAxes, **kwargs)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Broken2(arr, fre, ticks, labels, broken, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[fig_p.height_ratio, 1-fig_p.height_ratio], figsize=fig_p.size)
     fig.subplots_adjust(hspace=0.0)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
-    linewidth = fig_p.linewidth or [0.8, 0.8]
+    linewidth = fig_p.linewidth + [0.8] * (2 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 2 else fig_p.linewidth
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-    if len(linewidth) == 1:
-        linewidth = [linewidth[0], 0.8]
     ax1.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     f = ax2.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.xlim(arr[0][0], arr[0][-1])
     vertical = fig_p.vertical or plt.ylim()
     ax1.set_ylim(broken[1], vertical[1])
     ax2.set_ylim(vertical[0], broken[0])
     ax1.spines['bottom'].set_visible(False)
@@ -62,50 +62,46 @@
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     plt.xticks(ticks,labels)
     plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
     kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
                   linestyle='', color='k', mec='k', mew=1, clip_on=False)
     ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
     ax2.plot([0, 1], [0.98, 0.98], transform=ax2.transAxes, **kwargs)
-
     ax1_f = fig.add_subplot(2,1,1)
     ax1_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax1_f.set_xlim(arr[1][0], arr[1][-1])
     ax1_f.set_ylim(broken[1], vertical[1])
     ax1_f.axis('off')
     ax2_f = fig.add_subplot(2,1,2)
     g = ax2_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax2_f.set_xlim(arr[1][0], arr[1][-1])
     ax2_f.set_ylim(vertical[0], broken[0])
     ax2_f.axis('off')
-
-    L = ax2.legend([], frameon=False, loc='best', bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax2.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax2.add_artist(L)
-    ax2.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    ax2.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=location[1])
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Broken3(arr, fre, ticks, labels, broken, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[fig_p.height_ratio, 1-fig_p.height_ratio], figsize=fig_p.size)
     fig.subplots_adjust(hspace=0.0)
     color = fig_p.color or ['r', 'k', 'b']
     linestyle = fig_p.linestyle or ['-', '-.', ':']
-    linewidth = fig_p.linewidth or [0.8] * 3
+    linewidth = fig_p.linewidth + [0.8] * (3 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 3 else fig_p.linewidth
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     if len(color) < 3:
-        color = color + [''] * (3 - len(color))
+        color += [''] * (3 - len(color))
     if len(linestyle) < 3:
-        linestyle = linestyle + ['-'] * (3 - len(linestyle))
-    if len(linewidth) < 3:
-        linewidth = linewidth + [0.8] * (3 - len(linewidth))
+        linestyle += ['-'] * (3 - len(linestyle))
     ax1.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     f = ax2.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.xlim(arr[0][0], arr[0][-1])
     vertical = fig_p.vertical or plt.ylim()
     ax1.set_ylim(broken[1], vertical[1])
     ax2.set_ylim(vertical[0], broken[0])
     ax1.spines['bottom'].set_visible(False)
@@ -116,180 +112,165 @@
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     plt.xticks(ticks,labels)
     plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
     kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
                   linestyle='', color='k', mec='k', mew=1, clip_on=False)
     ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
     ax2.plot([0, 1], [0.98, 0.98], transform=ax2.transAxes, **kwargs)
-
     ax1_f = fig.add_subplot(2,1,1)
     ax1_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax1_f.set_xlim(arr[1][0], arr[1][-1])
     ax1_f.set_ylim(broken[1], vertical[1])
     ax1_f.axis('off')
     ax2_f = fig.add_subplot(2,1,2)
     g = ax2_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax2_f.set_xlim(arr[1][0], arr[1][-1])
     ax2_f.set_ylim(vertical[0], broken[0])
     ax2_f.axis('off')
-
     ax1_g = fig.add_subplot(2,1,1)
     ax1_g.plot(arr[2], fre[2].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     ax1_g.set_xlim(arr[2][0], arr[2][-1])
     ax1_g.set_ylim(broken[1], vertical[1])
     ax1_g.axis('off')
     ax2_g = fig.add_subplot(2,1,2)
     h = ax2_g.plot(arr[2], fre[2].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     ax2_g.set_xlim(arr[2][0], arr[2][-1])
     ax2_g.set_ylim(vertical[0], broken[0])
     ax2_g.axis('off')
-
-    L = ax2.legend([], frameon=False, loc='best', bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax2.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax2.add_artist(L)
-    ax2.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    ax2.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=location[1])
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Nobroken(arr, fre, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
+    location  = fig_p.location  or [0]
     plt.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
-    plt.legend([legend[0]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.legend([legend[0]], frameon=False, prop={'size':'medium'}, loc=location[0])
     plt.xticks(ticks,labels)
     plt.xlim(arr[0], arr[-1])
     plt.ylim(fig_p.vertical)
     plt.ylabel('Frequency (THz)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Nobroken2(arr, fre, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
-    linewidth = fig_p.linewidth or [0.8, 0.8]
+    linewidth = fig_p.linewidth + [0.8] * (2 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 2 else fig_p.linewidth
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-    if len(linewidth) == 1:
-        linewidth = [linewidth[0], 0.8]
     f = plt.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     plt.xticks(ticks,labels)
     plt.xlim(arr[0][0], arr[0][-1])
     ylim=plt.ylim(fig_p.vertical)
     plt.ylabel('Frequency (THz)')
     ax = plt.axes()
     g = ax.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax.set_xlim(arr[1][0], arr[1][-1])
     ax.set_ylim(ylim)
     ax.axis('off')
-
-    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
-    plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=location[1])
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Nobroken3(arr, fre, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k', 'b']
     linestyle = fig_p.linestyle or ['-', '-.', ':']
-    linewidth = fig_p.linewidth or [0.8] * 3
+    linewidth = fig_p.linewidth + [0.8] * (3 - len(fig_p.linewidth)) if len(fig_p.linewidth) < 3 else fig_p.linewidth
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     if len(color) < 3:
-        color = color + [''] * (3 - len(color))
+        color += [''] * (3 - len(color))
     if len(linestyle) < 3:
-        linestyle = linestyle + ['-'] * (3 - len(linestyle))
-    if len(linewidth) < 3:
-        linewidth = linewidth + [0.8] * (3 - len(linewidth))
+        linestyle += ['-'] * (3 - len(linestyle))
     f = plt.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     plt.xticks(ticks,labels)
     plt.xlim(arr[0][0], arr[0][-1])
     ylim=plt.ylim(fig_p.vertical)
     plt.ylabel('Frequency (THz)')
     ax = plt.axes()
     g = ax.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax.set_xlim(arr[1][0], arr[1][-1])
     ax.set_ylim(ylim)
     ax.axis('off')
-
     af = plt.axes()
     h = af.plot(arr[2], fre[2].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     af.set_xlim(arr[2][0], arr[2][-1])
     af.set_ylim(ylim)
     af.axis('off')
-
-    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
-    plt.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=location[1])
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 
 def BrokenWd(arr, fre, ticks, labels, broken, darr, dele, elements, legend, fig_p):
     fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2, height_ratios=[fig_p.height_ratio, 1-fig_p.height_ratio],
                                                  width_ratios=[1-fig_p.width_ratios, fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0, hspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax3.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = dele.shape[-1]
     p_dos = []
     if num + 1 > len(color):
-        color = color + [''] * (num - len(color) + 1)
-
+        color += [''] * (num - len(color) + 1)
     if num + 1 > len(linestyle):
-        linestyle = linestyle + ['-'] * (num - len(linestyle) + 1)
-
+        linestyle += ['-'] * (num - len(linestyle) + 1)
     if num + 1 > len(linewidth):
-        linewidth = linewidth + [0.8] * (num - len(linewidth) + 1)
-
+        linewidth += [0.8] * (num - len(linewidth) + 1)
     for i in range(num):
         if color[i+1]:
             ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
             p_dos = p_dos + ax4.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
             if fig_p.fill:
                 plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
         else:
             ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             p_dos = p_dos + ax4.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             if fig_p.fill:
                 plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
-
     ax1.set_xlim(arr[0], arr[-1])
     ax3.set_xlim(arr[0], arr[-1])
     vertical = fig_p.vertical or ax1.get_ylim()
-
     ax1.set_ylim(broken[1], vertical[1])
     ax2.set_ylim(broken[1], vertical[1])
     ax3.set_ylim(vertical[0], broken[0])
     ax4.set_ylim(vertical[0], broken[0])
     ax2.set_xlim(fig_p.horizontal)
     ax4.set_xlim(fig_p.horizontal)
     ax1.spines['bottom'].set_visible(False)
@@ -316,24 +297,22 @@
     if num > len(elements):
         elements = elements + [''] * (num - len(elements))
     elif num < len(elements):
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
-
-    ax3.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=fig_p.location)
-    ax4.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location,
+    ax3.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=location[0])
+    ax4.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=location[1],
                alignment='left', title="Phonon DOS", title_fontproperties={'size':'small'})
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax3.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     ax3.set_xticks(ticks,labels)
     plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
     kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
                   linestyle='', color='k', mec='k', mew=1, clip_on=False)
     ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
     ax3.plot([0, 1], [0.98, 0.98], transform=ax3.transAxes, **kwargs)
     ax2.plot(1, 0.02, transform=ax2.transAxes, **kwargs)
@@ -342,39 +321,35 @@
 
 def NobrokenWd(arr, fre, ticks, labels, darr, dele, elements, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-fig_p.width_ratios, fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = dele.shape[-1]
     p_dos = []
     if num + 1 > len(color):
-        color = color + [''] * (num - len(color) + 1)
-
+        color += [''] * (num - len(color) + 1)
     if num + 1 > len(linestyle):
-        linestyle = linestyle + ['-'] * (num - len(linestyle) + 1)
-
+        linestyle += ['-'] * (num - len(linestyle) + 1)
     if num + 1 > len(linewidth):
-        linewidth = linewidth + [0.8] * (num - len(linewidth) + 1)
-
+        linewidth += [0.8] * (num - len(linewidth) + 1)
     for i in range(num):
         if color[i+1]:
             p_dos = p_dos + ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
             if fig_p.fill:
                 plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
         else:
             p_dos = p_dos + ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             if fig_p.fill:
                 plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
-
     ax1.set_xlim(arr[0], arr[-1])
     vertical = fig_p.vertical or ax1.get_ylim()
-
     ax1.set_ylim(vertical)
     ax2.set_ylim(vertical)
     ax2.set_xlim(fig_p.horizontal)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='x', labelsize='small', labelcolor='dimgray', labelrotation=-90, pad=3)
@@ -384,57 +359,52 @@
     if num > len(elements):
         elements = elements + [''] * (num - len(elements))
     elif num < len(elements):
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
-
-    ax1.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=fig_p.location)
+    ax1.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=location[0])
     ax2.axvline(linewidth=0.4,linestyle='-.',c='dimgray')
-    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location,
+    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=location[1],
                alignment='left', title="Phonon DOS", title_fontproperties={'size':'small'})
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     ax1.set_xticks(ticks,labels)
     ax1.set_ylabel('Frequency (THz)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def dosfile(darr, dele, elements, legend, fig_p):
+def pdosfile(darr, dele, elements, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     plt.minorticks_on()
     plt.tick_params(axis='both', which='minor', color='gray')
     num = dele.shape[-1]
     color = fig_p.color
     linestyle = fig_p.linestyle
     linewidth = fig_p.linewidth
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     p_dos = []
     if num > len(color):
-        color = color + [''] * (num - len(color))
-
+        color += [''] * (num - len(color))
     if num > len(linestyle):
-        linestyle = linestyle + ['-'] * (num - len(linestyle))
-
+        linestyle += ['-'] * (num - len(linestyle))
     if num > len(linewidth):
-        linewidth = linewidth + [0.8] * (num - len(linewidth))
-
+        linewidth += [0.8] * (num - len(linewidth))
     if fig_p.exchange:
         for i in range(num):
             if color[i]:
                 p_dos = p_dos + plt.plot(darr, dele[:,i], linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
                 if fig_p.fill:
                     plt.fill_between(darr, dele[:,i], 0, color=color[i], alpha=fig_p.fill)
             else:
                 p_dos = p_dos + plt.plot(darr, dele[:,i], linewidth=linewidth[i], linestyle=linestyle[i])
                 if fig_p.fill:
                     plt.fill_between(darr, dele[:,i], 0, alpha=fig_p.fill)
-
         plt.xlim(fig_p.vertical)
         plt.ylim(fig_p.horizontal)
         plt.xlabel('Frequency (THz)')
         plt.ylabel('Phonon DOS')
         plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
     else:
         for i in range(num):
@@ -442,28 +412,25 @@
                 p_dos = p_dos + plt.plot(dele[:,i], darr, linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
                 if fig_p.fill:
                     plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
             else:
                 p_dos = p_dos + plt.plot(dele[:,i], darr, linewidth=linewidth[i], linestyle=linestyle[i])
                 if fig_p.fill:
                     plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
-
         plt.ylim(fig_p.vertical)
         plt.xlim(fig_p.horizontal)
         plt.ylabel('Frequency (THz)')
         plt.xlabel('Phonon DOS')
         plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
-
     plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if num > len(elements):
         elements = elements + [''] * (num - len(elements))
     elif num < len(elements):
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
-
-    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=location[0],
                alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## bandplot/projected.py

```diff
@@ -101,20 +101,21 @@
     return index_f, labels_elements
 
 def pplot(darr, dbands, composition, ticks, labels, index_f, elements, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['dimgray', 'b']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.1]
+    location  = fig_p.location + [0] * (2 - len(fig_p.location)) if len(fig_p.location) < 2 else fig_p.location
     num = len(index_f)
     if len(color) == 1:
         color = [color[0], 'b']
 
     plt.plot(darr[0], dbands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = darr[0][0],darr[0][-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
@@ -132,23 +133,24 @@
         else:
             compositions += composition[index_f[i][0]][index_f[i][1]]
             elem = elem + '\n' + elements[i]
     n = bands.shape[0]
     p = [''] * n
     for x in range(n):
         p[x] = plt.scatter(darr[0], bands[x,:], compositions[x,:] * 20, color=color[1], marker='o', facecolor='none', linewidth=0.4)
-    plt.legend([p[0]], [elem], frameon=False, prop={'size':'medium'}, loc=fig_p.location, markerfirst=False, markerscale=1.5)
+    plt.legend([p[0]], [elem], frameon=False, prop={'size':'medium'}, loc=location[1], markerfirst=False, markerscale=1.5)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def pplot2(darr, dbands, composition, ticks, labels, index_f, elements, ispin, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['dimgray', 'darkblue', 'b', 'r']
     linestyle = fig_p.linestyle or ['-'] * 2
     linewidth = fig_p.linewidth or [0.1] * 2
+    location  = fig_p.location + [0] * (3 - len(fig_p.location)) if len(fig_p.location) < 3 else fig_p.location
     num = len(index_f)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     if len(ticks) > 2:
@@ -162,15 +164,15 @@
     ax2.set_ylim(fig_p.vertical)
     if len(labels) > 0:
         ax1.set_xticks(ticks,labels[:-1]+[''])
     else:
         ax1.set_xticks(ticks,labels)
     ax2.set_xticks(ticks,labels)
     ax1.set_ylabel('Energy (eV)')
-    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc=location[0], bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     m = len(elements)
     elements =  elements + [''] * (num - m) if m < num else elements[:num]
     ax1_p = True
     ax2_p = True
     for i in range(num):
         if ispin[i] == 1:
@@ -196,11 +198,11 @@
     o = [''] * m
     ax1.plot(darr[0], bands_u.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(darr[0], bands_d.T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     for x in range(n):
         p[x] = ax1.scatter(darr[0], bands_u[x,:], compositions_u[x,:] * 20, color=color[2], marker='o', facecolor='none', linewidth=0.4)
     for x in range(m):
         o[x] = ax2.scatter(darr[0], bands_d[x,:], compositions_d[x,:] * 20, color=color[3], marker='o', facecolor='none', linewidth=0.4)
-    ax1.legend([p[0]], [elem1], frameon=False, prop={'size':'small'}, loc=fig_p.location, markerfirst=False, markerscale=1.5)
-    ax2.legend([o[0]], [elem2], frameon=False, prop={'size':'small'}, loc=fig_p.location, markerfirst=False, markerscale=1.5)
+    ax1.legend([p[0]], [elem1], frameon=False, prop={'size':'small'}, loc=location[1], markerfirst=False, markerscale=1.5)
+    ax2.legend([o[0]], [elem2], frameon=False, prop={'size':'small'}, loc=location[2], markerfirst=False, markerscale=1.5)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## bandplot/wrapper.py

```diff
@@ -21,47 +21,53 @@
     parser = argparse.ArgumentParser(description='Plot the band structure or DOS from vaspkit result.',
                                      epilog='''
 Example:
 bandplot -i BAND.dat -o BAND.png -l g m k g -d PDOS* -z -p C-s,p Ti-d
 ''',
     formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
-    parser.add_argument('-s', "--size",       type=int,   nargs=2,  help='figure size: width, height')
+    parser.add_argument('-s', "--size",       type=int,   nargs=2,  help='figure size: width, height', metavar=('width','height'))
     parser.add_argument('-b', "--divided",    action='store_true',  help="plot the up and down spin in divided subplot")
-    parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="energy (eV) range, default: [-5.0, 5.0]")
+    parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="energy (eV) range, default: [-5.0, 5.0]", metavar=('start','end'))
     parser.add_argument('-g', "--legend",     type=str,             nargs='+', help="legend labels", default=[])
-    parser.add_argument('-L', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
-                                                                             'center left', 'center right', 'lower center', 'upper center', 'center'],
-                                                                    help="arrange the legend location, default: best", default='best')
+    parser.add_argument('-a', "--location",   type=str.lower,       nargs='+', help="arrange the legend location, default: best", default=[], metavar="str")
     parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
-                                                                                    "k, black; w, white", default=[])
+                                                                                    "k, black; w, white", default=[], metavar="color")
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
-                                                                                    default=[])
-    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
-    parser.add_argument('-m', "--mass",       type=float,           nargs='*', help='calculate the effective masses, default: 0.15', default=None)
+                                                                                    default=[], metavar="str")
+    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[], metavar="0.8")
+    parser.add_argument('-m', "--mass",       type=float,           nargs='?', help='calculate the effective masses, default: 0.15', default=None, const=0.15,
+                                                                                    metavar="scale")
     parser.add_argument('-r', "--projected",  action='store_true',  help='plot the projected band structure')
     parser.add_argument('-i', "--input",      type=str,             nargs='+', help="plot figure from .dat file, default: BAND.dat", default=["BAND.dat"])
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-j', "--klabels",    type=str,             help="filename of KLABELS, default: KLABELS", default="KLABELS")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
-    parser.add_argument('-d', "--dos",        type=str,             nargs='+', default=[], help="plot DOS from .dat file, or file list")
-    parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
+    parser.add_argument('-d', "--dos",        type=str,             nargs='*', default=None, help="plot DOS from .dat file, or file list")
+    parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range", metavar=('start','end'))
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
     parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d, or symbol-s,p,d')
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-W', "--wratios",    type=float,           help='width ratio for DOS subplot')
-    parser.add_argument('-z', "--fill",       type=float,           nargs='*', help='fill a shaded region between PDOS and axis, default: 0.2', default=None)
+    parser.add_argument('-z', "--fill",       type=float,           nargs='?', help='fill a shaded region between PDOS and axis, default: 0.2', default=None,
+                                                                                    const=0.2, metavar="alpha")
     parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
-    dosfiles = [f for i in args.dos for f in glob.glob(i)]
+    if args.dos is not None:
+        if args.dos == []:
+            dosfiles = [f for f in glob.glob('PDOS*.dat')] or [f for f in glob.glob('TDOS.dat')]
+        else:
+            dosfiles = [f for i in args.dos for f in glob.glob(i)]
+    else:
+        dosfiles = None
 
     color = []
     for i in args.color:
         j = i.split('*')
         if len(j) == 2:
             color += [ast.literal_eval(j[0])] * int(j[1]) if '(' in j[0] and ')' in j[0] else [j[0]] * int(j[1])
         else:
@@ -101,28 +107,29 @@
     if os.path.exists(args.klabels):
         ticks, klabels = readdata.klabels(args.klabels)
 
     if len(labels) == 0:
         labels=[re.sub('GAMMA|Gamma|G', 'Γ', re.sub('Undefined|Un|[0-9]', '', i)) for i in klabels]
 
     if len(ticks) > len(labels):
-        labels = labels + [''] * (len(ticks) - len(labels))
+        labels += [''] * (len(ticks) - len(labels))
     elif len(ticks) < len(labels):
         labels = labels[:len(ticks)]
 
     width_ratios = args.wratios or (0.3 if args.divided else 0.5)
+    location = [int(i) if i.isdigit() else i for i in args.location]
 
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
-                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi,
+                    color=color, linestyle=linestyle, linewidth=linewidth, location=location, dpi=args.dpi,
                     width_ratios=width_ratios, exchange=args.exchange, fill=args.fill)
 # calculate the effective masses
     if args.mass is not None:
         if not fig_p.vertical:
             fig_p.vertical = [-5.0, 5.0]
-        scale = 0.15 if args.mass == [] else args.mass[0]
+        scale = 0.15 if args.mass > 0.75 or args.mass < 0.05 else args.mass
         from bandplot import mass
         if os.path.exists("BAND_GAP"):
             lumo, homo, homo_c, filename = mass.get_vbm_cbm("BAND_GAP")
             Extension = [len(lumo), len(homo), len(homo_c), len(filename)]
             if all(x == 1 for x in Extension):
                 data = mass.bs_dat_read(filename)
                 calM = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], scale)
@@ -195,17 +202,14 @@
                 elif ispin == "Ispin" and args.divided:
                     plots.Dispin(arr, bands, ticks, labels, legend, fig_p)
             else:
                 darr, dele, s_elements = readdata.dos(args.dos)
                 index_f, labels_elements = readdata.select(s_elements, args.partial)
                 if not elements:
                     elements = labels_elements
-                if fig_p.fill is not None:
-                    fig_p.fill = 0.2 if fig_p.fill == [] else fig_p.fill[0]
-
                 if ispin == "Noneispin":
                     plots.NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
                 elif ispin == "Ispin" and not args.divided:
                     plots.IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
                 elif ispin == "Ispin" and args.divided:
                     plots.DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
 # plot DOS
@@ -213,17 +217,14 @@
             if dosfiles:
                 if fig_p.output == "BAND.png":
                     fig_p.output = "DOS.png"
                 darr, dele, s_elements = readdata.dos(dosfiles)
                 index_f, labels_elements = readdata.select(s_elements, args.partial)
                 if not elements:
                     elements = labels_elements
-                if fig_p.fill is not None:
-                    fig_p.fill = 0.2 if fig_p.fill == [] else fig_p.fill[0]
-
                 plots.pdosfiles(darr, dele, index_f, elements, legend, fig_p)
             else:
                 print("ERROR: No *.dat file.")
 # compare two Band Structures
         elif len_bandfile == 2:
             if not fig_p.vertical:
                 fig_p.vertical = [-5.0, 5.0]
@@ -264,44 +265,49 @@
     parser = argparse.ArgumentParser(description='Plot the phonon band structure or DOS from phonopy results.',
                                      epilog='''
 Example:
 pbandplot -i BAND.dat -o BAND.png -l g m k g -d projected_dos.dat -g \$\\pi^2_4\$ -e Si C O
 ''',
     formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
-    parser.add_argument('-s', "--size",       type=float, nargs=2,  help='figure size: width, height')
+    parser.add_argument('-s', "--size",       type=float, nargs=2,  help='figure size: width, height', metavar=('width','height'))
     parser.add_argument('-b', "--broken",     type=float, nargs=2,  help='broken axis: start, end')
     parser.add_argument('-H', "--hratios",    type=float,           help='height ratio for broken axis, default: 0.2', default=0.2)
-    parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="frequency (THz) range")
+    parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="frequency (THz) range", metavar=('start','end'))
     parser.add_argument('-g', "--legend",     type=str,             nargs='+', help="legend labels", default=[])
-    parser.add_argument('-L', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
-                                                                             'center left', 'center right', 'lower center', 'upper center', 'center'],
-                                                                    help="arrange the legend location, default: best", default='best')
+    parser.add_argument('-a', "--location",   type=str.lower,       nargs='+', help="arrange the legend location, default: best", default=[], metavar="str")
     parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
-                                                                                    "k, black; w, white", default=[])
+                                                                                    "k, black; w, white", default=[], metavar="color")
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
-                                                                                    default=[])
-    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
+                                                                                    default=[], metavar="str")
+    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[], metavar="0.8")
     parser.add_argument('-i', "--input",      type=str,             nargs='+', help="plot figure from .dat file, default: BAND.dat", default=["BAND.dat"])
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-j', "--bandconf",   type=str,             help="filename of band setting file, default: band.conf", default="band.conf")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
-    parser.add_argument('-d', "--dos",        type=str,             help="plot Phonon DOS from .dat file")
-    parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Phonon density of states range")
+    parser.add_argument('-d', "--dos",        type=str,             nargs='?', default='', help="plot Phonon DOS from .dat file")
+    parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Phonon density of states range", metavar=('start','end'))
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of Phonon DOS")
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-W', "--wratios",    type=float,           help='width ratio for DOS subplot, default 0.5', default=0.5)
-    parser.add_argument('-z', "--fill",       type=float,           nargs='*', help='fill a shaded region between PDOS and axis, default: 0.2', default=None)
+    parser.add_argument('-z', "--fill",       type=float,           nargs='?', help='fill a shaded region between PDOS and axis, default: 0.2', default=None,
+                                                                                    const=0.2, metavar="alpha")
     parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
+    if args.dos != '':
+        dosfile = args.dos or ('projected_dos.dat' if os.path.exists('projected_dos.dat') else '') or ('total_dos.dat' if os.path.exists('total_dos.dat') else '')
+        dosfile = dosfile if os.path.exists(dosfile) else None
+    else:
+        dosfile = None
+
     color = []
     for i in args.color:
         j = i.split('*')
         if len(j) == 2:
             color += [ast.literal_eval(j[0])] * int(j[1]) if '(' in j[0] and ')' in j[0] else [j[0]] * int(j[1])
         else:
             color += [ast.literal_eval(i)] if '(' in i and ')' in i else [i]
@@ -345,83 +351,80 @@
         klabels = readdata.bandset(args.bandconf)
     if len(labels) == 0:
         labels=[re.sub('^GA[A-Z]+$|^G$', 'Γ', i) for i in klabels]
 
     broken = args.broken
     height_ratio = args.hratios if 0 < args.hratios < 1 else 0.2
     width_ratios = args.wratios if 0 < args.wratios < 1 else 0.5
+    location = [int(i) if i.isdigit() else i for i in args.location]
 
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
-                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi,
+                    color=color, linestyle=linestyle, linewidth=linewidth, location=location, dpi=args.dpi,
                     height_ratio=height_ratio, width_ratios=width_ratios, exchange=args.exchange, fill=args.fill)
 # plot Phonon Band Structure
     bandfile = [f for i in args.input for f in glob.glob(i)]
     len_bandfile = len(bandfile)
     if len_bandfile == 1:
         arr, fre, ticks = readdata.pbands(bandfile[0])
         if len(ticks) > len(labels):
-            labels = labels + [''] * (len(ticks) - len(labels))
+            labels += [''] * (len(ticks) - len(labels))
         elif len(ticks) < len(labels):
             labels = labels[:len(ticks)]
-        if args.dos is None:
-            if args.broken is None:
-                pplots.Nobroken(arr, fre, ticks, labels, legend, fig_p)
-            else:
-                pplots.Broken(arr, fre, ticks, labels, broken, legend, fig_p)
-        elif os.path.exists(args.dos):
-            darr, dele = readdata.pdos(args.dos)
-            if fig_p.fill is not None:
-                fig_p.fill = 0.2 if fig_p.fill == [] else fig_p.fill[0]
+        if dosfile:
+            darr, dele = readdata.pdos(dosfile)
             if args.broken is None:
                 pplots.NobrokenWd(arr, fre, ticks, labels, darr, dele, elements, legend, fig_p)
             else:
                 pplots.BrokenWd(arr, fre, ticks, labels, broken, darr, dele, elements, legend, fig_p)
+        else:
+            if args.broken is None:
+                pplots.Nobroken(arr, fre, ticks, labels, legend, fig_p)
+            else:
+                pplots.Broken(arr, fre, ticks, labels, broken, legend, fig_p)
 # plot Phonon DOS
     elif len_bandfile == 0:
-        if args.dos and os.path.exists(args.dos):
+        if dosfile:
             if fig_p.output == "BAND.png":
                     fig_p.output = "DOS.png"
-            darr, dele = readdata.pdos(args.dos)
-            if fig_p.fill is not None:
-                fig_p.fill = 0.2 if fig_p.fill == [] else fig_p.fill[0]
-            pplots.dosfile(darr, dele, elements, legend, fig_p)
+            darr, dele = readdata.pdos(dosfile)
+            pplots.pdosfile(darr, dele, elements, legend, fig_p)
         else:
             print('No *.dat file.')
 # compare two Phonon Band Structures
     elif len_bandfile == 2:
         arr = [''] * 2
         fre = [''] * 2
         ticks = [''] * 2
         arr[0], fre[0], ticks[0] = readdata.pbands(bandfile[0])
         arr[1], fre[1], ticks[1] = readdata.pbands(bandfile[1])
         if len(ticks[0]) > len(labels):
-            labels = labels + [''] * (len(ticks[0]) - len(labels))
+            labels += [''] * (len(ticks[0]) - len(labels))
         elif len(ticks[0]) < len(labels):
             labels = labels[:len(ticks[0])]
         if len(legend) < 3:
-            legend = legend + [''] * (3 - len(legend))
+            legend += [''] * (3 - len(legend))
 
         if args.broken is None:
             pplots.Nobroken2(arr, fre, ticks[0], labels, legend, fig_p)
         else:
             pplots.Broken2(arr, fre, ticks[0], labels, broken, legend, fig_p)
 # compare three Phonon Band Structures
     elif len_bandfile == 3:
         arr = [''] * 3
         fre = [''] * 3
         ticks = [''] * 3
         arr[0], fre[0], ticks[0] = readdata.pbands(bandfile[0])
         arr[1], fre[1], ticks[1] = readdata.pbands(bandfile[1])
         arr[2], fre[2], ticks[2] = readdata.pbands(bandfile[2])
         if len(ticks[0]) > len(labels):
-            labels = labels + [''] * (len(ticks[0]) - len(labels))
+            labels += [''] * (len(ticks[0]) - len(labels))
         elif len(ticks[0]) < len(labels):
             labels = labels[:len(ticks[0])]
         if len(legend) < 4:
-            legend = legend + [''] * (4 - len(legend))
+            legend += [''] * (4 - len(legend))
 
         if args.broken is None:
             pplots.Nobroken3(arr, fre, ticks[0], labels, legend, fig_p)
         else:
             pplots.Broken3(arr, fre, ticks[0], labels, broken, legend, fig_p)
     else:
         print("Input file mismatch.")
```

## Comparing `bandplot-0.1.5.3.dist-info/METADATA` & `bandplot-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.5.3
+Version: 0.1.6
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
```

## Comparing `bandplot-0.1.5.3.dist-info/RECORD` & `bandplot-0.1.6.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-bandplot/__init__.py,sha256=mFp-25ZLsKGYdenSxIDCsdXd-NbUGoaCoouHW35dmf4,26
-bandplot/mass.py,sha256=Sh3Eq-K8z7WNnUkDbPOcZKGruvEphlAqHYgr01-vpXE,7096
-bandplot/plots.py,sha256=yWFTG29hkF2NgHnnMn-Dg1_51Jra7zTwk2vzaNxicpM,25644
-bandplot/pplots.py,sha256=brKpvhhoB63uK3zUywgzDA9pml3U6C8YySui6g5MqFw,22446
-bandplot/projected.py,sha256=EketFLm4KUusA3wVslVVJke7HJIbCvhwyiiW-x3eslI,9321
+bandplot/__init__.py,sha256=oLEUf02I2FkQvbDBCKC2isJX6morDDwQWOjvkPlj6T8,24
+bandplot/mass.py,sha256=R8uBMrTuLscmGjjTwnm7Ez_P3GwxPTGksfQk4XeUfYU,7327
+bandplot/plots.py,sha256=KAqWh0LjmNoQWtczRudIbTok8mDLcXZ8L9xpyoO6xMc,26503
+bandplot/pplots.py,sha256=24-RmuzMFcaJlQ-aHX0VncverqPFCIaRMvrLLna3QfU,23084
+bandplot/projected.py,sha256=L-6621td5Pivj9g8bUU4YWtpDP1cQWpRxffE-ePwQb4,9548
 bandplot/readdata.py,sha256=vrxY7d4V8ONemimNxANrWkvXtt0raZyAbyRN1i8eoLM,6229
-bandplot/wrapper.py,sha256=wKlgDGtBpIeKiLHQrshZxXXGTBreCz1vVZA_DqObqx8,23361
-bandplot-0.1.5.3.dist-info/METADATA,sha256=HoRXJ32ss_V9EcDnLQXTKdPDtLROiTDpZ4x8N9RQEGg,3084
-bandplot-0.1.5.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bandplot-0.1.5.3.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
-bandplot-0.1.5.3.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
-bandplot-0.1.5.3.dist-info/RECORD,,
+bandplot/wrapper.py,sha256=HBFcUvWqTMytVehL-ONAJQy6SW2XpBXK1lZoRDTYTXs,23474
+bandplot-0.1.6.dist-info/METADATA,sha256=dHDOwmQiLK4OTsqYffcnsIe8uzngbsiUrGQQgtsqpYc,3082
+bandplot-0.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bandplot-0.1.6.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
+bandplot-0.1.6.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
+bandplot-0.1.6.dist-info/RECORD,,
```

