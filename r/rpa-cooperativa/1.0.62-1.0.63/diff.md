# Comparing `tmp/rpa_cooperativa-1.0.62.tar.gz` & `tmp/rpa_cooperativa-1.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.62.tar", last modified: Thu Jul  6 13:15:42 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.63.tar", last modified: Thu Jul 13 17:08:14 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.62.tar` & `rpa_cooperativa-1.0.63.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 13:15:42.639542 rpa_cooperativa-1.0.62/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.62/LICENSE
--rw-rw-rw-   0        0        0     6875 2023-07-06 13:15:42.635527 rpa_cooperativa-1.0.62/PKG-INFO
--rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.62/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 13:15:42.471167 rpa_cooperativa-1.0.62/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.62/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:15:42.572157 rpa_cooperativa-1.0.62/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.62/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.62/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.62/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.62/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.62/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.62/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.62/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.62/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.62/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.62/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.62/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    88577 2023-07-06 13:14:19.000000 rpa_cooperativa-1.0.62/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:15:42.628399 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6875 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      581 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 13:15:42.642206 rpa_cooperativa-1.0.62/setup.cfg
--rw-rw-rw-   0        0        0     2350 2023-07-06 13:15:20.000000 rpa_cooperativa-1.0.62/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:08:14.671725 rpa_cooperativa-1.0.63/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.63/LICENSE
+-rw-rw-rw-   0        0        0     6969 2023-07-13 17:08:14.668413 rpa_cooperativa-1.0.63/PKG-INFO
+-rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.63/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 17:08:14.445498 rpa_cooperativa-1.0.63/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.63/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:08:14.626747 rpa_cooperativa-1.0.63/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.63/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.63/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.63/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.63/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.63/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.63/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.63/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.63/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.63/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.63/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.63/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    91196 2023-07-13 17:04:43.000000 rpa_cooperativa-1.0.63/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:08:14.663415 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6969 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      581 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 17:08:14.672725 rpa_cooperativa-1.0.63/setup.cfg
+-rw-rw-rw-   0        0        0     2350 2023-07-13 16:50:58.000000 rpa_cooperativa-1.0.63/setup.py
```

### Comparing `rpa_cooperativa-1.0.62/LICENSE` & `rpa_cooperativa-1.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.62/PKG-INFO` & `rpa_cooperativa-1.0.63/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.62
+Version: 1.0.63
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -24,14 +24,15 @@
 License-File: LICENSE
 
 # Exemplos de utilizacao da bilioteca rpa_coop
 
 ```python
 # linha1: update pip 
 # linha2: install lib rpa-cooperativa via pip
+python -m pip config set global.trusted-host=pypi.org files.pythonhosted.org pypi.python.org
 python -m pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org --upgrade pip
 pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org pip rpa-cooperativa
 ```
 
 ```python
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
```

### Comparing `rpa_cooperativa-1.0.62/README.md` & `rpa_cooperativa-1.0.63/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Exemplos de utilizacao da bilioteca rpa_coop
 
 ```python
 # linha1: update pip 
 # linha2: install lib rpa-cooperativa via pip
+python -m pip config set global.trusted-host=pypi.org files.pythonhosted.org pypi.python.org
 python -m pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org --upgrade pip
 pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org pip rpa-cooperativa
 ```
 
 ```python
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
```

### Comparing `rpa_cooperativa-1.0.62/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.63/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.62/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.63/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.62/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.63/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.62/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.63/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.62/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.63/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.62/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.63/rpa_coop/rpa_coop.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,20 +88,21 @@
         result = f'{select_atributo} : {valor}'
         if print_atributo: print(result)
         if retorna_atributo: return valor
         return credenciais
 
 
 class Adobe:
+    # https://secure.na1.adobesign.com/public/docs/restapi/v6#://
     def __init__(self):
         self.token_api_adobe = str(gerador_pwd('api_adobe', 'senha'))
         self.url_api_adobe = str(gerador_pwd('api_adobe', 'ip_host'))
         
         
-    def alterar_status_usuario(self, email_usuario:str, status_usuario:str):
+    def alterar_status_usuario(self, email_usuario: str, status_usuario: str = 'INACTIVE'):
         '''status_usuario: ACTIVE, INACTIVE'''
         token_get_user = self.token_api_adobe
         url = f'{self.url_api_adobe}users'
         headers = { "Authorization": f"{token_get_user}"}
         response = requests.get(url, headers=headers)
         df = pd.DataFrame(response.json()['userInfoList'])
         for x in df.itertuples():
@@ -113,14 +114,65 @@
 
         if id_usuario == 'Não encontrado': raise Exception('Usuário não encontrado')
         url = f'{self.url_api_adobe}users/{id_usuario}/state'
         headers = { "Authorization": f"{token_get_user}"}
         body = {"state": f"{status_usuario}", "comment": "desativado por rpa"}
         response = requests.put(url, headers=headers, json=body)
         return response
+    
+    
+    def criar_usuario_adobe(self, email: str, nome_completo: str, cod_agencia: str, user_admin = False, status = 'ACTIVE', company = 'SICREDI', accountType = 'ENTERPRISE'):  
+        '''criar_usuario_adobe(email, nome_completo, cod_agencia)'''
+        groupName = '0718_' + cod_agencia  
+        id_adobe = str(email.split('@')[0])
+        primeiro_nome = str(nome_completo.split(' ')[0]) 
+        try:    ultimo_nome = str(nome_completo.split(' ')[1]) + ' ' + str(nome_completo.split(' ')[2])
+        except: ultimo_nome = str(nome_completo.split(' ')[1])
+        
+        hoje = datetime.now().strftime('%d-%m-%Y')
+        h = { "Authorization": f"{self.token_api_adobe}"}
+        
+        url = f'{self.url_api_adobe}groups'
+        res1 = requests.get(url, headers=h) # get grupos
+        r1 = res1.status_code
+        
+        if r1 == 200:
+            df = pd.DataFrame(res1.json()['groupInfoList'])
+            df = df[df['groupName'] == groupName]
+            id_grupo = str(df['groupId'].values[0])
+            
+            url = f'{self.url_api_adobe}users'    
+            body = { 
+                    "accountType": accountType,
+                    "email": email,
+                    "id": id_adobe,
+                    "isAccountAdmin": user_admin,
+                    "status": status,
+                    "company": company,
+                    "createdDate": hoje,
+                    "firstName": primeiro_nome,
+                    "lastName": ultimo_nome,
+                    "locale": "BR",
+                    "primaryGroupId": id_grupo,
+                    }
+
+            res2 = requests.post(url, headers=h, json=body)
+            r2 = res2.status_code
+            if r2 == 201:  
+                print('USUARIO ADOBE CRIADO COM SUCESSO')
+                print(res2.text)
+            elif r2 == 409:
+                print('OPS. O USUARIO ADOBE COM O EMAIL ESPECIFICADO JA EXISTE')
+            else:
+                print('ERRO AO TENTAR CRIAR USUARIO ADOBE VIA API')
+                print(res2.text)
+                raise Exception('Erro ao tentar criar usuario via api da adobe')
+            return res2.status_code
+        else:
+            raise Exception('Erro ao consultar a api da adobe, para pegar grupos de usuarios')
         
                 
 class Dados:
     
     def __init__(self):
         self.ip_planning = str(os.getenv('ip_planning'))
         self.user_planning = str(os.getenv('user_planning'))
@@ -933,15 +985,15 @@
         url = f'{self.url_api_whats}/optin/55{celular}'
         headers = {"Content-Type": "application/json; API Key","x-api-key": self.token_api_whats}
         response = requests.get(url, headers=headers)
         cod_response  = response.status_code
         return cod_response
 
 
-    def enviar_texto_whatsapp(self, celular: str, sistema_envio: str, texto:str):    
+    def enviar_texto_whatsapp(self, celular: str, sistema_envio: str, texto:str, template):    
         url = f'{self.url_api_whats}/notification'
         headers = {"Content-Type": "application/json; API Key", "x-api-key": self.token_api_whats}
         body = {
             "customerCoopCode": self.cod_coop,
             "customerBranchNum": "01",
             "customerPhoneNum": "55" + celular,
             "templateName": self.template_informa_novo,
@@ -1288,49 +1340,53 @@
         self.janela_sacg = janela
         self.janela_siat = janela
         self.janela_siac = janela
         
         opcoes = [x.upper() for x in opcoes]
         
         for menu in opcoes:
+            time.sleep(2)
             janela.activate()
             self.p.press('pgdn')
             time.sleep(1)
             
             if menu == 'SACG':
                 # Abrir SACG
                 try:
-                    posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, grayscale=True)
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, minSearchTime=2.0)
                 except:
-                    posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png', confidence=0.9, grayscale=True)
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png', confidence=0.9, minSearchTime=2.0)
+                print('posicao do click sacg', posicao)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_sacg = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
                 self.janelas.append(self.janela_sacg)
                 print('clicou no menu: sacg')
                 time.sleep(3)
                 # self.janela_sacg.activate()
             elif menu == 'SIAT':
                 # Abrir SIAT
                 try:
-                    posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png', confidence=0.9, grayscale=True)
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png', confidence=0.9, minSearchTime=2.0)
                 except:
-                    posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png', confidence=0.9, grayscale=True)
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png', confidence=0.9, minSearchTime=2.0)
+                print('posicao do click siat', posicao)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_siat = self.p.getWindowsWithTitle('teoff-exe')[num_menu] 
                 self.janelas.append(self.janela_siat)
                 print('clicou no menu: siat')
                 time.sleep(3)
                 # self.janela_siat.activate()
             elif menu == 'SIAC':
                 try:
-                    posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png', confidence=0.9, grayscale=True)
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png', confidence=0.9, minSearchTime=2.0)
                 except:
-                    posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png', confidence=0.9, grayscale=True)
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png', confidence=0.9, minSearchTime=2.0)
+                print('posicao do click siac', posicao)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_siac = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
                 self.janelas.append(self.janela_siac)
                 print('clicou no menu: siac')
                 time.sleep(3)
                 # self.janela_siac.activate()
```

### Comparing `rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.62
+Version: 1.0.63
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -24,14 +24,15 @@
 License-File: LICENSE
 
 # Exemplos de utilizacao da bilioteca rpa_coop
 
 ```python
 # linha1: update pip 
 # linha2: install lib rpa-cooperativa via pip
+python -m pip config set global.trusted-host=pypi.org files.pythonhosted.org pypi.python.org
 python -m pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org --upgrade pip
 pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org pip rpa-cooperativa
 ```
 
 ```python
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
```

### Comparing `rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 xlsxwriter
 xlrd
 openpyxl
 selenium==4.9.1
 webdriver_manager
 easygui
 pyperclip
-mysql-connector-python==8.0.28
+mysql-connector-python>=8.0.28
 pymysql
 pyodbc
 sqlalchemy==1.4.37
 psycopg2
 psycopg2-binary
 denodo-sqlalchemy
 pymssql
```

### Comparing `rpa_cooperativa-1.0.62/setup.py` & `rpa_cooperativa-1.0.63/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.62",
+    version="1.0.63",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
@@ -33,14 +33,14 @@
         "Intended Audience :: Developers",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
     python_requires='>=3.8',
-    install_requires=['wheel', 'pandas<=2.0.1', 'openpyxl', 'cryptography', 'xlsxwriter', 'xlrd', 'openpyxl','selenium==4.9.1', 'webdriver_manager', 'easygui', 'pyperclip', 'mysql-connector-python==8.0.28',
+    install_requires=['wheel', 'pandas<=2.0.1', 'openpyxl', 'cryptography', 'xlsxwriter', 'xlrd', 'openpyxl','selenium==4.9.1', 'webdriver_manager', 'easygui', 'pyperclip', 'mysql-connector-python>=8.0.28',
                       'pymysql', 'pyodbc', 'sqlalchemy==1.4.37', 'psycopg2', 'psycopg2-binary', 'denodo-sqlalchemy', 'pymssql', 'pillow', 'requests>=2.28.1', 'urllib3>=1.26.9', 
                       'certifi>=2022.5.18.1', 'pyopenssl>=22.0.0', 'idna>=3.3', 'charset-normalizer>=2.0.12', 'pyautogui',
                       'pyrect', 'pyscreeze', 'pytz', 'graypy', 'reportlab', 'psutil', 'requests-html', 'paramiko','opencv-python',
                       'pytesseract', 'xmltodict', 'pywin32', 'pywinauto', 'beautifulsoup4', 'mechanize', 'matplotlib', 
                       'Unidecode', 'WMI', 'tabulate', 'python-dateutil>=2.8.2', 'secure-smtplib']
 )
```

