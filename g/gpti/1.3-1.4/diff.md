# Comparing `tmp/gpti-1.3.tar.gz` & `tmp/gpti-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpti-1.3.tar", last modified: Sun Feb 18 05:15:27 2024, max compression
+gzip compressed data, was "gpti-1.4.tar", last modified: Sun Apr  7 00:19:54 2024, max compression
```

## Comparing `gpti-1.3.tar` & `gpti-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-18 05:15:27.038419 gpti-1.3/
--rw-rw-rw-   0        0        0     1084 2024-01-24 17:14:27.000000 gpti-1.3/LICENSE
--rw-rw-rw-   0        0        0    60502 2024-02-18 05:15:27.022098 gpti-1.3/PKG-INFO
--rw-rw-rw-   0        0        0    58614 2024-02-18 05:15:15.000000 gpti-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-18 05:15:26.973447 gpti-1.3/gpti/
--rw-rw-rw-   0        0        0    95943 2024-02-18 04:35:52.000000 gpti-1.3/gpti/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-18 05:15:27.010660 gpti-1.3/gpti.egg-info/
--rw-rw-rw-   0        0        0    60502 2024-02-18 05:15:26.000000 gpti-1.3/gpti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-02-18 05:15:26.000000 gpti-1.3/gpti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-18 05:15:26.000000 gpti-1.3/gpti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-02-18 05:15:26.000000 gpti-1.3/gpti.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-02-18 05:15:26.000000 gpti-1.3/gpti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-18 05:15:27.038419 gpti-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1156 2024-02-18 05:10:32.000000 gpti-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:19:54.488304 gpti-1.4/
+-rw-rw-rw-   0        0        0     1084 2024-01-24 17:14:27.000000 gpti-1.4/LICENSE
+-rw-rw-rw-   0        0        0    63532 2024-04-07 00:19:54.488304 gpti-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    61477 2024-04-07 00:16:22.000000 gpti-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 00:19:54.462589 gpti-1.4/gpti/
+-rw-rw-rw-   0        0        0   109640 2024-04-06 23:08:54.000000 gpti-1.4/gpti/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:19:54.478531 gpti-1.4/gpti.egg-info/
+-rw-rw-rw-   0        0        0    63532 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 00:19:54.488304 gpti-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2024-04-06 23:14:17.000000 gpti-1.4/setup.py
```

### Comparing `gpti-1.3/LICENSE` & `gpti-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpti-1.3/PKG-INFO` & `gpti-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gpti
-Version: 1.3
+Version: 1.4
 Summary: This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT
 Home-page: https://github.com/yandricr/gpti-py/
 Author: yandricr
 Author-email: yandribret@gmail.com
 License: MIT
 Project-URL: Documentation, https://nexra.aryahcr.cc/
 Project-URL: Funding, https://ko-fi.com/yandricr
 Project-URL: Source, https://github.com/yandricr/gpti-py/
-Keywords: gpt gpt-3 gpt-3.5 gpt-4 gpti gpt-free ai generate-image prodia bing chat stream dalle dalle-2 llama-2 stable-diffusion pixart EMI render3d pixel-art
+Keywords: gpt gpt-3 gpt-3.5 gpt-4 gpti gpt-free ai generate-image prodia bing chat stream dalle dalle-2 llama-2 stable-diffusion pixart EMI render3d pixel-art playground animagine-xl
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 
 # GPTI
 
 ![Downloads](https://img.shields.io/pypi/dw/gpti?style=for-the-badge) ![License](https://img.shields.io/pypi/l/gpti?style=for-the-badge) [![Contributors](https://img.shields.io/github/contributors/yandricr/gpti-py?style=for-the-badge)](https://github.com/yandricr/gpti-py/graphs/contributors) [![Size Package](https://img.shields.io/github/languages/code-size/yandricr/gpti-py?style=for-the-badge)](https://github.com/yandricr/gpti-py) ![Python](https://img.shields.io/badge/python-%233776AB.svg?style=for-the-badge&logo=python&logoColor=white) [![Ko-Fi](https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/yandricr)
 
 This package simplifies your interaction with various GPT models, eliminating the need for tokens or other methods to access GPT. It also allows you to use three artificial intelligences to generate images: DALL·E, Prodia and more, all of this without restrictions or limits
@@ -33,29 +34,39 @@
 GPTI provides access to a variety of artificial intelligence models to meet various needs. Currently, the available models include:
 
 - [**ChatGPT**](#gpt)
 - [**ChatGPT Web**](#gptweb)
 - [**Bing**](#bing)
 - [**LLaMA-2**](#llama2)
 - [**DALL·E**](#dalle)
-- [**DALL-E 2**](#dalle2)
+- [**DALL-E 2**](#dalle2) (PRO)
 - [**DALL-E Mini**](#dalle-mini)
 - [**Prodia**](#prodia)
 - [**Prodia Stable-Diffusion**](#prodia-stablediffusion)
-- [**Prodia Stable-Diffusion XL**](#prodia-stablediffusion-xl)
-- [**Pixart-A**](#pixart-a)
-- [**Pixart-LCM**](#pixart-lcm)
+- [**Prodia Stable-Diffusion XL**](#prodia-stablediffusion-xl) (PRO)
+- [**Pixart-A**](#pixart-a) (PRO)
+- [**Pixart-LCM**](#pixart-lcm) (PRO)
 - [**Stable-Diffusion 1.5**](#stablediffusion-1.5)
 - [**Stable-Diffusion 2.1**](#stablediffusion-2.1)
-- [**Stable-Diffusion XL**](#stablediffusion-xl)
+- [**Stable-Diffusion XL**](#stablediffusion-xl) (PRO)
 - [**EMI**](#emi)
-- [**Render3D**](#render3d)
-- [**PixelArt**](#pixelart)
+- [**Render3D**](#render3d) (PRO)
+- [**PixelArt**](#pixelart) (PRO)
+- [**Animagine-XL**](#animagine-xl) (PRO)
+- [**Playground**](#playground) (PRO)
 
-These are just some examples of the models available in this package. I will continue expanding to include an even greater variety of models.
+## Api key
+
+If you want to access the premium models, enter your credentials. You can obtain them by [clicking here](https://nexra.aryahcr.cc/api-key/en).
+
+```python
+from gpti import nexra
+
+nexra("user-xxxxxxxx", "nx-xxxxxxx-xxxxx-xxxxx");
+```
 
 <a id="gpt"></a>
 ## Usage GPT
 
 ```python
 import json
 from gpti import gpt
@@ -433,15 +444,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="dalle2"></a>
-## Usage DALL·E 2
+## Usage DALL·E 2 (PRO)
 
 ```python
 import json
 from gpti import dalle
 
 res = dalle.v2(prompt="An extensive green valley stretches toward imposing mountains, adorned with meadows and a winding stream. The morning sun paints the sky with warm tones, illuminating the landscape with a serenity that invites contemplation and peace.", data={
     "gpu": False,
@@ -555,14 +566,16 @@
 - amIReal_V41.safetensors [0a8a2e61]
 - analog-diffusion-1.0.ckpt [9ca13f02]
 - anythingv3_0-pruned.ckpt [2700c435]
 - anything-v4.5-pruned.ckpt [65745d25]
 - anythingV5_PrtRE.safetensors [893e49b9]
 - AOM3A3_orangemixs.safetensors [9600da17]
 - blazing_drive_v10g.safetensors [ca1c1eab]
+- breakdomain_I2428.safetensors [43cc7d2f]
+- breakdomain_M2150.safetensors [15f7afca]
 - cetusMix_Version35.safetensors [de2f2560]
 - childrensStories_v13D.safetensors [9dfaabcb]
 - childrensStories_v1SemiReal.safetensors [a1c56dbb]
 - childrensStories_v1ToonAnime.safetensors [2ec7b88b]
 - Counterfeit_v30.safetensors [9e2a8f19]
 - cuteyukimixAdorable_midchapter3.safetensors [04bdffe6]
 - cyberrealistic_v33.safetensors [82b0d085]
@@ -574,16 +587,19 @@
 - dreamlike-photoreal-2.0.safetensors [fdcf65e7]
 - dreamshaper_6BakedVae.safetensors [114c8abb]
 - dreamshaper_7.safetensors [5cf5ae06]
 - dreamshaper_8.safetensors [9d40847d]
 - edgeOfRealism_eorV20.safetensors [3ed5de15]
 - EimisAnimeDiffusion_V1.ckpt [4f828a15]
 - elldreths-vivid-mix.safetensors [342d9d26]
+- epicphotogasm_xPlusPlus.safetensors [1a8f6d35]
 - epicrealism_naturalSinRC1VAE.safetensors [90a4c676]
+- epicrealism_pureEvolutionV3.safetensors [42c8440c]
 - ICantBelieveItsNotPhotography_seco.safetensors [4e7a3dfd]
+- indigoFurryMix_v75Hybrid.safetensors [91208cbb]
 - juggernaut_aftermath.safetensors [5e20c455]
 - lofi_v4.safetensors [ccc204d6]
 - lyriel_v16.safetensors [68fceea2]
 - majicmixRealistic_v4.safetensors [29d0de58]
 - mechamix_v10.safetensors [ee685731]
 - meinamix_meinaV9.safetensors [2ec66ab0]
 - meinamix_meinaV11.safetensors [b56ce717]
@@ -597,14 +613,16 @@
 - Realistic_Vision_V4.0.safetensors [29a7afaa]
 - Realistic_Vision_V5.0.safetensors [614d1063]
 - redshift_diffusion-V10.safetensors [1400e684]
 - revAnimated_v122.safetensors [3f4fefd9]
 - rundiffusionFX25D_v10.safetensors [cd12b0ee]
 - rundiffusionFX_v10.safetensors [cd4e694d]
 - sdv1_4.ckpt [7460a6fa]
+- v1-5-pruned-emaonly.safetensors [d7049739]
+- v1-5-inpainting.safetensors [21c7ab71]
 - shoninsBeautiful_v10.safetensors [25d8c546]
 - theallys-mix-ii-churned.safetensors [5d9225a4]
 - timeless-1.0.ckpt [7c4971d4]
 - toonyou_beta6.safetensors [980f6b15]
 
 #### Parameters
 
@@ -662,24 +680,26 @@
 }
 ```
 
 #### Models
 
 List of models
 
-- absolutereality_v181.safetensors [3d9d4d2b]
 - 3Guofeng3_v34.safetensors [50f420de]
 - absolutereality_V16.safetensors [37db0fc3]
+- absolutereality_v181.safetensors [3d9d4d2b]
 - amIReal_V41.safetensors [0a8a2e61]
 - analog-diffusion-1.0.ckpt [9ca13f02]
 - anythingv3_0-pruned.ckpt [2700c435]
 - anything-v4.5-pruned.ckpt [65745d25]
 - anythingV5_PrtRE.safetensors [893e49b9]
 - AOM3A3_orangemixs.safetensors [9600da17]
 - blazing_drive_v10g.safetensors [ca1c1eab]
+- breakdomain_I2428.safetensors [43cc7d2f]
+- breakdomain_M2150.safetensors [15f7afca]
 - cetusMix_Version35.safetensors [de2f2560]
 - childrensStories_v13D.safetensors [9dfaabcb]
 - childrensStories_v1SemiReal.safetensors [a1c56dbb]
 - childrensStories_v1ToonAnime.safetensors [2ec7b88b]
 - Counterfeit_v30.safetensors [9e2a8f19]
 - cuteyukimixAdorable_midchapter3.safetensors [04bdffe6]
 - cyberrealistic_v33.safetensors [82b0d085]
@@ -691,16 +711,19 @@
 - dreamlike-photoreal-2.0.safetensors [fdcf65e7]
 - dreamshaper_6BakedVae.safetensors [114c8abb]
 - dreamshaper_7.safetensors [5cf5ae06]
 - dreamshaper_8.safetensors [9d40847d]
 - edgeOfRealism_eorV20.safetensors [3ed5de15]
 - EimisAnimeDiffusion_V1.ckpt [4f828a15]
 - elldreths-vivid-mix.safetensors [342d9d26]
+- epicphotogasm_xPlusPlus.safetensors [1a8f6d35]
 - epicrealism_naturalSinRC1VAE.safetensors [90a4c676]
+- epicrealism_pureEvolutionV3.safetensors [42c8440c]
 - ICantBelieveItsNotPhotography_seco.safetensors [4e7a3dfd]
+- indigoFurryMix_v75Hybrid.safetensors [91208cbb]
 - juggernaut_aftermath.safetensors [5e20c455]
 - lofi_v4.safetensors [ccc204d6]
 - lyriel_v16.safetensors [68fceea2]
 - majicmixRealistic_v4.safetensors [29d0de58]
 - mechamix_v10.safetensors [ee685731]
 - meinamix_meinaV9.safetensors [2ec66ab0]
 - meinamix_meinaV11.safetensors [b56ce717]
@@ -760,15 +783,15 @@
 | sampling_method  | DPM++ 2M Karras                       | Select from the list of methods          |
 | sampling_steps   | 25                                    | Min: 1, Max: 30                          |
 | width            | 512                                   | Min: 50, Max: 1024                       |
 | height           | 512                                   | Min: 50, Max: 1024                       |
 | cfg_scale        | 7                                     | Min: 1, Max: 20                          |
 
 <a id="prodia-stablediffusion-xl"></a>
-## Usage Prodia Stable-Diffusion XL
+## Usage Prodia Stable-Diffusion XL (PRO)
 
 ```python
 import json
 from gpti import prodia
 
 res = prodia.stablediffusion_xl(prompt="Friends gathered around a bonfire in an ancient forest. Laughter, stories, and a starry sky paint an unforgettable moment of connection beneath the shadows of the mountains.", data={
     "prompt_negative": "",
@@ -809,19 +832,21 @@
 }
 ```
 
 #### Models
 
 List of models:
 
-- sd_xl_base_1.0.safetensors [be9edd61]
 - dreamshaperXL10_alpha2.safetensors [c8afe2ef]
 - dynavisionXL_0411.safetensors [c39cc051]
 - juggernautXL_v45.safetensors [e75f5471]
 - realismEngineSDXL_v10.safetensors [af771c3f]
+- sd_xl_base_1.0.safetensors [be9edd61]
+- sd_xl_base_1.0_inpainting_0.1.safetensors [5679a81a]
+- turbovisionXL_v431.safetensors [78890989]
 
 #### Methods
 
 List of methods:
 
 - DPM++ 2M Karras
 - Euler
@@ -850,15 +875,15 @@
 | sampling_method  | DPM++ 2M Karras                  | Select from the list of methods          |
 | sampling_steps   | 25                               | Min: 1, Max: 30                          |
 | width            | 1024                             | Min: 512, Max: 1536                      |
 | height           | 1024                             | Min: 512, Max: 1536                      |
 | cfg_scale        | 7                                | Min: 1, Max: 20                          |
 
 <a id="pixart-a"></a>
-## Usage Pixart-A
+## Usage Pixart-A (PRO)
 
 ```python
 import json
 from gpti import pixart
 
 res = pixart.a(prompt="An urban landscape bathed in the sunset, where the warm tones of the sun reflect on modern buildings and the orange and purple sky. In the foreground, there's a group of friends gathered on a rooftop, laughing and enjoying the moment. Their expressions radiate joy and camaraderie as they embrace and point towards something on the horizon. The scene is enveloped in a nostalgic and emotional aura that conveys the beauty of friendship and the warmth of the sunset in a futuristic city with touches of anime style.", data={
     "prompt_negative": "",
@@ -914,15 +939,15 @@
 | height               | 1024         | Min: 256, Max: 2048                                  |
 | dpm_guidance_scale   | 4.5          | Min: 1, Max: 10                                      |
 | dpm_inference_steps  | 14           | Min: 5, Max: 40                                      |
 | sa_guidance_scale    | 3            | Min: 1, Max: 10                                      |
 | sa_inference_steps   | 25           | Min: 10, Max: 40                                     |
 
 <a id="pixart-lcm"></a>
-## Usage Pixart-LCM
+## Usage Pixart-LCM (PRO)
 
 ```python
 import json
 from gpti import pixart
 
 res = pixart.lcm(prompt="An urban landscape bathed in the sunset, where the warm tones of the sun reflect on modern buildings and the orange and purple sky. In the foreground, there's a group of friends gathered on a rooftop, laughing and enjoying the moment. Their expressions radiate joy and camaraderie as they embrace and point towards something on the horizon. The scene is enveloped in a nostalgic and emotional aura that conveys the beauty of friendship and the warmth of the sunset in a futuristic city with touches of anime style.", data={
     "prompt_negative": "",
@@ -1040,15 +1065,15 @@
 
 | Parameter         | Default | Description                           |
 |-------------------|---------|---------------------------------------|
 | prompt_negative   |         | Indicates what the AI should not do    |
 | guidance_scale    | 9       | Min: 0 Max: 50                        |
 
 <a id="stablediffusion-xl"></a>
-## Usage Stable-Diffusion XL
+## Usage Stable-Diffusion XL (PRO)
 
 ```python
 import json
 from gpti import stablediffusion
 
 res = stablediffusion.xl(prompt="An serene sunset landscape where a river winds through gentle hills covered in trees. The sky is tinged with warm and soft tones, with scattered clouds reflecting the last glimmers of the sun.", data={
     "prompt_negative": "",
@@ -1117,15 +1142,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="render3d"></a>
-## Usage Render3D
+## Usage Render3D (PRO)
 
 ```python
 import json
 from gpti import render3d
 
 res = render3d(prompt="In a remote corner of the galaxy, a star agonizes in its final stage of life. Its brightness, once dazzling, now fades slowly into the void of space, while a bright nebula forms around it.", data={
     "prompt_negative": ""
@@ -1151,15 +1176,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="pixelart"></a>
-## Usage PixelArt
+## Usage PixelArt (PRO)
 
 ```python
 import json
 from gpti import pixelart
 
 res = pixelart(prompt="A coastal city in the golden hour of the sunset. The sun slowly slips toward the horizon, tinting the sky with golden and pink hues. Skyscrapers stand out against this heavenly backdrop, reflecting the light in their glass windows. In the streets, lights flicker timidly, getting ready to illuminate the night.", data={
     "prompt_negative": ""
@@ -1184,28 +1209,121 @@
     },
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
+<a id="animagine-xl"></a>
+## Usage Animagine-XL (PRO)
+
+```python
+import json
+from gpti import animagine
+
+res = animagine(prompt="An anime girl surrounded by cherry blossoms", data={
+    "prompt_negative": "",
+    "quality_tags": "Standard",
+    "style_present": "(None)",
+    "width": 1024,
+    "height": 1024,
+    "strength": 0.5,
+    "upscale": 1.5,
+    "sampler": "Euler a",
+    "guidance_scale": 7,
+    "inference_steps": 28
+})
+
+if res.error != None:
+    print(json.dumps(res.error))
+else:
+    print(json.dumps(res.result))
+```
+
+#### JSON
+
+```json
+{
+    "code": 200,
+    "status": true,
+    "prompt": "An anime girl surrounded by cherry blossoms",
+    "model": "Animagine-XL",
+    "data": {
+        "prompt_negative": "",
+        "quality_tags": "Standard",
+        "style_present": "(None)",
+        "width": 1024,
+        "height": 1024,
+        "strength": 0.5,
+        "upscale": 1.5,
+        "sampler": "Euler a",
+        "guidance_scale": 7,
+        "inference_steps": 28
+    },
+    "images": [
+        "data:image/jpeg;base64,..."
+    ]
+}
+```
+
+<a id="playground"></a>
+## Usage Playground (PRO)
+
+```python
+import json
+from gpti import playground
+
+res = playground(prompt="An illustration of a red owl with bright blue eye", data={
+    "prompt_negative": "",
+    "width": 1024,
+    "height": 1024,
+    "guidance_scale": 3
+})
+
+if res.error != None:
+    print(json.dumps(res.error))
+else:
+    print(json.dumps(res.result))
+```
+
+#### JSON
+
+```json
+{
+    "code": 200,
+    "status": true,
+    "prompt": "An illustration of a red owl with bright blue eyes.",
+    "model": "Playground",
+    "data": {
+        "prompt_negative": "",
+        "width": 1024,
+        "height": 1024,
+        "guidance_scale": 3
+    },
+    "images": [
+        "data:image/jpeg;base64,..."
+    ]
+}
+```
+
 ## API Reference
 
-At present, the API doesn't have any access restrictions or usage limits. For further details and examples, please refer to the complete [documentation](https://nexra.aryahcr.cc/).
+Currently, some models require your credentials to access them, while others are free. For more details and examples, please refer to the complete [documentation](https://nexra.aryahcr.cc/).
 
 #### Code Errors
 
 These are the error codes that will be presented in case the API fails.
 
-| Code | Error                  | Description                                    |
-|------|------------------------|------------------------------------------------|
-| 400  | BAD_REQUEST            | Not all parameters have been entered correctly |
-| 500  | INTERNAL_SERVER_ERROR  | The server has experienced failures             |
-| 200  |                        | The API worked without issues                    |
+| Code | Error                  | Description                                           |
+|------|------------------------|-------------------------------------------------------|
+| 400  | BAD_REQUEST            | Not all parameters have been entered correctly        |
+| 500  | INTERNAL_SERVER_ERROR  | The server has experienced failures                   |
+| 200  |                        | The API worked without issues                          |
+| 403  | FORBIDDEN              | Your API key has expired and needs to be renewed      |
+| 401  | UNAUTHORIZED           | API credentials are required                          |
+
 
 ## ☕ Do you want to support this project?
 
 If this package has helped you save time or solve a problem, consider inviting me for a coffee through Ko-fi. Your support helps me maintain and improve this project for you and other users like you. Furthermore, each donation contributes to the creation and free availability of more AI models in the future. Every small donation counts and is greatly appreciated!
 
 [![Support on Ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/yandricr)
-
-Remember: Programmers don't need coffee... but it helps a lot! 😉
```

### Comparing `gpti-1.3/README.md` & `gpti-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,39 @@
 GPTI provides access to a variety of artificial intelligence models to meet various needs. Currently, the available models include:
 
 - [**ChatGPT**](#gpt)
 - [**ChatGPT Web**](#gptweb)
 - [**Bing**](#bing)
 - [**LLaMA-2**](#llama2)
 - [**DALL·E**](#dalle)
-- [**DALL-E 2**](#dalle2)
+- [**DALL-E 2**](#dalle2) (PRO)
 - [**DALL-E Mini**](#dalle-mini)
 - [**Prodia**](#prodia)
 - [**Prodia Stable-Diffusion**](#prodia-stablediffusion)
-- [**Prodia Stable-Diffusion XL**](#prodia-stablediffusion-xl)
-- [**Pixart-A**](#pixart-a)
-- [**Pixart-LCM**](#pixart-lcm)
+- [**Prodia Stable-Diffusion XL**](#prodia-stablediffusion-xl) (PRO)
+- [**Pixart-A**](#pixart-a) (PRO)
+- [**Pixart-LCM**](#pixart-lcm) (PRO)
 - [**Stable-Diffusion 1.5**](#stablediffusion-1.5)
 - [**Stable-Diffusion 2.1**](#stablediffusion-2.1)
-- [**Stable-Diffusion XL**](#stablediffusion-xl)
+- [**Stable-Diffusion XL**](#stablediffusion-xl) (PRO)
 - [**EMI**](#emi)
-- [**Render3D**](#render3d)
-- [**PixelArt**](#pixelart)
+- [**Render3D**](#render3d) (PRO)
+- [**PixelArt**](#pixelart) (PRO)
+- [**Animagine-XL**](#animagine-xl) (PRO)
+- [**Playground**](#playground) (PRO)
 
-These are just some examples of the models available in this package. I will continue expanding to include an even greater variety of models.
+## Api key
+
+If you want to access the premium models, enter your credentials. You can obtain them by [clicking here](https://nexra.aryahcr.cc/api-key/en).
+
+```python
+from gpti import nexra
+
+nexra("user-xxxxxxxx", "nx-xxxxxxx-xxxxx-xxxxx");
+```
 
 <a id="gpt"></a>
 ## Usage GPT
 
 ```python
 import json
 from gpti import gpt
@@ -418,15 +428,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="dalle2"></a>
-## Usage DALL·E 2
+## Usage DALL·E 2 (PRO)
 
 ```python
 import json
 from gpti import dalle
 
 res = dalle.v2(prompt="An extensive green valley stretches toward imposing mountains, adorned with meadows and a winding stream. The morning sun paints the sky with warm tones, illuminating the landscape with a serenity that invites contemplation and peace.", data={
     "gpu": False,
@@ -540,14 +550,16 @@
 - amIReal_V41.safetensors [0a8a2e61]
 - analog-diffusion-1.0.ckpt [9ca13f02]
 - anythingv3_0-pruned.ckpt [2700c435]
 - anything-v4.5-pruned.ckpt [65745d25]
 - anythingV5_PrtRE.safetensors [893e49b9]
 - AOM3A3_orangemixs.safetensors [9600da17]
 - blazing_drive_v10g.safetensors [ca1c1eab]
+- breakdomain_I2428.safetensors [43cc7d2f]
+- breakdomain_M2150.safetensors [15f7afca]
 - cetusMix_Version35.safetensors [de2f2560]
 - childrensStories_v13D.safetensors [9dfaabcb]
 - childrensStories_v1SemiReal.safetensors [a1c56dbb]
 - childrensStories_v1ToonAnime.safetensors [2ec7b88b]
 - Counterfeit_v30.safetensors [9e2a8f19]
 - cuteyukimixAdorable_midchapter3.safetensors [04bdffe6]
 - cyberrealistic_v33.safetensors [82b0d085]
@@ -559,16 +571,19 @@
 - dreamlike-photoreal-2.0.safetensors [fdcf65e7]
 - dreamshaper_6BakedVae.safetensors [114c8abb]
 - dreamshaper_7.safetensors [5cf5ae06]
 - dreamshaper_8.safetensors [9d40847d]
 - edgeOfRealism_eorV20.safetensors [3ed5de15]
 - EimisAnimeDiffusion_V1.ckpt [4f828a15]
 - elldreths-vivid-mix.safetensors [342d9d26]
+- epicphotogasm_xPlusPlus.safetensors [1a8f6d35]
 - epicrealism_naturalSinRC1VAE.safetensors [90a4c676]
+- epicrealism_pureEvolutionV3.safetensors [42c8440c]
 - ICantBelieveItsNotPhotography_seco.safetensors [4e7a3dfd]
+- indigoFurryMix_v75Hybrid.safetensors [91208cbb]
 - juggernaut_aftermath.safetensors [5e20c455]
 - lofi_v4.safetensors [ccc204d6]
 - lyriel_v16.safetensors [68fceea2]
 - majicmixRealistic_v4.safetensors [29d0de58]
 - mechamix_v10.safetensors [ee685731]
 - meinamix_meinaV9.safetensors [2ec66ab0]
 - meinamix_meinaV11.safetensors [b56ce717]
@@ -582,14 +597,16 @@
 - Realistic_Vision_V4.0.safetensors [29a7afaa]
 - Realistic_Vision_V5.0.safetensors [614d1063]
 - redshift_diffusion-V10.safetensors [1400e684]
 - revAnimated_v122.safetensors [3f4fefd9]
 - rundiffusionFX25D_v10.safetensors [cd12b0ee]
 - rundiffusionFX_v10.safetensors [cd4e694d]
 - sdv1_4.ckpt [7460a6fa]
+- v1-5-pruned-emaonly.safetensors [d7049739]
+- v1-5-inpainting.safetensors [21c7ab71]
 - shoninsBeautiful_v10.safetensors [25d8c546]
 - theallys-mix-ii-churned.safetensors [5d9225a4]
 - timeless-1.0.ckpt [7c4971d4]
 - toonyou_beta6.safetensors [980f6b15]
 
 #### Parameters
 
@@ -647,24 +664,26 @@
 }
 ```
 
 #### Models
 
 List of models
 
-- absolutereality_v181.safetensors [3d9d4d2b]
 - 3Guofeng3_v34.safetensors [50f420de]
 - absolutereality_V16.safetensors [37db0fc3]
+- absolutereality_v181.safetensors [3d9d4d2b]
 - amIReal_V41.safetensors [0a8a2e61]
 - analog-diffusion-1.0.ckpt [9ca13f02]
 - anythingv3_0-pruned.ckpt [2700c435]
 - anything-v4.5-pruned.ckpt [65745d25]
 - anythingV5_PrtRE.safetensors [893e49b9]
 - AOM3A3_orangemixs.safetensors [9600da17]
 - blazing_drive_v10g.safetensors [ca1c1eab]
+- breakdomain_I2428.safetensors [43cc7d2f]
+- breakdomain_M2150.safetensors [15f7afca]
 - cetusMix_Version35.safetensors [de2f2560]
 - childrensStories_v13D.safetensors [9dfaabcb]
 - childrensStories_v1SemiReal.safetensors [a1c56dbb]
 - childrensStories_v1ToonAnime.safetensors [2ec7b88b]
 - Counterfeit_v30.safetensors [9e2a8f19]
 - cuteyukimixAdorable_midchapter3.safetensors [04bdffe6]
 - cyberrealistic_v33.safetensors [82b0d085]
@@ -676,16 +695,19 @@
 - dreamlike-photoreal-2.0.safetensors [fdcf65e7]
 - dreamshaper_6BakedVae.safetensors [114c8abb]
 - dreamshaper_7.safetensors [5cf5ae06]
 - dreamshaper_8.safetensors [9d40847d]
 - edgeOfRealism_eorV20.safetensors [3ed5de15]
 - EimisAnimeDiffusion_V1.ckpt [4f828a15]
 - elldreths-vivid-mix.safetensors [342d9d26]
+- epicphotogasm_xPlusPlus.safetensors [1a8f6d35]
 - epicrealism_naturalSinRC1VAE.safetensors [90a4c676]
+- epicrealism_pureEvolutionV3.safetensors [42c8440c]
 - ICantBelieveItsNotPhotography_seco.safetensors [4e7a3dfd]
+- indigoFurryMix_v75Hybrid.safetensors [91208cbb]
 - juggernaut_aftermath.safetensors [5e20c455]
 - lofi_v4.safetensors [ccc204d6]
 - lyriel_v16.safetensors [68fceea2]
 - majicmixRealistic_v4.safetensors [29d0de58]
 - mechamix_v10.safetensors [ee685731]
 - meinamix_meinaV9.safetensors [2ec66ab0]
 - meinamix_meinaV11.safetensors [b56ce717]
@@ -745,15 +767,15 @@
 | sampling_method  | DPM++ 2M Karras                       | Select from the list of methods          |
 | sampling_steps   | 25                                    | Min: 1, Max: 30                          |
 | width            | 512                                   | Min: 50, Max: 1024                       |
 | height           | 512                                   | Min: 50, Max: 1024                       |
 | cfg_scale        | 7                                     | Min: 1, Max: 20                          |
 
 <a id="prodia-stablediffusion-xl"></a>
-## Usage Prodia Stable-Diffusion XL
+## Usage Prodia Stable-Diffusion XL (PRO)
 
 ```python
 import json
 from gpti import prodia
 
 res = prodia.stablediffusion_xl(prompt="Friends gathered around a bonfire in an ancient forest. Laughter, stories, and a starry sky paint an unforgettable moment of connection beneath the shadows of the mountains.", data={
     "prompt_negative": "",
@@ -794,19 +816,21 @@
 }
 ```
 
 #### Models
 
 List of models:
 
-- sd_xl_base_1.0.safetensors [be9edd61]
 - dreamshaperXL10_alpha2.safetensors [c8afe2ef]
 - dynavisionXL_0411.safetensors [c39cc051]
 - juggernautXL_v45.safetensors [e75f5471]
 - realismEngineSDXL_v10.safetensors [af771c3f]
+- sd_xl_base_1.0.safetensors [be9edd61]
+- sd_xl_base_1.0_inpainting_0.1.safetensors [5679a81a]
+- turbovisionXL_v431.safetensors [78890989]
 
 #### Methods
 
 List of methods:
 
 - DPM++ 2M Karras
 - Euler
@@ -835,15 +859,15 @@
 | sampling_method  | DPM++ 2M Karras                  | Select from the list of methods          |
 | sampling_steps   | 25                               | Min: 1, Max: 30                          |
 | width            | 1024                             | Min: 512, Max: 1536                      |
 | height           | 1024                             | Min: 512, Max: 1536                      |
 | cfg_scale        | 7                                | Min: 1, Max: 20                          |
 
 <a id="pixart-a"></a>
-## Usage Pixart-A
+## Usage Pixart-A (PRO)
 
 ```python
 import json
 from gpti import pixart
 
 res = pixart.a(prompt="An urban landscape bathed in the sunset, where the warm tones of the sun reflect on modern buildings and the orange and purple sky. In the foreground, there's a group of friends gathered on a rooftop, laughing and enjoying the moment. Their expressions radiate joy and camaraderie as they embrace and point towards something on the horizon. The scene is enveloped in a nostalgic and emotional aura that conveys the beauty of friendship and the warmth of the sunset in a futuristic city with touches of anime style.", data={
     "prompt_negative": "",
@@ -899,15 +923,15 @@
 | height               | 1024         | Min: 256, Max: 2048                                  |
 | dpm_guidance_scale   | 4.5          | Min: 1, Max: 10                                      |
 | dpm_inference_steps  | 14           | Min: 5, Max: 40                                      |
 | sa_guidance_scale    | 3            | Min: 1, Max: 10                                      |
 | sa_inference_steps   | 25           | Min: 10, Max: 40                                     |
 
 <a id="pixart-lcm"></a>
-## Usage Pixart-LCM
+## Usage Pixart-LCM (PRO)
 
 ```python
 import json
 from gpti import pixart
 
 res = pixart.lcm(prompt="An urban landscape bathed in the sunset, where the warm tones of the sun reflect on modern buildings and the orange and purple sky. In the foreground, there's a group of friends gathered on a rooftop, laughing and enjoying the moment. Their expressions radiate joy and camaraderie as they embrace and point towards something on the horizon. The scene is enveloped in a nostalgic and emotional aura that conveys the beauty of friendship and the warmth of the sunset in a futuristic city with touches of anime style.", data={
     "prompt_negative": "",
@@ -1025,15 +1049,15 @@
 
 | Parameter         | Default | Description                           |
 |-------------------|---------|---------------------------------------|
 | prompt_negative   |         | Indicates what the AI should not do    |
 | guidance_scale    | 9       | Min: 0 Max: 50                        |
 
 <a id="stablediffusion-xl"></a>
-## Usage Stable-Diffusion XL
+## Usage Stable-Diffusion XL (PRO)
 
 ```python
 import json
 from gpti import stablediffusion
 
 res = stablediffusion.xl(prompt="An serene sunset landscape where a river winds through gentle hills covered in trees. The sky is tinged with warm and soft tones, with scattered clouds reflecting the last glimmers of the sun.", data={
     "prompt_negative": "",
@@ -1102,15 +1126,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="render3d"></a>
-## Usage Render3D
+## Usage Render3D (PRO)
 
 ```python
 import json
 from gpti import render3d
 
 res = render3d(prompt="In a remote corner of the galaxy, a star agonizes in its final stage of life. Its brightness, once dazzling, now fades slowly into the void of space, while a bright nebula forms around it.", data={
     "prompt_negative": ""
@@ -1136,15 +1160,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="pixelart"></a>
-## Usage PixelArt
+## Usage PixelArt (PRO)
 
 ```python
 import json
 from gpti import pixelart
 
 res = pixelart(prompt="A coastal city in the golden hour of the sunset. The sun slowly slips toward the horizon, tinting the sky with golden and pink hues. Skyscrapers stand out against this heavenly backdrop, reflecting the light in their glass windows. In the streets, lights flicker timidly, getting ready to illuminate the night.", data={
     "prompt_negative": ""
@@ -1169,28 +1193,121 @@
     },
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
+<a id="animagine-xl"></a>
+## Usage Animagine-XL (PRO)
+
+```python
+import json
+from gpti import animagine
+
+res = animagine(prompt="An anime girl surrounded by cherry blossoms", data={
+    "prompt_negative": "",
+    "quality_tags": "Standard",
+    "style_present": "(None)",
+    "width": 1024,
+    "height": 1024,
+    "strength": 0.5,
+    "upscale": 1.5,
+    "sampler": "Euler a",
+    "guidance_scale": 7,
+    "inference_steps": 28
+})
+
+if res.error != None:
+    print(json.dumps(res.error))
+else:
+    print(json.dumps(res.result))
+```
+
+#### JSON
+
+```json
+{
+    "code": 200,
+    "status": true,
+    "prompt": "An anime girl surrounded by cherry blossoms",
+    "model": "Animagine-XL",
+    "data": {
+        "prompt_negative": "",
+        "quality_tags": "Standard",
+        "style_present": "(None)",
+        "width": 1024,
+        "height": 1024,
+        "strength": 0.5,
+        "upscale": 1.5,
+        "sampler": "Euler a",
+        "guidance_scale": 7,
+        "inference_steps": 28
+    },
+    "images": [
+        "data:image/jpeg;base64,..."
+    ]
+}
+```
+
+<a id="playground"></a>
+## Usage Playground (PRO)
+
+```python
+import json
+from gpti import playground
+
+res = playground(prompt="An illustration of a red owl with bright blue eye", data={
+    "prompt_negative": "",
+    "width": 1024,
+    "height": 1024,
+    "guidance_scale": 3
+})
+
+if res.error != None:
+    print(json.dumps(res.error))
+else:
+    print(json.dumps(res.result))
+```
+
+#### JSON
+
+```json
+{
+    "code": 200,
+    "status": true,
+    "prompt": "An illustration of a red owl with bright blue eyes.",
+    "model": "Playground",
+    "data": {
+        "prompt_negative": "",
+        "width": 1024,
+        "height": 1024,
+        "guidance_scale": 3
+    },
+    "images": [
+        "data:image/jpeg;base64,..."
+    ]
+}
+```
+
 ## API Reference
 
-At present, the API doesn't have any access restrictions or usage limits. For further details and examples, please refer to the complete [documentation](https://nexra.aryahcr.cc/).
+Currently, some models require your credentials to access them, while others are free. For more details and examples, please refer to the complete [documentation](https://nexra.aryahcr.cc/).
 
 #### Code Errors
 
 These are the error codes that will be presented in case the API fails.
 
-| Code | Error                  | Description                                    |
-|------|------------------------|------------------------------------------------|
-| 400  | BAD_REQUEST            | Not all parameters have been entered correctly |
-| 500  | INTERNAL_SERVER_ERROR  | The server has experienced failures             |
-| 200  |                        | The API worked without issues                    |
+| Code | Error                  | Description                                           |
+|------|------------------------|-------------------------------------------------------|
+| 400  | BAD_REQUEST            | Not all parameters have been entered correctly        |
+| 500  | INTERNAL_SERVER_ERROR  | The server has experienced failures                   |
+| 200  |                        | The API worked without issues                          |
+| 403  | FORBIDDEN              | Your API key has expired and needs to be renewed      |
+| 401  | UNAUTHORIZED           | API credentials are required                          |
+
 
 ## ☕ Do you want to support this project?
 
 If this package has helped you save time or solve a problem, consider inviting me for a coffee through Ko-fi. Your support helps me maintain and improve this project for you and other users like you. Furthermore, each donation contributes to the creation and free availability of more AI models in the future. Every small donation counts and is greatly appreciated!
 
-[![Support on Ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/yandricr)
-
-Remember: Programmers don't need coffee... but it helps a lot! 😉
+[![Support on Ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/yandricr)
```

### Comparing `gpti-1.3/gpti/__init__.py` & `gpti-1.4/gpti/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 import requests
 import json
 
+cred = {
+    "x-nexra-user": None,
+    "x-nexra-secret": None
+}
+
+def nexra(user, secret):
+    cred["x-nexra-secret"] = secret
+    cred["x-nexra-user"] = user
+
+
 class gpt:
     error = None
     result = None
     def __init__(self, messages=[], prompt="", model="", markdown=False) -> None:
         try:
             headers = {
                 "Content-Type": "application/json"
@@ -295,63 +305,82 @@
             return self.error
         def result(self):
             return self.result
     class v2:
         error = None
         result = None
         def __init__(self, prompt="", data={
-            "gpu": "",
-            "prompt_improvement": ""
+            "prompt_negative": "",
+            "width": "",
+            "height": "",
+            "guidance_scale": ""
         }) -> None:
             try:
                 headers = {
                     "Content-Type": "application/json"
                 }
+                headers.update(cred)
                 err = False
                 
                 md = {
-                    "gpu": False,
-                    "prompt_improvement": False
+                    "prompt_negative": "",
+                    "width": 1024,
+                    "height": 1024,
+                    "guidance_scale": 6
                 }
 
                 try:
                     prompt = prompt if prompt is not None else ""
                 except Exception as e:
                     prompt = ""
 
                 try :
-                    if data.get("gpu") != None:
-                        md["gpu"] = data.get("gpu")
+                    if data.get("prompt_negative") != None:
+                        md["prompt_negative"] = data.get("prompt_negative")
                     else:
-                        md["gpu"] = False
+                        md["prompt_negative"] = ""
 
-                    if data.get("prompt_improvement") != None:
-                        md["prompt_improvement"] = data.get("prompt_improvement")
+                    if data.get("width") != None:
+                        md["width"] = data.get("width")
+                    else:
+                        md["width"] = 1024
+
+                    if data.get("height") != None:
+                        md["height"] = data.get("height")
                     else:
-                        md["prompt_improvement"] = False
+                        md["height"] = 1024
+
+                    if data.get("guidance_scale") != None:
+                        md["guidance_scale"] = data.get("guidance_scale")
+                    else:
+                        md["guidance_scale"] = 6
                 except Exception as e:
                     md = {
-                        "gpu": False,
-                        "prompt_improvement": False
+                        "prompt_negative": "",
+                        "width": 1024,
+                        "height": 1024,
+                        "guidance_scale": 6
                     }
 
                 data = {}
                 try:
                     data = json.dumps({
                         "prompt": prompt,
                         "model": "dalle2",
                         "data": md
                     })
                 except Exception as e:
                     data = json.dumps({
                         "prompt": "",
                         "model": "dalle2",
                         "data": {
-                            "gpu": False,
-                            "prompt_improvement": False
+                            "prompt_negative": "",
+                            "width": 1024,
+                            "height": 1024,
+                            "guidance_scale": 6
                         }
                     })
                 
                 response = requests.post(url="https://nexra.aryahcr.cc/api/image/complements", headers=headers, data=data)
                 if response.status_code == 200:
                     err = None
                     result = None
@@ -861,14 +890,15 @@
             "height": "",
             "cfg_scale": ""
         }) -> None:
             try:
                 headers = {
                     "Content-Type": "application/json"
                 }
+                headers.update(cred)
 
                 try:
                     prompt = prompt if prompt is not None else ""
                 except Exception as e:
                     prompt = ""
 
                 md = {
@@ -1038,14 +1068,15 @@
             "sa_guidance_scale": "",
             "sa_inference_steps": ""
         }) -> None:
             try:
                 headers = {
                     "Content-Type": "application/json"
                 }
+                headers.update(cred)
 
                 try:
                     prompt = prompt if prompt is not None else ""
                 except Exception as e:
                     prompt = ""
 
                 md = {
@@ -1225,14 +1256,15 @@
             "height": "",
             "lcm_inference_steps": ""
         }) -> None:
             try:
                 headers = {
                     "Content-Type": "application/json"
                 }
+                headers.update(cred)
 
                 try:
                     prompt = prompt if prompt is not None else ""
                 except Exception as e:
                     prompt = ""
 
                 md = {
@@ -1603,14 +1635,15 @@
             "image_style": "",
             "guidance_scale": ""
         }) -> None:
             try:
                 headers = {
                     "Content-Type": "application/json"
                 }
+                headers.update(cred)
 
                 try:
                     prompt = prompt if prompt is not None else ""
                 except Exception as e:
                     prompt = ""
 
                 md = {
@@ -2222,14 +2255,15 @@
     def __init__(self, prompt="", data={
         "prompt_negative": ""
     }) -> None:
         try:
             headers = {
                 "Content-Type": "application/json"
             }
+            headers.update(cred)
 
             try:
                 prompt = prompt if prompt is not None else ""
             except Exception as e:
                 prompt = ""
 
             md = {
@@ -2332,24 +2366,375 @@
             self.result = None
         pass
     def error(self):
         return self.error
     def result(self):
         return self.result
 
+class animagine():
+    error = None
+    result = None
+    def __init__(self, prompt="", data={
+        "prompt_negative": "",
+        "width": "",
+        "height": "",
+        "guidance_scale": "",
+        "quality_tags": "",
+        "style_present": "",
+        "strength": "",
+        "upscale": "",
+        "sampler": "",
+        "inference_steps": "",
+    }) -> None:
+        try:
+            headers = {
+                "Content-Type": "application/json"
+            }
+            headers.update(cred)
+
+            try:
+                prompt = prompt if prompt is not None else ""
+            except Exception as e:
+                prompt = ""
+
+            md = {
+                "prompt_negative": "",
+                "width": 1024,
+                "height": 1024,
+                "guidance_scale": 7,
+                "quality_tags": "Standard",
+                "style_present": "(None)",
+                "strength": 0.5,
+                "upscale": 1.5,
+                "sampler": "Euler a",
+                "inference_steps": 28,
+            }
+
+            try :
+                if data.get("prompt_negative") != None:
+                    md["prompt_negative"] = data.get("prompt_negative")
+                else:
+                    md["prompt_negative"] = ""
+                
+                if data.get("width") != None:
+                    md["width"] = data.get("width")
+                else:
+                    md["width"] = 1024
+                
+                if data.get("height") != None:
+                    md["height"] = data.get("height")
+                else:
+                    md["height"] = 1024
+                
+                if data.get("guidance_scale") != None:
+                    md["guidance_scale"] = data.get("guidance_scale")
+                else:
+                    md["guidance_scale"] = 7
+                
+                if data.get("quality_tags") != None:
+                    md["quality_tags"] = data.get("quality_tags")
+                else:
+                    md["quality_tags"] = "Standard"
+                
+                if data.get("style_present") != None:
+                    md["style_present"] = data.get("style_present")
+                else:
+                    md["style_present"] = "(None)"
+                
+                if data.get("strength") != None:
+                    md["strength"] = data.get("strength")
+                else:
+                    md["strength"] = 0.5
+                
+                if data.get("upscale") != None:
+                    md["upscale"] = data.get("upscale")
+                else:
+                    md["upscale"] = 1.5
+                
+                if data.get("sampler") != None:
+                    md["sampler"] = data.get("sampler")
+                else:
+                    md["sampler"] = "Euler a"
+                
+                if data.get("inference_steps") != None:
+                    md["inference_steps"] = data.get("inference_steps")
+                else:
+                    md["inference_steps"] = 28
+            except Exception as e:
+                md = {
+                    "prompt_negative": "",
+                    "width": 1024,
+                    "height": 1024,
+                    "guidance_scale": 7,
+                    "quality_tags": "Standard",
+                    "style_present": "(None)",
+                    "strength": 0.5,
+                    "upscale": 1.5,
+                    "sampler": "Euler a",
+                    "inference_steps": 28,
+                }
+
+            data = {}
+            try:
+                data = json.dumps({
+                    "prompt": prompt,
+                    "model": "animagine-xl",
+                    "data": md
+                })
+            except Exception as e:
+                data = json.dumps({
+                    "prompt": "",
+                    "model": "animagine-xl",
+                    "data": {
+                        "prompt_negative": "",
+                        "width": 1024,
+                        "height": 1024,
+                        "guidance_scale": 7,
+                        "quality_tags": "Standard",
+                        "style_present": "(None)",
+                        "strength": 0.5,
+                        "upscale": 1.5,
+                        "sampler": "Euler a",
+                        "inference_steps": 28,
+                    }
+                })
+            
+            response = requests.post(url="https://nexra.aryahcr.cc/api/image/complements", headers=headers, data=data)
+            if response.status_code == 200:
+                err = None
+                result = None
+
+                count = -1
+                for i in range(len(response.text)):
+                    if count <= -1:
+                        if response.text[i] == "{":
+                            count = i
+                    else:
+                        break
+                
+                if count <= -1:
+                    err = {
+                        "code": 500,
+                        "status": False,
+                        "error": "INTERNAL_SERVER_ERROR",
+                        "message": "general (unknown) error"
+                    }
+                    result = None
+                else:
+                    try:
+                        js = response.text[count:]
+                        js = json.loads(js)
+                        if js != None and js["code"] != None and js["code"] == 200 and js["status"] != None and js["status"] == True:
+                            result = js
+                            err = None
+                        else:
+                            err = js
+                            result = None
+                    except Exception as e:
+                        err = {
+                            "code": 500,
+                            "status": False,
+                            "error": "INTERNAL_SERVER_ERROR",
+                            "message": "general (unknown) error"
+                        }
+                        result = None
+
+                    if result == None and err != None:
+                        self.error = err
+                        self.result = None
+                    else:
+                        self.result = result
+                        self.error = None
+            else:
+                data_err = {}
+                try:
+                    data_err = json.loads(response.text)
+                except Exception as e:
+                    data_err = {
+                        "code": 500,
+                        "status": False,
+                        "error": "INTERNAL_SERVER_ERROR",
+                        "message": "general (unknown) error"
+                    }
+                
+                self.error = data_err
+                self.result = None
+        except Exception as e:
+            self.error = {
+                "code": 500,
+                "status": False,
+                "error": "INTERNAL_SERVER_ERROR",
+                "message": "general (unknown) error"
+            }
+            self.result = None
+        pass
+    def error(self):
+        return self.error
+    def result(self):
+        return self.result
+
+class playground():
+    error = None
+    result = None
+    def __init__(self, prompt="", data={
+        "prompt_negative": "",
+        "width": "",
+        "height": "",
+        "guidance_scale": ""
+    }) -> None:
+        try:
+            headers = {
+                "Content-Type": "application/json"
+            }
+            headers.update(cred)
+
+            try:
+                prompt = prompt if prompt is not None else ""
+            except Exception as e:
+                prompt = ""
+
+            md = {
+                "prompt_negative": "",
+                "width": 1024,
+                "height": 1024,
+                "guidance_scale": 3
+            }
+
+            try :
+                if data.get("prompt_negative") != None:
+                    md["prompt_negative"] = data.get("prompt_negative")
+                else:
+                    md["prompt_negative"] = ""
+                
+                if data.get("width") != None:
+                    md["width"] = data.get("width")
+                else:
+                    md["width"] = 1024
+                
+                if data.get("height") != None:
+                    md["height"] = data.get("height")
+                else:
+                    md["height"] = 1024
+                
+                if data.get("guidance_scale") != None:
+                    md["guidance_scale"] = data.get("guidance_scale")
+                else:
+                    md["guidance_scale"] = 3
+            except Exception as e:
+                md = {
+                    "prompt_negative": "",
+                    "width": 1024,
+                    "height": 1024,
+                    "guidance_scale": 3
+                }
+
+            data = {}
+            try:
+                data = json.dumps({
+                    "prompt": prompt,
+                    "model": "playground",
+                    "data": md
+                })
+            except Exception as e:
+                data = json.dumps({
+                    "prompt": "",
+                    "model": "playground",
+                    "data": {
+                        "prompt_negative": "",
+                        "width": 1024,
+                        "height": 1024,
+                        "guidance_scale": 3
+                    }
+                })
+            
+            response = requests.post(url="https://nexra.aryahcr.cc/api/image/complements", headers=headers, data=data)
+            if response.status_code == 200:
+                err = None
+                result = None
+
+                count = -1
+                for i in range(len(response.text)):
+                    if count <= -1:
+                        if response.text[i] == "{":
+                            count = i
+                    else:
+                        break
+                
+                if count <= -1:
+                    err = {
+                        "code": 500,
+                        "status": False,
+                        "error": "INTERNAL_SERVER_ERROR",
+                        "message": "general (unknown) error"
+                    }
+                    result = None
+                else:
+                    try:
+                        js = response.text[count:]
+                        js = json.loads(js)
+                        if js != None and js["code"] != None and js["code"] == 200 and js["status"] != None and js["status"] == True:
+                            result = js
+                            err = None
+                        else:
+                            err = js
+                            result = None
+                    except Exception as e:
+                        err = {
+                            "code": 500,
+                            "status": False,
+                            "error": "INTERNAL_SERVER_ERROR",
+                            "message": "general (unknown) error"
+                        }
+                        result = None
+
+                    if result == None and err != None:
+                        self.error = err
+                        self.result = None
+                    else:
+                        self.result = result
+                        self.error = None
+            else:
+                data_err = {}
+                try:
+                    data_err = json.loads(response.text)
+                except Exception as e:
+                    data_err = {
+                        "code": 500,
+                        "status": False,
+                        "error": "INTERNAL_SERVER_ERROR",
+                        "message": "general (unknown) error"
+                    }
+                
+                self.error = data_err
+                self.result = None
+        except Exception as e:
+            self.error = {
+                "code": 500,
+                "status": False,
+                "error": "INTERNAL_SERVER_ERROR",
+                "message": "general (unknown) error"
+            }
+            self.result = None
+        pass
+    def error(self):
+        return self.error
+    def result(self):
+        return self.result
+
 class pixelart():
     error = None
     result = None
     def __init__(self, prompt="", data={
         "prompt_negative": ""
     }) -> None:
         try:
             headers = {
                 "Content-Type": "application/json"
             }
+            headers.update(cred)
 
             try:
                 prompt = prompt if prompt is not None else ""
             except Exception as e:
                 prompt = ""
 
             md = {
```

### Comparing `gpti-1.3/gpti.egg-info/PKG-INFO` & `gpti-1.4/gpti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gpti
-Version: 1.3
+Version: 1.4
 Summary: This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT
 Home-page: https://github.com/yandricr/gpti-py/
 Author: yandricr
 Author-email: yandribret@gmail.com
 License: MIT
 Project-URL: Documentation, https://nexra.aryahcr.cc/
 Project-URL: Funding, https://ko-fi.com/yandricr
 Project-URL: Source, https://github.com/yandricr/gpti-py/
-Keywords: gpt gpt-3 gpt-3.5 gpt-4 gpti gpt-free ai generate-image prodia bing chat stream dalle dalle-2 llama-2 stable-diffusion pixart EMI render3d pixel-art
+Keywords: gpt gpt-3 gpt-3.5 gpt-4 gpti gpt-free ai generate-image prodia bing chat stream dalle dalle-2 llama-2 stable-diffusion pixart EMI render3d pixel-art playground animagine-xl
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 
 # GPTI
 
 ![Downloads](https://img.shields.io/pypi/dw/gpti?style=for-the-badge) ![License](https://img.shields.io/pypi/l/gpti?style=for-the-badge) [![Contributors](https://img.shields.io/github/contributors/yandricr/gpti-py?style=for-the-badge)](https://github.com/yandricr/gpti-py/graphs/contributors) [![Size Package](https://img.shields.io/github/languages/code-size/yandricr/gpti-py?style=for-the-badge)](https://github.com/yandricr/gpti-py) ![Python](https://img.shields.io/badge/python-%233776AB.svg?style=for-the-badge&logo=python&logoColor=white) [![Ko-Fi](https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/yandricr)
 
 This package simplifies your interaction with various GPT models, eliminating the need for tokens or other methods to access GPT. It also allows you to use three artificial intelligences to generate images: DALL·E, Prodia and more, all of this without restrictions or limits
@@ -33,29 +34,39 @@
 GPTI provides access to a variety of artificial intelligence models to meet various needs. Currently, the available models include:
 
 - [**ChatGPT**](#gpt)
 - [**ChatGPT Web**](#gptweb)
 - [**Bing**](#bing)
 - [**LLaMA-2**](#llama2)
 - [**DALL·E**](#dalle)
-- [**DALL-E 2**](#dalle2)
+- [**DALL-E 2**](#dalle2) (PRO)
 - [**DALL-E Mini**](#dalle-mini)
 - [**Prodia**](#prodia)
 - [**Prodia Stable-Diffusion**](#prodia-stablediffusion)
-- [**Prodia Stable-Diffusion XL**](#prodia-stablediffusion-xl)
-- [**Pixart-A**](#pixart-a)
-- [**Pixart-LCM**](#pixart-lcm)
+- [**Prodia Stable-Diffusion XL**](#prodia-stablediffusion-xl) (PRO)
+- [**Pixart-A**](#pixart-a) (PRO)
+- [**Pixart-LCM**](#pixart-lcm) (PRO)
 - [**Stable-Diffusion 1.5**](#stablediffusion-1.5)
 - [**Stable-Diffusion 2.1**](#stablediffusion-2.1)
-- [**Stable-Diffusion XL**](#stablediffusion-xl)
+- [**Stable-Diffusion XL**](#stablediffusion-xl) (PRO)
 - [**EMI**](#emi)
-- [**Render3D**](#render3d)
-- [**PixelArt**](#pixelart)
+- [**Render3D**](#render3d) (PRO)
+- [**PixelArt**](#pixelart) (PRO)
+- [**Animagine-XL**](#animagine-xl) (PRO)
+- [**Playground**](#playground) (PRO)
 
-These are just some examples of the models available in this package. I will continue expanding to include an even greater variety of models.
+## Api key
+
+If you want to access the premium models, enter your credentials. You can obtain them by [clicking here](https://nexra.aryahcr.cc/api-key/en).
+
+```python
+from gpti import nexra
+
+nexra("user-xxxxxxxx", "nx-xxxxxxx-xxxxx-xxxxx");
+```
 
 <a id="gpt"></a>
 ## Usage GPT
 
 ```python
 import json
 from gpti import gpt
@@ -433,15 +444,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="dalle2"></a>
-## Usage DALL·E 2
+## Usage DALL·E 2 (PRO)
 
 ```python
 import json
 from gpti import dalle
 
 res = dalle.v2(prompt="An extensive green valley stretches toward imposing mountains, adorned with meadows and a winding stream. The morning sun paints the sky with warm tones, illuminating the landscape with a serenity that invites contemplation and peace.", data={
     "gpu": False,
@@ -555,14 +566,16 @@
 - amIReal_V41.safetensors [0a8a2e61]
 - analog-diffusion-1.0.ckpt [9ca13f02]
 - anythingv3_0-pruned.ckpt [2700c435]
 - anything-v4.5-pruned.ckpt [65745d25]
 - anythingV5_PrtRE.safetensors [893e49b9]
 - AOM3A3_orangemixs.safetensors [9600da17]
 - blazing_drive_v10g.safetensors [ca1c1eab]
+- breakdomain_I2428.safetensors [43cc7d2f]
+- breakdomain_M2150.safetensors [15f7afca]
 - cetusMix_Version35.safetensors [de2f2560]
 - childrensStories_v13D.safetensors [9dfaabcb]
 - childrensStories_v1SemiReal.safetensors [a1c56dbb]
 - childrensStories_v1ToonAnime.safetensors [2ec7b88b]
 - Counterfeit_v30.safetensors [9e2a8f19]
 - cuteyukimixAdorable_midchapter3.safetensors [04bdffe6]
 - cyberrealistic_v33.safetensors [82b0d085]
@@ -574,16 +587,19 @@
 - dreamlike-photoreal-2.0.safetensors [fdcf65e7]
 - dreamshaper_6BakedVae.safetensors [114c8abb]
 - dreamshaper_7.safetensors [5cf5ae06]
 - dreamshaper_8.safetensors [9d40847d]
 - edgeOfRealism_eorV20.safetensors [3ed5de15]
 - EimisAnimeDiffusion_V1.ckpt [4f828a15]
 - elldreths-vivid-mix.safetensors [342d9d26]
+- epicphotogasm_xPlusPlus.safetensors [1a8f6d35]
 - epicrealism_naturalSinRC1VAE.safetensors [90a4c676]
+- epicrealism_pureEvolutionV3.safetensors [42c8440c]
 - ICantBelieveItsNotPhotography_seco.safetensors [4e7a3dfd]
+- indigoFurryMix_v75Hybrid.safetensors [91208cbb]
 - juggernaut_aftermath.safetensors [5e20c455]
 - lofi_v4.safetensors [ccc204d6]
 - lyriel_v16.safetensors [68fceea2]
 - majicmixRealistic_v4.safetensors [29d0de58]
 - mechamix_v10.safetensors [ee685731]
 - meinamix_meinaV9.safetensors [2ec66ab0]
 - meinamix_meinaV11.safetensors [b56ce717]
@@ -597,14 +613,16 @@
 - Realistic_Vision_V4.0.safetensors [29a7afaa]
 - Realistic_Vision_V5.0.safetensors [614d1063]
 - redshift_diffusion-V10.safetensors [1400e684]
 - revAnimated_v122.safetensors [3f4fefd9]
 - rundiffusionFX25D_v10.safetensors [cd12b0ee]
 - rundiffusionFX_v10.safetensors [cd4e694d]
 - sdv1_4.ckpt [7460a6fa]
+- v1-5-pruned-emaonly.safetensors [d7049739]
+- v1-5-inpainting.safetensors [21c7ab71]
 - shoninsBeautiful_v10.safetensors [25d8c546]
 - theallys-mix-ii-churned.safetensors [5d9225a4]
 - timeless-1.0.ckpt [7c4971d4]
 - toonyou_beta6.safetensors [980f6b15]
 
 #### Parameters
 
@@ -662,24 +680,26 @@
 }
 ```
 
 #### Models
 
 List of models
 
-- absolutereality_v181.safetensors [3d9d4d2b]
 - 3Guofeng3_v34.safetensors [50f420de]
 - absolutereality_V16.safetensors [37db0fc3]
+- absolutereality_v181.safetensors [3d9d4d2b]
 - amIReal_V41.safetensors [0a8a2e61]
 - analog-diffusion-1.0.ckpt [9ca13f02]
 - anythingv3_0-pruned.ckpt [2700c435]
 - anything-v4.5-pruned.ckpt [65745d25]
 - anythingV5_PrtRE.safetensors [893e49b9]
 - AOM3A3_orangemixs.safetensors [9600da17]
 - blazing_drive_v10g.safetensors [ca1c1eab]
+- breakdomain_I2428.safetensors [43cc7d2f]
+- breakdomain_M2150.safetensors [15f7afca]
 - cetusMix_Version35.safetensors [de2f2560]
 - childrensStories_v13D.safetensors [9dfaabcb]
 - childrensStories_v1SemiReal.safetensors [a1c56dbb]
 - childrensStories_v1ToonAnime.safetensors [2ec7b88b]
 - Counterfeit_v30.safetensors [9e2a8f19]
 - cuteyukimixAdorable_midchapter3.safetensors [04bdffe6]
 - cyberrealistic_v33.safetensors [82b0d085]
@@ -691,16 +711,19 @@
 - dreamlike-photoreal-2.0.safetensors [fdcf65e7]
 - dreamshaper_6BakedVae.safetensors [114c8abb]
 - dreamshaper_7.safetensors [5cf5ae06]
 - dreamshaper_8.safetensors [9d40847d]
 - edgeOfRealism_eorV20.safetensors [3ed5de15]
 - EimisAnimeDiffusion_V1.ckpt [4f828a15]
 - elldreths-vivid-mix.safetensors [342d9d26]
+- epicphotogasm_xPlusPlus.safetensors [1a8f6d35]
 - epicrealism_naturalSinRC1VAE.safetensors [90a4c676]
+- epicrealism_pureEvolutionV3.safetensors [42c8440c]
 - ICantBelieveItsNotPhotography_seco.safetensors [4e7a3dfd]
+- indigoFurryMix_v75Hybrid.safetensors [91208cbb]
 - juggernaut_aftermath.safetensors [5e20c455]
 - lofi_v4.safetensors [ccc204d6]
 - lyriel_v16.safetensors [68fceea2]
 - majicmixRealistic_v4.safetensors [29d0de58]
 - mechamix_v10.safetensors [ee685731]
 - meinamix_meinaV9.safetensors [2ec66ab0]
 - meinamix_meinaV11.safetensors [b56ce717]
@@ -760,15 +783,15 @@
 | sampling_method  | DPM++ 2M Karras                       | Select from the list of methods          |
 | sampling_steps   | 25                                    | Min: 1, Max: 30                          |
 | width            | 512                                   | Min: 50, Max: 1024                       |
 | height           | 512                                   | Min: 50, Max: 1024                       |
 | cfg_scale        | 7                                     | Min: 1, Max: 20                          |
 
 <a id="prodia-stablediffusion-xl"></a>
-## Usage Prodia Stable-Diffusion XL
+## Usage Prodia Stable-Diffusion XL (PRO)
 
 ```python
 import json
 from gpti import prodia
 
 res = prodia.stablediffusion_xl(prompt="Friends gathered around a bonfire in an ancient forest. Laughter, stories, and a starry sky paint an unforgettable moment of connection beneath the shadows of the mountains.", data={
     "prompt_negative": "",
@@ -809,19 +832,21 @@
 }
 ```
 
 #### Models
 
 List of models:
 
-- sd_xl_base_1.0.safetensors [be9edd61]
 - dreamshaperXL10_alpha2.safetensors [c8afe2ef]
 - dynavisionXL_0411.safetensors [c39cc051]
 - juggernautXL_v45.safetensors [e75f5471]
 - realismEngineSDXL_v10.safetensors [af771c3f]
+- sd_xl_base_1.0.safetensors [be9edd61]
+- sd_xl_base_1.0_inpainting_0.1.safetensors [5679a81a]
+- turbovisionXL_v431.safetensors [78890989]
 
 #### Methods
 
 List of methods:
 
 - DPM++ 2M Karras
 - Euler
@@ -850,15 +875,15 @@
 | sampling_method  | DPM++ 2M Karras                  | Select from the list of methods          |
 | sampling_steps   | 25                               | Min: 1, Max: 30                          |
 | width            | 1024                             | Min: 512, Max: 1536                      |
 | height           | 1024                             | Min: 512, Max: 1536                      |
 | cfg_scale        | 7                                | Min: 1, Max: 20                          |
 
 <a id="pixart-a"></a>
-## Usage Pixart-A
+## Usage Pixart-A (PRO)
 
 ```python
 import json
 from gpti import pixart
 
 res = pixart.a(prompt="An urban landscape bathed in the sunset, where the warm tones of the sun reflect on modern buildings and the orange and purple sky. In the foreground, there's a group of friends gathered on a rooftop, laughing and enjoying the moment. Their expressions radiate joy and camaraderie as they embrace and point towards something on the horizon. The scene is enveloped in a nostalgic and emotional aura that conveys the beauty of friendship and the warmth of the sunset in a futuristic city with touches of anime style.", data={
     "prompt_negative": "",
@@ -914,15 +939,15 @@
 | height               | 1024         | Min: 256, Max: 2048                                  |
 | dpm_guidance_scale   | 4.5          | Min: 1, Max: 10                                      |
 | dpm_inference_steps  | 14           | Min: 5, Max: 40                                      |
 | sa_guidance_scale    | 3            | Min: 1, Max: 10                                      |
 | sa_inference_steps   | 25           | Min: 10, Max: 40                                     |
 
 <a id="pixart-lcm"></a>
-## Usage Pixart-LCM
+## Usage Pixart-LCM (PRO)
 
 ```python
 import json
 from gpti import pixart
 
 res = pixart.lcm(prompt="An urban landscape bathed in the sunset, where the warm tones of the sun reflect on modern buildings and the orange and purple sky. In the foreground, there's a group of friends gathered on a rooftop, laughing and enjoying the moment. Their expressions radiate joy and camaraderie as they embrace and point towards something on the horizon. The scene is enveloped in a nostalgic and emotional aura that conveys the beauty of friendship and the warmth of the sunset in a futuristic city with touches of anime style.", data={
     "prompt_negative": "",
@@ -1040,15 +1065,15 @@
 
 | Parameter         | Default | Description                           |
 |-------------------|---------|---------------------------------------|
 | prompt_negative   |         | Indicates what the AI should not do    |
 | guidance_scale    | 9       | Min: 0 Max: 50                        |
 
 <a id="stablediffusion-xl"></a>
-## Usage Stable-Diffusion XL
+## Usage Stable-Diffusion XL (PRO)
 
 ```python
 import json
 from gpti import stablediffusion
 
 res = stablediffusion.xl(prompt="An serene sunset landscape where a river winds through gentle hills covered in trees. The sky is tinged with warm and soft tones, with scattered clouds reflecting the last glimmers of the sun.", data={
     "prompt_negative": "",
@@ -1117,15 +1142,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="render3d"></a>
-## Usage Render3D
+## Usage Render3D (PRO)
 
 ```python
 import json
 from gpti import render3d
 
 res = render3d(prompt="In a remote corner of the galaxy, a star agonizes in its final stage of life. Its brightness, once dazzling, now fades slowly into the void of space, while a bright nebula forms around it.", data={
     "prompt_negative": ""
@@ -1151,15 +1176,15 @@
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
 <a id="pixelart"></a>
-## Usage PixelArt
+## Usage PixelArt (PRO)
 
 ```python
 import json
 from gpti import pixelart
 
 res = pixelart(prompt="A coastal city in the golden hour of the sunset. The sun slowly slips toward the horizon, tinting the sky with golden and pink hues. Skyscrapers stand out against this heavenly backdrop, reflecting the light in their glass windows. In the streets, lights flicker timidly, getting ready to illuminate the night.", data={
     "prompt_negative": ""
@@ -1184,28 +1209,121 @@
     },
     "images": [
         "data:image/jpeg;base64,..."
     ]
 }
 ```
 
+<a id="animagine-xl"></a>
+## Usage Animagine-XL (PRO)
+
+```python
+import json
+from gpti import animagine
+
+res = animagine(prompt="An anime girl surrounded by cherry blossoms", data={
+    "prompt_negative": "",
+    "quality_tags": "Standard",
+    "style_present": "(None)",
+    "width": 1024,
+    "height": 1024,
+    "strength": 0.5,
+    "upscale": 1.5,
+    "sampler": "Euler a",
+    "guidance_scale": 7,
+    "inference_steps": 28
+})
+
+if res.error != None:
+    print(json.dumps(res.error))
+else:
+    print(json.dumps(res.result))
+```
+
+#### JSON
+
+```json
+{
+    "code": 200,
+    "status": true,
+    "prompt": "An anime girl surrounded by cherry blossoms",
+    "model": "Animagine-XL",
+    "data": {
+        "prompt_negative": "",
+        "quality_tags": "Standard",
+        "style_present": "(None)",
+        "width": 1024,
+        "height": 1024,
+        "strength": 0.5,
+        "upscale": 1.5,
+        "sampler": "Euler a",
+        "guidance_scale": 7,
+        "inference_steps": 28
+    },
+    "images": [
+        "data:image/jpeg;base64,..."
+    ]
+}
+```
+
+<a id="playground"></a>
+## Usage Playground (PRO)
+
+```python
+import json
+from gpti import playground
+
+res = playground(prompt="An illustration of a red owl with bright blue eye", data={
+    "prompt_negative": "",
+    "width": 1024,
+    "height": 1024,
+    "guidance_scale": 3
+})
+
+if res.error != None:
+    print(json.dumps(res.error))
+else:
+    print(json.dumps(res.result))
+```
+
+#### JSON
+
+```json
+{
+    "code": 200,
+    "status": true,
+    "prompt": "An illustration of a red owl with bright blue eyes.",
+    "model": "Playground",
+    "data": {
+        "prompt_negative": "",
+        "width": 1024,
+        "height": 1024,
+        "guidance_scale": 3
+    },
+    "images": [
+        "data:image/jpeg;base64,..."
+    ]
+}
+```
+
 ## API Reference
 
-At present, the API doesn't have any access restrictions or usage limits. For further details and examples, please refer to the complete [documentation](https://nexra.aryahcr.cc/).
+Currently, some models require your credentials to access them, while others are free. For more details and examples, please refer to the complete [documentation](https://nexra.aryahcr.cc/).
 
 #### Code Errors
 
 These are the error codes that will be presented in case the API fails.
 
-| Code | Error                  | Description                                    |
-|------|------------------------|------------------------------------------------|
-| 400  | BAD_REQUEST            | Not all parameters have been entered correctly |
-| 500  | INTERNAL_SERVER_ERROR  | The server has experienced failures             |
-| 200  |                        | The API worked without issues                    |
+| Code | Error                  | Description                                           |
+|------|------------------------|-------------------------------------------------------|
+| 400  | BAD_REQUEST            | Not all parameters have been entered correctly        |
+| 500  | INTERNAL_SERVER_ERROR  | The server has experienced failures                   |
+| 200  |                        | The API worked without issues                          |
+| 403  | FORBIDDEN              | Your API key has expired and needs to be renewed      |
+| 401  | UNAUTHORIZED           | API credentials are required                          |
+
 
 ## ☕ Do you want to support this project?
 
 If this package has helped you save time or solve a problem, consider inviting me for a coffee through Ko-fi. Your support helps me maintain and improve this project for you and other users like you. Furthermore, each donation contributes to the creation and free availability of more AI models in the future. Every small donation counts and is greatly appreciated!
 
 [![Support on Ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/yandricr)
-
-Remember: Programmers don't need coffee... but it helps a lot! 😉
```

### Comparing `gpti-1.3/setup.py` & `gpti-1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as f:
         _long_description = f.read()
 except Exception as e:
     _long_description = ''
 
 setup(
     name='gpti',
-    version='1.3',
+    version='1.4',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='yandricr',
     author_email='yandribret@gmail.com',
     description='This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT',
@@ -21,12 +21,12 @@
     long_description_content_type='text/markdown',
     url='https://github.com/yandricr/gpti-py/',
     project_urls={
         'Documentation': 'https://nexra.aryahcr.cc/',
         'Funding': 'https://ko-fi.com/yandricr',
         'Source': 'https://github.com/yandricr/gpti-py/'
     },
-    keywords='gpt gpt-3 gpt-3.5 gpt-4 gpti gpt-free ai generate-image prodia bing chat stream dalle dalle-2 llama-2 stable-diffusion pixart EMI render3d pixel-art',
+    keywords='gpt gpt-3 gpt-3.5 gpt-4 gpti gpt-free ai generate-image prodia bing chat stream dalle dalle-2 llama-2 stable-diffusion pixart EMI render3d pixel-art playground animagine-xl',
     license='MIT',
     package_data={'': ['LICENSE']},
     include_package_data=True
 )
```

