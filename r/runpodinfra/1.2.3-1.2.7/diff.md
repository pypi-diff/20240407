# Comparing `tmp/runpodinfra-1.2.3.tar.gz` & `tmp/runpodinfra-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpodinfra-1.2.3.tar", last modified: Thu Apr  4 01:09:35 2024, max compression
+gzip compressed data, was "runpodinfra-1.2.7.tar", last modified: Sun Apr  7 01:24:08 2024, max compression
```

## Comparing `runpodinfra-1.2.3.tar` & `runpodinfra-1.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:35.853284 runpodinfra-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-04 01:09:35.853284 runpodinfra-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:35.849284 runpodinfra-1.2.3/runpodinfra/
--rw-------   0 runner    (1001) docker     (127)      921 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1918 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9279 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:35.853284 runpodinfra-1.2.3/runpodinfra/config/
--rw-------   0 runner    (1001) docker     (127)      267 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      564 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/config/vars.py
--rw-------   0 runner    (1001) docker     (127)     6351 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/network_storage.py
--rw-------   0 runner    (1001) docker     (127)    18526 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/outputs.py
--rw-------   0 runner    (1001) docker     (127)    31793 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/pod.py
--rw-------   0 runner    (1001) docker     (127)     3631 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/provider.py
--rw-------   0 runner    (1001) docker     (127)      110 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:35.853284 runpodinfra-1.2.3/runpodinfra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/runpodinfra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:09:35.853284 runpodinfra-1.2.3/setup.cfg
--rw-------   0 runner    (1001) docker     (127)     1307 2024-04-04 01:09:35.000000 runpodinfra-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:24:08.650161 runpodinfra-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-07 01:24:08.650161 runpodinfra-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:24:08.646161 runpodinfra-1.2.7/runpodinfra/
+-rw-------   0 runner    (1001) docker     (127)      921 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1918 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9279 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:24:08.646161 runpodinfra-1.2.7/runpodinfra/config/
+-rw-------   0 runner    (1001) docker     (127)      267 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      564 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/config/vars.py
+-rw-------   0 runner    (1001) docker     (127)     6351 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/network_storage.py
+-rw-------   0 runner    (1001) docker     (127)    18526 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    31793 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/pod.py
+-rw-------   0 runner    (1001) docker     (127)     3631 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/provider.py
+-rw-------   0 runner    (1001) docker     (127)      110 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:24:08.646161 runpodinfra-1.2.7/runpodinfra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/runpodinfra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 01:24:08.650161 runpodinfra-1.2.7/setup.cfg
+-rw-------   0 runner    (1001) docker     (127)     1307 2024-04-07 01:24:08.000000 runpodinfra-1.2.7/setup.py
```

### Comparing `runpodinfra-1.2.3/PKG-INFO` & `runpodinfra-1.2.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: runpodinfra
-Version: 1.2.3
-Summary: The Runpod Pulumi provider provides resources to interact with Runpod's native APIs.
-Home-page: https://runpod.io
-License: Apache-2.0
-Project-URL: Repository, https://github.com/runpod/pulumi-runpod-native
-Keywords: pulumi runpod gpus ml ai
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 ---
 title: Runpod
 meta_desc: Provides an overview of the Runpod Provider for Pulumi.
 layout: package
 ---
 
 The Runpod provider for Pulumi can be used to provision [Runpod](https://www.runpod.io) resources.
@@ -45,48 +33,63 @@
 ```
     go get github.com/runpod/pulumi-runpod-native/sdk/go/runpod@v1.1.8
 ```
 Replace the version above to any that you want. We advise you to pin a certain version as there will be fewer breaking changes.
 
 4. Use this example as a simple building guide for your example project:
 
-```typescript
-    import * as pulumi from "@pulumi/pulumi";
-    import * as runpod from "@runpod-infra/pulumi";
-
-    const testNetworkStorage = new runpod.NetworkStorage("testNetworkStorage", {
-        name: "testStorage1",
-        size: 20,
-        dataCenterId: "US-NJ",
-    });
-    const myRandomPod = new runpod.Pod("myRandomPod", {
-        cloudType: "ALL",
-        networkVolumeId: testNetworkStorage.networkStorage.apply(networkStorage => networkStorage.id),
-        gpuCount: 1,
-        volumeInGb: 50,
-        containerDiskInGb: 50,
-        minVcpuCount: 2,
-        minMemoryInGb: 15,
-        gpuTypeId: "NVIDIA GeForce RTX 3070",
-        name: "RunPod Pytorch",
-        imageName: "runpod/pytorch",
-        dockerArgs: "",
-        ports: "8888/http",
-        volumeMountPath: "/workspace",
-        env: [{
-            key: "JUPYTER_PASSWORD",
-            value: "rns1hunbsstltcpad22d",
-        }],
-    });
-    export const pod = {
-        value: myRandomPod.pod,
-    };
-    export const networkStorage = {
-        value: testNetworkStorage.networkStorage,
-    };
+```go
+package main
+
+import (
+	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
+	"github.com/runpod/pulumi-runpod-native/sdk/go/runpod"
+)
+
+func main() {
+	pulumi.Run(func(ctx *pulumi.Context) error {
+		testNetworkStorage, err := runpod.NewNetworkStorage(ctx, "testNetworkStorage", &runpod.NetworkStorageArgs{
+			Name:         pulumi.String("testStorage1"),
+			Size:         pulumi.Int(20),
+			DataCenterId: pulumi.String("US-NJ"),
+		})
+		if err != nil {
+			return err
+		}
+
+		myRandomPod, err := runpod.NewPod(ctx, "myRandomPod", &runpod.PodArgs{
+			CloudType:         pulumi.String("ALL"),
+			NetworkVolumeId:   testNetworkStorage.NetworkStorage.Id(),
+			GpuCount:          pulumi.Int(1),
+			VolumeInGb:        pulumi.Int(50),
+			ContainerDiskInGb: pulumi.Int(50),
+			MinVcpuCount:      pulumi.Int(2),
+			MinMemoryInGb:     pulumi.Int(15),
+			GpuTypeId:         pulumi.String("NVIDIA GeForce RTX 3070"),
+			Name:              pulumi.String("RunPod Pytorch"),
+			ImageName:         pulumi.String("runpod/pytorch"),
+			DockerArgs:        pulumi.String(""),
+			Ports:             pulumi.String("8888/http"),
+			VolumeMountPath:   pulumi.String("/workspace"),
+			Env: runpod.PodEnvArray{
+				&runpod.PodEnvArgs{
+					Key:   pulumi.String("JUPYTER_PASSWORD"),
+					Value: pulumi.String("rns1hunbsstltcpad22d"),
+				},
+			},
+		})
+		if err != nil {
+			return err
+		}
+
+		ctx.Export("pod", myRandomPod)
+		ctx.Export("networkStorage", testNetworkStorage)
+		return nil
+	})
+}
 ```
 
 5. PULUMI UP
 Create your resources using the command below:
 
 ```
     pulumi up
@@ -97,9 +100,8 @@
 
 ```
     pulumi down
 ```
 
 If you have any issues, please feel free to create an issue or reach out to us directly at support@runpod.io.
 
-> **Note:** For examples in Go and Python, please visit the documentation inside the docs directory or click [here](https://github.com/runpod/pulumi-runpod-native/tree/main/docs).
-
+> **Note:** For examples in TypeScript and Python, please visit the documentation inside the docs directory or click [here](https://github.com/runpod/pulumi-runpod-native/tree/main/docs).
```

### Comparing `runpodinfra-1.2.3/runpodinfra/__init__.py` & `runpodinfra-1.2.7/runpodinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `runpodinfra-1.2.3/runpodinfra/_inputs.py` & `runpodinfra-1.2.7/runpodinfra/_inputs.py`

 * *Files identical despite different names*

### Comparing `runpodinfra-1.2.3/runpodinfra/_utilities.py` & `runpodinfra-1.2.7/runpodinfra/_utilities.py`

 * *Files identical despite different names*

### Comparing `runpodinfra-1.2.3/runpodinfra/config/vars.py` & `runpodinfra-1.2.7/runpodinfra/config/vars.py`

 * *Files identical despite different names*

### Comparing `runpodinfra-1.2.3/runpodinfra/network_storage.py` & `runpodinfra-1.2.7/runpodinfra/network_storage.py`

 * *Files identical despite different names*

### Comparing `runpodinfra-1.2.3/runpodinfra/outputs.py` & `runpodinfra-1.2.7/runpodinfra/outputs.py`

 * *Files identical despite different names*

### Comparing `runpodinfra-1.2.3/runpodinfra/pod.py` & `runpodinfra-1.2.7/runpodinfra/pod.py`

 * *Files identical despite different names*

### Comparing `runpodinfra-1.2.3/runpodinfra/provider.py` & `runpodinfra-1.2.7/runpodinfra/provider.py`

 * *Files identical despite different names*

### Comparing `runpodinfra-1.2.3/runpodinfra.egg-info/PKG-INFO` & `runpodinfra-1.2.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpodinfra
-Version: 1.2.3
+Version: 1.2.7
 Summary: The Runpod Pulumi provider provides resources to interact with Runpod's native APIs.
 Home-page: https://runpod.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/runpod/pulumi-runpod-native
 Keywords: pulumi runpod gpus ml ai
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -45,48 +45,63 @@
 ```
     go get github.com/runpod/pulumi-runpod-native/sdk/go/runpod@v1.1.8
 ```
 Replace the version above to any that you want. We advise you to pin a certain version as there will be fewer breaking changes.
 
 4. Use this example as a simple building guide for your example project:
 
-```typescript
-    import * as pulumi from "@pulumi/pulumi";
-    import * as runpod from "@runpod-infra/pulumi";
-
-    const testNetworkStorage = new runpod.NetworkStorage("testNetworkStorage", {
-        name: "testStorage1",
-        size: 20,
-        dataCenterId: "US-NJ",
-    });
-    const myRandomPod = new runpod.Pod("myRandomPod", {
-        cloudType: "ALL",
-        networkVolumeId: testNetworkStorage.networkStorage.apply(networkStorage => networkStorage.id),
-        gpuCount: 1,
-        volumeInGb: 50,
-        containerDiskInGb: 50,
-        minVcpuCount: 2,
-        minMemoryInGb: 15,
-        gpuTypeId: "NVIDIA GeForce RTX 3070",
-        name: "RunPod Pytorch",
-        imageName: "runpod/pytorch",
-        dockerArgs: "",
-        ports: "8888/http",
-        volumeMountPath: "/workspace",
-        env: [{
-            key: "JUPYTER_PASSWORD",
-            value: "rns1hunbsstltcpad22d",
-        }],
-    });
-    export const pod = {
-        value: myRandomPod.pod,
-    };
-    export const networkStorage = {
-        value: testNetworkStorage.networkStorage,
-    };
+```go
+package main
+
+import (
+	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
+	"github.com/runpod/pulumi-runpod-native/sdk/go/runpod"
+)
+
+func main() {
+	pulumi.Run(func(ctx *pulumi.Context) error {
+		testNetworkStorage, err := runpod.NewNetworkStorage(ctx, "testNetworkStorage", &runpod.NetworkStorageArgs{
+			Name:         pulumi.String("testStorage1"),
+			Size:         pulumi.Int(20),
+			DataCenterId: pulumi.String("US-NJ"),
+		})
+		if err != nil {
+			return err
+		}
+
+		myRandomPod, err := runpod.NewPod(ctx, "myRandomPod", &runpod.PodArgs{
+			CloudType:         pulumi.String("ALL"),
+			NetworkVolumeId:   testNetworkStorage.NetworkStorage.Id(),
+			GpuCount:          pulumi.Int(1),
+			VolumeInGb:        pulumi.Int(50),
+			ContainerDiskInGb: pulumi.Int(50),
+			MinVcpuCount:      pulumi.Int(2),
+			MinMemoryInGb:     pulumi.Int(15),
+			GpuTypeId:         pulumi.String("NVIDIA GeForce RTX 3070"),
+			Name:              pulumi.String("RunPod Pytorch"),
+			ImageName:         pulumi.String("runpod/pytorch"),
+			DockerArgs:        pulumi.String(""),
+			Ports:             pulumi.String("8888/http"),
+			VolumeMountPath:   pulumi.String("/workspace"),
+			Env: runpod.PodEnvArray{
+				&runpod.PodEnvArgs{
+					Key:   pulumi.String("JUPYTER_PASSWORD"),
+					Value: pulumi.String("rns1hunbsstltcpad22d"),
+				},
+			},
+		})
+		if err != nil {
+			return err
+		}
+
+		ctx.Export("pod", myRandomPod)
+		ctx.Export("networkStorage", testNetworkStorage)
+		return nil
+	})
+}
 ```
 
 5. PULUMI UP
 Create your resources using the command below:
 
 ```
     pulumi up
@@ -97,9 +112,9 @@
 
 ```
     pulumi down
 ```
 
 If you have any issues, please feel free to create an issue or reach out to us directly at support@runpod.io.
 
-> **Note:** For examples in Go and Python, please visit the documentation inside the docs directory or click [here](https://github.com/runpod/pulumi-runpod-native/tree/main/docs).
+> **Note:** For examples in TypeScript and Python, please visit the documentation inside the docs directory or click [here](https://github.com/runpod/pulumi-runpod-native/tree/main/docs).
```

### Comparing `runpodinfra-1.2.3/setup.py` & `runpodinfra-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.2.3"
+VERSION = "1.2.7"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "runpod Pulumi Package - Development Version"
```

