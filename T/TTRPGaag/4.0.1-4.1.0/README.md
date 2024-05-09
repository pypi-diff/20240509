# Comparing `tmp/ttrpgaag-4.0.1.tar.gz` & `tmp/ttrpgaag-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttrpgaag-4.0.1.tar", last modified: Wed May  8 12:01:18 2024, max compression
+gzip compressed data, was "ttrpgaag-4.1.0.tar", last modified: Thu May  9 14:13:48 2024, max compression
```

## Comparing `ttrpgaag-4.0.1.tar` & `ttrpgaag-4.1.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.933378 ttrpgaag-4.0.1/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1075 2023-10-09 18:00:41.000000 ttrpgaag-4.0.1/LICENSE
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       47 2023-10-09 18:12:41.000000 ttrpgaag-4.0.1/MANIFEST.in
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1643 2024-05-08 12:01:18.932798 ttrpgaag-4.0.1/PKG-INFO
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1416 2024-05-08 11:58:33.000000 ttrpgaag-4.0.1/README.md
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.902106 ttrpgaag-4.0.1/RPG/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      254 2024-05-08 11:47:32.000000 ttrpgaag-4.0.1/RPG/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6480 2024-04-22 12:53:12.000000 ttrpgaag-4.0.1/RPG/baralho.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.904765 ttrpgaag-4.0.1/RPG/dado/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       94 2023-10-11 14:22:30.000000 ttrpgaag-4.0.1/RPG/dado/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3357 2023-11-13 11:34:50.000000 ttrpgaag-4.0.1/RPG/dado/dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     2117 2024-04-22 12:53:12.000000 ttrpgaag-4.0.1/RPG/dado/dados.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.906172 ttrpgaag-4.0.1/RPG/dado/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-4.0.1/RPG/dado/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1512 2024-05-08 11:48:20.000000 ttrpgaag-4.0.1/RPG/dado/helpers/converter_notacao_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      295 2023-10-11 18:00:52.000000 ttrpgaag-4.0.1/RPG/dado/helpers/monta_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2024-05-08 11:47:32.000000 ttrpgaag-4.0.1/RPG/dado/rolar_dado_notacao.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      803 2024-04-22 12:53:12.000000 ttrpgaag-4.0.1/RPG/iniciativa.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.906667 ttrpgaag-4.0.1/RPG/sistemas/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.908083 ttrpgaag-4.0.1/RPG/sistemas/dnd/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       91 2023-09-14 17:58:19.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.909898 ttrpgaag-4.0.1/RPG/sistemas/dnd/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      245 2024-01-22 19:11:21.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/data/mecanicas.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     7566 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/data/tesouro.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.911645 ttrpgaag-4.0.1/RPG/sistemas/dnd/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      247 2023-10-11 18:00:52.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/helpers/calcular_mod_atributo.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      391 2024-05-08 11:50:32.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/helpers/checa_testes.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1044 2024-05-08 11:49:30.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/rola_tesouro.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     5269 2024-05-08 11:49:50.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/teste.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.914162 ttrpgaag-4.0.1/RPG/sistemas/pf2/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     8697 2024-04-22 12:53:12.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/PC.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      191 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6181 2024-05-08 11:52:38.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/calcula_dano.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.918656 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      494 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3279 2023-11-27 11:50:56.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/defesas_monstros.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      109 2023-11-27 11:50:56.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/proficiency.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       74 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/saves.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      405 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/skills.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      119 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/tipos_ataques.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      101 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/tipos_defesas.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.921198 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-12-01 15:28:03.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      280 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/atributo.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     5426 2024-05-08 11:52:54.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/base_calcula_dano.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      807 2024-05-08 11:53:30.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/proficiencias.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      855 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/proficiencia.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.922516 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       64 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1315 2024-05-08 11:53:48.000000 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/consulta_critico.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.923542 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)    28276 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/data/criticos.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.925725 ttrpgaag-4.0.1/RPG/tabela_rolavel/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       80 2024-04-23 17:09:37.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.928638 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 17:28:48.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1014 2024-05-08 11:47:32.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/ajeita_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      723 2024-05-08 11:54:25.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/ajusta_resultados.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      183 2023-09-11 16:58:08.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/busca_index_item_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      322 2023-09-11 16:58:26.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/rolamento_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3215 2024-05-07 18:18:19.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/rolar_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     4858 2024-05-08 11:54:05.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/tabela_rolavel.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.932083 ttrpgaag-4.0.1/TTRPGaag.egg-info/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1643 2024-05-08 12:01:18.000000 ttrpgaag-4.0.1/TTRPGaag.egg-info/PKG-INFO
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1795 2024-05-08 12:01:18.000000 ttrpgaag-4.0.1/TTRPGaag.egg-info/SOURCES.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        1 2024-05-08 12:01:18.000000 ttrpgaag-4.0.1/TTRPGaag.egg-info/dependency_links.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       10 2024-05-08 12:01:18.000000 ttrpgaag-4.0.1/TTRPGaag.egg-info/top_level.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       38 2024-05-08 12:01:18.933510 ttrpgaag-4.0.1/setup.cfg
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      480 2024-05-08 11:58:05.000000 ttrpgaag-4.0.1/setup.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.931532 ttrpgaag-4.0.1/tests/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-09 18:10:54.000000 ttrpgaag-4.0.1/tests/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.648918 ttrpgaag-4.1.0/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1075 2023-10-09 18:00:41.000000 ttrpgaag-4.1.0/LICENSE
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       47 2023-10-09 18:12:41.000000 ttrpgaag-4.1.0/MANIFEST.in
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1797 2024-05-09 14:13:48.648079 ttrpgaag-4.1.0/PKG-INFO
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1570 2024-05-09 14:10:06.000000 ttrpgaag-4.1.0/README.md
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.616623 ttrpgaag-4.1.0/RPG/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      254 2024-05-09 11:50:29.000000 ttrpgaag-4.1.0/RPG/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     6480 2024-04-22 12:53:12.000000 ttrpgaag-4.1.0/RPG/baralho.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.619355 ttrpgaag-4.1.0/RPG/dado/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       94 2023-10-11 14:22:30.000000 ttrpgaag-4.1.0/RPG/dado/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3357 2023-11-13 11:34:50.000000 ttrpgaag-4.1.0/RPG/dado/dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     2117 2024-04-22 12:53:12.000000 ttrpgaag-4.1.0/RPG/dado/dados.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.620859 ttrpgaag-4.1.0/RPG/dado/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-4.1.0/RPG/dado/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1512 2024-05-09 11:50:29.000000 ttrpgaag-4.1.0/RPG/dado/helpers/converter_notacao_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      295 2023-10-11 18:00:52.000000 ttrpgaag-4.1.0/RPG/dado/helpers/monta_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2024-05-09 11:50:29.000000 ttrpgaag-4.1.0/RPG/dado/rolar_dado_notacao.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      803 2024-04-22 12:53:12.000000 ttrpgaag-4.1.0/RPG/iniciativa.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.621700 ttrpgaag-4.1.0/RPG/sistemas/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.1.0/RPG/sistemas/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.623839 ttrpgaag-4.1.0/RPG/sistemas/dnd/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       91 2023-09-14 17:58:19.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.625621 ttrpgaag-4.1.0/RPG/sistemas/dnd/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      245 2024-01-22 19:11:21.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/data/mecanicas.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     7566 2023-09-14 16:09:39.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/data/tesouro.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.627552 ttrpgaag-4.1.0/RPG/sistemas/dnd/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      247 2023-10-11 18:00:52.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/helpers/calcular_mod_atributo.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      391 2024-05-08 12:03:40.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/helpers/checa_testes.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1044 2024-05-08 12:03:40.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/rola_tesouro.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     5269 2024-05-08 12:03:40.000000 ttrpgaag-4.1.0/RPG/sistemas/dnd/teste.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.630217 ttrpgaag-4.1.0/RPG/sistemas/pf2/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     8697 2024-04-22 12:53:12.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/PC.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      191 2023-12-06 18:02:34.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     6181 2024-05-08 12:03:40.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/calcula_dano.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.635424 ttrpgaag-4.1.0/RPG/sistemas/pf2/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      494 2023-12-06 18:02:34.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3279 2023-11-27 11:50:56.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/data/defesas_monstros.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      109 2023-11-27 11:50:56.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/data/proficiency.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       74 2023-12-06 18:02:34.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/data/saves.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      405 2023-12-06 18:02:34.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/data/skills.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      119 2023-12-06 18:02:34.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/data/tipos_ataques.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      101 2023-12-06 18:02:34.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/data/tipos_defesas.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.637835 ttrpgaag-4.1.0/RPG/sistemas/pf2/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-12-01 15:28:03.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      280 2023-12-06 18:02:34.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/helpers/atributo.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     5426 2024-05-08 12:03:40.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/helpers/base_calcula_dano.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      807 2024-05-08 12:03:40.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/helpers/proficiencias.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      855 2023-12-06 18:02:34.000000 ttrpgaag-4.1.0/RPG/sistemas/pf2/proficiencia.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.639049 ttrpgaag-4.1.0/RPG/sistemas/rolemaster/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       64 2023-09-14 16:09:39.000000 ttrpgaag-4.1.0/RPG/sistemas/rolemaster/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1315 2024-05-08 12:03:40.000000 ttrpgaag-4.1.0/RPG/sistemas/rolemaster/consulta_critico.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.640271 ttrpgaag-4.1.0/RPG/sistemas/rolemaster/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.1.0/RPG/sistemas/rolemaster/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)    28276 2023-09-14 16:09:39.000000 ttrpgaag-4.1.0/RPG/sistemas/rolemaster/data/criticos.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.642067 ttrpgaag-4.1.0/RPG/tabela_rolavel/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      102 2024-05-09 11:57:03.000000 ttrpgaag-4.1.0/RPG/tabela_rolavel/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.644949 ttrpgaag-4.1.0/RPG/tabela_rolavel/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 17:28:48.000000 ttrpgaag-4.1.0/RPG/tabela_rolavel/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1014 2024-05-09 11:50:29.000000 ttrpgaag-4.1.0/RPG/tabela_rolavel/helpers/ajeita_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      723 2024-05-08 12:03:40.000000 ttrpgaag-4.1.0/RPG/tabela_rolavel/helpers/ajusta_resultados.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      183 2023-09-11 16:58:08.000000 ttrpgaag-4.1.0/RPG/tabela_rolavel/helpers/busca_index_item_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      322 2023-09-11 16:58:26.000000 ttrpgaag-4.1.0/RPG/tabela_rolavel/helpers/rolamento_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3215 2024-05-07 18:18:19.000000 ttrpgaag-4.1.0/RPG/tabela_rolavel/rolar_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     7008 2024-05-09 12:54:47.000000 ttrpgaag-4.1.0/RPG/tabela_rolavel/tabela_rolavel.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.647392 ttrpgaag-4.1.0/TTRPGaag.egg-info/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1797 2024-05-09 14:13:48.000000 ttrpgaag-4.1.0/TTRPGaag.egg-info/PKG-INFO
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1795 2024-05-09 14:13:48.000000 ttrpgaag-4.1.0/TTRPGaag.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        1 2024-05-09 14:13:48.000000 ttrpgaag-4.1.0/TTRPGaag.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       10 2024-05-09 14:13:48.000000 ttrpgaag-4.1.0/TTRPGaag.egg-info/top_level.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       38 2024-05-09 14:13:48.649072 ttrpgaag-4.1.0/setup.cfg
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      480 2024-05-09 14:09:10.000000 ttrpgaag-4.1.0/setup.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-09 14:13:48.647013 ttrpgaag-4.1.0/tests/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-09 18:10:54.000000 ttrpgaag-4.1.0/tests/__init__.py
```

### Comparing `ttrpgaag-4.0.1/LICENSE` & `ttrpgaag-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/PKG-INFO` & `ttrpgaag-4.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TTRPGaag
-Version: 4.0.1
+Version: 4.1.0
 Summary: Pacote básico de Ferramentas de RPG em português
 Author: Alessandro Guarita
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **4.1.0** - Nova classe para tabelas roláveis `TabelaRolavelSimples` para tabelas que cada item tem a mesma chance de sair (como 20 itens e rolar d20)
 - **4.0.1** - Atualização das importações usando caminho relativo
 - **4.0.0** - Métodos de criação de tabelas da `TabelaRolavel` renomeados para o verbo no infinitivo. Inclusão de parâmetro para rolar a subtabela ou não
 - **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
```

### Comparing `ttrpgaag-4.0.1/README.md` & `ttrpgaag-4.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **4.1.0** - Nova classe para tabelas roláveis `TabelaRolavelSimples` para tabelas que cada item tem a mesma chance de sair (como 20 itens e rolar d20)
 - **4.0.1** - Atualização das importações usando caminho relativo
 - **4.0.0** - Métodos de criação de tabelas da `TabelaRolavel` renomeados para o verbo no infinitivo. Inclusão de parâmetro para rolar a subtabela ou não
 - **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
```

### Comparing `ttrpgaag-4.0.1/RPG/baralho.py` & `ttrpgaag-4.1.0/RPG/baralho.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/dado/dado.py` & `ttrpgaag-4.1.0/RPG/dado/dado.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/dado/dados.py` & `ttrpgaag-4.1.0/RPG/dado/dados.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/dado/helpers/converter_notacao_dado.py` & `ttrpgaag-4.1.0/RPG/dado/helpers/converter_notacao_dado.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/dado/rolar_dado_notacao.py` & `ttrpgaag-4.1.0/RPG/dado/rolar_dado_notacao.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/iniciativa.py` & `ttrpgaag-4.1.0/RPG/iniciativa.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/dnd/data/tesouro.py` & `ttrpgaag-4.1.0/RPG/sistemas/dnd/data/tesouro.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/dnd/rola_tesouro.py` & `ttrpgaag-4.1.0/RPG/sistemas/dnd/rola_tesouro.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/dnd/teste.py` & `ttrpgaag-4.1.0/RPG/sistemas/dnd/teste.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/pf2/PC.py` & `ttrpgaag-4.1.0/RPG/sistemas/pf2/PC.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/pf2/calcula_dano.py` & `ttrpgaag-4.1.0/RPG/sistemas/pf2/calcula_dano.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/pf2/data/defesas_monstros.py` & `ttrpgaag-4.1.0/RPG/sistemas/pf2/data/defesas_monstros.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/base_calcula_dano.py` & `ttrpgaag-4.1.0/RPG/sistemas/pf2/helpers/base_calcula_dano.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/proficiencias.py` & `ttrpgaag-4.1.0/RPG/sistemas/pf2/helpers/proficiencias.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/pf2/proficiencia.py` & `ttrpgaag-4.1.0/RPG/sistemas/pf2/proficiencia.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/rolemaster/consulta_critico.py` & `ttrpgaag-4.1.0/RPG/sistemas/rolemaster/consulta_critico.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/sistemas/rolemaster/data/criticos.py` & `ttrpgaag-4.1.0/RPG/sistemas/rolemaster/data/criticos.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/ajeita_tabela.py` & `ttrpgaag-4.1.0/RPG/tabela_rolavel/helpers/ajeita_tabela.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/ajusta_resultados.py` & `ttrpgaag-4.1.0/RPG/tabela_rolavel/helpers/ajusta_resultados.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/tabela_rolavel/rolar_tabela.py` & `ttrpgaag-4.1.0/RPG/tabela_rolavel/rolar_tabela.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.1/RPG/tabela_rolavel/tabela_rolavel.py` & `ttrpgaag-4.1.0/RPG/tabela_rolavel/tabela_rolavel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from random import choice
+
 from .rolar_tabela import rolar_tabela
 from .helpers.ajeita_tabela import ajeita_tabela
 from .helpers.busca_index_item_tabela import busca_index_item_tabela
 from .helpers.rolamento_dado import DadoRolado
 from ..dado import rolar_dado_notacao
 
 
@@ -29,14 +31,15 @@
     def __repr__(self):
         return f'<Tabela Rolável={self._tabela},\n dado usado: {self._dados}>'
 
     def __str__(self):
         return f'Rolamento de {self._dados} + mod ({self.rolamento.modificador}): {self.rolamento.total}. Resultado: {self._resultado}'
 
     # Métodos de edição da _tabela ====================================================================================
+    # Usados para tabelas que podem ser mudadas conforme o resultado
     def inserir_linha_tabela(self, valor_menor: int, valor_maior: int, resultado) -> None:
         self._tabela.append([(valor_menor, valor_maior), resultado])
 
     def editar_alcance_da_linha(self, valor_da_busca: int, novo_minimo: int, novo_maximo: int) -> None:
         """
         Altera o alcance de uma linha da _tabela.
 
@@ -89,8 +92,63 @@
 
     @property
     def resultado(self):
         if type(self._resultado) is TabelaRolavel and self.rola_subtabela:
             self._resultado.rolar()
             return self._resultado.resultado
 
+        return self._resultado
+
+class TabelaRolavelSimples:
+    """
+    Igual a TabelaRolavel, a diferença é que todos os itens da tabela tem a mesma chance de saírem
+    Como uma tabela de 20 itens que rola o d20 para saber o resultado
+    """
+    def __init__(self, tabela: list = None, rola_subtabela: bool = False):
+        self._tabela = tabela
+        self._resultado = ''
+
+        self.rola_subtabela = rola_subtabela
+
+        self.rolar()
+
+    def __repr__(self):
+        return f'<Tabela Rolável Simples de {len(self._tabela)} itens={self._tabela},\n dado usado: d{len(self._tabela)}>'
+    
+    def __str__(self):
+        return f'Rolamento na tabela ({self.rolamento}): {self._resultado}'
+    
+    # Métodos de edição da _tabela ====================================================================================
+    # Usados para tabelas que podem ser mudadas conforme o resultado
+    def inserir_linha_tabela(self, entrada_nova: str):
+        self._tabela.append(entrada_nova)
+
+    def excluir_linha_tabela(self, entrada_excluir: str):
+        self._tabela.remove(entrada_excluir)
+
+    def editar_linha_tabela(self, entrada_antiga: str, entrada_nova: str):
+        indice = self._tabela.index(entrada_antiga)
+        self._tabela[indice] = entrada_nova
+
+    # Métodos de resultado da rolagem ================================================================================
+    def rolar(self, valor_fixo: int = None):
+        if valor_fixo:
+            self._resultado = self._tabela[valor_fixo]
+        else:
+            self._resultado = choice(self._tabela)
+
+    # Getters ========================================================================================================
+    @property
+    def tabela(self):
+        return self._tabela
+
+    @property
+    def rolamento(self):
+        return self._tabela.index(self._resultado)
+
+    @property
+    def resultado(self):
+        if type(self._resultado) is TabelaRolavel and self.rola_subtabela:
+            self._resultado.rolar()
+            return self._resultado.resultado
+
         return self._resultado
```

### Comparing `ttrpgaag-4.0.1/TTRPGaag.egg-info/PKG-INFO` & `ttrpgaag-4.1.0/TTRPGaag.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TTRPGaag
-Version: 4.0.1
+Version: 4.1.0
 Summary: Pacote básico de Ferramentas de RPG em português
 Author: Alessandro Guarita
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **4.1.0** - Nova classe para tabelas roláveis `TabelaRolavelSimples` para tabelas que cada item tem a mesma chance de sair (como 20 itens e rolar d20)
 - **4.0.1** - Atualização das importações usando caminho relativo
 - **4.0.0** - Métodos de criação de tabelas da `TabelaRolavel` renomeados para o verbo no infinitivo. Inclusão de parâmetro para rolar a subtabela ou não
 - **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
```

### Comparing `ttrpgaag-4.0.1/TTRPGaag.egg-info/SOURCES.txt` & `ttrpgaag-4.1.0/TTRPGaag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

