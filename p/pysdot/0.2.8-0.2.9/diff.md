# Comparing `tmp/pysdot-0.2.8.tar.gz` & `tmp/pysdot-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdot-0.2.8.tar", last modified: Fri May  5 12:52:12 2023, max compression
+gzip compressed data, was "pysdot-0.2.9.tar", last modified: Thu May 25 12:07:36 2023, max compression
```

## Comparing `pysdot-0.2.8.tar` & `pysdot-0.2.9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.809024 pysdot-0.2.8/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       29 2023-01-20 07:48:21.000000 pysdot-0.2.8/MANIFEST.in
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      454 2023-05-05 12:52:12.809024 pysdot-0.2.8/PKG-INFO
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     7281 2023-05-05 12:51:53.000000 pysdot-0.2.8/pysdot/OptimalTransport.py
--rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)    16769 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/PowerDiagram.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       86 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/cpp/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       25 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/__init__.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      204 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/comb_types.h
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      295 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/cpp_module.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    14376 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/inferno_color_map.h
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    44123 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/pybind_sdot.cpp
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      719 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/cpp/pybind_sdot_Arfd.cpp
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/domain_types/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     3094 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/domain_types/ConvexPolyhedraAssembly.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     1230 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/domain_types/ScaledImage.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       98 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/domain_types/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/radial_funcs/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      592 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncArfd.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      253 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncEntropy.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      264 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncInBall.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      256 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncPpWmR2.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      224 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncR2.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      222 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/RadialFuncUnit.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      268 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/radial_funcs/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot/solvers/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      630 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/solvers/CuPyx.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      929 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/solvers/Petsc.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      493 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/solvers/Scipy.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        0 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/solvers/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.809024 pysdot-0.2.8/pysdot/util/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     2557 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/util/FastMarching.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       39 2023-01-20 07:48:21.000000 pysdot-0.2.8/pysdot/util/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-05 12:52:12.805024 pysdot-0.2.8/pysdot.egg-info/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      454 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/PKG-INFO
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      930 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/SOURCES.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        1 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/dependency_links.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        6 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/requires.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       68 2023-05-05 12:52:12.000000 pysdot-0.2.8/pysdot.egg-info/top_level.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       38 2023-05-05 12:52:12.809024 pysdot-0.2.8/setup.cfg
--rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)     3372 2023-05-05 12:51:24.000000 pysdot-0.2.8/setup.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-25 12:07:36.021475 pysdot-0.2.9/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       29 2022-10-12 11:21:09.000000 pysdot-0.2.9/MANIFEST.in
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      454 2023-05-25 12:07:36.021475 pysdot-0.2.9/PKG-INFO
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-25 12:07:36.021475 pysdot-0.2.9/pysdot/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     7281 2023-05-25 12:05:30.000000 pysdot-0.2.9/pysdot/OptimalTransport.py
+-rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)    17095 2023-05-17 09:25:23.000000 pysdot-0.2.9/pysdot/PowerDiagram.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     5845 2023-05-17 13:48:14.000000 pysdot-0.2.9/pysdot/TransportMap.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      209 2023-05-17 09:47:14.000000 pysdot-0.2.9/pysdot/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-25 12:07:36.021475 pysdot-0.2.9/pysdot/cpp/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       25 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/cpp/__init__.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      204 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/cpp/comb_types.h
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      306 2023-05-16 13:13:31.000000 pysdot-0.2.9/pysdot/cpp/cpp_module.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    14376 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/cpp/inferno_color_map.h
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    47084 2023-05-25 12:05:49.000000 pysdot-0.2.9/pysdot/cpp/pybind_sdot.cpp
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      719 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/cpp/pybind_sdot_Arfd.cpp
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-25 12:07:36.021475 pysdot-0.2.9/pysdot/domain_types/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     3094 2022-10-12 11:35:06.000000 pysdot-0.2.9/pysdot/domain_types/ConvexPolyhedraAssembly.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     1230 2022-10-19 07:05:57.000000 pysdot-0.2.9/pysdot/domain_types/ScaledImage.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       98 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/domain_types/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-25 12:07:36.021475 pysdot-0.2.9/pysdot/radial_funcs/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      592 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/radial_funcs/RadialFuncArfd.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      253 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/radial_funcs/RadialFuncEntropy.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      264 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/radial_funcs/RadialFuncInBall.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      256 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/radial_funcs/RadialFuncPpWmR2.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      224 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/radial_funcs/RadialFuncR2.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      222 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/radial_funcs/RadialFuncUnit.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      268 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/radial_funcs/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-25 12:07:36.021475 pysdot-0.2.9/pysdot/solvers/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      794 2023-05-17 07:25:36.000000 pysdot-0.2.9/pysdot/solvers/CuPyx.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     1066 2023-05-17 07:25:06.000000 pysdot-0.2.9/pysdot/solvers/Petsc.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      493 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/solvers/Scipy.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        0 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/solvers/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-25 12:07:36.021475 pysdot-0.2.9/pysdot/util/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     2557 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/util/FastMarching.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       39 2022-10-12 11:21:09.000000 pysdot-0.2.9/pysdot/util/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-05-25 12:07:36.021475 pysdot-0.2.9/pysdot.egg-info/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      454 2023-05-25 12:07:35.000000 pysdot-0.2.9/pysdot.egg-info/PKG-INFO
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      953 2023-05-25 12:07:35.000000 pysdot-0.2.9/pysdot.egg-info/SOURCES.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        1 2023-05-25 12:07:35.000000 pysdot-0.2.9/pysdot.egg-info/dependency_links.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        6 2023-05-25 12:07:35.000000 pysdot-0.2.9/pysdot.egg-info/requires.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       68 2023-05-25 12:07:35.000000 pysdot-0.2.9/pysdot.egg-info/top_level.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       38 2023-05-25 12:07:36.021475 pysdot-0.2.9/setup.cfg
+-rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)     3372 2023-05-25 12:05:03.000000 pysdot-0.2.9/setup.py
```

### Comparing `pysdot-0.2.8/pysdot/OptimalTransport.py` & `pysdot-0.2.9/pysdot/OptimalTransport.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.8/pysdot/PowerDiagram.py` & `pysdot-0.2.9/pysdot/PowerDiagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,24 @@
             os.makedirs(dn, exist_ok=True)
         inst = self._updated_grid()
         return inst.display_vtk_points(
             np.ascontiguousarray( self.positions ),
             filename
         )
 
+    def vtk_mesh_data(self, shrink_factor=0.0):
+        inst = self._updated_grid()
+        return inst.vtk_mesh_data(
+            np.ascontiguousarray( self.positions ),
+            np.ascontiguousarray( self.weights ),
+            self.domain._inst,
+            self.radial_func.name(),
+            shrink_factor
+        )
+
     # make a .asy file for a representation of the power diagram
     def display_asy(self, filename, preamble="", closing="", output_format="pdf", linewidth=0.02, dotwidth=0.0, values=np.array([]), colormap="inferno", avoid_bounds=False, min_rf=1, max_rf=0):
         dn = os.path.dirname( filename )
         if len( dn ):
             os.makedirs( dn, exist_ok = True )
 
         p = "settings.outformat = \"{}\";\nunitsize(1cm);\n".format( output_format )
```

### Comparing `pysdot-0.2.8/pysdot/cpp/inferno_color_map.h` & `pysdot-0.2.9/pysdot/cpp/inferno_color_map.h`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.8/pysdot/cpp/pybind_sdot.cpp` & `pysdot-0.2.9/pysdot/cpp/pybind_sdot.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -520,27 +520,40 @@
         }
 
         template<class Domain,class FUNC>
         void display_vtk( pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, Domain &domain, const FUNC &func, const char *filename, bool points, bool centroids ) {
             //        sdot::VtkOutput<1,TF> vo({ "num" });
             //        grid.display( vo );
             //        vo.save( filename );
-            sdot::VtkOutput<3> vtk_output( { "weight", "num", "kind" } );
+            sdot::VtkOutput<6> vtk_output( { "weight", "num", "kind", "centroid_x", "centroid_y", "centroid_z" } );
 
             // auto buf_positions = positions.request();
             // auto buf_weights = weights.request();
             auto ptr_positions = reinterpret_cast<const Pt *>( positions.data() );
             auto ptr_weights = weights.data();
 
             find_radial_func( func, [&]( const auto &ft ) {
                 grid.for_each_laguerre_cell(
                     [&]( auto &lc, std::size_t num_dirac_0, int ) {
+                        // get centroid
+                        TF mass = 0;
+                        Pt centroid = TF( 0 );
+                        domain.bounds.for_each_intersection( lc, [&]( auto &cp, const auto &sf ) {
+                            cp.add_centroid_contrib( centroid, mass, sf, ft.func_for_final_cp_integration(), ptr_weights[ num_dirac_0 ] );
+                        } );
+                        if ( mass )
+                            centroid = 1 / mass * centroid;
+
                         domain.bounds.for_each_intersection( lc, [&]( auto &cp, auto space_func ) {
                             if ( space_func )
-                                cp.display( vtk_output, { ptr_weights[ num_dirac_0 ], TF( num_dirac_0 ), TF( 0 ) } );
+                                cp.display( vtk_output, { ptr_weights[ num_dirac_0 ], TF( num_dirac_0 ), TF( 0 ), 
+                                    0 < dim ? centroid[ 0 ] : TF( 0 ),
+                                    1 < dim ? centroid[ 1 ] : TF( 0 ),
+                                    2 < dim ? centroid[ 2 ] : TF( 0 )
+                                } );
                         } );
                     },
                     domain.bounds.englobing_convex_polyhedron(),
                     ptr_positions,
                     ptr_weights,
                     positions.shape( 0 ),
                     false,
@@ -565,14 +578,46 @@
                     vtk_output.add_point( c[ n ], { ptr_weights[ n ], TF( n ), TF( 2 ) } );
             }
 
             vtk_output.save( filename );
         }
 
         template<class Domain,class FUNC>
+        std::tuple<std::vector<PT>,std::vector<PT>,std::vector<PD_TYPE>> vtk_mesh_data( pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, Domain &domain, const FUNC &func, PD_TYPE shrink_factor ) {
+            auto ptr_positions = reinterpret_cast<const Pt *>( positions.data() );
+            auto ptr_weights = weights.data();
+
+            sdot::VtkOutput<0> vtk_output; // ( { "weight", "num", "kind" } )
+
+            find_radial_func( func, [&]( const auto &ft ) {
+                grid.for_each_laguerre_cell(
+                    [&]( auto &lc, std::size_t num_dirac_0, int ) {
+                        sdot::VtkOutput<0> local_vtk_output; // ( { "weight", "num", "kind" } )
+                        domain.bounds.for_each_intersection( lc, [&]( auto &cp, auto space_func ) {
+                            if ( space_func )
+                                cp.display( local_vtk_output ); // , { ptr_weights[ num_dirac_0 ], TF( num_dirac_0 ), TF( 0 ) }
+                        } );
+                        local_vtk_output.merge_polygons();
+                        vtk_output.mutex.lock();
+                        vtk_output.append( local_vtk_output );
+                        vtk_output.mutex.unlock();
+                    },
+                    domain.bounds.englobing_convex_polyhedron(),
+                    ptr_positions,
+                    ptr_weights,
+                    positions.shape( 0 ),
+                    false,
+                    ft.need_ball_cut()
+                );
+            } );
+
+            return { vtk_output.cells(), vtk_output.cell_types(), vtk_output.points() };
+        }
+
+        template<class Domain,class FUNC>
         std::string display_html_canvas( pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, Domain &domain, const FUNC &func, int hide_after ) {
             std::size_t nd = hide_after >= 0 ? std::min( hide_after, int( positions.shape( 0 ) ) ) : positions.shape( 0 );
             auto ptr_positions = reinterpret_cast<const Pt *>( positions.data() );
             auto ptr_weights = reinterpret_cast<const TF *>( weights.data() );
 
             // output variable
             std::ostringstream out;
@@ -760,14 +805,17 @@
             } \
             PyDerResult<dim,TF> der_integrals_wrt_weights_##NAME( pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, DOMAIN<dim,TF> &domain, const FUNC &func, bool stop_if_void ) { \
                 return der_integrals_wrt_weights( positions, weights, domain, func, stop_if_void ); \
             } \
             pybind11::array_t<TF> distances_from_boundaries_##NAME( pybind11::array_t<PD_TYPE> &points, pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, DOMAIN<dim,TF> &domain, const FUNC &func, bool count_domain_boundaries ) { \
                 return distances_from_boundaries( points, positions, weights, domain, func, count_domain_boundaries ); \
             } \
+            std::tuple<std::vector<PT>,std::vector<PT>,std::vector<PD_TYPE>> vtk_mesh_data_##NAME( pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, DOMAIN<dim,TF> &domain, const FUNC &func, TF shrink_factor ) { \
+                return vtk_mesh_data( positions, weights, domain, func, shrink_factor ); \
+            } \
             void display_vtk_##NAME( pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, DOMAIN<dim,TF> &domain, const FUNC &func, const char *filename, bool points, bool centroids ) { \
                 display_vtk( positions, weights, domain, func, filename, points, centroids ); \
             } \
             std::string display_html_canvas_##NAME( pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, DOMAIN<dim,TF> &domain, const FUNC &func, int hide_after ) { \
                 return display_html_canvas( positions, weights, domain, func, hide_after ); \
             } \
             PyDerResult<dim,TF> der_centroids_and_integrals_wrt_weight_and_positions_##NAME( pybind11::array_t<PD_TYPE> &positions, pybind11::array_t<PD_TYPE> &weights, DOMAIN<dim,TF> &domain, const FUNC &func ) { \
@@ -826,14 +874,15 @@
         .def( "add_replication"                                             , &PowerDiagramZGrid::add_replication                                            , "" )
         #define DEF_FOR( NAME, DOMAIN, FUNC ) \
                 .def( "integrals"                                           , &PowerDiagramZGrid::integrals_##NAME                                           , "" ) \
                 .def( "image_integrals"                                     , &PowerDiagramZGrid::image_integrals_##NAME                                     , "" ) \
                 .def( "der_integrals_wrt_weights"                           , &PowerDiagramZGrid::der_integrals_wrt_weights_##NAME                           , "" ) \
                 .def( "distances_from_boundaries"                           , &PowerDiagramZGrid::distances_from_boundaries_##NAME                           , "" ) \
                 .def( "centroids"                                           , &PowerDiagramZGrid::centroids_##NAME                                           , "" ) \
+                .def( "vtk_mesh_data"                                       , &PowerDiagramZGrid::vtk_mesh_data_##NAME                                        , "" ) \
                 .def( "display_vtk"                                         , &PowerDiagramZGrid::display_vtk_##NAME                                         , "" ) \
                 .def( "display_html_canvas"                                 , &PowerDiagramZGrid::display_html_canvas_##NAME                                 , "" ) \
                 .def( "der_centroids_and_integrals_wrt_weight_and_positions", &PowerDiagramZGrid::der_centroids_and_integrals_wrt_weight_and_positions_##NAME, "" ) \
                 .def( "display_asy"                                         , &PowerDiagramZGrid::display_asy_##NAME                                         , "" )
         #include "comb_types.h"
         #undef DEF_FOR
         .def( "display_vtk_points"                                  , &PowerDiagramZGrid::display_vtk_points                                                 , "" )
```

### Comparing `pysdot-0.2.8/pysdot/cpp/pybind_sdot_Arfd.cpp` & `pysdot-0.2.9/pysdot/cpp/pybind_sdot_Arfd.cpp`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.8/pysdot/domain_types/ConvexPolyhedraAssembly.py` & `pysdot-0.2.9/pysdot/domain_types/ConvexPolyhedraAssembly.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.8/pysdot/domain_types/ScaledImage.py` & `pysdot-0.2.9/pysdot/domain_types/ScaledImage.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.8/pysdot/radial_funcs/RadialFuncArfd.py` & `pysdot-0.2.9/pysdot/radial_funcs/RadialFuncArfd.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.8/pysdot/solvers/CuPyx.py` & `pysdot-0.2.9/pysdot/solvers/CuPyx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-
 import numpy as np
 import cupy as cp
 from cupyx.scipy.sparse import csr_matrix
-from cupyx.linalg.sparse.solve import lschol
+# from cupyx.linalg.sparse._solve import csr_matrix
+from cupyx.linalg.sparse._solve import lschol
     
 class Solver:
+    """
+       Solver that uses cupy (that can be installed for instance using `pip install cupy`)
+    """
+    
     def __init__(self):
         self.dtype = np.float64
 
     def create_matrix(self, N, *args):
         (offsets, columns, values) = map(cp.asarray, args)
         return csr_matrix((values, columns, offsets))
```

### Comparing `pysdot-0.2.8/pysdot/solvers/Petsc.py` & `pysdot-0.2.9/pysdot/solvers/Petsc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from petsc4py import PETSc
 
 
 #
 class Solver:
+    """
+       Solver that uses petsc4py (that can be installed for instance using `conda install -c conda-forge petsc4py`)
+    """
+    
     def __init__(self):
         pass
 
     def create_matrix(self, N, offsets, columns, values):
         A = PETSc.Mat().createAIJ([N, N], csr=(
             offsets.astype(PETSc.IntType),
             columns.astype(PETSc.IntType),
```

### Comparing `pysdot-0.2.8/pysdot/util/FastMarching.py` & `pysdot-0.2.9/pysdot/util/FastMarching.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.8/pysdot.egg-info/SOURCES.txt` & `pysdot-0.2.9/pysdot.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 setup.py
 pysdot/OptimalTransport.py
 pysdot/PowerDiagram.py
+pysdot/TransportMap.py
 pysdot/__init__.py
 pysdot.egg-info/PKG-INFO
 pysdot.egg-info/SOURCES.txt
 pysdot.egg-info/dependency_links.txt
 pysdot.egg-info/requires.txt
 pysdot.egg-info/top_level.txt
 pysdot/cpp/__init__.py
```

### Comparing `pysdot-0.2.8/setup.py` & `pysdot-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             subprocess.check_call(['git', 'clone', 'https://github.com/eigenteam/eigen-git-mirror.git', 'ext/eigen3'])
         if not os.path.isdir('./ext/pybind11'):
             subprocess.check_call(['git', 'clone', 'https://github.com/pybind/pybind11.git', 'ext/pybind11'])
         setuptools.command.build_py.build_py.run(self)
 
 setup(
     name='pysdot',
-    version='0.2.8',
+    version='0.2.9',
     packages=find_packages(exclude=[
         'hugo', 'ext', 'build', 'dist',
         'examples', 'results', 'tests'
     ]),
     cmdclass={
         'build_py': BuildPyCommand,
     },
```

