# Comparing `tmp/VideoOpinionMining-1.0.tar.gz` & `tmp/VideoOpinionMining-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VideoOpinionMining-1.0.tar", last modified: Sat Apr  6 14:21:20 2024, max compression
+gzip compressed data, was "VideoOpinionMining-1.1.tar", last modified: Sun Apr  7 12:32:32 2024, max compression
```

## Comparing `VideoOpinionMining-1.0.tar` & `VideoOpinionMining-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-06 14:21:20.759431 VideoOpinionMining-1.0/
--rw-r--r--   0 art       (1000) art       (1000)     1081 2024-04-06 12:43:21.000000 VideoOpinionMining-1.0/LICENSE
--rw-r--r--   0 art       (1000) art       (1000)     2236 2024-04-06 14:21:20.759431 VideoOpinionMining-1.0/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)     1598 2024-04-06 12:41:33.000000 VideoOpinionMining-1.0/README.md
--rw-r--r--   0 art       (1000) art       (1000)      710 2024-04-06 14:21:14.000000 VideoOpinionMining-1.0/pyproject.toml
--rw-r--r--   0 art       (1000) art       (1000)       38 2024-04-06 14:21:20.759431 VideoOpinionMining-1.0/setup.cfg
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-06 14:21:20.759431 VideoOpinionMining-1.0/src/
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-06 14:21:20.759431 VideoOpinionMining-1.0/src/VideoOpinionMining/
--rw-r--r--   0 art       (1000) art       (1000)       29 2024-04-06 13:38:23.000000 VideoOpinionMining-1.0/src/VideoOpinionMining/__init__.py
--rw-r--r--   0 art       (1000) art       (1000)    28580 2024-04-06 13:37:23.000000 VideoOpinionMining-1.0/src/VideoOpinionMining/vem.py
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-06 14:21:20.759431 VideoOpinionMining-1.0/src/VideoOpinionMining.egg-info/
--rw-r--r--   0 art       (1000) art       (1000)     2236 2024-04-06 14:21:20.000000 VideoOpinionMining-1.0/src/VideoOpinionMining.egg-info/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)      281 2024-04-06 14:21:20.000000 VideoOpinionMining-1.0/src/VideoOpinionMining.egg-info/SOURCES.txt
--rw-r--r--   0 art       (1000) art       (1000)        1 2024-04-06 14:21:20.000000 VideoOpinionMining-1.0/src/VideoOpinionMining.egg-info/dependency_links.txt
--rw-r--r--   0 art       (1000) art       (1000)       19 2024-04-06 14:21:20.000000 VideoOpinionMining-1.0/src/VideoOpinionMining.egg-info/top_level.txt
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-07 12:32:32.024619 VideoOpinionMining-1.1/
+-rw-r--r--   0 art       (1000) art       (1000)     1081 2024-04-06 12:43:21.000000 VideoOpinionMining-1.1/LICENSE
+-rw-r--r--   0 art       (1000) art       (1000)     2236 2024-04-07 12:32:32.014619 VideoOpinionMining-1.1/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)     1598 2024-04-06 12:41:33.000000 VideoOpinionMining-1.1/README.md
+-rw-r--r--   0 art       (1000) art       (1000)      710 2024-04-07 12:22:07.000000 VideoOpinionMining-1.1/pyproject.toml
+-rw-r--r--   0 art       (1000) art       (1000)       38 2024-04-07 12:32:32.024619 VideoOpinionMining-1.1/setup.cfg
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-07 12:32:32.014619 VideoOpinionMining-1.1/src/
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-07 12:32:32.014619 VideoOpinionMining-1.1/src/VideoOpinionMining/
+-rw-r--r--   0 art       (1000) art       (1000)       29 2024-04-06 13:38:23.000000 VideoOpinionMining-1.1/src/VideoOpinionMining/__init__.py
+-rw-r--r--   0 art       (1000) art       (1000)    28874 2024-04-07 12:21:55.000000 VideoOpinionMining-1.1/src/VideoOpinionMining/vem.py
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-07 12:32:32.014619 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/
+-rw-r--r--   0 art       (1000) art       (1000)     2236 2024-04-07 12:32:32.000000 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)      281 2024-04-07 12:32:32.000000 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/SOURCES.txt
+-rw-r--r--   0 art       (1000) art       (1000)        1 2024-04-07 12:32:32.000000 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/dependency_links.txt
+-rw-r--r--   0 art       (1000) art       (1000)       19 2024-04-07 12:32:32.000000 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/top_level.txt
```

### Comparing `VideoOpinionMining-1.0/LICENSE` & `VideoOpinionMining-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `VideoOpinionMining-1.0/PKG-INFO` & `VideoOpinionMining-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VideoOpinionMining
-Version: 1.0
+Version: 1.1
 Summary: This package receives an mp4 file classfying it according to its emotions and generating a heat map
 Author-email: Artur Lima <vligmart@gmail.com>
 Project-URL: Homepage, https://github.com/Labic-ICMC-USP/VEM
 Project-URL: Example, https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `VideoOpinionMining-1.0/README.md` & `VideoOpinionMining-1.1/README.md`

 * *Files identical despite different names*

### Comparing `VideoOpinionMining-1.0/pyproject.toml` & `VideoOpinionMining-1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "VideoOpinionMining"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Artur Lima", email="vligmart@gmail.com" },
 ]
 description = "This package receives an mp4 file classfying it according to its emotions and generating a heat map"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `VideoOpinionMining-1.0/src/VideoOpinionMining/vem.py` & `VideoOpinionMining-1.1/src/VideoOpinionMining/vem.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,18 @@
 from transformers import RobertaTokenizerFast, BertForSequenceClassification
 
 
 class VEMProcessor:
     """
         Here is the main class that makes this module, VEMProcessor
     """
-    def __init__(self, video_file):
+    def __init__(self):
         """
             To initialize it, pass the video fto be analyzed as an argument
         """
-        self.video_file = video_file
         self.segmenter = VideoSegmenter()
 
         self.opinion_model_transc = OpinionExtractionModel()
         self.opinion_model_transc.set_model(modality = "transcript")
 
         self.opinion_model_audio = OpinionExtractionModel()
         self.opinion_model_audio.set_model(modality = "audio")
@@ -54,29 +53,30 @@
         self.opinion_extractor_audio = OpinionExtractor([],self.opinion_model_audio)
         self.opinion_extractor_video = OpinionExtractor([],self.opinion_model_video)
 
         self.multimodal_extractor = MultimodalOpinionExtractor([])
 
         self.emotion_map_generator = EmotionMapGenerator([])  # Adjust segment_block_size as needed
 
-    def process_video(self, segment_block_size = 10):
+    def process_video(self, video_file, segment_block_size = 10):
         """
           Use this to run the models for all the modalities(transcript, audio, video and multimodal) and generate the heatmaps.
 
           Args:
+            **video_file (mp4)**: video to be analized.
             **segment_block_size (int)**: size of the block used in each frame of the heatmap.
 
           Return:
             Nothing.
 
           In case you also want the dataframes generated with all the emotions, object_of_class.segmented_video contains it.
 
         """
         # Step 1: Segment the video
-        self.segmented_video = self.segmenter.segment_video(self.video_file)
+        self.segmented_video = self.segmenter.segment_video(video_file)
         
         # Step 2: Extract opinions
         self.opinion_extractor_transc = OpinionExtractor([],self.opinion_model_transc)
         self.opinion_extractor_audio = OpinionExtractor([],self.opinion_model_audio)
         self.opinion_extractor_video = OpinionExtractor([],self.opinion_model_video)
 
         self.opinion_extractor_transc.segmenter_result = self.segmented_video
@@ -87,17 +87,14 @@
         self.opinion_extractor_audio.extract_opinions()
         self.opinion_extractor_video.extract_opinions()
         
         # Step 3: Extract multimodal opinions
         self.multimodal_extractor.segmented_with_emotion = self.segmented_video
         self.multimodal_extractor.extract_multimodal_opinions()
 
-        self.multimodal_extractor.segmented_with_emotion = self.opinion_extractor.segmenter_result
-        self.multimodal_extractor.extract_multimodal_opinions()
-
         # Step 4: Generate emotion map
         self.emotion_map_generator.segments_with_emotion = self.segmented_video
         self.emotion_map_generator.graph = self.multimodal_extractor.G_multimodal
 
         self.emotion_map_generator.generate_emotion_map("transcript",segment_block_size)
         self.emotion_map_generator.generate_emotion_map("audio",segment_block_size)
         self.emotion_map_generator.generate_emotion_map("video",segment_block_size)
@@ -109,29 +106,30 @@
         timestamps and name of the parts contained in a dataframe
     """
     def __init__(self):
         logging.basicConfig(filename="newfile.log",
         format='%(asctime)s %(message)s',filemode='w')
         self.logger = logging.getLogger()
         self.logger.setLevel(logging.INFO)
-        os.mkdir("parts")
         pass
 
     def segment_video(self, video_file):
         """
         Receives an MP4 file and returns a list of video segments.
         Each segment is represented as a series in a dataframe: (start_time, end_time, transcript_text, segment_file.mp4)
 
         Args:
-            **video_file (mp4)**: video to be analyzed.
+            **video_file (str)**: video to be analyzed.
 
         Return:
             Dataframe with all the segments.
 
         """
+        os.makedirs(video_file[0:3] + "parts", exist_ok=True)
+
         # Segment the video and extract transcript for each segment
         # Store each segment with its start time, end time, transcript, and save it as a new file
         self.logger.info("Transcripting the video")
         dataframe = transcript(video_file)
 
         self.logger.info("Done")
 
@@ -143,15 +141,15 @@
         for i in range(0, maximo):
             #Usando os timestamps da transcricao, corto o video separando aproximadamente cada frase
             startPos = dataframe[0][i]
             endPos = dataframe[1][i]
 
             clip = video.subclip(startPos, endPos)
 
-            part_name = "parts/part_"+str(i)+".mp4"
+            part_name = video_file[0:3] + "parts/part_"+str(i)+".mp4"
 
             names.append(part_name)
 
             clip.write_videofile(part_name, codec='libx264', fps=video.fps)
 
         video.close()
 
@@ -450,43 +448,55 @@
             respective modality have to be done befor)
 
             **segment_block_size (int)**: how many phrases are shown in the same frame of the heatmap.
         """
         if modality == 'multimodal':
           x = []
           y = []
+          x_img = []
+          y_img = []
           GCP(self.graph,mi=1,audio_weight=0.4, text_weight=0.6,max_iter=30)
           for index in self.segments_with_emotion.index:
             v = self.graph.nodes[index]['f']
+            x.append(v[0])
+            y.append(v[1])
             if (np.abs(v[0]) > 0.1 or np.abs(v[1]) > 0.1):
-              x.append(v[0])
-              y.append(v[1])
+              x_img.append(v[0])
+              y_img.append(v[1])
         else:
           df = get_labels(self.segments_with_emotion, modality)
 
           label = modality + '_label'
 
           df.loc[df[label] == 'no_face', [label]] = 'neutral'
           resp = list(df[label].apply(generate_coord, args = (self.emotions_coord,)))
           temp = pd.DataFrame.from_records(resp, columns=['x', 'y'])
 
           df = pd.concat([df, temp], axis=1)
 
-          #df = df[df[label]!='neutral']
-          df = df.reset_index(drop=True)
-
           array_x = df['x'].to_numpy()
           x = array_x.tolist()
           array_y = df['y'].to_numpy()
           y = array_y.tolist()
 
+          dfimage = df[df[label]!='neutral']
+          dfimage = dfimage.reset_index(drop=True)
+
+          array_x_img = dfimage['x'].to_numpy()
+          x_img = array_x_img.tolist()
+          array_y_img = dfimage['y'].to_numpy()
+          y_img = array_y_img.tolist()
+
+
+        vid_name = self.segments_with_emotion["segment_file"][0]
+        vid_name = vid_name[0:3]
         os.makedirs("tempjpgs", exist_ok=True)
-        os.makedirs("heatmaps", exist_ok=True)
+        os.makedirs(vid_name + "heatmaps", exist_ok=True)
         
-        plot_heatmap(x, y, self.emotions_coord, modality)
+        plot_heatmap(x_img, y_img, self.emotions_coord, modality, vid_name)
 
 
         id_ini = 0
         id_fim = segment_block_size
         atual = 1
         quant = self.segments_with_emotion.shape[0]
         tam = quant / segment_block_size
@@ -498,15 +508,14 @@
             if all(val == 0 for val in x_temp) and all(val == 0 for val in y_temp):
               x_temp = np.array([0])
               y_temp = np.array([0])
             else:
               x_temp = [i for i,j in zip(x_temp,y_temp) if (i != 0 and j != 0)]
               y_temp = [j for i,j in zip(x[id_ini: id_fim],y_temp) if (i != 0 and j != 0)]
 
-            plot_heatmap(x_temp, y_temp, self.emotions_coord, "animated")
             plt.title("Emotions from " + str(id_ini) + " to " + str(id_fim-1) + " block")
             plt.savefig("tempjpgs/output" + str(atual) + ".jpg")
             plt.close()
 
             id_ini += segment_block_size
             id_fim += segment_block_size
             atual += 1
@@ -520,23 +529,23 @@
             size = (width,height)
             img_array.append(img)
             os.remove(filename)
 
         os.rmdir("tempjpgs")
 
         rate = 1
-        out = cv2.VideoWriter("heatmaps/"+ modality + '_heatmap.mp4',cv2.VideoWriter_fourcc(*'XVID'), rate, size)
+        out = cv2.VideoWriter(vid_name +"heatmaps/"+ modality + '_heatmap.mp4',cv2.VideoWriter_fourcc(*'XVID'), rate, size)
 
         for i in range(len(img_array)):
           for j in range(2):
             out.write(img_array[i])
 
         out.release()
 
-        myvideo = VideoFileClip("heatmaps/"+modality + '_heatmap.mp4')
+        myvideo = VideoFileClip(vid_name + "heatmaps/"+modality + '_heatmap.mp4')
         self.logger.info("Video created")
 
         return ipython_display(myvideo)
 
 #Função para extrair do dicionario retornado pelo goemotions a emoção mais provável e sua probabilidade
 def emocao_provavel(frase, emot_pipe):
     emotion_labels = emot_pipe(frase)
@@ -578,15 +587,15 @@
     x = coords.iloc[index]['X']
     y = coords.iloc[index]['Y']
     return (x,y)
 def kde_quartic(d,h):
     dn=d/h
     P=(15/16)*(1-dn**2)**2
     return P
-def plot_heatmap(x, y, emotions_coord, modality):
+def plot_heatmap(x, y, emotions_coord, modality, vid_name):
     #Definindo tamanho do grid e do raio(h)
     grid_size=0.02
     h=0.5
 
     #Tomando valores de máximos e mínimos de X e Y.
     x_min=-1
     x_max=1
@@ -644,15 +653,15 @@
     ax.add_patch(plt.Circle((0, 0), 1, color='black', fill=False))
     plt.axvline(x = 0, color = 'black', label = 'Arousal')
     plt.axhline(y = 0, color = 'black', label = 'Valence')
 
     #plt.colorbar()
 
     plt.plot(x,y,'x',color='white')
-    plt.savefig("heatmaps/" + modality + "heatmap.png")
+    plt.savefig(vid_name + "heatmaps/" + modality + "heatmap.png")
 
 #Funcoes auxiliares para a transcricao
 def transcript(video, method = "whisperx", min_time = 1):
     """
       Transform the audio of a video into a dataframe with it's phrases in text form separated by time frames
     """
     bashCommand = "whisperx --compute_type float32 --output_format vtt " + video
```

### Comparing `VideoOpinionMining-1.0/src/VideoOpinionMining.egg-info/PKG-INFO` & `VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VideoOpinionMining
-Version: 1.0
+Version: 1.1
 Summary: This package receives an mp4 file classfying it according to its emotions and generating a heat map
 Author-email: Artur Lima <vligmart@gmail.com>
 Project-URL: Homepage, https://github.com/Labic-ICMC-USP/VEM
 Project-URL: Example, https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

