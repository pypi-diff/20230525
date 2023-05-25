# Comparing `tmp/elgin-0.1.3-py3-none-any.whl.zip` & `tmp/elgin-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,8 @@
-Zip file size: 7832 bytes, number of entries: 8
+Zip file size: 5391 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 23-May-24 18:41 elgin/__init__.py
--rw-r--r--  2.0 unx    12047 b- defN 23-May-25 15:38 elgin/monitoramento.py
--rw-r--r--  2.0 unx     3978 b- defN 23-May-24 18:09 elgin/templates/template_email_log.html
--rw-r--r--  2.0 unx     4019 b- defN 23-May-24 20:41 elgin/templates/template_teams.json
--rw-r--r--  2.0 unx     2430 b- defN 23-May-25 15:40 elgin-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 15:40 elgin-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-25 15:40 elgin-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      628 b- defN 23-May-25 15:40 elgin-0.1.3.dist-info/RECORD
-8 files, 23200 bytes uncompressed, 6736 bytes compressed:  71.0%
+-rw-r--r--  2.0 unx    12044 b- defN 23-May-25 15:44 elgin/monitoramento.py
+-rw-r--r--  2.0 unx     2430 b- defN 23-May-25 15:44 elgin-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 15:44 elgin-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-25 15:44 elgin-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      440 b- defN 23-May-25 15:44 elgin-0.1.4.dist-info/RECORD
+6 files, 15012 bytes uncompressed, 4595 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,25 +1,19 @@
 Filename: elgin/__init__.py
 Comment: 
 
 Filename: elgin/monitoramento.py
 Comment: 
 
-Filename: elgin/templates/template_email_log.html
+Filename: elgin-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: elgin/templates/template_teams.json
+Filename: elgin-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: elgin-0.1.3.dist-info/METADATA
+Filename: elgin-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: elgin-0.1.3.dist-info/WHEEL
-Comment: 
-
-Filename: elgin-0.1.3.dist-info/top_level.txt
-Comment: 
-
-Filename: elgin-0.1.3.dist-info/RECORD
+Filename: elgin-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elgin/monitoramento.py

```diff
@@ -248,15 +248,15 @@
                 "tipo_servico": self.__tipo_servico,
                 'data_ref': datetime.now(pytz.timezone('America/Sao_Paulo')).strftime('%d/%m/%Y %H:%M'),
                 "status": status,
                 "ambiente": self.__environment.upper(),
                 "exception": exception.replace('"',"'").replace('\n','')
             }
             
-            with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'templates','template_teams.json',encoding='utf-8')) as file:
+            with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'templates','template_teams.json'),encoding='utf-8') as file:
                 template_data = json.load(file)
             
             payload = json.dumps(template_data) % data
             headers = { 'Content-Type': 'application/json' }
             url = wr.secretsmanager.get_secret_json(f'{self.__environment}/teams/webhook', boto3_session=awsSession)['webhook_url']
 
             response = requests.post(url, data=payload, headers=headers)
@@ -280,15 +280,15 @@
             emailPort   = emailCredentials['port']  
             
             dtRef = datetime.now(pytz.timezone('America/Sao_Paulo')).strftime('%d/%m/%Y %H:%M')
             
             responsaveis = TbResponsaveis().filtrar(f"ambiente LIKE '%{self.__environment}%' AND recebe_alertas = True AND ativo = True").executar()
             receivers = [email['email'] for email in responsaveis]
 
-            with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'templates','template_email_log.html','r',encoding='utf-8')) as template:
+            with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'templates','template_email_log.html'), encoding='utf-8') as template:
 
                 html = template.read()
                 html = html.format( status=self.verifica_status(status=status)
                                    ,alerta=self.verifica_status(level=level)
                                    ,dtRef=dtRef
                                    ,nome_processo=self.__nome_processo.title()
                                    ,tipo_servico = self.__tipo_servico
```

## Comparing `elgin-0.1.3.dist-info/METADATA` & `elgin-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgin
-Version: 0.1.3
+Version: 0.1.4
 Summary: Biblioteca responsavel por gerar o monitoramento dos processos da empresa elgin.
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

