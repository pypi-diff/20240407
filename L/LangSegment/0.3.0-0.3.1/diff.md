# Comparing `tmp/LangSegment-0.3.0-py3-none-any.whl.zip` & `tmp/LangSegment-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 21087 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    44676 b- defN 24-Apr-03 09:55 LangSegment/LangSegment.py
--rw-rw-rw-  2.0 fat      278 b- defN 24-Apr-03 09:55 LangSegment/__init__.py
--rw-rw-rw-  2.0 fat    15200 b- defN 24-Apr-03 09:56 LangSegment-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 09:56 LangSegment-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-03 09:56 LangSegment-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 24-Apr-03 09:56 LangSegment-0.3.0.dist-info/RECORD
-6 files, 60736 bytes uncompressed, 20223 bytes compressed:  66.7%
+Zip file size: 21195 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    44850 b- defN 24-Apr-07 05:24 LangSegment/LangSegment.py
+-rw-rw-rw-  2.0 fat      278 b- defN 24-Apr-07 05:25 LangSegment/__init__.py
+-rw-rw-rw-  2.0 fat    15227 b- defN 24-Apr-07 05:25 LangSegment-0.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-07 05:25 LangSegment-0.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-07 05:25 LangSegment-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 24-Apr-07 05:25 LangSegment-0.3.1.dist-info/RECORD
+6 files, 60937 bytes uncompressed, 20331 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: LangSegment/LangSegment.py
 Comment: 
 
 Filename: LangSegment/__init__.py
 Comment: 
 
-Filename: LangSegment-0.3.0.dist-info/METADATA
+Filename: LangSegment-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: LangSegment-0.3.0.dist-info/WHEEL
+Filename: LangSegment-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: LangSegment-0.3.0.dist-info/top_level.txt
+Filename: LangSegment-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: LangSegment-0.3.0.dist-info/RECORD
+Filename: LangSegment-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## LangSegment/LangSegment.py

```diff
@@ -268,15 +268,15 @@
         input = re.sub(r'\s+', '', input)
         if len(input) == 0 or abs(index) > len(input):return False,None
         ending_pattern = re.compile(r'([「」“”‘’"\':：。.！!?．？])')
         return ending_pattern.match(input[index]),input[index]
     
     @staticmethod
     def _cleans_text(cleans_text):
-        cleans_text = re.sub(r'(.*?)([^\w]+)', r'\1\2', cleans_text)
+        cleans_text = re.sub(r'(.*?)([^\w]+)', r'\1 ', cleans_text)
         cleans_text = re.sub(r'(.)\1+', r'\1', cleans_text)
         return cleans_text.strip()
     
     @staticmethod
     def _lang_classify(cleans_text):
         language, score = langid.classify(cleans_text)
         return language, score
@@ -305,14 +305,15 @@
             nextPunc = len(re.sub(regex_pattern,'',re.sub(r'\n+','',nextText)).strip()) == 0
             textPunc = len(re.sub(regex_pattern,'',re.sub(r'\n+','',text)).strip()) == 0
             if not EOS and (textPunc == True or ( len(nextText.strip()) >= 0 and nextPunc == True)):
                 lines[nextId] = f'{text}{nextText}'
                 continue
             number_tags = re.compile(r'(⑥\d{6,}⑥)')
             cleans_text = re.sub(number_tags, '' ,text)
+            cleans_text = re.sub(r'\d+', '' ,cleans_text)
             cleans_text = LangSegment._cleans_text(cleans_text)
             # fix:Langid's recognition of short sentences is inaccurate, and it is spliced longer.
             if not EOS and len(cleans_text) <= 2:
                 lines[nextId] = f'{text}{nextText}'
                 continue
             language,score = LangSegment._lang_classify(cleans_text)
             prev_language , prev_text = LangSegment._get_prev_data(words)
@@ -779,14 +780,16 @@
 비 오는 날에 음악을 듣는 것을 즐깁니다。
 J'aime écouter de la musique les jours de pluie.
 Tôi thích nghe nhạc vào những ngày mưa.
 Мне нравится слушать музыку в дождливую погоду.
 ฉันชอบฟังเพลงในวันที่ฝนตก
 """
 
+    text = "那我们拆分来看一下：Part A（传统阅读理解）,每题0.5分，共10分，第二部分"
+
 
     # 进行分词：（接入TTS项目仅需一行代码调用）Segmentation: (Only one line of code is required to access the TTS project)
     langlist = LangSegment.getTexts(text)
     printList(langlist)
     
     
     # 语种统计:Language statistics:
```

## LangSegment/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .LangSegment import LangSegment,getTexts,classify,getCounts,printList,setfilters,getfilters,setPriorityThreshold,getPriorityThreshold,setEnablePreview,getEnablePreview,setKeepPinyin,getKeepPinyin
 
 # release
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 
 # develop
 __develop__ = 'dev-0.0.1'
```

## Comparing `LangSegment-0.3.0.dist-info/METADATA` & `LangSegment-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LangSegment
-Version: 0.3.0
+Version: 0.3.1
 Summary: This is a multilingual tokenization tool that currently supports for zh/ja/en/ko, and more languages.
 Home-page: https://github.com/juntaosun/LangSegment
 Author: sunnyboxs
 License: BSD
 Keywords: language detection,language identification,langid,langid.py,nlp,language
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -35,17 +35,17 @@
 https://github.com/adbar/py3langid  
 
 
 功能：将文章或句子里的例如（中/英/日/韩），按不同语言自动识别分词，使文本更适合AI处理。    
 本代码专为各种 TTS 项目的前端文本多语种混合标注区分，多语言混合训练和推理而编写。
 
 ## 最近更新：News   
-* 版本：v0.3.0    
-* 添加支持： "zh"中文（数字拼音pinyin），保留发音指定。 
-* 添加支持： "ru"俄语Russian / "th"泰语Thai。（更新帮助见下文）。
+* 版本：v0.3.0   （更新帮助见下文）。
+* 添加支持： "zh"中文（数字拼音pinyin），保留多音字（音素）指定。 
+* 添加支持： "ru"俄语Russian / "th"泰语Thai。
 * 添加支持： "fr"法语French  / "vi"越南语Vietnamese。
 * 语言优先级，置信度评分和阀值。
 * 优化字符处理。fix: LangSegment.setfilters    
 * 更细致的处理，中日英韩，分词更精准！  
 * 多语言过滤组功能（默认:中/英/日/韩）！帮您自动清理不需要的语言内容。   
 * 添加 WebUI 可视化界面，运行 app.py 即可快捷体验（如图所示）。  
 
@@ -118,23 +118,23 @@
     # {'lang': 'en', 'text': 'L C D'}
     # {'lang': 'zh', 'text': '屏幕'}
     # ===========================================================================
     # 其中英文缩写字母如“LCD”，英文标准发音为“L-C-D”，
     # 而在语音合成TTS项目中，一般用空格隔开字母来单独发音：“L C D”
 ```
 
-## 拼读规则：支持  
+## 英文拼读：支持  
 ```python
 TTS语音合成（英文字母）大小写拼读规则：
 （1）需要单个字母发音就大写，比如：USA，USB，ChatGPT，LCD，GPU，CEO。
 （2）其它情况正常拼读，就按正常拼写。比如：Nvidia ， Cuda 或者全小写 （nvidia ， cuda ）
 ```
 
-## 拼音保留：支持  
-> 版本支持：>= 3.0.0    
+## 拼音保留：支持（多音字）  
+> 版本支持：>= 0.3.0  
 > 常见需求：直接修改 TTS 的汉字读音，保留拼音输入。  
 ```python
 # 开启汉语拼音保留，（TTS标准：数字拼音格式），默认关闭。  
 LangSegment.setKeepPinyin(True)  
 
 # 汉字拼音指定示例：以下句子，括号中的拼音，均识别为中文。
 text = "这个字的读音是角(jue2)色，而不是角(jiao3)色"
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LangSegment Version: 0.3.0 Summary: This is a
+Metadata-Version: 2.1 Name: LangSegment Version: 0.3.1 Summary: This is a
 multilingual tokenization tool that currently supports for zh/ja/en/ko, and
 more languages. Home-page: https://github.com/juntaosun/LangSegment Author:
 sunnyboxs License: BSD Keywords: language detection,language
 identification,langid,langid.py,nlp,language Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -22,18 +22,19 @@
 TTS (Text-to-Speech) synthesis projects, preprocessing of multilingual text
 mixing for both training and inference. >Implementation based on
 py3langidï¼See LICENSE file for more info. https://github.com/adbar/py3langid
 åè½ï¼å°æç« æå¥å­éçä¾å¦ï¼ä¸­/è±/æ¥/
 é©ï¼ï¼æä¸åè¯­è¨èªå¨è¯å«åè¯ï¼ä½¿ææ¬æ´éåAIå¤çã
 æ¬ä»£ç ä¸ä¸ºåç§ TTS
 é¡¹ç®çåç«¯ææ¬å¤è¯­ç§æ··åæ æ³¨åºåï¼å¤è¯­è¨æ··åè®­ç»åæ¨çèç¼åã
-## æè¿æ´æ°ï¼News * çæ¬ï¼v0.3.0 * æ·»å æ¯æï¼
-"zh"ä¸­æï¼æ°å­æ¼é³pinyinï¼ï¼ä¿çåé³æå®ã * æ·»å æ¯æï¼
-"ru"ä¿è¯­Russian / "th"æ³°è¯­Thaiãï¼æ´æ°å¸®å©è§ä¸æï¼ã *
-æ·»å æ¯æï¼ "fr"æ³è¯­French / "vi"è¶åè¯­Vietnameseã *
+## æè¿æ´æ°ï¼News * çæ¬ï¼v0.3.0 ï¼æ´æ°å¸®å©è§ä¸æï¼ã *
+æ·»å æ¯æï¼
+"zh"ä¸­æï¼æ°å­æ¼é³pinyinï¼ï¼ä¿çå¤é³å­ï¼é³ç´ ï¼æå®ã *
+æ·»å æ¯æï¼ "ru"ä¿è¯­Russian / "th"æ³°è¯­Thaiã * æ·»å æ¯æï¼
+"fr"æ³è¯­French / "vi"è¶åè¯­Vietnameseã *
 è¯­è¨ä¼åçº§ï¼ç½®ä¿¡åº¦è¯ååéå¼ã * ä¼åå­ç¬¦å¤çãfix:
 LangSegment.setfilters * æ´ç»è´çå¤çï¼ä¸­æ¥è±é©ï¼åè¯æ´ç²¾åï¼
 * å¤è¯­è¨è¿æ»¤ç»åè½ï¼é»è®¤:ä¸­/è±/æ¥/
 é©ï¼ï¼å¸®æ¨èªå¨æ¸çä¸éè¦çè¯­è¨åå®¹ã * æ·»å  WebUI
 å¯è§åçé¢ï¼è¿è¡ app.py å³å¯å¿«æ·ä½éªï¼å¦å¾æç¤ºï¼ã *
 _ç__¹_å__»_å__¨_ç_º_¿_ä_½__é_ª__ï_¼__æ___è_°_¢_ _h_u_g_g_i_n_g_f_a_c_e_ _æ___ä_¾__æ___å__¡_æ__¯_æ___ï_¼__[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-_S_p_a_c_e_s_-_b_l_u_e_] ![image](./
@@ -78,21 +79,22 @@
 {'lang': 'zh', 'text': ' 15ç³»åæºååä¸æ¬¾'} # {'lang': 'en', 'text':
 'Apple Watch'} # {'lang': 'zh', 'text': 'ç­ä¸ç³»åæ°åï¼è¿æ¬¡ç'} #
 {'lang': 'en', 'text': 'i Pad Air'} # {'lang': 'zh', 'text': 'éç¨äº'} #
 {'lang': 'en', 'text': 'L C D'} # {'lang': 'zh', 'text': 'å±å¹'} #
 =========================================================================== #
 å¶ä¸­è±æç¼©åå­æ¯å¦âLCDâï¼è±ææ ååé³ä¸ºâL-C-Dâï¼ #
 èå¨è¯­é³åæTTSé¡¹ç®ä¸­ï¼ä¸è¬ç¨ç©ºæ ¼éå¼å­æ¯æ¥åç¬åé³ï¼âL
-C Dâ ``` ## æ¼è¯»è§åï¼æ¯æ ```python
+C Dâ ``` ## è±ææ¼è¯»ï¼æ¯æ ```python
 TTSè¯­é³åæï¼è±æå­æ¯ï¼å¤§å°åæ¼è¯»è§åï¼
 ï¼1ï¼éè¦åä¸ªå­æ¯åé³å°±å¤§åï¼æ¯å¦ï¼USAï¼USBï¼ChatGPTï¼LCDï¼GPUï¼CEOã
 ï¼2ï¼å¶å®æåµæ­£å¸¸æ¼è¯»ï¼å°±ææ­£å¸¸æ¼åãæ¯å¦ï¼Nvidia ï¼ Cuda
-æèå¨å°å ï¼nvidia ï¼ cuda ï¼ ``` ## æ¼é³ä¿çï¼æ¯æ >
-çæ¬æ¯æï¼>= 3.0.0 > å¸¸è§éæ±ï¼ç´æ¥ä¿®æ¹ TTS
-çæ±å­è¯»é³ï¼ä¿çæ¼é³è¾å¥ã ```python #
+æèå¨å°å ï¼nvidia ï¼ cuda ï¼ ``` ##
+æ¼é³ä¿çï¼æ¯æï¼å¤é³å­ï¼ > çæ¬æ¯æï¼>= 0.3.0 >
+å¸¸è§éæ±ï¼ç´æ¥ä¿®æ¹ TTS çæ±å­è¯»é³ï¼ä¿çæ¼é³è¾å¥ã
+```python #
 å¼å¯æ±è¯­æ¼é³ä¿çï¼ï¼TTSæ åï¼æ°å­æ¼é³æ ¼å¼ï¼ï¼é»è®¤å³é­ã
 LangSegment.setKeepPinyin(True) #
 æ±å­æ¼é³æå®ç¤ºä¾ï¼ä»¥ä¸å¥å­ï¼æ¬å·ä¸­çæ¼é³ï¼åè¯å«ä¸ºä¸­æã
 text = "è¿ä¸ªå­çè¯»é³æ¯è§(jue2)è²ï¼èä¸æ¯è§(jiao3)è²" ``` ##
 åè¯çº éï¼å¾éè¦ï¼
 >ç»¼ä¸æè¿°ï¼âèªå¨åè¯âå·²ç»æå¤§çæé«äºæä»¬çå·¥ä½æçï¼ä½è¿æ¯å»ºè®®æ¨å¯¹åè¯ç»æè¿è¡äººå·¥æ ¡å¯¹ã
 ç¹å«æ¯ä¸­æä¸æ¥æï¼å­å¨å¤§éæ±å­äºç¨ï¼è¿å¯¹èªå¨åè¯æ¯æå·æææ§çï¼âåè¯çº éâ
```

