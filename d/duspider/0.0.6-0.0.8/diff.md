# Comparing `tmp/duspider-0.0.6.tar.gz` & `tmp/duspider-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duspider-0.0.6.tar", last modified: Mon Nov 13 08:23:58 2023, max compression
+gzip compressed data, was "duspider-0.0.8.tar", last modified: Tue Nov 28 08:32:31 2023, max compression
```

## Comparing `duspider-0.0.6.tar` & `duspider-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-11-13 08:23:58.429796 duspider-0.0.6/
--rw-rw-rw-   0        0        0      385 2023-11-13 08:23:58.428795 duspider-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-09-18 00:50:10.000000 duspider-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-11-13 08:23:58.418296 duspider-0.0.6/duspider/
--rw-rw-rw-   0        0        0       89 2023-09-18 02:11:31.000000 duspider-0.0.6/duspider/__init__.py
--rw-rw-rw-   0        0        0     5945 2023-11-13 08:22:18.000000 duspider-0.0.6/duspider/askbob.py
--rw-rw-rw-   0        0        0     2603 2023-11-08 07:54:55.000000 duspider-0.0.6/duspider/base.py
--rw-rw-rw-   0        0        0    18555 2023-11-13 08:23:17.000000 duspider-0.0.6/duspider/drugbank.py
--rw-rw-rw-   0        0        0      652 2023-11-08 07:32:07.000000 duspider-0.0.6/duspider/exceptions.py
--rw-rw-rw-   0        0        0     4334 2023-11-09 02:00:33.000000 duspider-0.0.6/duspider/medscape.py
--rw-rw-rw-   0        0        0      601 2023-11-09 01:58:51.000000 duspider-0.0.6/duspider/tools.py
--rw-rw-rw-   0        0        0     3857 2023-09-18 02:17:35.000000 duspider-0.0.6/duspider/uniprot.py
-drwxrwxrwx   0        0        0        0 2023-11-13 08:23:58.426797 duspider-0.0.6/duspider.egg-info/
--rw-rw-rw-   0        0        0      385 2023-11-13 08:23:58.000000 duspider-0.0.6/duspider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-11-13 08:23:58.000000 duspider-0.0.6/duspider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-13 08:23:58.000000 duspider-0.0.6/duspider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-11-13 08:23:58.000000 duspider-0.0.6/duspider.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-11-13 08:23:58.000000 duspider-0.0.6/duspider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-13 08:23:58.429796 duspider-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2015 2023-11-13 08:23:34.000000 duspider-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-28 08:32:31.038434 duspider-0.0.8/
+-rw-rw-rw-   0        0        0      385 2023-11-28 08:32:31.037433 duspider-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-09-18 00:50:10.000000 duspider-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-11-28 08:32:31.009934 duspider-0.0.8/duspider/
+-rw-rw-rw-   0        0        0       89 2023-09-18 02:11:31.000000 duspider-0.0.8/duspider/__init__.py
+-rw-rw-rw-   0        0        0     2637 2023-11-17 01:00:39.000000 duspider-0.0.8/duspider/base.py
+drwxrwxrwx   0        0        0        0 2023-11-28 08:32:31.023936 duspider-0.0.8/duspider/diseases/
+-rw-rw-rw-   0        0        0       92 2023-11-27 08:58:32.000000 duspider-0.0.8/duspider/diseases/__init__.py
+-rw-rw-rw-   0        0        0     6037 2023-11-28 02:41:46.000000 duspider-0.0.8/duspider/diseases/askbob.py
+-rw-rw-rw-   0        0        0     3424 2023-11-28 08:30:30.000000 duspider-0.0.8/duspider/diseases/baidu.py
+drwxrwxrwx   0        0        0        0 2023-11-28 08:32:31.035434 duspider-0.0.8/duspider/drugs/
+-rw-rw-rw-   0        0        0       92 2023-11-16 07:38:54.000000 duspider-0.0.8/duspider/drugs/__init__.py
+-rw-rw-rw-   0        0        0     5945 2023-11-13 08:22:18.000000 duspider-0.0.8/duspider/drugs/askbob.py
+-rw-rw-rw-   0        0        0    19340 2023-11-21 11:02:19.000000 duspider-0.0.8/duspider/drugs/drugbank.py
+-rw-rw-rw-   0        0        0     9051 2023-11-27 08:59:01.000000 duspider-0.0.8/duspider/drugs/medlive.py
+-rw-rw-rw-   0        0        0     4334 2023-11-09 02:00:33.000000 duspider-0.0.8/duspider/drugs/medscape.py
+-rw-rw-rw-   0        0        0     5682 2023-11-27 03:20:28.000000 duspider-0.0.8/duspider/drugs/nmpa_gov.py
+-rw-rw-rw-   0        0        0     3857 2023-09-18 02:17:35.000000 duspider-0.0.8/duspider/drugs/uniprot.py
+-rw-rw-rw-   0        0        0      652 2023-11-08 07:32:07.000000 duspider-0.0.8/duspider/exceptions.py
+-rw-rw-rw-   0        0        0      601 2023-11-09 01:58:51.000000 duspider-0.0.8/duspider/tools.py
+drwxrwxrwx   0        0        0        0 2023-11-28 08:32:31.019435 duspider-0.0.8/duspider.egg-info/
+-rw-rw-rw-   0        0        0      385 2023-11-28 08:32:30.000000 duspider-0.0.8/duspider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-11-28 08:32:30.000000 duspider-0.0.8/duspider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-28 08:32:30.000000 duspider-0.0.8/duspider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-11-28 08:32:30.000000 duspider-0.0.8/duspider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-11-28 08:32:30.000000 duspider-0.0.8/duspider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-28 08:32:31.038434 duspider-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2015 2023-11-28 08:32:15.000000 duspider-0.0.8/setup.py
```

### Comparing `duspider-0.0.6/duspider/askbob.py` & `duspider-0.0.8/duspider/drugs/askbob.py`

 * *Files identical despite different names*

### Comparing `duspider-0.0.6/duspider/base.py` & `duspider-0.0.8/duspider/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.cookies = cookies
         self.timeout = timeout
         self.max_retry = max_retry  # 最多重试次数
         # max_keepalive_connections 允许的保持活动状态连接数，或None始终允许。（默认值 20）
         # max_connections 允许的最大连接数，或None无限制。（默认值 100）
         limits = httpx.Limits(max_keepalive_connections=sem, max_connections=sem + 3)
         # client = httpx.Client(limits=limits) # 同步
-        self.client = httpx.AsyncClient(limits=limits)  # 异步
+        self.client = httpx.AsyncClient(cookies=cookies, headers=headers, limits=limits)  # 异步
 
     async def post(self, url, **kwargs):
         for i in range(self.max_retry):
             try:
                 resp = await self.client.post(url,
                                               timeout=self.timeout,
                                               follow_redirects=True,
```

### Comparing `duspider-0.0.6/duspider/drugbank.py` & `duspider-0.0.8/duspider/drugs/drugbank.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     pathways: List = []  # 作用通路
     pharmacogenomic_effects: List = []  # 药物基因组学效应
     absorption: List = []  # 吸收
     volume_distribution: List = []  # 分布容积
     protein_binding: List = []  # 蛋白结合
     metabolism: List = []  # 代谢
     half_life: List = []  # 半衰期
+    route_elimination: List = []  # 排泄路径
     clearance: List = []  # 清除率
     drug_interaction: List[DrugInteraction] = []  # 相互作用
     food_interaction: List = []  # 食物相互作用
     toxicity: List = []  # 毒性
 
     async def get_drug_interaction(self) -> List[DrugInteraction]:
         """获取药物相互作用"""
@@ -79,36 +80,37 @@
             "APPROVED": "approved",
             "VET APPROVED": "vet_approved",
             "NUTRACEUTICAL": "nutraceutical",
             "ILLICIT": "illicit",
             "WITHDRAWN": "withdrawn",
             "INVESTIGATIONAL": "investigational",
             "EXPERIMENTAL": "experimental",
-            # "ALL DRUGS": "approved",
+            "ALL DRUGS": "",
 
         }
 
         self.cookies = {
-            'cf_clearance': 'iVXRxn7oiGYaKCn9xvS2Vvh18onAE14BP3qBXxOAdIw-1699411572-0-1-49c08f63.a63988a7.1ec1d083-250.0.0',
-            '_ga': 'GA1.1.414772354.1699411591',
-            '_clck': '1iz72qk|2|fgj|0|1407',
-            '_gcl_au': '1.1.1616239398.1699411594',
-            'hubspotutk': '41c7d7c1e3ab76361ec9f970d6f71fe5',
+            'cf_clearance': '9CxXKpW8mebKnSit5yh1NZN6gFpNMMzoVNkeEvWbnss-1700557883-0-1-ab8f8168.58cca9e0.47421a7d-250.0.0',
+            '_ga': 'GA1.1.95134515.1700557898',
+            '_clck': 'bq5bql%7C2%7Cfgw%7C0%7C1420',
+            '_gcl_au': '1.1.559936620.1700559173',
+            '__hstc': '49600953.7bf0ba33f1c267f0db05efea95a2ca13.1700559180121.1700559180121.1700559180121.1',
+            'hubspotutk': '7bf0ba33f1c267f0db05efea95a2ca13',
             '__hssrc': '1',
-            '__hstc': '49600953.41c7d7c1e3ab76361ec9f970d6f71fe5.1699411596013.1699428178142.1699435168990.4',
-            '_omx_drug_bank_session': 'VJRsvDDYUOI9yCgaJl6KFEKKhD%2FPrQupM%2BR1IQfb%2FdHZrOUYg6LwdpaMWtedF9WCuvjZEsEWUOoQccrUoOJlnMdqIv3zCWsxhdV%2FrS72Yg7X8WPJphIKSmg%2BM6frrx29%2F%2Fe98VLjwAZ7HmVuqWJrUxaTYRBmFS1G7p3rqllDrFmqeO7WZQdcXv0x%2BavjLDpf5lKpzu8WkbY73LBJ1%2FoFMMPPYVAQZJnozYGubDBzt2tmoBFrD1BAzZpVIegf5vl2wvWLKSfal2y8n7nwjEOEQsOU9c2nWQsX6JK2eFvBC%2FCrRUlRHt3%2BTun0RBBgY4R9jN%2Fjo%2BSnQ%2FUsk2O6TNhfaRKZKkNr4%2FIwvN8q%2Ftuxl8THsnl%2B03o%3D--%2FhCjuwnK7HfGranh--YZCJ6lHNcfTtZ082h2QBNA%3D%3D',
-            '_ga_DDLJ7EEV9M': 'GS1.1.1699443244.6.1.1699443245.59.0.0',
-            '_clsk': 'vgvnve|1699443246906|1|1|u.clarity.ms/collect',
+            '_omx_drug_bank_session': '4FapiRjA7Z2zO5ghJjCWnl3DIPna5l5ZTKuOGnq64n2%2B5LOCV6sICC2lr89L%2BiZdkVnrzQBhibMFwJowHG1GwFQ%2BxMxAlI%2FNxgUnTpj4V1yCVOPnSq%2BgmUClErgxdQ8OdisQRJKJp5EBwTMjJ56%2FuTPGPr%2FLrK1wsXkGeKkb%2B73TpvMupVOh6aXGGv4yB89bs2oAGqftWXWHFG92s2HfFyYhLjJtFuKA6pTpqbRDio4vc7PQREEDAbo2SK2AUyZdWfJVIqj%2BGREP5AZacJiS0wb8kL59n5tftQUaJ%2BwglK15WG%2BW2kraRAXKE5%2FOLe%2FJF5zc2g17eTh65FPbdVk%2BQk5nKri0aSmQAp9%2BeQPSFmC0IL81B9s%3D--CV2%2FalJJ2uGjbJSR--uEOqXApPLoSQU9n%2F7Bi7IA%3D%3D',
+            '_ga_DDLJ7EEV9M': 'GS1.1.1700564382.2.0.1700564382.60.0.0',
+            '_clsk': '1ew0qm%7C1700564418090%7C1%7C1%7Cy.clarity.ms%2Fcollect',
         }
+
         self.headers = {
             'authority': 'go.drugbank.com',
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
             'accept-language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
             'cache-control': 'no-cache',
-            # 'cookie': 'cf_clearance=iVXRxn7oiGYaKCn9xvS2Vvh18onAE14BP3qBXxOAdIw-1699411572-0-1-49c08f63.a63988a7.1ec1d083-250.0.0; _ga=GA1.1.414772354.1699411591; _clck=1iz72qk|2|fgj|0|1407; _gcl_au=1.1.1616239398.1699411594; hubspotutk=41c7d7c1e3ab76361ec9f970d6f71fe5; __hssrc=1; __hstc=49600953.41c7d7c1e3ab76361ec9f970d6f71fe5.1699411596013.1699428178142.1699435168990.4; _omx_drug_bank_session=VJRsvDDYUOI9yCgaJl6KFEKKhD%2FPrQupM%2BR1IQfb%2FdHZrOUYg6LwdpaMWtedF9WCuvjZEsEWUOoQccrUoOJlnMdqIv3zCWsxhdV%2FrS72Yg7X8WPJphIKSmg%2BM6frrx29%2F%2Fe98VLjwAZ7HmVuqWJrUxaTYRBmFS1G7p3rqllDrFmqeO7WZQdcXv0x%2BavjLDpf5lKpzu8WkbY73LBJ1%2FoFMMPPYVAQZJnozYGubDBzt2tmoBFrD1BAzZpVIegf5vl2wvWLKSfal2y8n7nwjEOEQsOU9c2nWQsX6JK2eFvBC%2FCrRUlRHt3%2BTun0RBBgY4R9jN%2Fjo%2BSnQ%2FUsk2O6TNhfaRKZKkNr4%2FIwvN8q%2Ftuxl8THsnl%2B03o%3D--%2FhCjuwnK7HfGranh--YZCJ6lHNcfTtZ082h2QBNA%3D%3D; _ga_DDLJ7EEV9M=GS1.1.1699443244.6.1.1699443245.59.0.0; _clsk=vgvnve|1699443246906|1|1|u.clarity.ms/collect',
+            # 'cookie': 'cf_clearance=9CxXKpW8mebKnSit5yh1NZN6gFpNMMzoVNkeEvWbnss-1700557883-0-1-ab8f8168.58cca9e0.47421a7d-250.0.0; _ga=GA1.1.95134515.1700557898; _clck=bq5bql%7C2%7Cfgw%7C0%7C1420; _gcl_au=1.1.559936620.1700559173; __hstc=49600953.7bf0ba33f1c267f0db05efea95a2ca13.1700559180121.1700559180121.1700559180121.1; hubspotutk=7bf0ba33f1c267f0db05efea95a2ca13; __hssrc=1; _omx_drug_bank_session=4FapiRjA7Z2zO5ghJjCWnl3DIPna5l5ZTKuOGnq64n2%2B5LOCV6sICC2lr89L%2BiZdkVnrzQBhibMFwJowHG1GwFQ%2BxMxAlI%2FNxgUnTpj4V1yCVOPnSq%2BgmUClErgxdQ8OdisQRJKJp5EBwTMjJ56%2FuTPGPr%2FLrK1wsXkGeKkb%2B73TpvMupVOh6aXGGv4yB89bs2oAGqftWXWHFG92s2HfFyYhLjJtFuKA6pTpqbRDio4vc7PQREEDAbo2SK2AUyZdWfJVIqj%2BGREP5AZacJiS0wb8kL59n5tftQUaJ%2BwglK15WG%2BW2kraRAXKE5%2FOLe%2FJF5zc2g17eTh65FPbdVk%2BQk5nKri0aSmQAp9%2BeQPSFmC0IL81B9s%3D--CV2%2FalJJ2uGjbJSR--uEOqXApPLoSQU9n%2F7Bi7IA%3D%3D; _ga_DDLJ7EEV9M=GS1.1.1700564382.2.0.1700564382.60.0.0; _clsk=1ew0qm%7C1700564418090%7C1%7C1%7Cy.clarity.ms%2Fcollect',
             'dnt': '1',
             'pragma': 'no-cache',
             'sec-ch-ua': '"Microsoft Edge";v="119", "Chromium";v="119", "Not?A_Brand";v="24"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'document',
             'sec-fetch-mode': 'navigate',
@@ -121,43 +123,43 @@
     def get_time(self):
         millis = int(round(time.time() * 1000))
         return str(millis)
 
     def get_params(self, g_type, size=100):
         return {
             'group': g_type,
-            'draw': '1',
+            'draw': 1,
             'columns[0][data]': '0',
             'columns[0][name]': '',
             'columns[0][searchable]': 'true',
             'columns[0][orderable]': 'true',
             'columns[0][search][value]': '',
             'columns[0][search][regex]': 'false',
             'columns[1][data]': '1',
             'columns[1][name]': '',
             'columns[1][searchable]': 'true',
             'columns[1][orderable]': 'true',
             'columns[1][search][value]': '',
             'columns[1][search][regex]': 'false',
-            'start': '0',
-            'length': f'{size}',  # 最大
+            'start': 0,
+            'length': size,  # 最大
             'search[value]': '',
             'search[regex]': 'false',
             '_': self.get_time(),
         }
 
     def parse_drug_interactions(self, k, data):
         _list = []
         for row in data:
             try:
                 _list.append(DrugInteraction(
-                uid=re.findall("/drugs/(.*?)\">", row[0])[0],
-                name=re.findall(">(.*?)</a>", row[0])[0],
-                desc=row[1],
-                type=k
+                    uid=re.findall("/drugs/(.*?)\">", row[0])[0],
+                    name=re.findall(">(.*?)</a>", row[0])[0],
+                    desc=row[1],
+                    type=k
                 ))
             except Exception as e:
                 print(row)
         return _list
 
     async def sem_drug_interactions(self, k, url, params):
         res = await self.get(url, params=params, headers=self.headers, cookies=self.cookies)
@@ -170,28 +172,35 @@
     @aio_timer
     async def get_drug_interactions(self, drug_id):
         url = f'https://go.drugbank.com/drugs/{drug_id}/drug_interactions.json'
         res_list = []
         self.headers['referer'] = f'https://go.drugbank.com/drugs/{drug_id}'
         for k, v in self.data.items():
             params = self.get_params(v)
+            params["draw"] = 0
+            if v == '':
+                del params['group']
             res = await self.get(url, params=params, headers=self.headers, cookies=self.cookies)
-            if res:
-                data = res.json()
-                total = data['recordsTotal']
-                info = self.parse_drug_interactions(k, data.get('data', []))
-                if info:
-                    res_list += info
-                if total > 100:
-                    pages = ceil(total / 100)
-                    for page_ in range(1, pages):
-                        params['start'] = f'{page_}'
-                        info = self.parse_drug_interactions(k, data.get('data', []))
+            data = res.json()
+            total = data['recordsTotal']
+            info = self.parse_drug_interactions(k, data.get('data', []))
+            if info:
+                res_list += info
+            if total > 100:
+                pages = ceil(total / 100)
+                for page_ in range(1, pages):
+                    params['start'] += 100
+                    params["draw"] += 2
+                    params["_"] = self.get_time()
+                    resp = await self.get(url, params=params, headers=self.headers, cookies=self.cookies)
+                    data = resp.json()
+                    info = self.parse_drug_interactions(k, data.get('data', []))
+                    if info:
                         res_list += info
-                        time.sleep(20)
+                    # time.sleep(20)
         return res_list
 
     @aio_timer
     async def get_drug_interactions2(self, drug_id):
         url = f'https://go.drugbank.com/drugs/{drug_id}/drug_interactions.json'
         task_list = []
         res_list = []
@@ -308,14 +317,18 @@
         protein_binding = self.parse_list(protein_binding_list)
         volume_distribution_list = doc.xpath('//dt[@id="volume-of-distribution"]/following-sibling::dd[1]//p')
         volume_distribution = self.parse_list(volume_distribution_list)
 
         absorption_list = doc.xpath('//dt[@id="absorption"]/following-sibling::dd[1]//p')
         absorption = self.parse_list(absorption_list)
 
+        route_of_elimination = doc.xpath('//dt[@id="route-of-elimination"]/following-sibling::dd[1]//p')
+        print('aa:', route_of_elimination)
+        route_elimination = self.parse_list(route_of_elimination)
+
         pharmacodynamics_list = doc.xpath('//dt[@id="pharmacodynamics"]/following-sibling::dd[1]//p')
         pharmacodynamics = self.parse_list(pharmacodynamics_list)
 
         biologic_classification_1 = doc.xpath(
             '//dt[@id="biologic-classification"]/following-sibling::dd[1]/text()').get('').strip()
         biologic_classification_2 = doc.xpath(
             'string(//dt[@id="biologic-classification"]/following-sibling::dd[1]//span)').get('').strip()
@@ -368,14 +381,15 @@
             pharmacogenomic_effects=pharmacogenomic_effects,
             mechanism_action=mechanism_action,
             food_interaction=food_interaction,
             toxicity=toxicity,
             pharmacodynamics=pharmacodynamics,
             biologic_classification=biologic_classification,
             sequences=sequences,
+            route_elimination=route_elimination,
             structure=structure,
             absorption=absorption,
             volume_distribution=volume_distribution,
             protein_binding=protein_binding,
             clearance=clearance,
             metabolism=metabolism,
             half_life=half_life,
@@ -388,10 +402,15 @@
 
 
 if __name__ == '__main__':
     drug = DrugBank()
     import asyncio
 
     # res = asyncio.run(drug.get_data('DB09532'))
-    # res = asyncio.run(drug.get_data('DB00091'))
-    res = asyncio.run(drug.get_drug_interactions('DB00023'))
-    # print(res.json())
+    res = asyncio.run(drug.get_data('DB00091'))
+    # https://go.drugbank.com/drugs/DB00001
+    # res = asyncio.run(drug.get_drug_interactions('DB00001'))
+    print(res)
+
+    # print(json.dumps(res))
+    # print(json.dumps(res))
+    # print(json.dumps([dict(i) for i in res]))
```

### Comparing `duspider-0.0.6/duspider/exceptions.py` & `duspider-0.0.8/duspider/exceptions.py`

 * *Files identical despite different names*

### Comparing `duspider-0.0.6/duspider/medscape.py` & `duspider-0.0.8/duspider/drugs/medscape.py`

 * *Files identical despite different names*

### Comparing `duspider-0.0.6/duspider/tools.py` & `duspider-0.0.8/duspider/tools.py`

 * *Files identical despite different names*

### Comparing `duspider-0.0.6/duspider/uniprot.py` & `duspider-0.0.8/duspider/drugs/uniprot.py`

 * *Files identical despite different names*

### Comparing `duspider-0.0.6/setup.py` & `duspider-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 # 提供一些有用的信息
 NAME = 'duspider'  # Python 包的名称，即在 pip install 时后面跟的包名
-VERSION = '0.0.6'  # 包的版本，每次上传到 PyPI 都需要改变这个版本号，否则只会往存储空间增加新内容，无法达到预期
+VERSION = '0.0.8'  # 包的版本，每次上传到 PyPI 都需要改变这个版本号，否则只会往存储空间增加新内容，无法达到预期
 DESCRIPTION = "Commonly used spiders"  # 关于该包的剪短描述
 
 readme = Path('README.md')
 
 if readme.exists():  # 如果需要，可以加入一段较长的描述，比如读取 README.md，该段长描述会直接显示在 PyPI 的页面上
     with open(readme, encoding='utf-8') as f:
         LONG_DESCRIPTION = f.read()
```

