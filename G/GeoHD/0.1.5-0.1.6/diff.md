# Comparing `tmp/GeoHD-0.1.5.tar.gz` & `tmp/GeoHD-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.1.5.tar", last modified: Fri Apr  5 18:55:29 2024, max compression
+gzip compressed data, was "GeoHD-0.1.6.tar", last modified: Sun Apr  7 19:29:54 2024, max compression
```

## Comparing `GeoHD-0.1.5.tar` & `GeoHD-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 18:55:29.963652 GeoHD-0.1.5/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:55:29.955590 GeoHD-0.1.5/GeoHD/
--rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.5/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.1.5/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.5/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.1.5/GeoHD/process.py
--rw-rw-rw-   0        0        0     7367 2024-04-02 18:00:56.000000 GeoHD-0.1.5/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.1.5/GeoHD/visualize.py
--rw-rw-rw-   0        0        0     9599 2024-04-05 18:21:57.000000 GeoHD-0.1.5/GeoHD/zone.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:55:29.961645 GeoHD-0.1.5/GeoHD.egg-info/
--rw-rw-rw-   0        0        0      405 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      405 2024-04-05 18:55:29.962649 GeoHD-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4768 2024-04-05 18:54:02.000000 GeoHD-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 18:55:29.963995 GeoHD-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      484 2024-04-05 18:54:02.000000 GeoHD-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:55:29.961110 GeoHD-0.1.5/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.5/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:29:54.035588 GeoHD-0.1.6/
+drwxrwxrwx   0        0        0        0 2024-04-07 19:29:54.025587 GeoHD-0.1.6/GeoHD/
+-rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.6/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.1.6/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.6/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.1.6/GeoHD/process.py
+-rw-rw-rw-   0        0        0    10832 2024-04-07 19:23:12.000000 GeoHD-0.1.6/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.1.6/GeoHD/visualize.py
+-rw-rw-rw-   0        0        0     9599 2024-04-05 18:21:57.000000 GeoHD-0.1.6/GeoHD/zone.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:29:54.033587 GeoHD-0.1.6/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0     5266 2024-04-07 19:29:53.000000 GeoHD-0.1.6/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-07 19:29:53.000000 GeoHD-0.1.6/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 19:29:53.000000 GeoHD-0.1.6/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-07 19:29:53.000000 GeoHD-0.1.6/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 19:29:53.000000 GeoHD-0.1.6/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     5266 2024-04-07 19:29:54.034586 GeoHD-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4768 2024-04-05 18:54:02.000000 GeoHD-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 19:29:54.035588 GeoHD-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-04-07 19:27:57.000000 GeoHD-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:29:54.032586 GeoHD-0.1.6/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.6/test/__init__.py
```

### Comparing `GeoHD-0.1.5/GeoHD/AKDE.py` & `GeoHD-0.1.6/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.5/GeoHD/analyze.py` & `GeoHD-0.1.6/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.5/GeoHD/process.py` & `GeoHD-0.1.6/GeoHD/process.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.5/GeoHD/utils.py` & `GeoHD-0.1.6/GeoHD/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -48,14 +48,97 @@
     plt.scatter(hotspots[:, 1], hotspots[:, 0], color='red', s=5, label='Hotspots')
     plt.xlabel('X')
     plt.ylabel('Y')
     plt.title('Hotspot Extraction')
     plt.legend()
     plt.show()
 
+def spectral_clustering_with_plot(points_shapefile, num_clusters=3, k=5, sigma=1):
+    """
+    Perform spectral clustering on a set of points from a shapefile and plot the clusters.
+
+    Args:
+    points_shapefile (str): Path to the shapefile containing point data.
+    num_clusters (int): Number of clusters to partition the data into.
+    k (int): Number of nearest neighbors to consider for constructing the adjacency matrix.
+    sigma (float): Sigma parameter for the Gaussian similarity function.
+
+    Returns:
+    np.array: Cluster labels for each point.
+    """
+
+    def gaussian_similarity_matrix(points, sigma=1):
+        n = len(points)
+        similarity_matrix = np.zeros((n, n))
+        for i in range(n):
+            for j in range(n):
+                similarity_matrix[i][j] = np.exp(-((points[i].x - points[j].x) ** 2 + (points[i].y - points[j].y) ** 2) / (2 * sigma ** 2))
+        return similarity_matrix
+
+    def adjacency_matrix(similarity_matrix, k):
+        n = len(similarity_matrix)
+        adjacency_matrix = np.zeros((n, n))
+        for i in range(n):
+            idx = np.argsort(similarity_matrix[i])[::-1][:k]
+            adjacency_matrix[i][idx] = similarity_matrix[i][idx]
+        return adjacency_matrix
+
+    def laplacian_matrix(adjacency_matrix):
+        degree_matrix = np.diag(np.sum(adjacency_matrix, axis=1))
+        laplacian_matrix = degree_matrix - adjacency_matrix
+        return laplacian_matrix
+
+    def compute_eigenvectors(laplacian_matrix, num_eigenvectors):
+        eigenvalues, eigenvectors = np.linalg.eig(laplacian_matrix)
+        sorted_indices = np.argsort(eigenvalues)
+        sorted_eigenvalues = eigenvalues[sorted_indices]
+        sorted_eigenvectors = eigenvectors[:, sorted_indices]
+        return sorted_eigenvalues, sorted_eigenvectors[:, :num_eigenvectors]
+
+    def kmeans_clustering(data, k, max_iters=100):
+        centroids = data[np.random.choice(data.shape[0], k, replace=False)]
+        for _ in range(max_iters):
+            distances = np.sqrt(((data - centroids[:, np.newaxis])**2).sum(axis=2))
+            labels = np.argmin(distances, axis=0)
+            new_centroids = np.array([data[labels == i].mean(axis=0) for i in range(k)])
+            if np.all(centroids == new_centroids):
+                break
+            centroids = new_centroids
+        return labels
+
+    # Load shapefile point data
+    points_gdf = gpd.read_file(points_shapefile)
+
+    # Compute similarity matrix
+    similarity_matrix = gaussian_similarity_matrix(points_gdf.geometry, sigma)
+
+    # Construct adjacency matrix
+    adj_matrix = adjacency_matrix(similarity_matrix, k)
+
+    # Compute Laplacian matrix
+    laplacian_matrix = laplacian_matrix(adj_matrix)
+
+    # Compute eigenvectors of Laplacian matrix
+    eigenvalues, eigenvectors = compute_eigenvectors(laplacian_matrix, num_clusters)
+
+    # K-means clustering using eigenvectors
+    cluster_labels = kmeans_clustering(eigenvectors, num_clusters)
+
+    # Plot clusters
+    fig, ax = plt.subplots(figsize=(10, 10))
+    colors = ['r', 'g', 'b']
+    for i in range(cluster_labels.max() + 1):
+        ax.scatter(points_gdf.geometry.x[cluster_labels == i], points_gdf.geometry.y[cluster_labels == i], c=colors[i], label=f'Cluster {i+1}')
+    ax.legend()
+    plt.title('Spectral Clustering')
+    plt.xlabel('Longitude')
+    plt.ylabel('Latitude')
+    plt.show()
+
+    return cluster_labels
 
 def km_euclidean_distance(x1, x2):
     """Calculate the Euclidean distance between two points for K-Means."""
     return np.sqrt(np.sum((x1 - x2)**2))
 
 def km_initialize_centroids(X, n_clusters, random_state=None):
     """Initialize centroids for K-Means clustering."""
@@ -195,14 +278,12 @@
     plt.show()
 
 
 
 
 
 
-
-
 # Example usage:
 if __name__ == "__main__":
     density_data_path = './output/AKDE_density_grid.npy'
     hotspots = extract_hotspots(density_data_path)
     visualize_hotspots(np.load(density_data_path), hotspots)
```

### Comparing `GeoHD-0.1.5/GeoHD/visualize.py` & `GeoHD-0.1.6/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.5/GeoHD/zone.py` & `GeoHD-0.1.6/GeoHD/zone.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.5/LICENSE` & `GeoHD-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.5/README.md` & `GeoHD-0.1.6/README.md`

 * *Files identical despite different names*

