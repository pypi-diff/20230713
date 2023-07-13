# Comparing `tmp/pysisnoapi-0.1.0.tar.gz` & `tmp/pysisnoapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysisnoapi-0.1.0.tar", max compression
+gzip compressed data, was "pysisnoapi-0.1.1.tar", max compression
```

## Comparing `pysisnoapi-0.1.0.tar` & `pysisnoapi-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1110 2023-05-17 15:04:44.164424 pysisnoapi-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      443 2023-07-07 10:50:41.800472 pysisnoapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    33193 2023-07-07 10:50:41.803140 pysisnoapi-0.1.0/pysisnoapi/__init__.py
--rw-r--r--   0        0        0     4832 2023-07-07 10:50:41.805140 pysisnoapi-0.1.0/pysisnoapi/misc.py
--rw-r--r--   0        0        0    26902 2023-07-07 10:50:41.807139 pysisnoapi-0.1.0/pysisnoapi/nfe.py
--rw-r--r--   0        0        0    14107 2023-07-07 10:50:41.809141 pysisnoapi-0.1.0/pysisnoapi/nfse.py
--rw-r--r--   0        0        0     1948 2023-06-15 16:45:12.885630 pysisnoapi-0.1.0/README.md
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 pysisnoapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-05-17 15:04:44.164424 pysisnoapi-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      443 2023-07-13 13:14:25.911967 pysisnoapi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    33193 2023-07-07 10:50:41.803140 pysisnoapi-0.1.1/pysisnoapi/__init__.py
+-rw-r--r--   0        0        0     4832 2023-07-07 10:50:41.805140 pysisnoapi-0.1.1/pysisnoapi/misc.py
+-rw-r--r--   0        0        0    26902 2023-07-07 10:50:41.807139 pysisnoapi-0.1.1/pysisnoapi/nfe.py
+-rw-r--r--   0        0        0    14078 2023-07-12 14:48:56.857910 pysisnoapi-0.1.1/pysisnoapi/nfse.py
+-rw-r--r--   0        0        0     1881 2023-07-07 17:08:58.354975 pysisnoapi-0.1.1/README.md
+-rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 pysisnoapi-0.1.1/PKG-INFO
```

### Comparing `pysisnoapi-0.1.0/LICENSE.md` & `pysisnoapi-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysisnoapi-0.1.0/pysisnoapi/__init__.py` & `pysisnoapi-0.1.1/pysisnoapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pysisnoapi-0.1.0/pysisnoapi/misc.py` & `pysisnoapi-0.1.1/pysisnoapi/misc.py`

 * *Files identical despite different names*

### Comparing `pysisnoapi-0.1.0/pysisnoapi/nfe.py` & `pysisnoapi-0.1.1/pysisnoapi/nfe.py`

 * *Files identical despite different names*

### Comparing `pysisnoapi-0.1.0/pysisnoapi/nfse.py` & `pysisnoapi-0.1.1/pysisnoapi/nfse.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,23 +329,22 @@
         params['ordenacao'] = ordencao
     if tipo_ordenacao:
         params['tipoOrdenacao'] = tipo_ordenacao
 
     url = f'{BASE_URL}/nfse'
     
     response  = requests.get(url, headers=headers, params=params)
-    resp_dict = response.json()
 
     match (response.status_code):
         case 200:
-            json_dados = resp_dict.get('dados')
+            json_dados = response.json().get('dados')
             nfses      = [NotaFiscalServico.from_json(**d) for d in json_dados['itens']]
-            return (resp_dict, nfses)
+            return (response, nfses)
     
-    return (resp_dict, None)
+    return (response, None)
 
 def retransmitir(token_emissor: str, 
                  token_secret_emissor: str,
                  token_empresa:str, 
                  token_secret_empresa:str, 
                  *args, **kwargs):
     raise NotImplementedError
```

### Comparing `pysisnoapi-0.1.0/README.md` & `pysisnoapi-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 
 ## Instalação
 Para instalar a biblioteca pySisnoAPI, execute o seguinte comando:
 ```
 pip install pysisnoapi
 ```
 
-**OBS: Ainda não está disponível para instalação via pip**
-
 ## Contribuição
 Contribuições são bem-vindas! Se você deseja contribuir para o projeto, siga as etapas abaixo:
 
 - Faça um fork do repositório.
 - Crie uma branch para a sua feature (`git checkout -b minha-feature`).
 - Implemente suas alterações.
 - Execute os testes unitários (`python -m unittest discover`).
```

### Comparing `pysisnoapi-0.1.0/PKG-INFO` & `pysisnoapi-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysisnoapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Vinícius Costa
 Author-email: viniciusccosta95@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -37,16 +37,14 @@
 
 ## Instalação
 Para instalar a biblioteca pySisnoAPI, execute o seguinte comando:
 ```
 pip install pysisnoapi
 ```
 
-**OBS: Ainda não está disponível para instalação via pip**
-
 ## Contribuição
 Contribuições são bem-vindas! Se você deseja contribuir para o projeto, siga as etapas abaixo:
 
 - Faça um fork do repositório.
 - Crie uma branch para a sua feature (`git checkout -b minha-feature`).
 - Implemente suas alterações.
 - Execute os testes unitários (`python -m unittest discover`).
```

