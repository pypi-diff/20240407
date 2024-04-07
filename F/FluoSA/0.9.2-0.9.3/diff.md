# Comparing `tmp/fluosa-0.9.2.tar.gz` & `tmp/fluosa-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluosa-0.9.2.tar", last modified: Sat Mar 30 18:50:52 2024, max compression
+gzip compressed data, was "fluosa-0.9.3.tar", last modified: Sun Apr  7 04:47:59 2024, max compression
```

## Comparing `fluosa-0.9.2.tar` & `fluosa-0.9.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     6148 2024-03-30 18:46:35.978414 fluosa-0.9.2/FluoSA/.DS_Store
--rw-r--r--   0        0        0      214 2024-03-30 05:27:38.592003 fluosa-0.9.2/FluoSA/COPYRIGHT.txt
--rw-r--r--   0        0        0      131 2024-03-30 05:27:38.592232 fluosa-0.9.2/FluoSA/NOTICE.txt
--rw-r--r--   0        0        0      883 2024-03-30 18:48:01.071760 fluosa-0.9.2/FluoSA/__init__.py
--rw-r--r--   0        0        0     1509 2024-03-30 18:40:16.006232 fluosa-0.9.2/FluoSA/__main__.py
--rw-r--r--   0        0        0    16642 2024-03-30 05:27:38.593141 fluosa-0.9.2/FluoSA/analyzer.py
--rw-r--r--   0        0        0     5835 2024-03-30 05:27:38.593539 fluosa-0.9.2/FluoSA/detector.py
--rw-r--r--   0        0        0      860 2024-03-30 05:27:38.593889 fluosa-0.9.2/FluoSA/detectors/__init__.py
--rw-r--r--   0        0        0    39776 2024-03-30 06:12:49.167591 fluosa-0.9.2/FluoSA/gui.py
--rw-r--r--   0        0        0    31919 2024-03-30 05:27:38.594623 fluosa-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0      131 2024-03-30 05:27:38.594877 fluosa-0.9.2/NOTICE.txt
--rw-r--r--   0        0        0       93 2024-03-30 05:27:38.595082 fluosa-0.9.2/README.md
--rw-r--r--   0        0        0     1663 2024-03-30 18:50:52.341586 fluosa-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 fluosa-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      214 2024-04-07 04:47:54.270952 fluosa-0.9.3/FluoSA/COPYRIGHT.txt
+-rw-r--r--   0        0        0      131 2024-04-07 04:47:54.270952 fluosa-0.9.3/FluoSA/NOTICE.txt
+-rw-r--r--   0        0        0      883 2024-04-07 04:47:54.270952 fluosa-0.9.3/FluoSA/__init__.py
+-rw-r--r--   0        0        0     1506 2024-04-07 04:47:54.270952 fluosa-0.9.3/FluoSA/__main__.py
+-rw-r--r--   0        0        0    16793 2024-04-07 04:47:54.270952 fluosa-0.9.3/FluoSA/analyzer.py
+-rw-r--r--   0        0        0     5835 2024-04-07 04:47:54.270952 fluosa-0.9.3/FluoSA/detector.py
+-rw-r--r--   0        0        0      860 2024-04-07 04:47:54.270952 fluosa-0.9.3/FluoSA/detectors/__init__.py
+-rw-r--r--   0        0        0    39809 2024-04-07 04:47:54.270952 fluosa-0.9.3/FluoSA/gui.py
+-rw-r--r--   0        0        0    31919 2024-04-07 04:47:54.270952 fluosa-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0      131 2024-04-07 04:47:54.270952 fluosa-0.9.3/NOTICE.txt
+-rw-r--r--   0        0        0     1347 2024-04-07 04:47:54.270952 fluosa-0.9.3/README.md
+-rw-r--r--   0        0        0     1677 2024-04-07 04:47:59.042994 fluosa-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 fluosa-0.9.3/PKG-INFO
```

### Comparing `fluosa-0.9.2/FluoSA/__init__.py` & `fluosa-0.9.3/FluoSA/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 
 Email: bingye@umich.edu
 '''
 
 
 
 
-__version__='0.9.2'
+__version__='0.9.3'
```

### Comparing `fluosa-0.9.2/FluoSA/__main__.py` & `fluosa-0.9.3/FluoSA/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 		current_version=version.parse(__version__)
 		pypi_json=requests.get('https://pypi.org/pypi/FluoSA/json').json()
 		latest_version=version.parse(pypi_json['info']['version'])
 
 		if latest_version>current_version:
 			print('A newer version '+'('+str(latest_version)+')'+' of FluoSA is available.')
 			print('You may upgrade it by "python3 -m pip install --upgrade FluoSA".')
-			print('For the details of new changes, check: "https://github.com/yujiahu415/FluoSA".')
+			print('For the details of new changes, check: "https://github.com/umyelab/FluoSA".')
 
 	except:
 		
 		pass
 
 	gui.main_window()
```

### Comparing `fluosa-0.9.2/FluoSA/analyzer.py` & `fluosa-0.9.3/FluoSA/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 	def __init__(self,path_to_lif,results_path,stim_t,duration):
 
 		self.detector=None
 		self.neuro_mapping=None
 		self.path_to_lif=path_to_lif
 		self.results_path=os.path.join(results_path,os.path.splitext(os.path.basename(self.path_to_lif))[0])
+		os.makedirs(self.results_path,exist_ok=True)
 		self.neuro_number=None
 		self.neuro_kinds=None  # the catgories of neural structures to be analyzed
 		self.stim_t=stim_t  # the frame number when stimulation is on 
 		lifdata=LifFile(self.path_to_lif)
 		file=[i for i in lifdata.get_iter_image()][0]
 		self.full_duration=len([i for i in file.get_iter_t(c=0,z=0)])-1
 		self.duration=duration # the duration (in frames) for example generation / analysis, 0: use entire duration
@@ -80,15 +81,14 @@
 		cfg=get_cfg()
 		cfg.merge_from_file(config)
 		cfg.MODEL.DEVICE='cuda' if torch.cuda.is_available() else 'cpu'
 		self.detector=build_model(cfg)
 		DetectionCheckpointer(self.detector).load(detector)
 		self.detector.eval()
 
-		os.makedirs(self.results_path,exist_ok=True)
 		self.neuro_number=neuro_number
 		self.neuro_kinds=neuro_kinds
 
 		total_number=0
 
 		for neuro_name in self.neuro_kinds:
 
@@ -241,15 +241,16 @@
 		channels=[i for i in file.get_iter_c(t=0,z=0)]
 
 		while True:
 
 			if frame_count<self.duration:
 
 				frame_project=[np.array(i) for i in file.get_iter_z(t=frame_count,c=self.main_channel)]
-				frame_project=np.array(frame_project).sum(0)/len(frame_project)
+				#frame_project=np.array(frame_project).sum(0)/len(frame_project)
+				frame_project=np.array(frame_project).max(0)
 
 				if autofind_t is True:
 
 					frame_project_stim=[np.array(i) for i in file.get_iter_z(t=frame_count,c=stimulation_channel)]
 					frame_project_stim=np.array(frame_project_stim).sum(0)/len(frame_project_stim)
 
 					if initial_frame is None:
@@ -361,15 +362,16 @@
 		writer=None
 
 		while True:
 
 			if frame_count<self.duration:
 
 				frame_project=[np.array(i) for i in file.get_iter_z(t=frame_count,c=self.main_channel)]
-				frame_project=np.array(frame_project).sum(0)/len(frame_project)
+				#frame_project=np.array(frame_project).sum(0)/len(frame_project)
+				frame_project=np.array(frame_project).max(0)
 				frame_project[frame_project>255]=255
 				frame_project=cv2.cvtColor(np.uint8(frame_project),cv2.COLOR_GRAY2BGR)
 
 				if writer is None:
 					(h,w)=frame_project.shape[:2]
 					out=os.path.join(self.results_path,'Annotated video.avi')
 					writer=cv2.VideoWriter(out,cv2.VideoWriter_fourcc(*'MJPG'),1,(w,h),True)
@@ -458,14 +460,15 @@
 		for channel in range(len(channels)):
 
 			for frame_count in range(self.full_duration):
 
 				if self.stim_t<=frame_count<end_t and frame_count%skip_redundant==0:
 
 					frame_project=[np.array(i) for i in file.get_iter_z(t=frame_count,c=channel)]
-					frame_project=np.array(frame_project).sum(0)/len(frame_project)
+					#frame_project=np.array(frame_project).sum(0)/len(frame_project)
+					frame_project=np.array(frame_project).max(0)
 					frame_project[frame_project>255]=255
 					out_image=os.path.join(self.results_path,str(channel)+'_'+str(frame_count)+'.jpg')
 					cv2.imwrite(out_image,np.uint8(np.array(frame_project)))
 
 		print('The images stored in: '+self.results_path)
```

### Comparing `fluosa-0.9.2/FluoSA/detector.py` & `fluosa-0.9.3/FluoSA/detector.py`

 * *Files identical despite different names*

### Comparing `fluosa-0.9.2/FluoSA/detectors/__init__.py` & `fluosa-0.9.3/FluoSA/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `fluosa-0.9.2/FluoSA/gui.py` & `fluosa-0.9.3/FluoSA/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 		self.text_developers=wx.StaticText(panel,
 			label='Developed by Yujia Hu\n\nBing Ye Lab, Life Sciences Institute, University of Michigan',
 			style=wx.ALIGN_CENTER|wx.ST_ELLIPSIZE_END)
 		boxsizer.Add(self.text_developers,0,wx.LEFT|wx.RIGHT|wx.EXPAND,5)
 		boxsizer.Add(0,60,0)
 		
 		links=wx.BoxSizer(wx.HORIZONTAL)
-		homepage=hl.HyperLinkCtrl(panel,0,'Home Page',URL='')
+		homepage=hl.HyperLinkCtrl(panel,0,'Home Page',URL='https://github.com/umyelab/FluoSA')
 		userguide=hl.HyperLinkCtrl(panel,0,'Extended Guide',URL='')
 		links.Add(homepage,0,wx.LEFT|wx.EXPAND,10)
 		links.Add(userguide,0,wx.LEFT|wx.RIGHT|wx.EXPAND,10)
 		boxsizer.Add(links,0,wx.ALIGN_CENTER,50)
 		boxsizer.Add(0,50,0)
 
 		module_modules=wx.BoxSizer(wx.HORIZONTAL)
```

### Comparing `fluosa-0.9.2/LICENSE.txt` & `fluosa-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluosa-0.9.2/pyproject.toml` & `fluosa-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "openpyxl",
     "xlsxwriter",
     "pandas",
     "wxPython",
     "torch==2.0.1;platform_system=='Darwin'",
     "torchvision==0.15.2;platform_system=='Darwin'",
     "packaging",
+    "requests",
 ]
 requires-python = ">=3.9,<3.11"
 readme = "README.md"
 keywords = [
     "Fluorescence Signal",
     "Calcium imaging",
     "Leica confocal",
@@ -36,21 +37,21 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = []
-version = "0.9.2"
+version = "0.9.3"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.urls]
-Homepage = "http://github.com/yujiahu415/FluoSA"
+Homepage = "https://github.com/umyelab/FluoSA"
 
 [project.scripts]
 FluoSA = "FluoSA.__main__:main"
 
 [tool.pdm]
 distribution = true
```

