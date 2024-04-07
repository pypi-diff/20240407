# Comparing `tmp/moby_distribution-0.7.0.tar.gz` & `tmp/moby_distribution-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moby_distribution-0.7.0.tar", max compression
+gzip compressed data, was "moby_distribution-0.7.1.tar", max compression
```

## Comparing `moby_distribution-0.7.0.tar` & `moby_distribution-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/LICENSE
--rw-r--r--   0        0        0     7006 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/README.md
--rw-r--r--   0        0        0      895 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/moby_distribution/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/moby_distribution/registry/__init__.py
--rw-r--r--   0        0        0     5910 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/moby_distribution/registry/auth.py
--rw-r--r--   0        0        0     7598 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/moby_distribution/registry/client.py
--rw-r--r--   0        0        0      917 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/exceptions.py
--rw-r--r--   0        0        0      752 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/__init__.py
--rw-r--r--   0        0        0    11137 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/blobs.py
--rw-r--r--   0        0        0    14792 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/image.py
--rw-r--r--   0        0        0     4875 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/manifests.py
--rw-r--r--   0        0        0     1033 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/tags.py
--rw-r--r--   0        0        0     3972 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/utils.py
--rw-r--r--   0        0        0        0 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/__init__.py
--rw-r--r--   0        0        0     1140 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/auth.py
--rw-r--r--   0        0        0     1070 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/base.py
--rw-r--r--   0        0        0     4204 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/endpoint.py
--rw-r--r--   0        0        0     3757 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/image_json.py
--rw-r--r--   0        0        0     4594 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/manifest.py
--rw-r--r--   0        0        0      910 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 moby_distribution-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/LICENSE
+-rw-r--r--   0        0        0     7006 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/README.md
+-rw-r--r--   0        0        0      954 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/__init__.py
+-rw-r--r--   0        0        0     5910 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/auth.py
+-rw-r--r--   0        0        0     7598 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/client.py
+-rw-r--r--   0        0        0      917 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/exceptions.py
+-rw-r--r--   0        0        0      752 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/__init__.py
+-rw-r--r--   0        0        0    11137 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/blobs.py
+-rw-r--r--   0        0        0    15826 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/image.py
+-rw-r--r--   0        0        0     4875 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/manifests.py
+-rw-r--r--   0        0        0     1033 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/tags.py
+-rw-r--r--   0        0        0     3972 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/__init__.py
+-rw-r--r--   0        0        0     1140 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/auth.py
+-rw-r--r--   0        0        0     1077 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/base.py
+-rw-r--r--   0        0        0     4204 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/endpoint.py
+-rw-r--r--   0        0        0     3985 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/image_json.py
+-rw-r--r--   0        0        0     4615 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/manifest.py
+-rw-r--r--   0        0        0      910 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 moby_distribution-0.7.1/PKG-INFO
```

### Comparing `moby_distribution-0.7.0/LICENSE` & `moby_distribution-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/README.md` & `moby_distribution-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/__init__.py` & `moby_distribution-0.7.1/moby_distribution/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,32 @@
-from moby_distribution.registry.client import DockerRegistryV2Client, default_client, set_default_client
+from moby_distribution.registry.client import (
+    DockerRegistryV2Client,
+    default_client,
+    set_default_client,
+)
 from moby_distribution.registry.resources.blobs import Blob
 from moby_distribution.registry.resources.image import ImageRef, LayerRef
 from moby_distribution.registry.resources.manifests import ManifestRef
 from moby_distribution.registry.resources.tags import Tags
 from moby_distribution.spec.endpoint import OFFICIAL_ENDPOINT, APIEndpoint
 from moby_distribution.spec.image_json import ImageJSON
-from moby_distribution.spec.manifest import ManifestSchema1, ManifestSchema2, OCIManifestSchema1
+from moby_distribution.spec.manifest import (
+    ManifestSchema1,
+    ManifestSchema2,
+    OCIManifestSchema1,
+)
 
-__version__ = "0.7.0"
-__ALL__ = [
+__version__ = "0.7.1"
+__all__ = [
     "DockerRegistryV2Client",
     "Blob",
     "ManifestRef",
     "Tags",
     "APIEndpoint",
+    "OFFICIAL_ENDPOINT",
     "ManifestSchema1",
     "ManifestSchema2",
     "OCIManifestSchema1",
     "ImageJSON",
     "ImageRef",
     "LayerRef",
     "default_client",
```

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/auth.py` & `moby_distribution-0.7.1/moby_distribution/registry/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/client.py` & `moby_distribution-0.7.1/moby_distribution/registry/client.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/exceptions.py` & `moby_distribution-0.7.1/moby_distribution/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/resources/__init__.py` & `moby_distribution-0.7.1/moby_distribution/registry/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/resources/blobs.py` & `moby_distribution-0.7.1/moby_distribution/registry/resources/blobs.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/resources/image.py` & `moby_distribution-0.7.1/moby_distribution/registry/resources/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 import logging
 import shutil
 import tarfile
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from typing import List, Optional
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, __version__
 
 from moby_distribution.registry.client import DockerRegistryV2Client, default_client
 from moby_distribution.registry.resources import RepositoryResource
 from moby_distribution.registry.resources.blobs import Blob, HashSignWrapper
 from moby_distribution.registry.resources.manifests import ManifestRef
-from moby_distribution.registry.utils import TypeTimeout, client_default_timeout, generate_temp_dir, parse_image
+from moby_distribution.registry.utils import (
+    TypeTimeout,
+    client_default_timeout,
+    generate_temp_dir,
+    parse_image,
+)
 from moby_distribution.spec.image_json import History, ImageJSON, default_created
 from moby_distribution.spec.manifest import (
     DockerManifestConfigDescriptor,
     DockerManifestLayerDescriptor,
     ManifestSchema2,
 )
 
@@ -33,15 +38,15 @@
 
 
 class LayerRef(BaseModel):
     repo: str = ""
     digest: str = ""
     size: int = -1
     exists: bool = False
-    local_path: Optional[Path]
+    local_path: Optional[Path] = None
 
 
 class ImageRef(RepositoryResource):
     """ImageRef is used to Manipulate Docker images"""
 
     def __init__(
         self,
@@ -75,27 +80,34 @@
 
         if no `to_repo` or `to_reference` given, use `from_repo` or `from_reference` as default.
         """
         if to_repo is None:
             to_repo = from_repo
         if to_reference is None:
             to_reference = from_reference
-        manifest = ManifestRef(repo=from_repo, reference=from_reference, client=client).get(
-            ManifestSchema2.content_type()
-        )
+        manifest = ManifestRef(
+            repo=from_repo, reference=from_reference, client=client
+        ).get(ManifestSchema2.content_type())
         layers = [
-            LayerRef(repo=from_repo, digest=layer.digest, size=layer.size, exists=True) for layer in manifest.layers
+            LayerRef(repo=from_repo, digest=layer.digest, size=layer.size, exists=True)
+            for layer in manifest.layers
         ]
 
         fh = io.BytesIO()
-        Blob(repo=from_repo, digest=manifest.config.digest, client=client, fileobj=fh).download()
+        Blob(
+            repo=from_repo, digest=manifest.config.digest, client=client, fileobj=fh
+        ).download()
         fh.seek(0)
 
         return cls(
-            repo=to_repo, reference=to_reference, layers=layers, initial_config=fh.read().decode(), client=client
+            repo=to_repo,
+            reference=to_reference,
+            layers=layers,
+            initial_config=fh.read().decode(),
+            client=client,
         )
 
     @classmethod
     def from_tarball(
         cls,
         workplace: Path,
         src: Path,
@@ -130,15 +142,17 @@
             if to_reference is None:
                 to_reference = named.tag or "latest"
 
             layers = []
             for layer in manifest.Layers:
                 # gzip it for smaller size
                 gzipped_filepath = workplace / (layer + ".gz")
-                with (workplace / layer).open(mode="rb") as fh, gzip.open(gzipped_filepath, mode="wb") as compressed:
+                with (workplace / layer).open(mode="rb") as fh, gzip.open(
+                    gzipped_filepath, mode="wb"
+                ) as compressed:
                     shutil.copyfileobj(fh, compressed)
 
                 # The gzipped file can only be obtained after the compressed object is closed
                 # (because the gzip context information has not yet been written).
                 gzipped_signer = HashSignWrapper()
                 with gzipped_filepath.open(mode="rb") as fh:
                     shutil.copyfileobj(fh, gzipped_signer)
@@ -174,51 +188,66 @@
             (workplace / manifest.config).write_text(self.image_json_str)
 
             # Step 2. download layers
             for layer in self.layers:
                 manifest.Layers.append(self._save_layer(workplace, layer=layer))
 
             # Step 3. save manifest
-            (workplace / "manifest.json").write_text(f"[{manifest.json(by_alias=True)}]")
+            (workplace / "manifest.json").write_text(
+                f"[{manifest.json(by_alias=True)}]"
+            )
 
             # Step 4. save as tar
             with tarfile.open(mode="w", name=dest) as tarball:
                 for f in workplace.iterdir():
-                    tarball.add(name=str(f.absolute()), arcname=str(f.relative_to(workplace)))
+                    tarball.add(
+                        name=str(f.absolute()), arcname=str(f.relative_to(workplace))
+                    )
         return dest
 
-    def push(self, media_type: str = ManifestSchema2.content_type(), *, max_worker: int = 5):
+    def push(
+        self, media_type: str = ManifestSchema2.content_type(), *, max_worker: int = 5
+    ):
         """push the image to the registry."""
         if media_type == ManifestSchema2.content_type():
             return self.push_v2(max_worker=max_worker)
         raise NotImplementedError("only support push images with Manifest Schema2.")
 
     def push_v2(self, *, max_worker: int = 5) -> ManifestSchema2:
         """push the image to the registry, with Manifest Schema2."""
         layer_descriptors_futures = []
         layer_descriptors = []
         # Step 1: upload all layers
         with ThreadPoolExecutor(max_workers=max_worker) as thread_pool:
             for layer in self.layers:
-                layer_descriptors_futures.append(thread_pool.submit(self._upload_layer, layer))
+                layer_descriptors_futures.append(
+                    thread_pool.submit(self._upload_layer, layer)
+                )
         for future in layer_descriptors_futures:
             layer_descriptors.append(future.result())
 
         # Step 2: upload the image json
         config_descriptor = self._upload_config(self.image_json_str)
 
         # Step 3.: upload the manifest
         manifest = ManifestSchema2(config=config_descriptor, layers=layer_descriptors)
-        ref = ManifestRef(repo=self.repo, reference=self.reference, client=self.client, timeout=self.timeout)
+        ref = ManifestRef(
+            repo=self.repo,
+            reference=self.reference,
+            client=self.client,
+            timeout=self.timeout,
+        )
         ref.put(manifest)
         if self._dirty:
             return ref.get(media_type=ManifestSchema2.content_type())
         return manifest
 
-    def add_layer(self, layer: LayerRef, history: Optional[History] = None) -> DockerManifestLayerDescriptor:
+    def add_layer(
+        self, layer: LayerRef, history: Optional[History] = None
+    ) -> DockerManifestLayerDescriptor:
         """Add a layer to this image.
 
         Step:
           1. calculate the sha256 sum for the gzipped_tarball, as digest
           2. calculate the sha256 sum for the uncompressed_tarball, as diff_id
         """
         if not layer.exists and not layer.local_path:
@@ -255,24 +284,31 @@
         # Add remote layer if the layer is exists in registry
         else:
             with generate_temp_dir() as temp_dir:
                 # Step 1: calculate the sha256 sum for the gzipped_tarball
                 with (temp_dir / "blob").open(mode="wb") as fh:
                     raw_tarball_signer = HashSignWrapper(fh=fh)
                     Blob(
-                        repo=layer.repo, digest=layer.digest, fileobj=raw_tarball_signer, client=self.client
+                        repo=layer.repo,
+                        digest=layer.digest,
+                        fileobj=raw_tarball_signer,
+                        client=self.client,
                     ).download()
                     size = raw_tarball_signer.tell()
 
                 # Step 2: calculate the sha256 sum for the uncompressed_tarball
                 with gzip.open(filename=(temp_dir / "blob")) as uncompressed:
                     shutil.copyfileobj(uncompressed, uncompressed_tarball_signer)
 
             if layer.size != size:
-                raise ValueError("Wrong Size, layer.size<'%d'> != signer.size<'%d'>", layer.size, size)
+                raise ValueError(
+                    "Wrong Size, layer.size<'%d'> != signer.size<'%d'>",
+                    layer.size,
+                    size,
+                )
             if layer.digest != raw_tarball_signer.digest():
                 raise ValueError(
                     "Wrong digest, layer.digest<'%s'> != signer.digest<'%s'>",
                     layer.digest,
                     raw_tarball_signer.digest(),
                 )
 
@@ -304,51 +340,73 @@
         return base
 
     @property
     def image_json_str(self) -> str:
         if not self._dirty:
             return self._initial_config
         image_json = self.image_json
-        return image_json.json(exclude_unset=True, exclude_defaults=True, separators=(",", ":"))
+        if __version__.startswith("2."):
+            return json.dumps(
+                image_json.model_dump(
+                    mode="json", exclude_unset=True, exclude_defaults=True
+                ),
+                separators=(",", ":"),
+            )
+        else:
+            return image_json.json(
+                exclude_unset=True, exclude_defaults=True, separators=(",", ":")
+            )
 
     def _save_layer(self, workplace: Path, layer: LayerRef) -> str:
         """Download the gzipped layer, and uncompress as the raw tarball.
 
         if layer is exists in local disk(the local_path is not None), will skip download.
 
         :raise RequestErrorWithResponse: raise if an error occur.
         """
         gzip_path = layer.local_path or (workplace / "layers.tar.gz")
         temp_tarball_path = workplace / "layer.tar"
 
         if layer.local_path is None:
-            Blob(repo=layer.repo, digest=layer.digest, local_path=gzip_path, client=self.client).download()
-
-        with gzip.open(filename=gzip_path) as uncompressed, temp_tarball_path.open(mode="wb") as fh:
+            Blob(
+                repo=layer.repo,
+                digest=layer.digest,
+                local_path=gzip_path,
+                client=self.client,
+            ).download()
+
+        with gzip.open(filename=gzip_path) as uncompressed, temp_tarball_path.open(
+            mode="wb"
+        ) as fh:
             signer = HashSignWrapper(fh)
             shutil.copyfileobj(uncompressed, signer)
 
         tarball_path = f"{signer.digest()}/layer.tar"
         (workplace / tarball_path).parent.mkdir(exist_ok=True, parents=True)
 
         if layer.local_path is None:
             gzip_path.unlink()
 
-        shutil.move(str(temp_tarball_path.absolute()), str((workplace / tarball_path).absolute()))
+        shutil.move(
+            str(temp_tarball_path.absolute()),
+            str((workplace / tarball_path).absolute()),
+        )
         return tarball_path
 
     def _upload_layer(self, layer: LayerRef) -> DockerManifestLayerDescriptor:
         """Upload the layer to the registry
         this func will mount the existed layers from other repo or upload the local layers to the repo.
 
         :raise RequestErrorWithResponse: raise if an error occur.
         """
 
         if layer.exists and layer.repo != self.repo:
-            descriptor = Blob(repo=self.repo, digest=layer.digest, client=self.client).mount_from(from_repo=layer.repo)
+            descriptor = Blob(
+                repo=self.repo, digest=layer.digest, client=self.client
+            ).mount_from(from_repo=layer.repo)
         elif not layer.exists:
             blob = Blob(repo=self.repo, local_path=layer.local_path, client=self.client)
             descriptor = blob.upload()
         else:
             descriptor = Blob(repo=self.repo, client=self.client).stat(layer.digest)
 
         return DockerManifestLayerDescriptor(
@@ -358,13 +416,17 @@
         )
 
     def _upload_config(self, image_json_str: str) -> DockerManifestConfigDescriptor:
         """Upload the Image JSON to the registry
 
         :raise RequestErrorWithResponse: raise if an error occur.
         """
-        descriptor = Blob(repo=self.repo, fileobj=io.BytesIO(image_json_str.encode()), client=self.client).upload()
+        descriptor = Blob(
+            repo=self.repo,
+            fileobj=io.BytesIO(image_json_str.encode()),
+            client=self.client,
+        ).upload()
         return DockerManifestConfigDescriptor(
             size=len(image_json_str),
             digest=descriptor.digest,
             urls=descriptor.urls,
         )
```

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/resources/manifests.py` & `moby_distribution-0.7.1/moby_distribution/registry/resources/manifests.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/resources/tags.py` & `moby_distribution-0.7.1/moby_distribution/registry/resources/tags.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/registry/utils.py` & `moby_distribution-0.7.1/moby_distribution/registry/utils.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/spec/auth.py` & `moby_distribution-0.7.1/moby_distribution/spec/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/spec/base.py` & `moby_distribution-0.7.1/moby_distribution/spec/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     """
 
     mediaType: str
     size: int
     digest: str
     urls: List[str] = Field(default_factory=list)
     annotations: Dict[str, str] = Field(default_factory=dict)
-    platform: Optional[Platform]
+    platform: Optional[Platform] = None
```

### Comparing `moby_distribution-0.7.0/moby_distribution/spec/endpoint.py` & `moby_distribution-0.7.1/moby_distribution/spec/endpoint.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.0/moby_distribution/spec/image_json.py` & `moby_distribution-0.7.1/moby_distribution/spec/image_json.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,70 +22,97 @@
         {"NONE"} : disable healthcheck
         {"CMD", args...} : exec arguments directly
         {"CMD-SHELL", command} : run command with system's default shell
     """
         ),
     )
     Interval: int = Field(..., description="the time to wait between checks.")
-    Timeout: int = Field(..., description="the time to wait before considering the check to have hung.")
+    Timeout: int = Field(
+        ..., description="the time to wait before considering the check to have hung."
+    )
     StartPeriod: int = Field(
-        ..., description="the period for the container to initialize before the retries starts to count down."
+        ...,
+        description="the period for the container to initialize before the retries starts to count down.",
     )
     Retries: int = Field(
-        ..., description="the number of consecutive failures needed to consider a container as unhealthy."
+        ...,
+        description="the number of consecutive failures needed to consider a container as unhealthy.",
     )
 
 
 class ContainerConfig(BaseModel):
     """ContainerConfig contains the configuration data when running a container using the image
     spec: https://github.com/opencontainers/image-spec/blob/main/config.md
     """
 
     User: str = Field(
-        "", description="User that will run the command(s) inside the container, also support user:group"
+        "",
+        description="User that will run the command(s) inside the container, also support user:group",
     )
     Memory: Optional[int] = Field(default=None, description="Memory limit (in bytes)")
     MemorySwap: Optional[int] = Field(
-        default=None, description=" Total memory usage (memory + swap); set `-1` to enable unlimited swap"
+        default=None,
+        description=" Total memory usage (memory + swap); set `-1` to enable unlimited swap",
+    )
+    CpuShares: Optional[int] = Field(
+        default=None, description="CPU shares (relative weight vs. other containers)"
+    )
+    ExposedPorts: Optional[Dict[str, Dict]] = Field(
+        None, description="List of exposed ports"
+    )
+    Env: Optional[List[str]] = Field(
+        default=None, description="List of environment variable to set in the container"
     )
-    CpuShares: Optional[int] = Field(default=None, description="CPU shares (relative weight vs. other containers)")
-    ExposedPorts: Optional[Dict[str, Dict]] = Field(None, description="List of exposed ports")
-    Env: Optional[List[str]] = Field(default=None, description="List of environment variable to set in the container")
     Entrypoint: Optional[List[str]] = Field(
-        None, description="A list of arguments to use as the command to execute when the container starts. "
+        None,
+        description="A list of arguments to use as the command to execute when the container starts. ",
+    )
+    Cmd: Optional[List[str]] = Field(
+        default=None,
+        description="Default arguments to the entrypoint of the container.",
+    )
+    Volumes: Optional[Dict] = Field(
+        default=None, description="List of volumes (mounts) used for the container."
     )
-    Cmd: Optional[List[str]] = Field(default=None, description="Default arguments to the entrypoint of the container.")
-    Volumes: Optional[Dict] = Field(default=None, description="List of volumes (mounts) used for the container.")
     WorkingDir: Optional[str] = Field(
-        default=None, description="Current directory (PWD) in the command will be launched"
+        default=None,
+        description="Current directory (PWD) in the command will be launched",
+    )
+    Labels: Optional[Dict[str, str]] = Field(
+        default=None, description="List of labels set to this container"
     )
-    Labels: Optional[Dict[str, str]] = Field(default=None, description="List of labels set to this container")
     StopSignal: Optional[str] = Field(
-        default=None, description="The signal that will be sent to the container to exit."
+        default=None,
+        description="The signal that will be sent to the container to exit.",
     )
     Healthcheck: Optional[HealthConfig] = Field(
-        default=None, description="Healthcheck describes how to check the container is healthy"
+        default=None,
+        description="Healthcheck describes how to check the container is healthy",
     )
 
 
 class RootFS(BaseModel):
-    diff_ids: List[str] = Field(..., description="diff id is the digest of uncompressed tarball")
+    diff_ids: List[str] = Field(
+        ..., description="diff id is the digest of uncompressed tarball"
+    )
     type: str = "layers"
 
 
 class History(BaseModel):
     created: Optional[datetime.datetime] = Field(default_factory=default_created)
-    author: Optional[str]
-    created_by: Optional[str]
-    comment: Optional[str]
+    author: Optional[str] = None
+    created_by: Optional[str] = None
+    comment: Optional[str] = None
     empty_layer: Optional[bool] = False
 
 
 class ImageJSON(BaseModel):
     created: datetime.datetime
     author: str = "anonymous"
     architecture: str
     os: str
-    variant: Optional[str] = Field(default=None, description="The variant of the specified CPU architecture.")
+    variant: Optional[str] = Field(
+        default=None, description="The variant of the specified CPU architecture."
+    )
     config: ContainerConfig
     rootfs: RootFS
     history: List[History]
```

### Comparing `moby_distribution-0.7.0/moby_distribution/spec/manifest.py` & `moby_distribution-0.7.1/moby_distribution/spec/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     schemaVersion: int = 1
     name: str
     tag: str
     architecture: str
     fsLayers: List[FileSystemLayer]
     history: List[Schema1History]
-    signatures: Optional[List[JWS]]
+    signatures: Optional[List[JWS]] = None
 
     @staticmethod
     def content_type() -> str:
         return "application/vnd.docker.distribution.manifest.v1+prettyjws"
 
     @validator("schemaVersion")
     def validate_schema_version(cls, v):
@@ -48,15 +48,15 @@
 
 
 class PlatformSpec(Platform):
     """
     PlatformSpec specifies a platform where a particular image manifest is applicable.
     """
 
-    features: Optional[List[str]]
+    features: Optional[List[str]] = None
 
 
 class DockerManifestConfigDescriptor(Descriptor):
     @staticmethod
     def content_type() -> str:
         return "application/vnd.docker.container.image.v1+json"
 
@@ -143,8 +143,8 @@
 
     _validate_media_type = validator("mediaType", allow_reuse=True)(validate_media_type)
 
 
 class ManifestDescriptor(Descriptor):
     """ManifestDescriptor references a platform-specific manifest."""
 
-    platform: Optional[PlatformSpec]
+    platform: Optional[PlatformSpec] = None
```

### Comparing `moby_distribution-0.7.0/pyproject.toml` & `moby_distribution-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moby-distribution"
-version = "0.7.0"
+version = "0.7.1"
 description = "Yet another moby(docker) distribution implement by python."
 authors = ["shabbywu <shabbywu@qq.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 repository = "https://github.com/shabbywu/distribution"
 homepage = "https://github.com/shabbywu/distribution"
```

### Comparing `moby_distribution-0.7.0/PKG-INFO` & `moby_distribution-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moby-distribution
-Version: 0.7.0
+Version: 0.7.1
 Summary: Yet another moby(docker) distribution implement by python.
 Home-page: https://github.com/shabbywu/distribution
 License: Apache-2.0
 Author: shabbywu
 Author-email: shabbywu@qq.com
 Requires-Python: >=3.6.2,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

