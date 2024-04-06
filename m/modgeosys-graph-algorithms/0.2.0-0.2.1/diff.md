# Comparing `tmp/modgeosys_graph_algorithms-0.2.0.tar.gz` & `tmp/modgeosys_graph_algorithms-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.2.0.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.2.1.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.2.0.tar` & `modgeosys_graph_algorithms-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3535 2024-04-06 17:32:32.989368 modgeosys_graph_algorithms-0.2.0/README.md
--rw-r--r--   0        0        0      489 2024-04-06 19:06:02.327222 modgeosys_graph_algorithms-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.2.0/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     3088 2024-04-06 18:54:45.417423 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     4729 2024-04-06 18:49:38.140617 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     1529 2024-04-06 18:55:42.785567 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     7194 2024-04-06 19:01:38.862501 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     2955 2024-04-06 18:58:26.381989 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3165 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.2.1/README.md
+-rw-r--r--   0        0        0      489 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.2.1/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     3088 2024-04-06 18:54:45.417423 modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     5816 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     1944 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     7683 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0    23944 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     3698 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.2.1/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.2.0/README.md` & `modgeosys_graph_algorithms-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: modgeosys-graph-algorithms
+Version: 0.2.1
+Summary: 
+Author: Kevin Weller
+Author-email: klweller@icloud.com
+Requires-Python: >=3.12,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: heapdict (>=1.0.1,<2.0.0)
+Requires-Dist: numpy (>=1.26.3,<2.0.0)
+Description-Content-Type: text/markdown
+
 # modgeosys-graph-algorithms: Graph Algorithms
 
 A repository for [hopefully] clean, readable, and easily-called implementations of some navigation,
 path planning, and obstacle avoidance algorithms I will be using in the near future, written in modern
 Python and/or Rust with Python bindings. I'll be adding more algorithm implementations over time.
 
 ## Algorithms: Currently implemented + planned
@@ -19,30 +32,24 @@
 
 ### A\*
 
 ```python
 import pickle
 from pprint import pprint
 
-from modgeosys.graph.types import Node, Edge, Graph
+from modgeosys.graph.types import Graph
 from modgeosys.graph.distance import manhattan_distance, euclidean_distance
 from modgeosys.graph.a_star import a_star
 
 # Define a toy graph.
-nodes = [Node(coordinates=(0.0, 0.0)),
-         Node(coordinates=(0.0, 2.0)),
-         Node(coordinates=(1.0, 0.0)),
-         Node(coordinates=(2.0, 1.0)),
-         Node(coordinates=(2.0, 3.0))]
-edges = (Edge(weight=2.0, node_indices=frozenset((0, 1))),
-         Edge(weight=1.0, node_indices=frozenset((0, 2))),
-         Edge(weight=1.0, node_indices=frozenset((2, 3))),
-         Edge(weight=3.0, node_indices=frozenset((1, 4))),
-         Edge(weight=1.0, node_indices=frozenset((3, 4))))
-toy_graph = Graph(nodes=nodes, edges=edges)
+toy_graph = Graph.from_edge_definitions(((2, ((0.0, 0.0), (0.0, 2.0))),
+                                         (1, ((0.0, 0.0), (1.0, 0.0))),
+                                         (1, ((1.0, 0.0), (2.0, 1.0))),
+                                         (3, ((0.0, 2.0), (2.0, 3.0))),
+                                         (1, ((2.0, 1.0), (2.0, 3.0)))))
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
     larger_graph = pickle.load(pickled_sample_larger_graph_file)
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
@@ -55,36 +62,30 @@
 ```
 
 ### Prim's algorithm
 
 ```python
 import pickle
 
-from modgeosys.graph.types import Node, Edge, Graph
+from modgeosys.graph.types import Graph
 from modgeosys.graph.prim import prim
 
 # Define a toy graph.
-nodes = [Node(coordinates=(0.0, 0.0)),
-         Node(coordinates=(0.0, 2.0)),
-         Node(coordinates=(1.0, 0.0)),
-         Node(coordinates=(2.0, 1.0)),
-         Node(coordinates=(2.0, 3.0))]
-edges = (Edge(weight=2.0, node_indices=frozenset((0, 1))),
-         Edge(weight=1.0, node_indices=frozenset((0, 2))),
-         Edge(weight=1.0, node_indices=frozenset((2, 3))),
-         Edge(weight=3.0, node_indices=frozenset((1, 4))),
-         Edge(weight=1.0, node_indices=frozenset((3, 4))))
-toy_graph = Graph(nodes=nodes, edges=edges)
+toy_graph = Graph.from_edge_definitions(((2, ((0.0, 0.0), (0.0, 2.0))),
+                                         (1, ((0.0, 0.0), (1.0, 0.0))),
+                                         (1, ((1.0, 0.0), (2.0, 1.0))),
+                                         (3, ((0.0, 2.0), (2.0, 3.0))),
+                                         (1, ((2.0, 1.0), (2.0, 3.0)))))
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
     larger_graph = pickle.load(pickled_sample_larger_graph_file)
 
 # Call the Prim function.
 toy_minimum_spanning_tree = prim(graph=toy_graph, start_node_index=0)
 print('Toy Prim Minimum Spanning Tree:')
 print(toy_minimum_spanning_tree)
 print()
 larger_minimum_spanning_tree = prim(graph=larger_graph, start_node_index=0)
 print('Prim Minimum Spanning Tree:')
 print(larger_minimum_spanning_tree)
-```
+```
```

### Comparing `modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.2.1/src/modgeosys/graph/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 NDType = TypeVar("NDType", bound=np.generic)
 Vector = Annotated[npt.NDArray[NDType], Literal["N", 1]]
 
 type NodeSequence = Sequence[Node]
 type EdgeSequence = Sequence[Edge]
+type EdgeDefinitionSequence = Sequence[tuple[int | float, tuple[tuple, tuple]]]
 type AdjacencyMap = Mapping[Node, Sequence[Edge]]
 type HeuristicDistanceCallable = Callable[[Node, Node], int | float]
 type ValidEdgeCallable = Callable[[Edge], bool]
 
 
 @dataclass
 class Node:
@@ -99,14 +100,39 @@
 
 
 class Graph:
     """A graph."""
     nodes: NodeSequence = field(default_factory=list)
     edges: EdgeSequence = field(default_factory=tuple)
 
+    @classmethod
+    def from_edge_definitions(cls, edge_definitions: EdgeDefinitionSequence):
+        coordinates_of_all_nodes = []
+
+        for edge_definition in edge_definitions:
+            for edge_node_coordinates in edge_definition[1]:
+                if edge_node_coordinates not in coordinates_of_all_nodes:
+                    coordinates_of_all_nodes.append(edge_node_coordinates)
+
+        nodes = dict()
+        edges = []
+
+        for edge_definition in edge_definitions:
+            indices = []
+            for edge_node_coordinates in edge_definition[1]:
+                index = coordinates_of_all_nodes.index(edge_node_coordinates)
+                indices.append(index)
+                nodes[index] = Node(coordinates=edge_node_coordinates)
+            node_indices = frozenset(indices)
+            edge = Edge(weight=edge_definition[0], node_indices=node_indices)
+            edges.append(edge)
+
+        nodes = [nodes[index] for index in sorted(nodes)]
+        return cls(nodes, edges)
+
     def __init__(self, nodes: NodeSequence, edges: EdgeSequence):
         """Initialize a graph."""
         self.nodes = copy(nodes)
         self.edges = tuple(copy(edge) for edge in edges)
 
     def __repr__(self):
         return f'Graph(nodes={self.nodes}, edges={self.edges})'
```

### Comparing `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,14 +34,23 @@
 
 @pytest.fixture
 def valid_graph2(valid_nodes, valid_edges2):
     return Graph(valid_nodes, valid_edges2)
 
 
 @pytest.fixture
+def valid_graph_from_edge_definitions():
+    return Graph.from_edge_definitions(((2, ((0.0, 0.0), (0.0, 2.0))),
+                                        (1, ((0.0, 0.0), (1.0, 0.0))),
+                                        (1, ((1.0, 0.0), (2.0, 1.0))),
+                                        (3, ((0.0, 2.0), (2.0, 3.0))),
+                                        (1, ((2.0, 1.0), (2.0, 3.0)))))
+
+
+@pytest.fixture
 def valid_graph_larger():
     with open('data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
         return pickle.load(pickled_sample_larger_graph_file)
 
 
 @pytest.fixture
 def valid_graph_larger_with_string_edge_weights():
```

### Comparing `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/test_a_star.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,22 @@
     result = a_star(graph=valid_graph1, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
 
     assert len(result) == 2
     assert result == [Hop(Edge(weight=2.0, node_indices=frozenset({0, 1})), cached_f=5.0, g=2.0, h=3.0),
                       Hop(Edge(weight=3.0, node_indices=frozenset({1, 4})), cached_f=5.0, g=5.0, h=0.0)]
 
 
+def test_a_star_find_shortest_path_manhattan_graph_from_edge_definitions(valid_graph_from_edge_definitions):
+    result = a_star(graph=valid_graph_from_edge_definitions, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+
+    assert len(result) == 2
+    assert result == [Hop(Edge(weight=2.0, node_indices=frozenset({0, 1})), cached_f=5.0, g=2.0, h=3.0),
+                      Hop(Edge(weight=3.0, node_indices=frozenset({1, 4})), cached_f=5.0, g=5.0, h=0.0)]
+
+
 def test_a_star_finds_shortest_path_manhattan_graph2(valid_graph2):
     result = a_star(graph=valid_graph2, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
 
     assert len(result) == 3
     assert result == [Hop(Edge(weight=1.0, node_indices=frozenset({0, 2})), cached_f=5.0, g=1.0, h=4.0),
                       Hop(Edge(weight=1.0, node_indices=frozenset({2, 3})), cached_f=4.0, g=2.0, h=2.0),
                       Hop(Edge(weight=1.0, node_indices=frozenset({3, 4})), cached_f=3.0, g=3.0, h=0.0)]
```

### Comparing `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.2.1/tests/modgeosys/graph/test_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,14 +55,22 @@
 
 
 def test_graph_creation(valid_nodes, valid_edges1, valid_graph1):
     assert valid_graph1.nodes == valid_nodes
     assert valid_graph1.edges == valid_edges1
 
 
+def test_graph_creation_from_edge_definitions(valid_graph_from_edge_definitions):
+    assert valid_graph_from_edge_definitions.nodes == [Node((0.0, 0.0)), Node((0.0, 2.0)), Node((1.0, 0.0)), Node((2.0, 1.0)), Node((2.0, 3.0))]
+    assert valid_graph_from_edge_definitions.edges == (Edge(weight=2, node_indices=frozenset((0, 1))),
+                                                       Edge(weight=1, node_indices=frozenset((0, 2))),
+                                                       Edge(weight=1, node_indices=frozenset((2, 3))),
+                                                       Edge(weight=3, node_indices=frozenset((1, 4))),
+                                                       Edge(weight=1, node_indices=frozenset((3, 4))))
+
 def test_graph_adjacency_map(valid_graph1):
     adjacency_map = valid_graph1.adjacency_map()
     assert adjacency_map == {Node((0.0, 0.0)): [Edge(weight=1, node_indices=frozenset((0, 2))), Edge(weight=2, node_indices=frozenset((0, 1)))],
                              Node((0.0, 2.0)): [Edge(weight=2, node_indices=frozenset((0, 1))), Edge(weight=3, node_indices=frozenset((1, 4)))],
                              Node((1.0, 0.0)): [Edge(weight=1, node_indices=frozenset((0, 2))), Edge(weight=1, node_indices=frozenset((2, 3)))],
                              Node((2.0, 1.0)): [Edge(weight=1, node_indices=frozenset((2, 3))), Edge(weight=1, node_indices=frozenset((3, 4)))],
                              Node((2.0, 3.0)): [Edge(weight=1, node_indices=frozenset((3, 4))), Edge(weight=3, node_indices=frozenset((1, 4)))]}
```

