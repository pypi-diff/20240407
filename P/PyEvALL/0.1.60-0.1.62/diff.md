# Comparing `tmp/PyEvALL-0.1.60.tar.gz` & `tmp/PyEvALL-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEvALL-0.1.60.tar", last modified: Thu Apr  4 11:03:38 2024, max compression
+gzip compressed data, was "PyEvALL-0.1.62.tar", last modified: Sun Apr  7 13:17:03 2024, max compression
```

## Comparing `PyEvALL-0.1.60.tar` & `PyEvALL-0.1.62.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.581058 PyEvALL-0.1.60/
--rw-rw-rw-   0        0        0       24 2024-03-13 22:18:07.000000 PyEvALL-0.1.60/MANIFEST.in
--rw-rw-rw-   0        0        0      447 2024-04-04 11:03:38.580061 PyEvALL-0.1.60/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.530050 PyEvALL-0.1.60/PyEvALL.egg-info/
--rw-rw-rw-   0        0        0      447 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    25635 2024-04-04 10:56:47.000000 PyEvALL-0.1.60/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.538606 PyEvALL-0.1.60/pyevall/
--rw-rw-rw-   0        0        0        0 2023-02-07 00:42:14.000000 PyEvALL-0.1.60/pyevall/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.555766 PyEvALL-0.1.60/pyevall/comparators/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:43:21.000000 PyEvALL-0.1.60/pyevall/comparators/__init__.py
--rw-rw-rw-   0        0        0    15925 2024-04-03 20:07:49.000000 PyEvALL-0.1.60/pyevall/comparators/comparators.py
--rw-rw-rw-   0        0        0    20371 2024-04-03 09:08:50.000000 PyEvALL-0.1.60/pyevall/comparators/formats.py
--rw-rw-rw-   0        0        0     9855 2024-04-03 09:08:55.000000 PyEvALL-0.1.60/pyevall/evaluation.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.571725 PyEvALL-0.1.60/pyevall/metrics/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:42:54.000000 PyEvALL-0.1.60/pyevall/metrics/__init__.py
--rw-rw-rw-   0        0        0     4187 2024-04-03 09:09:44.000000 PyEvALL-0.1.60/pyevall/metrics/metricfactory.py
--rw-rw-rw-   0        0        0    55383 2024-04-04 08:29:36.000000 PyEvALL-0.1.60/pyevall/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.572722 PyEvALL-0.1.60/pyevall/reports/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:42:12.000000 PyEvALL-0.1.60/pyevall/reports/__init__.py
--rw-rw-rw-   0        0        0    27269 2024-04-04 10:04:56.000000 PyEvALL-0.1.60/pyevall/reports/reports.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.576323 PyEvALL-0.1.60/pyevall/utils/
--rw-rw-rw-   0        0        0      479 2024-03-06 07:06:10.000000 PyEvALL-0.1.60/pyevall/utils/file.conf
--rw-rw-rw-   0        0        0     2459 2024-04-04 10:28:07.000000 PyEvALL-0.1.60/pyevall/utils/pyevall_keys_texts_reports.rep
--rw-rw-rw-   0        0        0     8000 2024-04-03 13:16:56.000000 PyEvALL-0.1.60/pyevall/utils/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-04 11:03:38.581058 PyEvALL-0.1.60/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-04-04 10:58:18.000000 PyEvALL-0.1.60/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.579061 PyEvALL-0.1.60/test/
--rw-rw-rw-   0        0        0    10405 2024-04-03 16:37:42.000000 PyEvALL-0.1.60/test/testformats.py
--rw-rw-rw-   0        0        0    11154 2024-04-03 20:01:38.000000 PyEvALL-0.1.60/test/testmetrics.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.027772 PyEvALL-0.1.62/
+-rw-rw-rw-   0        0        0       24 2024-03-13 22:18:07.000000 PyEvALL-0.1.62/MANIFEST.in
+-rw-rw-rw-   0        0        0      447 2024-04-07 13:17:03.027772 PyEvALL-0.1.62/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.004140 PyEvALL-0.1.62/PyEvALL.egg-info/
+-rw-rw-rw-   0        0        0      447 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    26380 2024-04-07 13:15:19.000000 PyEvALL-0.1.62/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.004140 PyEvALL-0.1.62/pyevall/
+-rw-rw-rw-   0        0        0        0 2023-02-07 00:42:14.000000 PyEvALL-0.1.62/pyevall/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.004140 PyEvALL-0.1.62/pyevall/comparators/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:43:21.000000 PyEvALL-0.1.62/pyevall/comparators/__init__.py
+-rw-rw-rw-   0        0        0    15325 2024-04-07 06:02:05.000000 PyEvALL-0.1.62/pyevall/comparators/comparators.py
+-rw-rw-rw-   0        0        0    21114 2024-04-07 13:08:09.000000 PyEvALL-0.1.62/pyevall/comparators/formats.py
+-rw-rw-rw-   0        0        0     9855 2024-04-03 09:08:55.000000 PyEvALL-0.1.62/pyevall/evaluation.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.019763 PyEvALL-0.1.62/pyevall/metrics/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:42:54.000000 PyEvALL-0.1.62/pyevall/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4187 2024-04-03 09:09:44.000000 PyEvALL-0.1.62/pyevall/metrics/metricfactory.py
+-rw-rw-rw-   0        0        0    55383 2024-04-05 22:08:18.000000 PyEvALL-0.1.62/pyevall/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.019763 PyEvALL-0.1.62/pyevall/reports/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:42:12.000000 PyEvALL-0.1.62/pyevall/reports/__init__.py
+-rw-rw-rw-   0        0        0    27269 2024-04-04 10:04:56.000000 PyEvALL-0.1.62/pyevall/reports/reports.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.019763 PyEvALL-0.1.62/pyevall/utils/
+-rw-rw-rw-   0        0        0      479 2024-03-06 07:06:10.000000 PyEvALL-0.1.62/pyevall/utils/file.conf
+-rw-rw-rw-   0        0        0     2459 2024-04-04 10:28:07.000000 PyEvALL-0.1.62/pyevall/utils/pyevall_keys_texts_reports.rep
+-rw-rw-rw-   0        0        0     8000 2024-04-03 13:16:56.000000 PyEvALL-0.1.62/pyevall/utils/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 13:17:03.027772 PyEvALL-0.1.62/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-04-07 06:35:30.000000 PyEvALL-0.1.62/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.019763 PyEvALL-0.1.62/test/
+-rw-rw-rw-   0        0        0    10405 2024-04-03 16:37:42.000000 PyEvALL-0.1.62/test/testformats.py
+-rw-rw-rw-   0        0        0    11154 2024-04-03 20:01:38.000000 PyEvALL-0.1.62/test/testmetrics.py
```

### Comparing `PyEvALL-0.1.60/PyEvALL.egg-info/SOURCES.txt` & `PyEvALL-0.1.62/PyEvALL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.60/README.md` & `PyEvALL-0.1.62/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 <p>
     <img src="img/Logo_PyEvALL.png#gh-light-mode-only" height="auto" width="300"/>
     <img src="img/Logo_PyEvALL_dark.png#gh-dark-mode-only" height="auto" width="300"/>
 </p>
 
 
 
-PyEvALL (The Python library to Evaluate ALL) is a evaluation tool for information systems that allows assessing a wide range of metrics covering various evaluation contexts, including classification, ranking, or LeWeDi (Learning with disagreement). PyEvALL is designed based on the following concepts: (i) **persistence**, users can save evaluations and retrieve past evaluations; (ii) **replicability**, all evaluations are conducted using the same methodology, making them strictly comparable; (iii) **effectiveness**, all metrics are unified under measurement theory and have been doubly implemented and compared; (iv) **generalization**, generalization is achieved through the use of a standardized input format enabling users to evaluate all evaluation contexts.
+PyEvALL (The Python library to Evaluate ALL) is an evaluation tool for information systems that allows assessing a wide range of metrics covering various evaluation contexts, including classification, ranking, or LeWiDi (Learning with disagreement). PyEvALL is designed based on the following concepts: (i) **persistence**, users can save evaluations and retrieve past evaluations; (ii) **replicability**, all evaluations are conducted using the same methodology, making them strictly comparable; (iii) **effectiveness**, all metrics are unified under measurement theory and have been doubly implemented and compared; (iv) **generalization**, achieved through the use of a standardized input format enabling users to evaluate all evaluation contexts.
 
 <!---
 ************************		INDEX		************************
 -->
 
 - [What evaluation contexts and metrics does PyEvALL include?](#what-evaluation-contexts-and-metrics-does-pyevall-include)
 - [Quickstart Guide](#quickstart-guide)
-   * [Intallating PyEvALL](#intallating-pyevall)
+   * [Installing PyEvALL](#installing-pyevall)
    * [Evaluating a prediction file](#evaluating-a-prediction-file)
       + [Input format parameter](#input-format-parameter)
       + [PyEvALL report format parameter](#pyevall-report-format-parameter)
          - [PyEvALL embedded report](#pyevall-embedded-report)
          - [PyEvALL dataframe report](#pyevall-dataframe-report)
       + [Hierarchy parameter](#hierarchy-parameter)
    * [Evaluating a list of prediction files](#evaluating-a-list-of-prediction-files)
@@ -32,15 +32,15 @@
 
 
 <!---
 ************************		SECTION 1		************************
 -->
 
 # What evaluation contexts and metrics does PyEvALL include?
-PyEvALL 2.0 allows evaluation in the following evaluation contexts:
+PyEvALL 2.0 allows evaluation in the following contexts:
 
 - **Mono-label classification**: evaluation context where each instance is assigned one target class, and only one. Additionally, the classes have no order or hierarchy among them, and all have the same relevance. The available metrics for this context are: *Accuracy, System Precision, Kappa, Precision, Recall, F-Measure, ICM* and *ICM Norm*.
 
 - **Multi-label classification**: evaluation context where each instance is assigned one or more classes from a set of target classes. Additionally, the classes have no order or hierarchy among them, and all have the same relevance. In this context, evaluation can be performed with the metrics *Precision, Recall* and *F-measure*.
 
 - **Mono-label hierarchical classification**: evaluation context where each instance is assigned one target class, and only one. Additionally, the classes have a hierarchical relationship, so that errors between classes at the same hierarchical level represent less failure than errors between classes at different hierarchical levels. In this context, the metrics *ICM* and *ICM Norm* are available.
 
@@ -55,15 +55,15 @@
 <!---
 ************************		SECTION 2		************************
 -->
 
 # Quickstart Guide
 PyEvALL is available via code, by downloading the source or installing the pip package, or via web interface (available soon, may 2024).
 
-## Intallating PyEvALL
+## Installing PyEvALL
 PyEvALL can be installed via source code, downloading the content of this repository, or installing the [PyEvALL](https://pypi.org/project/PyEvALL/#description)
 
 ```python  
 pip install PyEvALL
 
 ```
 
@@ -81,15 +81,15 @@
 metrics: list with the metrics to evaluate.
 
 params: dictionary with different parameters that can be configured for each evaluation.
 '''
 def evaluate(self, predictions, goldstandard, lst_metrics, **params):
 
 ```
-As seen in the above code, the function requires three mandatory parameters and one optional. The mandatory parameters represent the file with the predictions, the file with the gold standard, and the list of metrics to evaluate, respectively. On the other hand, the optional parameter params allows configuring different aspects of the evaluation.
+As seen in the code above, the function requires three mandatory parameters and one optional. The mandatory parameters represent the file with the predictions, the file with the gold standard, and the list of metrics to evaluate, respectively. On the other hand, the optional parameter "params" allows configuring different aspects of the evaluation.
 
 An example code of how to evaluate a prediction file is:
 
 ```python
 from pyevall.evaluation import PyEvALLEvaluation
 from pyevall.utils.utils import PyEvALLUtils
 predictions = "test/resources/metric/test/classification/predictions/SYS5.txt"
@@ -101,17 +101,22 @@
 params={PyEvALLUtils.PARAM_FORMAT: PyEvALLUtils.PARAM_OPTION_FORMAT_TSV }   
 report = test.evaluate(predictions, gold, metrics, **params)
 report.print_report()
 
 
 ```
 
+It is important to notice that all metrics' names can be accessed via *MetricFactory* class:
+
+```python
+metrics = [MetricFactory.Accuracy.value, MetricFactory.Precision.value, MetricFactory.Recall.value, MetricFactory.FMeasure.value]
+```
 
 ### Input format parameter
-PyEvALL currently supports 3 different formats: JSON, TSV, and CSV, with JSON being the default and primary format. It is important to emphasize that both files, both predictions, and the gold standard, must be in the same format for the evaluation to be carried out correctly. To modify the format of the input files, it is necessary to indicate it in the params parameter as follows:
+PyEvALL currently supports 3 different formats: JSON, TSV, and CSV, with JSON being the default and primary format. It is important to emphasize that both files, the predictions and the gold standard, must be in the same format for the evaluation to be carried out correctly. To modify the format of the input files, it is necessary to indicate it in the "params" parameter as follows:
 
 ```python
 
     params[PyEvALLUtils.PARAM_FORMAT]= PyEvALLUtils.PARAM_OPTION_FORMAT_TSV
 
 ```
 
@@ -121,15 +126,15 @@
 
     params[PyEvALLUtils.PARAM_FORMAT]= PyEvALLUtils.PARAM_OPTION_FORMAT_JSON
     params[PyEvALLUtils.PARAM_FORMAT]= PyEvALLUtils.PARAM_OPTION_FORMAT_TSV
     params[PyEvALLUtils.PARAM_FORMAT]= PyEvALLUtils.PARAM_OPTION_FORMAT_CSV
 
 ```
 
-Note that JSON format is the default format, so it is not necessary to specify it if not desired.
+Note that JSON format is the default format, so it is not necessary to specify it.
 
 ### PyEvALL report format parameter
 PyEvALL evaluation reports are generated in JSON format by concatenating different Python dictionaries containing information generated during the evaluation process. This composition of different dictionaries generates a generic JSON used by PyEvALL for its entire internal evaluation process. PyEvALL is designed around the pair *prediction file, gold standard file*, and likewise, the reports focus on this pair.
 
 ```python
 {
   "metrics": {
@@ -179,30 +184,30 @@
       "gold": true,
       "description": "Use parameter: report=\"embedded\"!",
       "errors": {}
     }
   }
 }
 ```
-In the metrics element, the main attributes of the metric are found, which can be useful for generating reports of other types, such as the name or acronym, as well as the results of the metric itself. Additionally, this element includes any potential errors in the analysis of the preconditions of each metric, if any. For example, as seen in the Figure, the metric *precision* has not met its input format precondition for the provided file pair, so it has not been executed, and this is reported to the user.
+In the "metrics" element, the main attributes of the metric are found, which can be useful for generating reports of other types, such as the name or acronym, as well as the results of the metric itself. Additionally, this element includes any potential errors in the analysis of the preconditions of each metric, if any. For example, as seen in the Figure, the metric *precision* has not met its input format precondition for the provided file pair, so it has not been executed, and this is reported to the user.
 
-On the other hand, the files element collects any potential errors detected in the files analyzed during the evaluation, i.e., the prediction file and the gold standard file. Each element also includes a description of each error or analysis, allowing for the generation of more explanatory and comprehensive reports. Specifically, to obtain textual explanations of the errors and the analysis of the evaluation process with embedded explanations, the parameter *report=embedded* is used.
+On the other hand, the "files" element collects any potential errors detected in the files analyzed during the evaluation, i.e., the prediction file and the gold standard file. Each element also includes a description of each error or analysis, allowing for the generation of more explanatory and comprehensive reports. Specifically, to obtain textual explanations of the errors and the analysis of the evaluation process with embedded explanations, the parameter *report=embedded* is used.
 
 The proposed format can be interpreted by various analyzers, providing users with enriched reports tailored to their needs, such as the report with embedded explanations.
 
 
 
 #### PyEvALL embedded report
 The embedded explanations report of PyEvALL is a JSON report with embedded textual information describing the errors and analysis processes carried out during the evaluation. It provides clear and precise details about the errors detected in the input files. The parameter included should be the following:
 
 ```python
 params[PyEvALLUtils.PARAM_REPORT]= PyEvALLUtils.PARAM_OPTION_REPORT_EMBEDDED  
 ```
 
-An example of the embedded explanations report format can be seen in Figure. As shown in the image, this report is almost identical to the previous one except that the description field includes descriptions. Referring to the previous example, the precision metric generates an error because the input format is not appropriate for this evaluation context, as explained in the message. Likewise, it is indicated that the files have been processed correctly.
+An example of the embedded explanations report format can be seen in next figure. As shown in the image, this report is almost identical to the previous one except that the description field includes explanations to describe the process. Referring to the previous example, the precision metric generates an error because the input format is not appropriate for this evaluation context, as explained in the message. Likewise, it is indicated that the files have been processed correctly.
 
 ```python
 {
   "metrics": {
     "PrecisionAtK": {
       "name": "Precision at k",
       "acronym": "P@k",
@@ -327,15 +332,15 @@
     params[PyEvALLUtils.PARAM_HIERARCHY]= DIPROMATS_TASK3
 
 ```
 
 As shown in the code snippet, the hierarchy is a Python dictionary where each level is formed by a new dictionary, and the leaves are formed by arrays. Note that if the parameter is not specified, metrics that require it cannot be evaluated, or they will be evaluated in a non-hierarchical manner.
 
 ## Evaluating a list of prediction files
-PyEvALL also provides a method by which a list of prediction files can be evaluated, allowing multiple systems to be evaluated at once. In this mode, PyEvALL generates a meta-report that includes the reports of each prediction file, gold standard file pair. The execution of this method would be as follows:
+PyEvALL also provides a method by which a list of prediction files can be evaluated, allowing multiple systems to be evaluated at once. In this mode, PyEvALL generates a meta-report that includes the reports of each *prediction file, gold standard* file pair. The execution of this method would be as follows:
 
 ```python
 from pyevall.evaluation import PyEvALLEvaluation
 from pyevall.utils.utils import PyEvALLUtils
 predictions_1 = "test/resources/metric/test/classification/predictions/SYS3.txt"
 predictions_2 = "test/resources/metric/test/classification/predictions/SYS4.txt"
 predictions_3 = "test/resources/metric/test/classification/predictions/SYS5.txt"
@@ -424,14 +429,24 @@
 ```
 
 Specifically, each attribute represents:
 - **test_case**: in string format, a specific experiment or use case, which could be, for example, different runs of a classification algorithm or different queries in a ranking context.
 - **id**: accepts both string or int format, but it has to be the same for both the predictions and gold standard files. It is the unique identifier of the instance in the dataset.
 - **value**: this field represents the value assigned to each item, and its type will vary depending on the applied evaluation context. For example, for mono-label classification, the element will be composed of a string, while for multi-label classification, the element will be composed of a vector of strings.
 
+This format can be easily obtained form a dataframe by using the option *gold_df.to_json(orient="records")*, like in the following example:
+
+```python
+gold_df = pd.DataFrame({'test_case': ['EXIST2023','EXIST2023','EXIST2023','EXIST2023'], 
+                        'id': ['101','102','103','104'],
+                        'value': ["0","1","0","1"]})
+with open(output_file_json, 'w', encoding='utf-8') as output_file: 
+            output_file.write(gold_df.to_json(orient="records"))                   
+```
+
 This format can be adapted for different evaluation contexts. Below are examples of the format based on the context:
 
 ## Mono-label Classification Format
 
 This format is the typical format for mono-label classification tasks where each item has a single associated class. In this format, the label can be any string of characters. An example for this format is:
 
 ```python
@@ -449,19 +464,21 @@
           {  
             "test_case":"EXIST2023",
 	    	 "id":"I3",
             "value":"C"
           }  
 ]
 ```
-In the example shown, it can be seen that the array consists of three elements belonging to the same test_case, 'EXIST2023', with three different identifiers (I1, I2, and I3), and three different target classes ('A', 'B', and 'C').
+
+In the example above, it can be seen that the array consists of three elements belonging to the same test_case, 'EXIST2023', with three different identifiers (I1, I2, and I3), and three different target classes ('A', 'B', and 'C').
+
 
 ## Multi-label Classification Format
 
-The multi-label classification format is one in which each item can be classified with one or several target classes. For this reason, the PyEvALL format for this type is composed of the same elements as in the previous case, with the difference that the "value" attribute in this case is an array of elements. These elements, in turn, must be strings. An example for this format can be found in the following code snippet:
+In the multi-label classification format, each item can be classified with one or several target classes. For this reason, the PyEvALL format for this type is composed of the same elements as in the previous case, with the difference that the "value" attribute is now an array of elements. These elements, in turn, must be strings. An example for this format can be found in the following code snippet:
 
 ```python
 [
 	  {  
 	    "test_case":"EXIST2023",
 	    "id":"I1",
 	    "value":["A"]  
@@ -480,15 +497,15 @@
 ```
 
 
 As seen in the example, the file consists of an array of JSON objects with three elements with the same fields as in the previous case, but with the difference that, in this case, the "value" attribute is composed of an array with the target classes of each item.
 
 ## LeWiDi Classification Format
 
-The disagreement classification format allows assigning a probability distribution to each class for every element in the dataset. Instead of selecting a single absolute category for each item, the label distribution by annotator is assigned to each element. In this format, as shown in the example below, PyEvALL uses the same structure, except that in this case, the "value" attribute is represented with a dictionary where each element represents a target class and its value represents the probability of assignment. Note that in the case of monolabel disagreement classification, the sum for each element must be 1, while for multilabel classification, it is not necessary.
+The disagreement classification format allows assigning a probability distribution to each class for every element in the dataset. Instead of selecting a single absolute category for each item, the label distribution by annotator is assigned to each element. In this format, as shown in the example below, PyEvALL uses the same structure, except that, in this case, the "value" attribute is represented with a dictionary where each element represents a target class and its value represents the probability of assignment. Note that in the case of mono-label disagreement classification, the sum for each element must be 1, while for multi-label classification, it is not necessary.
 
 ```python
 [
 	  {  
 	    "test_case":"1",
 	    "id":"I1",
 	    "value":{
@@ -530,8 +547,8 @@
 	    "test_case":"GOLD1",
 	    "id":"B",
 	    "value":2
 	  }  
 ]
 ```
 
-As seen in the example, this shows the predictions of a ranking system indicating that the item with identifier "A" is assigned position 1 in the ranking, while the item with identifier "B" is assigned position 2 in the ranking.
+As seen in the example, this shows the predictions of a ranking system indicating that the item with identifier "A" is assigned the position 1 in the ranking, while the item with identifier "B" is assigned the position 2 in the ranking.
```

### Comparing `PyEvALL-0.1.60/pyevall/comparators/comparators.py` & `PyEvALL-0.1.62/pyevall/comparators/comparators.py`

 * *Files 6% similar despite different names*

```diff
@@ -282,30 +282,17 @@
         if self.proporties[Comparator.COMPARATOR_PROPERTY_RANKING]:
             self.pred_df_sorted= self.pred_df.sort_values(PyEvALLFormat.VALUE)
 
 
     def preprocess_df_format_ranking(self):         
         #Si el gold tiene diferentes tipos de datos en value es un error          
         lst_g_type=self.gold_df[PyEvALLFormat.VALUE].apply(type).unique()
-                   
         if not (lst_g_type[0]==type(1)):
-            try:
-                self.gold_df[PyEvALLFormat.VALUE] = pd.to_numeric(self.gold_df[PyEvALLFormat.VALUE])
-            except ValueError as e:
-                self.proporties[Comparator.COMPARATOR_PROPERTY_RANKING]= False
-                return 
-            
-        lst_p_type=self.pred_df[PyEvALLFormat.VALUE].apply(type).unique()
-                   
-        if not (lst_p_type[0]==type(1)):
-            try:
-                self.pred_df[PyEvALLFormat.VALUE] = pd.to_numeric(self.pred_df[PyEvALLFormat.VALUE])
-            except ValueError as e:
-                self.proporties[Comparator.COMPARATOR_PROPERTY_RANKING]= False
-                return 
+            self.proporties[Comparator.COMPARATOR_PROPERTY_RANKING]= False
+            return 
         
     
     def get_first_k_relevant_items_in_pred(self, param_k):
         relevants=0
         k= min(param_k, len(self.pred_df_sorted))
         for i in range(0,k):
             id = self.pred_df_sorted.iloc[i, 1]
```

### Comparing `PyEvALL-0.1.60/pyevall/comparators/formats.py` & `PyEvALL-0.1.62/pyevall/comparators/formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -365,34 +365,46 @@
         arr = [] 
         file = open(path_input_file, 'r') 
         a = file.readline() 
           
         # The first line consist of headings of the record  
         # so we will store it in an array and move to  
         # next line in input_file. 
+        df_data=None
         
-        titles = [t.strip() for t in a.split('\t')] 
+        #We read with pandas to preserver the format
+        titles = [t.strip() for t in a.split(self.delimiter)] 
         if not self.check_headers(titles):
             titles[0]=PyEvALLFormat.TEST_CASE
             titles[1]=PyEvALLFormat.ID
-            titles[2]=PyEvALLFormat.VALUE            
-            
-        for line in file: 
-            d = {} 
-            for t, f in zip(titles, line.split('\t')):                 
-                # Convert each row into dictionary with keys as titles 
-                d[t] = f.strip()                   
-            # we will use strip to remove '\n'. 
-            arr.append(d) 
-              
-            # we will append all the individual dictionaires into list  
-            # and dump into file. 
+            titles[2]=PyEvALLFormat.VALUE       
+            df_data = pd.read_csv(path_input_file, sep=self.delimiter, index_col=False, header=None,
+                          skip_blank_lines=False, names=titles, dtype={
+                            PyEvALLFormat.TEST_CASE: 'str',
+                            PyEvALLFormat.ID: 'str',
+                            PyEvALLFormat.VALUE: 'str'
+                        })   
+        else:
+            df_data = pd.read_csv(path_input_file, sep=self.delimiter, index_col=False,
+                          skip_blank_lines=False, dtype={
+                            PyEvALLFormat.TEST_CASE: 'str',
+                            PyEvALLFormat.ID: 'str',
+                            PyEvALLFormat.VALUE: 'str'
+                        })                                
+        
+        #if all the value columns are numbers convert to ranking format, otherwise mataint str
+        try:
+            df_data[PyEvALLFormat.VALUE] = pd.to_numeric(df_data[PyEvALLFormat.VALUE])
+        except ValueError as e:
+            df_data[PyEvALLFormat.VALUE]=df_data[PyEvALLFormat.VALUE].astype("str")
+
+        
         output_file_json= self.get_temp_file(input_file_name)   
         with open(output_file_json, 'w', encoding='utf-8') as output_file: 
-            output_file.write(json.dumps(arr, indent=4)) 
+            output_file.write(df_data.to_json(orient="records"))            
         
         return output_file_json
 
     
     def get_temp_file(self, file_name):
         return os.path.join(PyEvALLUtils.get_tmp_dir_execution(), file_name)
```

### Comparing `PyEvALL-0.1.60/pyevall/evaluation.py` & `PyEvALL-0.1.62/pyevall/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.60/pyevall/metrics/metricfactory.py` & `PyEvALL-0.1.62/pyevall/metrics/metricfactory.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.60/pyevall/metrics/metrics.py` & `PyEvALL-0.1.62/pyevall/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.60/pyevall/reports/reports.py` & `PyEvALL-0.1.62/pyevall/reports/reports.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.60/pyevall/utils/pyevall_keys_texts_reports.rep` & `PyEvALL-0.1.62/pyevall/utils/pyevall_keys_texts_reports.rep`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.60/pyevall/utils/utils.py` & `PyEvALL-0.1.62/pyevall/utils/utils.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.60/setup.py` & `PyEvALL-0.1.62/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PyEvALL',
-    version='0.1.60',
+    version='0.1.62',
     description='PyEvALL (The Python library to Evaluate ALL) is a evaluation tool for information systems that allows assessing a wide range of metrics covering various evaluation contexts, including classification, ranking, or LeWiDi (Learning with disagreement).',
     author='JORGE CARRILLO-DE-ALBORNOZ',
     author_email='jcalbornoz@lsi.uned.es',
     url="https://github.com/UNEDLENAR/PyEvALL/tree/main",
     include_package_data=True,
     packages=['pyevall','pyevall.metrics','pyevall.utils',
               'pyevall.comparators','pyevall.reports'],
```

### Comparing `PyEvALL-0.1.60/test/testformats.py` & `PyEvALL-0.1.62/test/testformats.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.60/test/testmetrics.py` & `PyEvALL-0.1.62/test/testmetrics.py`

 * *Files identical despite different names*

