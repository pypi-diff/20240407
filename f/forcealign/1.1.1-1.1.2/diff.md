# Comparing `tmp/forcealign-1.1.1.tar.gz` & `tmp/forcealign-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forcealign-1.1.1.tar", last modified: Mon Mar 25 19:35:32 2024, max compression
+gzip compressed data, was "forcealign-1.1.2.tar", last modified: Sat Apr  6 22:57:20 2024, max compression
```

## Comparing `forcealign-1.1.1.tar` & `forcealign-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-03-25 19:35:32.312925 forcealign-1.1.1/
--rw-r--r--   0 luke       (501) staff       (20)     1067 2024-03-18 13:49:23.000000 forcealign-1.1.1/LICENSE
--rw-r--r--   0 luke       (501) staff       (20)     4389 2024-03-25 19:35:32.312117 forcealign-1.1.1/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)     3725 2024-03-18 19:16:07.000000 forcealign-1.1.1/README.md
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-03-25 19:35:32.308734 forcealign-1.1.1/forcealign/
--rw-r--r--   0 luke       (501) staff       (20)       34 2024-03-18 15:39:18.000000 forcealign-1.1.1/forcealign/__init__.py
--rw-r--r--   0 luke       (501) staff       (20)     6775 2024-03-25 19:31:26.000000 forcealign-1.1.1/forcealign/forcealign.py
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-03-25 19:35:32.311248 forcealign-1.1.1/forcealign.egg-info/
--rw-r--r--   0 luke       (501) staff       (20)     4389 2024-03-25 19:35:32.000000 forcealign-1.1.1/forcealign.egg-info/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)      243 2024-03-25 19:35:32.000000 forcealign-1.1.1/forcealign.egg-info/SOURCES.txt
--rw-r--r--   0 luke       (501) staff       (20)        1 2024-03-25 19:35:32.000000 forcealign-1.1.1/forcealign.egg-info/dependency_links.txt
--rw-r--r--   0 luke       (501) staff       (20)       59 2024-03-25 19:35:32.000000 forcealign-1.1.1/forcealign.egg-info/requires.txt
--rw-r--r--   0 luke       (501) staff       (20)       11 2024-03-25 19:35:32.000000 forcealign-1.1.1/forcealign.egg-info/top_level.txt
--rw-r--r--   0 luke       (501) staff       (20)       38 2024-03-25 19:35:32.313158 forcealign-1.1.1/setup.cfg
--rw-r--r--   0 luke       (501) staff       (20)      969 2024-03-25 19:33:38.000000 forcealign-1.1.1/setup.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-06 22:57:20.124873 forcealign-1.1.2/
+-rw-r--r--   0 luke       (501) staff       (20)     1067 2024-03-18 13:49:23.000000 forcealign-1.1.2/LICENSE
+-rw-r--r--   0 luke       (501) staff       (20)     4528 2024-04-06 22:57:20.123419 forcealign-1.1.2/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)     3864 2024-04-05 18:03:54.000000 forcealign-1.1.2/README.md
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-06 22:57:20.117250 forcealign-1.1.2/forcealign/
+-rw-r--r--   0 luke       (501) staff       (20)       34 2024-03-18 15:39:18.000000 forcealign-1.1.2/forcealign/__init__.py
+-rw-r--r--   0 luke       (501) staff       (20)     7285 2024-04-06 22:57:11.000000 forcealign-1.1.2/forcealign/forcealign.py
+-rw-r--r--   0 luke       (501) staff       (20)        0 2024-04-05 18:05:30.000000 forcealign-1.1.2/forcealign/util.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-06 22:57:20.121922 forcealign-1.1.2/forcealign.egg-info/
+-rw-r--r--   0 luke       (501) staff       (20)     4528 2024-04-06 22:57:19.000000 forcealign-1.1.2/forcealign.egg-info/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)      262 2024-04-06 22:57:20.000000 forcealign-1.1.2/forcealign.egg-info/SOURCES.txt
+-rw-r--r--   0 luke       (501) staff       (20)        1 2024-04-06 22:57:19.000000 forcealign-1.1.2/forcealign.egg-info/dependency_links.txt
+-rw-r--r--   0 luke       (501) staff       (20)       59 2024-04-06 22:57:19.000000 forcealign-1.1.2/forcealign.egg-info/requires.txt
+-rw-r--r--   0 luke       (501) staff       (20)       11 2024-04-06 22:57:19.000000 forcealign-1.1.2/forcealign.egg-info/top_level.txt
+-rw-r--r--   0 luke       (501) staff       (20)       38 2024-04-06 22:57:20.125048 forcealign-1.1.2/setup.cfg
+-rw-r--r--   0 luke       (501) staff       (20)      969 2024-04-06 22:57:09.000000 forcealign-1.1.2/setup.py
```

### Comparing `forcealign-1.1.1/LICENSE` & `forcealign-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `forcealign-1.1.1/PKG-INFO` & `forcealign-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcealign
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python library for forced alignment of English text to English audio.
 Home-page: https://github.com/lukerbs/forcealign
 Author: Luke Kerbs
 Keywords: force align,forced alignment,audio segmentation,audio forced alignment,python forced alignment,phoneme,generate subtitles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,54 +18,59 @@
 # ForceAlign 
 ForceAlign is a Python library for forced alignment of English text to English Audio. You can use this library to get word or [phoneme](https://en.wikipedia.org/wiki/Phoneme)-level text alignments to English audio. In short, forced alignment is the process of identifying the specific time a word (or words) was spoken within an audio recording. ForceAlign supports forced alignment for .mp3 and .wav audio file formats.
 
 For phoneme level text alignments, ForceAlign currently only supports the [ARPABET](https://en.wikipedia.org/wiki/ARPABET) phonetic transcription encoding. 
 
 ForceAlign uses Pytorch's WAV2VEC2 pretrained model for acoustic feature extraction and can be ran on both CPU and CUDA GPU devices.
 
-# Installation and Dependencies
+## Features
+- Fast and accurate word and phoneme level forced alignment of text to audio.
+- Is optimized for both CPU and GPU.
+- OS independent! Use ForceAlign on Mac, Windows, and Linux.
+
+## Installation and Dependencies
 1. Pip Install ForceAlign
 	- `pip3 install forcealign`
 2. Install ffmpeg
 	- Mac: `brew install ffmpeg`
 	- Linux: `sudo apt install ffmpeg`
 	- Windows: Install from [ffmpeg.org](https://ffmpeg.org/download.html)
 
-# Usage Examples
-To use ForceAlign, instantiate a ForceAlign object instance with your specified audio file and corresponding text file. 
+## Usage Examples
+To use ForceAlign, instantiate a ForceAlign object instance with your specified audio file and corresponding text transcript. 
 
 **Example 1: Getting Word-Level Text Alignments**
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
-words = align.inference() 
+words = align.inference()
 
 # Show predicted word-level alignments
 for word in words:
 	print(word.word) # The word spoken in audio at associated time
 	print(word.time_start) # Time (seconds) the word starts in speech.mp3
-	print(word.time_end) # Time (seconds) the word ends in speech.mp3
+	print(word.time_end) # Time (seconds) the word ends in speech.mp3w
 
 ```
 
 **Example 2: Getting Phoneme-Level Text Alignments**
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
 words = align.inference() 
 
-# Show predicted phenome-level alignments
+# Accessing predicted phenome-level alignments
 for word in words:
 	print(word.word)
 	for phoneme in word.phonemes:
 		print(phoneme.phoneme) # ARPABET phonome spoken in audio at associated time
 		print(phoneme.time_start) # Time (seconds) the phoneme starts in speech.mp3
 		print(phoneme.time_end) # Time (seconds) the phoneme ends in speech.mp3
 
@@ -73,30 +78,30 @@
 
 **Example 3: Reviewing Word Level-Alignments**
 
 You can use the review_alignment() method to check the quality of your alignment in real-time. The review_alignment() method will play the audio file and print the individual words at their predicted times. This is useful for heuristically checking the accuracy of the word-level alignment predictions.
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
 words = align.inference() 
 
 # Plays audio and prints each word in real-time at predicted alignment time.
 align.review_alignment()
 
 ```
 
-# Use Cases
+## Use Cases
 Forced alignment can be useful for generating subtitles for video, and for generating automated lip-syncing of animated characters with phoneme-level forced alignments. 
 
-# FAQ
+## FAQ
 **1. Does ForceAlign have speech-to-text capabilities?**
 No. This is a feature that I plan on adding soon when I have time.
 
 **2. Can ForceAlign be used with both CPU and GPU?**
 Yes. Running with CPU is surprisingly fast, and it will be even faster with GPU. 
 
-# Acknowledgements
+## Acknowledgements
 This project is heavily based upon a demo from Pytorch by Moto Hira: [FORCED ALIGNMENT WITH WAV2VEC2](https://pytorch.org/audio/stable/tutorials/forced_alignment_tutorial.html)
```

### Comparing `forcealign-1.1.1/README.md` & `forcealign-1.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 # ForceAlign 
 ForceAlign is a Python library for forced alignment of English text to English Audio. You can use this library to get word or [phoneme](https://en.wikipedia.org/wiki/Phoneme)-level text alignments to English audio. In short, forced alignment is the process of identifying the specific time a word (or words) was spoken within an audio recording. ForceAlign supports forced alignment for .mp3 and .wav audio file formats.
 
 For phoneme level text alignments, ForceAlign currently only supports the [ARPABET](https://en.wikipedia.org/wiki/ARPABET) phonetic transcription encoding. 
 
 ForceAlign uses Pytorch's WAV2VEC2 pretrained model for acoustic feature extraction and can be ran on both CPU and CUDA GPU devices.
 
-# Installation and Dependencies
+## Features
+- Fast and accurate word and phoneme level forced alignment of text to audio.
+- Is optimized for both CPU and GPU.
+- OS independent! Use ForceAlign on Mac, Windows, and Linux.
+
+## Installation and Dependencies
 1. Pip Install ForceAlign
 	- `pip3 install forcealign`
 2. Install ffmpeg
 	- Mac: `brew install ffmpeg`
 	- Linux: `sudo apt install ffmpeg`
 	- Windows: Install from [ffmpeg.org](https://ffmpeg.org/download.html)
 
-# Usage Examples
-To use ForceAlign, instantiate a ForceAlign object instance with your specified audio file and corresponding text file. 
+## Usage Examples
+To use ForceAlign, instantiate a ForceAlign object instance with your specified audio file and corresponding text transcript. 
 
 **Example 1: Getting Word-Level Text Alignments**
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
-words = align.inference() 
+words = align.inference()
 
 # Show predicted word-level alignments
 for word in words:
 	print(word.word) # The word spoken in audio at associated time
 	print(word.time_start) # Time (seconds) the word starts in speech.mp3
-	print(word.time_end) # Time (seconds) the word ends in speech.mp3
+	print(word.time_end) # Time (seconds) the word ends in speech.mp3w
 
 ```
 
 **Example 2: Getting Phoneme-Level Text Alignments**
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
 words = align.inference() 
 
-# Show predicted phenome-level alignments
+# Accessing predicted phenome-level alignments
 for word in words:
 	print(word.word)
 	for phoneme in word.phonemes:
 		print(phoneme.phoneme) # ARPABET phonome spoken in audio at associated time
 		print(phoneme.time_start) # Time (seconds) the phoneme starts in speech.mp3
 		print(phoneme.time_end) # Time (seconds) the phoneme ends in speech.mp3
 
@@ -56,30 +61,30 @@
 
 **Example 3: Reviewing Word Level-Alignments**
 
 You can use the review_alignment() method to check the quality of your alignment in real-time. The review_alignment() method will play the audio file and print the individual words at their predicted times. This is useful for heuristically checking the accuracy of the word-level alignment predictions.
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
 words = align.inference() 
 
 # Plays audio and prints each word in real-time at predicted alignment time.
 align.review_alignment()
 
 ```
 
-# Use Cases
+## Use Cases
 Forced alignment can be useful for generating subtitles for video, and for generating automated lip-syncing of animated characters with phoneme-level forced alignments. 
 
-# FAQ
+## FAQ
 **1. Does ForceAlign have speech-to-text capabilities?**
 No. This is a feature that I plan on adding soon when I have time.
 
 **2. Can ForceAlign be used with both CPU and GPU?**
 Yes. Running with CPU is surprisingly fast, and it will be even faster with GPU. 
 
-# Acknowledgements
+## Acknowledgements
 This project is heavily based upon a demo from Pytorch by Moto Hira: [FORCED ALIGNMENT WITH WAV2VEC2](https://pytorch.org/audio/stable/tutorials/forced_alignment_tutorial.html)
```

### Comparing `forcealign-1.1.1/forcealign/forcealign.py` & `forcealign-1.1.2/forcealign/forcealign.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 @dataclass
 class Word:
 	word: str
 	phonemes: list
 	time_start: float
 	time_end: float
+	breath: bool
 
 	def __repr__(self):
 		return f'{self.word}: {self.time_start} -- {self.time_end}(s)'
 
 
 @dataclass
 class Phoneme:
@@ -99,14 +100,15 @@
 
 			self.emissions, _ = self.model(self.waveform.to(self.device))
 			self.emissions = torch.log_softmax(self.emissions, dim=-1)
 
 		self.emission = self.emissions[0].cpu().detach()
 
 		# Read the text file to a string 
+		self.breath_idx = get_breath_idx(transcript)
 		self.raw_text = transcript
 		text = self.raw_text.replace('—',' ')
 		text = alphabetical(text).upper().split()
 		self.transcript = f'{"|".join(text)}|'
 
 		self.tokens = [self.dictionary[c] for c in self.transcript]
 
@@ -217,14 +219,15 @@
 	def inference(self):
 		trellis = self.get_trellis()
 		path = self.backtrack(trellis)
 		segments = self.merge_repeats(path)
 		word_segments = self.merge_words(segments)
 
 		words = []
+		idx = 0
 		for word in word_segments:
 			ratio = self.waveform.size(1) / trellis.size(0)
 			start = int(ratio * word.start)
 			end = int(ratio * word.end)
 			time_start = round((start/self.bundle.sample_rate),3)
 			time_end = round((end/self.bundle.sample_rate),3)
 
@@ -234,15 +237,21 @@
 			start_phoneme = time_start
 			for i,_ in enumerate(phonemes):
 				end_phoneme = start_phoneme + phoneme_duration - 0.1
 				phoneme = Phoneme(phoneme=phonemes[i], time_start=start_phoneme, time_end=end_phoneme)
 				self.phoneme_alignments.append(phoneme)
 				start_phoneme += phoneme_duration
 
-			words.append(Word(word=word.label, phonemes=phonemes, time_start=time_start, time_end=time_end))
+			if idx in self.breath_idx:
+				breath = True
+			else:
+				breath = False
+
+			words.append(Word(word=word.label, phonemes=phonemes, time_start=time_start, time_end=time_end, breath=breath))
+			idx += 1
 
 		self.word_alignments = words
 		return words
 
 	def review_alignment(self):
 		audio = AudioSegment.from_file(self.SPEECH_FILE, format=self.audio_format)
 
@@ -250,14 +259,24 @@
 		for word in self.word_alignments:
 			timer = threading.Timer(word.time_start, print, args=[repr(word)])
 			timers.append(timer)
 			timer.start()
 		play(audio)
 
 
+def get_breath_idx(transcript):
+	transcript = transcript.replace('—',' ')
+	transcript = alpha_with_punct(transcript).upper().split()
+	idxs = []
+	for i in range(len(transcript)-1):
+		if "," in transcript[i] or "." in transcript[i]:
+			idxs.append(i)
+	return idxs
 
+def alpha_with_punct(text):
+	return re.sub(r'[^a-zA-Z\s,.]', '', text)
```

### Comparing `forcealign-1.1.1/forcealign.egg-info/PKG-INFO` & `forcealign-1.1.2/forcealign.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcealign
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python library for forced alignment of English text to English audio.
 Home-page: https://github.com/lukerbs/forcealign
 Author: Luke Kerbs
 Keywords: force align,forced alignment,audio segmentation,audio forced alignment,python forced alignment,phoneme,generate subtitles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,54 +18,59 @@
 # ForceAlign 
 ForceAlign is a Python library for forced alignment of English text to English Audio. You can use this library to get word or [phoneme](https://en.wikipedia.org/wiki/Phoneme)-level text alignments to English audio. In short, forced alignment is the process of identifying the specific time a word (or words) was spoken within an audio recording. ForceAlign supports forced alignment for .mp3 and .wav audio file formats.
 
 For phoneme level text alignments, ForceAlign currently only supports the [ARPABET](https://en.wikipedia.org/wiki/ARPABET) phonetic transcription encoding. 
 
 ForceAlign uses Pytorch's WAV2VEC2 pretrained model for acoustic feature extraction and can be ran on both CPU and CUDA GPU devices.
 
-# Installation and Dependencies
+## Features
+- Fast and accurate word and phoneme level forced alignment of text to audio.
+- Is optimized for both CPU and GPU.
+- OS independent! Use ForceAlign on Mac, Windows, and Linux.
+
+## Installation and Dependencies
 1. Pip Install ForceAlign
 	- `pip3 install forcealign`
 2. Install ffmpeg
 	- Mac: `brew install ffmpeg`
 	- Linux: `sudo apt install ffmpeg`
 	- Windows: Install from [ffmpeg.org](https://ffmpeg.org/download.html)
 
-# Usage Examples
-To use ForceAlign, instantiate a ForceAlign object instance with your specified audio file and corresponding text file. 
+## Usage Examples
+To use ForceAlign, instantiate a ForceAlign object instance with your specified audio file and corresponding text transcript. 
 
 **Example 1: Getting Word-Level Text Alignments**
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
-words = align.inference() 
+words = align.inference()
 
 # Show predicted word-level alignments
 for word in words:
 	print(word.word) # The word spoken in audio at associated time
 	print(word.time_start) # Time (seconds) the word starts in speech.mp3
-	print(word.time_end) # Time (seconds) the word ends in speech.mp3
+	print(word.time_end) # Time (seconds) the word ends in speech.mp3w
 
 ```
 
 **Example 2: Getting Phoneme-Level Text Alignments**
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
 words = align.inference() 
 
-# Show predicted phenome-level alignments
+# Accessing predicted phenome-level alignments
 for word in words:
 	print(word.word)
 	for phoneme in word.phonemes:
 		print(phoneme.phoneme) # ARPABET phonome spoken in audio at associated time
 		print(phoneme.time_start) # Time (seconds) the phoneme starts in speech.mp3
 		print(phoneme.time_end) # Time (seconds) the phoneme ends in speech.mp3
 
@@ -73,30 +78,30 @@
 
 **Example 3: Reviewing Word Level-Alignments**
 
 You can use the review_alignment() method to check the quality of your alignment in real-time. The review_alignment() method will play the audio file and print the individual words at their predicted times. This is useful for heuristically checking the accuracy of the word-level alignment predictions.
 ```
 from forcealign import ForceAlign
 
-# Provide path to audio_file and corresponding txt_file with audio transcript
-align = ForceAlign(audio_file='./speech.mp3', txt_file='./speech.txt')
+# Provide path to audio_file and corresponding transcript
+align = ForceAlign(audio_file='./speech.mp3', transcript=transcript)
 
 # Runs prediction and returns alignment results
 words = align.inference() 
 
 # Plays audio and prints each word in real-time at predicted alignment time.
 align.review_alignment()
 
 ```
 
-# Use Cases
+## Use Cases
 Forced alignment can be useful for generating subtitles for video, and for generating automated lip-syncing of animated characters with phoneme-level forced alignments. 
 
-# FAQ
+## FAQ
 **1. Does ForceAlign have speech-to-text capabilities?**
 No. This is a feature that I plan on adding soon when I have time.
 
 **2. Can ForceAlign be used with both CPU and GPU?**
 Yes. Running with CPU is surprisingly fast, and it will be even faster with GPU. 
 
-# Acknowledgements
+## Acknowledgements
 This project is heavily based upon a demo from Pytorch by Moto Hira: [FORCED ALIGNMENT WITH WAV2VEC2](https://pytorch.org/audio/stable/tutorials/forced_alignment_tutorial.html)
```

### Comparing `forcealign-1.1.1/setup.py` & `forcealign-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='forcealign',
-    version='1.1.1',
+    version='1.1.2',
     packages=find_packages(),
     install_requires=['torch==2.2.1', 'torchaudio==2.2.1', 'pydub==0.25.1', 'g2p-en==2.1.0'],
     author='Luke Kerbs',
     description='A Python library for forced alignment of English text to English audio.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lukerbs/forcealign',
```

