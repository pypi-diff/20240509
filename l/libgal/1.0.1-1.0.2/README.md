# Comparing `tmp/libgal-1.0.1.tar.gz` & `tmp/libgal-1.0.2.tar.gz`

## Comparing `libgal-1.0.1.tar` & `libgal-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,39 @@
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 libgal-1.0.1/docs/FSUtils.md
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 libgal-1.0.1/docs/Installation.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 libgal-1.0.1/docs/SQLMemory.md
--rw-r--r--   0        0        0    12917 2020-02-02 00:00:00.000000 libgal-1.0.1/docs/Teradata.md
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/DatabaseAPI.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/FSUtils.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/Logger.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/MLS.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/ODBCTools.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/SQLAlchemy.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/SQLMemory.py
--rw-r--r--   0        0        0    10366 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/Sqlite.py
--rw-r--r--   0        0        0    20174 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/Teradata.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/Utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-1.0.1/libgal/modules/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/CSVFileLoggerTests.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/FileLoggerTests.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/JSONFileLoggerTests.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/LoggerTests.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/SQLAlchemy_test.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/SQliteTests.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/TeradataMLTests.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/Teradata_Basic_Test.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/TestEvaluateKsAndRocAuc.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/TestNumNormTransformer.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/TestsUtils.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 libgal-1.0.1/tests/test_dataframe.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 libgal-1.0.1/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0    19075 2020-02-02 00:00:00.000000 libgal-1.0.1/README.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 libgal-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    20705 2020-02-02 00:00:00.000000 libgal-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/FSUtils.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/HTMLParser.md
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Installation.md
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/LoadEnv.md
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Logger.md
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/SQLAlchemy.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/SQLMemory.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Selenium.md
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/SimpleTeradata.md
+-rw-r--r--   0        0        0    13840 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Teradata.md
+-rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Utils.md
+-rw-r--r--   0        0        0    15306 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/by_example/TeradataExamples.md
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/DatabaseAPI.py
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/FSUtils.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/Logger.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/MLS.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/ODBCTools.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/SQLAlchemy.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/SQLMemory.py
+-rw-r--r--   0        0        0    10366 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/Sqlite.py
+-rw-r--r--   0        0        0    21087 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/Teradata.py
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/Utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/CSVFileLoggerTests.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/FileLoggerTests.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/JSONFileLoggerTests.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/LoggerTests.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/SQLAlchemyTests.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/SQliteTests.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/TeradataBasicTest.py
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/TeradataMLTests.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/TestEvaluateKsAndRocAuc.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/TestNumNormTransformer.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 libgal-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 libgal-1.0.2/README.md
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 libgal-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 libgal-1.0.2/PKG-INFO
```

### Comparing `libgal-1.0.1/docs/FSUtils.md` & `libgal-1.0.2/docs/FSUtils.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ## Utilidades para el manejo de archivos y directorios.
 Permite la creación de directorios, eliminar archivos antiguos, cambiar permisos e iniciar el entorno del proyecto.
 
+[Volver al readme principal](../README.md)
+
 **Nota:** todas las operaciones se realizan en el directorio de trabajo actual.
 Para cambiar el directorio de trabajo actual al raíz del proyecto se debe invocar 
 ```python
 import os
 os.chdir(os.path.dirname(os.path.realpath(__file__)))
 ```
 Al principio del script principal (ejecutar.py o main.py)
```

### Comparing `libgal-1.0.1/docs/Installation.md` & `libgal-1.0.2/docs/Installation.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ## Instrucciones de instalación
 
+[Volver al readme principal](../README.md)
+
 ### Requisitos previos
 
 - [Python](https://www.python.org/downloads/) 3.7 o versión superior
 - git [Git-SCM](https://git-scm.com/)
 - IDE [PyCharm Community Edition](https://www.jetbrains.com/pycharm/download/), [VSCode](https://code.visualstudio.com/) o su favorito con soporte para debug de Python (para desarrollo, no necesario para ejecución) 
 - virtualenv (opcional)
```

### Comparing `libgal-1.0.1/docs/SQLMemory.md` & `libgal-1.0.2/docs/SQLMemory.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SQLMemory
 
 ## Interfaz simplificada para la carga de Dataframes a SQL en memoria
 
 ### Descripción
 La clase SQLMemory permite cargar Dataframes a SQL en memoria y hacer consultas sobre ellos.
 
+[Volver al readme principal](../README.md)
+
 ### Importar la librería
 ```python
 from libgal.modules.SQLMemory import SQLMemory
 ```
 
 ### Crear una instancia
 ```python
```

### Comparing `libgal-1.0.1/docs/Teradata.md` & `libgal-1.0.2/docs/Teradata.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 
 ### Descripción
 Libgal define una interfaz simplificada para la carga de DataFrames a Teradata.
 
 La carga se realiza por Fastload cuando la cantidad de registros es mayor a 10000, y por ODBC cuando es menor o igual a 10000.  
 El parámetro de corte para utilizar un método u otro se puede modificar con el parámetro odbc_limit.
 
+Para ver ejemplos de uso, ver la sección de [Ejemplos](by_example/TeradataExamples.md).
+
+[Volver al readme principal](../README.md)
+
 ## Importar la librería
+
 ```python
-from libgal.modules.Teradata import Teradata
+from libgal.modules.Teradata import TeradataML
 ```
 ---
 
-**Índice**
+## Índice
 - [Conectarse al motor de base de datos y mantener la conexión abierta.](#teradatahost-str-user-str-passw-str-logmech-str--ldap-schema-str--none)
 - [Ejecutar sentencias que no retornan datos (ej: create table, drop table, insert, update, delete, etc).](#doquery-str--executequery-str)
 - [Ejecutar queries que retornan datos (ej: select) y devolver el resultado en un dataframe.](#queryquery-str-mode-str--normal---dataframe)
 - [Truncar una tabla.](#truncate_tableschema-str-table-str)
 - [Borrar una tabla.](#drop_tableschema-str-table-str)
 - [Borrar una tabla si existe.](#drop_table_if_existsschema-str-table-str)
 - [Obtener la lista de nombres de columnas de una tabla.](#table_columnsschema-str-table-str---liststr)
@@ -46,15 +51,15 @@
 - passw: Contraseña
 - logmech (opcional): Mecanismo de autenticación
 - schema (opcional): Schema por defecto
 - return: Objeto Teradata
 
 **Ejemplo:**
 ```python
-td = Teradata(host='nombre_host', user='usuario', passw='contraseña')
+td = TeradataML(host='nombre_host', user='usuario', passw='contraseña')
 ```
 
 Si se va a usar TD2 para la autenticación, se debe especificar el parámetro logmech='TD2'.  
 En caso contrario, se puede omitir el parámetro logmech y por defecto será 'LDAP'.  
 Opcionalmente se puede especificar el schema por defecto con el parámetro schema. 
 
 ---
@@ -66,26 +71,30 @@
 - db: Nombre de la base de datos
 
 **Ejemplo:** 
 ```python
 td.use_db('nombre_base_datos')
 ```
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### do(query: str) / execute(query: str)
 Ejecuta una sentencia sin retorno de datos. 
 
 Argumentos:
 - query: Query a ejecutar
 
 **Ejemplo:**
 ```python
 td.do('CREATE TABLE tabla (campo1 INT, campo2 VARCHAR(10))')
 ```
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### query(query: str, mode: str = 'normal') -> DataFrame 
 Ejecuta una query que devuelve un dataframe  
 
 Argumentos:
 - query: Query a ejecutar
 - mode (opcional): Modo de ejecución, puede ser 'normal' o 'legacy'
@@ -95,28 +104,31 @@
 ```python
 df = td.query('SELECT TOP 100 * FROM tabla')
 ```
 Si se especifica el parámetro mode='legacy', utiliza el driver ODBC en vez de el engine de SQLAlchemy.  
 Esto puede ser útil para ejecutar queries que no son soportadas por el engine de SQLAlchemy.  
 Por lo general no es necesario especificar el modo.  
 
+[Volver al inicio del documento](#Índice)
 
 ---
 ### current_date() 
 
 Obtiene la fecha desde el servidor
 
 Devuelve:  
 return: datetime.date
 
 **Ejemplo:**
 ```python
 current_date = td.current_date()
 ```
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### show_tables(db: str, prefix: str) -> DataFrame
 
 Obtiene una lista de tablas de una base de datos que coinciden con prefijo + nombre_tabla
 
 Argumentos:
 - db: Base de datos
@@ -124,14 +136,16 @@
 - return: DataFrame con las tablas cuyo nombre empieza con el prefijo indicado
 
 **Ejemplo:**
 ```python
 tablas_df = td.show_tables(db='nombre_base_datos', prefix='prefijo_tabla')
 ```
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### drop_table(schema: str, table: str)
 
 Elimina una tabla
 
 Argumentos:
 - schema: Schema de la tabla
@@ -140,14 +154,16 @@
 **Ejemplo:**
 ```python
 td.drop_table(schema='nombre_schema', table='nombre_tabla')
 ```
 Ejecuta DROP TABLE nombre_schema.nombre_tabla;  
 Si la tabla no existe, se produce una excepción teradatasql.OperationalError.  
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### drop_table_if_exists(schema: str, table: str) 
 
 Borra una tabla si existe.  
 
 Argumentos:
 - schema: Schema de la tabla
@@ -155,14 +171,16 @@
 
 **Ejemplo:**
 ```python
 td.drop_table_if_exists(schema='nombre_schema', table='nombre_tabla')
 ```
 En el caso de que la tabla no exista, no se produce ningún error.
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### truncate_table(schema: str, table: str)
 
 Trunca una tabla (borra todos los registros pero no la estructura).  
 
 Argumentos:
 - schema: Schema de la tabla
@@ -170,27 +188,31 @@
 
 **Ejemplo:**
 ```python
 td.truncate_table(schema='nombre_schema', table='nombre_tabla')
 ```
 Ejecuta DELETE FROM nombre_schema.nombre_tabla ALL;
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### table_columns(schema: str, table: str) -> List[str]  
 Devuelve una lista con los nombres de las columnas de una tabla.  
 
 Argumentos:
 - schema: Schema de la tabla
 - table: Nombre de la tabla
 
 **Ejemplo:**
 ```python
 columnas = td.table_columns(schema='nombre_schema', table='nombre_tabla')
 ```
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### create_table_like(schema: str, table: str, schema_orig: str, table_orig: str) 
 Crea una tabla que es copia de la estructura de otra
 
 Argumentos:
 - schema: Schema de la tabla a crear
 - table: Nombre de la tabla a crear
@@ -199,14 +221,16 @@
 
 **Ejemplo:**
 ```python
 td.create_table_like(schema='nombre_schema', table='nombre_tabla', schema_orig='nombre_schema_orig', table_orig='nombre_tabla_orig')
 ```
 Crea la tabla nombre_schema.nombre_tabla con la misma estructura que nombre_schema_orig.nombre_tabla_orig. 
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### insert(df: DataFrame, schema: str, table: str, pk: str, use_odbc: bool = True, odbc_limit: int = 10000)
 Inserta un dataframe en una tabla.  
 
 Argumentos:
 - df: DataFrame a insertar
 - schema: Schema de la tabla
@@ -220,14 +244,16 @@
 td.insert(df=df, schema='nombre_schema', table='nombre_tabla', pk='nombre_pk')
 ``` 
 Inserta el dataframe df en la tabla nombre_schema.nombre_tabla.  
 Si los registros existen, se produce una excepción teradatasql.IntegrityError.  
 Al insertar menos de 10000 registros, se utiliza el driver ODBC, caso contrario se utiliza fastload.  
 El límite de 10000 registros se puede modificar con el parámetro odbc_limit, y si se especifica use_odbc=False, se fuerza el uso de fastload. 
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### upsert(df: DataFrame, schema: str, table: str, pk: str, use_odbc: bool = True, odbc_limit: int = 10000, parser_limit: int = 10000)
 
 Actualiza un dataframe en una tabla forzado (insert overwrite/upsert)
 
 Argumentos:
 - df: DataFrame a insertar
@@ -244,14 +270,16 @@
 ```python
 td.upsert(df=df, schema='nombre_schema', table='nombre_tabla', pk='nombre_pk')
 ```
 La actualización se realiza borrando los registros existentes y volviendo a insertarlos.  
 El parámetro parser_limit se utiliza para dividir la cantidad de pks en grupos de tamaño parser_limit, y así evitar errores de parser al ejecutar el delete.  
 Por lo general no es necesario modificar el parámetro parser_limit, pero si existen excepciones de parser, se puede probar con un valor mas bajo.
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### fastload(df: DataFrame, schema: str, table: str, pk: str, index: bool = False)
 
 Fastload de un dataframe a una tabla.
 
 Argumentos:
 - df: DataFrame a insertar
@@ -264,14 +292,16 @@
 ```python
 td.fastload(df=df, schema='nombre_schema', table='nombre_tabla', pk='nombre_pk')
 ```
 
 Inserta el dataframe df en la tabla nombre_schema.nombre_tabla utilizando fastload.  
 Si los registros existen, se produce una excepción teradatasql.IntegrityError.
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### retry_fastload(df: DataFrame, schema: str, table: str, pk: str, retries: int = 30, retry_sleep: int = 20)
 
 Fastload con reintentos.  
 
 Argumentos:
 - df: DataFrame a insertar
@@ -286,14 +316,16 @@
 Por defecto se realizan 30 reintentos con un tiempo de espera de 20 segundos entre reintentos.
 
 **Ejemplo:**
 ```python
 td.retry_fastload(df=df, schema='nombre_schema', table='nombre_tabla', pk='nombre_pk')
 ```
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### diff(schema_src: str, table_src: str, schema_dst: str, table_dst: str) -> DataFrame
 
 Devuelve un DataFrame con las diferencias entre dos tablas
 
 Argumentos:
 - schema_src: Schema de la tabla origen
@@ -306,14 +338,16 @@
 ```python
 df_diff = td.diff(schema_src='nombre_schema_src', table_src='nombre_tabla_src', schema_dst='nombre_schema_dst', table_dst='nombre_tabla_dst')
 ```  
 Ejecuta SELECT * FROM nombre_schema_src.nombre_tabla_src MINUS SELECT * FROM nombre_schema_dst.nombre_tabla_dst; y devuelve el resultado en un dataframe.  
 Este método se utiliza para la carga incremental de tablas que no tienen un primary key.  
 Es recomendable de todas formas, que las tablas que vayan a realizar cargas incrementales tengan un primary key.  
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### staging_insert(df: DataFrame, schema_stg: str, table_stg: str, schema_dst: str, table_dst: str, pk: str)
 
 Realiza una carga incremental de un dataframe a una tabla.  
 Primero se sube el lote a cargar a una tabla staging, y luego se realiza un insert desde ese staging a la tabla destino de todos los registros que no existen en la tabla destino.
 
 Argumentos:
@@ -325,18 +359,22 @@
 - pk: Primary key de la tabla
 
 **Ejemplo:**
 ```python
 td.staging_insert(df=df, schema_stg='nombre_schema_stg', table_stg='nombre_tabla_stg', schema_dst='nombre_schema_dst', table_dst='nombre_tabla_dst', pk='nombre_pk')
 ```
 
+[Volver al inicio del documento](#Índice)
+
 ---
 ### staging_upsert(df: DataFrame, schema_stg: str, table_stg: str, schema_dst: str, table_dst: str, pk: str, parser_limit: int = 10000):
 
 Hace un upsert incremental de un dataframe a una tabla.  
 La actualización se realiza borrando los registros existentes y volviendo a insertarlos al igual que en el método upsert.    
 El parámetro parser_limit se utiliza de la misma forma que en el método upsert.
 
 **Ejemplo:**
 ```python
 td.staging_upsert(df=df, schema_stg='nombre_schema_stg', table_stg='nombre_tabla_stg', schema_dst='nombre_schema_dst', table_dst='nombre_tabla_dst', pk='nombre_pk')
 ```
+
+[Volver al inicio del documento](#Índice)
```

### Comparing `libgal-1.0.1/libgal/__init__.py` & `libgal-1.0.2/libgal/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 try:
 
     import logging  # Libreria para logs
     import os
     from pathlib import Path
+    import time
 
     # Selenium
     from selenium import webdriver
     from selenium.webdriver.firefox.service import Service
     from selenium.webdriver.common.by import By
     from selenium.webdriver.support.select import Select
 
@@ -58,43 +59,44 @@
     """
     Descripción: Toma las variables de entorno del archivo .env o del SO
     Parámetro:
     - path_env_file (String):
     """
 
     if path_env_file != None and Path(path_env_file).exists():
-
         load_dotenv(path_env_file)
-
     else:
-
-        print(
-            f"No se encontró el archivo {path_env_file} indicado para funcion variables_entorno() de libgal por lo que se toma las variables de entorno de sistema.")
+        from libgal.modules.Logger import Logger
+        logger = Logger().get_logger()
+        logger.warning(
+            f"No se encontró el archivo {path_env_file} indicado para funcion variables_entorno() de libgal por lo "
+            f"que se toma las variables de entorno de sistema."
+        )
 
     return dict(os.environ)
 
 
 class LoggerFormatException(Exception):
     pass
 
 
-def logger(format_output="JSON", app_name=__name__):
+def logger(format_output="JSON", app_name=__name__, dir_name=None):
     """
     Descripción: Crea un nuevo logger
     Parámetro:
     - format_output (String): Tipo de Salida del Log (JSON, CSV)
     - app_name (String): Nombre de la aplicación para el log
     """
     from libgal.modules.Logger import Logger
 
     if format_output not in ['CSV', 'JSON']:
         raise LoggerFormatException("Tipo de formato de Log inválido. Formatos soportados (JSON y CSV).")
 
     # Create a custom logger
-    _logger = Logger(format_output=format_output, app_name=app_name, dirname=None)
+    _logger = Logger(format_output=format_output, app_name=app_name, dirname=str(dir_name))
     _logger.set_format(format_output)
     _logger.get_logger().setLevel(logging.INFO)
 
     return _logger.get_logger()
 
 
 def shutdown_logger():
```

### Comparing `libgal-1.0.1/libgal/modules/DatabaseAPI.py` & `libgal-1.0.2/libgal/modules/DatabaseAPI.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/libgal/modules/FSUtils.py` & `libgal-1.0.2/libgal/modules/FSUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from os import listdir, stat, remove, chdir
 from os.path import isfile, join, dirname
 from pathlib import Path
 from time import time
 
 from libgal.modules.Logger import Logger
 
@@ -98,12 +99,13 @@
 
 
 def init_env(home):
     """
     Inicializa el entorno de ejecución
         :param home: Directorio raíz
     """
+    os.chdir(home)
     create_output_dirs(home)
     for dir_ in OUTPUT_DIRS:
         delete_older_files(dir_, max_days=90)
     change_to_public_permissions('logs')
     delete_files(Path('output'))
```

### Comparing `libgal-1.0.1/libgal/modules/Logger.py` & `libgal-1.0.2/libgal/modules/Logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,17 @@
             dirname: Optional[str] = None,
             level: Optional[int] = logging.DEBUG
     ):
         self._logger = logging.getLogger(app_name)
 
         self._logger.setLevel(level)
         self._id = id(self)
+        self._app_name=app_name
 
-        formatter = self.set_format(format_output)
-
-        streamHandler = logging.StreamHandler()
-        streamHandler.setFormatter(formatter)
-        self._logger.addHandler(streamHandler)
+        self.set_format(format_output)
 
         if dirname is not None:
             self.set_outputdir(dirname, format_output)
 
         self._logger.info(f"Generate new instance, hash = {self._id}")
 
     def __del__(self):
@@ -107,32 +104,40 @@
             )
         else:
             formatter = logging.Formatter(
                 f'%(asctime)s PID: %(process)d ({self._id}) %(threadName)s [%(levelname)s | %(filename)s:%(lineno)s] '
                 f'> %(message)s '
             )
 
+        found_stream_handler = False
         for handler in self._logger.handlers:
+            if isinstance(handler, logging.StreamHandler):
+                found_stream_handler = True
             handler.setFormatter(formatter)
 
+        if not found_stream_handler:
+            streamHandler = logging.StreamHandler()
+            streamHandler.setFormatter(formatter)
+            self._logger.addHandler(streamHandler)
+
         return formatter
 
     def set_outputdir(self, dirname: Optional[str], log_format: Optional[str] = None):
         if dirname is not None:
             if not os.path.isdir(dirname):
                 os.mkdir(dirname)
             formatter = self.set_format(log_format)
             now = datetime.datetime.now()
             for handler in self._logger.handlers:
                 if isinstance(handler, BufferingHandler):
                     handler.close()
                     self._logger.removeHandler(handler)
 
             file_handler = BufferingHandler(
-                dirname + "/log_" + now.strftime("%Y-%m-%d") + ".log", encoding='utf-8')
+                dirname + f"/{self._app_name}_{os.getpid()}_" + now.strftime("%Y-%m-%d") + ".log", encoding='utf-8')
             file_handler.setFormatter(formatter)
             self._logger.addHandler(file_handler)
         else:
             self._logger.warning("No se ha especificado un directorio de salida para los logs")
 
 
 # a simple usecase
```

### Comparing `libgal-1.0.1/libgal/modules/MLS.py` & `libgal-1.0.2/libgal/modules/MLS.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/libgal/modules/ODBCTools.py` & `libgal-1.0.2/libgal/modules/ODBCTools.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/libgal/modules/SQLMemory.py` & `libgal-1.0.2/libgal/modules/SQLMemory.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/libgal/modules/Sqlite.py` & `libgal-1.0.2/libgal/modules/Sqlite.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/libgal/modules/Teradata.py` & `libgal-1.0.2/libgal/modules/Teradata.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     - host (String): uri del servidor de base de datos
     - username (String): Usuario que autentica la conexión a la base de datos
     - password (String): Contraseña para la autenticación de la connexión de la base de datos
     - logmech (String): Parámetro Opcional que indica el método de autenticación del usuario. LDAP por defecto
     - database (String): Parámetro Opcional que indica la base de datos a la cual nos vamos a conectar
     """
     if database is not None:
-        td = Teradata(host=host, user=username, passw=password, logmech=logmech.upper(), schema=database)
+        td = TeradataML(host=host, user=username, passw=password, logmech=logmech.upper(), schema=database)
     else:
-        td = Teradata(host=host, user=username, passw=password, logmech=logmech.upper())
+        td = TeradataML(host=host, user=username, passw=password, logmech=logmech.upper())
 
     return td.connection
 
 
 class Scripting:
 
     def __init__(self):
@@ -143,15 +143,15 @@
                 statement = re.sub(r'VALUES \(.*\?.*\);', '', item['statement'])
                 str_arr.append(statement + 'VALUES (' + ', '.join(self._stringify(item['values'])) + ');')
             else:
                 str_arr.append(item['statement'])
         return str_arr
 
 
-class Teradata(DatabaseAPI):
+class TeradataML(DatabaseAPI):
 
     def __init__(self, host: str, user: str, passw: str,
                  logmech: Optional[str] = 'LDAP', schema: Optional[str] = 'DBC'):
         """
         Inicializa una conexión a Teradata
             :param host: Host de la base de datos
             :param user: Usuario
@@ -365,14 +365,21 @@
     @property
     def engine(self):
         """
         Devuelve el engine de SQLAlchemy
         """
         return self.eng
 
+    @property
+    def is_connected(self):
+        """
+        Devuelve si la conexión está activa
+        """
+        return self.conn is not None
+
     def tml_connect(self, host, user, passw, db, logmech=None):
         """
         Crea una conexión a TeradataML
             :param host: Host de la base de datos
             :param user: Usuario
             :param passw: Contraseña
             :param db: Base de datos
@@ -497,7 +504,25 @@
         query = f'INSERT INTO {schema_dst}.{table_dst} SELECT {", ".join(named_columns)} ' + \
             f'FROM {schema_stg}.{table_stg} stg ' + \
             f'LEFT JOIN {schema_dst}.{table_dst} prd ON prd.{pk} = stg.{pk} ' + \
             f'WHERE prd.{pk} IS NULL;'
 
         self.do(query)
         self.drop_table(schema_stg, table_stg)
+
+
+class Teradata(TeradataML):
+
+    def __init__(self, host: str, user: str, passw: str,
+                 logmech: Optional[str] = 'LDAP', schema: Optional[str] = 'DBC'):
+        """
+        Inicializa una conexión a Teradata
+            :param host: Host de la base de datos
+            :param user: Usuario
+            :param passw: Contraseña
+            :param logmech: Mecanismo de autenticación
+            :param schema: Schema por defecto
+        """
+        from libgal.modules.Logger import Logger
+        self._logger = Logger(dirname=None).get_logger()
+        self._logger.warning('FutureWarning: Teradata está deprecado, utilice TeradataML en su lugar')
+        super().__init__(host, user, passw, logmech, schema)
```

### Comparing `libgal-1.0.1/tests/FileLoggerTests.py` & `libgal-1.0.2/tests/FileLoggerTests.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/tests/LoggerTests.py` & `libgal-1.0.2/tests/LoggerTests.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/tests/SQLAlchemy_test.py` & `libgal-1.0.2/tests/SQLAlchemyTests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import unittest
 from time import time
 from sqlalchemy import Table, MetaData
 from sqlalchemy.ext.declarative import declarative_base
 import libgal
 from pandas import DataFrame
 from libgal.modules.Logger import Logger
-from TestsUtils import ask_user_pwd
-from test_dataframe import generate_dataframe
+from libgal.modules.Utils import generate_dataframe, ask_user_pwd
 
 
 logger = Logger().get_logger()
 
 
 # Defino clase de la tabla
 class ClaseTabla(declarative_base(metadata=MetaData())):
@@ -84,15 +83,15 @@
         # Crea la tabla desde el dataframe
         df_structure_only = test_df.drop(test_df.index)
         df_structure_only.to_sql(table_name, schema=table_schema, con=self.con.engine, if_exists='replace', index=False)
 
         # Inserta el dataframe
         t_start = time()
         logger.info(f'Insertando datos en tabla {table_schema}.{table_name}')
-        self.con.InsertDataframe(test_df, table_schema, table_name)
+        self.con.insert(test_df, table_schema, table_name)
         elapsed = time() - t_start
         logger.info(f'Tiempo de inserción: {elapsed: .2f} segundos')
 
         # Borra la tabla
         logger.info(f'Borrando tabla {table_schema}.{table_name}')
         self.con.query(f'DROP TABLE {table_schema}.{table_name}')
 
@@ -103,14 +102,13 @@
             session.add(nuevo_dato)
             session.commit()
             logger.error("Datos almacenados correctamente")
             assert False, "No se generó el error esperado"
 
         except libgal.SQLAlchemyError as e:
             session.rollback()
-            logger.info(e)
 
         session.close()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `libgal-1.0.1/tests/SQliteTests.py` & `libgal-1.0.2/tests/SQliteTests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from time import time
 from pandas import DataFrame
 from libgal.modules.Logger import Logger
-from test_dataframe import generate_dataframe
+from libgal.modules.Utils import generate_dataframe
 from libgal.modules.SQLMemory import SQLMemory
 import os
 
 logger = Logger().get_logger()
 
 DB_FILENAME = 'sqlite_test_staging.db'
 logger.info('Generando dataframe de prueba')
```

### Comparing `libgal-1.0.1/tests/TeradataMLTests.py` & `libgal-1.0.2/tests/TeradataMLTests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import unittest
 from time import time
 from pandas import DataFrame
-from test_dataframe import generate_dataframe
-from libgal.modules.Teradata import Teradata
+from libgal.modules.Teradata import TeradataML
 from libgal.modules.Logger import Logger
-from TestsUtils import ask_user_pwd
+from libgal.modules.Utils import ask_user_pwd, generate_dataframe
 
 logger = Logger().get_logger()
 
 host, usr, passw, logmech = ask_user_pwd()
 logger.info('Generando dataframe de prueba')
 test_df: DataFrame = generate_dataframe(num_rows=500000)
 logger.info('Realizando conexiones a la base de datos')
 t_st = time()
-teradata = Teradata(host=host, user=usr, passw=passw, logmech=logmech)
+teradata = TeradataML(host=host, user=usr, passw=passw, logmech=logmech)
 t_conn = time() - t_st
 logger.info('Conexión exitosa')
 logger.info(f'Tiempo de conexión: {round(t_conn, 2)} s')
 
 
 class TeradataTests(unittest.TestCase):
```

### Comparing `libgal-1.0.1/tests/Teradata_Basic_Test.py` & `libgal-1.0.2/tests/TeradataBasicTest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from libgal.modules.Logger import Logger
 from libgal import teradata, TeradataError
-from TestsUtils import ask_user_pwd
+from libgal.modules.Utils import ask_user_pwd
 
 logger = Logger().get_logger()
 
 
 host, usr, passw, logmech = ask_user_pwd()
 conexion = teradata(host=host, username=usr, password=passw, logmech=logmech)
```

### Comparing `libgal-1.0.1/tests/TestEvaluateKsAndRocAuc.py` & `libgal-1.0.2/tests/TestEvaluateKsAndRocAuc.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/tests/TestNumNormTransformer.py` & `libgal-1.0.2/tests/TestNumNormTransformer.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/LICENSE.txt` & `libgal-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libgal-1.0.1/pyproject.toml` & `libgal-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel.force-include]
 "libgal/modules" = "libgal/modules"
 
 [project]
 name = "libgal"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Jean Manuel González Mejía", email="ebrainding@gmail.com" },
   { name="Julián Leandro Giraldez", email="juliangiraldez@outlook.com"},
   { name="Sebastian Wilwerth", email="sebastian.wilwerth@gmail.com" }
 ]
 
 license = { file = "LICENSE.txt" }
```

