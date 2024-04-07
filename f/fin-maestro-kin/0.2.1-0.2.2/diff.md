# Comparing `tmp/fin_maestro_kin-0.2.1.tar.gz` & `tmp/fin_maestro_kin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fin_maestro_kin-0.2.1.tar", max compression
+gzip compressed data, was "fin_maestro_kin-0.2.2.tar", max compression
```

## Comparing `fin_maestro_kin-0.2.1.tar` & `fin_maestro_kin-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.1/fin_maestro_kin/__init__.py
--rw-r--r--   0        0        0     1518 2024-03-31 12:25:13.472776 fin_maestro_kin-0.2.1/fin_maestro_kin/constants.py
--rw-r--r--   0        0        0      545 2024-03-09 11:03:03.068361 fin_maestro_kin-0.2.1/fin_maestro_kin/main.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/__init__.py
--rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/data_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
--rw-r--r--   0        0        0    11609 2024-03-31 12:25:13.473778 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/data_toolkit/nse/helper.py
--rw-r--r--   0        0        0    18970 2024-03-31 12:25:13.475780 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
--rw-r--r--   0        0        0     7772 2024-03-16 08:38:01.420066 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/sentiment_analysis/__init__.py
--rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
--rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/trend_detector/__init__.py
--rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.1/fin_maestro_kin/modules/trend_detector/trend_detector.py
--rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.1/LICENSE
--rw-r--r--   0        0        0      582 2024-03-31 12:41:01.027333 fin_maestro_kin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5339 2024-03-31 06:18:04.202217 fin_maestro_kin-0.2.1/README.md
--rw-r--r--   0        0        0     6218 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.2/fin_maestro_kin/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-07 12:51:01.798236 fin_maestro_kin-0.2.2/fin_maestro_kin/constants.py
+-rw-r--r--   0        0        0      545 2024-03-09 11:03:03.068361 fin_maestro_kin-0.2.2/fin_maestro_kin/main.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/__init__.py
+-rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
+-rw-r--r--   0        0        0    12664 2024-04-07 13:52:02.139544 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/helper.py
+-rw-r--r--   0        0        0    18970 2024-04-07 12:51:02.233160 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
+-rw-r--r--   0        0        0     7634 2024-04-07 13:52:15.430589 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/__init__.py
+-rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
+-rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/trend_detector/__init__.py
+-rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/trend_detector/trend_detector.py
+-rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.2/LICENSE
+-rw-r--r--   0        0        0      614 2024-04-07 13:53:15.823782 fin_maestro_kin-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5339 2024-03-31 06:18:04.202217 fin_maestro_kin-0.2.2/README.md
+-rw-r--r--   0        0        0     6179 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.2/PKG-INFO
```

### Comparing `fin_maestro_kin-0.2.1/fin_maestro_kin/constants.py` & `fin_maestro_kin-0.2.2/fin_maestro_kin/constants.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.1/fin_maestro_kin/main.py` & `fin_maestro_kin-0.2.2/fin_maestro_kin/main.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.1/fin_maestro_kin/modules/data_toolkit/nse/helper.py` & `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -294,7 +294,37 @@
             "company": entry["companyName"],
             "from_year": entry["fromYr"],
             "to_year": entry["toYr"],
             "attachment": entry["fileName"],
         }
         processed_data.append(processed_entry)
     return processed_data
+
+
+import json
+
+import json
+
+def process_index_data(data):
+    data_json = data.to_json(orient="records")
+
+    try:
+        data = json.loads(data_json)
+    except json.JSONDecodeError:
+        return {"error": "Invalid JSON data"}
+
+    processed_data = []
+    for entry in data:
+        processed_entry = {
+            "index_name": entry["indexCloseOnlineRecords"]["EOD_INDEX_NAME"],
+            "open_value": entry["indexCloseOnlineRecords"]["EOD_OPEN_INDEX_VAL"],
+            "high_value": entry["indexCloseOnlineRecords"]["EOD_HIGH_INDEX_VAL"],
+            "close_value": entry["indexCloseOnlineRecords"]["EOD_CLOSE_INDEX_VAL"],
+            "low_value": entry["indexCloseOnlineRecords"]["EOD_LOW_INDEX_VAL"],
+            "timestamp": entry["indexCloseOnlineRecords"]["EOD_TIMESTAMP"],
+            "traded_quantity": entry["indexTurnoverRecords"]["HIT_TRADED_QTY"],
+            "turnover": entry["indexTurnoverRecords"]["HIT_TURN_OVER"]
+        }
+        processed_data.append(processed_entry)
+    return processed_data
+
+
```

### Comparing `fin_maestro_kin-0.2.1/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py` & `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.1/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py` & `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,40 @@
 from fastapi.responses import JSONResponse
 import requests
 import json
 import pandas as pd
 import datetime
 
 router = APIRouter(tags=["NSE Indices"])
-
+    
 
 def index_history(symbol, start_date, end_date):
-    start_date = datetime.datetime.strptime(start_date, "%d-%b-%Y").strftime("%d %b %Y")
-    end_date = datetime.datetime.strptime(end_date, "%d-%b-%Y").strftime("%d %b %Y")
-
-    data = {"cinfo": f"{{'name':'{symbol}','startDate':'{start_date}','endDate':'{end_date}'}}"}
-    payload = requests.post('https://www.niftyindices.com/Backpage.aspx/getpepbHistoricaldataDBtoString', json=data, headers=niftyindices_headers).json()
-    payload = json.loads(payload["d"])
+    base_url="https://www.nseindia.com/api/historical/indicesHistory"
+    customized_request_url = f"{base_url}?indexType={symbol}&from={start_date}&to={end_date}"
+    response=fetch_data_from_nse(customized_request_url)
+    
+    payload = response.get('data', [])
     
     if not payload:
-        raise HTTPException(status_code=404, detail="No historical data found.")
+        raise HTTPException(status_code=404, detail=f"No data found for the specified parameters.")
     
-    payload = pd.DataFrame.from_records(payload)
-    return payload
+    return pd.DataFrame(payload)
 
 
-#Example usage - 127.0.0.1:8000/nseindices/history?symbol=NIFTY 50&start_date=10-Jan-2024&end_date=12-Jan-2024
+#Example usage - 127.0.0.1:8000/nseindices/history?symbol=NIFTY 50&start_date=10-01-2024&end_date=12-02-2024
 @router.get("/nseindices/history",tags=["NSE Indices"])
-def get_nse_indices_history(
-    symbol: str = Query(..., title="Symbol", description="Nifty indices symbol"),
-    start_date: str = Query(..., title="Start Date", description="Start date for historical data in dd-mmm-yyyy format"),
-    end_date: str = Query(..., title="End Date", description="End date for historical data in dd-mmm-yyyy format")
+def get_nse_index_history(
+    symbol: str = Query(..., title="Symbol", description="NSE indices symbol"),
+    start_date: str = Query(..., title="Start Date", description="Start date for historical data in dd-mm-yyyy format"),
+    end_date: str = Query(..., title="End Date", description="End date for historical data in dd-mm-yyyy format")
 ):
     try:
         history_data = index_history(symbol, start_date, end_date)
-        return history_data.to_dict(orient='records')
+        processed_data = process_index_data(history_data)
+        return JSONResponse(content={"index_historical_data": processed_data})
     except Exception as e:
         raise HTTPException(status_code=500, detail=f"Error fetching historical data: {e}")
     
 
 def index_pe_pb_div(symbol, start_date, end_date):
     start_date = datetime.datetime.strptime(start_date, "%d-%b-%Y").strftime("%d %b %Y")
     end_date = datetime.datetime.strptime(end_date, "%d-%b-%Y").strftime("%d %b %Y")
```

### Comparing `fin_maestro_kin-0.2.1/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py` & `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.1/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py` & `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.1/fin_maestro_kin/modules/trend_detector/trend_detector.py` & `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/trend_detector/trend_detector.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.1/LICENSE` & `fin_maestro_kin-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.1/pyproject.toml` & `fin_maestro_kin-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fin-maestro-kin"
-version = "0.2.1"
+version = "0.2.2"
 description = "Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API."
 authors = ["DEV_FINWIZ <devjuneja43@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,13 +12,14 @@
 uvicorn = "^0.25.0"
 pydantic = "^2.5.3"
 requests = "^2.31.0"
 yfinance = "^0.2.35"
 matplotlib = "^3.8.2"
 pandas = "^2.1.4"
 numpy = "^1.26.3"
-pytest = "^8.1.1"
 
+[tool.poetry.dev-dependencies]
+pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fin_maestro_kin-0.2.1/README.md` & `fin_maestro_kin-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.1/PKG-INFO` & `fin_maestro_kin-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fin-maestro-kin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API.
 License: MIT
 Author: DEV_FINWIZ
 Author-email: devjuneja43@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
-Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.25.0,<0.26.0)
 Requires-Dist: yfinance (>=0.2.35,<0.3.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img width="394" alt="image" src="https://github.com/devfinwiz/Fin-Maestro-Kin/assets/78873223/9a6e71e2-2867-49c5-b930-980a871bcb34">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.1 Summary: Where Data
+Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.2 Summary: Where Data
 Meets FastAPI Brilliance with Fin-Maestro-Kin â Your All-in-One Finance API.
 License: MIT Author: DEV_FINWIZ Author-email: devjuneja43@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0) Requires-Dist: numpy
 (>=1.26.3,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist:
-pydantic (>=2.5.3,<3.0.0) Requires-Dist: pytest (>=8.1.1,<9.0.0) Requires-Dist:
-requests (>=2.31.0,<3.0.0) Requires-Dist: uvicorn (>=0.25.0,<0.26.0) Requires-
-Dist: yfinance (>=0.2.35,<0.3.0) Description-Content-Type: text/markdown
+pydantic (>=2.5.3,<3.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
+Dist: uvicorn (>=0.25.0,<0.26.0) Requires-Dist: yfinance (>=0.2.35,<0.3.0)
+Description-Content-Type: text/markdown
                                     [image]
                          ************ FFiinn--MMaaeessttrroo--KKiinn ************
         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_F_a_c_t_o_r_-_A_-_b_l_u_e_&_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
  _b_a_d_g_e_&_c_o_l_o_r_=_b_l_u_e_][https://img.shields.io/badge/Python-3.9.1-blue&?style=for-
   the-badge&color=blue]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-
  _M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_p_u_r_p_l_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
 _l_a_s_t_-_c_o_m_m_i_t_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_y_e_l_l_o_w_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/
```

