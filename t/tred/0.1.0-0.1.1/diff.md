# Comparing `tmp/tred-0.1.0.tar.gz` & `tmp/tred-0.1.1.tar.gz`

## Comparing `tred-0.1.0.tar` & `tred-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tred-0.1.0/requirements.txt
--rw-r--r--   0        0        0    19615 2020-02-02 00:00:00.000000 tred-0.1.0/examples/basic.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tred-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 tred-0.1.0/tests/test_m_transforms.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 tred-0.1.0/tests/test_tensor_ops.py
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 tred-0.1.0/tests/test_tensor_pca.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tred-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tred-0.1.0/tred/__init__.py
--rw-r--r--   0        0        0     8117 2020-02-02 00:00:00.000000 tred-0.1.0/tred/_m_transforms.py
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 tred-0.1.0/tred/_tensor_ops.py
--rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 tred-0.1.0/tred/_tensor_pca.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 tred-0.1.0/tred/_utils.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 tred-0.1.0/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tred-0.1.0/LICENSE
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tred-0.1.0/README.txt
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tred-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tred-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tred-0.1.1/requirements.txt
+-rw-r--r--   0        0        0    18447 2020-02-02 00:00:00.000000 tred-0.1.1/examples/basic.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tred-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 tred-0.1.1/tests/test_m_transforms.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 tred-0.1.1/tests/test_tensor_ops.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 tred-0.1.1/tests/test_tensor_pca.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tred-0.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tred-0.1.1/tred/__init__.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 tred-0.1.1/tred/_m_transforms.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 tred-0.1.1/tred/_tensor_ops.py
+-rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 tred-0.1.1/tred/_tensor_pca.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tred-0.1.1/tred/_utils.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 tred-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tred-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tred-0.1.1/README.txt
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tred-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tred-0.1.1/PKG-INFO
```

### Comparing `tred-0.1.0/examples/basic.ipynb` & `tred-0.1.1/examples/basic.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835460184103275%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1}, 3: {'execution_count': 2}, 5: {'execution_count': 3, "*

 * *            "'outputs': {0: {'text': {insert: [(0, 'Tensor with shape (3, 4, 2)\\n'), (1, "*

 * *            "'[[[0.9767   0.923246 0.319097 0.241766]\\n'), (2, '  [0.964079 0.441006 0.863621 "*

 * *            "0.674881]\\n'), (3, '  [0.735758 0.172066 0.060139 0.671238]]\\n'), (5, ' [[0.380196 "*

 * *            "0.261692 0.118091 0.318534]\\n'), (6, '  [0.26365  0.609871 0.863758 0.659874]\\n'), "*

 * *            "(7, '  [0.2227 […]*

```diff
@@ -12,24 +12,14 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "%load_ext autoreload\n",
-                "%autoreload 2"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 2,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "import numpy as np\n",
                 "from numpy.testing import assert_allclose\n",
                 "\n",
                 "import tred\n",
                 "from tred import display_tensor_facewise as disp"
             ]
         },
@@ -38,15 +28,15 @@
             "metadata": {},
             "source": [
                 "First we will create some dummy data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# let's use a numpy rng\n",
                 "RNG = np.random.default_rng(seed=1234)\n",
                 "\n",
                 "# then we will generate some dummy data\n",
@@ -59,29 +49,29 @@
             "metadata": {},
             "source": [
                 "Let's quickly view our data using the `display_tensor_facewise` function, which we imported as `disp`. Note: this looks a bit nicer than calling `print(X)`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Tensor with dimensions (3, 4, 2)\n",
-                        "[[[0.97669977 0.92324623 0.31909706 0.24176629]\n",
-                        "  [0.96407925 0.44100612 0.8636213  0.67488131]\n",
-                        "  [0.7357577  0.17206618 0.06013866 0.67123802]]\n",
+                        "Tensor with shape (3, 4, 2)\n",
+                        "[[[0.9767   0.923246 0.319097 0.241766]\n",
+                        "  [0.964079 0.441006 0.863621 0.674881]\n",
+                        "  [0.735758 0.172066 0.060139 0.671238]]\n",
                         "\n",
-                        " [[0.38019574 0.26169242 0.11809123 0.31853393]\n",
-                        "  [0.2636498  0.60987081 0.86375767 0.65987435]\n",
-                        "  [0.22275366 0.87041497 0.68368891 0.61101798]]]\n"
+                        " [[0.380196 0.261692 0.118091 0.318534]\n",
+                        "  [0.26365  0.609871 0.863758 0.659874]\n",
+                        "  [0.222754 0.870415 0.683689 0.611018]]]\n"
                     ]
                 }
             ],
             "source": [
                 "disp(X)"
             ]
         },
@@ -91,127 +81,127 @@
             "source": [
                 "## tsvdm tensor decomposition algorithm\n",
                 "Let's get the tsvdm decomposition first, using the `tsvdm` function"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# so, first we can use tred's tsvdm decomposition\n",
                 "# NOTE: we return V not Vt\n",
                 "U, S, V = tred.tsvdm(X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Tensor with dimensions (3, 3, 2)\n",
-                        "[[[ 0.17155477 -0.03254445 -0.56750142]\n",
-                        "  [ 0.77376295 -0.77505461  0.24995519]\n",
-                        "  [ 1.00613179  0.03661673  0.27647539]]\n",
+                        "Tensor with shape (3, 3, 2)\n",
+                        "[[[ 0.171555 -0.032544 -0.567501]\n",
+                        "  [ 0.773763 -0.775055  0.249955]\n",
+                        "  [ 1.006132  0.036617  0.276475]]\n",
                         "\n",
-                        " [[ 0.49697207  1.1805333   0.08253392]\n",
-                        "  [ 0.21963571 -0.04814225 -0.82918402]\n",
-                        "  [-0.25364858  0.03023034  0.91905817]]]\n"
+                        " [[ 0.496972  1.180533  0.082534]\n",
+                        "  [ 0.219636 -0.048142 -0.829184]\n",
+                        "  [-0.253649  0.03023   0.919058]]]\n"
                     ]
                 }
             ],
             "source": [
                 "disp(U)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Tensor with dimensions (3, 4, 2)\n",
-                        "[[[ 2.49071429  0.          0.          0.        ]\n",
-                        "  [ 0.          0.95133804  0.          0.        ]\n",
-                        "  [ 0.          0.          0.33545775  0.        ]]\n",
+                        "Tensor with shape (3, 4, 2)\n",
+                        "[[[ 2.490714  0.        0.        0.      ]\n",
+                        "  [ 0.        0.951338  0.        0.      ]\n",
+                        "  [ 0.        0.        0.335458  0.      ]]\n",
                         "\n",
-                        " [[ 1.2959226   0.          0.          0.        ]\n",
-                        "  [ 0.         -0.06058465  0.          0.        ]\n",
-                        "  [ 0.          0.          0.10984777  0.        ]]]\n"
+                        " [[ 1.295923  0.        0.        0.      ]\n",
+                        "  [ 0.       -0.060585  0.        0.      ]\n",
+                        "  [ 0.        0.        0.109848  0.      ]]]\n"
                     ]
                 }
             ],
             "source": [
                 "disp(S)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Tensor with dimensions (4, 4, 2)\n",
-                        "[[[ 0.72770621 -0.26446627 -0.16542903 -0.41692012]\n",
-                        "  [-0.15139073 -0.0209886  -0.29168408  0.60752868]\n",
-                        "  [-0.01705587 -0.61095445  0.23509181  0.09922585]\n",
-                        "  [ 0.39762985 -0.16678187  0.60880143  0.52113841]]\n",
+                        "Tensor with shape (4, 4, 2)\n",
+                        "[[[ 0.727706 -0.264466 -0.165429 -0.41692 ]\n",
+                        "  [-0.151391 -0.020989 -0.291684  0.607529]\n",
+                        "  [-0.017056 -0.610954  0.235092  0.099226]\n",
+                        "  [ 0.39763  -0.166782  0.608801  0.521138]]\n",
                         "\n",
-                        " [[ 0.0244148   0.95052807 -0.33592066 -0.4270477 ]\n",
-                        "  [ 0.84344351  0.65517601  0.43308422  0.44074385]\n",
-                        "  [ 0.69522119 -0.36615433 -0.96110795  0.14212615]\n",
-                        "  [ 0.30626555 -0.2484096   0.48735324 -0.8825139 ]]]\n"
+                        " [[ 0.024415  0.950528 -0.335921 -0.427048]\n",
+                        "  [ 0.843444  0.655176  0.433084  0.440744]\n",
+                        "  [ 0.695221 -0.366154 -0.961108  0.142126]\n",
+                        "  [ 0.306266 -0.24841   0.487353 -0.882514]]]\n"
                     ]
                 }
             ],
             "source": [
                 "disp(V)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# NOTE: the V tensor is not transposed (facewise)!\n",
                 "# in order to do a facewise transpose - use numpy\n",
                 "Vt = V.transpose(1, 0, 2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Tensor with dimensions (4, 4, 2)\n",
-                        "[[[ 0.72770621 -0.15139073 -0.01705587  0.39762985]\n",
-                        "  [-0.26446627 -0.0209886  -0.61095445 -0.16678187]\n",
-                        "  [-0.16542903 -0.29168408  0.23509181  0.60880143]\n",
-                        "  [-0.41692012  0.60752868  0.09922585  0.52113841]]\n",
+                        "Tensor with shape (4, 4, 2)\n",
+                        "[[[ 0.727706 -0.151391 -0.017056  0.39763 ]\n",
+                        "  [-0.264466 -0.020989 -0.610954 -0.166782]\n",
+                        "  [-0.165429 -0.291684  0.235092  0.608801]\n",
+                        "  [-0.41692   0.607529  0.099226  0.521138]]\n",
                         "\n",
-                        " [[ 0.0244148   0.84344351  0.69522119  0.30626555]\n",
-                        "  [ 0.95052807  0.65517601 -0.36615433 -0.2484096 ]\n",
-                        "  [-0.33592066  0.43308422 -0.96110795  0.48735324]\n",
-                        "  [-0.4270477   0.44074385  0.14212615 -0.8825139 ]]]\n"
+                        " [[ 0.024415  0.843444  0.695221  0.306266]\n",
+                        "  [ 0.950528  0.655176 -0.366154 -0.24841 ]\n",
+                        "  [-0.335921  0.433084 -0.961108  0.487353]\n",
+                        "  [-0.427048  0.440744  0.142126 -0.882514]]]\n"
                     ]
                 }
             ],
             "source": [
                 "disp(Vt)"
             ]
         },
@@ -221,15 +211,15 @@
             "source": [
                 "Let's also verify that we can use the tsvdm decomposition to reconstruct the \n",
                 "original tensor `X`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# see documentation - allows us to apply a function over a sequence of inputs \n",
                 "# cumulatively from left to right\n",
                 "from functools import reduce\n",
                 "\n",
@@ -257,24 +247,24 @@
                 "Notice how the last column of `S` is all zeroes. This means that some of the\n",
                 "`V` tensor is redundant. We can pass in `full_frontal_slices=False` to only\n",
                 "return us the necessary elements in the tensor."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "((3, 3, 2), (3, 3, 2), (4, 3, 2))"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "U2, S2, V2 = tred.tsvdm(X, full_frontal_slices=False)\n",
                 "\n",
@@ -287,15 +277,15 @@
             "source": [
                 "Sense check that we have not 'loss' any information, and we can still \n",
                 "fully reconstruct our original tensor"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "V2t = V2.transpose(1, 0, 2)\n",
                 "X_reconstructed2 = reduce(m_product_wrapper, (U2, S2, V2t))\n",
                 "assert_allclose(X_reconstructed2, X)"
             ]
@@ -306,15 +296,15 @@
             "source": [
                 "## TPCA unsupervised tensor dimensionality reduction algorithm\n",
                 "Now, let's use the tensor decomposition using the `tpca` object. Revise some basics of object oriented programming and scikit-learn's interface if you are coming from R."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# first, create a transformer object\n",
                 "tpca = tred.TPCA()"
             ]
         },
@@ -326,76 +316,83 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "1. You explicitly fit your tpca object _first_, and then transform your data.\n",
+                "\n",
                 "Let's see what happens if you call `transform` _before_ `fit`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "NotFittedError",
                     "evalue": "This TPCA instance is not fitted yet. Call 'fit' with appropriate arguments before using this estimator.",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[1;31mNotFittedError\u001b[0m                            Traceback (most recent call last)",
-                        "Cell \u001b[1;32mIn[15], line 2\u001b[0m\n\u001b[0;32m      1\u001b[0m \u001b[38;5;66;03m# ERROR\u001b[39;00m\n\u001b[1;32m----> 2\u001b[0m X_transformed_1 \u001b[38;5;241m=\u001b[39m \u001b[43mtpca\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mtransform\u001b[49m\u001b[43m(\u001b[49m\u001b[43mX\u001b[49m\u001b[43m)\u001b[49m\n",
+                        "Cell \u001b[1;32mIn[14], line 2\u001b[0m\n\u001b[0;32m      1\u001b[0m \u001b[38;5;66;03m# ERROR\u001b[39;00m\n\u001b[1;32m----> 2\u001b[0m X_transformed_1 \u001b[38;5;241m=\u001b[39m \u001b[43mtpca\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mtransform\u001b[49m\u001b[43m(\u001b[49m\u001b[43mX\u001b[49m\u001b[43m)\u001b[49m\n",
                         "File \u001b[1;32mc:\\Users\\brend\\OneDrive\\Documents\\GITHUB STUFF\\tred\\.venv\\lib\\site-packages\\sklearn\\utils\\_set_output.py:157\u001b[0m, in \u001b[0;36m_wrap_method_output.<locals>.wrapped\u001b[1;34m(self, X, *args, **kwargs)\u001b[0m\n\u001b[0;32m    155\u001b[0m \u001b[38;5;129m@wraps\u001b[39m(f)\n\u001b[0;32m    156\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mwrapped\u001b[39m(\u001b[38;5;28mself\u001b[39m, X, \u001b[38;5;241m*\u001b[39margs, \u001b[38;5;241m*\u001b[39m\u001b[38;5;241m*\u001b[39mkwargs):\n\u001b[1;32m--> 157\u001b[0m     data_to_wrap \u001b[38;5;241m=\u001b[39m f(\u001b[38;5;28mself\u001b[39m, X, \u001b[38;5;241m*\u001b[39margs, \u001b[38;5;241m*\u001b[39m\u001b[38;5;241m*\u001b[39mkwargs)\n\u001b[0;32m    158\u001b[0m     \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(data_to_wrap, \u001b[38;5;28mtuple\u001b[39m):\n\u001b[0;32m    159\u001b[0m         \u001b[38;5;66;03m# only wrap the first output for cross decomposition\u001b[39;00m\n\u001b[0;32m    160\u001b[0m         return_tuple \u001b[38;5;241m=\u001b[39m (\n\u001b[0;32m    161\u001b[0m             _wrap_data_with_container(method, data_to_wrap[\u001b[38;5;241m0\u001b[39m], X, \u001b[38;5;28mself\u001b[39m),\n\u001b[0;32m    162\u001b[0m             \u001b[38;5;241m*\u001b[39mdata_to_wrap[\u001b[38;5;241m1\u001b[39m:],\n\u001b[0;32m    163\u001b[0m         )\n",
                         "File \u001b[1;32m~\\OneDrive\\Documents\\GITHUB STUFF\\tred\\tred\\_tensor_pca.py:318\u001b[0m, in \u001b[0;36mTPCA.transform\u001b[1;34m(self, X)\u001b[0m\n\u001b[0;32m    298\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mtransform\u001b[39m(\u001b[38;5;28mself\u001b[39m, X):\n\u001b[0;32m    299\u001b[0m \u001b[38;5;250m    \u001b[39m\u001b[38;5;124;03m\"\"\"Apply dimensionality reduction to X.\u001b[39;00m\n\u001b[0;32m    300\u001b[0m \n\u001b[0;32m    301\u001b[0m \u001b[38;5;124;03m    See the TCAM algorithm from Mor et al. (2022)\u001b[39;00m\n\u001b[1;32m   (...)\u001b[0m\n\u001b[0;32m    315\u001b[0m \u001b[38;5;124;03m        TCAM projections in 2D transformed space.\u001b[39;00m\n\u001b[0;32m    316\u001b[0m \u001b[38;5;124;03m    \"\"\"\u001b[39;00m\n\u001b[1;32m--> 318\u001b[0m     \u001b[43mcheck_is_fitted\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;28;43mself\u001b[39;49m\u001b[43m)\u001b[49m\n\u001b[0;32m    319\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28mlen\u001b[39m(X\u001b[38;5;241m.\u001b[39mshape) \u001b[38;5;241m==\u001b[39m \u001b[38;5;241m3\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mEnsure order-3 tensor input\u001b[39m\u001b[38;5;124m\"\u001b[39m\n\u001b[0;32m    320\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m (\n\u001b[0;32m    321\u001b[0m         X\u001b[38;5;241m.\u001b[39mshape[\u001b[38;5;241m1\u001b[39m] \u001b[38;5;241m==\u001b[39m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mp_ \u001b[38;5;129;01mand\u001b[39;00m X\u001b[38;5;241m.\u001b[39mshape[\u001b[38;5;241m2\u001b[39m] \u001b[38;5;241m==\u001b[39m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mt_\n\u001b[0;32m    322\u001b[0m     ), \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mEnsure the number of features, and time points, matches the model fit data\u001b[39m\u001b[38;5;124m\"\u001b[39m\n",
                         "File \u001b[1;32mc:\\Users\\brend\\OneDrive\\Documents\\GITHUB STUFF\\tred\\.venv\\lib\\site-packages\\sklearn\\utils\\validation.py:1461\u001b[0m, in \u001b[0;36mcheck_is_fitted\u001b[1;34m(estimator, attributes, msg, all_or_any)\u001b[0m\n\u001b[0;32m   1458\u001b[0m     \u001b[38;5;28;01mraise\u001b[39;00m \u001b[38;5;167;01mTypeError\u001b[39;00m(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;132;01m%s\u001b[39;00m\u001b[38;5;124m is not an estimator instance.\u001b[39m\u001b[38;5;124m\"\u001b[39m \u001b[38;5;241m%\u001b[39m (estimator))\n\u001b[0;32m   1460\u001b[0m \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;129;01mnot\u001b[39;00m _is_fitted(estimator, attributes, all_or_any):\n\u001b[1;32m-> 1461\u001b[0m     \u001b[38;5;28;01mraise\u001b[39;00m NotFittedError(msg \u001b[38;5;241m%\u001b[39m {\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mname\u001b[39m\u001b[38;5;124m\"\u001b[39m: \u001b[38;5;28mtype\u001b[39m(estimator)\u001b[38;5;241m.\u001b[39m\u001b[38;5;18m__name__\u001b[39m})\n",
                         "\u001b[1;31mNotFittedError\u001b[0m: This TPCA instance is not fitted yet. Call 'fit' with appropriate arguments before using this estimator."
                     ]
                 }
             ],
             "source": [
                 "# ERROR\n",
                 "X_transformed_1 = tpca.transform(X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# so, we need to fit the tpca object first - then call transform!\n",
                 "tpca.fit(X)\n",
                 "X_transformed_1 = tpca.transform(X)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Bit of a late update - but `disp` (named `display_tensor_facewise`) actually \n",
+                "works for matrix and vector inputs too. It just does a bit of rounding and \n",
+                "prints the size of the input. We have left the unfortunate original name as is, \n",
+                "to avoid breaking existing workflows. "
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "array([[ 5.68460112e-01,  5.11808598e-01, -1.54348130e-01,\n",
-                            "        -6.89881787e-02,  1.42247325e-16, -2.77555756e-17],\n",
-                            "       [-6.66509430e-03, -5.59723785e-01, -1.17834904e-01,\n",
-                            "         1.40461250e-01, -1.70870262e-16, -2.77555756e-17],\n",
-                            "       [-5.61795018e-01,  4.79151878e-02,  2.72183034e-01,\n",
-                            "        -7.14730711e-02,  1.73472348e-17,  1.80411242e-16]])"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Matrix with shape (3, 6)\n",
+                        "[[ 0.56846  0.51181 -0.15435 -0.06899  0.      -0.     ]\n",
+                        " [-0.00667 -0.55972 -0.11783  0.14046 -0.      -0.     ]\n",
+                        " [-0.5618   0.04792  0.27218 -0.07147  0.       0.     ]]\n"
+                    ]
                 }
             ],
             "source": [
                 "# the size of this is n rows by min(n, p) columns\n",
-                "X_transformed_1"
+                "disp(X_transformed_1)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "2. Use `fit_transform`\n",
@@ -404,52 +401,47 @@
                 "use a slightly more efficient computation to obtain the transformed data. \n",
                 "\n",
                 "See the `tred` library implementation for more details"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [],
             "source": [
                 "X_transformed_2 = tpca.fit_transform(X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "array([[ 5.68460112e-01,  5.11808598e-01, -1.54348130e-01,\n",
-                            "        -6.89881787e-02, -6.00850325e-17,  5.86791256e-17],\n",
-                            "       [-6.66509430e-03, -5.59723785e-01, -1.17834904e-01,\n",
-                            "         1.40461250e-01, -6.00850325e-17,  5.86791256e-17],\n",
-                            "       [-5.61795018e-01,  4.79151878e-02,  2.72183034e-01,\n",
-                            "        -7.14730711e-02, -6.00850325e-17,  5.86791256e-17]])"
-                        ]
-                    },
-                    "execution_count": 30,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Matrix with shape (3, 6)\n",
+                        "[[ 0.56846  0.51181 -0.15435 -0.06899 -0.       0.     ]\n",
+                        " [-0.00667 -0.55972 -0.11783  0.14046 -0.       0.     ]\n",
+                        " [-0.5618   0.04792  0.27218 -0.07147 -0.       0.     ]]\n"
+                    ]
                 }
             ],
             "source": [
                 "# NOTE: this is the same as the array above - to machine precision\n",
-                "# some numbers LOOK different, but you'll see that they are tiny and\n",
+                "# some numbers might LOOK different, but you'll see that they are tiny and\n",
                 "# are effectively the same\n",
-                "X_transformed_2"
+                "disp(X_transformed_2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# the tensor operations produce some floating point errors\n",
                 "# below are the tolerances we use in tred's testing module, which show that the two\n",
                 "# transformations of X are indeed the same\n",
                 "RTOL = 1e-7\n",
@@ -462,61 +454,58 @@
             "metadata": {},
             "source": [
                 "We can use the fitted objects to transform out of bag data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# imagine one new observation, with p features, across t time points\n",
                 "new_obs = RNG.random(size=(1, p, t))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Tensor with dimensions (1, 4, 2)\n",
-                        "[[[0.06013731 0.43895163 0.00313229 0.85849044]]\n",
+                        "Tensor with shape (1, 4, 2)\n",
+                        "[[[0.060137 0.438952 0.003132 0.85849 ]]\n",
                         "\n",
-                        " [[0.97776927 0.53259502 0.25126711 0.42529835]]]\n"
+                        " [[0.977769 0.532595 0.251267 0.425298]]]\n"
                     ]
                 }
             ],
             "source": [
                 "disp(new_obs)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "array([[-0.13546024,  0.34661962,  0.39718925, -0.55304217,  0.95086191,\n",
-                            "         0.07885213]])"
-                        ]
-                    },
-                    "execution_count": 34,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Matrix with shape (1, 6)\n",
+                        "[[-0.13546  0.34662  0.39719 -0.55304  0.95086  0.07885]]\n"
+                    ]
                 }
             ],
             "source": [
-                "tpca.transform(new_obs)"
+                "disp(tpca.transform(new_obs))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Make sure you do not call `fit` or `fit_transform` on the new data, otherwise \n",
```

### Comparing `tred-0.1.0/tests/test_m_transforms.py` & `tred-0.1.1/tests/test_m_transforms.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/tests/test_tensor_ops.py` & `tred-0.1.1/tests/test_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/tests/test_tensor_pca.py` & `tred-0.1.1/tests/test_tensor_pca.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/tests/test_utils.py` & `tred-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/tred/__init__.py` & `tred-0.1.1/tred/__init__.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/tred/_m_transforms.py` & `tred-0.1.1/tred/_m_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 import sys
 
 import numpy.linalg as linalg
 from scipy.fft import dct, idct, dst, idst
 
 
 # the transform generator functions below all work for:
-#   1. order 3 tensors: by applying the transform along the tubal fibres
-#   2. matrices: by applying the transform along the rows
+#   1. 3D array (tensor): by applying the transform along the tubal fibres
+#   2. 2D array (matrices): by applying the transform along the rows
+#   3. 1D array (vector): by applying the transform on the vector
 # i.e., along the -1 axis of order-2 and order-3 arrays
 #
 # we do not need extensive parameter validation however, as the M and Minv Callables
 # returned by the generator functions are meant to be passed into classes and functions
 # in the tred package - which do some of their own parameter validation
-SUPPORTED_TRANSFORM_ORDERS = (1, 2, 3)
+SUPPORTED_TRANSFORM_DIMENSIONS = (1, 2, 3)
 
 
 def _assert_t_and_order(X_input, t_expected):
     assert (
-        len(X_input.shape) in SUPPORTED_TRANSFORM_ORDERS
-    ), "Expecting matrix or order-3 tensor input"
+        len(X_input.shape) in SUPPORTED_TRANSFORM_DIMENSIONS
+    ), "Expecting 1D (vector), 2D (matrix) or 3D (tensor) input"
     assert (
         X_input.shape[-1] == t_expected
     ), f"Expecting last input dimension to be {t_expected}"
 
 
 def generate_transform_pair_from_matrix(M_mat, Minv_mat=None, *, inplace=False):
     """Generate a pair of functions to apply a matrix, and its inverse, to the tubal
```

### Comparing `tred-0.1.0/tred/_tensor_ops.py` & `tred-0.1.1/tred/_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/tred/_tensor_pca.py` & `tred-0.1.1/tred/_tensor_pca.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/tred/_utils.py` & `tred-0.1.1/tred/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 RealNotInt.register(float)
 
 
 def display_tensor_facewise(tens):
     """By default Numpy prints order-3 arrays as vertical stacks of order-2 arrays, in
     line with their broadcasting rules. This function prints a transpose view so the
     print output is a more intuitive sequence of frontal slices. We often use this in
-    notebooks.
+    notebooks. It also prints the rounded values.
+
+    UPDATE: Also works for matrices and vectors now.
 
     Parameters
     ----------
         tens : ArrayLike of shape (n, p, t)
             Order-3 tensor representation
 
     Examples
@@ -48,17 +50,29 @@
     [1.]]]
     >>> disp(test)
     Tensor with dimensions (3, 3, 1)
     [[[1. 0. 0.]
     [0. 1. 0.]
     [0. 0. 1.]]]
     """
-    assert len(tens.shape) == 3, "expecting tensor (order-3) array input!"
-    print(f"Tensor with dimensions {tens.shape}")
-    print(tens.transpose(2, 0, 1))
+    assert len(tens.shape) in (
+        1,  # vector
+        2,  # matrix
+        3,  # tensor
+    ), "Expecting 1D (vector), 2D (matrix) or 3D (tensor) input"
+
+    if len(tens.shape) == 3:
+        print(f"Tensor with shape {tens.shape}")
+        print(tens.transpose(2, 0, 1).round(6))
+    else:
+        if len(tens.shape) == 2:
+            print(f"Matrix with shape {tens.shape}")
+        else:
+            print(f"Vector with length {tens.shape}")
+        print(tens.round(5))
 
 
 def _singular_vals_mat_to_tensor(mat, n, p, t):
     """Decompress $k \times t$ matrix of singular values into $\hat{S}$ from literature.
 
     NOTE: There's probably a cool numpy way to do this without the for loop...but for now
     it works fine as $t$ is usually modest for the data we work with
```

### Comparing `tred-0.1.0/.gitignore` & `tred-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/LICENSE` & `tred-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/README.txt` & `tred-0.1.1/README.txt`

 * *Files identical despite different names*

### Comparing `tred-0.1.0/pyproject.toml` & `tred-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tred"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Brendan Lu", email="brendannlu5@gmail.com" },
 ]
 description = "Dimensionality reduction techniques for order-3 tensors"
 readme = "README.txt"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tred-0.1.0/PKG-INFO` & `tred-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tred
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dimensionality reduction techniques for order-3 tensors
 Project-URL: Homepage, https://github.com/brendanlu/tred
 Project-URL: Issues, https://github.com/brendanlu/tred/issues
 Author-email: Brendan Lu <brendannlu5@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

