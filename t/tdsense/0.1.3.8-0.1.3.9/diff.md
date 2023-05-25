# Comparing `tmp/tdsense-0.1.3.8-py3-none-any.whl.zip` & `tmp/tdsense-0.1.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6059 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       95 b- defN 23-Apr-04 08:31 tdsense/__init__.py
--rw-rw-rw-  2.0 fat    12605 b- defN 23-Feb-17 16:48 tdsense/clustering.py
--rw-rw-rw-  2.0 fat     3662 b- defN 23-Apr-04 08:31 tdsense/plot.py
--rw-rw-rw-  2.0 fat      412 b- defN 23-Jan-02 15:29 tdsense/utils.py
--rw-rw-rw-  2.0 fat      395 b- defN 23-Apr-04 08:33 tdsense-0.1.3.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-04 08:33 tdsense-0.1.3.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-04 08:33 tdsense-0.1.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      601 b- defN 23-Apr-04 08:33 tdsense-0.1.3.8.dist-info/RECORD
-8 files, 17870 bytes uncompressed, 5015 bytes compressed:  71.9%
+Zip file size: 9513 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       95 b- defN 23-May-25 11:13 tdsense/__init__.py
+-rw-rw-rw-  2.0 fat    27231 b- defN 23-May-25 11:11 tdsense/clustering.py
+-rw-rw-rw-  2.0 fat     7424 b- defN 23-May-25 10:52 tdsense/plot.py
+-rw-rw-rw-  2.0 fat     1639 b- defN 23-May-25 11:13 tdsense/utils.py
+-rw-rw-rw-  2.0 fat      395 b- defN 23-May-25 11:13 tdsense-0.1.3.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 11:13 tdsense-0.1.3.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-25 11:13 tdsense-0.1.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      602 b- defN 23-May-25 11:13 tdsense-0.1.3.9.dist-info/RECORD
+8 files, 37486 bytes uncompressed, 8469 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: tdsense/plot.py
 Comment: 
 
 Filename: tdsense/utils.py
 Comment: 
 
-Filename: tdsense-0.1.3.8.dist-info/METADATA
+Filename: tdsense-0.1.3.9.dist-info/METADATA
 Comment: 
 
-Filename: tdsense-0.1.3.8.dist-info/WHEEL
+Filename: tdsense-0.1.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: tdsense-0.1.3.8.dist-info/top_level.txt
+Filename: tdsense-0.1.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: tdsense-0.1.3.8.dist-info/RECORD
+Filename: tdsense-0.1.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdsense/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = '0.1.3.8'
+__version__ = '0.1.3.9'
 
 from .clustering import *
 from .plot import *
 from .utils import *
```

## tdsense/clustering.py

```diff
@@ -10,17 +10,38 @@
 from sklearn.cluster import DBSCAN
 import tqdm
 from scipy.cluster.hierarchy import set_link_color_palette
 
 from matplotlib.pyplot import cm
 import matplotlib as mpl
 
-
+# This function calculates the Dynamic Time Warping (DTW) distance between a reference curve and other curves in a DataFrame.
+# It executes a SQL query using the TD_DTW function in Teradata and returns the result as a DataFrame.
 def dtw(df, curveid_reference, field='calculated_resistance', row_axis='time_no_unit', series_id='curve_id',radius=100, distance='Manhattan'):
+    """
+    Calculate the Dynamic Time Warping (DTW) distance between a reference curve and other curves in a DataFrame.
+
+    Parameters:
+    - df: DataFrame containing the curves data.
+    - curveid_reference: Curve ID of the reference curve.
+    - field: Field name to calculate DTW distance (default: 'calculated_resistance').
+    - row_axis: Field name representing the x-axis (default: 'time_no_unit').
+    - series_id: Field name representing the series identifier (default: 'curve_id').
+    - radius: Radius parameter for DTW calculation (default: 100).
+    - distance: Distance measure for DTW calculation (default: 'Manhattan').
+
+    Returns:
+    - DataFrame containing the DTW distances between the reference curve and other curves.
+
+    Note:
+    - The function assumes the existence of the TD_DTW function in the Teradata environment.
+    - The function requires the 'tdml' module to be available for DataFrame operations.
+    """
 
+    # Construct the SQL query for DTW calculation
     query = f"""
     SELECT
 		{curveid_reference} AS CURVE_ID_1
 	,	A.{series_id} AS CURVE_ID_2
 	,	A.WARPDISTANCE AS DISTANCE
 	FROM (EXECUTE FUNCTION TD_DTW
 	(
@@ -34,22 +55,50 @@
 		),
 		INPUT_FMT(INPUT_MODE(MANY2ONE))
 		)
 	) A
 
     """
 
+    # Execute the SQL query and return the result as a DataFrame
     return tdml.DataFrame.from_query(query)
 
-
+# This function queries the DTW distances between multiple curves using the TD_DTW function in Teradata.
+# It constructs an SQL query to calculate DTW distances in a triangular matrix form and returns the result as a DataFrame.
 def query_dtw_triangle(df, curveids, no, field='calculated_resistance', row_axis='time_no_unit', series_id='curve_id',radius=100, distance='Manhattan',query_only=False):
+    """
+    Query the DTW distances between multiple curves using the TD_DTW function in Teradata.
+
+    Parameters:
+    - df: DataFrame containing the curves data.
+    - curveids: List of curve IDs.
+    - no: Index of the curve ID to use as a reference for calculating DTW distances.
+    - field: Field name to calculate DTW distance (default: 'calculated_resistance').
+    - row_axis: Field name representing the x-axis (default: 'time_no_unit').
+    - series_id: Field name representing the series identifier (default: 'curve_id').
+    - radius: Radius parameter for DTW calculation (default: 100).
+    - distance: Distance measure for DTW calculation (default: 'Manhattan').
+    - query_only: If True, returns the SQL query string without executing it (default: False).
+
+    Returns:
+    - If query_only is True, returns the SQL query string.
+    - Otherwise, returns the result of the query as a DataFrame.
+
+    Note:
+    - The function assumes the existence of the TD_DTW function in the Teradata environment.
+    - The function requires the 'tdml' module to be available for DataFrame operations.
+    """
+
+    # Execute the DataFrame node to obtain the table name
     df._DataFrame__execute_node_and_set_table_name(df._nodeid, df._metaexpr)
 
-    curveids.sort()
+    # Sort the curve IDs
+    curveids = curveids.sort()
 
+    # Construct the SQL query for DTW distance calculation
     query = f"""
     SELECT
         CAST({no} AS BIGINT) AS MATRIX_ROW
 	,	CAST({curveids[no]} AS BIGINT) AS CURVE_ID_1
 	,	CAST(A.{series_id} AS BIGINT) AS CURVE_ID_2
 	,	A.ROW_I
 	,	A.WARPDISTANCE AS DISTANCE
@@ -68,33 +117,86 @@
 	) A
 
     """
 
     if query_only:
         return query
 
+    # Execute the SQL query and return the result as a DataFrame
     return tdml.DataFrame.from_query(query)
 
-
+# This function computes the DTW distance matrix between multiple curves and stores it in a table in Teradata.
+# It iterates over the curve IDs and uses the query_dtw_triangle function to calculate DTW distances.
+# The distances are stored in the specified table in Teradata, and the result is returned as a DataFrame.
 def dtw_distance_matrix_computation(df, curveids, table_name, schema_name, field='calculated_resistance', row_axis='time_no_unit', series_id='curve_id',radius=100, distance='Manhattan'):
+    """
+    Compute the DTW distance matrix between multiple curves and store it in a table in Teradata.
 
+    Parameters:
+    - df: DataFrame containing the curves data.
+    - curveids: List of curve IDs.
+    - table_name: Name of the table to store the distance matrix in Teradata.
+    - schema_name: Schema name in Teradata for table creation.
+    - field: Field name to calculate DTW distance (default: 'calculated_resistance').
+    - row_axis: Field name representing the x-axis (default: 'time_no_unit').
+    - series_id: Field name representing the series identifier (default: 'curve_id').
+    - radius: Radius parameter for DTW calculation (default: 100).
+    - distance: Distance measure for DTW calculation (default: 'Manhattan').
+
+    Returns:
+    - DataFrame containing the DTW distance matrix.
+
+    Note:
+    - The function assumes the existence of the query_dtw_triangle and insert_into functions.
+    - The function assumes the availability of the 'tdml' module for DataFrame operations.
+    """
+
+    # Iterate over the curve IDs
     for no in range(1, len(curveids)):
+        # Generate the DTW query for the current curve ID
         dtw_query = query_dtw_triangle(df, curveids, no, field=field, row_axis=row_axis,
                                series_id=series_id, radius=radius, distance=distance, query_only=True)
         if no == 1:
+            # Create the distance matrix table in Teradata using the first DTW query
             tdml.DataFrame.from_query(dtw_query).to_sql(table_name=table_name,schema_name=schema_name,if_exists='replace')
         else:
+            # Insert the DTW distances into the distance matrix table for subsequent curve IDs
             tdml.get_context().execute(insert_into(dtw_query,table_name,schema_name))
 
-
+    # Return the distance matrix as a DataFrame
     return tdml.DataFrame.from_table(tdml.in_schema(schema_name,table_name))
 
+# This function computes the DTW distance matrix between curves in a DataFrame and stores it in a table in Teradata.
+# It iterates over the curves and uses the query_dtw_triangle function to calculate DTW distances.
+# The distances are stored in the specified table in Teradata, and the result is returned as a DataFrame.
 def dtw_distance_matrix_computation(df, table_name, schema_name, field='calculated_resistance', row_axis='time_no_unit', series_id='curve_id',radius=100, distance='Manhattan'):
+    """
+    Compute the DTW distance matrix between curves in a DataFrame and store it in a table in Teradata.
+
+    Parameters:
+    - df: DataFrame containing the curves data.
+    - table_name: Name of the table to store the distance matrix in Teradata.
+    - schema_name: Schema name in Teradata for table creation.
+    - field: Field name to calculate DTW distance (default: 'calculated_resistance').
+    - row_axis: Field name representing the x-axis (default: 'time_no_unit').
+    - series_id: Field name representing the series identifier (default: 'curve_id').
+    - radius: Radius parameter for DTW calculation (default: 100).
+    - distance: Distance measure for DTW calculation (default: 'Manhattan').
+
+    Returns:
+    - DataFrame containing the DTW distance matrix.
+
+    Note:
+    - The function assumes the existence of the query_dtw_triangle and insert_into functions.
+    - The function assumes the availability of the 'tdml' module for DataFrame operations.
+    """
 
+    # Iterate over the curves
     for no in range(1, len(curveids)):
+        # Generate the DTW query for the current curve
         dtw_query = query_dtw_triangle(df, curveids, no, field=field, row_axis=row_axis,
                                series_id=series_id, radius=radius, distance=distance, query_only=True)
         if no == 1:
             tdml.DataFrame.from_query(dtw_query).to_sql(table_name=table_name,schema_name=schema_name,if_exists='replace')
         else:
             tdml.get_context().execute(insert_into(dtw_query,table_name,schema_name))
 
@@ -103,125 +205,273 @@
 
 def dtw_distance_matrix_computation(df, table_name, schema_name, field='calculated_resistance', row_axis='time_no_unit', series_id='curve_id',radius=100, distance='Manhattan'):
 
     for no in range(1, len(curveids)):
         dtw_query = query_dtw_triangle(df, curveids, no, field=field, row_axis=row_axis,
                                series_id=series_id, radius=radius, distance=distance, query_only=True)
         if no == 1:
+            # Create the distance matrix table in Teradata using the first DTW query
             tdml.DataFrame.from_query(dtw_query).to_sql(table_name=table_name,schema_name=schema_name,if_exists='replace')
         else:
+            # Insert the DTW distances into the distance matrix table for subsequent curves
             tdml.get_context().execute(insert_into(dtw_query,table_name,schema_name))
 
-
+    # Return the distance matrix as a DataFrame
     return tdml.DataFrame.from_table(tdml.in_schema(schema_name,table_name))
+
+# This function retrieves the DTW distance matrix from a local DataFrame and sorts it based on curve IDs.
 def get_dtw_distance_matrix_local(dtw_matrix_vantage):
+    """
+    Get the DTW distance matrix from a local DataFrame and sort it based on curve IDs.
+
+    Parameters:
+    - dtw_matrix: Local DataFrame containing the DTW distance matrix.
 
+    Returns:
+    - Sorted DTW distance matrix as a pandas DataFrame.
+
+    Note:
+    - The function assumes the availability of the pandas library.
+    """
+    # Sort the DTW distance matrix based on curve IDs and Convert the sorted DTW distance matrix to a pandas DataFrame
     return dtw_matrix.sort(columns=['CURVE_ID_2','CURVE_ID_1']).to_pandas(all_rows=True)
 
+# This function extracts the DTW distances and labels from a local DTW distance matrix DataFrame.
 def extractmatrixlabel(dtw_matrix_vantage_local):
+    """
+    Extract the DTW distances and labels from a local DTW distance matrix DataFrame.
+
+    Parameters:
+    - dtw_matrix_local: Local DataFrame containing the DTW distance matrix.
+
+    Returns:
+    - X: NumPy array containing the DTW distances.
+    - labelList: List containing the labels.
+
+    Note:
+    - The function assumes the availability of the NumPy library.
+    """
+
+    # Extract the DTW distances from the DataFrame
     X = dtw_matrix_vantage_local.DISTANCE.values
+
+    # Extract the labels from the DataFrame
     labelList = [dtw_matrix_vantage_local.iloc[0,2]] + list(dtw_matrix_vantage_local.iloc[0:int(np.floor(np.sqrt(len(X)*2))),1])
+
+    # Return the DTW distances and labels
     return X, labelList
 
+# This function generates a hierarchical dendrogram based on a DTW distance matrix.
 def hierarchy_dendrogram(dtw_matrix_vantage_local, cluster_distance = 'single'):
+    """
+    Generate a hierarchical dendrogram based on a DTW distance matrix.
 
+    Parameters:
+    - dtw_matrix_local: Local DataFrame containing the DTW distance matrix.
+    - cluster_distance: Distance metric for hierarchical clustering (default: 'single').
+
+    Returns:
+    - linked: Resulting linkage matrix from hierarchical clustering.
+    - labelList: List of labels.
+
+    Note:
+    - The function assumes the availability of the matplotlib and scipy libraries.
+    """
+
+    # Extract DTW distances and labels from the DTW distance matrix
     X, labelList = extractmatrixlabel(dtw_matrix_vantage_local)
 
+    # Update the font size for better visualization
     rcParams.update({'font.size': 22})
 
+    # Perform hierarchical clustering and obtain the linkage matrix
     linked = linkage(X, cluster_distance)
 
+    # Create the dendrogram plot
     plt.figure(figsize=(25, 15))
     Z = dendrogram(linked,
                    orientation='top',
                    labels=labelList,
                    distance_sort='ascending',
                    show_leaf_counts=True)
+
+    # Update the font size for better axis label visibility
     plt.rcParams.update({'font.size': 22})
     ax = plt.gca()
     ax.tick_params(axis='x', which='major', labelsize=15)
 
+    # Return the linkage matrix and label list
     return linked, labelList
 
 
 from scipy.cluster.hierarchy import dendrogram, linkage, cut_tree, set_link_color_palette
 import pandas as pd
 from matplotlib.pyplot import cm
 import matplotlib as mpl
 
-
+# This function performs hierarchical clustering based on a linkage matrix and returns the resulting clusters.
 def hierarchy_clustering(linked, labelList, n_clusters=None, height=None, plot_dendrogram=True):
+    """
+    Perform hierarchical clustering based on a linkage matrix and return the resulting clusters.
+
+    Parameters:
+    - linked: Linkage matrix from hierarchical clustering.
+    - labelList: List of labels.
+    - n_clusters: Number of clusters to extract (default: None).
+    - height: Height threshold to extract clusters (default: None).
+    - plot_dendrogram: Whether to plot the dendrogram with cluster colors (default: True).
+
+    Returns:
+    - clusters: DataFrame containing the cluster assignments and labels.
+
+    Note:
+    - The function assumes the availability of the pandas, numpy, and matplotlib libraries.
+    """
+
+    # Perform clustering based on the specified parameters
     if n_clusters is not None:
         cutree_ = cut_tree(linked, n_clusters=n_clusters)
     if height is not None:
         cutree_ = cut_tree(linked, height=height)
 
     # Get the cluster labels for each data point
     cluster_labels = cutree_.flatten()
 
     cl = [x[0] for x in cutree_]
     n_clusters = len(set(cl))
     clusters = pd.DataFrame()
     clusters['CURVE_ID'] = labelList
     clusters['cluster'] = cl
 
+    # Compute the color threshold for plotting the dendrogram
     thresh = np.sort(-linked[:, 2])
     thresh = -thresh[n_clusters - 1] + 1e-10
 
+    # Compute the color map for the clusters
     cmap = cm.rainbow(np.linspace(0, 1, n_clusters))
     set_link_color_palette([mpl.colors.rgb2hex(rgb[:3]) for rgb in cmap])
 
     if plot_dendrogram:
         # Create a figure and plot the dendrogram with the cluster colors
         fig, ax = plt.subplots(figsize=(15, 15))
         dn = dendrogram(linked, color_threshold=thresh)
 
+        # Create a DataFrame with the cluster assignments, labels, and color information
         df = pd.DataFrame(columns=['leaves_color_list'])
         df['leaves_color_list'] = dn['leaves_color_list']
         df['cluster'] = [cl[x] for x in dn['leaves']]
         df['CURVE_ID'] = [labelList[x] for x in dn['leaves']]
         df.drop_duplicates(inplace=True)
         df_ = df.copy().drop('CURVE_ID',axis=1).drop_duplicates()
+
         # Create a list of labels for the clusters
         cluster_labels = ['Cluster ' + str(x['cluster']) for i, x in df_.iterrows()]
         plt.legend(cluster_labels)
 
         clusters = df[list(clusters.columns) + ['leaves_color_list']].sort_values('CURVE_ID')
 
     return clusters
 
 
 
-
+# This function computes the distance elbow plot based on a DTW distance matrix.
 def distance_elbow(dtw_matrix_vantage_local):
+    """
+    Compute the distance elbow plot based on a DTW distance matrix.
+
+    Parameters:
+    - dtw_matrix_local: Local DataFrame containing the DTW distance matrix.
+
+    Returns:
+    - None
+
+    Note:
+    - The function assumes the availability of the sklearn and matplotlib libraries.
+    """
+
+    # Extract DTW distances and labels from the DTW distance matrix
     X, labelList = extractmatrixlabel(dtw_matrix_vantage_local)
+
+    # Fit the nearest neighbors model to the DTW distance matrix
     neigh = NearestNeighbors(n_neighbors=2)
     nbrs = neigh.fit(squareform(X))
+
+    # Compute the distances to the nearest neighbor for each point
     distances, indices = nbrs.kneighbors(squareform(X))
     distances = np.sort(distances, axis=0)
     distances = distances[:, 1]
+
+    # Plot the distance elbow plot
     plt.plot(distances)
+
+    # No need to return anything since the plot is displayed
     return
 
+# This function performs density-based clustering using DBSCAN on a DTW distance matrix.
 def densityscan(dtw_matrix_vantage_local, eps, min_samples):
+    """
+    Perform density-based clustering using DBSCAN on a DTW distance matrix.
+
+    Parameters:
+    - dtw_matrix_local: Local DataFrame containing the DTW distance matrix.
+    - eps: The maximum distance between two samples to be considered as neighbors (DBSCAN parameter).
+    - min_samples: The minimum number of samples in a neighborhood for a point to be considered as a core point (DBSCAN parameter).
+
+    Returns:
+    - clusters: DataFrame containing the cluster assignments and labels.
+
+    Note:
+    - The function assumes the availability of the sklearn and pandas libraries.
+    """
+
+    # Extract DTW distances and labels from the DTW distance matrix
     X, labelList = extractmatrixlabel(dtw_matrix_vantage_local)
+
+    # Perform density-based clustering using DBSCAN
     db = DBSCAN(eps=eps, min_samples=min_samples).fit(squareform(X))
+
+    # Create the clusters DataFrame with CURVE_ID and cluster columns
     clusters = pd.DataFrame()
     clusters['CURVE_ID'] = labelList
     clusters['cluster'] = db.labels_
-    return clusters
 
+    # Return the clusters DataFrame
+    return clusters
 
+# This function computes the DTW distance matrix for a specific curve against a subset of curves in a DataFrame.
 def query_dtw_triangle2(df, curveids, no, field='calculated_resistance', row_axis='time_no_unit', series_id='curve_id',
                         radius=100, distance='Manhattan', query_only=False):
+    """
+    Compute the DTW distance matrix for a specific curve against a subset of curves in a DataFrame.
+
+    Parameters:
+    - df: DataFrame containing the curves data.
+    - curveids: List of curve IDs.
+    - no: Index of the current curve in curveids.
+    - field: Field name to calculate DTW distance (default: 'calculated_resistance').
+    - row_axis: Field name representing the x-axis (default: 'time_no_unit').
+    - series_id: Field name representing the series identifier (default: 'curve_id').
+    - radius: Radius parameter for DTW calculation (default: 100).
+    - distance: Distance measure for DTW calculation (default: 'Manhattan').
+    - query_only: Whether to return the DTW query string only (default: False).
+
+    Returns:
+    - DataFrame containing the DTW distance matrix for the specific curve.
+
+    Note:
+    - The function assumes the availability of the tdml module for DataFrame operations.
+    """
+
+    # Extract the subsets of curves for DTW computation
     df1 = df[df[series_id] < curveids[no]]
     df1._DataFrame__execute_node_and_set_table_name(df1._nodeid, df1._metaexpr)
     df2 = df[df[series_id] == curveids[no]]
     df2._DataFrame__execute_node_and_set_table_name(df2._nodeid, df2._metaexpr)
 
+    # Generate the DTW query for the specific curve and subset of curves
     query = f"""
     SELECT
         CAST({no} AS BIGINT) AS MATRIX_ROW
 	,	CAST({curveids[no]} AS BIGINT) AS {series_id}_1
 	,	CAST(A.{series_id} AS BIGINT) AS {series_id}_2
 	,	A.ROW_I
 	,	A.WARPDISTANCE AS DISTANCE
@@ -237,29 +487,53 @@
 		),
 		INPUT_FMT(INPUT_MODE(MANY2ONE))
 		)
 	) A
 
     """
 
+    # Return the DTW query string if query_only is True
     if query_only:
         return query
 
+    # Return the DTW distance matrix as a DataFrame
     return tdml.DataFrame.from_query(query)
 
-
+# This function computes the DTW distance matrix for a set of curves and stores the results in a table.
 def dtw_distance_matrix_computation2(df, table_name, schema_name, curveids=None, field='calculated_resistance',
                                      row_axis='time_no_unit', series_id='curve_id', radius=100, distance='Manhattan',
                                      restart=1):
-    # get the list of curve ids
+    """
+    Compute the DTW distance matrix for a set of curves and store the results in a table.
+
+    Parameters:
+    - df: DataFrame containing the curves data.
+    - table_name: Name of the table to store the DTW distance matrix.
+    - schema_name: Name of the schema where the table will be created.
+    - curveids: List of curve IDs (default: None).
+    - field: Field name to calculate DTW distance (default: 'calculated_resistance').
+    - row_axis: Field name representing the x-axis (default: 'time_no_unit').
+    - series_id: Field name representing the series identifier (default: 'curve_id').
+    - radius: Radius parameter for DTW calculation (default: 100).
+    - distance: Distance measure for DTW calculation (default: 'Manhattan').
+    - restart: Index to restart the computation from (default: 1).
+
+    Returns:
+    - DataFrame containing the DTW distance matrix.
+
+    Note:
+    - The function assumes the availability of the pandas, tqdm, and tdml modules.
+    """
+
+    # Get the list of curve IDs if not provided
     if curveids == None:
         filter_curveid = {'drop_columns': True, series_id: df[series_id].distinct()}
         curveids = list(df.assign(**filter_curveid).sort(series_id).to_pandas()[series_id])
 
-    # create the table to store the results
+    # Create the table to store the results if restart is 1
     if restart == 1:
         # only in this case we recreate the table from scratch
         res = pd.DataFrame(columns=['MATRIX_ROW', series_id + '_1', series_id + '_2', 'ROW_ID', 'DISTANCE'])
         tdml.copy_to_sql(res,
                          schema_name=schema_name,
                          table_name=table_name,
                          if_exists='replace',
@@ -267,14 +541,15 @@
                              'MATRIX_ROW': tdml.BIGINT,
                              series_id + '_1': tdml.BIGINT,
                              series_id + '_2': tdml.BIGINT,
                              'ROW_ID': tdml.BIGINT,
                              'DISTANCE': tdml.FLOAT
                          })
 
+    # Perform the DTW distance matrix computation for each curve
     progress_bar = tqdm.tqdm(range(1, len(curveids)))
     for no in progress_bar:
 
         if no >= restart:
             progress_bar.set_description(f"Process curve {curveids[no]}")
             dtw_query = query_dtw_triangle2(df, curveids, no, field=field, row_axis=row_axis,
                                             series_id=series_id, radius=radius, distance=distance, query_only=True)
@@ -282,19 +557,43 @@
                 INSERT INTO {schema_name}.{table_name} (MATRIX_ROW, {series_id + '_1'}, {series_id + '_2'}, ROW_ID, DISTANCE)
                 {dtw_query}
             '''
             tdml.get_context().execute(query)
         else:
             progress_bar.set_description(f"Skip curve {curveids[no]}")
 
+    # Return the DTW distance matrix as a DataFrame
     return tdml.DataFrame.from_table(tdml.in_schema(schema_name, table_name))
 
+# This function resamples a time series DataFrame based on a specified duration.
 def resample(df, duration, field, series_id, row_axis, start_value=0, interpolate='LINEAR',query_only=False):
+    """
+    Resample a time series DataFrame based on a specified duration.
+
+    Parameters:
+    - df: DataFrame containing the time series data.
+    - duration: Duration for resampling.
+    - field: Field name to resample.
+    - series_id: Field name representing the series identifier.
+    - row_axis: Field name representing the row axis.
+    - start_value: Starting value for the resampling sequence (default: 0).
+    - interpolate: Interpolation method for resampling (default: 'LINEAR').
+    - query_only: Whether to return the resampling query string only (default: False).
+
+    Returns:
+    - DataFrame containing the resampled time series.
+
+    Note:
+    - The function assumes the availability of the tdml module for DataFrame operations.
+    """
+
+    # Set the table name for the DataFrame
     df._DataFrame__execute_node_and_set_table_name(df._nodeid, df._metaexpr)
 
+    # Generate the resampling query
     query = f"""
     SELECT
         {series_id}
     ,   ROW_I AS {row_axis}
     ,   {field}
     FROM (
         EXECUTE FUNCTION
@@ -313,11 +612,13 @@
                 SEQUENCE (START_VALUE ({start_value}), DURATION ({duration})),
                 INTERPOLATE ('{interpolate}')
             )
             )
         ) A
     """
 
+    # Return the resampling query string if query_only is True
     if query_only:
         return query
 
+    # Return the resampled time series as a DataFrame
     return tdml.DataFrame.from_query(query)
```

## tdsense/plot.py

```diff
@@ -1,43 +1,72 @@
 import teradataml as tdml
 import io
 from IPython.display import Image
 import imageio
 
-
+# This function plots curves using TD_PLOT function from a DataFrame in Teradata.
+# It generates an image of the plot and returns either the image data or displays the image.
 def plotcurves(df, field='calculated_resistance', row_axis='time_no_unit', series_id='curve_id', select_id=None,
                width=1024, height=768, noplot=False, color=None, row_axis_type='SEQUENCE', plot_type='line'):
+    """
+    Plot curves using TD_PLOT function from a DataFrame in Teradata.
+
+    Parameters:
+    - df: DataFrame containing the data to plot.
+    - field: Field name to plot (default: 'calculated_resistance').
+    - row_axis: Field name representing the x-axis (default: 'time_no_unit').
+    - series_id: Field name representing the series identifier (default: 'curve_id').
+    - select_id: Optional, series identifier(s) to select (can be a single value or a list) (default: None).
+    - width: Width of the plot image in pixels (default: 1024).
+    - height: Height of the plot image in pixels (default: 768).
+    - noplot: If True, returns the image data without displaying the image (default: False).
+    - color: Optional, color specification for the plot (default: None).
+    - row_axis_type: Type of the row axis, either 'SEQUENCE' or 'TIME' (default: 'SEQUENCE').
+    - plot_type: Type of plot, either 'line' or 'scatter' (default: 'line').
+
+    Returns:
+    - If noplot is True, returns the image data as a NumPy array.
+    - Otherwise, displays the image.
+
+    Note:
+    - The function assumes the existence of a TD_PLOT function in the Teradata environment.
+    - The function requires the 'imageio' and 'Pillow' libraries to be installed.
+    """
+
+    # Execute the DataFrame node to obtain the table name
     df._DataFrame__execute_node_and_set_table_name(df._nodeid, df._metaexpr)
 
+    # Construct the filter clause based on select_id
     if isinstance(select_id, list):
         if len(series_id) > 0:
             filter_ = f"WHERE {series_id} IN ({','.join([str(x) for x in select_id])}),"
         else:
             filter_ = ','
     else:
         if select_id is not None:
             filter_ = f"WHERE {series_id} = {select_id},"
         else:
             filter_ = ','
 
-
-
+    # Calculate the number of series in the DataFrame
     nb_series = df[[series_id]+[row_axis]].groupby(series_id).count().shape[0]
 
+    # Determine the number of plots based on series_id
     n = 1
     if type(series_id) == list:
         n = len(series_id)
         series_id = ','.join(series_id)
 
+    # Handle the color parameter
     if color == None:
         color = ''
     else:
         color = f",FORMAT('{color}')"
 
-
+    # Construct the query based on the number of series
     if nb_series < 1025:
         query = f"""
         EXECUTE FUNCTION
             TD_PLOT(
                 SERIES_SPEC(
                 TABLE_NAME({df._table_name}),
                 ROW_AXIS({row_axis_type}({row_axis})),
@@ -56,14 +85,15 @@
             )],
             WIDTH({width}),
             HEIGHT({height})
             )
             );
         """
     else:
+        # Create a modified DataFrame to handle a large number of series
         df_ = df.assign(**{series_id: 1})
         df_._DataFrame__execute_node_and_set_table_name(df_._nodeid, df_._metaexpr)
         query = f"""
         EXECUTE FUNCTION
             TD_PLOT(
                 SERIES_SPEC(
                 TABLE_NAME({df_._table_name}),
@@ -83,37 +113,69 @@
             )],
             WIDTH({width}),
             HEIGHT({height})
             )
             );
         """
 
+    # Print the query if tdml.display.print_sqlmr_query is True
     if tdml.display.print_sqlmr_query:
         print(query)
 
+    # Execute the query and fetch the result
     res = tdml.get_context().execute(query).fetchall()
 
+    # Get the image data from the result
     stream_str = io.BytesIO(res[0][1 + n])
 
+    # Return the image data or display the image
     if noplot:
         return imageio.imread(stream_str.getvalue())
     else:
         return Image(stream_str.getvalue())
 
+# This function plots curves from a DataFrame that belongs to a specific cluster.
+# It copies the cluster DataFrame to a temporary table in Teradata, performs a join with the original DataFrame,
+# and then calls the plotcurves function to generate the plot.
 def plotcurvescluster(df, cluster, no_cluster, schema, field='calculated_resistance', row_axis='time_no_unit', series_id='CURVE_ID', select_id=None):
+    """
+    Plot curves from a DataFrame that belongs to a specific cluster.
+
+    Parameters:
+    - df: Original DataFrame containing the data to plot.
+    - cluster: DataFrame containing the cluster information.
+    - no_cluster: Cluster number to select.
+    - schema: Schema name in the Teradata environment for temporary table creation.
+    - field: Field name to plot (default: 'calculated_resistance').
+    - row_axis: Field name representing the x-axis (default: 'time_no_unit').
+    - series_id: Field name representing the series identifier (default: 'CURVE_ID').
+    - select_id: Optional, series identifier(s) to select (can be a single value or a list) (default: None).
+
+    Returns:
+    - The result of the plotcurves function called on the selected DataFrame.
+
+    Note:
+    - The function assumes the existence of the plotcurves function.
+    - The function assumes the availability of the 'tdml' module for DataFrame operations.
+    """
 
+    # Copy the cluster DataFrame to a temporary table in Teradata
     tdml.copy_to_sql(df=cluster,table_name='cluster_temp',if_exists='replace',schema_name=schema)
 
+    # Create a DataFrame for the cluster temporary table
     df_cluster = tdml.DataFrame(tdml.in_schema(schema,'cluster_temp'))
+
+    # Join the original DataFrame with the cluster DataFrame based on the cluster number and series identifier
     df_select = df.join(df_cluster[df_cluster.cluster == no_cluster],
                         how='inner',
                         on=f'{series_id}=CURVE_ID', rsuffix='r',
                         lsuffix='l')
     try:
+        # Assign the selected series identifier from the left DataFrame and drop unnecessary columns
         df_select = df_select.assign(**{series_id: df_select['l_' + series_id]}).drop(
             columns=[f'l_{series_id}', 'r_CURVE_ID'])
     except:
-        1==1
+        1==1 # Placeholder statement to handle any exception silently
     df_select.shape
 
-
+    # Call the plotcurves function with the selected DataFrame and other parameters
     return plotcurves(df_select,field=field, row_axis=row_axis, series_id=series_id,select_id=select_id)
```

## tdsense/utils.py

```diff
@@ -1,19 +1,55 @@
+# This function creates a table based on a given query.
 def create_table(query, table_name, schema_name):
+    """
+    Create a table based on a given query.
+
+    Parameters:
+    - query: SQL query for creating the table.
+    - table_name: Name of the table to be created.
+    - schema_name: Name of the schema where the table will be created.
+
+    Returns:
+    - query: SQL query for creating the table.
+
+    Note:
+    - The function assumes the availability of the specified schema.
+    """
+
+    # Generate the SQL query for creating the table
     query = f"""
     CREATE TABLE {schema_name}.{table_name} AS 
     (
         {query}
     ) WITH DATA
     --PRIMARY INDEX (CURVE_ID_1, CURVE_ID_2)
     NO PRIMARY INDEX
     """
-    return query
 
+    # Return the SQL query for creating the table
+    return query
 
+# This function generates an INSERT INTO query for inserting data into a table.
 def insert_into(query, table_name, schema_name):
+    """
+    Generate an INSERT INTO query for inserting data into a table.
+
+    Parameters:
+    - query: SQL query for the data to be inserted.
+    - table_name: Name of the table to insert the data into.
+    - schema_name: Name of the schema where the table is located.
+
+    Returns:
+    - query: SQL query for inserting data into the table.
+
+    Note:
+    - The function assumes the availability of the specified schema and table.
+    """
+
+    # Generate the SQL query for inserting data into the table
     query = f"""
     INSERT INTO {schema_name}.{table_name}  
     {query}
     """
 
+    # Return the SQL query for inserting data into the table
     return query
```

