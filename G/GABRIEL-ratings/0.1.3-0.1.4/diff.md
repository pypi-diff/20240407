# Comparing `tmp/GABRIEL-ratings-0.1.3.tar.gz` & `tmp/GABRIEL-ratings-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GABRIEL-ratings-0.1.3.tar", last modified: Sat Apr  6 20:09:52 2024, max compression
+gzip compressed data, was "dist/GABRIEL-ratings-0.1.4.tar", last modified: Sun Apr  7 02:16:06 2024, max compression
```

## Comparing `GABRIEL-ratings-0.1.3.tar` & `GABRIEL-ratings-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-06 20:09:52.250261 GABRIEL-ratings-0.1.3/
-drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-06 20:09:52.248212 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/
--rw-r--r--   0 elliottmokski   (501) staff       (20)     7037 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/PKG-INFO
--rw-r--r--   0 elliottmokski   (501) staff       (20)      434 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/SOURCES.txt
--rw-r--r--   0 elliottmokski   (501) staff       (20)        1 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/dependency_links.txt
--rw-r--r--   0 elliottmokski   (501) staff       (20)       70 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/requires.txt
--rw-r--r--   0 elliottmokski   (501) staff       (20)        8 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/top_level.txt
--rw-r--r--   0 elliottmokski   (501) staff       (20)       41 2024-03-22 11:53:15.000000 GABRIEL-ratings-0.1.3/MANIFEST.in
--rw-r--r--   0 elliottmokski   (501) staff       (20)     7037 2024-04-06 20:09:52.250113 GABRIEL-ratings-0.1.3/PKG-INFO
--rw-r--r--   0 elliottmokski   (501) staff       (20)     5858 2024-04-06 20:09:14.000000 GABRIEL-ratings-0.1.3/README.md
-drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-06 20:09:52.249711 GABRIEL-ratings-0.1.3/gabriel/
-drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-06 20:09:52.249942 GABRIEL-ratings-0.1.3/gabriel/Prompts/
--rw-r--r--   0 elliottmokski   (501) staff       (20)        0 2024-03-22 12:02:02.000000 GABRIEL-ratings-0.1.3/gabriel/Prompts/__init__.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)        0 2024-03-22 10:50:50.000000 GABRIEL-ratings-0.1.3/gabriel/__init__.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     7894 2024-04-06 20:06:07.000000 GABRIEL-ratings-0.1.3/gabriel/archangel.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     6899 2024-04-06 19:56:15.000000 GABRIEL-ratings-0.1.3/gabriel/combined_assistant.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     2292 2024-04-06 19:55:40.000000 GABRIEL-ratings-0.1.3/gabriel/decorators.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     7178 2024-04-06 19:51:15.000000 GABRIEL-ratings-0.1.3/gabriel/foundational_functions.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     5206 2024-04-06 19:57:30.000000 GABRIEL-ratings-0.1.3/gabriel/openai_api_calls.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     1049 2024-04-06 19:51:29.000000 GABRIEL-ratings-0.1.3/gabriel/prompt_wrapping.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)       38 2024-04-06 20:09:52.250308 GABRIEL-ratings-0.1.3/setup.cfg
--rw-r--r--   0 elliottmokski   (501) staff       (20)      915 2024-04-06 20:03:15.000000 GABRIEL-ratings-0.1.3/setup.py
+drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-07 02:16:06.148609 GABRIEL-ratings-0.1.4/
+drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-07 02:16:06.146645 GABRIEL-ratings-0.1.4/GABRIEL_ratings.egg-info/
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     6959 2024-04-07 02:16:06.000000 GABRIEL-ratings-0.1.4/GABRIEL_ratings.egg-info/PKG-INFO
+-rw-r--r--   0 elliottmokski   (501) staff       (20)      434 2024-04-07 02:16:06.000000 GABRIEL-ratings-0.1.4/GABRIEL_ratings.egg-info/SOURCES.txt
+-rw-r--r--   0 elliottmokski   (501) staff       (20)        1 2024-04-07 02:16:06.000000 GABRIEL-ratings-0.1.4/GABRIEL_ratings.egg-info/dependency_links.txt
+-rw-r--r--   0 elliottmokski   (501) staff       (20)       70 2024-04-07 02:16:06.000000 GABRIEL-ratings-0.1.4/GABRIEL_ratings.egg-info/requires.txt
+-rw-r--r--   0 elliottmokski   (501) staff       (20)        8 2024-04-07 02:16:06.000000 GABRIEL-ratings-0.1.4/GABRIEL_ratings.egg-info/top_level.txt
+-rw-r--r--   0 elliottmokski   (501) staff       (20)       41 2024-03-22 11:53:15.000000 GABRIEL-ratings-0.1.4/MANIFEST.in
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     6959 2024-04-07 02:16:06.148441 GABRIEL-ratings-0.1.4/PKG-INFO
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     5772 2024-04-06 21:03:45.000000 GABRIEL-ratings-0.1.4/README.md
+drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-07 02:16:06.148009 GABRIEL-ratings-0.1.4/gabriel/
+drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-07 02:16:06.148242 GABRIEL-ratings-0.1.4/gabriel/Prompts/
+-rw-r--r--   0 elliottmokski   (501) staff       (20)        0 2024-03-22 12:02:02.000000 GABRIEL-ratings-0.1.4/gabriel/Prompts/__init__.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)        0 2024-03-22 10:50:50.000000 GABRIEL-ratings-0.1.4/gabriel/__init__.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     8089 2024-04-07 02:15:55.000000 GABRIEL-ratings-0.1.4/gabriel/archangel.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     6899 2024-04-07 01:57:50.000000 GABRIEL-ratings-0.1.4/gabriel/combined_assistant.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     2292 2024-04-06 19:55:40.000000 GABRIEL-ratings-0.1.4/gabriel/decorators.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     7178 2024-04-06 19:51:15.000000 GABRIEL-ratings-0.1.4/gabriel/foundational_functions.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     5136 2024-04-07 02:09:25.000000 GABRIEL-ratings-0.1.4/gabriel/openai_api_calls.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     1049 2024-04-06 19:51:29.000000 GABRIEL-ratings-0.1.4/gabriel/prompt_wrapping.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)       38 2024-04-07 02:16:06.148656 GABRIEL-ratings-0.1.4/setup.cfg
+-rw-r--r--   0 elliottmokski   (501) staff       (20)      915 2024-04-07 02:15:49.000000 GABRIEL-ratings-0.1.4/setup.py
```

### Comparing `GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/PKG-INFO` & `GABRIEL-ratings-0.1.4/GABRIEL_ratings.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GABRIEL-ratings
-Version: 0.1.3
+Version: 0.1.4
 Summary: THE GABRIEL library for numerical analysis of texts in the social sciences.
 Home-page: https://github.com/elliottmokski/GABRIEL-distribution
 Author: Hemanth Asirvatham and Elliott Mokski
 Author-email: elliottpmokski@gmail.com
 License: UNKNOWN
 Description: # The Generalized Attribute Based Ratings Information Extraction Library (GABRIEL)
         
@@ -37,20 +37,22 @@
         The main way to get ratings from GABRIEL is using the Archangel class. The class requires an OpenAI api-key for instantiation. We strongly recommend you store the key as an environment variable. To create an Archangel object, use the following syntax. 
         
         ```python
         from GABRIEL.Archangel import Archangel
         combined_assistant = Archangel(your_api_key)
         ```
         
-        Once you create the object, you can run a simple ratings framework through the *rate_texts* function. You must supply a list of the texts to rate, *texts*; an *attributes_dict*, where the keys are your attributes, and the values are the definitions; an object category (*object_category*) and an attribute category (*attribute_category*). You can also specify a specific OpenAI model for your call, using the *model* parameter (the default is GPT-3.5-turbo). See below for the full list of parameters, and more detailed descriptions.
+        Once you create the object, you can run a simple ratings framework through the *rate_texts* function. You must supply a list of the texts to rate, *texts*; an *attributes_dict*, where the keys are your attributes, and the values are the definitions, and a *task_description*, which is a few sentence description of what you're trying to acccomplish (your data, your question, etc.). In addition, we require a *save_folder* and a *file_name*, which is where the output from your run will be saved.
+        
+        You can also specify a specific OpenAI model for your call, using the *model* parameter (the default is GPT-3.5-turbo). See below for the full list of parameters, and more detailed descriptions.
         
         The simplest ratings call, which returns a Pandas dataframe, is just:
         
         ```python
-        ratings = archangel.rate_texts(texts, attributes_dict= attribute_dict, save_folder = 'path_to_your_folder', file_name = 'your_file_name.csv', attribute_category = your_attribute_category, object_category = your_object_category)
+        ratings = archangel.rate_texts(texts, attribute_dict= attribute_dict, save_folder = 'path_to_your_folder', file_name = 'your_file_name.csv', task_description = 'your_task_description')
         ```
         
         ### Features 
         
         The Archangel class comes with a number of easy to use features to help you run your code. 
         - parallelization: the library parallelizes API calls to dramatically speed up running time. We configure this by default.
         - cost estimates: we provide a very rough cost estimate of each run when you begin the call, based on the model and texts you input. 
@@ -62,25 +64,24 @@
         - 'mazda': cheap, fast, and reliable. Uses GPT-3.5-turbo, with text truncation to 9500 words to allow for prompts. Runs 50 queries in parallel.  
         - 'tesla': expensive. Uses GPT-4-turbo, with 30 parallel queries. Not recommended due to cost. 
         
         ### Function parameters
         
         The full list of parameters for the function is as follows. 
         
-        - **`search_axis_1`** (mandatory): A list containing the texts being evaluated. For example, `search_axis_1 = ['fed statement 1', 'fed statement 2', ...]`.
-        - **`object_category`** (mandatory): A string, simply describing the category of objects being evaluated. For example, `object_category = 'Fed Statements'` or `'Short Stories'`.
-        - **`attribute_category`** (mandatory): The category of attributes being evaluated. For example, `attribute_category = 'emotions'` or `'tastes'`.
-        - **`attributes`** (optional): A list containing the desired attributes for evaluation. If this is not specified, the model will generate **`n_search_attributes`** attributes itself. For example, `n_search_attributes = ['optimism', 'negativity', 'concern about unemployment']`.
-        - **`n_search_attributes`** (optional): An integer containing the number of attributes to generate if no attributes were specified. Defaults to 5. For example, `n_search_attributes = 10`.
-        - **`descriptions`** (optional): A list of descriptions for the attributes if **`attributes`** are provided explicitly. Otherwise, the descriptions will be generated by the model. For example, `descriptions = ['The happy attribute refers to a positive emotional state characterized by feelings of joy, contentment, and satisfaction.', 'The "sad" attribute is a feeling of sorrow, unhappiness, or distress. It is an emotional state characterized by a low mood and a sense of loss or disappointment.']`.
-        - **`object_clarification`** (optional): A string providing further clarification on the objects (e.g., a string of comma-separated examples).
-        - **`attribute_clarification`** (optional): A string providing further clarification on the attributes (e.g., a string of comma-separated examples). For use in the generation of attributes.
-        - **`use_classification`** (optional - defaults to False): Toggles whether the model uses a ratings or classification approach.
-        - **`classification_clarification`** (optional - only considered when `use_classification = True`): An additional string to provide context on the classification process.
-        - **`truncate`** (optional, defaults to True): Whether to truncate the text to the first 10,000 words. This avoids overloading the API token limit (16k tokens for the default model).
+        - **`attribute_dict`** A dictionary where the keys are the attributes you want to evaluate, and the values are the descriptions. See Colab notebook for examplse. 
+        <!-- - **`attributes`** (optional): A list containing the desired attributes for evaluation. If this is not specified, the model will generate **`n_search_attributes`** attributes itself. For example, `n_search_attributes = ['optimism', 'negativity', 'concern about unemployment']`. -->
+        <!-- - **`n_search_attributes`** (optional): An integer containing the number of attributes to generate if no attributes were specified. Defaults to 5. For example, `n_search_attributes = 10`. -->
+        <!-- - **`descriptions`** (optional): A list of descriptions for the attributes if **`attributes`** are provided explicitly. Otherwise, the descriptions will be generated by the model. For example, `descriptions = ['The happy attribute refers to a positive emotional state characterized by feelings of joy, contentment, and satisfaction.', 'The "sad" attribute is a feeling of sorrow, unhappiness, or distress. It is an emotional state characterized by a low mood and a sense of loss or disappointment.']`. -->
+        <!-- - **`object_clarification`** (optional): A string providing further clarification on the objects (e.g., a string of comma-separated examples). -->
+        <!-- - **`attribute_clarification`** (optional): A string providing further clarification on the attributes (e.g., a string of comma-separated examples). For use in the generation of attributes. -->
+        <!-- - **`use_classification`** (optional - defaults to False): Toggles whether the model uses a ratings or classification approach. -->
+        <!-- - **`classification_clarification`** (optional - only considered when `use_classification = True`): An additional string to provide context on the classification process. -->
+        - **`truncate`** (optional, defaults to True): Whether to truncate the text. This avoids overloading the API token limit (16k tokens for the default model).
+        -**`truncate_len`** (optional, defaults to 5000) the amount of text to keep. 
         - **`project_probs`** (optional, defaults to False): Whether to project the probabilities from 0 to 100 to a 0 to 1 scale.
         - **`api_key`** (mandatory): Your OpenAI API key.
         - **`model`** (optional): Backend model, default = `gpt-3.5-turbo-1106`.
         - **`seed`** (optional, RECOMMENDED): Set a seed for cross-run replicability. For instance, `seed = 0`.
         
         ## Citation
```

### Comparing `GABRIEL-ratings-0.1.3/PKG-INFO` & `GABRIEL-ratings-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GABRIEL-ratings
-Version: 0.1.3
+Version: 0.1.4
 Summary: THE GABRIEL library for numerical analysis of texts in the social sciences.
 Home-page: https://github.com/elliottmokski/GABRIEL-distribution
 Author: Hemanth Asirvatham and Elliott Mokski
 Author-email: elliottpmokski@gmail.com
 License: UNKNOWN
 Description: # The Generalized Attribute Based Ratings Information Extraction Library (GABRIEL)
         
@@ -37,20 +37,22 @@
         The main way to get ratings from GABRIEL is using the Archangel class. The class requires an OpenAI api-key for instantiation. We strongly recommend you store the key as an environment variable. To create an Archangel object, use the following syntax. 
         
         ```python
         from GABRIEL.Archangel import Archangel
         combined_assistant = Archangel(your_api_key)
         ```
         
-        Once you create the object, you can run a simple ratings framework through the *rate_texts* function. You must supply a list of the texts to rate, *texts*; an *attributes_dict*, where the keys are your attributes, and the values are the definitions; an object category (*object_category*) and an attribute category (*attribute_category*). You can also specify a specific OpenAI model for your call, using the *model* parameter (the default is GPT-3.5-turbo). See below for the full list of parameters, and more detailed descriptions.
+        Once you create the object, you can run a simple ratings framework through the *rate_texts* function. You must supply a list of the texts to rate, *texts*; an *attributes_dict*, where the keys are your attributes, and the values are the definitions, and a *task_description*, which is a few sentence description of what you're trying to acccomplish (your data, your question, etc.). In addition, we require a *save_folder* and a *file_name*, which is where the output from your run will be saved.
+        
+        You can also specify a specific OpenAI model for your call, using the *model* parameter (the default is GPT-3.5-turbo). See below for the full list of parameters, and more detailed descriptions.
         
         The simplest ratings call, which returns a Pandas dataframe, is just:
         
         ```python
-        ratings = archangel.rate_texts(texts, attributes_dict= attribute_dict, save_folder = 'path_to_your_folder', file_name = 'your_file_name.csv', attribute_category = your_attribute_category, object_category = your_object_category)
+        ratings = archangel.rate_texts(texts, attribute_dict= attribute_dict, save_folder = 'path_to_your_folder', file_name = 'your_file_name.csv', task_description = 'your_task_description')
         ```
         
         ### Features 
         
         The Archangel class comes with a number of easy to use features to help you run your code. 
         - parallelization: the library parallelizes API calls to dramatically speed up running time. We configure this by default.
         - cost estimates: we provide a very rough cost estimate of each run when you begin the call, based on the model and texts you input. 
@@ -62,25 +64,24 @@
         - 'mazda': cheap, fast, and reliable. Uses GPT-3.5-turbo, with text truncation to 9500 words to allow for prompts. Runs 50 queries in parallel.  
         - 'tesla': expensive. Uses GPT-4-turbo, with 30 parallel queries. Not recommended due to cost. 
         
         ### Function parameters
         
         The full list of parameters for the function is as follows. 
         
-        - **`search_axis_1`** (mandatory): A list containing the texts being evaluated. For example, `search_axis_1 = ['fed statement 1', 'fed statement 2', ...]`.
-        - **`object_category`** (mandatory): A string, simply describing the category of objects being evaluated. For example, `object_category = 'Fed Statements'` or `'Short Stories'`.
-        - **`attribute_category`** (mandatory): The category of attributes being evaluated. For example, `attribute_category = 'emotions'` or `'tastes'`.
-        - **`attributes`** (optional): A list containing the desired attributes for evaluation. If this is not specified, the model will generate **`n_search_attributes`** attributes itself. For example, `n_search_attributes = ['optimism', 'negativity', 'concern about unemployment']`.
-        - **`n_search_attributes`** (optional): An integer containing the number of attributes to generate if no attributes were specified. Defaults to 5. For example, `n_search_attributes = 10`.
-        - **`descriptions`** (optional): A list of descriptions for the attributes if **`attributes`** are provided explicitly. Otherwise, the descriptions will be generated by the model. For example, `descriptions = ['The happy attribute refers to a positive emotional state characterized by feelings of joy, contentment, and satisfaction.', 'The "sad" attribute is a feeling of sorrow, unhappiness, or distress. It is an emotional state characterized by a low mood and a sense of loss or disappointment.']`.
-        - **`object_clarification`** (optional): A string providing further clarification on the objects (e.g., a string of comma-separated examples).
-        - **`attribute_clarification`** (optional): A string providing further clarification on the attributes (e.g., a string of comma-separated examples). For use in the generation of attributes.
-        - **`use_classification`** (optional - defaults to False): Toggles whether the model uses a ratings or classification approach.
-        - **`classification_clarification`** (optional - only considered when `use_classification = True`): An additional string to provide context on the classification process.
-        - **`truncate`** (optional, defaults to True): Whether to truncate the text to the first 10,000 words. This avoids overloading the API token limit (16k tokens for the default model).
+        - **`attribute_dict`** A dictionary where the keys are the attributes you want to evaluate, and the values are the descriptions. See Colab notebook for examplse. 
+        <!-- - **`attributes`** (optional): A list containing the desired attributes for evaluation. If this is not specified, the model will generate **`n_search_attributes`** attributes itself. For example, `n_search_attributes = ['optimism', 'negativity', 'concern about unemployment']`. -->
+        <!-- - **`n_search_attributes`** (optional): An integer containing the number of attributes to generate if no attributes were specified. Defaults to 5. For example, `n_search_attributes = 10`. -->
+        <!-- - **`descriptions`** (optional): A list of descriptions for the attributes if **`attributes`** are provided explicitly. Otherwise, the descriptions will be generated by the model. For example, `descriptions = ['The happy attribute refers to a positive emotional state characterized by feelings of joy, contentment, and satisfaction.', 'The "sad" attribute is a feeling of sorrow, unhappiness, or distress. It is an emotional state characterized by a low mood and a sense of loss or disappointment.']`. -->
+        <!-- - **`object_clarification`** (optional): A string providing further clarification on the objects (e.g., a string of comma-separated examples). -->
+        <!-- - **`attribute_clarification`** (optional): A string providing further clarification on the attributes (e.g., a string of comma-separated examples). For use in the generation of attributes. -->
+        <!-- - **`use_classification`** (optional - defaults to False): Toggles whether the model uses a ratings or classification approach. -->
+        <!-- - **`classification_clarification`** (optional - only considered when `use_classification = True`): An additional string to provide context on the classification process. -->
+        - **`truncate`** (optional, defaults to True): Whether to truncate the text. This avoids overloading the API token limit (16k tokens for the default model).
+        -**`truncate_len`** (optional, defaults to 5000) the amount of text to keep. 
         - **`project_probs`** (optional, defaults to False): Whether to project the probabilities from 0 to 100 to a 0 to 1 scale.
         - **`api_key`** (mandatory): Your OpenAI API key.
         - **`model`** (optional): Backend model, default = `gpt-3.5-turbo-1106`.
         - **`seed`** (optional, RECOMMENDED): Set a seed for cross-run replicability. For instance, `seed = 0`.
         
         ## Citation
```

### Comparing `GABRIEL-ratings-0.1.3/README.md` & `GABRIEL-ratings-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -29,20 +29,22 @@
 The main way to get ratings from GABRIEL is using the Archangel class. The class requires an OpenAI api-key for instantiation. We strongly recommend you store the key as an environment variable. To create an Archangel object, use the following syntax. 
 
 ```python
 from GABRIEL.Archangel import Archangel
 combined_assistant = Archangel(your_api_key)
 ```
 
-Once you create the object, you can run a simple ratings framework through the *rate_texts* function. You must supply a list of the texts to rate, *texts*; an *attributes_dict*, where the keys are your attributes, and the values are the definitions; an object category (*object_category*) and an attribute category (*attribute_category*). You can also specify a specific OpenAI model for your call, using the *model* parameter (the default is GPT-3.5-turbo). See below for the full list of parameters, and more detailed descriptions.
+Once you create the object, you can run a simple ratings framework through the *rate_texts* function. You must supply a list of the texts to rate, *texts*; an *attributes_dict*, where the keys are your attributes, and the values are the definitions, and a *task_description*, which is a few sentence description of what you're trying to acccomplish (your data, your question, etc.). In addition, we require a *save_folder* and a *file_name*, which is where the output from your run will be saved.
+
+You can also specify a specific OpenAI model for your call, using the *model* parameter (the default is GPT-3.5-turbo). See below for the full list of parameters, and more detailed descriptions.
 
 The simplest ratings call, which returns a Pandas dataframe, is just:
 
 ```python
-ratings = archangel.rate_texts(texts, attributes_dict= attribute_dict, save_folder = 'path_to_your_folder', file_name = 'your_file_name.csv', attribute_category = your_attribute_category, object_category = your_object_category)
+ratings = archangel.rate_texts(texts, attribute_dict= attribute_dict, save_folder = 'path_to_your_folder', file_name = 'your_file_name.csv', task_description = 'your_task_description')
 ```
 
 ### Features 
 
 The Archangel class comes with a number of easy to use features to help you run your code. 
 - parallelization: the library parallelizes API calls to dramatically speed up running time. We configure this by default.
 - cost estimates: we provide a very rough cost estimate of each run when you begin the call, based on the model and texts you input. 
@@ -54,25 +56,24 @@
 - 'mazda': cheap, fast, and reliable. Uses GPT-3.5-turbo, with text truncation to 9500 words to allow for prompts. Runs 50 queries in parallel.  
 - 'tesla': expensive. Uses GPT-4-turbo, with 30 parallel queries. Not recommended due to cost. 
 
 ### Function parameters
 
 The full list of parameters for the function is as follows. 
 
-- **`search_axis_1`** (mandatory): A list containing the texts being evaluated. For example, `search_axis_1 = ['fed statement 1', 'fed statement 2', ...]`.
-- **`object_category`** (mandatory): A string, simply describing the category of objects being evaluated. For example, `object_category = 'Fed Statements'` or `'Short Stories'`.
-- **`attribute_category`** (mandatory): The category of attributes being evaluated. For example, `attribute_category = 'emotions'` or `'tastes'`.
-- **`attributes`** (optional): A list containing the desired attributes for evaluation. If this is not specified, the model will generate **`n_search_attributes`** attributes itself. For example, `n_search_attributes = ['optimism', 'negativity', 'concern about unemployment']`.
-- **`n_search_attributes`** (optional): An integer containing the number of attributes to generate if no attributes were specified. Defaults to 5. For example, `n_search_attributes = 10`.
-- **`descriptions`** (optional): A list of descriptions for the attributes if **`attributes`** are provided explicitly. Otherwise, the descriptions will be generated by the model. For example, `descriptions = ['The happy attribute refers to a positive emotional state characterized by feelings of joy, contentment, and satisfaction.', 'The "sad" attribute is a feeling of sorrow, unhappiness, or distress. It is an emotional state characterized by a low mood and a sense of loss or disappointment.']`.
-- **`object_clarification`** (optional): A string providing further clarification on the objects (e.g., a string of comma-separated examples).
-- **`attribute_clarification`** (optional): A string providing further clarification on the attributes (e.g., a string of comma-separated examples). For use in the generation of attributes.
-- **`use_classification`** (optional - defaults to False): Toggles whether the model uses a ratings or classification approach.
-- **`classification_clarification`** (optional - only considered when `use_classification = True`): An additional string to provide context on the classification process.
-- **`truncate`** (optional, defaults to True): Whether to truncate the text to the first 10,000 words. This avoids overloading the API token limit (16k tokens for the default model).
+- **`attribute_dict`** A dictionary where the keys are the attributes you want to evaluate, and the values are the descriptions. See Colab notebook for examplse. 
+<!-- - **`attributes`** (optional): A list containing the desired attributes for evaluation. If this is not specified, the model will generate **`n_search_attributes`** attributes itself. For example, `n_search_attributes = ['optimism', 'negativity', 'concern about unemployment']`. -->
+<!-- - **`n_search_attributes`** (optional): An integer containing the number of attributes to generate if no attributes were specified. Defaults to 5. For example, `n_search_attributes = 10`. -->
+<!-- - **`descriptions`** (optional): A list of descriptions for the attributes if **`attributes`** are provided explicitly. Otherwise, the descriptions will be generated by the model. For example, `descriptions = ['The happy attribute refers to a positive emotional state characterized by feelings of joy, contentment, and satisfaction.', 'The "sad" attribute is a feeling of sorrow, unhappiness, or distress. It is an emotional state characterized by a low mood and a sense of loss or disappointment.']`. -->
+<!-- - **`object_clarification`** (optional): A string providing further clarification on the objects (e.g., a string of comma-separated examples). -->
+<!-- - **`attribute_clarification`** (optional): A string providing further clarification on the attributes (e.g., a string of comma-separated examples). For use in the generation of attributes. -->
+<!-- - **`use_classification`** (optional - defaults to False): Toggles whether the model uses a ratings or classification approach. -->
+<!-- - **`classification_clarification`** (optional - only considered when `use_classification = True`): An additional string to provide context on the classification process. -->
+- **`truncate`** (optional, defaults to True): Whether to truncate the text. This avoids overloading the API token limit (16k tokens for the default model).
+-**`truncate_len`** (optional, defaults to 5000) the amount of text to keep. 
 - **`project_probs`** (optional, defaults to False): Whether to project the probabilities from 0 to 100 to a 0 to 1 scale.
 - **`api_key`** (mandatory): Your OpenAI API key.
 - **`model`** (optional): Backend model, default = `gpt-3.5-turbo-1106`.
 - **`seed`** (optional, RECOMMENDED): Set a seed for cross-run replicability. For instance, `seed = 0`.
 
 ## Citation
```

### Comparing `GABRIEL-ratings-0.1.3/gabriel/archangel.py` & `GABRIEL-ratings-0.1.4/gabriel/archangel.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,20 @@
         elif 'gpt-4' in model:
             return round(sum([(len(text.split()) + 3000 + 2000) for text in texts]) / 1000 / 1000 * 1.33 * 20,3)
         else:
             return 'Unknown model'
 
     def get_preset_params(self, preset='mazda'):
         if preset == 'mazda':
-            return {'model': 'gpt-3.5-turbo', 'n_parallel': 50, 'num_runs': 10, 'rate_first': False, 'temperature':0.8,
-                    'timeout': 75, 'truncate_len': 5000, 'seed': None, 'truncate':True, 'format':'json',"batch_len":50}
+            return {'model': 'gpt-3.5-turbo', 'n_parallel': 3, 'num_runs': 10, 'rate_first': False, 'temperature':0.8,
+                    'timeout': 75, 'truncate_len': 5000, 'seed': None, 'truncate':True, 'format':'json'}
         
         elif preset == 'tesla':
-            return {'model': 'gpt-4-turbo', 'n_parallel': 30, 'num_runs': 10, 'rate_first': False, 'temperature':0.8,
-                    'timeout': 75, 'truncate_len': 5000, 'seed': None, 'truncate':True, 'format':'json', "batch_len":50}
+            return {'model': 'gpt-4-turbo', 'n_parallel': 3, 'num_runs': 10, 'rate_first': False, 'temperature':0.8,
+                    'timeout': 75, 'truncate_len': 5000, 'seed': None, 'truncate':True, 'format':'json'}
         
     def get_attributes(self, attributes_dict=None, attribute_mode='compare'):
         attribute_dict = self.attributor.get_attributes(attributes_dict=attributes_dict, attribute_mode=attribute_mode)
         return attributes_dict
 
     def rate(self, preset='mazda', task_explainer=None, entities=None, attributes_dict=None, attribute_mode='compare',
              model='gpt-3.5-turbo', examples=None, n_parallel=50,
@@ -40,15 +40,15 @@
         return ratings
 
     def rate_texts(self, texts, preset='mazda', task_description=None, attribute_dict=None, attribute_mode='rate',
              model=None, examples='', n_parallel=None,
              save_folder=None, mode='rate', num_runs=None, rate_first=False, file_name = None,
              temperature = None, timeout = None, 
              truncate_len = None, seed = None,truncate = None, use_classification = False, 
-             format = None, project_probs = None, classification_clarification = None, batch_len = None, reset_files = False):
+             format = None, project_probs = None, classification_clarification = None, reset_files = False):
         
         if file_name == None:
             raise Exception('You must provide a file name to save to.')
 
         full_path = os.path.join(save_folder, file_name)
         if not os.path.isdir(save_folder):
             raise Exception('The save folder does not exist. Please provide a valid save_folder.')
@@ -68,49 +68,63 @@
             df['Text'] = texts
             df.to_csv(full_path, index = False)
             df = pd.read_csv(full_path)
             print(f'Creating a new file at {full_path}')
             texts = df['Text'].to_list()
         
         preset_params = self.get_preset_params(preset)
+        call_params = preset_params.copy()
+
 
-        #Override the ones without None
         for param in preset_params.keys():
-            if locals()[param] is None:
-                locals()[param] = preset_params[param]
+            if locals()[param] == None:
+                call_params[param] = preset_params[param]
+            else:
+                call_params[param] = locals()[param]
+
+        call_params['project_probs'] = False
+        call_params['api_key'] = self.api_key
         
         if task_description == None:
             raise Exception('Please provide a task_description')
         else:
             print(f'Extracting categories for task: {task_description}')
             categories = json.loads(identify_categories(task_description= task_description, api_key = self.api_key))
-            entity_category = categories['entity category']
-            attribute_category = categories['attribute category']
+            call_params['entity_category'] = categories['entity category']
+            call_params['attribute_category'] = categories['attribute category']
+            call_params['classification_clarification'] = classification_clarification
+            call_params['use_classification'] = use_classification
 
         if attribute_mode == 'rate':
             rating_function = self.attributor.rate_single_text
-            call_params = {'entity_category': entity_category, 'attribute_category': attribute_category, 'api_key': self.api_key,
-                      'model': preset_params['model'], 'temperature': preset_params['temperature'], 'use_classification': use_classification, 
-                      'format': preset_params['format'],'project_probs': False, 'truncate': preset_params['truncate'], 
-                      'seed': preset_params['seed'],'timeout': preset_params['timeout'], 'truncate_len': preset_params['truncate_len'],
-                      'classification_clarification': classification_clarification}
         elif attribute_mode == 'classify':
             rating_function = generate_simple_classification
         elif attribute_mode == 'compare':
             pass
 
         final = pd.DataFrame()  # Initialize the final DataFrame
-        processed_rows = 0  # Initialize the processed rows counter
+
+        # {'model': 'gpt-3.5-turbo', 'n_parallel': 10, 'num_runs': 10, 'rate_first': False, 'temperature':0.8,
+        #             'timeout': 75, 'truncate_len': 5000, 'seed': None, 'truncate':True, 'format':'json'}
+
+        # text, attribute_dict, entity_category, attribute_category, temperature,use_classification, format, classification_clarification, 
+        #                         project_probs, truncate, model, seed, api_key, truncate_len, timeout
+
+        batches = [texts[i:i + call_params['n_parallel']] for i in range(0, len(texts),call_params['n_parallel'])]  
+
+        del call_params['num_runs']
+        del call_params['rate_first']
 
         print('Here are the parameters for this run:\n')
-        print(json.dumps(preset_params, indent=4))
+        print(json.dumps(call_params, indent=4))
+        del call_params['n_parallel']
+
         print(f'The output file will be saved at: {save_folder}/{file_name}')
         print(f'''Rough estimated cost in dollars: {self.estimate_cost(texts, call_params['model'])}''')
 
-        batches = [texts[i:i + preset_params['batch_len']] for i in range(0, len(texts), preset_params['batch_len'])]  
         
         for batch in tqdm(batches, total=len(batches)):
             batch_results = []
             with ThreadPoolExecutor(max_workers=len(batch)) as executor:
                 futures = {executor.submit(rating_function, text = text, attribute_dict = attribute_dict, **call_params): text for text in batch}
                 for future in as_completed(futures):
                     text = futures[future]
```

### Comparing `GABRIEL-ratings-0.1.3/gabriel/combined_assistant.py` & `GABRIEL-ratings-0.1.4/gabriel/combined_assistant.py`

 * *Files identical despite different names*

### Comparing `GABRIEL-ratings-0.1.3/gabriel/decorators.py` & `GABRIEL-ratings-0.1.4/gabriel/decorators.py`

 * *Files identical despite different names*

### Comparing `GABRIEL-ratings-0.1.3/gabriel/foundational_functions.py` & `GABRIEL-ratings-0.1.4/gabriel/foundational_functions.py`

 * *Files identical despite different names*

### Comparing `GABRIEL-ratings-0.1.3/gabriel/openai_api_calls.py` & `GABRIEL-ratings-0.1.4/gabriel/openai_api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 def retry_on_api_error(max_retries, delay=45):
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             for attempt in range(max_retries):
                 try:
                     return func(*args, **kwargs)
-                except openai._exceptions.RateLimitError as e:
+                except openai.RateLimitError as e:
                     print(f"Rate limit error on attempt {attempt + 1}/{max_retries}. Retrying after delay.")
                     time.sleep(delay)  # Sleep and retry after delay
-                except openai._exceptions.OpenAIError as e:
+                except openai.OpenAIError as e:
                     print(f"OpenAI error on attempt {attempt + 1}/{max_retries}: {e}")
                     if attempt == max_retries - 1:
                         raise APIError("Failed after max retries due to OpenAI error.")
                 except Exception as e:
                     print(f"Unexpected error on attempt {attempt + 1}/{max_retries}: {e}")
                     if attempt == max_retries - 1:
                         raise APIError("Failed after max retries due to an unexpected error.")
@@ -108,19 +108,18 @@
                 )
                 # Extract the response content based on the specified format
                 # if desired_response_format == 'text':
                 response_message = response.choices[0].message.content
                 # else: # If the response format is 'json', handle accordingly
                     # response_message = response.choices[0].message
 
-            except openai._exceptions.RateLimitError:
-                time.sleep(45)
-                raise
-            except openai._exceptions.OpenAIError as e:
-                raise
+            except openai.RateLimitError as e:
+                raise e
+            except openai.OpenAIError as e:
+                raise e
             response_queue.put(response_message)
 
         # Start the thread to make the API call
         thread = threading.Thread(target=target)
         thread.start()
         thread.join(timeout)
```

### Comparing `GABRIEL-ratings-0.1.3/gabriel/prompt_wrapping.py` & `GABRIEL-ratings-0.1.4/gabriel/prompt_wrapping.py`

 * *Files identical despite different names*

### Comparing `GABRIEL-ratings-0.1.3/setup.py` & `GABRIEL-ratings-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GABRIEL-ratings', 
-    version='0.1.3',  
+    version='0.1.4',  
     author='Hemanth Asirvatham and Elliott Mokski',  
     author_email='elliottpmokski@gmail.com',  
     description='THE GABRIEL library for numerical analysis of texts in the social sciences.', 
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/elliottmokski/GABRIEL-distribution',  
     packages=find_packages(),
```

