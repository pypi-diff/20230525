# Comparing `tmp/OpenGeode_Inspector-3.0.4-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Inspector-3.0.5-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 262749 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      175 b- defN 23-May-11 08:13 opengeode_inspector/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-May-11 08:13 opengeode_inspector/inspector.py
--rw-rw-rw-  2.0 fat   436736 b- defN 23-May-11 08:14 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
--rw-rw-rw-  2.0 fat   451072 b- defN 23-May-11 08:14 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     5481 b- defN 23-May-11 08:14 OpenGeode_Inspector-3.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-11 08:14 OpenGeode_Inspector-3.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-May-11 08:14 OpenGeode_Inspector-3.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      772 b- defN 23-May-11 08:14 OpenGeode_Inspector-3.0.4.dist-info/RECORD
-8 files, 894627 bytes uncompressed, 261377 bytes compressed:  70.8%
+Zip file size: 262751 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      175 b- defN 23-May-17 08:11 opengeode_inspector/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-May-17 08:11 opengeode_inspector/inspector.py
+-rw-rw-rw-  2.0 fat   436736 b- defN 23-May-17 08:12 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
+-rw-rw-rw-  2.0 fat   451072 b- defN 23-May-17 08:12 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     5480 b- defN 23-May-17 08:12 OpenGeode_Inspector-3.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-17 08:12 OpenGeode_Inspector-3.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-May-17 08:12 OpenGeode_Inspector-3.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      772 b- defN 23-May-17 08:12 OpenGeode_Inspector-3.0.5.dist-info/RECORD
+8 files, 894626 bytes uncompressed, 261379 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
 Comment: 
 
 Filename: opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.4.dist-info/METADATA
+Filename: OpenGeode_Inspector-3.0.5.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.4.dist-info/WHEEL
+Filename: OpenGeode_Inspector-3.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.4.dist-info/top_level.txt
+Filename: OpenGeode_Inspector-3.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.4.dist-info/RECORD
+Filename: OpenGeode_Inspector-3.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180049210
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 11 08:13:46 2023
+Time/Date		Wed May 17 08:11:50 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000004b800
 SizeOfInitializedData	000000000001ee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000049210
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0006f000
 SizeOfHeaders		00000400
-CheckSum		00077085
+CheckSum		00074361
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -65,100 +65,100 @@
 The Import Tables (interpreted .rdata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
  000636b8	00063cf8 00000000 00000000 0006577e 0004d4e8
 
 	DLL Name: OpenGeode_model.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	65706	  797  ?end@CornerRange@?$Corners@$01@geode@@QEBAAEBV123@XZ
+	65706	  801  ?end@CornerRange@?$Corners@$01@geode@@QEBAAEBV123@XZ
 	656cc	  574  ?begin@CornerRange@?$Corners@$01@geode@@QEBAAEBV123@XZ
 	6573e	  459  ??DCornerRange@?$Corners@$01@geode@@QEBAAEBV?$Corner@$01@2@XZ
-	64a80	  922  ?mesh@?$Corner@$01@geode@@QEBAAEBV?$PointSet@$01@2@XZ
+	64a80	  926  ?mesh@?$Corner@$01@geode@@QEBAAEBV?$PointSet@$01@2@XZ
 	6569e	  362  ??1CornerRange@?$Corners@$01@geode@@QEAA@XZ
 	65668	  185  ??0CornerRange@?$Corners@$01@geode@@QEAA@AEBV012@@Z
 	65636	  490  ??ECornerRangeBase@?$Corners@$01@geode@@QEAAXXZ
 	655fa	  438  ??9CornerRangeBase@?$Corners@$01@geode@@QEBA_NAEBV012@@Z
-	655c0	  684  ?corners@?$Corners@$01@geode@@QEBA?AVCornerRange@12@XZ
-	65576	  880  ?is_internal@BRep@geode@@QEBA_NAEBV?$Line@$02@2@AEBV?$Surface@$02@2@@Z
-	6552c	  869  ?is_boundary@BRep@geode@@QEBA_NAEBV?$Line@$02@2@AEBV?$Surface@$02@2@@Z
-	654f2	  882  ?is_internal@Relationships@geode@@QEBA_NAEBUuuid@2@0@Z
-	654a8	  788  ?embeddings@Relationships@geode@@QEBA?AVEmbeddingRange@12@AEBUuuid@2@@Z
+	655c0	  688  ?corners@?$Corners@$01@geode@@QEBA?AVCornerRange@12@XZ
+	65576	  884  ?is_internal@BRep@geode@@QEBA_NAEBV?$Line@$02@2@AEBV?$Surface@$02@2@@Z
+	6552c	  873  ?is_boundary@BRep@geode@@QEBA_NAEBV?$Line@$02@2@AEBV?$Surface@$02@2@@Z
+	654f2	  886  ?is_internal@Relationships@geode@@QEBA_NAEBUuuid@2@0@Z
+	654a8	  792  ?embeddings@Relationships@geode@@QEBA?AVEmbeddingRange@12@AEBUuuid@2@@Z
 	6546e	  202  ??0EmbeddingRange@Relationships@geode@@QEAA@AEBV012@@Z
 	6543c	  368  ??1EmbeddingRange@Relationships@geode@@QEAA@XZ
 	653f2	  462  ??DEmbeddingRangeIterator@Relationships@geode@@QEBAAEBVComponentID@2@XZ
 	653b8	  493  ??EEmbeddingRangeIterator@Relationships@geode@@QEAAXXZ
 	65376	  440  ??9EmbeddingRangeIterator@Relationships@geode@@QEBA_NAEBV012@@Z
-	6533c	  871  ?is_boundary@Relationships@geode@@QEBA_NAEBUuuid@2@0@Z
-	65302	  985  ?nb_embeddings@Relationships@geode@@QEBAIAEBUuuid@2@@Z
-	652c8	  986  ?nb_incidences@Relationships@geode@@QEBAIAEBUuuid@2@@Z
-	651ca	  639  ?component_mesh_vertices@VertexIdentifier@geode@@QEBA?AV?$vector@UComponentMeshVertex@geode@@V?$allocator@UComponentMeshVertex@geode@@@std@@@std@@IAEBV?$NamedType@V?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@UComponentTag@geode@@@2@@Z
+	6533c	  875  ?is_boundary@Relationships@geode@@QEBA_NAEBUuuid@2@0@Z
+	65302	  990  ?nb_embeddings@Relationships@geode@@QEBAIAEBUuuid@2@@Z
+	652c8	  991  ?nb_incidences@Relationships@geode@@QEBAIAEBUuuid@2@@Z
+	651ca	  643  ?component_mesh_vertices@VertexIdentifier@geode@@QEBA?AV?$vector@UComponentMeshVertex@geode@@V?$allocator@UComponentMeshVertex@geode@@@std@@@std@@IAEBV?$NamedType@V?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@UComponentTag@geode@@@2@@Z
 	6518a	  460  ??DCornerRange@?$Corners@$02@geode@@QEBAAEBV?$Corner@$02@2@XZ
-	65152	  798  ?end@CornerRange@?$Corners@$02@geode@@QEBAAEBV123@XZ
+	65152	  802  ?end@CornerRange@?$Corners@$02@geode@@QEBAAEBV123@XZ
 	65118	  575  ?begin@CornerRange@?$Corners@$02@geode@@QEBAAEBV123@XZ
 	650ea	  363  ??1CornerRange@?$Corners@$02@geode@@QEAA@XZ
 	650b4	  187  ??0CornerRange@?$Corners@$02@geode@@QEAA@AEBV012@@Z
 	65082	  491  ??ECornerRangeBase@?$Corners@$02@geode@@QEAAXXZ
 	65046	  439  ??9CornerRangeBase@?$Corners@$02@geode@@QEBA_NAEBV012@@Z
-	6500c	  685  ?corners@?$Corners@$02@geode@@QEBA?AVCornerRange@12@XZ
-	64fc0	  844  ?has_component_mesh_vertices@VertexIdentifier@geode@@QEBA_NIAEBUuuid@2@@Z
-	64f62	  732  ?create_surface_meshes_aabb_trees@geode@@YA?AU?$ModelMeshesAABBTree@$01@1@AEBVSection@1@@Z
-	64f08	  733  ?create_surface_meshes_aabb_trees@geode@@YA?AU?$ModelMeshesAABBTree@$02@1@AEBVBRep@1@@Z
+	6500c	  689  ?corners@?$Corners@$02@geode@@QEBA?AVCornerRange@12@XZ
+	64fc0	  848  ?has_component_mesh_vertices@VertexIdentifier@geode@@QEBA_NIAEBUuuid@2@@Z
+	64f62	  736  ?create_surface_meshes_aabb_trees@geode@@YA?AU?$ModelMeshesAABBTree@$01@1@AEBVSection@1@@Z
+	64f08	  737  ?create_surface_meshes_aabb_trees@geode@@YA?AU?$ModelMeshesAABBTree@$02@1@AEBVBRep@1@@Z
 	64ece	  481  ??DLineRange@?$Lines@$02@geode@@QEBAAEBV?$Line@$02@2@XZ
-	64e9a	  819  ?end@LineRange@?$Lines@$02@geode@@QEBAAEBV123@XZ
+	64e9a	  823  ?end@LineRange@?$Lines@$02@geode@@QEBAAEBV123@XZ
 	64e64	  596  ?begin@LineRange@?$Lines@$02@geode@@QEBAAEBV123@XZ
 	64e3a	  391  ??1LineRange@?$Lines@$02@geode@@QEAA@XZ
 	64e08	  259  ??0LineRange@?$Lines@$02@geode@@QEAA@AEBV012@@Z
 	64dda	  505  ??ELineRangeBase@?$Lines@$02@geode@@QEAAXXZ
 	64da2	  445  ??9LineRangeBase@?$Lines@$02@geode@@QEBA_NAEBV012@@Z
 	64d68	  480  ??DLineRange@?$Lines@$01@geode@@QEBAAEBV?$Line@$01@2@XZ
-	64d34	  818  ?end@LineRange@?$Lines@$01@geode@@QEBAAEBV123@XZ
+	64d34	  822  ?end@LineRange@?$Lines@$01@geode@@QEBAAEBV123@XZ
 	64cfe	  595  ?begin@LineRange@?$Lines@$01@geode@@QEBAAEBV123@XZ
 	64cd4	  390  ??1LineRange@?$Lines@$01@geode@@QEAA@XZ
 	64ca2	  257  ??0LineRange@?$Lines@$01@geode@@QEAA@AEBV012@@Z
 	64c74	  504  ??ELineRangeBase@?$Lines@$01@geode@@QEAAXXZ
 	64c3c	  444  ??9LineRangeBase@?$Lines@$01@geode@@QEBA_NAEBV012@@Z
-	64c08	  894  ?lines@?$Lines@$01@geode@@QEBA?AVLineRange@12@XZ
-	6419a	 1100  ?surfaces@?$Surfaces@$02@geode@@QEBA?AVSurfaceRange@12@XZ
-	641d6	 1099  ?surfaces@?$Surfaces@$01@geode@@QEBA?AVSurfaceRange@12@XZ
+	64c08	  898  ?lines@?$Lines@$01@geode@@QEBA?AVLineRange@12@XZ
+	6419a	 1106  ?surfaces@?$Surfaces@$02@geode@@QEBA?AVSurfaceRange@12@XZ
+	641d6	 1105  ?surfaces@?$Surfaces@$01@geode@@QEBA?AVSurfaceRange@12@XZ
 	64212	  449  ??9SurfaceRangeBase@?$Surfaces@$01@geode@@QEBA_NAEBV012@@Z
 	64250	  509  ??ESurfaceRangeBase@?$Surfaces@$01@geode@@QEAAXXZ
 	64284	  309  ??0SurfaceRange@?$Surfaces@$01@geode@@QEAA@AEBV012@@Z
 	642bc	  411  ??1SurfaceRange@?$Surfaces@$01@geode@@QEAA@XZ
 	642ec	  600  ?begin@SurfaceRange@?$Surfaces@$01@geode@@QEBAAEBV123@XZ
-	64328	  823  ?end@SurfaceRange@?$Surfaces@$01@geode@@QEBAAEBV123@XZ
+	64328	  827  ?end@SurfaceRange@?$Surfaces@$01@geode@@QEBAAEBV123@XZ
 	64362	  485  ??DSurfaceRange@?$Surfaces@$01@geode@@QEBAAEBV?$Surface@$01@2@XZ
-	643a6	  837  ?get_mesh@?$Surface@$01@geode@@AEBAAEBV?$SurfaceMesh@$01@2@XZ
+	643a6	  841  ?get_mesh@?$Surface@$01@geode@@AEBAAEBV?$SurfaceMesh@$01@2@XZ
 	643e6	  450  ??9SurfaceRangeBase@?$Surfaces@$02@geode@@QEBA_NAEBV012@@Z
 	64424	  510  ??ESurfaceRangeBase@?$Surfaces@$02@geode@@QEAAXXZ
 	64458	  311  ??0SurfaceRange@?$Surfaces@$02@geode@@QEAA@AEBV012@@Z
 	64490	  412  ??1SurfaceRange@?$Surfaces@$02@geode@@QEAA@XZ
 	644c0	  601  ?begin@SurfaceRange@?$Surfaces@$02@geode@@QEBAAEBV123@XZ
-	644fc	  824  ?end@SurfaceRange@?$Surfaces@$02@geode@@QEBAAEBV123@XZ
+	644fc	  828  ?end@SurfaceRange@?$Surfaces@$02@geode@@QEBAAEBV123@XZ
 	64536	  486  ??DSurfaceRange@?$Surfaces@$02@geode@@QEBAAEBV?$Surface@$02@2@XZ
-	6457a	  838  ?get_mesh@?$Surface@$02@geode@@AEBAAEBV?$SurfaceMesh@$02@2@XZ
-	64bd4	  895  ?lines@?$Lines@$02@geode@@QEBA?AVLineRange@12@XZ
-	64b88	 1105  ?unique_vertex@VertexIdentifier@geode@@QEBAIAEBUComponentMeshVertex@2@@Z
+	6457a	  842  ?get_mesh@?$Surface@$02@geode@@AEBAAEBV?$SurfaceMesh@$02@2@XZ
+	64bd4	  899  ?lines@?$Lines@$02@geode@@QEBA?AVLineRange@12@XZ
+	64b88	 1111  ?unique_vertex@VertexIdentifier@geode@@QEBAIAEBUComponentMeshVertex@2@@Z
 	64b60	  361  ??1ComponentMeshVertex@geode@@QEAA@XZ
 	64b28	  184  ??0ComponentMeshVertex@geode@@QEAA@VComponentID@1@I@Z
-	64af0	  923  ?mesh@?$Corner@$02@geode@@QEBAAEBV?$PointSet@$02@2@XZ
-	64ab8	  925  ?mesh@?$Line@$02@geode@@QEBAAEBV?$EdgedCurve@$02@2@XZ
-	64168	  858  ?initialize@OpenGeodeModelLibrary@geode@@SAXXZ
-	64a48	  924  ?mesh@?$Line@$01@geode@@QEBAAEBV?$EdgedCurve@$01@2@XZ
-	64a00	 1094  ?surface@?$Surfaces@$01@geode@@QEBAAEBV?$Surface@$01@2@AEBUuuid@2@@Z
-	649c2	  890  ?line@?$Lines@$01@geode@@QEBAAEBV?$Line@$01@2@AEBUuuid@2@@Z
-	6497e	  680  ?corner@?$Corners@$01@geode@@QEBAAEBV?$Corner@$01@2@AEBUuuid@2@@Z
+	64af0	  927  ?mesh@?$Corner@$02@geode@@QEBAAEBV?$PointSet@$02@2@XZ
+	64ab8	  929  ?mesh@?$Line@$02@geode@@QEBAAEBV?$EdgedCurve@$02@2@XZ
+	64168	  862  ?initialize@OpenGeodeModelLibrary@geode@@SAXXZ
+	64a48	  928  ?mesh@?$Line@$01@geode@@QEBAAEBV?$EdgedCurve@$01@2@XZ
+	64a00	 1100  ?surface@?$Surfaces@$01@geode@@QEBAAEBV?$Surface@$01@2@AEBUuuid@2@@Z
+	649c2	  894  ?line@?$Lines@$01@geode@@QEBAAEBV?$Line@$01@2@AEBUuuid@2@@Z
+	6497e	  684  ?corner@?$Corners@$01@geode@@QEBAAEBV?$Corner@$01@2@AEBUuuid@2@@Z
 	6493c	  603  ?block@?$Blocks@$02@geode@@QEBAAEBV?$Block@$02@2@AEBUuuid@2@@Z
-	648f4	 1095  ?surface@?$Surfaces@$02@geode@@QEBAAEBV?$Surface@$02@2@AEBUuuid@2@@Z
-	648b6	  891  ?line@?$Lines@$02@geode@@QEBAAEBV?$Line@$02@2@AEBUuuid@2@@Z
-	64872	  681  ?corner@?$Corners@$02@geode@@QEBAAEBV?$Corner@$02@2@AEBUuuid@2@@Z
-	647d8	  640  ?component_mesh_vertices@VertexIdentifier@geode@@QEBAAEBV?$vector@UComponentMeshVertex@geode@@V?$allocator@UComponentMeshVertex@geode@@@std@@@std@@I@Z
-	647a2	 1004  ?nb_unique_vertices@VertexIdentifier@geode@@QEBAIXZ
-	64766	  836  ?get_mesh@?$Block@$02@geode@@AEBAAEBV?$SolidMesh@$02@2@XZ
+	648f4	 1101  ?surface@?$Surfaces@$02@geode@@QEBAAEBV?$Surface@$02@2@AEBUuuid@2@@Z
+	648b6	  895  ?line@?$Lines@$02@geode@@QEBAAEBV?$Line@$02@2@AEBUuuid@2@@Z
+	64872	  685  ?corner@?$Corners@$02@geode@@QEBAAEBV?$Corner@$02@2@AEBUuuid@2@@Z
+	647d8	  644  ?component_mesh_vertices@VertexIdentifier@geode@@QEBAAEBV?$vector@UComponentMeshVertex@geode@@V?$allocator@UComponentMeshVertex@geode@@@std@@@std@@I@Z
+	647a2	 1009  ?nb_unique_vertices@VertexIdentifier@geode@@QEBAIXZ
+	64766	  840  ?get_mesh@?$Block@$02@geode@@AEBAAEBV?$SolidMesh@$02@2@XZ
 	64728	  451  ??DBlockRange@?$Blocks@$02@geode@@QEBAAEBV?$Block@$02@2@XZ
-	646f2	  789  ?end@BlockRange@?$Blocks@$02@geode@@QEBAAEBV123@XZ
+	646f2	  793  ?end@BlockRange@?$Blocks@$02@geode@@QEBAAEBV123@XZ
 	646ba	  566  ?begin@BlockRange@?$Blocks@$02@geode@@QEBAAEBV123@XZ
 	6468e	  350  ??1BlockRange@?$Blocks@$02@geode@@QEAA@XZ
 	6465a	  155  ??0BlockRange@?$Blocks@$02@geode@@QEAA@AEBV012@@Z
 	6462a	  487  ??EBlockRangeBase@?$Blocks@$02@geode@@QEAAXXZ
 	645f0	  435  ??9BlockRangeBase@?$Blocks@$02@geode@@QEBA_NAEBV012@@Z
 	645ba	  606  ?blocks@?$Blocks@$02@geode@@QEBA?AVBlockRange@12@XZ
 
@@ -236,61 +236,61 @@
 	66a48	 1641  ?polygon_edge_vertices@?$SurfaceMesh@$02@geode@@QEBA?AV?$array@I$01@std@@AEBUPolygonEdge@2@@Z
 	66aa8	 1579  ?nb_polyhedron_vertices@?$SolidMesh@$02@geode@@QEBAEI@Z
 
  000636e0	000639c8 00000000 00000000 000675c0 0004d1b8
 
 	DLL Name: OpenGeode_geometry.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	66cc4	  301  ??1?$NNSearch@$01@geode@@QEAA@XZ
+	66cc4	  306  ??1?$NNSearch@$01@geode@@QEAA@XZ
 	6755c	   42  ??$point_triangle_position@$02@geode@@YA?AW4Position@0@AEBV?$Point@$02@0@AEBV?$Triangle@$02@0@@Z
-	674b2	  646  ?vertices@?$GenericSegment@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$01@std@@XZ
-	67408	  645  ?vertices@?$GenericSegment@V?$reference_wrapper@$$CBV?$Point@$01@geode@@@std@@$01@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$01@geode@@@std@@$01@std@@XZ
-	673d0	  512  ?intersects@?$BoundingBox@$01@geode@@QEBA_NAEBV12@@Z
-	67398	  515  ?intersects@?$BoundingBox@$02@geode@@QEBA_NAEBV12@@Z
-	67362	  532  ?mapping_morton@Impl@?$AABBTree@$01@geode@@QEBAII@Z
-	6731e	  550  ?node@Impl@?$AABBTree@$01@geode@@QEBAAEBV?$BoundingBox@$01@3@I@Z
-	672d0	  504  ?get_recursive_iterators@Impl@?$AABBTree@$01@geode@@SA?AUIterator@123@III@Z
-	672a0	  518  ?is_leaf@Impl@?$AABBTree@$01@geode@@SA_NII@Z
-	6726a	  533  ?mapping_morton@Impl@?$AABBTree@$02@geode@@QEBAII@Z
-	67226	  551  ?node@Impl@?$AABBTree@$02@geode@@QEBAAEBV?$BoundingBox@$02@3@I@Z
-	671d8	  505  ?get_recursive_iterators@Impl@?$AABBTree@$02@geode@@SA?AUIterator@123@III@Z
-	671a8	  519  ?is_leaf@Impl@?$AABBTree@$02@geode@@SA_NII@Z
-	6717c	  542  ?nb_bboxes@?$AABBTree@$01@geode@@QEBAIXZ
-	67158	  296  ??1?$AABBTree@$01@geode@@QEAA@XZ
-	6712c	  543  ?nb_bboxes@?$AABBTree@$02@geode@@QEBAIXZ
-	67108	  297  ??1?$AABBTree@$02@geode@@QEAA@XZ
-	670d2	  248  ??0?$Segment@$02@geode@@QEAA@AEBV?$Point@$02@1@0@Z
-	67026	  652  ?vertices@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@std@@XZ
+	674b2	  658  ?vertices@?$GenericSegment@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$01@std@@XZ
+	67408	  657  ?vertices@?$GenericSegment@V?$reference_wrapper@$$CBV?$Point@$01@geode@@@std@@$01@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$01@geode@@@std@@$01@std@@XZ
+	673d0	  523  ?intersects@?$BoundingBox@$01@geode@@QEBA_NAEBV12@@Z
+	67398	  526  ?intersects@?$BoundingBox@$02@geode@@QEBA_NAEBV12@@Z
+	67362	  543  ?mapping_morton@Impl@?$AABBTree@$01@geode@@QEBAII@Z
+	6731e	  561  ?node@Impl@?$AABBTree@$01@geode@@QEBAAEBV?$BoundingBox@$01@3@I@Z
+	672d0	  515  ?get_recursive_iterators@Impl@?$AABBTree@$01@geode@@SA?AUIterator@123@III@Z
+	672a0	  529  ?is_leaf@Impl@?$AABBTree@$01@geode@@SA_NII@Z
+	6726a	  544  ?mapping_morton@Impl@?$AABBTree@$02@geode@@QEBAII@Z
+	67226	  562  ?node@Impl@?$AABBTree@$02@geode@@QEBAAEBV?$BoundingBox@$02@3@I@Z
+	671d8	  516  ?get_recursive_iterators@Impl@?$AABBTree@$02@geode@@SA?AUIterator@123@III@Z
+	671a8	  530  ?is_leaf@Impl@?$AABBTree@$02@geode@@SA_NII@Z
+	6717c	  553  ?nb_bboxes@?$AABBTree@$01@geode@@QEBAIXZ
+	67158	  301  ??1?$AABBTree@$01@geode@@QEAA@XZ
+	6712c	  554  ?nb_bboxes@?$AABBTree@$02@geode@@QEBAIXZ
+	67108	  302  ??1?$AABBTree@$02@geode@@QEAA@XZ
+	670d2	  253  ??0?$Segment@$02@geode@@QEAA@AEBV?$Point@$02@1@0@Z
+	67026	  664  ?vertices@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@std@@XZ
 	66fc2	   41  ??$point_triangle_position@$01@geode@@YA?AW4Position@0@AEBV?$Point@$01@0@AEBV?$Triangle@$01@0@@Z
-	66f8c	  244  ??0?$Segment@$01@geode@@QEAA@AEBV?$Point@$01@1@0@Z
-	66f04	  616  ?segment_triangle_intersection_detection@geode@@YA?AU?$pair@W4Position@geode@@W412@@std@@AEBV?$Segment@$02@1@AEBV?$Triangle@$02@1@@Z
-	66e92	  613  ?segment_segment_intersection_detection@geode@@YA?AU?$pair@W4Position@geode@@W412@@std@@AEBV?$Segment@$01@1@0@Z
+	66f8c	  249  ??0?$Segment@$01@geode@@QEAA@AEBV?$Point@$01@1@0@Z
+	66f04	  628  ?segment_triangle_intersection_detection@geode@@YA?AU?$pair@W4Position@geode@@W412@@std@@AEBV?$Segment@$02@1@AEBV?$Triangle@$02@1@@Z
+	66e92	  625  ?segment_segment_intersection_detection@geode@@YA?AU?$pair@W4Position@geode@@W412@@std@@AEBV?$Segment@$01@1@0@Z
 	66e54	   26  ??$point_point_distance@$02@geode@@YANAEBV?$Point@$02@0@0@Z
 	66e16	   25  ??$point_point_distance@$01@geode@@YANAEBV?$Point@$01@0@0@Z
-	66dc8	  479  ?colocated_index_mapping@?$NNSearch@$02@geode@@QEBA?AUColocatedInfo@12@N@Z
-	66da4	  302  ??1?$NNSearch@$02@geode@@QEAA@XZ
-	66d36	  176  ??0?$NNSearch@$02@geode@@QEAA@V?$vector@V?$Point@$02@geode@@V?$allocator@V?$Point@$02@geode@@@std@@@std@@@Z
-	66ce8	  478  ?colocated_index_mapping@?$NNSearch@$01@geode@@QEBA?AUColocatedInfo@12@N@Z
-	66c56	  174  ??0?$NNSearch@$01@geode@@QEAA@V?$vector@V?$Point@$01@geode@@V?$allocator@V?$Point@$01@geode@@@std@@@std@@@Z
+	66dc8	  490  ?colocated_index_mapping@?$NNSearch@$02@geode@@QEBA?AUColocatedInfo@12@N@Z
+	66da4	  307  ??1?$NNSearch@$02@geode@@QEAA@XZ
+	66d36	  181  ??0?$NNSearch@$02@geode@@QEAA@V?$vector@V?$Point@$02@geode@@V?$allocator@V?$Point@$02@geode@@@std@@@std@@@Z
+	66ce8	  489  ?colocated_index_mapping@?$NNSearch@$01@geode@@QEBA?AUColocatedInfo@12@N@Z
+	66c56	  179  ??0?$NNSearch@$01@geode@@QEAA@V?$vector@V?$Point@$01@geode@@V?$allocator@V?$Point@$01@geode@@@std@@@std@@@Z
 
  000636f4	00063968 00000000 00000000 00067844 0004d158
 
 	DLL Name: OpenGeode_basic.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	67616	  140  ?instance@Singleton@geode@@CAPEAV12@AEBVtype_info@@@Z
+	67616	  141  ?instance@Singleton@geode@@CAPEAV12@AEBVtype_info@@@Z
 	67822	   71  ??Muuid@geode@@QEBA_NAEBU01@@Z
-	677c0	  153  ?log_warn@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
-	67762	  199  ?string@uuid@geode@@QEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
+	677c0	  154  ?log_warn@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
+	67762	  200  ?string@uuid@geode@@QEBA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@XZ
 	67740	   69  ??8uuid@geode@@QEBA_NAEBU01@@Z
 	67716	  127  ?id@Identifier@geode@@QEBAAEBUuuid@2@XZ
-	676b4	  151  ?log_info@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
+	676b4	  152  ?log_info@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
 	67686	   89  ?call_initialize@Library@geode@@IEAAXPEBD@Z
 	6766a	   26  ??0Library@geode@@IEAA@XZ
 	6764e	   49  ??1Library@geode@@UEAA@XZ
-	675d8	  192  ?set_instance@Singleton@geode@@CAXAEBVtype_info@@PEAV12@@Z
+	675d8	  193  ?set_instance@Singleton@geode@@CAXAEBVtype_info@@PEAV12@@Z
 
  00063708	00064080 00000000 00000000 000678a8 0004d870
 
 	DLL Name: absl_hash.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	67858	   12  ?CombineLargeContiguousImpl64@CityHashState@hash_internal@absl@@CA_K_KPEBE0@Z
 
@@ -12486,22 +12486,22 @@
 	  e860: 00 00 00 00 7e 84 06 00 00 00 00 00 4e 84 06 00
 	  e870: 00 00 00 00 00 00 00 00 00 00 00 00 f0 84 06 00
 	  e880: 00 00 00 00 98 84 06 00 00 00 00 00 86 84 06 00
 	  e890: 00 00 00 00 08 85 06 00 00 00 00 00 70 84 06 00
 	  e8a0: 00 00 00 00 64 84 06 00 00 00 00 00 1c 84 06 00
 	  e8b0: 00 00 00 00 d4 84 06 00 00 00 00 00 42 84 06 00
 	  e8c0: 00 00 00 00 b2 84 06 00 00 00 00 00 00 00 00 00
-	  e8d0: 00 00 00 00 5a 03 3f 69 6e 69 74 69 61 6c 69 7a
+	  e8d0: 00 00 00 00 5e 03 3f 69 6e 69 74 69 61 6c 69 7a
 	  e8e0: 65 40 4f 70 65 6e 47 65 6f 64 65 4d 6f 64 65 6c
 	  e8f0: 4c 69 62 72 61 72 79 40 67 65 6f 64 65 40 40 53
-	  e900: 41 58 58 5a 00 00 4c 04 3f 73 75 72 66 61 63 65
+	  e900: 41 58 58 5a 00 00 52 04 3f 73 75 72 66 61 63 65
 	  e910: 73 40 3f 24 53 75 72 66 61 63 65 73 40 24 30 32
 	  e920: 40 67 65 6f 64 65 40 40 51 45 42 41 3f 41 56 53
 	  e930: 75 72 66 61 63 65 52 61 6e 67 65 40 31 32 40 58
-	  e940: 5a 00 4b 04 3f 73 75 72 66 61 63 65 73 40 3f 24
+	  e940: 5a 00 51 04 3f 73 75 72 66 61 63 65 73 40 3f 24
 	  e950: 53 75 72 66 61 63 65 73 40 24 30 31 40 67 65 6f
 	  e960: 64 65 40 40 51 45 42 41 3f 41 56 53 75 72 66 61
 	  e970: 63 65 52 61 6e 67 65 40 31 32 40 58 5a 00 c1 01
 	  e980: 3f 3f 39 53 75 72 66 61 63 65 52 61 6e 67 65 42
 	  e990: 61 73 65 40 3f 24 53 75 72 66 61 63 65 73 40 24
 	  e9a0: 30 31 40 67 65 6f 64 65 40 40 51 45 42 41 5f 4e
 	  e9b0: 41 45 42 56 30 31 32 40 40 5a 00 00 fd 01 3f 3f
@@ -12514,23 +12514,23 @@
 	  ea20: 56 30 31 32 40 40 5a 00 9b 01 3f 3f 31 53 75 72
 	  ea30: 66 61 63 65 52 61 6e 67 65 40 3f 24 53 75 72 66
 	  ea40: 61 63 65 73 40 24 30 31 40 67 65 6f 64 65 40 40
 	  ea50: 51 45 41 41 40 58 5a 00 58 02 3f 62 65 67 69 6e
 	  ea60: 40 53 75 72 66 61 63 65 52 61 6e 67 65 40 3f 24
 	  ea70: 53 75 72 66 61 63 65 73 40 24 30 31 40 67 65 6f
 	  ea80: 64 65 40 40 51 45 42 41 41 45 42 56 31 32 33 40
-	  ea90: 58 5a 00 00 37 03 3f 65 6e 64 40 53 75 72 66 61
+	  ea90: 58 5a 00 00 3b 03 3f 65 6e 64 40 53 75 72 66 61
 	  eaa0: 63 65 52 61 6e 67 65 40 3f 24 53 75 72 66 61 63
 	  eab0: 65 73 40 24 30 31 40 67 65 6f 64 65 40 40 51 45
 	  eac0: 42 41 41 45 42 56 31 32 33 40 58 5a 00 00 e5 01
 	  ead0: 3f 3f 44 53 75 72 66 61 63 65 52 61 6e 67 65 40
 	  eae0: 3f 24 53 75 72 66 61 63 65 73 40 24 30 31 40 67
 	  eaf0: 65 6f 64 65 40 40 51 45 42 41 41 45 42 56 3f 24
 	  eb00: 53 75 72 66 61 63 65 40 24 30 31 40 32 40 58 5a
-	  eb10: 00 00 45 03 3f 67 65 74 5f 6d 65 73 68 40 3f 24
+	  eb10: 00 00 49 03 3f 67 65 74 5f 6d 65 73 68 40 3f 24
 	  eb20: 53 75 72 66 61 63 65 40 24 30 31 40 67 65 6f 64
 	  eb30: 65 40 40 41 45 42 41 41 45 42 56 3f 24 53 75 72
 	  eb40: 66 61 63 65 4d 65 73 68 40 24 30 31 40 32 40 58
 	  eb50: 5a 00 c2 01 3f 3f 39 53 75 72 66 61 63 65 52 61
 	  eb60: 6e 67 65 42 61 73 65 40 3f 24 53 75 72 66 61 63
 	  eb70: 65 73 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
 	  eb80: 42 41 5f 4e 41 45 42 56 30 31 32 40 40 5a 00 00
@@ -12543,23 +12543,23 @@
 	  ebf0: 40 41 45 42 56 30 31 32 40 40 5a 00 9c 01 3f 3f
 	  ec00: 31 53 75 72 66 61 63 65 52 61 6e 67 65 40 3f 24
 	  ec10: 53 75 72 66 61 63 65 73 40 24 30 32 40 67 65 6f
 	  ec20: 64 65 40 40 51 45 41 41 40 58 5a 00 59 02 3f 62
 	  ec30: 65 67 69 6e 40 53 75 72 66 61 63 65 52 61 6e 67
 	  ec40: 65 40 3f 24 53 75 72 66 61 63 65 73 40 24 30 32
 	  ec50: 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42 56
-	  ec60: 31 32 33 40 58 5a 00 00 38 03 3f 65 6e 64 40 53
+	  ec60: 31 32 33 40 58 5a 00 00 3c 03 3f 65 6e 64 40 53
 	  ec70: 75 72 66 61 63 65 52 61 6e 67 65 40 3f 24 53 75
 	  ec80: 72 66 61 63 65 73 40 24 30 32 40 67 65 6f 64 65
 	  ec90: 40 40 51 45 42 41 41 45 42 56 31 32 33 40 58 5a
 	  eca0: 00 00 e6 01 3f 3f 44 53 75 72 66 61 63 65 52 61
 	  ecb0: 6e 67 65 40 3f 24 53 75 72 66 61 63 65 73 40 24
 	  ecc0: 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 41 45
 	  ecd0: 42 56 3f 24 53 75 72 66 61 63 65 40 24 30 32 40
-	  ece0: 32 40 58 5a 00 00 46 03 3f 67 65 74 5f 6d 65 73
+	  ece0: 32 40 58 5a 00 00 4a 03 3f 67 65 74 5f 6d 65 73
 	  ecf0: 68 40 3f 24 53 75 72 66 61 63 65 40 24 30 32 40
 	  ed00: 67 65 6f 64 65 40 40 41 45 42 41 41 45 42 56 3f
 	  ed10: 24 53 75 72 66 61 63 65 4d 65 73 68 40 24 30 32
 	  ed20: 40 32 40 58 5a 00 5e 02 3f 62 6c 6f 63 6b 73 40
 	  ed30: 3f 24 42 6c 6f 63 6b 73 40 24 30 32 40 67 65 6f
 	  ed40: 64 65 40 40 51 45 42 41 3f 41 56 42 6c 6f 63 6b
 	  ed50: 52 61 6e 67 65 40 31 32 40 58 5a 00 b3 01 3f 3f
@@ -12574,97 +12574,97 @@
 	  ede0: 30 32 40 67 65 6f 64 65 40 40 51 45 41 41 40 41
 	  edf0: 45 42 56 30 31 32 40 40 5a 00 5e 01 3f 3f 31 42
 	  ee00: 6c 6f 63 6b 52 61 6e 67 65 40 3f 24 42 6c 6f 63
 	  ee10: 6b 73 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
 	  ee20: 41 41 40 58 5a 00 36 02 3f 62 65 67 69 6e 40 42
 	  ee30: 6c 6f 63 6b 52 61 6e 67 65 40 3f 24 42 6c 6f 63
 	  ee40: 6b 73 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
-	  ee50: 42 41 41 45 42 56 31 32 33 40 58 5a 00 00 15 03
+	  ee50: 42 41 41 45 42 56 31 32 33 40 58 5a 00 00 19 03
 	  ee60: 3f 65 6e 64 40 42 6c 6f 63 6b 52 61 6e 67 65 40
 	  ee70: 3f 24 42 6c 6f 63 6b 73 40 24 30 32 40 67 65 6f
 	  ee80: 64 65 40 40 51 45 42 41 41 45 42 56 31 32 33 40
 	  ee90: 58 5a 00 00 c3 01 3f 3f 44 42 6c 6f 63 6b 52 61
 	  eea0: 6e 67 65 40 3f 24 42 6c 6f 63 6b 73 40 24 30 32
 	  eeb0: 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42 56
 	  eec0: 3f 24 42 6c 6f 63 6b 40 24 30 32 40 32 40 58 5a
-	  eed0: 00 00 44 03 3f 67 65 74 5f 6d 65 73 68 40 3f 24
+	  eed0: 00 00 48 03 3f 67 65 74 5f 6d 65 73 68 40 3f 24
 	  eee0: 42 6c 6f 63 6b 40 24 30 32 40 67 65 6f 64 65 40
 	  eef0: 40 41 45 42 41 41 45 42 56 3f 24 53 6f 6c 69 64
-	  ef00: 4d 65 73 68 40 24 30 32 40 32 40 58 5a 00 ec 03
+	  ef00: 4d 65 73 68 40 24 30 32 40 32 40 58 5a 00 f1 03
 	  ef10: 3f 6e 62 5f 75 6e 69 71 75 65 5f 76 65 72 74 69
 	  ef20: 63 65 73 40 56 65 72 74 65 78 49 64 65 6e 74 69
 	  ef30: 66 69 65 72 40 67 65 6f 64 65 40 40 51 45 42 41
-	  ef40: 49 58 5a 00 80 02 3f 63 6f 6d 70 6f 6e 65 6e 74
+	  ef40: 49 58 5a 00 84 02 3f 63 6f 6d 70 6f 6e 65 6e 74
 	  ef50: 5f 6d 65 73 68 5f 76 65 72 74 69 63 65 73 40 56
 	  ef60: 65 72 74 65 78 49 64 65 6e 74 69 66 69 65 72 40
 	  ef70: 67 65 6f 64 65 40 40 51 45 42 41 41 45 42 56 3f
 	  ef80: 24 76 65 63 74 6f 72 40 55 43 6f 6d 70 6f 6e 65
 	  ef90: 6e 74 4d 65 73 68 56 65 72 74 65 78 40 67 65 6f
 	  efa0: 64 65 40 40 56 3f 24 61 6c 6c 6f 63 61 74 6f 72
 	  efb0: 40 55 43 6f 6d 70 6f 6e 65 6e 74 4d 65 73 68 56
 	  efc0: 65 72 74 65 78 40 67 65 6f 64 65 40 40 40 73 74
-	  efd0: 64 40 40 40 73 74 64 40 40 49 40 5a 00 00 a9 02
+	  efd0: 64 40 40 40 73 74 64 40 40 49 40 5a 00 00 ad 02
 	  efe0: 3f 63 6f 72 6e 65 72 40 3f 24 43 6f 72 6e 65 72
 	  eff0: 73 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42
 	  f000: 41 41 45 42 56 3f 24 43 6f 72 6e 65 72 40 24 30
 	  f010: 32 40 32 40 41 45 42 55 75 75 69 64 40 32 40 40
-	  f020: 5a 00 7b 03 3f 6c 69 6e 65 40 3f 24 4c 69 6e 65
+	  f020: 5a 00 7f 03 3f 6c 69 6e 65 40 3f 24 4c 69 6e 65
 	  f030: 73 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42
 	  f040: 41 41 45 42 56 3f 24 4c 69 6e 65 40 24 30 32 40
 	  f050: 32 40 41 45 42 55 75 75 69 64 40 32 40 40 5a 00
-	  f060: 47 04 3f 73 75 72 66 61 63 65 40 3f 24 53 75 72
+	  f060: 4d 04 3f 73 75 72 66 61 63 65 40 3f 24 53 75 72
 	  f070: 66 61 63 65 73 40 24 30 32 40 67 65 6f 64 65 40
 	  f080: 40 51 45 42 41 41 45 42 56 3f 24 53 75 72 66 61
 	  f090: 63 65 40 24 30 32 40 32 40 41 45 42 55 75 75 69
 	  f0a0: 64 40 32 40 40 5a 00 00 5b 02 3f 62 6c 6f 63 6b
 	  f0b0: 40 3f 24 42 6c 6f 63 6b 73 40 24 30 32 40 67 65
 	  f0c0: 6f 64 65 40 40 51 45 42 41 41 45 42 56 3f 24 42
 	  f0d0: 6c 6f 63 6b 40 24 30 32 40 32 40 41 45 42 55 75
-	  f0e0: 75 69 64 40 32 40 40 5a 00 00 a8 02 3f 63 6f 72
+	  f0e0: 75 69 64 40 32 40 40 5a 00 00 ac 02 3f 63 6f 72
 	  f0f0: 6e 65 72 40 3f 24 43 6f 72 6e 65 72 73 40 24 30
 	  f100: 31 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42
 	  f110: 56 3f 24 43 6f 72 6e 65 72 40 24 30 31 40 32 40
-	  f120: 41 45 42 55 75 75 69 64 40 32 40 40 5a 00 7a 03
+	  f120: 41 45 42 55 75 75 69 64 40 32 40 40 5a 00 7e 03
 	  f130: 3f 6c 69 6e 65 40 3f 24 4c 69 6e 65 73 40 24 30
 	  f140: 31 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42
 	  f150: 56 3f 24 4c 69 6e 65 40 24 30 31 40 32 40 41 45
-	  f160: 42 55 75 75 69 64 40 32 40 40 5a 00 46 04 3f 73
+	  f160: 42 55 75 75 69 64 40 32 40 40 5a 00 4c 04 3f 73
 	  f170: 75 72 66 61 63 65 40 3f 24 53 75 72 66 61 63 65
 	  f180: 73 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 42
 	  f190: 41 41 45 42 56 3f 24 53 75 72 66 61 63 65 40 24
 	  f1a0: 30 31 40 32 40 41 45 42 55 75 75 69 64 40 32 40
-	  f1b0: 40 5a 00 00 9c 03 3f 6d 65 73 68 40 3f 24 4c 69
+	  f1b0: 40 5a 00 00 a0 03 3f 6d 65 73 68 40 3f 24 4c 69
 	  f1c0: 6e 65 40 24 30 31 40 67 65 6f 64 65 40 40 51 45
 	  f1d0: 42 41 41 45 42 56 3f 24 45 64 67 65 64 43 75 72
-	  f1e0: 76 65 40 24 30 31 40 32 40 58 5a 00 9a 03 3f 6d
+	  f1e0: 76 65 40 24 30 31 40 32 40 58 5a 00 9e 03 3f 6d
 	  f1f0: 65 73 68 40 3f 24 43 6f 72 6e 65 72 40 24 30 31
 	  f200: 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42 56
 	  f210: 3f 24 50 6f 69 6e 74 53 65 74 40 24 30 31 40 32
-	  f220: 40 58 5a 00 9d 03 3f 6d 65 73 68 40 3f 24 4c 69
+	  f220: 40 58 5a 00 a1 03 3f 6d 65 73 68 40 3f 24 4c 69
 	  f230: 6e 65 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
 	  f240: 42 41 41 45 42 56 3f 24 45 64 67 65 64 43 75 72
-	  f250: 76 65 40 24 30 32 40 32 40 58 5a 00 9b 03 3f 6d
+	  f250: 76 65 40 24 30 32 40 32 40 58 5a 00 9f 03 3f 6d
 	  f260: 65 73 68 40 3f 24 43 6f 72 6e 65 72 40 24 30 32
 	  f270: 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42 56
 	  f280: 3f 24 50 6f 69 6e 74 53 65 74 40 24 30 32 40 32
 	  f290: 40 58 5a 00 b8 00 3f 3f 30 43 6f 6d 70 6f 6e 65
 	  f2a0: 6e 74 4d 65 73 68 56 65 72 74 65 78 40 67 65 6f
 	  f2b0: 64 65 40 40 51 45 41 41 40 56 43 6f 6d 70 6f 6e
 	  f2c0: 65 6e 74 49 44 40 31 40 49 40 5a 00 69 01 3f 3f
 	  f2d0: 31 43 6f 6d 70 6f 6e 65 6e 74 4d 65 73 68 56 65
 	  f2e0: 72 74 65 78 40 67 65 6f 64 65 40 40 51 45 41 41
-	  f2f0: 40 58 5a 00 51 04 3f 75 6e 69 71 75 65 5f 76 65
+	  f2f0: 40 58 5a 00 57 04 3f 75 6e 69 71 75 65 5f 76 65
 	  f300: 72 74 65 78 40 56 65 72 74 65 78 49 64 65 6e 74
 	  f310: 69 66 69 65 72 40 67 65 6f 64 65 40 40 51 45 42
 	  f320: 41 49 41 45 42 55 43 6f 6d 70 6f 6e 65 6e 74 4d
 	  f330: 65 73 68 56 65 72 74 65 78 40 32 40 40 5a 00 00
-	  f340: 7f 03 3f 6c 69 6e 65 73 40 3f 24 4c 69 6e 65 73
+	  f340: 83 03 3f 6c 69 6e 65 73 40 3f 24 4c 69 6e 65 73
 	  f350: 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41
 	  f360: 3f 41 56 4c 69 6e 65 52 61 6e 67 65 40 31 32 40
-	  f370: 58 5a 00 00 7e 03 3f 6c 69 6e 65 73 40 3f 24 4c
+	  f370: 58 5a 00 00 82 03 3f 6c 69 6e 65 73 40 3f 24 4c
 	  f380: 69 6e 65 73 40 24 30 31 40 67 65 6f 64 65 40 40
 	  f390: 51 45 42 41 3f 41 56 4c 69 6e 65 52 61 6e 67 65
 	  f3a0: 40 31 32 40 58 5a 00 00 bc 01 3f 3f 39 4c 69 6e
 	  f3b0: 65 52 61 6e 67 65 42 61 73 65 40 3f 24 4c 69 6e
 	  f3c0: 65 73 40 24 30 31 40 67 65 6f 64 65 40 40 51 45
 	  f3d0: 42 41 5f 4e 41 45 42 56 30 31 32 40 40 5a 00 00
 	  f3e0: f8 01 3f 3f 45 4c 69 6e 65 52 61 6e 67 65 42 61
@@ -12675,15 +12675,15 @@
 	  f430: 51 45 41 41 40 41 45 42 56 30 31 32 40 40 5a 00
 	  f440: 86 01 3f 3f 31 4c 69 6e 65 52 61 6e 67 65 40 3f
 	  f450: 24 4c 69 6e 65 73 40 24 30 31 40 67 65 6f 64 65
 	  f460: 40 40 51 45 41 41 40 58 5a 00 53 02 3f 62 65 67
 	  f470: 69 6e 40 4c 69 6e 65 52 61 6e 67 65 40 3f 24 4c
 	  f480: 69 6e 65 73 40 24 30 31 40 67 65 6f 64 65 40 40
 	  f490: 51 45 42 41 41 45 42 56 31 32 33 40 58 5a 00 00
-	  f4a0: 32 03 3f 65 6e 64 40 4c 69 6e 65 52 61 6e 67 65
+	  f4a0: 36 03 3f 65 6e 64 40 4c 69 6e 65 52 61 6e 67 65
 	  f4b0: 40 3f 24 4c 69 6e 65 73 40 24 30 31 40 67 65 6f
 	  f4c0: 64 65 40 40 51 45 42 41 41 45 42 56 31 32 33 40
 	  f4d0: 58 5a 00 00 e0 01 3f 3f 44 4c 69 6e 65 52 61 6e
 	  f4e0: 67 65 40 3f 24 4c 69 6e 65 73 40 24 30 31 40 67
 	  f4f0: 65 6f 64 65 40 40 51 45 42 41 41 45 42 56 3f 24
 	  f500: 4c 69 6e 65 40 24 30 31 40 32 40 58 5a 00 bd 01
 	  f510: 3f 3f 39 4c 69 6e 65 52 61 6e 67 65 42 61 73 65
@@ -12697,38 +12697,38 @@
 	  f590: 65 6f 64 65 40 40 51 45 41 41 40 41 45 42 56 30
 	  f5a0: 31 32 40 40 5a 00 87 01 3f 3f 31 4c 69 6e 65 52
 	  f5b0: 61 6e 67 65 40 3f 24 4c 69 6e 65 73 40 24 30 32
 	  f5c0: 40 67 65 6f 64 65 40 40 51 45 41 41 40 58 5a 00
 	  f5d0: 54 02 3f 62 65 67 69 6e 40 4c 69 6e 65 52 61 6e
 	  f5e0: 67 65 40 3f 24 4c 69 6e 65 73 40 24 30 32 40 67
 	  f5f0: 65 6f 64 65 40 40 51 45 42 41 41 45 42 56 31 32
-	  f600: 33 40 58 5a 00 00 33 03 3f 65 6e 64 40 4c 69 6e
+	  f600: 33 40 58 5a 00 00 37 03 3f 65 6e 64 40 4c 69 6e
 	  f610: 65 52 61 6e 67 65 40 3f 24 4c 69 6e 65 73 40 24
 	  f620: 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 41 45
 	  f630: 42 56 31 32 33 40 58 5a 00 00 e1 01 3f 3f 44 4c
 	  f640: 69 6e 65 52 61 6e 67 65 40 3f 24 4c 69 6e 65 73
 	  f650: 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41
 	  f660: 41 45 42 56 3f 24 4c 69 6e 65 40 24 30 32 40 32
-	  f670: 40 58 5a 00 dd 02 3f 63 72 65 61 74 65 5f 73 75
+	  f670: 40 58 5a 00 e1 02 3f 63 72 65 61 74 65 5f 73 75
 	  f680: 72 66 61 63 65 5f 6d 65 73 68 65 73 5f 61 61 62
 	  f690: 62 5f 74 72 65 65 73 40 67 65 6f 64 65 40 40 59
 	  f6a0: 41 3f 41 55 3f 24 4d 6f 64 65 6c 4d 65 73 68 65
 	  f6b0: 73 41 41 42 42 54 72 65 65 40 24 30 32 40 31 40
-	  f6c0: 41 45 42 56 42 52 65 70 40 31 40 40 5a 00 dc 02
+	  f6c0: 41 45 42 56 42 52 65 70 40 31 40 40 5a 00 e0 02
 	  f6d0: 3f 63 72 65 61 74 65 5f 73 75 72 66 61 63 65 5f
 	  f6e0: 6d 65 73 68 65 73 5f 61 61 62 62 5f 74 72 65 65
 	  f6f0: 73 40 67 65 6f 64 65 40 40 59 41 3f 41 55 3f 24
 	  f700: 4d 6f 64 65 6c 4d 65 73 68 65 73 41 41 42 42 54
 	  f710: 72 65 65 40 24 30 31 40 31 40 41 45 42 56 53 65
-	  f720: 63 74 69 6f 6e 40 31 40 40 5a 00 00 4c 03 3f 68
+	  f720: 63 74 69 6f 6e 40 31 40 40 5a 00 00 50 03 3f 68
 	  f730: 61 73 5f 63 6f 6d 70 6f 6e 65 6e 74 5f 6d 65 73
 	  f740: 68 5f 76 65 72 74 69 63 65 73 40 56 65 72 74 65
 	  f750: 78 49 64 65 6e 74 69 66 69 65 72 40 67 65 6f 64
 	  f760: 65 40 40 51 45 42 41 5f 4e 49 41 45 42 55 75 75
-	  f770: 69 64 40 32 40 40 5a 00 ad 02 3f 63 6f 72 6e 65
+	  f770: 69 64 40 32 40 40 5a 00 b1 02 3f 63 6f 72 6e 65
 	  f780: 72 73 40 3f 24 43 6f 72 6e 65 72 73 40 24 30 32
 	  f790: 40 67 65 6f 64 65 40 40 51 45 42 41 3f 41 56 43
 	  f7a0: 6f 72 6e 65 72 52 61 6e 67 65 40 31 32 40 58 5a
 	  f7b0: 00 00 b7 01 3f 3f 39 43 6f 72 6e 65 72 52 61 6e
 	  f7c0: 67 65 42 61 73 65 40 3f 24 43 6f 72 6e 65 72 73
 	  f7d0: 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41
 	  f7e0: 5f 4e 41 45 42 56 30 31 32 40 40 5a 00 00 eb 01
@@ -12740,23 +12740,23 @@
 	  f840: 65 6f 64 65 40 40 51 45 41 41 40 41 45 42 56 30
 	  f850: 31 32 40 40 5a 00 6b 01 3f 3f 31 43 6f 72 6e 65
 	  f860: 72 52 61 6e 67 65 40 3f 24 43 6f 72 6e 65 72 73
 	  f870: 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 41 41
 	  f880: 40 58 5a 00 3f 02 3f 62 65 67 69 6e 40 43 6f 72
 	  f890: 6e 65 72 52 61 6e 67 65 40 3f 24 43 6f 72 6e 65
 	  f8a0: 72 73 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
-	  f8b0: 42 41 41 45 42 56 31 32 33 40 58 5a 00 00 1e 03
+	  f8b0: 42 41 41 45 42 56 31 32 33 40 58 5a 00 00 22 03
 	  f8c0: 3f 65 6e 64 40 43 6f 72 6e 65 72 52 61 6e 67 65
 	  f8d0: 40 3f 24 43 6f 72 6e 65 72 73 40 24 30 32 40 67
 	  f8e0: 65 6f 64 65 40 40 51 45 42 41 41 45 42 56 31 32
 	  f8f0: 33 40 58 5a 00 00 cc 01 3f 3f 44 43 6f 72 6e 65
 	  f900: 72 52 61 6e 67 65 40 3f 24 43 6f 72 6e 65 72 73
 	  f910: 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41
 	  f920: 41 45 42 56 3f 24 43 6f 72 6e 65 72 40 24 30 32
-	  f930: 40 32 40 58 5a 00 7f 02 3f 63 6f 6d 70 6f 6e 65
+	  f930: 40 32 40 58 5a 00 83 02 3f 63 6f 6d 70 6f 6e 65
 	  f940: 6e 74 5f 6d 65 73 68 5f 76 65 72 74 69 63 65 73
 	  f950: 40 56 65 72 74 65 78 49 64 65 6e 74 69 66 69 65
 	  f960: 72 40 67 65 6f 64 65 40 40 51 45 42 41 3f 41 56
 	  f970: 3f 24 76 65 63 74 6f 72 40 55 43 6f 6d 70 6f 6e
 	  f980: 65 6e 74 4d 65 73 68 56 65 72 74 65 78 40 67 65
 	  f990: 6f 64 65 40 40 56 3f 24 61 6c 6c 6f 63 61 74 6f
 	  f9a0: 72 40 55 43 6f 6d 70 6f 6e 65 6e 74 4d 65 73 68
@@ -12764,22 +12764,22 @@
 	  f9c0: 74 64 40 40 40 73 74 64 40 40 49 41 45 42 56 3f
 	  f9d0: 24 4e 61 6d 65 64 54 79 70 65 40 56 3f 24 62 61
 	  f9e0: 73 69 63 5f 73 74 72 69 6e 67 40 44 55 3f 24 63
 	  f9f0: 68 61 72 5f 74 72 61 69 74 73 40 44 40 73 74 64
 	  fa00: 40 40 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40 44
 	  fa10: 40 32 40 40 73 74 64 40 40 55 43 6f 6d 70 6f 6e
 	  fa20: 65 6e 74 54 61 67 40 67 65 6f 64 65 40 40 40 32
-	  fa30: 40 40 5a 00 da 03 3f 6e 62 5f 69 6e 63 69 64 65
+	  fa30: 40 40 5a 00 df 03 3f 6e 62 5f 69 6e 63 69 64 65
 	  fa40: 6e 63 65 73 40 52 65 6c 61 74 69 6f 6e 73 68 69
 	  fa50: 70 73 40 67 65 6f 64 65 40 40 51 45 42 41 49 41
-	  fa60: 45 42 55 75 75 69 64 40 32 40 40 5a 00 00 d9 03
+	  fa60: 45 42 55 75 75 69 64 40 32 40 40 5a 00 00 de 03
 	  fa70: 3f 6e 62 5f 65 6d 62 65 64 64 69 6e 67 73 40 52
 	  fa80: 65 6c 61 74 69 6f 6e 73 68 69 70 73 40 67 65 6f
 	  fa90: 64 65 40 40 51 45 42 41 49 41 45 42 55 75 75 69
-	  faa0: 64 40 32 40 40 5a 00 00 67 03 3f 69 73 5f 62 6f
+	  faa0: 64 40 32 40 40 5a 00 00 6b 03 3f 69 73 5f 62 6f
 	  fab0: 75 6e 64 61 72 79 40 52 65 6c 61 74 69 6f 6e 73
 	  fac0: 68 69 70 73 40 67 65 6f 64 65 40 40 51 45 42 41
 	  fad0: 5f 4e 41 45 42 55 75 75 69 64 40 32 40 30 40 5a
 	  fae0: 00 00 b8 01 3f 3f 39 45 6d 62 65 64 64 69 6e 67
 	  faf0: 52 61 6e 67 65 49 74 65 72 61 74 6f 72 40 52 65
 	  fb00: 6c 61 74 69 6f 6e 73 68 69 70 73 40 67 65 6f 64
 	  fb10: 65 40 40 51 45 42 41 5f 4e 41 45 42 56 30 31 32
@@ -12794,32 +12794,32 @@
 	  fba0: 49 44 40 32 40 58 5a 00 70 01 3f 3f 31 45 6d 62
 	  fbb0: 65 64 64 69 6e 67 52 61 6e 67 65 40 52 65 6c 61
 	  fbc0: 74 69 6f 6e 73 68 69 70 73 40 67 65 6f 64 65 40
 	  fbd0: 40 51 45 41 41 40 58 5a 00 00 ca 00 3f 3f 30 45
 	  fbe0: 6d 62 65 64 64 69 6e 67 52 61 6e 67 65 40 52 65
 	  fbf0: 6c 61 74 69 6f 6e 73 68 69 70 73 40 67 65 6f 64
 	  fc00: 65 40 40 51 45 41 41 40 41 45 42 56 30 31 32 40
-	  fc10: 40 5a 00 00 14 03 3f 65 6d 62 65 64 64 69 6e 67
+	  fc10: 40 5a 00 00 18 03 3f 65 6d 62 65 64 64 69 6e 67
 	  fc20: 73 40 52 65 6c 61 74 69 6f 6e 73 68 69 70 73 40
 	  fc30: 67 65 6f 64 65 40 40 51 45 42 41 3f 41 56 45 6d
 	  fc40: 62 65 64 64 69 6e 67 52 61 6e 67 65 40 31 32 40
-	  fc50: 41 45 42 55 75 75 69 64 40 32 40 40 5a 00 72 03
+	  fc50: 41 45 42 55 75 75 69 64 40 32 40 40 5a 00 76 03
 	  fc60: 3f 69 73 5f 69 6e 74 65 72 6e 61 6c 40 52 65 6c
 	  fc70: 61 74 69 6f 6e 73 68 69 70 73 40 67 65 6f 64 65
 	  fc80: 40 40 51 45 42 41 5f 4e 41 45 42 55 75 75 69 64
-	  fc90: 40 32 40 30 40 5a 00 00 65 03 3f 69 73 5f 62 6f
+	  fc90: 40 32 40 30 40 5a 00 00 69 03 3f 69 73 5f 62 6f
 	  fca0: 75 6e 64 61 72 79 40 42 52 65 70 40 67 65 6f 64
 	  fcb0: 65 40 40 51 45 42 41 5f 4e 41 45 42 56 3f 24 4c
 	  fcc0: 69 6e 65 40 24 30 32 40 32 40 41 45 42 56 3f 24
 	  fcd0: 53 75 72 66 61 63 65 40 24 30 32 40 32 40 40 5a
-	  fce0: 00 00 70 03 3f 69 73 5f 69 6e 74 65 72 6e 61 6c
+	  fce0: 00 00 74 03 3f 69 73 5f 69 6e 74 65 72 6e 61 6c
 	  fcf0: 40 42 52 65 70 40 67 65 6f 64 65 40 40 51 45 42
 	  fd00: 41 5f 4e 41 45 42 56 3f 24 4c 69 6e 65 40 24 30
 	  fd10: 32 40 32 40 41 45 42 56 3f 24 53 75 72 66 61 63
-	  fd20: 65 40 24 30 32 40 32 40 40 5a 00 00 ac 02 3f 63
+	  fd20: 65 40 24 30 32 40 32 40 40 5a 00 00 b0 02 3f 63
 	  fd30: 6f 72 6e 65 72 73 40 3f 24 43 6f 72 6e 65 72 73
 	  fd40: 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 42 41
 	  fd50: 3f 41 56 43 6f 72 6e 65 72 52 61 6e 67 65 40 31
 	  fd60: 32 40 58 5a 00 00 b6 01 3f 3f 39 43 6f 72 6e 65
 	  fd70: 72 52 61 6e 67 65 42 61 73 65 40 3f 24 43 6f 72
 	  fd80: 6e 65 72 73 40 24 30 31 40 67 65 6f 64 65 40 40
 	  fd90: 51 45 42 41 5f 4e 41 45 42 56 30 31 32 40 40 5a
@@ -12832,15 +12832,15 @@
 	  fe00: 45 42 56 30 31 32 40 40 5a 00 6a 01 3f 3f 31 43
 	  fe10: 6f 72 6e 65 72 52 61 6e 67 65 40 3f 24 43 6f 72
 	  fe20: 6e 65 72 73 40 24 30 31 40 67 65 6f 64 65 40 40
 	  fe30: 51 45 41 41 40 58 5a 00 3e 02 3f 62 65 67 69 6e
 	  fe40: 40 43 6f 72 6e 65 72 52 61 6e 67 65 40 3f 24 43
 	  fe50: 6f 72 6e 65 72 73 40 24 30 31 40 67 65 6f 64 65
 	  fe60: 40 40 51 45 42 41 41 45 42 56 31 32 33 40 58 5a
-	  fe70: 00 00 1d 03 3f 65 6e 64 40 43 6f 72 6e 65 72 52
+	  fe70: 00 00 21 03 3f 65 6e 64 40 43 6f 72 6e 65 72 52
 	  fe80: 61 6e 67 65 40 3f 24 43 6f 72 6e 65 72 73 40 24
 	  fe90: 30 31 40 67 65 6f 64 65 40 40 51 45 42 41 41 45
 	  fea0: 42 56 31 32 33 40 58 5a 00 00 cb 01 3f 3f 44 43
 	  feb0: 6f 72 6e 65 72 52 61 6e 67 65 40 3f 24 43 6f 72
 	  fec0: 6e 65 72 73 40 24 30 31 40 67 65 6f 64 65 40 40
 	  fed0: 51 45 42 41 41 45 42 56 3f 24 43 6f 72 6e 65 72
 	  fee0: 40 24 30 31 40 32 40 58 5a 00 4f 70 65 6e 47 65
@@ -13173,148 +13173,148 @@
 	  11350: 40 3f 24 53 75 72 66 61 63 65 4d 65 73 68 40 24
 	  11360: 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 5f 4e
 	  11370: 49 40 5a 00 d2 05 3f 69 73 5f 76 65 72 74 65 78
 	  11380: 5f 6f 6e 5f 62 6f 72 64 65 72 40 3f 24 53 75 72
 	  11390: 66 61 63 65 4d 65 73 68 40 24 30 31 40 67 65 6f
 	  113a0: 64 65 40 40 51 45 42 41 5f 4e 49 40 5a 00 4f 70
 	  113b0: 65 6e 47 65 6f 64 65 5f 6d 65 73 68 2e 64 6c 6c
-	  113c0: 00 00 ae 00 3f 3f 30 3f 24 4e 4e 53 65 61 72 63
+	  113c0: 00 00 b3 00 3f 3f 30 3f 24 4e 4e 53 65 61 72 63
 	  113d0: 68 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 41
 	  113e0: 41 40 56 3f 24 76 65 63 74 6f 72 40 56 3f 24 50
 	  113f0: 6f 69 6e 74 40 24 30 31 40 67 65 6f 64 65 40 40
 	  11400: 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40 56 3f 24
 	  11410: 50 6f 69 6e 74 40 24 30 31 40 67 65 6f 64 65 40
 	  11420: 40 40 73 74 64 40 40 40 73 74 64 40 40 40 5a 00
-	  11430: 2d 01 3f 3f 31 3f 24 4e 4e 53 65 61 72 63 68 40
+	  11430: 32 01 3f 3f 31 3f 24 4e 4e 53 65 61 72 63 68 40
 	  11440: 24 30 31 40 67 65 6f 64 65 40 40 51 45 41 41 40
-	  11450: 58 5a 00 00 de 01 3f 63 6f 6c 6f 63 61 74 65 64
+	  11450: 58 5a 00 00 e9 01 3f 63 6f 6c 6f 63 61 74 65 64
 	  11460: 5f 69 6e 64 65 78 5f 6d 61 70 70 69 6e 67 40 3f
 	  11470: 24 4e 4e 53 65 61 72 63 68 40 24 30 31 40 67 65
 	  11480: 6f 64 65 40 40 51 45 42 41 3f 41 55 43 6f 6c 6f
 	  11490: 63 61 74 65 64 49 6e 66 6f 40 31 32 40 4e 40 5a
-	  114a0: 00 00 b0 00 3f 3f 30 3f 24 4e 4e 53 65 61 72 63
+	  114a0: 00 00 b5 00 3f 3f 30 3f 24 4e 4e 53 65 61 72 63
 	  114b0: 68 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 41
 	  114c0: 41 40 56 3f 24 76 65 63 74 6f 72 40 56 3f 24 50
 	  114d0: 6f 69 6e 74 40 24 30 32 40 67 65 6f 64 65 40 40
 	  114e0: 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40 56 3f 24
 	  114f0: 50 6f 69 6e 74 40 24 30 32 40 67 65 6f 64 65 40
 	  11500: 40 40 73 74 64 40 40 40 73 74 64 40 40 40 5a 00
-	  11510: 2e 01 3f 3f 31 3f 24 4e 4e 53 65 61 72 63 68 40
+	  11510: 33 01 3f 3f 31 3f 24 4e 4e 53 65 61 72 63 68 40
 	  11520: 24 30 32 40 67 65 6f 64 65 40 40 51 45 41 41 40
-	  11530: 58 5a 00 00 df 01 3f 63 6f 6c 6f 63 61 74 65 64
+	  11530: 58 5a 00 00 ea 01 3f 63 6f 6c 6f 63 61 74 65 64
 	  11540: 5f 69 6e 64 65 78 5f 6d 61 70 70 69 6e 67 40 3f
 	  11550: 24 4e 4e 53 65 61 72 63 68 40 24 30 32 40 67 65
 	  11560: 6f 64 65 40 40 51 45 42 41 3f 41 55 43 6f 6c 6f
 	  11570: 63 61 74 65 64 49 6e 66 6f 40 31 32 40 4e 40 5a
 	  11580: 00 00 19 00 3f 3f 24 70 6f 69 6e 74 5f 70 6f 69
 	  11590: 6e 74 5f 64 69 73 74 61 6e 63 65 40 24 30 31 40
 	  115a0: 67 65 6f 64 65 40 40 59 41 4e 41 45 42 56 3f 24
 	  115b0: 50 6f 69 6e 74 40 24 30 31 40 30 40 30 40 5a 00
 	  115c0: 1a 00 3f 3f 24 70 6f 69 6e 74 5f 70 6f 69 6e 74
 	  115d0: 5f 64 69 73 74 61 6e 63 65 40 24 30 32 40 67 65
 	  115e0: 6f 64 65 40 40 59 41 4e 41 45 42 56 3f 24 50 6f
-	  115f0: 69 6e 74 40 24 30 32 40 30 40 30 40 5a 00 65 02
+	  115f0: 69 6e 74 40 24 30 32 40 30 40 30 40 5a 00 71 02
 	  11600: 3f 73 65 67 6d 65 6e 74 5f 73 65 67 6d 65 6e 74
 	  11610: 5f 69 6e 74 65 72 73 65 63 74 69 6f 6e 5f 64 65
 	  11620: 74 65 63 74 69 6f 6e 40 67 65 6f 64 65 40 40 59
 	  11630: 41 3f 41 55 3f 24 70 61 69 72 40 57 34 50 6f 73
 	  11640: 69 74 69 6f 6e 40 67 65 6f 64 65 40 40 57 34 31
 	  11650: 32 40 40 73 74 64 40 40 41 45 42 56 3f 24 53 65
 	  11660: 67 6d 65 6e 74 40 24 30 31 40 31 40 30 40 5a 00
-	  11670: 68 02 3f 73 65 67 6d 65 6e 74 5f 74 72 69 61 6e
+	  11670: 74 02 3f 73 65 67 6d 65 6e 74 5f 74 72 69 61 6e
 	  11680: 67 6c 65 5f 69 6e 74 65 72 73 65 63 74 69 6f 6e
 	  11690: 5f 64 65 74 65 63 74 69 6f 6e 40 67 65 6f 64 65
 	  116a0: 40 40 59 41 3f 41 55 3f 24 70 61 69 72 40 57 34
 	  116b0: 50 6f 73 69 74 69 6f 6e 40 67 65 6f 64 65 40 40
 	  116c0: 57 34 31 32 40 40 73 74 64 40 40 41 45 42 56 3f
 	  116d0: 24 53 65 67 6d 65 6e 74 40 24 30 32 40 31 40 41
 	  116e0: 45 42 56 3f 24 54 72 69 61 6e 67 6c 65 40 24 30
-	  116f0: 32 40 31 40 40 5a 00 00 f4 00 3f 3f 30 3f 24 53
+	  116f0: 32 40 31 40 40 5a 00 00 f9 00 3f 3f 30 3f 24 53
 	  11700: 65 67 6d 65 6e 74 40 24 30 31 40 67 65 6f 64 65
 	  11710: 40 40 51 45 41 41 40 41 45 42 56 3f 24 50 6f 69
 	  11720: 6e 74 40 24 30 31 40 31 40 30 40 5a 00 00 29 00
 	  11730: 3f 3f 24 70 6f 69 6e 74 5f 74 72 69 61 6e 67 6c
 	  11740: 65 5f 70 6f 73 69 74 69 6f 6e 40 24 30 31 40 67
 	  11750: 65 6f 64 65 40 40 59 41 3f 41 57 34 50 6f 73 69
 	  11760: 74 69 6f 6e 40 30 40 41 45 42 56 3f 24 50 6f 69
 	  11770: 6e 74 40 24 30 31 40 30 40 41 45 42 56 3f 24 54
 	  11780: 72 69 61 6e 67 6c 65 40 24 30 31 40 30 40 40 5a
-	  11790: 00 00 8c 02 3f 76 65 72 74 69 63 65 73 40 3f 24
+	  11790: 00 00 98 02 3f 76 65 72 74 69 63 65 73 40 3f 24
 	  117a0: 47 65 6e 65 72 69 63 54 72 69 61 6e 67 6c 65 40
 	  117b0: 56 3f 24 72 65 66 65 72 65 6e 63 65 5f 77 72 61
 	  117c0: 70 70 65 72 40 24 24 43 42 56 3f 24 50 6f 69 6e
 	  117d0: 74 40 24 30 32 40 67 65 6f 64 65 40 40 40 73 74
 	  117e0: 64 40 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
 	  117f0: 42 41 41 45 42 56 3f 24 61 72 72 61 79 40 56 3f
 	  11800: 24 72 65 66 65 72 65 6e 63 65 5f 77 72 61 70 70
 	  11810: 65 72 40 24 24 43 42 56 3f 24 50 6f 69 6e 74 40
 	  11820: 24 30 32 40 67 65 6f 64 65 40 40 40 73 74 64 40
-	  11830: 40 24 30 32 40 73 74 64 40 40 58 5a 00 00 f8 00
+	  11830: 40 24 30 32 40 73 74 64 40 40 58 5a 00 00 fd 00
 	  11840: 3f 3f 30 3f 24 53 65 67 6d 65 6e 74 40 24 30 32
 	  11850: 40 67 65 6f 64 65 40 40 51 45 41 41 40 41 45 42
 	  11860: 56 3f 24 50 6f 69 6e 74 40 24 30 32 40 31 40 30
-	  11870: 40 5a 00 00 29 01 3f 3f 31 3f 24 41 41 42 42 54
+	  11870: 40 5a 00 00 2e 01 3f 3f 31 3f 24 41 41 42 42 54
 	  11880: 72 65 65 40 24 30 32 40 67 65 6f 64 65 40 40 51
-	  11890: 45 41 41 40 58 5a 00 00 1f 02 3f 6e 62 5f 62 62
+	  11890: 45 41 41 40 58 5a 00 00 2a 02 3f 6e 62 5f 62 62
 	  118a0: 6f 78 65 73 40 3f 24 41 41 42 42 54 72 65 65 40
 	  118b0: 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 49
-	  118c0: 58 5a 00 00 28 01 3f 3f 31 3f 24 41 41 42 42 54
+	  118c0: 58 5a 00 00 2d 01 3f 3f 31 3f 24 41 41 42 42 54
 	  118d0: 72 65 65 40 24 30 31 40 67 65 6f 64 65 40 40 51
-	  118e0: 45 41 41 40 58 5a 00 00 1e 02 3f 6e 62 5f 62 62
+	  118e0: 45 41 41 40 58 5a 00 00 29 02 3f 6e 62 5f 62 62
 	  118f0: 6f 78 65 73 40 3f 24 41 41 42 42 54 72 65 65 40
 	  11900: 24 30 31 40 67 65 6f 64 65 40 40 51 45 42 41 49
-	  11910: 58 5a 00 00 07 02 3f 69 73 5f 6c 65 61 66 40 49
+	  11910: 58 5a 00 00 12 02 3f 69 73 5f 6c 65 61 66 40 49
 	  11920: 6d 70 6c 40 3f 24 41 41 42 42 54 72 65 65 40 24
 	  11930: 30 32 40 67 65 6f 64 65 40 40 53 41 5f 4e 49 49
-	  11940: 40 5a 00 00 f9 01 3f 67 65 74 5f 72 65 63 75 72
+	  11940: 40 5a 00 00 04 02 3f 67 65 74 5f 72 65 63 75 72
 	  11950: 73 69 76 65 5f 69 74 65 72 61 74 6f 72 73 40 49
 	  11960: 6d 70 6c 40 3f 24 41 41 42 42 54 72 65 65 40 24
 	  11970: 30 32 40 67 65 6f 64 65 40 40 53 41 3f 41 55 49
 	  11980: 74 65 72 61 74 6f 72 40 31 32 33 40 49 49 49 40
-	  11990: 5a 00 27 02 3f 6e 6f 64 65 40 49 6d 70 6c 40 3f
+	  11990: 5a 00 32 02 3f 6e 6f 64 65 40 49 6d 70 6c 40 3f
 	  119a0: 24 41 41 42 42 54 72 65 65 40 24 30 32 40 67 65
 	  119b0: 6f 64 65 40 40 51 45 42 41 41 45 42 56 3f 24 42
 	  119c0: 6f 75 6e 64 69 6e 67 42 6f 78 40 24 30 32 40 33
-	  119d0: 40 49 40 5a 00 00 15 02 3f 6d 61 70 70 69 6e 67
+	  119d0: 40 49 40 5a 00 00 20 02 3f 6d 61 70 70 69 6e 67
 	  119e0: 5f 6d 6f 72 74 6f 6e 40 49 6d 70 6c 40 3f 24 41
 	  119f0: 41 42 42 54 72 65 65 40 24 30 32 40 67 65 6f 64
-	  11a00: 65 40 40 51 45 42 41 49 49 40 5a 00 06 02 3f 69
+	  11a00: 65 40 40 51 45 42 41 49 49 40 5a 00 11 02 3f 69
 	  11a10: 73 5f 6c 65 61 66 40 49 6d 70 6c 40 3f 24 41 41
 	  11a20: 42 42 54 72 65 65 40 24 30 31 40 67 65 6f 64 65
-	  11a30: 40 40 53 41 5f 4e 49 49 40 5a 00 00 f8 01 3f 67
+	  11a30: 40 40 53 41 5f 4e 49 49 40 5a 00 00 03 02 3f 67
 	  11a40: 65 74 5f 72 65 63 75 72 73 69 76 65 5f 69 74 65
 	  11a50: 72 61 74 6f 72 73 40 49 6d 70 6c 40 3f 24 41 41
 	  11a60: 42 42 54 72 65 65 40 24 30 31 40 67 65 6f 64 65
 	  11a70: 40 40 53 41 3f 41 55 49 74 65 72 61 74 6f 72 40
-	  11a80: 31 32 33 40 49 49 49 40 5a 00 26 02 3f 6e 6f 64
+	  11a80: 31 32 33 40 49 49 49 40 5a 00 31 02 3f 6e 6f 64
 	  11a90: 65 40 49 6d 70 6c 40 3f 24 41 41 42 42 54 72 65
 	  11aa0: 65 40 24 30 31 40 67 65 6f 64 65 40 40 51 45 42
 	  11ab0: 41 41 45 42 56 3f 24 42 6f 75 6e 64 69 6e 67 42
-	  11ac0: 6f 78 40 24 30 31 40 33 40 49 40 5a 00 00 14 02
+	  11ac0: 6f 78 40 24 30 31 40 33 40 49 40 5a 00 00 1f 02
 	  11ad0: 3f 6d 61 70 70 69 6e 67 5f 6d 6f 72 74 6f 6e 40
 	  11ae0: 49 6d 70 6c 40 3f 24 41 41 42 42 54 72 65 65 40
 	  11af0: 24 30 31 40 67 65 6f 64 65 40 40 51 45 42 41 49
-	  11b00: 49 40 5a 00 03 02 3f 69 6e 74 65 72 73 65 63 74
+	  11b00: 49 40 5a 00 0e 02 3f 69 6e 74 65 72 73 65 63 74
 	  11b10: 73 40 3f 24 42 6f 75 6e 64 69 6e 67 42 6f 78 40
 	  11b20: 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 5f
-	  11b30: 4e 41 45 42 56 31 32 40 40 5a 00 00 00 02 3f 69
+	  11b30: 4e 41 45 42 56 31 32 40 40 5a 00 00 0b 02 3f 69
 	  11b40: 6e 74 65 72 73 65 63 74 73 40 3f 24 42 6f 75 6e
 	  11b50: 64 69 6e 67 42 6f 78 40 24 30 31 40 67 65 6f 64
 	  11b60: 65 40 40 51 45 42 41 5f 4e 41 45 42 56 31 32 40
-	  11b70: 40 5a 00 00 85 02 3f 76 65 72 74 69 63 65 73 40
+	  11b70: 40 5a 00 00 91 02 3f 76 65 72 74 69 63 65 73 40
 	  11b80: 3f 24 47 65 6e 65 72 69 63 53 65 67 6d 65 6e 74
 	  11b90: 40 56 3f 24 72 65 66 65 72 65 6e 63 65 5f 77 72
 	  11ba0: 61 70 70 65 72 40 24 24 43 42 56 3f 24 50 6f 69
 	  11bb0: 6e 74 40 24 30 31 40 67 65 6f 64 65 40 40 40 73
 	  11bc0: 74 64 40 40 24 30 31 40 67 65 6f 64 65 40 40 51
 	  11bd0: 45 42 41 41 45 42 56 3f 24 61 72 72 61 79 40 56
 	  11be0: 3f 24 72 65 66 65 72 65 6e 63 65 5f 77 72 61 70
 	  11bf0: 70 65 72 40 24 24 43 42 56 3f 24 50 6f 69 6e 74
 	  11c00: 40 24 30 31 40 67 65 6f 64 65 40 40 40 73 74 64
-	  11c10: 40 40 24 30 31 40 73 74 64 40 40 58 5a 00 86 02
+	  11c10: 40 40 24 30 31 40 73 74 64 40 40 58 5a 00 92 02
 	  11c20: 3f 76 65 72 74 69 63 65 73 40 3f 24 47 65 6e 65
 	  11c30: 72 69 63 53 65 67 6d 65 6e 74 40 56 3f 24 72 65
 	  11c40: 66 65 72 65 6e 63 65 5f 77 72 61 70 70 65 72 40
 	  11c50: 24 24 43 42 56 3f 24 50 6f 69 6e 74 40 24 30 32
 	  11c60: 40 67 65 6f 64 65 40 40 40 73 74 64 40 40 24 30
 	  11c70: 32 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42
 	  11c80: 56 3f 24 61 72 72 61 79 40 56 3f 24 72 65 66 65
@@ -13325,45 +13325,45 @@
 	  11cd0: 6e 74 5f 74 72 69 61 6e 67 6c 65 5f 70 6f 73 69
 	  11ce0: 74 69 6f 6e 40 24 30 32 40 67 65 6f 64 65 40 40
 	  11cf0: 59 41 3f 41 57 34 50 6f 73 69 74 69 6f 6e 40 30
 	  11d00: 40 41 45 42 56 3f 24 50 6f 69 6e 74 40 24 30 32
 	  11d10: 40 30 40 41 45 42 56 3f 24 54 72 69 61 6e 67 6c
 	  11d20: 65 40 24 30 32 40 30 40 40 5a 00 00 4f 70 65 6e
 	  11d30: 47 65 6f 64 65 5f 67 65 6f 6d 65 74 72 79 2e 64
-	  11d40: 6c 6c 00 00 c0 00 3f 73 65 74 5f 69 6e 73 74 61
+	  11d40: 6c 6c 00 00 c1 00 3f 73 65 74 5f 69 6e 73 74 61
 	  11d50: 6e 63 65 40 53 69 6e 67 6c 65 74 6f 6e 40 67 65
 	  11d60: 6f 64 65 40 40 43 41 58 41 45 42 56 74 79 70 65
 	  11d70: 5f 69 6e 66 6f 40 40 50 45 41 56 31 32 40 40 5a
-	  11d80: 00 00 8c 00 3f 69 6e 73 74 61 6e 63 65 40 53 69
+	  11d80: 00 00 8d 00 3f 69 6e 73 74 61 6e 63 65 40 53 69
 	  11d90: 6e 67 6c 65 74 6f 6e 40 67 65 6f 64 65 40 40 43
 	  11da0: 41 50 45 41 56 31 32 40 41 45 42 56 74 79 70 65
 	  11db0: 5f 69 6e 66 6f 40 40 40 5a 00 31 00 3f 3f 31 4c
 	  11dc0: 69 62 72 61 72 79 40 67 65 6f 64 65 40 40 55 45
 	  11dd0: 41 41 40 58 5a 00 1a 00 3f 3f 30 4c 69 62 72 61
 	  11de0: 72 79 40 67 65 6f 64 65 40 40 49 45 41 41 40 58
 	  11df0: 5a 00 59 00 3f 63 61 6c 6c 5f 69 6e 69 74 69 61
 	  11e00: 6c 69 7a 65 40 4c 69 62 72 61 72 79 40 67 65 6f
 	  11e10: 64 65 40 40 49 45 41 41 58 50 45 42 44 40 5a 00
-	  11e20: 97 00 3f 6c 6f 67 5f 69 6e 66 6f 40 4c 6f 67 67
+	  11e20: 98 00 3f 6c 6f 67 5f 69 6e 66 6f 40 4c 6f 67 67
 	  11e30: 65 72 40 67 65 6f 64 65 40 40 43 41 58 41 45 42
 	  11e40: 56 3f 24 62 61 73 69 63 5f 73 74 72 69 6e 67 40
 	  11e50: 44 55 3f 24 63 68 61 72 5f 74 72 61 69 74 73 40
 	  11e60: 44 40 73 74 64 40 40 56 3f 24 61 6c 6c 6f 63 61
 	  11e70: 74 6f 72 40 44 40 32 40 40 73 74 64 40 40 40 5a
 	  11e80: 00 00 7f 00 3f 69 64 40 49 64 65 6e 74 69 66 69
 	  11e90: 65 72 40 67 65 6f 64 65 40 40 51 45 42 41 41 45
 	  11ea0: 42 55 75 75 69 64 40 32 40 58 5a 00 45 00 3f 3f
 	  11eb0: 38 75 75 69 64 40 67 65 6f 64 65 40 40 51 45 42
-	  11ec0: 41 5f 4e 41 45 42 55 30 31 40 40 5a 00 00 c7 00
+	  11ec0: 41 5f 4e 41 45 42 55 30 31 40 40 5a 00 00 c8 00
 	  11ed0: 3f 73 74 72 69 6e 67 40 75 75 69 64 40 67 65 6f
 	  11ee0: 64 65 40 40 51 45 42 41 3f 41 56 3f 24 62 61 73
 	  11ef0: 69 63 5f 73 74 72 69 6e 67 40 44 55 3f 24 63 68
 	  11f00: 61 72 5f 74 72 61 69 74 73 40 44 40 73 74 64 40
 	  11f10: 40 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40 44 40
-	  11f20: 32 40 40 73 74 64 40 40 58 5a 00 00 99 00 3f 6c
+	  11f20: 32 40 40 73 74 64 40 40 58 5a 00 00 9a 00 3f 6c
 	  11f30: 6f 67 5f 77 61 72 6e 40 4c 6f 67 67 65 72 40 67
 	  11f40: 65 6f 64 65 40 40 43 41 58 41 45 42 56 3f 24 62
 	  11f50: 61 73 69 63 5f 73 74 72 69 6e 67 40 44 55 3f 24
 	  11f60: 63 68 61 72 5f 74 72 61 69 74 73 40 44 40 73 74
 	  11f70: 64 40 40 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40
 	  11f80: 44 40 32 40 40 73 74 64 40 40 40 5a 00 00 47 00
 	  11f90: 3f 3f 4d 75 75 69 64 40 67 65 6f 64 65 40 40 51
@@ -100922,15 +100922,15 @@
    18004f01a:	(bad)
    18004f01b:	addb   $0x0,(%rcx)
    18004f01e:	add    %al,(%rax)
    18004f020:	rclb   0x18006(%rsi)
    18004f026:	add    %al,(%rax)
    18004f028:	add    %al,(%rax)
    18004f02a:	add    %al,(%rax)
-   18004f02c:	mov    $0x645ca3,%edx
+   18004f02c:	rex.RX mov %fs,0x0(%rsp,%r12,2)
    18004f031:	add    %al,(%rax)
    18004f033:	add    %cl,-0x14000000(%rip)        # 0x16c04f039
    18004f039:	add    (%rax),%al
    18004f03b:	add    %bl,-0x16e3fffc(,%rdi,8)
    18004f042:	add    $0x0,%al
 	...
    18004f050:	cmp    %al,(%rcx)
@@ -137601,15 +137601,15 @@
    18006414f:	add    %al,-0x7c(%rdx)
    180064152:	(bad)
    180064153:	add    %al,(%rax)
    180064155:	add    %al,(%rax)
    180064157:	add    %dh,0x684(%rdx)
 	...
    180064165:	add    %al,(%rax)
-   180064167:	add    %bl,0x3(%rdx)
+   180064167:	add    %bl,0x3(%rsi)
    18006416a:	(bad)
    18006416b:	imul   $0x6c616974,0x69(%rsi),%ebp
    180064172:	imul   $0x65704f40,0x65(%rdx),%edi
    180064179:	outsb  %ds:(%rsi),(%dx)
    18006417a:	rex.RXB
    18006417b:	outsl  %gs:(%rsi),(%dx)
    18006417d:	fs rex.WRB outsl %gs:(%rsi),(%dx)
@@ -137618,15 +137618,16 @@
    18006418c:	outsl  %gs:(%esi),(%dx)
    18006418f:	fs gs rex
    180064192:	rex push %rbx
    180064194:	pop    %r8
    180064196:	pop    %rax
    180064197:	pop    %rdx
    180064198:	add    %al,(%rax)
-   18006419a:	rex.WR add $0x3f,%al
+   18006419a:	push   %rdx
+   18006419b:	add    $0x3f,%al
    18006419d:	jae    0x180064214
    18006419f:	jb     0x180064207
    1800641a1:	(bad)
    1800641a2:	movsxd 0x73(%rbp),%esp
    1800641a5:	rex (bad)
    1800641a7:	and    $0x53,%al
    1800641a9:	jne    0x18006421d
@@ -137646,15 +137647,15 @@
    1800641c6:	data16 (bad)
    1800641c8:	movsxd 0x52(%rbp),%esp
    1800641cb:	(bad)
    1800641cc:	outsb  %ds:(%rsi),(%dx)
    1800641cd:	rex xor %esi,%gs:(%edx)
    1800641d2:	rex pop %rax
    1800641d4:	pop    %rdx
-   1800641d5:	add    %cl,0x4(%rbx)
+   1800641d5:	add    %dl,0x4(%rcx)
    1800641d8:	(bad)
    1800641d9:	jae    0x180064250
    1800641db:	jb     0x180064243
    1800641dd:	(bad)
    1800641de:	movsxd 0x73(%rbp),%esp
    1800641e1:	rex (bad)
    1800641e3:	and    $0x53,%al
@@ -137811,16 +137812,16 @@
    18006431c:	rex.B
    18006431d:	rex.RB
    18006431e:	rex.X push %rsi
    180064320:	xor    %esi,(%rdx)
    180064322:	xor    0x58(%rax),%eax
    180064325:	pop    %rdx
    180064326:	add    %al,(%rax)
-   180064328:	(bad)
-   180064329:	add    (%rdi),%edi
+   180064328:	cmp    (%rbx),%eax
+   18006432a:	(bad)
    18006432b:	outsb  %gs:(%rsi),(%dx)
    18006432d:	fs rex push %rbx
    180064330:	jne    0x1800643a4
    180064332:	data16 (bad)
    180064334:	movsxd 0x52(%rbp),%esp
    180064337:	(bad)
    180064338:	outsb  %ds:(%rsi),(%dx)
@@ -137875,15 +137876,15 @@
    180064397:	data16 (bad)
    180064399:	movsxd 0x40(%rbp),%esp
    18006439c:	and    $0x30,%al
    18006439e:	xor    %eax,0x32(%rax)
    1800643a1:	rex pop %rax
    1800643a3:	pop    %rdx
    1800643a4:	add    %al,(%rax)
-   1800643a6:	add    (%r15),%r15d
+   1800643a6:	add    (%r15),%rdi
    1800643a9:	addr32 gs je 0x18006440c
    1800643ad:	insl   (%dx),%es:(%rdi)
    1800643ae:	gs jae 0x180064419
    1800643b1:	rex (bad)
    1800643b3:	and    $0x53,%al
    1800643b5:	jne    0x180064429
    1800643b7:	data16 (bad)
@@ -138043,15 +138044,15 @@
    1800644f0:	rex.B
    1800644f1:	rex.RB
    1800644f2:	rex.X push %rsi
    1800644f4:	xor    %esi,(%rdx)
    1800644f6:	xor    0x58(%rax),%eax
    1800644f9:	pop    %rdx
    1800644fa:	add    %al,(%rax)
-   1800644fc:	cmp    %al,(%rbx)
+   1800644fc:	cmp    $0x3,%al
    1800644fe:	(bad)
    1800644ff:	outsb  %gs:(%rsi),(%dx)
    180064501:	fs rex push %rbx
    180064504:	jne    0x180064578
    180064506:	data16 (bad)
    180064508:	movsxd 0x52(%rbp),%esp
    18006450b:	(bad)
@@ -138107,15 +138108,15 @@
    18006456b:	data16 (bad)
    18006456d:	movsxd 0x40(%rbp),%esp
    180064570:	and    $0x30,%al
    180064572:	xor    0x32(%rax),%al
    180064575:	rex pop %rax
    180064577:	pop    %rdx
    180064578:	add    %al,(%rax)
-   18006457a:	rex.RX add (%rdi),%r15d
+   18006457a:	rex.WX add (%rdi),%rdi
    18006457d:	addr32 gs je 0x1800645e0
    180064581:	insl   (%dx),%es:(%rdi)
    180064582:	gs jae 0x1800645ed
    180064585:	rex (bad)
    180064587:	and    $0x53,%al
    180064589:	jne    0x1800645fd
    18006458b:	data16 (bad)
@@ -138299,15 +138300,17 @@
    1800646e6:	rex.B
    1800646e7:	rex.RB
    1800646e8:	rex.X push %rsi
    1800646ea:	xor    %esi,(%rdx)
    1800646ec:	xor    0x58(%rax),%eax
    1800646ef:	pop    %rdx
    1800646f0:	add    %al,(%rax)
-   1800646f2:	adc    $0x6e653f03,%eax
+   1800646f2:	sbb    %eax,(%rbx)
+   1800646f4:	(bad)
+   1800646f5:	outsb  %gs:(%rsi),(%dx)
    1800646f7:	fs rex
    1800646f9:	rex.X insb (%dx),%es:(%rdi)
    1800646fb:	outsl  %ds:(%rsi),(%dx)
    1800646fc:	movsxd 0x52(%rbx),%ebp
    1800646ff:	(bad)
    180064700:	outsb  %ds:(%rsi),(%dx)
    180064701:	addr32 gs rex (bad)
@@ -138361,15 +138364,15 @@
    180064758:	outsl  %ds:(%rsi),(%dx)
    180064759:	movsxd 0x40(%rbx),%ebp
    18006475c:	and    $0x30,%al
    18006475e:	xor    0x32(%rax),%al
    180064761:	rex pop %rax
    180064763:	pop    %rdx
    180064764:	add    %al,(%rax)
-   180064766:	add    (%rdi),%r15d
+   180064766:	add    (%rdi),%rdi
    180064769:	addr32 gs je 0x1800647cc
    18006476d:	insl   (%dx),%es:(%rdi)
    18006476e:	gs jae 0x1800647d9
    180064771:	rex (bad)
    180064773:	and    $0x42,%al
    180064775:	insb   (%dx),%es:(%rdi)
    180064776:	outsl  %ds:(%rsi),(%dx)
@@ -138390,15 +138393,15 @@
    18006478e:	and    $0x53,%al
    180064790:	outsl  %ds:(%rsi),(%dx)
    180064791:	insb   (%dx),%es:(%rdi)
    180064792:	imul   $0x24406873,0x65(%rbp,%rcx,2),%esp
    18006479a:	xor    %dh,(%rdx)
    18006479c:	rex xor 0x58(%rax),%al
    1800647a0:	pop    %rdx
-   1800647a1:	add    %ch,%ah
+   1800647a1:	add    %dh,%cl
    1800647a3:	add    (%rdi),%edi
    1800647a5:	outsb  %ds:(%rsi),(%dx)
    1800647a6:	(bad)
    1800647a7:	pop    %rdi
    1800647a8:	jne    0x180064818
    1800647aa:	imul   $0x65765f65,0x75(%rcx),%esi
    1800647b1:	jb     0x180064827
@@ -138412,16 +138415,15 @@
    1800647cc:	fs gs rex
    1800647cf:	rex push %rcx
    1800647d1:	rex.RB
    1800647d2:	rex.X
    1800647d3:	rex.B
    1800647d4:	rex.WB pop %r8
    1800647d6:	pop    %rdx
-   1800647d7:	add    %al,0x6f633f02(%rax)
-   1800647dd:	insl   (%dx),%es:(%rdi)
+   1800647d7:	add    %al,0x6d6f633f(%rdx,%rax,1)
    1800647de:	jo     0x18006484f
    1800647e0:	outsb  %ds:(%rsi),(%dx)
    1800647e1:	outsb  %gs:(%rsi),(%dx)
    1800647e3:	je     0x180064844
    1800647e5:	insl   (%dx),%es:(%rdi)
    1800647e6:	gs jae 0x180064851
    1800647e9:	pop    %rdi
@@ -138486,16 +138488,18 @@
    180064866:	rex
    180064867:	rex jae 0x1800648de
    18006486a:	fs rex
    18006486c:	rex
    18006486d:	rex.WB
    18006486e:	rex pop %rdx
    180064870:	add    %al,(%rax)
-   180064872:	test   $0x6f633f02,%eax
-   180064877:	jb     0x1800648e7
+   180064872:	lods   %ds:(%rsi),%eax
+   180064873:	add    (%rdi),%bh
+   180064875:	movsxd 0x72(%rdi),%ebp
+   180064878:	outsb  %ds:(%rsi),(%dx)
    180064879:	gs jb  0x1800648bc
    18006487c:	(bad)
    18006487d:	and    $0x43,%al
    18006487f:	outsl  %ds:(%rsi),(%dx)
    180064880:	jb     0x1800648f0
    180064882:	gs jb  0x1800648f8
    180064885:	rex and $0x30,%al
@@ -138518,15 +138522,15 @@
    1800648a4:	xor    0x32(%rax),%al
    1800648a7:	rex
    1800648a8:	rex.B
    1800648a9:	rex.RB
    1800648aa:	rex.X push %rbp
    1800648ac:	jne    0x180064923
    1800648ae:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   1800648b6:	jnp    0x1800648bb
+   1800648b6:	jg     0x1800648bb
    1800648b8:	(bad)
    1800648b9:	insb   (%dx),%es:(%rdi)
    1800648ba:	imul   $0x4c243f40,0x65(%rsi),%ebp
    1800648c1:	imul   $0x30244073,0x65(%rsi),%ebp
    1800648c8:	xor    0x67(%rax),%al
    1800648cb:	outsl  %gs:(%rsi),(%dx)
    1800648cd:	fs gs rex
@@ -138541,15 +138545,15 @@
    1800648da:	and    $0x4c,%al
    1800648dc:	imul   $0x32302440,0x65(%rsi),%ebp
    1800648e3:	rex xor 0x41(%rax),%al
    1800648e7:	rex.RB
    1800648e8:	rex.X push %rbp
    1800648ea:	jne    0x180064961
    1800648ec:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   1800648f4:	rex.RXB add $0x3f,%al
+   1800648f4:	rex.WRB add $0x3f,%al
    1800648f7:	jae    0x18006496e
    1800648f9:	jb     0x180064961
    1800648fb:	(bad)
    1800648fc:	movsxd 0x40(%rbp),%esp
    1800648ff:	(bad)
    180064900:	and    $0x53,%al
    180064902:	jne    0x180064976
@@ -138610,16 +138614,16 @@
    18006496b:	xor    0x32(%rax),%al
    18006496e:	rex
    18006496f:	rex.B
    180064970:	rex.RB
    180064971:	rex.X push %rbp
    180064973:	jne    0x1800649ea
    180064975:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   18006497d:	add    %ch,0x6f633f02(%rax)
-   180064983:	jb     0x1800649f3
+   18006497d:	add    %ch,0x726f633f(%rdx,%rax,1)
+   180064984:	outsb  %ds:(%rsi),(%dx)
    180064985:	gs jb  0x1800649c8
    180064988:	(bad)
    180064989:	and    $0x43,%al
    18006498b:	outsl  %ds:(%rsi),(%dx)
    18006498c:	jb     0x1800649fc
    18006498e:	gs jb  0x180064a04
    180064991:	rex and $0x30,%al
@@ -138642,15 +138646,15 @@
    1800649b0:	xor    %eax,0x32(%rax)
    1800649b3:	rex
    1800649b4:	rex.B
    1800649b5:	rex.RB
    1800649b6:	rex.X push %rbp
    1800649b8:	jne    0x180064a2f
    1800649ba:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   1800649c2:	jp     0x1800649c7
+   1800649c2:	jle    0x1800649c7
    1800649c4:	(bad)
    1800649c5:	insb   (%dx),%es:(%rdi)
    1800649c6:	imul   $0x4c243f40,0x65(%rsi),%ebp
    1800649cd:	imul   $0x30244073,0x65(%rsi),%ebp
    1800649d4:	xor    %eax,0x67(%rax)
    1800649d7:	outsl  %gs:(%rsi),(%dx)
    1800649d9:	fs gs rex
@@ -138665,15 +138669,15 @@
    1800649e6:	and    $0x4c,%al
    1800649e8:	imul   $0x31302440,0x65(%rsi),%ebp
    1800649ef:	rex xor 0x41(%rax),%al
    1800649f3:	rex.RB
    1800649f4:	rex.X push %rbp
    1800649f6:	jne    0x180064a6d
    1800649f8:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   180064a00:	rex.RX add $0x3f,%al
+   180064a00:	rex.WR add $0x3f,%al
    180064a03:	jae    0x180064a7a
    180064a05:	jb     0x180064a6d
    180064a07:	(bad)
    180064a08:	movsxd 0x40(%rbp),%esp
    180064a0b:	(bad)
    180064a0c:	and    $0x53,%al
    180064a0e:	jne    0x180064a82
@@ -138699,16 +138703,18 @@
    180064a35:	xor    %eax,0x32(%rax)
    180064a38:	rex
    180064a39:	rex.B
    180064a3a:	rex.RB
    180064a3b:	rex.X push %rbp
    180064a3d:	jne    0x180064ab4
    180064a3f:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   180064a47:	add    %bl,0x73656d3f(%rbx,%rax,1)
-   180064a4e:	push   $0x4c243f40
+   180064a47:	add    %ah,0x656d3f03(%rax)
+   180064a4d:	jae    0x180064ab7
+   180064a4f:	rex (bad)
+   180064a51:	and    $0x4c,%al
    180064a53:	imul   $0x31302440,0x65(%rsi),%ebp
    180064a5a:	rex
    180064a5b:	outsl  %gs:(%esi),(%dx)
    180064a5e:	fs gs rex
    180064a61:	rex push %rcx
    180064a63:	rex.RB
    180064a64:	rex.X
@@ -138720,15 +138726,15 @@
    180064a6b:	and    $0x45,%al
    180064a6d:	fs addr32 gs fs rex.XB jne 0x180064ae6
    180064a74:	jbe    0x180064adb
    180064a76:	rex and $0x30,%al
    180064a79:	xor    %eax,0x32(%rax)
    180064a7c:	rex pop %rax
    180064a7e:	pop    %rdx
-   180064a7f:	add    %bl,0x656d3f03(%rdx)
+   180064a7f:	add    %bl,0x656d3f03(%rsi)
    180064a85:	jae    0x180064aef
    180064a87:	rex (bad)
    180064a89:	and    $0x43,%al
    180064a8b:	outsl  %ds:(%rsi),(%dx)
    180064a8c:	jb     0x180064afc
    180064a8e:	gs jb  0x180064ad1
    180064a91:	and    $0x30,%al
@@ -138746,15 +138752,15 @@
    180064aa5:	and    $0x50,%al
    180064aa7:	outsl  %ds:(%rsi),(%dx)
    180064aa8:	imul   $0x40746553,0x74(%rsi),%ebp
    180064aaf:	and    $0x30,%al
    180064ab1:	xor    %eax,0x32(%rax)
    180064ab4:	rex pop %rax
    180064ab6:	pop    %rdx
-   180064ab7:	add    %bl,0x656d3f03(%rbp)
+   180064ab7:	add    %ah,0x656d3f03(%rcx)
    180064abd:	jae    0x180064b27
    180064abf:	rex (bad)
    180064ac1:	and    $0x4c,%al
    180064ac3:	imul   $0x32302440,0x65(%rsi),%ebp
    180064aca:	rex
    180064acb:	outsl  %gs:(%esi),(%dx)
    180064ace:	fs gs rex
@@ -138769,15 +138775,15 @@
    180064adb:	and    $0x45,%al
    180064add:	fs addr32 gs fs rex.XB jne 0x180064b56
    180064ae4:	jbe    0x180064b4b
    180064ae6:	rex and $0x30,%al
    180064ae9:	xor    0x32(%rax),%al
    180064aec:	rex pop %rax
    180064aee:	pop    %rdx
-   180064aef:	add    %bl,0x656d3f03(%rbx)
+   180064aef:	add    %bl,0x656d3f03(%rdi)
    180064af5:	jae    0x180064b5f
    180064af7:	rex (bad)
    180064af9:	and    $0x43,%al
    180064afb:	outsl  %ds:(%rsi),(%dx)
    180064afc:	jb     0x180064b6c
    180064afe:	gs jb  0x180064b41
    180064b01:	and    $0x30,%al
@@ -138843,15 +138849,15 @@
    180064b7c:	fs gs rex
    180064b7f:	rex push %rcx
    180064b81:	rex.RB
    180064b82:	rex.B
    180064b83:	rex.B
    180064b84:	rex pop %rax
    180064b86:	pop    %rdx
-   180064b87:	add    %dl,0x4(%rcx)
+   180064b87:	add    %dl,0x4(%rdi)
    180064b8a:	(bad)
    180064b8b:	jne    0x180064bfb
    180064b8d:	imul   $0x65765f65,0x75(%rcx),%esi
    180064b94:	jb     0x180064c0a
    180064b96:	gs js  0x180064bd9
    180064b99:	push   %rsi
    180064b9a:	gs jb  0x180064c11
@@ -138878,16 +138884,15 @@
    180064bc4:	gs jae 0x180064c2f
    180064bc7:	push   %rsi
    180064bc8:	gs jb  0x180064c3f
    180064bcb:	gs js  0x180064c0e
    180064bce:	xor    0x40(%rax),%al
    180064bd1:	pop    %rdx
    180064bd2:	add    %al,(%rax)
-   180064bd4:	jg     0x180064bd9
-   180064bd6:	(bad)
+   180064bd4:	addl   $0x3f,(%rbx)
    180064bd7:	insb   (%dx),%es:(%rdi)
    180064bd8:	imul   $0x243f4073,0x65(%rsi),%ebp
    180064bdf:	imul   $0x30244073,0x65(%rsi),%r13
    180064be7:	xor    0x67(%rax),%al
    180064bea:	outsl  %gs:(%rsi),(%dx)
    180064bec:	fs gs rex
    180064bef:	rex push %rcx
@@ -138896,16 +138901,16 @@
    180064bf3:	rex.B (bad)
    180064bf5:	push   %r14
    180064bf7:	imul   $0x676e6152,0x65(%rsi),%r13
    180064bff:	rex xor %esi,%gs:(%rdx)
    180064c03:	rex pop %rax
    180064c05:	pop    %rdx
    180064c06:	add    %al,(%rax)
-   180064c08:	jle    0x180064c0d
-   180064c0a:	(bad)
+   180064c08:	(bad)
+   180064c09:	add    (%rdi),%edi
    180064c0b:	insb   (%dx),%es:(%rdi)
    180064c0c:	imul   $0x243f4073,0x65(%rsi),%ebp
    180064c13:	imul   $0x30244073,0x65(%rsi),%r13
    180064c1b:	xor    %eax,0x67(%rax)
    180064c1e:	outsl  %gs:(%rsi),(%dx)
    180064c20:	fs gs rex
    180064c23:	rex push %rcx
@@ -139015,16 +139020,15 @@
    180064d28:	rex.B
    180064d29:	rex.RB
    180064d2a:	rex.X push %rsi
    180064d2c:	xor    %esi,(%rdx)
    180064d2e:	xor    0x58(%rax),%eax
    180064d31:	pop    %rdx
    180064d32:	add    %al,(%rax)
-   180064d34:	xor    (%rbx),%al
-   180064d36:	(bad)
+   180064d34:	ss add (%rdi),%edi
    180064d37:	outsb  %gs:(%rsi),(%dx)
    180064d39:	fs rex
    180064d3b:	imul   $0x676e6152,0x65(%rsi),%r13
    180064d43:	gs rex (bad)
    180064d46:	and    $0x4c,%al
    180064d48:	imul   $0x30244073,0x65(%rsi),%ebp
    180064d4f:	xor    %eax,0x67(%rax)
@@ -139160,16 +139164,16 @@
    180064e8e:	rex.B
    180064e8f:	rex.RB
    180064e90:	rex.X push %rsi
    180064e92:	xor    %esi,(%rdx)
    180064e94:	xor    0x58(%rax),%eax
    180064e97:	pop    %rdx
    180064e98:	add    %al,(%rax)
-   180064e9a:	xor    (%rbx),%eax
-   180064e9c:	(bad)
+   180064e9a:	(bad)
+   180064e9b:	add    (%rdi),%edi
    180064e9d:	outsb  %gs:(%rsi),(%dx)
    180064e9f:	fs rex
    180064ea1:	imul   $0x676e6152,0x65(%rsi),%r13
    180064ea9:	gs rex (bad)
    180064eac:	and    $0x4c,%al
    180064eae:	imul   $0x30244073,0x65(%rsi),%ebp
    180064eb5:	xor    0x67(%rax),%al
@@ -139205,15 +139209,15 @@
    180064ef5:	rex.RB
    180064ef6:	rex.X push %rsi
    180064ef8:	(bad)
    180064ef9:	and    $0x4c,%al
    180064efb:	imul   $0x32302440,0x65(%rsi),%ebp
    180064f02:	rex xor 0x58(%rax),%al
    180064f06:	pop    %rdx
-   180064f07:	add    %bl,%ch
+   180064f07:	add    %ah,%cl
    180064f09:	add    (%rdi),%bh
    180064f0b:	movsxd 0x65(%rdx),%esi
    180064f0e:	(bad)
    180064f0f:	je     0x180064f76
    180064f11:	pop    %rdi
    180064f12:	jae    0x180064f89
    180064f14:	jb     0x180064f7c
@@ -139248,15 +139252,15 @@
    180064f54:	rex.B
    180064f55:	rex.RB
    180064f56:	rex.X push %rsi
    180064f58:	rex.X push %rdx
    180064f5a:	gs jo  0x180064f9d
    180064f5d:	xor    %eax,0x40(%rax)
    180064f60:	pop    %rdx
-   180064f61:	add    %bl,%ah
+   180064f61:	add    %ah,%al
    180064f63:	add    (%rdi),%bh
    180064f65:	movsxd 0x65(%rdx),%esi
    180064f68:	(bad)
    180064f69:	je     0x180064fd0
    180064f6b:	pop    %rdi
    180064f6c:	jae    0x180064fe3
    180064f6e:	jb     0x180064fd6
@@ -139293,15 +139297,16 @@
    180064fb0:	rex.X push %rsi
    180064fb2:	push   %rbx
    180064fb3:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    180064fb8:	outsb  %ds:(%rsi),(%dx)
    180064fb9:	rex xor %eax,0x40(%rax)
    180064fbd:	pop    %rdx
    180064fbe:	add    %al,(%rax)
-   180064fc0:	add    (%rdi),%r15
+   180064fc0:	push   %rax
+   180064fc1:	add    (%rdi),%edi
    180064fc3:	push   $0x635f7361
    180064fc8:	outsl  %ds:(%rsi),(%dx)
    180064fc9:	insl   (%dx),%es:(%rdi)
    180064fca:	jo     0x18006503b
    180064fcc:	outsb  %ds:(%rsi),(%dx)
    180064fcd:	outsb  %gs:(%rsi),(%dx)
    180064fcf:	je     0x180065030
@@ -139325,16 +139330,16 @@
    180064ffc:	rex.WRX
    180064ffd:	rex.WB
    180064ffe:	rex.B
    180064fff:	rex.RB
    180065000:	rex.X push %rbp
    180065002:	jne    0x180065079
    180065004:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   18006500c:	lods   %ds:(%rsi),%eax
-   18006500d:	add    (%rdi),%bh
+   18006500c:	mov    $0x2,%cl
+   18006500e:	(bad)
    18006500f:	movsxd 0x72(%rdi),%ebp
    180065012:	outsb  %ds:(%rsi),(%dx)
    180065013:	gs jb  0x180065089
    180065016:	rex (bad)
    180065018:	and    $0x43,%al
    18006501a:	outsl  %ds:(%rsi),(%dx)
    18006501b:	jb     0x18006508b
@@ -139488,16 +139493,16 @@
    180065146:	rex.B
    180065147:	rex.RB
    180065148:	rex.X push %rsi
    18006514a:	xor    %esi,(%rdx)
    18006514c:	xor    0x58(%rax),%eax
    18006514f:	pop    %rdx
    180065150:	add    %al,(%rax)
-   180065152:	(bad)
-   180065153:	add    (%rdi),%edi
+   180065152:	and    (%rbx),%al
+   180065154:	(bad)
    180065155:	outsb  %gs:(%rsi),(%dx)
    180065157:	fs rex
    180065159:	rex.XB outsl %ds:(%rsi),(%dx)
    18006515b:	jb     0x1800651cb
    18006515d:	gs jb  0x1800651b2
    180065160:	(bad)
    180065161:	outsb  %ds:(%rsi),(%dx)
@@ -139551,17 +139556,16 @@
    1800651bb:	outsl  %ds:(%rsi),(%dx)
    1800651bc:	jb     0x18006522c
    1800651be:	gs jb  0x180065201
    1800651c1:	and    $0x30,%al
    1800651c3:	xor    0x32(%rax),%al
    1800651c6:	rex pop %rax
    1800651c8:	pop    %rdx
-   1800651c9:	add    %bh,0x2(%rdi)
-   1800651cc:	(bad)
-   1800651cd:	movsxd 0x6d(%rdi),%ebp
+   1800651c9:	add    %al,0x6f633f02(%rbx)
+   1800651cf:	insl   (%dx),%es:(%rdi)
    1800651d0:	jo     0x180065241
    1800651d2:	outsb  %ds:(%rsi),(%dx)
    1800651d3:	outsb  %gs:(%rsi),(%dx)
    1800651d5:	je     0x180065236
    1800651d7:	insl   (%dx),%es:(%rdi)
    1800651d8:	gs jae 0x180065243
    1800651db:	pop    %rdi
@@ -139671,15 +139675,15 @@
    1800652b8:	(bad)
    1800652b9:	addr32 rex
    1800652bb:	outsl  %gs:(%esi),(%dx)
    1800652be:	fs gs rex
    1800652c1:	rex
    1800652c2:	rex xor 0x40(%rax),%al
    1800652c6:	pop    %rdx
-   1800652c7:	add    %bl,%dl
+   1800652c7:	add    %bl,%bh
    1800652c9:	add    (%rdi),%edi
    1800652cb:	outsb  %ds:(%rsi),(%dx)
    1800652cc:	(bad)
    1800652cd:	pop    %rdi
    1800652ce:	imul   $0x6e656469,0x63(%rsi),%ebp
    1800652d5:	movsxd 0x73(%rbp),%esp
    1800652d8:	rex push %rdx
@@ -139697,15 +139701,15 @@
    1800652f1:	rex.B
    1800652f2:	rex.WB
    1800652f3:	rex.B
    1800652f4:	rex.RB
    1800652f5:	rex.X push %rbp
    1800652f7:	jne    0x18006536e
    1800652f9:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   180065301:	add    %bl,%cl
+   180065301:	add    %bl,%dh
    180065303:	add    (%rdi),%edi
    180065305:	outsb  %ds:(%rsi),(%dx)
    180065306:	(bad)
    180065307:	pop    %rdi
    180065308:	gs insl (%dx),%es:(%rdi)
    18006530a:	(bad)
    18006530f:	outsb  %ds:(%rsi),(%dx)
@@ -139725,15 +139729,15 @@
    18006532b:	rex.B
    18006532c:	rex.WB
    18006532d:	rex.B
    18006532e:	rex.RB
    18006532f:	rex.X push %rbp
    180065331:	jne    0x1800653a8
    180065333:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   18006533b:	add    %ah,0x3(%rdi)
+   18006533b:	add    %ch,0x3(%rbx)
    18006533e:	(bad)
    18006533f:	imul   $0x6e756f62,0x5f(%rbx),%esi
    180065346:	fs (bad)
    180065348:	jb     0x1800653c3
    18006534a:	rex push %rdx
    18006534c:	gs insb (%dx),%es:(%rdi)
    18006534e:	(bad)
@@ -139904,15 +139908,15 @@
    18006549c:	rex.B
    18006549d:	rex.RB
    18006549e:	rex.X push %rsi
    1800654a0:	xor    %dh,(%rcx)
    1800654a2:	xor    0x40(%rax),%al
    1800654a5:	pop    %rdx
    1800654a6:	add    %al,(%rax)
-   1800654a8:	adc    $0x3,%al
+   1800654a8:	sbb    %al,(%rbx)
    1800654aa:	(bad)
    1800654ab:	gs insl (%dx),%es:(%rdi)
    1800654ad:	(bad)
    1800654b2:	outsb  %ds:(%rsi),(%dx)
    1800654b3:	addr32 jae 0x1800654f6
    1800654b6:	push   %rdx
    1800654b7:	gs insb (%dx),%es:(%rdi)
@@ -139937,15 +139941,15 @@
    1800654de:	rex xor %esi,%gs:(%edx)
    1800654e3:	rex
    1800654e4:	rex.B
    1800654e5:	rex.RB
    1800654e6:	rex.X push %rbp
    1800654e8:	jne    0x18006555f
    1800654ea:	imul   $0x5a4040,0x32(%rax,%rax,2),%esp
-   1800654f2:	jb     0x1800654f7
+   1800654f2:	jbe    0x1800654f7
    1800654f4:	(bad)
    1800654f5:	imul   $0x65746e69,0x5f(%rbx),%esi
    1800654fc:	jb     0x18006556c
    1800654fe:	(bad)
    1800654ff:	insb   (%dx),%es:(%rdi)
    180065500:	rex push %rdx
    180065502:	gs insb (%dx),%es:(%rdi)
@@ -139963,16 +139967,18 @@
    18006551b:	rex.WRX
    18006551c:	rex.B
    18006551d:	rex.RB
    18006551e:	rex.X push %rbp
    180065520:	jne    0x180065597
    180065522:	imul   $0x5a403040,0x32(%rax,%rax,2),%esp
    18006552a:	add    %al,(%rax)
-   18006552c:	add    %gs:(%rdi),%edi
-   18006552f:	imul   $0x6e756f62,0x5f(%rbx),%esi
+   18006552c:	imul   $0x5f73693f,(%rbx),%eax
+   180065532:	(bad)
+   180065533:	outsl  %ds:(%rsi),(%dx)
+   180065534:	jne    0x1800655a4
    180065536:	fs (bad)
    180065538:	jb     0x1800655b3
    18006553a:	rex
    18006553b:	rex.X push %rdx
    18006553d:	gs jo  0x180065580
    180065540:	outsl  %gs:(%esi),(%dx)
    180065543:	fs gs rex
@@ -139996,15 +140002,15 @@
    180065567:	data16 (bad)
    180065569:	movsxd 0x40(%rbp),%esp
    18006556c:	and    $0x30,%al
    18006556e:	xor    0x32(%rax),%al
    180065571:	rex
    180065572:	rex pop %rdx
    180065574:	add    %al,(%rax)
-   180065576:	jo     0x18006557b
+   180065576:	je     0x18006557b
    180065578:	(bad)
    180065579:	imul   $0x65746e69,0x5f(%rbx),%esi
    180065580:	jb     0x1800655f0
    180065582:	(bad)
    180065583:	insb   (%dx),%es:(%rdi)
    180065584:	rex
    180065585:	rex.X push %rdx
@@ -140031,16 +140037,16 @@
    1800655b1:	data16 (bad)
    1800655b3:	movsxd 0x40(%rbp),%esp
    1800655b6:	and    $0x30,%al
    1800655b8:	xor    0x32(%rax),%al
    1800655bb:	rex
    1800655bc:	rex pop %rdx
    1800655be:	add    %al,(%rax)
-   1800655c0:	lods   %ds:(%rsi),%al
-   1800655c1:	add    (%rdi),%bh
+   1800655c0:	mov    $0x2,%al
+   1800655c2:	(bad)
    1800655c3:	movsxd 0x72(%rdi),%ebp
    1800655c6:	outsb  %ds:(%rsi),(%dx)
    1800655c7:	gs jb  0x18006563d
    1800655ca:	rex (bad)
    1800655cc:	and    $0x43,%al
    1800655ce:	outsl  %ds:(%rsi),(%dx)
    1800655cf:	jb     0x18006563f
@@ -140194,15 +140200,17 @@
    1800656fa:	rex.B
    1800656fb:	rex.RB
    1800656fc:	rex.X push %rsi
    1800656fe:	xor    %esi,(%rdx)
    180065700:	xor    0x58(%rax),%eax
    180065703:	pop    %rdx
    180065704:	add    %al,(%rax)
-   180065706:	sbb    $0x6e653f03,%eax
+   180065706:	and    %eax,(%rbx)
+   180065708:	(bad)
+   180065709:	outsb  %gs:(%rsi),(%dx)
    18006570b:	fs rex
    18006570d:	rex.XB outsl %ds:(%rsi),(%dx)
    18006570f:	jb     0x18006577f
    180065711:	gs jb  0x180065766
    180065714:	(bad)
    180065715:	outsb  %ds:(%rsi),(%dx)
    180065716:	addr32 gs rex (bad)
@@ -142832,16 +142840,16 @@
    180066c47:	outsl  %gs:(%rsi),(%dx)
    180066c49:	fs gs pop %rdi
    180066c4c:	insl   (%dx),%es:(%rdi)
    180066c4d:	gs jae 0x180066cb8
    180066c50:	cs fs insb (%dx),%es:(%rdi)
    180066c53:	insb   (%dx),%es:(%rdi)
    180066c54:	add    %al,(%rax)
-   180066c56:	scas   %es:(%rdi),%al
-   180066c57:	add    %bh,(%rdi)
+   180066c56:	mov    $0x0,%bl
+   180066c58:	(bad)
    180066c59:	(bad)
    180066c5a:	xor    %bh,(%rdi)
    180066c5c:	and    $0x4e,%al
    180066c5e:	rex.WRX push %rbx
    180066c60:	gs (bad)
    180066c62:	jb     0x180066cc7
    180066c64:	push   $0x31302440
@@ -142885,16 +142893,18 @@
    180066cb5:	rex jae 0x180066d2c
    180066cb8:	fs rex
    180066cba:	rex
    180066cbb:	rex jae 0x180066d32
    180066cbe:	fs rex
    180066cc0:	rex
    180066cc1:	rex pop %rdx
-   180066cc3:	add    %ch,0x313f3f01(%rip)        # 0x1b145abca
-   180066cc9:	(bad)
+   180066cc3:	add    %dh,(%rdx)
+   180066cc5:	add    %edi,(%rdi)
+   180066cc7:	(bad)
+   180066cc8:	xor    %edi,(%rdi)
    180066cca:	and    $0x4e,%al
    180066ccc:	rex.WRX push %rbx
    180066cce:	gs (bad)
    180066cd0:	jb     0x180066d35
    180066cd2:	push   $0x31302440
    180066cd7:	rex
    180066cd8:	outsl  %gs:(%esi),(%dx)
@@ -142902,17 +142912,16 @@
    180066cde:	rex push %rcx
    180066ce0:	rex.RB
    180066ce1:	rex.B
    180066ce2:	rex.B
    180066ce3:	rex pop %rax
    180066ce5:	pop    %rdx
    180066ce6:	add    %al,(%rax)
-   180066ce8:	fiadds (%rcx)
-   180066cea:	(bad)
-   180066ceb:	movsxd 0x6c(%rdi),%ebp
+   180066ce8:	jmp    0x1ef69abee
+   180066ced:	insb   (%dx),%es:(%rdi)
    180066cee:	outsl  %ds:(%rsi),(%dx)
    180066cef:	movsxd 0x74(%rcx),%esp
    180066cf2:	gs fs pop %rdi
    180066cf5:	imul   $0x6d5f7865,0x64(%rsi),%ebp
    180066cfc:	(bad)
    180066cfd:	jo     0x180066d6f
    180066cff:	imul   $0x4e243f40,0x67(%rsi),%ebp
@@ -142935,15 +142944,15 @@
    180066d27:	gs rex.WB outsb %fs:(%rsi),(%dx)
    180066d2b:	outsw  %ds:(%rsi),(%dx)
    180066d2d:	rex xor %esi,(%rdx)
    180066d30:	rex
    180066d31:	rex.WRX
    180066d32:	rex pop %rdx
    180066d34:	add    %al,(%rax)
-   180066d36:	mov    $0x0,%al
+   180066d36:	mov    $0x0,%ch
    180066d38:	(bad)
    180066d39:	(bad)
    180066d3a:	xor    %bh,(%rdi)
    180066d3c:	and    $0x4e,%al
    180066d3e:	rex.WRX push %rbx
    180066d40:	gs (bad)
    180066d42:	jb     0x180066da7
@@ -142988,15 +142997,15 @@
    180066d95:	rex jae 0x180066e0c
    180066d98:	fs rex
    180066d9a:	rex
    180066d9b:	rex jae 0x180066e12
    180066d9e:	fs rex
    180066da0:	rex
    180066da1:	rex pop %rdx
-   180066da3:	add    %ch,(%rsi)
+   180066da3:	add    %dh,(%rbx)
    180066da5:	add    %edi,(%rdi)
    180066da7:	(bad)
    180066da8:	xor    %edi,(%rdi)
    180066daa:	and    $0x4e,%al
    180066dac:	rex.WRX push %rbx
    180066dae:	gs (bad)
    180066db0:	jb     0x180066e15
@@ -143007,16 +143016,16 @@
    180066dbe:	rex push %rcx
    180066dc0:	rex.RB
    180066dc1:	rex.B
    180066dc2:	rex.B
    180066dc3:	rex pop %rax
    180066dc5:	pop    %rdx
    180066dc6:	add    %al,(%rax)
-   180066dc8:	filds  (%rcx)
-   180066dca:	(bad)
+   180066dc8:	(bad)
+   180066dc9:	add    %edi,(%rdi)
    180066dcb:	movsxd 0x6c(%rdi),%ebp
    180066dce:	outsl  %ds:(%rsi),(%dx)
    180066dcf:	movsxd 0x74(%rcx),%esp
    180066dd2:	gs fs pop %rdi
    180066dd5:	imul   $0x6d5f7865,0x64(%rsi),%ebp
    180066ddc:	(bad)
    180066ddd:	jo     0x180066e4f
@@ -143090,15 +143099,15 @@
    180066e7e:	rex.X push %rsi
    180066e80:	(bad)
    180066e81:	and    $0x50,%al
    180066e83:	outsl  %ds:(%rsi),(%dx)
    180066e84:	imul   $0x32302440,0x74(%rsi),%ebp
    180066e8b:	rex xor %al,0x30(%rax)
    180066e8f:	rex pop %rdx
-   180066e91:	add    %ah,0x2(%rbp)
+   180066e91:	add    %dh,0x2(%rcx)
    180066e94:	(bad)
    180066e95:	jae    0x180066efc
    180066e97:	insl   (%dx),%es:(%edi)
    180066e99:	outsb  %gs:(%rsi),(%dx)
    180066e9b:	je     0x180066efc
    180066e9d:	jae    0x180066f04
    180066e9f:	insl   (%dx),%es:(%edi)
@@ -143141,16 +143150,15 @@
    180066ef1:	and    $0x53,%al
    180066ef3:	gs insl (%dx),%es:(%edi)
    180066ef6:	outsb  %gs:(%rsi),(%dx)
    180066ef8:	je     0x180066f3a
    180066efa:	and    $0x30,%al
    180066efc:	xor    %eax,0x31(%rax)
    180066eff:	rex xor %al,0x5a(%rax)
-   180066f03:	add    %ch,0x2(%rax)
-   180066f06:	(bad)
+   180066f03:	add    %dh,0x3f(%rdx,%rax,1)
    180066f07:	jae    0x180066f6e
    180066f09:	insl   (%dx),%es:(%edi)
    180066f0b:	outsb  %gs:(%rsi),(%dx)
    180066f0d:	je     0x180066f6e
    180066f0f:	je     0x180066f83
    180066f11:	imul   $0x5f656c67,0x6e(%rcx),%esp
    180066f18:	imul   $0x65737265,0x74(%rsi),%ebp
@@ -143204,15 +143212,15 @@
    180066f7d:	outsb  %ds:(%rsi),(%dx)
    180066f7e:	insb   (%dx),%es:(%edi)
    180066f80:	gs rex and $0x30,%al
    180066f84:	xor    0x31(%rax),%al
    180066f87:	rex
    180066f88:	rex pop %rdx
    180066f8a:	add    %al,(%rax)
-   180066f8c:	hlt
+   180066f8c:	stc
    180066f8d:	add    %bh,(%rdi)
    180066f8f:	(bad)
    180066f90:	xor    %bh,(%rdi)
    180066f92:	and    $0x53,%al
    180066f94:	gs insl (%dx),%es:(%edi)
    180066f97:	outsb  %gs:(%rsi),(%dx)
    180066f99:	je     0x180066fdb
@@ -143280,16 +143288,16 @@
    180067017:	outsb  %ds:(%rsi),(%dx)
    180067018:	insb   (%dx),%es:(%edi)
    18006701a:	gs rex and $0x30,%al
    18006701e:	xor    %eax,0x30(%rax)
    180067021:	rex
    180067022:	rex pop %rdx
    180067024:	add    %al,(%rax)
-   180067026:	mov    %es,(%rdx)
-   180067028:	(bad)
+   180067026:	cwtl
+   180067027:	add    (%rdi),%bh
    180067029:	jbe    0x180067090
    18006702b:	jb     0x1800670a1
    18006702d:	imul   $0x243f4073,0x65(%rbx),%esp
    180067034:	rex.RXB
    180067035:	outsb  %gs:(%rsi),(%dx)
    180067037:	gs jb  0x1800670a3
    18006703a:	movsxd 0x69(%rdx,%rsi,2),%edx
@@ -143361,15 +143369,15 @@
    1800670c4:	rex and $0x30,%al
    1800670c7:	xor    0x73(%rax),%al
    1800670ca:	je     0x180067130
    1800670cc:	rex
    1800670cd:	rex pop %rax
    1800670cf:	pop    %rdx
    1800670d0:	add    %al,(%rax)
-   1800670d2:	clc
+   1800670d2:	std
    1800670d3:	add    %bh,(%rdi)
    1800670d5:	(bad)
    1800670d6:	xor    %bh,(%rdi)
    1800670d8:	and    $0x53,%al
    1800670da:	gs insl (%dx),%es:(%edi)
    1800670dd:	outsb  %gs:(%rsi),(%dx)
    1800670df:	je     0x180067121
@@ -143388,16 +143396,15 @@
    1800670f5:	(bad)
    1800670f6:	and    $0x50,%al
    1800670f8:	outsl  %ds:(%rsi),(%dx)
    1800670f9:	imul   $0x32302440,0x74(%rsi),%ebp
    180067100:	rex xor %eax,0x30(%rax)
    180067104:	rex pop %rdx
    180067106:	add    %al,(%rax)
-   180067108:	sub    %eax,(%rcx)
-   18006710a:	(bad)
+   180067108:	cs add %edi,(%rdi)
    18006710b:	(bad)
    18006710c:	xor    %edi,(%rdi)
    18006710e:	and    $0x41,%al
    180067110:	rex.B
    180067111:	rex.X
    180067112:	rex.X push %rsp
    180067114:	jb     0x18006717b
@@ -143408,16 +143415,16 @@
    180067122:	rex push %rcx
    180067124:	rex.RB
    180067125:	rex.B
    180067126:	rex.B
    180067127:	rex pop %rax
    180067129:	pop    %rdx
    18006712a:	add    %al,(%rax)
-   18006712c:	(bad)
-   18006712d:	add    (%rdi),%bh
+   18006712c:	sub    (%rdx),%al
+   18006712e:	(bad)
    18006712f:	outsb  %ds:(%rsi),(%dx)
    180067130:	(bad)
    180067131:	pop    %rdi
    180067132:	(bad)
    180067137:	jae    0x180067179
    180067139:	(bad)
    18006713a:	and    $0x41,%al
@@ -143432,18 +143439,16 @@
    18006714e:	rex push %rcx
    180067150:	rex.RB
    180067151:	rex.X
    180067152:	rex.B
    180067153:	rex.WB pop %r8
    180067155:	pop    %rdx
    180067156:	add    %al,(%rax)
-   180067158:	sub    %al,(%rcx)
-   18006715a:	(bad)
-   18006715b:	(bad)
-   18006715c:	xor    %edi,(%rdi)
+   180067158:	sub    $0x313f3f01,%eax
+   18006715d:	(bad)
    18006715e:	and    $0x41,%al
    180067160:	rex.B
    180067161:	rex.X
    180067162:	rex.X push %rsp
    180067164:	jb     0x1800671cb
    180067166:	gs rex and $0x30,%al
    18006716a:	xor    %eax,0x67(%rax)
@@ -143452,16 +143457,16 @@
    180067172:	rex push %rcx
    180067174:	rex.RB
    180067175:	rex.B
    180067176:	rex.B
    180067177:	rex pop %rax
    180067179:	pop    %rdx
    18006717a:	add    %al,(%rax)
-   18006717c:	(bad)
-   18006717d:	add    (%rdi),%bh
+   18006717c:	sub    %eax,(%rdx)
+   18006717e:	(bad)
    18006717f:	outsb  %ds:(%rsi),(%dx)
    180067180:	(bad)
    180067181:	pop    %rdi
    180067182:	(bad)
    180067187:	jae    0x1800671c9
    180067189:	(bad)
    18006718a:	and    $0x41,%al
@@ -143476,16 +143481,16 @@
    18006719e:	rex push %rcx
    1800671a0:	rex.RB
    1800671a1:	rex.X
    1800671a2:	rex.B
    1800671a3:	rex.WB pop %r8
    1800671a5:	pop    %rdx
    1800671a6:	add    %al,(%rax)
-   1800671a8:	(bad)
-   1800671a9:	add    (%rdi),%bh
+   1800671a8:	adc    (%rdx),%al
+   1800671aa:	(bad)
    1800671ab:	imul   $0x6661656c,0x5f(%rbx),%esi
    1800671b2:	rex
    1800671b3:	rex.WB insl (%dx),%es:(%rdi)
    1800671b5:	jo     0x180067223
    1800671b7:	rex (bad)
    1800671b9:	and    $0x41,%al
    1800671bb:	rex.B
@@ -143499,16 +143504,16 @@
    1800671cd:	rex push %rbx
    1800671cf:	pop    %r15
    1800671d1:	rex.WRX
    1800671d2:	rex.WB
    1800671d3:	rex.WB
    1800671d4:	rex pop %rdx
    1800671d6:	add    %al,(%rax)
-   1800671d8:	stc
-   1800671d9:	add    %edi,(%rdi)
+   1800671d8:	add    $0x2,%al
+   1800671da:	(bad)
    1800671db:	addr32 gs je 0x18006723e
    1800671df:	jb     0x180067246
    1800671e1:	movsxd 0x72(%rbp),%esi
    1800671e4:	jae    0x18006724f
    1800671e6:	jbe    0x18006724d
    1800671e8:	pop    %rdi
    1800671e9:	imul   $0x726f7461,0x72(%rbp,%riz,2),%esi
@@ -143533,15 +143538,15 @@
    180067218:	je     0x180067289
    18006721a:	jb     0x18006725c
    18006721c:	xor    %esi,(%rdx)
    18006721e:	xor    0x49(%rax),%eax
    180067221:	rex.WB
    180067222:	rex.WB
    180067223:	rex pop %rdx
-   180067225:	add    %ah,(%rdi)
+   180067225:	add    %dh,(%rdx)
    180067227:	add    (%rdi),%bh
    180067229:	outsb  %ds:(%rsi),(%dx)
    18006722a:	outsl  %ds:(%rsi),(%dx)
    18006722b:	fs gs rex
    18006722e:	rex.WB insl (%dx),%es:(%rdi)
    180067230:	jo     0x18006729e
    180067232:	rex (bad)
@@ -143568,15 +143573,18 @@
    180067257:	imul   $0x40786f42,%fs:0x67(%rsi),%ebp
    18006725f:	and    $0x30,%al
    180067261:	xor    0x33(%rax),%al
    180067264:	rex
    180067265:	rex.WB
    180067266:	rex pop %rdx
    180067268:	add    %al,(%rax)
-   18006726a:	adc    $0x616d3f02,%eax
+   18006726a:	and    %al,(%rdx)
+   18006726c:	(bad)
+   18006726d:	insl   (%dx),%es:(%rdi)
+   18006726e:	(bad)
    18006726f:	jo     0x1800672e1
    180067271:	imul   $0x726f6d5f,0x67(%rsi),%ebp
    180067278:	je     0x1800672e9
    18006727a:	outsb  %ds:(%rsi),(%dx)
    18006727b:	rex
    18006727c:	rex.WB insl (%dx),%es:(%rdi)
    18006727e:	jo     0x1800672ec
@@ -143593,15 +143601,15 @@
    180067296:	rex push %rcx
    180067298:	rex.RB
    180067299:	rex.X
    18006729a:	rex.B
    18006729b:	rex.WB
    18006729c:	rex.WB
    18006729d:	rex pop %rdx
-   18006729f:	add    %al,(%rsi)
+   18006729f:	add    %dl,(%rcx)
    1800672a1:	add    (%rdi),%bh
    1800672a3:	imul   $0x6661656c,0x5f(%rbx),%esi
    1800672aa:	rex
    1800672ab:	rex.WB insl (%dx),%es:(%rdi)
    1800672ad:	jo     0x18006731b
    1800672af:	rex (bad)
    1800672b1:	and    $0x41,%al
@@ -143616,16 +143624,16 @@
    1800672c5:	rex push %rbx
    1800672c7:	pop    %r15
    1800672c9:	rex.WRX
    1800672ca:	rex.WB
    1800672cb:	rex.WB
    1800672cc:	rex pop %rdx
    1800672ce:	add    %al,(%rax)
-   1800672d0:	clc
-   1800672d1:	add    %edi,(%rdi)
+   1800672d0:	add    (%rdx),%eax
+   1800672d2:	(bad)
    1800672d3:	addr32 gs je 0x180067336
    1800672d7:	jb     0x18006733e
    1800672d9:	movsxd 0x72(%rbp),%esi
    1800672dc:	jae    0x180067347
    1800672de:	jbe    0x180067345
    1800672e0:	pop    %rdi
    1800672e1:	imul   $0x726f7461,0x72(%rbp,%riz,2),%esi
@@ -143650,15 +143658,15 @@
    180067310:	je     0x180067381
    180067312:	jb     0x180067354
    180067314:	xor    %esi,(%rdx)
    180067316:	xor    0x49(%rax),%eax
    180067319:	rex.WB
    18006731a:	rex.WB
    18006731b:	rex pop %rdx
-   18006731d:	add    %ah,(%rsi)
+   18006731d:	add    %dh,(%rcx)
    18006731f:	add    (%rdi),%bh
    180067321:	outsb  %ds:(%rsi),(%dx)
    180067322:	outsl  %ds:(%rsi),(%dx)
    180067323:	fs gs rex
    180067326:	rex.WB insl (%dx),%es:(%rdi)
    180067328:	jo     0x180067396
    18006732a:	rex (bad)
@@ -143685,16 +143693,16 @@
    18006734f:	imul   $0x40786f42,%fs:0x67(%rsi),%ebp
    180067357:	and    $0x30,%al
    180067359:	xor    %eax,0x33(%rax)
    18006735c:	rex
    18006735d:	rex.WB
    18006735e:	rex pop %rdx
    180067360:	add    %al,(%rax)
-   180067362:	adc    $0x2,%al
-   180067364:	(bad)
+   180067362:	(bad)
+   180067363:	add    (%rdi),%bh
    180067365:	insl   (%dx),%es:(%rdi)
    180067366:	(bad)
    180067367:	jo     0x1800673d9
    180067369:	imul   $0x726f6d5f,0x67(%rsi),%ebp
    180067370:	je     0x1800673e1
    180067372:	outsb  %ds:(%rsi),(%dx)
    180067373:	rex
@@ -143713,15 +143721,15 @@
    18006738e:	rex push %rcx
    180067390:	rex.RB
    180067391:	rex.X
    180067392:	rex.B
    180067393:	rex.WB
    180067394:	rex.WB
    180067395:	rex pop %rdx
-   180067397:	add    %al,(%rbx)
+   180067397:	add    %cl,(%rsi)
    180067399:	add    (%rdi),%bh
    18006739b:	imul   $0x65737265,0x74(%rsi),%ebp
    1800673a2:	movsxd 0x40(%rbx,%rsi,2),%esi
    1800673a6:	(bad)
    1800673a7:	and    $0x42,%al
    1800673a9:	outsl  %ds:(%rsi),(%dx)
    1800673aa:	jne    0x18006741a
@@ -143738,15 +143746,15 @@
    1800673c5:	rex.B
    1800673c6:	rex.RB
    1800673c7:	rex.X push %rsi
    1800673c9:	xor    %esi,(%rdx)
    1800673cb:	rex
    1800673cc:	rex pop %rdx
    1800673ce:	add    %al,(%rax)
-   1800673d0:	add    %al,(%rdx)
+   1800673d0:	or     (%rdx),%eax
    1800673d2:	(bad)
    1800673d3:	imul   $0x65737265,0x74(%rsi),%ebp
    1800673da:	movsxd 0x40(%rbx,%rsi,2),%esi
    1800673de:	(bad)
    1800673df:	and    $0x42,%al
    1800673e1:	outsl  %ds:(%rsi),(%dx)
    1800673e2:	jne    0x180067452
@@ -143763,16 +143771,16 @@
    1800673fd:	rex.B
    1800673fe:	rex.RB
    1800673ff:	rex.X push %rsi
    180067401:	xor    %esi,(%rdx)
    180067403:	rex
    180067404:	rex pop %rdx
    180067406:	add    %al,(%rax)
-   180067408:	test   %eax,(%rdx)
-   18006740a:	(bad)
+   180067408:	xchg   %eax,%ecx
+   180067409:	add    (%rdi),%bh
    18006740b:	jbe    0x180067472
    18006740d:	jb     0x180067483
    18006740f:	imul   $0x243f4073,0x65(%rbx),%esp
    180067416:	rex.RXB
    180067417:	outsb  %gs:(%rsi),(%dx)
    180067419:	gs jb  0x180067485
    18006741c:	movsxd 0x65(%rbx),%edx
@@ -143843,15 +143851,15 @@
    1800674a3:	fs rex
    1800674a5:	rex and $0x30,%al
    1800674a8:	xor    %eax,0x73(%rax)
    1800674ab:	je     0x180067511
    1800674ad:	rex
    1800674ae:	rex pop %rax
    1800674b0:	pop    %rdx
-   1800674b1:	add    %al,0x65763f02(%rsi)
+   1800674b1:	add    %dl,0x65763f02(%rdx)
    1800674b7:	jb     0x18006752d
    1800674b9:	imul   $0x243f4073,0x65(%rbx),%esp
    1800674c0:	rex.RXB
    1800674c1:	outsb  %gs:(%rsi),(%dx)
    1800674c3:	gs jb  0x18006752f
    1800674c6:	movsxd 0x65(%rbx),%edx
    1800674c9:	insl   (%dx),%es:(%edi)
@@ -143982,15 +143990,15 @@
    1800675ca:	outsl  %gs:(%esi),(%dx)
    1800675cd:	insl   (%dx),%es:(%rdi)
    1800675ce:	gs je  0x180067643
    1800675d1:	jns    0x180067601
    1800675d3:	fs insb (%dx),%es:(%rdi)
    1800675d5:	insb   (%dx),%es:(%rdi)
    1800675d6:	add    %al,(%rax)
-   1800675d8:	rolb   $0x3f,(%rax)
+   1800675d8:	roll   $0x3f,(%rax)
    1800675db:	jae    0x180067642
    1800675dd:	je     0x18006763e
    1800675df:	imul   $0x636e6174,0x73(%rsi),%ebp
    1800675e6:	gs rex push %rbx
    1800675e9:	imul   $0x6f74656c,0x67(%rsi),%ebp
    1800675f0:	outsb  %ds:(%rsi),(%dx)
    1800675f1:	rex
@@ -144008,15 +144016,15 @@
    180067605:	imul   $0x5040406f,0x66(%rsi),%ebp
    18006760c:	rex.RB
    18006760d:	push   %r14
    18006760f:	xor    %esi,(%rdx)
    180067611:	rex
    180067612:	rex pop %rdx
    180067614:	add    %al,(%rax)
-   180067616:	mov    %es,(%rax)
+   180067616:	lea    (%rax),%eax
    180067618:	(bad)
    180067619:	imul   $0x636e6174,0x73(%rsi),%ebp
    180067620:	gs rex push %rbx
    180067623:	imul   $0x6f74656c,0x67(%rsi),%ebp
    18006762a:	outsb  %ds:(%rsi),(%dx)
    18006762b:	rex
    18006762c:	outsl  %gs:(%esi),(%dx)
@@ -144085,15 +144093,15 @@
    1800676aa:	rex.B
    1800676ab:	pop    %r8
    1800676ad:	push   %rax
    1800676ae:	rex.RB
    1800676af:	rex.X
    1800676b0:	rex.R
    1800676b1:	rex pop %rdx
-   1800676b3:	add    %dl,0x6f6c3f00(%rdi)
+   1800676b3:	add    %bl,0x6f6c3f00(%rax)
    1800676b9:	addr32 pop %rdi
    1800676bb:	imul   $0x6f4c406f,0x66(%rsi),%ebp
    1800676c2:	addr32 addr32 gs jb 0x180067707
    1800676c7:	outsl  %gs:(%esi),(%dx)
    1800676ca:	fs gs rex
    1800676cd:	rex
    1800676ce:	rex.XB
@@ -144157,15 +144165,16 @@
    180067757:	rex.B
    180067758:	rex.RB
    180067759:	rex.X push %rbp
    18006775b:	xor    %dh,(%rcx)
    18006775d:	rex
    18006775e:	rex pop %rdx
    180067760:	add    %al,(%rax)
-   180067762:	movl   $0x7274733f,(%rax)
+   180067762:	enter  $0x3f00,$0x73
+   180067766:	je     0x1800677da
    180067768:	imul   $0x69757540,0x67(%rsi),%ebp
    18006776f:	fs rex
    180067771:	outsl  %gs:(%esi),(%dx)
    180067774:	fs gs rex
    180067777:	rex push %rcx
    180067779:	rex.RB
    18006777a:	rex.X
@@ -144195,15 +144204,15 @@
    1800677b2:	rex.R
    1800677b3:	rex xor 0x40(%rax),%al
    1800677b7:	jae    0x18006782d
    1800677b9:	fs rex
    1800677bb:	rex pop %rax
    1800677bd:	pop    %rdx
    1800677be:	add    %al,(%rax)
-   1800677c0:	cltd
+   1800677c0:	(bad)
    1800677c1:	add    %bh,(%rdi)
    1800677c3:	insb   (%dx),%es:(%rdi)
    1800677c4:	outsl  %ds:(%rsi),(%dx)
    1800677c5:	addr32 pop %rdi
    1800677c7:	ja     0x18006782a
    1800677c9:	jb     0x180067839
    1800677cb:	rex
```

## Comparing `OpenGeode_Inspector-3.0.4.dist-info/METADATA` & `OpenGeode_Inspector-3.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Inspector
-Version: 3.0.4
+Version: 3.0.5
 Summary: Open source framework for inspecting the validity of geometric models
 Home-page: https://github.com/Geode-solutions/OpenGeode-Inspector
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.0.16)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.6)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.2)
-Requires-Dist: opengeode-io (==6.*,>=6.0.4)
+Requires-Dist: opengeode-core (==14.*,>=14.1.0)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.7)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.3)
+Requires-Dist: opengeode-io (==6.*,>=6.0.6)
 
 <h1 align="center">OpenGeode-Inspector<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenGeode module for inspecting meshes and models</h3>
 
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-ModuleTemplate/workflows/CI/badge.svg" alt="Build Status">
```

### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.4 Summary: Open
+Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.5 Summary: Open
 source framework for inspecting the validity of geometric models Home-page:
 https://github.com/Geode-solutions/OpenGeode-Inspector Author: Geode-solutions
 Author-email: contact@geode-solutions.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown Requires-Dist: opengeode-core
-(==14.*,>=14.0.16) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.6)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.2) Requires-Dist:
-opengeode-io (==6.*,>=6.0.4)
+(==14.*,>=14.1.0) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.7)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.3) Requires-Dist:
+opengeode-io (==6.*,>=6.0.6)
               ****** OpenGeode-Inspectorby Geode-solutions ******
           **** OpenGeode module for inspecting meshes and models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
       [Language] [License] [Semantic-release] [Slack_invite] [DOI] --- ##
  Introduction OpenGeode-Inspector is a module of [OpenGeode] providing ways of
  inspecting your meshes and models and verifying their validity. [OpenGeode]:
```

## Comparing `OpenGeode_Inspector-3.0.4.dist-info/RECORD` & `OpenGeode_Inspector-3.0.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 opengeode_inspector/__init__.py,sha256=PxQ3SsdhF6R2_6Gj0-wVDgy1a-veIjTQApBSB7X5b2U,175
 opengeode_inspector/inspector.py,sha256=gouwVrJtM8c0PoZuR6t9cbtvdpJhrgk_Lvm9PTj-Tws,271
-opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll,sha256=mwBa-sk7Z01L4Fvji0Gczarh6R6I5sLxDjS-f65rDk8,436736
-opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd,sha256=lo-lUJTvUk8QIhNn7VC7fltFKusOFk3Wz9540D1lDoE,451072
-OpenGeode_Inspector-3.0.4.dist-info/METADATA,sha256=qpmSKDHa0gbtjXZwvM8VTu323RB1Sk71E6g3USC7SgM,5481
-OpenGeode_Inspector-3.0.4.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-OpenGeode_Inspector-3.0.4.dist-info/top_level.txt,sha256=HB6mBr33nBKSATXRcJ4Yof7xiFcQAnhw3pFzWTv8zso,20
-OpenGeode_Inspector-3.0.4.dist-info/RECORD,,
+opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll,sha256=vM_KBHgGQOcSDUApz8D3lkkwo5Ei7QFoKScaXyyfTb4,436736
+opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd,sha256=9iHXstA6ALDcMTH2U3Ny_wFR-_zGUsKIVhz6btksd2w,451072
+OpenGeode_Inspector-3.0.5.dist-info/METADATA,sha256=H-GG479HpTFIbP0QkY9YeuqNxfo6MGm9sCoSR4mH2Y8,5480
+OpenGeode_Inspector-3.0.5.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+OpenGeode_Inspector-3.0.5.dist-info/top_level.txt,sha256=HB6mBr33nBKSATXRcJ4Yof7xiFcQAnhw3pFzWTv8zso,20
+OpenGeode_Inspector-3.0.5.dist-info/RECORD,,
```

