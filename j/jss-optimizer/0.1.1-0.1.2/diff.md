# Comparing `tmp/jss_optimizer-0.1.1.tar.gz` & `tmp/jss_optimizer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jss_optimizer-0.1.1.tar", last modified: Wed Apr  3 13:54:20 2024, max compression
+gzip compressed data, was "jss_optimizer-0.1.2.tar", last modified: Sun Apr  7 06:56:28 2024, max compression
```

## Comparing `jss_optimizer-0.1.1.tar` & `jss_optimizer-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:54:20.691076 jss_optimizer-0.1.1/
--rw-rw-rw-   0        0        0     2530 2024-04-03 13:54:20.691076 jss_optimizer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1955 2024-04-03 13:45:18.000000 jss_optimizer-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 13:54:20.671907 jss_optimizer-0.1.1/jss_optimizer/
--rw-rw-rw-   0        0        0       50 2024-04-03 13:36:06.000000 jss_optimizer-0.1.1/jss_optimizer/__init__.py
--rw-rw-rw-   0        0        0     4884 2024-04-03 13:34:45.000000 jss_optimizer-0.1.1/jss_optimizer/jss_optimizer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:54:20.691076 jss_optimizer-0.1.1/jss_optimizer.egg-info/
--rw-rw-rw-   0        0        0     2530 2024-04-03 13:54:19.000000 jss_optimizer-0.1.1/jss_optimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-04-03 13:54:20.000000 jss_optimizer-0.1.1/jss_optimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:54:19.000000 jss_optimizer-0.1.1/jss_optimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 13:54:19.000000 jss_optimizer-0.1.1/jss_optimizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-03 13:54:19.000000 jss_optimizer-0.1.1/jss_optimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 13:54:20.691076 jss_optimizer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1216 2024-04-03 13:51:25.000000 jss_optimizer-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:56:28.531479 jss_optimizer-0.1.2/
+-rw-rw-rw-   0        0        0     2937 2024-04-07 06:56:28.530475 jss_optimizer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2455 2024-04-07 06:51:50.000000 jss_optimizer-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 06:56:28.487866 jss_optimizer-0.1.2/jss_optimizer/
+-rw-rw-rw-   0        0        0       50 2024-04-03 13:36:06.000000 jss_optimizer-0.1.2/jss_optimizer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:56:28.528475 jss_optimizer-0.1.2/jss_optimizer/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-04-07 06:54:29.000000 jss_optimizer-0.1.2/jss_optimizer/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4628 2024-04-07 06:54:29.000000 jss_optimizer-0.1.2/jss_optimizer/__pycache__/jss_optimizer.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5036 2024-04-07 06:40:06.000000 jss_optimizer-0.1.2/jss_optimizer/jss_optimizer.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:56:28.523589 jss_optimizer-0.1.2/jss_optimizer.egg-info/
+-rw-rw-rw-   0        0        0     2937 2024-04-07 06:56:27.000000 jss_optimizer-0.1.2/jss_optimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-04-07 06:56:28.000000 jss_optimizer-0.1.2/jss_optimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 06:56:27.000000 jss_optimizer-0.1.2/jss_optimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 06:56:27.000000 jss_optimizer-0.1.2/jss_optimizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-07 06:56:27.000000 jss_optimizer-0.1.2/jss_optimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 06:56:28.532475 jss_optimizer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-04-07 06:53:57.000000 jss_optimizer-0.1.2/setup.py
```

### Comparing `jss_optimizer-0.1.1/PKG-INFO` & `jss_optimizer-0.1.2/jss_optimizer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
-Name: jss_optimizer
-Version: 0.1.1
+Name: jss-optimizer
+Version: 0.1.2
 Author: Jegadit S Saravanan
 Author-email: jegaditssaravanan@yahoo.com
 Keywords: machine-learning,parameter optimization,genetic algorithm,simulated annealing
-Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 
 
 ### Based on the paper: J. S. Saravanan and A. Mahadevan, "AI based parameter estimation of ML model using Hybrid of Genetic Algorithm and Simulated Annealing," 2023 14th International Conference on Computing Communication and Networking Technologies (ICCCNT), Delhi, India, 2023, pp. 1-5, doi: 10.1109/ICCCNT56998.2023.10308077. 
 
@@ -27,38 +25,45 @@
 pip install jss_optimizer
 
 ```
 
 # Usage Example
 
 ```python
-from jss_optimizer.optimizer import HyperparameterOptimizer
+from jss_optimizer.jss_optimizer import HyperparameterOptimizer
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 
 # Load dataset
 df = pd.read_csv('dataset/heart_v2.csv')
 X = df.drop('heart disease', axis=1)
 y = df['heart disease']
-X_train, _, y_train, _ = train_test_split(X, y, train_size=0.7, random_state=42)
+X_train, X_test, y_train, y_test = train_test_split(X, y, train_size=0.7, random_state=42)
 
 # Define model and parameters
 model = RandomForestClassifier
 params = ['max_depth', 'min_samples_leaf', 'n_estimators']
 
 # Create an instance of HyperparameterOptimizer
 optimizer = HyperparameterOptimizer(model, params)
 
 # Optimize hyperparameters using genetic algorithm
-best_solution_genetic = optimizer.optimize(X_train, y_train)
-# print('Best solution found by genetic algorithm:', best_solution_genetic)
+best_solution_genetic = optimizer.optimize(X_train, y_train, X_test, y_test)
+print('Best solution found by genetic algorithm:', best_solution_genetic)
 
-# Perform simulated annealing
-best_solution_simulated_annealing = optimizer.simulate_annealing(best_solution_genetic, X_train, y_train)
+# NOTE
+# Most of the time, genetic algorithm itself could give an optimal solution. But it could also get caught in a local optima. 
+# To aviod such senarios, further optimization with simulated annealing is recommended.
+# Use the solution that you see fit is optimal.  
+
+# Perform simulated annealing 
+best_solution_simulated_annealing = optimizer.simulate_annealing(best_solution_genetic, X_train, y_train, X_test, y_test)
 print('Best solution found by GA-SA hybrid optimization algorithm:', best_solution_simulated_annealing)
 
 ```
 
-## For now, this will work only with Random Forest Classifier on any dataset. 
+## works are under progress to extend it to work with every data and model in any given senario
 
-## works are under progress to extend it to work on other models as well
+## Version Logs
+### version: 0.1.1 - This will work only with Random Forest Classifier on any dataset. 
+### version: 0.1.2 - Same as version: 0.1.1. Added improvements & support for train-test spitting with proper score metrics
```

### Comparing `jss_optimizer-0.1.1/README.md` & `jss_optimizer-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,38 +12,45 @@
 pip install jss_optimizer
 
 ```
 
 # Usage Example
 
 ```python
-from jss_optimizer.optimizer import HyperparameterOptimizer
+from jss_optimizer.jss_optimizer import HyperparameterOptimizer
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 
 # Load dataset
 df = pd.read_csv('dataset/heart_v2.csv')
 X = df.drop('heart disease', axis=1)
 y = df['heart disease']
-X_train, _, y_train, _ = train_test_split(X, y, train_size=0.7, random_state=42)
+X_train, X_test, y_train, y_test = train_test_split(X, y, train_size=0.7, random_state=42)
 
 # Define model and parameters
 model = RandomForestClassifier
 params = ['max_depth', 'min_samples_leaf', 'n_estimators']
 
 # Create an instance of HyperparameterOptimizer
 optimizer = HyperparameterOptimizer(model, params)
 
 # Optimize hyperparameters using genetic algorithm
-best_solution_genetic = optimizer.optimize(X_train, y_train)
-# print('Best solution found by genetic algorithm:', best_solution_genetic)
+best_solution_genetic = optimizer.optimize(X_train, y_train, X_test, y_test)
+print('Best solution found by genetic algorithm:', best_solution_genetic)
 
-# Perform simulated annealing
-best_solution_simulated_annealing = optimizer.simulate_annealing(best_solution_genetic, X_train, y_train)
+# NOTE
+# Most of the time, genetic algorithm itself could give an optimal solution. But it could also get caught in a local optima. 
+# To aviod such senarios, further optimization with simulated annealing is recommended.
+# Use the solution that you see fit is optimal.  
+
+# Perform simulated annealing 
+best_solution_simulated_annealing = optimizer.simulate_annealing(best_solution_genetic, X_train, y_train, X_test, y_test)
 print('Best solution found by GA-SA hybrid optimization algorithm:', best_solution_simulated_annealing)
 
 ```
 
-## For now, this will work only with Random Forest Classifier on any dataset. 
+## works are under progress to extend it to work with every data and model in any given senario
 
-## works are under progress to extend it to work on other models as well
+## Version Logs
+### version: 0.1.1 - This will work only with Random Forest Classifier on any dataset. 
+### version: 0.1.2 - Same as version: 0.1.1. Added improvements & support for train-test spitting with proper score metrics
```

### Comparing `jss_optimizer-0.1.1/jss_optimizer/jss_optimizer.py` & `jss_optimizer-0.1.2/jss_optimizer/jss_optimizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 warnings.simplefilter("ignore", UserWarning)
 
 class HyperparameterOptimizer:
     def __init__(self, model, params):
         self.model = model
         self.params = params
 
-    def cal_pop_fitness(self, pop, X_train, y_train):
+    def cal_pop_fitness(self, pop, X_train, y_train, X_test, y_test):
         fitness = []
         for i in range(len(pop)):
             if pop[i][1] >= 1:
                 classifier = self.model(random_state=42, **{self.params[j]: pop[i][j] for j in range(len(pop[i]))}, oob_score=True)
                 classifier.fit(X_train, y_train)
-                fitness.append(classifier.oob_score_)
+                fitness.append(classifier.score(X_train, y_train))
             else:
                 fitness.append(0)
         return fitness
 
     def select_mating_pool(self, pop, fitness, num_parents):
         parents = np.empty((num_parents, pop.shape[1]))
         for parent_num in range(num_parents):
@@ -46,56 +46,56 @@
             gene_idx = mutations_counter - 1
             for mutation_num in range(num_mutations):
                 random_value = np.random.randint(1, 6)
                 offspring_crossover[idx, gene_idx] = offspring_crossover[idx, gene_idx] + random_value
                 gene_idx = gene_idx + mutations_counter
         return offspring_crossover
 
-    def optimize(self, X_train, y_train, sol_per_pop=5, num_parents_mating=3, num_generations=100):
+    def optimize(self, X_train, y_train, X_test, y_test, sol_per_pop=5, num_parents_mating=3, num_generations=100):
         pop_size = (sol_per_pop, len(self.params))
         new_population = np.random.randint(low=1, high=(20 - 4), size=pop_size)
 
         best_solution = None
         best_fitness = float('-inf')
         print("\n")
         for generation in tqdm(range(num_generations)):
-            fitness = self.cal_pop_fitness(new_population, X_train, y_train)
+            fitness = self.cal_pop_fitness(new_population, X_train, y_train, X_test, y_test)
             best_fitness_in_gen = max(fitness)
             if best_fitness_in_gen > best_fitness:
                 best_fitness = best_fitness_in_gen
                 best_solution = new_population[np.argmax(fitness)]
 
             parents = self.select_mating_pool(new_population, fitness, num_parents_mating)
             offspring_crossover = self.crossover(parents, offspring_size=(pop_size[0] - parents.shape[0], len(self.params)))
             offspring_mutation = self.mutation(offspring_crossover, num_mutations=2)
             new_population[0:parents.shape[0], :] = parents
             new_population[parents.shape[0]:, :] = offspring_mutation
         print("\nFinished applying genetic algorithm.")
         print("Score of the best candidates after parameter optimizing with genetic algorithm: ", best_fitness)
-        print("Appplying Simulated Annealing to optimize by escaping local optimas ... \n")
         return best_solution
 
-    def objective_function(self, combination, X_train, y_train):
+    def objective_function(self, combination, X_train, y_train, X_test, y_test):
         classifier = self.model(random_state=42, **{self.params[j]: combination[j] for j in range(len(combination))}, oob_score=True)
         classifier.fit(X_train, y_train)
-        return classifier.oob_score_
+        return classifier.score(X_test, y_test)
 
-    def simulate_annealing(self, start_solution, X_train, y_train, T=10, T_min=0.001, alpha=0.99):
+    def simulate_annealing(self, start_solution, X_train, y_train, X_test, y_test, T=10, T_min=0.001, alpha=0.99):
+        print("Appplying Simulated Annealing to optimize by escaping local optimas ... \n")
         combination = start_solution.copy()
         with tqdm(total=int((T-T_min)/alpha)) as pbar:
             while T > T_min:
                 new_combination = combination.copy()
                 i = random.randint(0, len(combination) - 1)
                 new_combination[i] = random.randint(1, 20)
-                delta_E = self.objective_function(new_combination, X_train, y_train) - self.objective_function(combination, X_train, y_train)
+                delta_E = self.objective_function(new_combination, X_train, y_train, X_test, y_test) - self.objective_function(combination, X_train, y_train, X_test, y_test)
                 if delta_E > 0:
                     combination = new_combination
                 else:
                     p = np.exp(delta_E / T)
                     if random.uniform(0, 1) < p:
                         combination = new_combination
                 T *= alpha
                 pbar.update(1)
-        print("\nScore of the best candidates after parameter optimizing with GA-SA algorithm:  ", self.objective_function(combination, X_train, y_train))
+        print("\nScore of the best candidates after parameter optimizing with GA-SA algorithm:  ", self.objective_function(combination, X_train, y_train, X_test, y_test))
         return combination
```

### Comparing `jss_optimizer-0.1.1/jss_optimizer.egg-info/PKG-INFO` & `jss_optimizer-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
-Name: jss-optimizer
-Version: 0.1.1
+Name: jss_optimizer
+Version: 0.1.2
 Author: Jegadit S Saravanan
 Author-email: jegaditssaravanan@yahoo.com
 Keywords: machine-learning,parameter optimization,genetic algorithm,simulated annealing
-Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 
 
 ### Based on the paper: J. S. Saravanan and A. Mahadevan, "AI based parameter estimation of ML model using Hybrid of Genetic Algorithm and Simulated Annealing," 2023 14th International Conference on Computing Communication and Networking Technologies (ICCCNT), Delhi, India, 2023, pp. 1-5, doi: 10.1109/ICCCNT56998.2023.10308077. 
 
@@ -27,38 +25,45 @@
 pip install jss_optimizer
 
 ```
 
 # Usage Example
 
 ```python
-from jss_optimizer.optimizer import HyperparameterOptimizer
+from jss_optimizer.jss_optimizer import HyperparameterOptimizer
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 
 # Load dataset
 df = pd.read_csv('dataset/heart_v2.csv')
 X = df.drop('heart disease', axis=1)
 y = df['heart disease']
-X_train, _, y_train, _ = train_test_split(X, y, train_size=0.7, random_state=42)
+X_train, X_test, y_train, y_test = train_test_split(X, y, train_size=0.7, random_state=42)
 
 # Define model and parameters
 model = RandomForestClassifier
 params = ['max_depth', 'min_samples_leaf', 'n_estimators']
 
 # Create an instance of HyperparameterOptimizer
 optimizer = HyperparameterOptimizer(model, params)
 
 # Optimize hyperparameters using genetic algorithm
-best_solution_genetic = optimizer.optimize(X_train, y_train)
-# print('Best solution found by genetic algorithm:', best_solution_genetic)
+best_solution_genetic = optimizer.optimize(X_train, y_train, X_test, y_test)
+print('Best solution found by genetic algorithm:', best_solution_genetic)
 
-# Perform simulated annealing
-best_solution_simulated_annealing = optimizer.simulate_annealing(best_solution_genetic, X_train, y_train)
+# NOTE
+# Most of the time, genetic algorithm itself could give an optimal solution. But it could also get caught in a local optima. 
+# To aviod such senarios, further optimization with simulated annealing is recommended.
+# Use the solution that you see fit is optimal.  
+
+# Perform simulated annealing 
+best_solution_simulated_annealing = optimizer.simulate_annealing(best_solution_genetic, X_train, y_train, X_test, y_test)
 print('Best solution found by GA-SA hybrid optimization algorithm:', best_solution_simulated_annealing)
 
 ```
 
-## For now, this will work only with Random Forest Classifier on any dataset. 
+## works are under progress to extend it to work with every data and model in any given senario
 
-## works are under progress to extend it to work on other models as well
+## Version Logs
+### version: 0.1.1 - This will work only with Random Forest Classifier on any dataset. 
+### version: 0.1.2 - Same as version: 0.1.1. Added improvements & support for train-test spitting with proper score metrics
```

### Comparing `jss_optimizer-0.1.1/setup.py` & `jss_optimizer-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 with open("README.md") as f:
     LONG_DESCRIPTION = "\n" + f.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'AI based optimized parameter estimation for ML models.'
 # LONG_DESCRIPTION = 'AI based optimized parameter estimation of ML models using Hybrid of Genetic Algorithm and Simulated Annealing. based on the paper by Jegadit S Saravanan @ https://ieeexplore.ieee.org/document/10308077'
 
 
 setup(
     name='jss_optimizer',
     version=VERSION,
@@ -17,15 +17,13 @@
     author_email='jegaditssaravanan@yahoo.com',
     # description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     keywords=['machine-learning', 'parameter optimization', 'genetic algorithm', 'simulated annealing'],
     classifiers=[
-        "Development Status :: 1 - Planning",
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
-        'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
 )
```

