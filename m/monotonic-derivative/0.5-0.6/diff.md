# Comparing `tmp/monotonic derivative-0.5.tar.gz` & `tmp/monotonic derivative-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic derivative-0.5.tar", last modified: Mon May  8 08:55:28 2023, max compression
+gzip compressed data, was "monotonic derivative-0.6.tar", last modified: Thu May 25 11:00:07 2023, max compression
```

## Comparing `monotonic derivative-0.5.tar` & `monotonic derivative-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:55:28.809052 monotonic derivative-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 08:55:18.000000 monotonic derivative-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-08 08:55:28.809052 monotonic derivative-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-08 08:55:18.000000 monotonic derivative-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:55:28.809052 monotonic derivative-0.5/monotonic_derivative/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 08:55:18.000000 monotonic derivative-0.5/monotonic_derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:55:18.000000 monotonic derivative-0.5/monotonic_derivative/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-08 08:55:18.000000 monotonic derivative-0.5/monotonic_derivative/curve_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 08:55:18.000000 monotonic derivative-0.5/monotonic_derivative/monotonic_derivative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:55:28.809052 monotonic derivative-0.5/monotonic_derivative.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 08:55:28.000000 monotonic derivative-0.5/monotonic_derivative.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:55:28.809052 monotonic derivative-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 08:55:18.000000 monotonic derivative-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:55:28.809052 monotonic derivative-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-08 08:55:18.000000 monotonic derivative-0.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:00:07.220100 monotonic derivative-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 10:59:52.000000 monotonic derivative-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-25 11:00:07.220100 monotonic derivative-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-25 10:59:52.000000 monotonic derivative-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:00:07.220100 monotonic derivative-0.6/monotonic_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 10:59:52.000000 monotonic derivative-0.6/monotonic_derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 10:59:52.000000 monotonic derivative-0.6/monotonic_derivative/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-25 10:59:52.000000 monotonic derivative-0.6/monotonic_derivative/curve_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-25 10:59:52.000000 monotonic derivative-0.6/monotonic_derivative/monotonic_derivative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:00:07.220100 monotonic derivative-0.6/monotonic_derivative.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 11:00:07.000000 monotonic derivative-0.6/monotonic_derivative.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:00:07.220100 monotonic derivative-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-25 10:59:52.000000 monotonic derivative-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:00:07.220100 monotonic derivative-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-25 10:59:52.000000 monotonic derivative-0.6/tests/test.py
```

### Comparing `monotonic derivative-0.5/LICENSE` & `monotonic derivative-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.5/PKG-INFO` & `monotonic derivative-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic derivative
-Version: 0.5
+Version: 0.6
 Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
 Home-page: https://github.com/A-Wpro/monotonic_derivative
 Author: Adam Wecker
 Author-email: adam.wecker0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `monotonic derivative-0.5/README.md` & `monotonic derivative-0.6/README.md`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.5/monotonic_derivative/curve_smoothing.py` & `monotonic derivative-0.6/monotonic_derivative/curve_smoothing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,157 +1,167 @@
-
 import numpy as np
 from scipy.interpolate import CubicSpline
 from scipy.optimize import minimize
 import matplotlib.pyplot as plt
 from io import BytesIO
 import imageio
 import os
 
+
 def initialize_population(population_size, num_points):
     """
     Initializes the population with random individuals.
-    
+
     Args:
         population_size (int): Number of individuals in the population.
         num_points (int): Number of points in each individual.
-    
+
     Returns:
         numpy.ndarray: Initial population as a 2D array.
     """
-    return np.random.randint(0, 100, size=(population_size, num_points))
+    return np.random.uniform(0, 100, size=(population_size, num_points))
+
 
 def calculate_fitness(individual, points, alpha):
     """
     Calculates the fitness of an individual based on the total deviation from the original points
     and the abrupt changes in the smoothed curve.
-    
+
     Args:
         individual (numpy.ndarray): The individual for which the fitness is calculated.
         points (numpy.ndarray): The original points.
         alpha (float): Weighting factor for the total deviation (range: 0 to 1).
-    
+
     Returns:
         float: Fitness value for the individual.
     """
     total_deviation = np.sum(np.abs(individual - points))
     abrupt_changes = np.sum(np.abs(np.diff(np.diff(individual))))
-    return - (alpha * total_deviation + (1 - alpha) * abrupt_changes)
+    return -(alpha * total_deviation + (1 - alpha) * abrupt_changes)
+
 
 def selection(population, points, alpha):
     """
     Selects the top two individuals from the population based on their fitness.
-    
+
     Args:
         population (numpy.ndarray): The current population.
         points (numpy.ndarray): The original points.
         alpha (float): Weighting factor for the total deviation (range: 0 to 1).
-    
+
     Returns:
         numpy.ndarray: The top two individuals from the population.
     """
-    fitness = [calculate_fitness(individual, points, alpha) for individual in population]
+    fitness = [
+        calculate_fitness(individual, points, alpha) for individual in population
+    ]
     indices = np.argsort(fitness)[-2:]
     return population[indices]
 
+
 def crossover(parent1, parent2):
     """
     Performs crossover between two parents to create two offspring.
-    
+
     Args:
         parent1 (numpy.ndarray): The first parent.
         parent2 (numpy.ndarray): The second parent.
-    
+
     Returns:
         tuple: Two offspring as numpy arrays.
     """
     crossover_point = np.random.randint(1, len(parent1) - 1)
     child1 = np.concatenate((parent1[:crossover_point], parent2[crossover_point:]))
     child2 = np.concatenate((parent2[:crossover_point], parent1[crossover_point:]))
     return child1, child2
 
+
 def mutation(individual, mutation_rate):
     """
     Mutates an individual by changing the value of a point with a certain probability.
-    
+
     Args:
         individual (numpy.ndarray): The individual to be mutated.
         mutation_rate (float): The probability of mutating a point (range: 0 to 1).
-    
+
     Returns:
         numpy.ndarray: The mutated individual.
     """
     for i in range(len(individual)):
         if np.random.random() < mutation_rate:
-            individual[i] = np.random.randint(0, 100)
+            individual[i] = np.random.uniform(0, 100)
     return individual
 
 
-def curve_smoothing(points, population_size=100, num_generations=1000, mutation_rate=0.1, alpha=0.5, save_plots=False, output_folder="output"):
+def curve_smoothing(
+    points,
+    population_size=100,
+    num_generations=1000,
+    mutation_rate=0.1,
+    alpha=0.5,
+    save_plots=False,
+    output_folder="output",
+):
     """
     Apply a genetic algorithm to smooth a curve represented by a sequence of points.
-    
+
     Parameters:
     points (numpy.array): An array of Y-coordinates representing the original curve.
     population_size (int, optional): The number of individuals in the population. Default is 100.
     num_generations (int, optional): The number of generations to run the algorithm. Default is 1000.
     mutation_rate (float, optional): The probability of a mutation occurring during reproduction. Default is 0.1.
     alpha (float, optional): The trade-off between smoothness and similarity to the original curve. Default is 0.5.
     save_plots (bool, optional): Whether to save the progress of the algorithm as a GIF. Default is False.
     output_folder (str, optional): The folder to save the progress GIF if `save_plots` is True. Default is "output".
-    
+
     Returns:
     numpy.array: The best individual (smoothed curve) found by the genetic algorithm.
     """
     # Create the output folder if it doesn't exist and save_plots is True
     if save_plots:
         if not os.path.exists(output_folder):
             os.makedirs(output_folder)
-    
+
     # Initialize the population
     population = initialize_population(population_size, len(points))
     images = []
-    
+
     # Iterate through the generations
     for generation in range(num_generations):
         # Select the parents based on their fitness
         parents = selection(population, points, alpha)
         children = []
-        
+
         # Create the next generation by crossover and mutation
         for i in range(int(population_size / 2)):
             child1, child2 = crossover(parents[0], parents[1])
             children.append(mutation(child1, mutation_rate))
             children.append(mutation(child2, mutation_rate))
-        
+
         # Update the population
         population = np.array(children)
-        
+
         # Save the progress as images for the GIF
         if save_plots and generation % 50 == 0:
             best_individual = selection(population, points, alpha)[0]
-            plt.plot(points, 'bo-', label='Original curve')
-            plt.plot(best_individual, 'ro-', label='Smoothed curve')
+            plt.plot(points, "bo-", label="Original curve")
+            plt.plot(best_individual, "ro-", label="Smoothed curve")
             plt.legend()
-            
+
             if generation == num_generations - 1:
-                plt.title('Final curve', fontsize=24, alpha=0.2)
-            
+                plt.title("Final curve", fontsize=24, alpha=0.2)
+
             buf = BytesIO()
-            plt.savefig(buf, format='png')
+            plt.savefig(buf, format="png")
             buf.seek(0)
             images.append(imageio.imread(buf))
             plt.clf()
-    
+
     # Select the best individual from the final population
     best_individual = selection(population, points, alpha)[0]
-    
+
     # Save the progress as a GIF
     if save_plots:
         gif_filename = os.path.join(output_folder, "progress.gif")
         imageio.mimsave(gif_filename, images[:-1] + [images[-1]] * 15, duration=0.2)
-    
-    return best_individual
-
-
-
 
+    return best_individual
```

### Comparing `monotonic derivative-0.5/monotonic_derivative.egg-info/PKG-INFO` & `monotonic derivative-0.6/monotonic_derivative.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-derivative
-Version: 0.5
+Version: 0.6
 Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
 Home-page: https://github.com/A-Wpro/monotonic_derivative
 Author: Adam Wecker
 Author-email: adam.wecker0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `monotonic derivative-0.5/setup.py` & `monotonic derivative-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="monotonic derivative",
-    version="0.5",
+    version="0.6",
     description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. There is also a genetic base curve smoothing tool with several paramter to suit your needs, This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Adam Wecker",
     author_email="adam.wecker0@gmail.com",
     url="https://github.com/A-Wpro/monotonic_derivative",
     packages=["monotonic_derivative"],
```

### Comparing `monotonic derivative-0.5/tests/test.py` & `monotonic derivative-0.6/tests/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 def test_invalid_degree():
     x = np.array([0, 1, 2, 3, 4, 5])
     y = np.array([100, 55, 53, 40, 35, 5])
 
     with pytest.raises(ValueError):
-        ensure_monotonic_derivative(x, y, degree=5)
+        ensure_monotonic_derivative(x, y, degree=-1)
 
 
 def test_negative_derivative():
     x = np.array([0, 1, 2, 3, 4, 5])
     y = np.array([100, 55, 53, 40, 35, 5])
     d = 2
     modified_y = ensure_monotonic_derivative(
@@ -41,22 +41,14 @@
     x = np.array([0, 1, 2, 3, 4, 5])
     y = np.array([100, 55, 53, 40, 35])
 
     with pytest.raises(ValueError):
         ensure_monotonic_derivative(x, y)
 
 
-def test_same_lengths():
-    x = np.array([0, 1, 2, 3, 4, 5])
-    y = np.array([100, 55, 53, 40, 35, 5])
-
-    with pytest.raises(ValueError):
-        ensure_monotonic_derivative(x, y, degree=6)
-
-
 ### Test for curve smoothing with genetic algo
 from monotonic_derivative.curve_smoothing import (
     initialize_population,
     selection,
     crossover,
     mutation,
     calculate_fitness,
```

