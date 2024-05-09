# Comparing `tmp/pypath_omnipath-0.16.5.tar.gz` & `tmp/pypath_omnipath-0.16.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypath_omnipath-0.16.5.tar", max compression
+gzip compressed data, was "pypath_omnipath-0.16.9.tar", max compression
```

## Comparing `pypath_omnipath-0.16.5.tar` & `pypath_omnipath-0.16.9.tar`

### file list

```diff
@@ -1,371 +1,371 @@
--rw-r--r--   0        0        0    35141 2016-11-05 19:50:35.500333 pypath_omnipath-0.16.5/LICENSE
--rw-r--r--   0        0        0    11505 2023-06-22 21:35:04.475207 pypath_omnipath-0.16.5/README.rst
--rw-r--r--   0        0        0     3244 2023-11-30 09:57:24.113869 pypath_omnipath-0.16.5/pypath/__init__.py
--rw-r--r--   0        0        0     1953 2024-02-04 10:05:05.010160 pypath_omnipath-0.16.5/pypath/_metadata.py
--rw-r--r--   0        0        0      534 2023-11-15 00:54:37.135737 pypath_omnipath-0.16.5/pypath/biocypher/__init__.py
--rw-r--r--   0        0        0     7732 2023-11-15 00:54:37.135737 pypath_omnipath-0.16.5/pypath/biocypher/adapter.py
--rw-r--r--   0        0        0      466 2023-11-15 00:54:37.412403 pypath_omnipath-0.16.5/pypath/core/__init__.py
--rw-r--r--   0        0        0   174619 2023-11-15 00:54:37.389070 pypath_omnipath-0.16.5/pypath/core/annot.py
--rw-r--r--   0        0        0     4090 2023-11-15 00:54:37.429070 pypath_omnipath-0.16.5/pypath/core/attrs.py
--rw-r--r--   0        0        0     4329 2023-11-15 00:54:37.385737 pypath_omnipath-0.16.5/pypath/core/common.py
--rw-r--r--   0        0        0    18802 2023-11-15 00:54:37.432403 pypath_omnipath-0.16.5/pypath/core/complex.py
--rw-r--r--   0        0        0    13137 2023-11-15 00:54:37.429070 pypath_omnipath-0.16.5/pypath/core/entity.py
--rw-r--r--   0        0        0    37304 2023-11-15 00:54:37.429070 pypath_omnipath-0.16.5/pypath/core/enz_sub.py
--rw-r--r--   0        0        0    22791 2023-11-15 00:54:37.429070 pypath_omnipath-0.16.5/pypath/core/evidence.py
--rw-r--r--   0        0        0    97860 2023-11-15 00:54:37.382403 pypath_omnipath-0.16.5/pypath/core/interaction.py
--rw-r--r--   0        0        0    29848 2023-11-15 00:54:37.385737 pypath_omnipath-0.16.5/pypath/core/intercell.py
--rw-r--r--   0        0        0   230501 2023-11-15 00:54:37.419070 pypath_omnipath-0.16.5/pypath/core/intercell_annot.py
--rw-r--r--   0        0        0   141652 2023-11-15 00:54:37.422403 pypath_omnipath-0.16.5/pypath/core/network.py
--rw-r--r--   0        0        0      668 2023-11-30 09:57:24.113869 pypath_omnipath-0.16.5/pypath/data/__init__.py
--rw-r--r--   0        0        0      917 2023-11-30 09:57:24.113869 pypath_omnipath-0.16.5/pypath/data/_data.py
--rw-r--r--   0        0        0     1300 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/embl_colors
--rw-r--r--   0        0        0      271 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/ensembl_biomart_query.xml
--rw-r--r--   0        0        0      227 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/goose_ancestors.sql
--rw-r--r--   0        0        0      712 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/goose_annotations.sql
--rw-r--r--   0        0        0      120 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/goose_terms.sql
--rw-r--r--   0        0        0      185 2023-06-14 13:36:25.323042 pypath_omnipath-0.16.5/pypath/data/licenses/afl_v3.json
--rw-r--r--   0        0        0      186 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/apache_2.0.json
--rw-r--r--   0        0        0      190 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/artistic_2.0.json
--rw-r--r--   0        0        0      199 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/biocarta.json
--rw-r--r--   0        0        0      188 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/bsd.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_2.5.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_3.0.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_4.0.json
--rw-r--r--   0        0        0      242 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nc-nd_3.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nc-nd_4.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nc_2.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nc_3.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nc_4.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nc_sa_3.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nc_sa_4.0.json
--rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nd_3.0.json
--rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_nd_4.0.json
--rw-r--r--   0        0        0      224 2023-06-14 13:36:25.323042 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_sa_2.5.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_sa_3.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_by_sa_4.0.json
--rw-r--r--   0        0        0      233 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cc_zero.json
--rw-r--r--   0        0        0      196 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cellcellinteractions.json
--rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/composite.json
--rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/cosmic.json
--rw-r--r--   0        0        0      194 2022-03-18 18:18:43.477819 pypath_omnipath-0.16.5/pypath/data/licenses/cytosig.json
--rw-r--r--   0        0        0      182 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/dsl.json
--rw-r--r--   0        0        0      185 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/elm.json
--rw-r--r--   0        0        0      174 2022-12-05 01:12:34.015062 pypath_omnipath-0.16.5/pypath/data/licenses/embl-ebi.json
--rw-r--r--   0        0        0      212 2023-06-14 13:36:25.326376 pypath_omnipath-0.16.5/pypath/data/licenses/eul.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/gnu_gpl_v2.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/gnu_gpl_v3.json
--rw-r--r--   0        0        0      200 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/gnu_lgpl_v3.json
--rw-r--r--   0        0        0      311 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/hgnc.json
--rw-r--r--   0        0        0      150 2022-09-15 18:20:39.089511 pypath_omnipath-0.16.5/pypath/data/licenses/hpo.json
--rw-r--r--   0        0        0      139 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/hprd.json
--rw-r--r--   0        0        0      168 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/i2d.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/informal.json
--rw-r--r--   0        0        0      175 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/kegg.json
--rw-r--r--   0        0        0      174 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/kinase-com.json
--rw-r--r--   0        0        0      268 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/mirecords.json
--rw-r--r--   0        0        0      184 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/mirtarbase.json
--rw-r--r--   0        0        0      154 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/mit.json
--rw-r--r--   0        0        0      165 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/mppi.json
--rw-r--r--   0        0        0      360 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/nar.json
--rw-r--r--   0        0        0      179 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/no_license.json
--rw-r--r--   0        0        0      187 2023-09-11 20:08:33.865064 pypath_omnipath-0.16.5/pypath/data/licenses/opentargets.json
--rw-r--r--   0        0        0      177 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/pathwaycommons.json
--rw-r--r--   0        0        0      351 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/pdb.json
--rw-r--r--   0        0        0      363 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/phosphonetworks.json
--rw-r--r--   0        0        0      464 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/licenses/unspecified.json
--rw-r--r--   0        0        0     1150 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/www/favicon.ico
--rw-r--r--   0        0        0      486 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/www/http500.html
--rw-r--r--   0        0        0      324 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.5/pypath/data/www/index.html
--rw-r--r--   0        0        0     5712 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.5/pypath/formats/obo.py
--rw-r--r--   0        0        0    15803 2023-11-30 09:57:24.113869 pypath_omnipath-0.16.5/pypath/formats/sdf.py
--rw-r--r--   0        0        0     8487 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.5/pypath/formats/sqldump.py
--rw-r--r--   0        0        0     1221 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.5/pypath/formats/sqlite.py
--rw-r--r--   0        0        0     7413 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.5/pypath/formats/xml.py
--rw-r--r--   0        0        0     2085 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.5/pypath/inputs/__init__.py
--rw-r--r--   0        0        0      972 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.5/pypath/inputs/abs.py
--rw-r--r--   0        0        0     3052 2023-11-15 00:54:37.325737 pypath_omnipath-0.16.5/pypath/inputs/acsn.py
--rw-r--r--   0        0        0     2263 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.5/pypath/inputs/adhesome.py
--rw-r--r--   0        0        0     4936 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.5/pypath/inputs/adrecs.py
--rw-r--r--   0        0        0     2240 2023-11-15 00:54:37.159070 pypath_omnipath-0.16.5/pypath/inputs/almen2009.py
--rw-r--r--   0        0        0     5184 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.5/pypath/inputs/baccin2019.py
--rw-r--r--   0        0        0     6216 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.5/pypath/inputs/biogps.py
--rw-r--r--   0        0        0     4889 2023-11-15 00:54:37.262403 pypath_omnipath-0.16.5/pypath/inputs/biogrid.py
--rw-r--r--   0        0        0    10224 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.5/pypath/inputs/biomart.py
--rw-r--r--   0        0        0     5262 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.5/pypath/inputs/biomodels.py
--rw-r--r--   0        0        0     1691 2023-11-15 00:54:37.162403 pypath_omnipath-0.16.5/pypath/inputs/ca1.py
--rw-r--r--   0        0        0     2657 2023-11-15 00:54:37.219070 pypath_omnipath-0.16.5/pypath/inputs/cancercellmap.py
--rw-r--r--   0        0        0     5490 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.5/pypath/inputs/cancerdrugsdb.py
--rw-r--r--   0        0        0     1804 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.5/pypath/inputs/cancersea.py
--rw-r--r--   0        0        0     3255 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.5/pypath/inputs/cell.py
--rw-r--r--   0        0        0     6235 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.5/pypath/inputs/cellcall.py
--rw-r--r--   0        0        0     1448 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.5/pypath/inputs/cellcellinteractions.py
--rw-r--r--   0        0        0     9032 2023-11-15 00:54:37.179070 pypath_omnipath-0.16.5/pypath/inputs/cellchatdb.py
--rw-r--r--   0        0        0    14933 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.5/pypath/inputs/cellinker.py
--rw-r--r--   0        0        0     8984 2023-11-15 00:54:37.352403 pypath_omnipath-0.16.5/pypath/inputs/cellphonedb.py
--rw-r--r--   0        0        0     5238 2023-11-15 00:54:37.302403 pypath_omnipath-0.16.5/pypath/inputs/celltalkdb.py
--rw-r--r--   0        0        0     2097 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.5/pypath/inputs/celltypist.py
--rw-r--r--   0        0        0    13772 2023-11-15 00:54:37.295737 pypath_omnipath-0.16.5/pypath/inputs/chembl.py
--rw-r--r--   0        0        0     3841 2023-11-15 00:54:37.312403 pypath_omnipath-0.16.5/pypath/inputs/clinvar.py
--rw-r--r--   0        0        0     5525 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.5/pypath/inputs/collectri.py
--rw-r--r--   0        0        0     8341 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.5/pypath/inputs/common.py
--rw-r--r--   0        0        0     2412 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.5/pypath/inputs/compath.py
--rw-r--r--   0        0        0     2553 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.5/pypath/inputs/compleat.py
--rw-r--r--   0        0        0     4406 2023-11-15 00:54:37.309070 pypath_omnipath-0.16.5/pypath/inputs/complexportal.py
--rw-r--r--   0        0        0     3933 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.5/pypath/inputs/comppi.py
--rw-r--r--   0        0        0     2685 2023-11-15 00:54:37.259070 pypath_omnipath-0.16.5/pypath/inputs/connectomedb.py
--rw-r--r--   0        0        0     2690 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.5/pypath/inputs/corum.py
--rw-r--r--   0        0        0     4676 2023-11-15 00:54:37.329070 pypath_omnipath-0.16.5/pypath/inputs/cosmic.py
--rw-r--r--   0        0        0     4061 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.5/pypath/inputs/cpad.py
--rw-r--r--   0        0        0     1886 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.5/pypath/inputs/cpdb.py
--rw-r--r--   0        0        0     3309 2023-11-15 00:54:37.312403 pypath_omnipath-0.16.5/pypath/inputs/credentials.py
--rw-r--r--   0        0        0     3241 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.5/pypath/inputs/csa.py
--rw-r--r--   0        0        0     3444 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.5/pypath/inputs/cspa.py
--rw-r--r--   0        0        0     4976 2023-11-15 00:54:37.295737 pypath_omnipath-0.16.5/pypath/inputs/ctdbase.py
--rw-r--r--   0        0        0     3240 2023-11-15 00:54:37.145737 pypath_omnipath-0.16.5/pypath/inputs/cytosig.py
--rw-r--r--   0        0        0     4662 2023-11-15 00:54:37.172403 pypath_omnipath-0.16.5/pypath/inputs/dbptm.py
--rw-r--r--   0        0        0     5188 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.5/pypath/inputs/ddinter.py
--rw-r--r--   0        0        0     2734 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.5/pypath/inputs/deathdomain.py
--rw-r--r--   0        0        0     4281 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.5/pypath/inputs/depod.py
--rw-r--r--   0        0        0     3589 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.5/pypath/inputs/dgidb.py
--rw-r--r--   0        0        0     4851 2023-11-15 00:54:37.175737 pypath_omnipath-0.16.5/pypath/inputs/dip.py
--rw-r--r--   0        0        0     5635 2024-02-04 09:38:34.186749 pypath_omnipath-0.16.5/pypath/inputs/diseases.py
--rw-r--r--   0        0        0      592 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/__init__.py
--rw-r--r--   0        0        0      671 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_api/__init__.py
--rw-r--r--   0        0        0     6335 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_api/meta.py
--rw-r--r--   0        0        0     5726 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_api/schema.py
--rw-r--r--   0        0        0     4949 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_api/simple.py
--rw-r--r--   0        0        0     3522 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_auth.py
--rw-r--r--   0        0        0     1925 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_client.py
--rw-r--r--   0        0        0     2587 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_field.py
--rw-r--r--   0        0        0     2355 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_proc.py
--rw-r--r--   0        0        0     2109 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_records.py
--rw-r--r--   0        0        0     6242 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_request.py
--rw-r--r--   0        0        0     1548 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_schema.py
--rw-r--r--   0        0        0     2604 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.5/pypath/inputs/disgenet/_valid.py
--rw-r--r--   0        0        0    17032 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.5/pypath/inputs/domino.py
--rw-r--r--   0        0        0    12556 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.5/pypath/inputs/dorothea.py
--rw-r--r--   0        0        0    20545 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.5/pypath/inputs/drugbank.py
--rw-r--r--   0        0        0     4575 2023-11-15 00:54:37.309070 pypath_omnipath-0.16.5/pypath/inputs/drugcentral.py
--rw-r--r--   0        0        0     4696 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.5/pypath/inputs/ebi.py
--rw-r--r--   0        0        0     4826 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.5/pypath/inputs/elm.py
--rw-r--r--   0        0        0     2420 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.5/pypath/inputs/embopress.py
--rw-r--r--   0        0        0     4424 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.5/pypath/inputs/embrace.py
--rw-r--r--   0        0        0     1117 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.5/pypath/inputs/encode.py
--rw-r--r--   0        0        0     1879 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.5/pypath/inputs/ensembl.py
--rw-r--r--   0        0        0     3134 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.5/pypath/inputs/eutils.py
--rw-r--r--   0        0        0     3049 2023-11-15 00:54:37.322404 pypath_omnipath-0.16.5/pypath/inputs/exocarta.py
--rw-r--r--   0        0        0     3179 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.5/pypath/inputs/expasy.py
--rw-r--r--   0        0        0     3322 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.5/pypath/inputs/genecards.py
--rw-r--r--   0        0        0    25944 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.5/pypath/inputs/go.py
--rw-r--r--   0        0        0     2253 2023-11-15 00:54:37.312403 pypath_omnipath-0.16.5/pypath/inputs/gpcrdb.py
--rw-r--r--   0        0        0     1834 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.5/pypath/inputs/graphviz.py
--rw-r--r--   0        0        0     8158 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.5/pypath/inputs/guide2pharma.py
--rw-r--r--   0        0        0     3448 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.5/pypath/inputs/gutmgene.py
--rw-r--r--   0        0        0     1494 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.5/pypath/inputs/havugimana.py
--rw-r--r--   0        0        0     1525 2023-11-15 00:54:37.239070 pypath_omnipath-0.16.5/pypath/inputs/hgnc.py
--rw-r--r--   0        0        0     3660 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.5/pypath/inputs/hippie.py
--rw-r--r--   0        0        0     1075 2023-11-15 00:54:37.242403 pypath_omnipath-0.16.5/pypath/inputs/hmdb/__init__.py
--rw-r--r--   0        0        0     6310 2023-11-15 00:54:37.239070 pypath_omnipath-0.16.5/pypath/inputs/hmdb/common.py
--rw-r--r--   0        0        0     5066 2023-11-15 00:54:37.239070 pypath_omnipath-0.16.5/pypath/inputs/hmdb/metabolites.py
--rw-r--r--   0        0        0     5019 2023-11-15 00:54:37.242403 pypath_omnipath-0.16.5/pypath/inputs/hmdb/proteins.py
--rw-r--r--   0        0        0      579 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.5/pypath/inputs/hmdb/schema/__init__.py
--rw-r--r--   0        0        0     2196 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.5/pypath/inputs/hmdb/schema/common.py
--rw-r--r--   0        0        0     5002 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.5/pypath/inputs/hmdb/schema/metabolites.py
--rw-r--r--   0        0        0     2871 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.5/pypath/inputs/hmdb/schema/proteins.py
--rw-r--r--   0        0        0     1168 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.5/pypath/inputs/hmdb/structures.py
--rw-r--r--   0        0        0     1591 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.5/pypath/inputs/hmdb/visual.py
--rw-r--r--   0        0        0     1189 2023-11-15 00:54:37.242403 pypath_omnipath-0.16.5/pypath/inputs/hmdb/xml.py
--rw-r--r--   0        0        0     4697 2023-11-15 00:54:37.295737 pypath_omnipath-0.16.5/pypath/inputs/homologene.py
--rw-r--r--   0        0        0    10232 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.5/pypath/inputs/hpmr.py
--rw-r--r--   0        0        0     4943 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.5/pypath/inputs/hpo.py
--rw-r--r--   0        0        0     2645 2023-11-15 00:54:37.172403 pypath_omnipath-0.16.5/pypath/inputs/hprd.py
--rw-r--r--   0        0        0     1388 2023-11-15 00:54:37.219070 pypath_omnipath-0.16.5/pypath/inputs/htri.py
--rw-r--r--   0        0        0     1669 2023-11-15 00:54:37.302403 pypath_omnipath-0.16.5/pypath/inputs/humancellmap.py
--rw-r--r--   0        0        0     1945 2023-11-15 00:54:37.309070 pypath_omnipath-0.16.5/pypath/inputs/humap.py
--rw-r--r--   0        0        0     2189 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.5/pypath/inputs/humsavar.py
--rw-r--r--   0        0        0     7990 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.5/pypath/inputs/huri.py
--rw-r--r--   0        0        0     2562 2023-11-15 00:54:37.179070 pypath_omnipath-0.16.5/pypath/inputs/i3d.py
--rw-r--r--   0        0        0     6610 2023-11-15 00:54:37.175737 pypath_omnipath-0.16.5/pypath/inputs/icellnet.py
--rw-r--r--   0        0        0     8010 2023-11-15 00:54:37.259070 pypath_omnipath-0.16.5/pypath/inputs/ielm.py
--rw-r--r--   0        0        0     3811 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.5/pypath/inputs/imweb.py
--rw-r--r--   0        0        0     2139 2023-11-15 00:54:37.172403 pypath_omnipath-0.16.5/pypath/inputs/innatedb.py
--rw-r--r--   0        0        0     2902 2023-11-15 00:54:37.329070 pypath_omnipath-0.16.5/pypath/inputs/instruct.py
--rw-r--r--   0        0        0     5561 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.5/pypath/inputs/intact.py
--rw-r--r--   0        0        0     1638 2023-11-15 00:54:37.179070 pypath_omnipath-0.16.5/pypath/inputs/integrins.py
--rw-r--r--   0        0        0     8739 2023-11-15 00:54:37.262403 pypath_omnipath-0.16.5/pypath/inputs/interpro.py
--rw-r--r--   0        0        0     2427 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.5/pypath/inputs/intogen.py
--rw-r--r--   0        0        0     1605 2023-11-15 00:54:37.262403 pypath_omnipath-0.16.5/pypath/inputs/ipi.py
--rw-r--r--   0        0        0     3462 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.5/pypath/inputs/iptmnet.py
--rw-r--r--   0        0        0     3033 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.5/pypath/inputs/italk.py
--rw-r--r--   0        0        0     2454 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.5/pypath/inputs/kea.py
--rw-r--r--   0        0        0    20520 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.5/pypath/inputs/kegg.py
--rw-r--r--   0        0        0    15410 2023-11-15 00:54:37.259070 pypath_omnipath-0.16.5/pypath/inputs/kegg_api.py
--rw-r--r--   0        0        0     1829 2023-11-15 00:54:37.219070 pypath_omnipath-0.16.5/pypath/inputs/kinasedotcom.py
--rw-r--r--   0        0        0     2419 2023-11-15 00:54:37.172403 pypath_omnipath-0.16.5/pypath/inputs/kirouac2010.py
--rw-r--r--   0        0        0     4224 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.5/pypath/inputs/lambert2018.py
--rw-r--r--   0        0        0     2071 2023-11-15 00:54:37.159070 pypath_omnipath-0.16.5/pypath/inputs/laudanna.py
--rw-r--r--   0        0        0     5534 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.5/pypath/inputs/li2012.py
--rw-r--r--   0        0        0     2522 2023-11-15 00:54:37.265737 pypath_omnipath-0.16.5/pypath/inputs/lincs.py
--rw-r--r--   0        0        0      494 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.5/pypath/inputs/lipidmaps/__init__.py
--rw-r--r--   0        0        0     1246 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.5/pypath/inputs/lipidmaps/structures.py
--rw-r--r--   0        0        0     2823 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.5/pypath/inputs/lmpid.py
--rw-r--r--   0        0        0     1508 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.5/pypath/inputs/lncdisease.py
--rw-r--r--   0        0        0     2003 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.5/pypath/inputs/lncrnadb.py
--rw-r--r--   0        0        0     7781 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.5/pypath/inputs/locate.py
--rw-r--r--   0        0        0     3489 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.5/pypath/inputs/lrdb.py
--rw-r--r--   0        0        0     2804 2023-11-15 00:54:37.319070 pypath_omnipath-0.16.5/pypath/inputs/macrophage.py
--rw-r--r--   0        0        0      468 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.5/pypath/inputs/main.py
--rw-r--r--   0        0        0     2231 2023-11-15 00:54:37.219070 pypath_omnipath-0.16.5/pypath/inputs/matrisome.py
--rw-r--r--   0        0        0     4065 2023-11-15 00:54:37.302403 pypath_omnipath-0.16.5/pypath/inputs/matrixdb.py
--rw-r--r--   0        0        0     1004 2023-11-15 00:54:37.152403 pypath_omnipath-0.16.5/pypath/inputs/mcam.py
--rw-r--r--   0        0        0     1885 2023-11-15 00:54:37.329070 pypath_omnipath-0.16.5/pypath/inputs/membranome.py
--rw-r--r--   0        0        0     4193 2023-11-15 00:54:37.319070 pypath_omnipath-0.16.5/pypath/inputs/mimp.py
--rw-r--r--   0        0        0     1262 2023-11-15 00:54:37.325737 pypath_omnipath-0.16.5/pypath/inputs/mir2disease.py
--rw-r--r--   0        0        0     3779 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.5/pypath/inputs/mirbase.py
--rw-r--r--   0        0        0     1639 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.5/pypath/inputs/mirdeathdb.py
--rw-r--r--   0        0        0     1655 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.5/pypath/inputs/mirecords.py
--rw-r--r--   0        0        0     2231 2023-11-15 00:54:37.322404 pypath_omnipath-0.16.5/pypath/inputs/mirtarbase.py
--rw-r--r--   0        0        0      968 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.5/pypath/inputs/mitab.py
--rw-r--r--   0        0        0     3063 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.5/pypath/inputs/mppi.py
--rw-r--r--   0        0        0    11388 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.5/pypath/inputs/msigdb.py
--rw-r--r--   0        0        0     1997 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.5/pypath/inputs/ncrdeathdb.py
--rw-r--r--   0        0        0     1727 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.5/pypath/inputs/negatome.py
--rw-r--r--   0        0        0     1655 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.5/pypath/inputs/netbiol.py
--rw-r--r--   0        0        0     6273 2023-11-15 00:54:37.175737 pypath_omnipath-0.16.5/pypath/inputs/netpath.py
--rw-r--r--   0        0        0     1862 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.5/pypath/inputs/offsides.py
--rw-r--r--   0        0        0     7220 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.5/pypath/inputs/oma.py
--rw-r--r--   0        0        0     3497 2023-11-15 00:54:37.159070 pypath_omnipath-0.16.5/pypath/inputs/ontology.py
--rw-r--r--   0        0        0     6747 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.5/pypath/inputs/opentargets.py
--rw-r--r--   0        0        0     2742 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.5/pypath/inputs/opm.py
--rw-r--r--   0        0        0     2210 2023-11-15 00:54:37.299070 pypath_omnipath-0.16.5/pypath/inputs/oreganno.py
--rw-r--r--   0        0        0     3900 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.5/pypath/inputs/panglaodb.py
--rw-r--r--   0        0        0     3426 2023-11-15 00:54:37.145737 pypath_omnipath-0.16.5/pypath/inputs/pathophenodb.py
--rw-r--r--   0        0        0     4465 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.5/pypath/inputs/pathwaycommons.py
--rw-r--r--   0        0        0      968 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.5/pypath/inputs/pazar.py
--rw-r--r--   0        0        0     6230 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.5/pypath/inputs/pdb.py
--rw-r--r--   0        0        0     2308 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.5/pypath/inputs/pdzbase.py
--rw-r--r--   0        0        0     6557 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.5/pypath/inputs/pepcyber.py
--rw-r--r--   0        0        0     8994 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.5/pypath/inputs/pfam.py
--rw-r--r--   0        0        0     6485 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.5/pypath/inputs/pharos.py
--rw-r--r--   0        0        0     1514 2023-11-15 00:54:37.175737 pypath_omnipath-0.16.5/pypath/inputs/phobius.py
--rw-r--r--   0        0        0     2196 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.5/pypath/inputs/phosphatome.py
--rw-r--r--   0        0        0     3330 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.5/pypath/inputs/phosphoelm.py
--rw-r--r--   0        0        0     2097 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.5/pypath/inputs/phosphonetworks.py
--rw-r--r--   0        0        0     1196 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.5/pypath/inputs/phosphopoint.py
--rw-r--r--   0        0        0    37214 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.5/pypath/inputs/phosphosite.py
--rw-r--r--   0        0        0     9873 2023-11-15 00:54:37.162403 pypath_omnipath-0.16.5/pypath/inputs/pisa.py
--rw-r--r--   0        0        0     1747 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.5/pypath/inputs/pro.py
--rw-r--r--   0        0        0     3086 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.5/pypath/inputs/progeny.py
--rw-r--r--   0        0        0     7428 2023-11-15 00:54:37.299070 pypath_omnipath-0.16.5/pypath/inputs/proteinatlas.py
--rw-r--r--   0        0        0     3470 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.5/pypath/inputs/proteins.py
--rw-r--r--   0        0        0     3705 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.5/pypath/inputs/protmapper.py
--rw-r--r--   0        0        0     2360 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.5/pypath/inputs/pubchem.py
--rw-r--r--   0        0        0     3453 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.5/pypath/inputs/pubmed.py
--rw-r--r--   0        0        0     4315 2023-11-15 00:54:37.239070 pypath_omnipath-0.16.5/pypath/inputs/ramilowski2015.py
--rw-r--r--   0        0        0     5289 2023-11-15 00:54:37.159070 pypath_omnipath-0.16.5/pypath/inputs/ramp.py
--rw-r--r--   0        0        0     6393 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.5/pypath/inputs/rdata.py
--rw-r--r--   0        0        0    40019 2023-11-15 00:54:37.162403 pypath_omnipath-0.16.5/pypath/inputs/reaction.py
--rw-r--r--   0        0        0     3714 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.5/pypath/inputs/reactome.py
--rw-r--r--   0        0        0     7578 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.5/pypath/inputs/scconnect.py
--rw-r--r--   0        0        0     2352 2023-11-15 00:54:37.152403 pypath_omnipath-0.16.5/pypath/inputs/science.py
--rw-r--r--   0        0        0     4356 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.5/pypath/inputs/sider.py
--rw-r--r--   0        0        0     5475 2023-11-15 00:54:37.319070 pypath_omnipath-0.16.5/pypath/inputs/signalink.py
--rw-r--r--   0        0        0    11624 2023-11-15 00:54:37.262403 pypath_omnipath-0.16.5/pypath/inputs/signor.py
--rw-r--r--   0        0        0     5578 2023-11-15 00:54:37.145737 pypath_omnipath-0.16.5/pypath/inputs/spike.py
--rw-r--r--   0        0        0     4160 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.5/pypath/inputs/stitch.py
--rw-r--r--   0        0        0     7188 2023-11-15 00:54:37.179070 pypath_omnipath-0.16.5/pypath/inputs/string.py
--rw-r--r--   0        0        0     1476 2023-11-15 00:54:37.322404 pypath_omnipath-0.16.5/pypath/inputs/surfaceome.py
--rw-r--r--   0        0        0     4309 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.5/pypath/inputs/switches_elm.py
--rw-r--r--   0        0        0     3122 2023-11-15 00:54:37.299070 pypath_omnipath-0.16.5/pypath/inputs/talklr.py
--rw-r--r--   0        0        0     2513 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.5/pypath/inputs/tcdb.py
--rw-r--r--   0        0        0     2016 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.5/pypath/inputs/tfcensus.py
--rw-r--r--   0        0        0     7823 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.5/pypath/inputs/threedcomplex.py
--rw-r--r--   0        0        0    17262 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.5/pypath/inputs/threedid.py
--rw-r--r--   0        0        0     3589 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.5/pypath/inputs/topdb.py
--rw-r--r--   0        0        0     1350 2023-11-15 00:54:37.352403 pypath_omnipath-0.16.5/pypath/inputs/transmir.py
--rw-r--r--   0        0        0     9801 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.5/pypath/inputs/trip.py
--rw-r--r--   0        0        0     2158 2023-11-15 00:54:37.145737 pypath_omnipath-0.16.5/pypath/inputs/trrust.py
--rw-r--r--   0        0        0     1384 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.5/pypath/inputs/twosides.py
--rw-r--r--   0        0        0     5093 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.5/pypath/inputs/unichem.py
--rw-r--r--   0        0        0    46655 2023-11-18 00:12:01.136439 pypath_omnipath-0.16.5/pypath/inputs/uniprot.py
--rw-r--r--   0        0        0     3418 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.5/pypath/inputs/uniprot_db.py
--rw-r--r--   0        0        0     7499 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.5/pypath/inputs/wang.py
--rw-r--r--   0        0        0     2068 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.5/pypath/inputs/wojtowicz2020.py
--rw-r--r--   0        0        0     1516 2023-11-15 00:54:37.162403 pypath_omnipath-0.16.5/pypath/inputs/zhong2015.py
--rw-r--r--   0        0        0      466 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.5/pypath/internals/__init__.py
--rw-r--r--   0        0        0    11713 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.5/pypath/internals/annot_formats.py
--rw-r--r--   0        0        0    25898 2024-02-04 09:38:13.366748 pypath_omnipath-0.16.5/pypath/internals/input_formats.py
--rw-r--r--   0        0        0    43659 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.5/pypath/internals/intera.py
--rw-r--r--   0        0        0     7416 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.5/pypath/internals/license.py
--rw-r--r--   0        0        0     4558 2024-02-04 09:38:13.366748 pypath_omnipath-0.16.5/pypath/internals/maps.py
--rw-r--r--   0        0        0     4102 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.5/pypath/internals/refs.py
--rw-r--r--   0        0        0    13178 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.5/pypath/internals/resource.py
--rw-r--r--   0        0        0      466 2023-11-15 00:54:37.352403 pypath_omnipath-0.16.5/pypath/legacy/__init__.py
--rw-r--r--   0        0        0     4421 2023-11-15 00:54:37.369070 pypath_omnipath-0.16.5/pypath/legacy/db_categories.py
--rw-r--r--   0        0        0   556333 2023-11-15 00:54:37.369070 pypath_omnipath-0.16.5/pypath/legacy/main.py
--rw-r--r--   0        0        0     1580 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/__init__.py
--rw-r--r--   0        0        0    17814 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/app.py
--rw-r--r--   0        0        0    16762 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/bel.py
--rw-r--r--   0        0        0    16578 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/cellphonedb.py
--rw-r--r--   0        0        0     1290 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/databases/__init__.py
--rw-r--r--   0        0        0     1660 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/databases/build.py
--rw-r--r--   0        0        0     1729 2022-12-05 01:12:34.028395 pypath_omnipath-0.16.5/pypath/omnipath/databases/builtins.json
--rw-r--r--   0        0        0      522 2022-01-24 11:42:01.191613 pypath_omnipath-0.16.5/pypath/omnipath/databases/classes.json
--rw-r--r--   0        0        0     7366 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/databases/define.py
--rw-r--r--   0        0        0    30885 2023-11-15 00:55:01.929072 pypath_omnipath-0.16.5/pypath/omnipath/export.py
--rw-r--r--   0        0        0     4076 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/legacy.py
--rw-r--r--   0        0        0     1605 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/omnipath/param.py
--rw-r--r--   0        0        0      466 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.5/pypath/omnipath/server/__init__.py
--rw-r--r--   0        0        0   122710 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.5/pypath/omnipath/server/_html.py
--rw-r--r--   0        0        0    10404 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.5/pypath/omnipath/server/build.py
--rw-r--r--   0        0        0    17053 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.5/pypath/omnipath/server/generate_about_page.py
--rw-r--r--   0        0        0    11019 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.5/pypath/omnipath/server/legacy.py
--rw-r--r--   0        0        0    79455 2024-02-04 09:38:13.370082 pypath_omnipath-0.16.5/pypath/omnipath/server/run.py
--rw-r--r--   0        0        0     4209 2023-11-15 00:54:37.519070 pypath_omnipath-0.16.5/pypath/reader/field.py
--rw-r--r--   0        0        0     1517 2023-11-15 00:54:37.519070 pypath_omnipath-0.16.5/pypath/reader/network.py
--rw-r--r--   0        0        0      914 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.5/pypath/resources/__init__.py
--rw-r--r--   0        0        0    14134 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.5/pypath/resources/controller.py
--rw-r--r--   0        0        0      466 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.5/pypath/resources/data/__init__.py
--rw-r--r--   0        0        0      139 2023-01-10 18:56:49.559042 pypath_omnipath-0.16.5/pypath/resources/data/complex_input_template.json
--rw-r--r--   0        0        0      239 2023-01-10 18:56:35.023580 pypath_omnipath-0.16.5/pypath/resources/data/enz_sub_input_template.json
--rw-r--r--   0        0        0   179340 2023-09-11 20:49:37.078549 pypath_omnipath-0.16.5/pypath/resources/data/resources.json
--rw-r--r--   0        0        0   100598 2023-11-15 00:54:37.519070 pypath_omnipath-0.16.5/pypath/resources/data_formats.py
--rw-r--r--   0        0        0   178871 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.5/pypath/resources/descriptions.py
--rw-r--r--   0        0        0     2629 2023-11-15 00:54:37.519070 pypath_omnipath-0.16.5/pypath/resources/licenses.py
--rw-r--r--   0        0        0     5620 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.5/pypath/resources/network.py
--rw-r--r--   0        0        0    77246 2023-11-15 01:16:43.172484 pypath_omnipath-0.16.5/pypath/resources/urls.py
--rw-r--r--   0        0        0      465 2023-11-15 00:54:37.439070 pypath_omnipath-0.16.5/pypath/share/__init__.py
--rw-r--r--   0        0        0     1844 2023-11-18 21:10:57.369047 pypath_omnipath-0.16.5/pypath/share/cache.py
--rw-r--r--   0        0        0      500 2023-11-15 00:54:37.439070 pypath_omnipath-0.16.5/pypath/share/common.py
--rw-r--r--   0        0        0      505 2023-11-15 00:54:37.439070 pypath_omnipath-0.16.5/pypath/share/constants.py
--rw-r--r--   0        0        0    56969 2023-11-15 01:04:39.212440 pypath_omnipath-0.16.5/pypath/share/curl.py
--rw-r--r--   0        0        0    17263 2023-11-15 00:54:37.435737 pypath_omnipath-0.16.5/pypath/share/lookup/_manytomany.py
--rw-r--r--   0        0        0     1885 2023-11-15 00:54:37.435737 pypath_omnipath-0.16.5/pypath/share/lookup/_onetomany.py
--rw-r--r--   0        0        0     2422 2023-11-15 00:54:37.432403 pypath_omnipath-0.16.5/pypath/share/lookup/_onetomany2.py
--rw-r--r--   0        0        0     5181 2023-11-15 00:54:37.432403 pypath_omnipath-0.16.5/pypath/share/progress.py
--rw-r--r--   0        0        0      194 2023-11-15 00:54:37.439070 pypath_omnipath-0.16.5/pypath/share/session.py
--rw-r--r--   0        0        0      112 2023-11-15 00:54:37.442403 pypath_omnipath-0.16.5/pypath/share/settings.py
--rw-r--r--   0        0        0      465 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.5/pypath/utils/__init__.py
--rw-r--r--   0        0        0    37070 2023-11-15 00:54:37.482403 pypath_omnipath-0.16.5/pypath/utils/go.py
--rw-r--r--   0        0        0      503 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/utils/homology.py
--rw-r--r--   0        0        0   110391 2024-02-04 09:38:13.370082 pypath_omnipath-0.16.5/pypath/utils/mapping.py
--rw-r--r--   0        0        0      605 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.5/pypath/utils/metabo/__init__.py
--rw-r--r--   0        0        0     1413 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.5/pypath/utils/metabo/struct/visual.py
--rw-r--r--   0        0        0    64348 2023-11-15 01:16:43.172484 pypath_omnipath-0.16.5/pypath/utils/orthology.py
--rw-r--r--   0        0        0     5662 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.5/pypath/utils/pdb.py
--rw-r--r--   0        0        0    11702 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.5/pypath/utils/proteomicsdb.py
--rw-r--r--   0        0        0   108984 2023-11-15 01:06:36.305780 pypath_omnipath-0.16.5/pypath/utils/pyreact.py
--rw-r--r--   0        0        0     6577 2023-11-15 00:59:28.489088 pypath_omnipath-0.16.5/pypath/utils/reflists.py
--rw-r--r--   0        0        0     8699 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.5/pypath/utils/residues.py
--rw-r--r--   0        0        0    10600 2023-11-16 03:04:16.587131 pypath_omnipath-0.16.5/pypath/utils/seq.py
--rw-r--r--   0        0        0    11522 2023-11-15 00:54:37.512403 pypath_omnipath-0.16.5/pypath/utils/taxonomy.py
--rw-r--r--   0        0        0    11853 2023-11-15 00:54:37.509070 pypath_omnipath-0.16.5/pypath/utils/unichem.py
--rw-r--r--   0        0        0    17874 2023-11-18 13:41:01.440725 pypath_omnipath-0.16.5/pypath/utils/uniprot.py
--rw-r--r--   0        0        0      466 2023-11-15 00:54:37.375737 pypath_omnipath-0.16.5/pypath/visual/__init__.py
--rw-r--r--   0        0        0    26868 2023-11-15 01:06:09.402445 pypath_omnipath-0.16.5/pypath/visual/drawing.py
--rw-r--r--   0        0        0    20727 2023-11-15 00:54:37.372403 pypath_omnipath-0.16.5/pypath/visual/igraph_drawing/__init__.py
--rw-r--r--   0        0        0    13435 2023-11-15 00:54:37.372403 pypath_omnipath-0.16.5/pypath/visual/igraph_drawing/edge.py
--rw-r--r--   0        0        0     5235 2023-11-15 00:54:37.372403 pypath_omnipath-0.16.5/pypath/visual/igraph_drawing/vertex.py
--rw-r--r--   0        0        0   156062 2023-11-15 00:54:37.379070 pypath_omnipath-0.16.5/pypath/visual/plot.py
--rw-r--r--   0        0        0     3225 2024-02-04 10:05:05.006826 pypath_omnipath-0.16.5/pyproject.toml
--rw-r--r--   0        0        0    13834 1970-01-01 00:00:00.000000 pypath_omnipath-0.16.5/PKG-INFO
+-rw-r--r--   0        0        0    35141 2016-11-05 19:50:35.500333 pypath_omnipath-0.16.9/LICENSE
+-rw-r--r--   0        0        0    11505 2023-06-22 21:35:04.475207 pypath_omnipath-0.16.9/README.rst
+-rw-r--r--   0        0        0     3244 2023-11-30 09:57:24.113869 pypath_omnipath-0.16.9/pypath/__init__.py
+-rw-r--r--   0        0        0     1953 2024-02-19 19:50:19.307297 pypath_omnipath-0.16.9/pypath/_metadata.py
+-rw-r--r--   0        0        0      534 2023-11-15 00:54:37.135737 pypath_omnipath-0.16.9/pypath/biocypher/__init__.py
+-rw-r--r--   0        0        0     7732 2023-11-15 00:54:37.135737 pypath_omnipath-0.16.9/pypath/biocypher/adapter.py
+-rw-r--r--   0        0        0      466 2023-11-15 00:54:37.412403 pypath_omnipath-0.16.9/pypath/core/__init__.py
+-rw-r--r--   0        0        0   174619 2023-11-15 00:54:37.389070 pypath_omnipath-0.16.9/pypath/core/annot.py
+-rw-r--r--   0        0        0     4090 2023-11-15 00:54:37.429070 pypath_omnipath-0.16.9/pypath/core/attrs.py
+-rw-r--r--   0        0        0     4329 2023-11-15 00:54:37.385737 pypath_omnipath-0.16.9/pypath/core/common.py
+-rw-r--r--   0        0        0    18802 2023-11-15 00:54:37.432403 pypath_omnipath-0.16.9/pypath/core/complex.py
+-rw-r--r--   0        0        0    13137 2023-11-15 00:54:37.429070 pypath_omnipath-0.16.9/pypath/core/entity.py
+-rw-r--r--   0        0        0    37304 2023-11-15 00:54:37.429070 pypath_omnipath-0.16.9/pypath/core/enz_sub.py
+-rw-r--r--   0        0        0    22791 2023-11-15 00:54:37.429070 pypath_omnipath-0.16.9/pypath/core/evidence.py
+-rw-r--r--   0        0        0    97860 2023-11-15 00:54:37.382403 pypath_omnipath-0.16.9/pypath/core/interaction.py
+-rw-r--r--   0        0        0    29848 2023-11-15 00:54:37.385737 pypath_omnipath-0.16.9/pypath/core/intercell.py
+-rw-r--r--   0        0        0   230501 2023-11-15 00:54:37.419070 pypath_omnipath-0.16.9/pypath/core/intercell_annot.py
+-rw-r--r--   0        0        0   141652 2023-11-15 00:54:37.422403 pypath_omnipath-0.16.9/pypath/core/network.py
+-rw-r--r--   0        0        0      668 2023-11-30 09:57:24.113869 pypath_omnipath-0.16.9/pypath/data/__init__.py
+-rw-r--r--   0        0        0      917 2023-11-30 09:57:24.113869 pypath_omnipath-0.16.9/pypath/data/_data.py
+-rw-r--r--   0        0        0     1300 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/embl_colors
+-rw-r--r--   0        0        0      271 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/ensembl_biomart_query.xml
+-rw-r--r--   0        0        0      227 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/goose_ancestors.sql
+-rw-r--r--   0        0        0      712 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/goose_annotations.sql
+-rw-r--r--   0        0        0      120 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/goose_terms.sql
+-rw-r--r--   0        0        0      185 2023-06-14 13:36:25.323042 pypath_omnipath-0.16.9/pypath/data/licenses/afl_v3.json
+-rw-r--r--   0        0        0      186 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/apache_2.0.json
+-rw-r--r--   0        0        0      190 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/artistic_2.0.json
+-rw-r--r--   0        0        0      199 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/biocarta.json
+-rw-r--r--   0        0        0      188 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/bsd.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_2.5.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_3.0.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_4.0.json
+-rw-r--r--   0        0        0      242 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nc-nd_3.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.168281 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nc-nd_4.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nc_2.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nc_3.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nc_4.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nc_sa_3.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nc_sa_4.0.json
+-rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nd_3.0.json
+-rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_nd_4.0.json
+-rw-r--r--   0        0        0      224 2023-06-14 13:36:25.323042 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_sa_2.5.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_sa_3.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_by_sa_4.0.json
+-rw-r--r--   0        0        0      233 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cc_zero.json
+-rw-r--r--   0        0        0      196 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cellcellinteractions.json
+-rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/composite.json
+-rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/cosmic.json
+-rw-r--r--   0        0        0      194 2022-03-18 18:18:43.477819 pypath_omnipath-0.16.9/pypath/data/licenses/cytosig.json
+-rw-r--r--   0        0        0      182 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/dsl.json
+-rw-r--r--   0        0        0      185 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/elm.json
+-rw-r--r--   0        0        0      174 2022-12-05 01:12:34.015062 pypath_omnipath-0.16.9/pypath/data/licenses/embl-ebi.json
+-rw-r--r--   0        0        0      212 2023-06-14 13:36:25.326376 pypath_omnipath-0.16.9/pypath/data/licenses/eul.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/gnu_gpl_v2.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/gnu_gpl_v3.json
+-rw-r--r--   0        0        0      200 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/gnu_lgpl_v3.json
+-rw-r--r--   0        0        0      311 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/hgnc.json
+-rw-r--r--   0        0        0      150 2022-09-15 18:20:39.089511 pypath_omnipath-0.16.9/pypath/data/licenses/hpo.json
+-rw-r--r--   0        0        0      139 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/hprd.json
+-rw-r--r--   0        0        0      168 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/i2d.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/informal.json
+-rw-r--r--   0        0        0      175 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/kegg.json
+-rw-r--r--   0        0        0      174 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/kinase-com.json
+-rw-r--r--   0        0        0      268 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/mirecords.json
+-rw-r--r--   0        0        0      184 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/mirtarbase.json
+-rw-r--r--   0        0        0      154 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/mit.json
+-rw-r--r--   0        0        0      165 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/mppi.json
+-rw-r--r--   0        0        0      360 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/nar.json
+-rw-r--r--   0        0        0      179 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/no_license.json
+-rw-r--r--   0        0        0      187 2023-09-11 20:08:33.865064 pypath_omnipath-0.16.9/pypath/data/licenses/opentargets.json
+-rw-r--r--   0        0        0      177 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/pathwaycommons.json
+-rw-r--r--   0        0        0      351 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/pdb.json
+-rw-r--r--   0        0        0      363 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/phosphonetworks.json
+-rw-r--r--   0        0        0      464 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/licenses/unspecified.json
+-rw-r--r--   0        0        0     1150 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/www/favicon.ico
+-rw-r--r--   0        0        0      486 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/www/http500.html
+-rw-r--r--   0        0        0      324 2022-01-24 11:42:01.171614 pypath_omnipath-0.16.9/pypath/data/www/index.html
+-rw-r--r--   0        0        0     5712 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.9/pypath/formats/obo.py
+-rw-r--r--   0        0        0    15803 2023-11-30 09:57:24.113869 pypath_omnipath-0.16.9/pypath/formats/sdf.py
+-rw-r--r--   0        0        0     8487 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.9/pypath/formats/sqldump.py
+-rw-r--r--   0        0        0     1221 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.9/pypath/formats/sqlite.py
+-rw-r--r--   0        0        0     7413 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.9/pypath/formats/xml.py
+-rw-r--r--   0        0        0     2085 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.9/pypath/inputs/__init__.py
+-rw-r--r--   0        0        0      972 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.9/pypath/inputs/abs.py
+-rw-r--r--   0        0        0     3052 2023-11-15 00:54:37.325737 pypath_omnipath-0.16.9/pypath/inputs/acsn.py
+-rw-r--r--   0        0        0     2263 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.9/pypath/inputs/adhesome.py
+-rw-r--r--   0        0        0     4936 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.9/pypath/inputs/adrecs.py
+-rw-r--r--   0        0        0     2240 2023-11-15 00:54:37.159070 pypath_omnipath-0.16.9/pypath/inputs/almen2009.py
+-rw-r--r--   0        0        0     5184 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.9/pypath/inputs/baccin2019.py
+-rw-r--r--   0        0        0     6216 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.9/pypath/inputs/biogps.py
+-rw-r--r--   0        0        0     4889 2023-11-15 00:54:37.262403 pypath_omnipath-0.16.9/pypath/inputs/biogrid.py
+-rw-r--r--   0        0        0    10274 2024-02-19 15:57:30.860598 pypath_omnipath-0.16.9/pypath/inputs/biomart.py
+-rw-r--r--   0        0        0     5262 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.9/pypath/inputs/biomodels.py
+-rw-r--r--   0        0        0     1691 2023-11-15 00:54:37.162403 pypath_omnipath-0.16.9/pypath/inputs/ca1.py
+-rw-r--r--   0        0        0     2657 2023-11-15 00:54:37.219070 pypath_omnipath-0.16.9/pypath/inputs/cancercellmap.py
+-rw-r--r--   0        0        0     5490 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.9/pypath/inputs/cancerdrugsdb.py
+-rw-r--r--   0        0        0     1804 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.9/pypath/inputs/cancersea.py
+-rw-r--r--   0        0        0     3255 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.9/pypath/inputs/cell.py
+-rw-r--r--   0        0        0     6235 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.9/pypath/inputs/cellcall.py
+-rw-r--r--   0        0        0     1448 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.9/pypath/inputs/cellcellinteractions.py
+-rw-r--r--   0        0        0     9032 2023-11-15 00:54:37.179070 pypath_omnipath-0.16.9/pypath/inputs/cellchatdb.py
+-rw-r--r--   0        0        0    14933 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.9/pypath/inputs/cellinker.py
+-rw-r--r--   0        0        0     9192 2024-02-19 15:57:30.860598 pypath_omnipath-0.16.9/pypath/inputs/cellphonedb.py
+-rw-r--r--   0        0        0     5238 2023-11-15 00:54:37.302403 pypath_omnipath-0.16.9/pypath/inputs/celltalkdb.py
+-rw-r--r--   0        0        0     2097 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.9/pypath/inputs/celltypist.py
+-rw-r--r--   0        0        0    13772 2023-11-15 00:54:37.295737 pypath_omnipath-0.16.9/pypath/inputs/chembl.py
+-rw-r--r--   0        0        0     3841 2023-11-15 00:54:37.312403 pypath_omnipath-0.16.9/pypath/inputs/clinvar.py
+-rw-r--r--   0        0        0     5525 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.9/pypath/inputs/collectri.py
+-rw-r--r--   0        0        0     8341 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.9/pypath/inputs/common.py
+-rw-r--r--   0        0        0     2412 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.9/pypath/inputs/compath.py
+-rw-r--r--   0        0        0     2553 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.9/pypath/inputs/compleat.py
+-rw-r--r--   0        0        0     4406 2023-11-15 00:54:37.309070 pypath_omnipath-0.16.9/pypath/inputs/complexportal.py
+-rw-r--r--   0        0        0     3933 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.9/pypath/inputs/comppi.py
+-rw-r--r--   0        0        0     2685 2023-11-15 00:54:37.259070 pypath_omnipath-0.16.9/pypath/inputs/connectomedb.py
+-rw-r--r--   0        0        0     2690 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.9/pypath/inputs/corum.py
+-rw-r--r--   0        0        0     4676 2023-11-15 00:54:37.329070 pypath_omnipath-0.16.9/pypath/inputs/cosmic.py
+-rw-r--r--   0        0        0     4061 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.9/pypath/inputs/cpad.py
+-rw-r--r--   0        0        0     1886 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.9/pypath/inputs/cpdb.py
+-rw-r--r--   0        0        0     3309 2023-11-15 00:54:37.312403 pypath_omnipath-0.16.9/pypath/inputs/credentials.py
+-rw-r--r--   0        0        0     3241 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.9/pypath/inputs/csa.py
+-rw-r--r--   0        0        0     3444 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.9/pypath/inputs/cspa.py
+-rw-r--r--   0        0        0     4976 2023-11-15 00:54:37.295737 pypath_omnipath-0.16.9/pypath/inputs/ctdbase.py
+-rw-r--r--   0        0        0     3240 2023-11-15 00:54:37.145737 pypath_omnipath-0.16.9/pypath/inputs/cytosig.py
+-rw-r--r--   0        0        0     4662 2023-11-15 00:54:37.172403 pypath_omnipath-0.16.9/pypath/inputs/dbptm.py
+-rw-r--r--   0        0        0     5188 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.9/pypath/inputs/ddinter.py
+-rw-r--r--   0        0        0     2734 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.9/pypath/inputs/deathdomain.py
+-rw-r--r--   0        0        0     4281 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.9/pypath/inputs/depod.py
+-rw-r--r--   0        0        0     3589 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.9/pypath/inputs/dgidb.py
+-rw-r--r--   0        0        0     4851 2023-11-15 00:54:37.175737 pypath_omnipath-0.16.9/pypath/inputs/dip.py
+-rw-r--r--   0        0        0     5635 2024-02-19 15:57:30.863932 pypath_omnipath-0.16.9/pypath/inputs/diseases.py
+-rw-r--r--   0        0        0      592 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/__init__.py
+-rw-r--r--   0        0        0      671 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_api/__init__.py
+-rw-r--r--   0        0        0     6335 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_api/meta.py
+-rw-r--r--   0        0        0     5726 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_api/schema.py
+-rw-r--r--   0        0        0     4949 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_api/simple.py
+-rw-r--r--   0        0        0     3522 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_auth.py
+-rw-r--r--   0        0        0     1925 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_client.py
+-rw-r--r--   0        0        0     2587 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_field.py
+-rw-r--r--   0        0        0     2355 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_proc.py
+-rw-r--r--   0        0        0     2109 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_records.py
+-rw-r--r--   0        0        0     6242 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_request.py
+-rw-r--r--   0        0        0     1548 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_schema.py
+-rw-r--r--   0        0        0     2604 2023-11-15 00:54:37.202403 pypath_omnipath-0.16.9/pypath/inputs/disgenet/_valid.py
+-rw-r--r--   0        0        0    17032 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.9/pypath/inputs/domino.py
+-rw-r--r--   0        0        0    12556 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.9/pypath/inputs/dorothea.py
+-rw-r--r--   0        0        0    20545 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.9/pypath/inputs/drugbank.py
+-rw-r--r--   0        0        0     4575 2023-11-15 00:54:37.309070 pypath_omnipath-0.16.9/pypath/inputs/drugcentral.py
+-rw-r--r--   0        0        0     4696 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.9/pypath/inputs/ebi.py
+-rw-r--r--   0        0        0     4826 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.9/pypath/inputs/elm.py
+-rw-r--r--   0        0        0     2420 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.9/pypath/inputs/embopress.py
+-rw-r--r--   0        0        0     4424 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.9/pypath/inputs/embrace.py
+-rw-r--r--   0        0        0     1117 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.9/pypath/inputs/encode.py
+-rw-r--r--   0        0        0     1879 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.9/pypath/inputs/ensembl.py
+-rw-r--r--   0        0        0     3134 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.9/pypath/inputs/eutils.py
+-rw-r--r--   0        0        0     3049 2023-11-15 00:54:37.322404 pypath_omnipath-0.16.9/pypath/inputs/exocarta.py
+-rw-r--r--   0        0        0     3179 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.9/pypath/inputs/expasy.py
+-rw-r--r--   0        0        0     3322 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.9/pypath/inputs/genecards.py
+-rw-r--r--   0        0        0    25944 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.9/pypath/inputs/go.py
+-rw-r--r--   0        0        0     2253 2023-11-15 00:54:37.312403 pypath_omnipath-0.16.9/pypath/inputs/gpcrdb.py
+-rw-r--r--   0        0        0     1834 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.9/pypath/inputs/graphviz.py
+-rw-r--r--   0        0        0     8158 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.9/pypath/inputs/guide2pharma.py
+-rw-r--r--   0        0        0     3448 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.9/pypath/inputs/gutmgene.py
+-rw-r--r--   0        0        0     1494 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.9/pypath/inputs/havugimana.py
+-rw-r--r--   0        0        0     1525 2023-11-15 00:54:37.239070 pypath_omnipath-0.16.9/pypath/inputs/hgnc.py
+-rw-r--r--   0        0        0     3660 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.9/pypath/inputs/hippie.py
+-rw-r--r--   0        0        0     1075 2023-11-15 00:54:37.242403 pypath_omnipath-0.16.9/pypath/inputs/hmdb/__init__.py
+-rw-r--r--   0        0        0     6310 2023-11-15 00:54:37.239070 pypath_omnipath-0.16.9/pypath/inputs/hmdb/common.py
+-rw-r--r--   0        0        0     5066 2023-11-15 00:54:37.239070 pypath_omnipath-0.16.9/pypath/inputs/hmdb/metabolites.py
+-rw-r--r--   0        0        0     5019 2023-11-15 00:54:37.242403 pypath_omnipath-0.16.9/pypath/inputs/hmdb/proteins.py
+-rw-r--r--   0        0        0      579 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.9/pypath/inputs/hmdb/schema/__init__.py
+-rw-r--r--   0        0        0     2196 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.9/pypath/inputs/hmdb/schema/common.py
+-rw-r--r--   0        0        0     5002 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.9/pypath/inputs/hmdb/schema/metabolites.py
+-rw-r--r--   0        0        0     2871 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.9/pypath/inputs/hmdb/schema/proteins.py
+-rw-r--r--   0        0        0     1168 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.9/pypath/inputs/hmdb/structures.py
+-rw-r--r--   0        0        0     1591 2023-11-15 00:54:37.245737 pypath_omnipath-0.16.9/pypath/inputs/hmdb/visual.py
+-rw-r--r--   0        0        0     1189 2023-11-15 00:54:37.242403 pypath_omnipath-0.16.9/pypath/inputs/hmdb/xml.py
+-rw-r--r--   0        0        0     4705 2024-02-19 15:57:30.863932 pypath_omnipath-0.16.9/pypath/inputs/homologene.py
+-rw-r--r--   0        0        0    10232 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.9/pypath/inputs/hpmr.py
+-rw-r--r--   0        0        0     4943 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.9/pypath/inputs/hpo.py
+-rw-r--r--   0        0        0     2645 2023-11-15 00:54:37.172403 pypath_omnipath-0.16.9/pypath/inputs/hprd.py
+-rw-r--r--   0        0        0     1388 2023-11-15 00:54:37.219070 pypath_omnipath-0.16.9/pypath/inputs/htri.py
+-rw-r--r--   0        0        0     1669 2023-11-15 00:54:37.302403 pypath_omnipath-0.16.9/pypath/inputs/humancellmap.py
+-rw-r--r--   0        0        0     1945 2023-11-15 00:54:37.309070 pypath_omnipath-0.16.9/pypath/inputs/humap.py
+-rw-r--r--   0        0        0     2189 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.9/pypath/inputs/humsavar.py
+-rw-r--r--   0        0        0     7990 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.9/pypath/inputs/huri.py
+-rw-r--r--   0        0        0     2562 2023-11-15 00:54:37.179070 pypath_omnipath-0.16.9/pypath/inputs/i3d.py
+-rw-r--r--   0        0        0     6610 2023-11-15 00:54:37.175737 pypath_omnipath-0.16.9/pypath/inputs/icellnet.py
+-rw-r--r--   0        0        0     8010 2023-11-15 00:54:37.259070 pypath_omnipath-0.16.9/pypath/inputs/ielm.py
+-rw-r--r--   0        0        0     3811 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.9/pypath/inputs/imweb.py
+-rw-r--r--   0        0        0     2139 2023-11-15 00:54:37.172403 pypath_omnipath-0.16.9/pypath/inputs/innatedb.py
+-rw-r--r--   0        0        0     2902 2023-11-15 00:54:37.329070 pypath_omnipath-0.16.9/pypath/inputs/instruct.py
+-rw-r--r--   0        0        0     5561 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.9/pypath/inputs/intact.py
+-rw-r--r--   0        0        0     1638 2023-11-15 00:54:37.179070 pypath_omnipath-0.16.9/pypath/inputs/integrins.py
+-rw-r--r--   0        0        0     8739 2023-11-15 00:54:37.262403 pypath_omnipath-0.16.9/pypath/inputs/interpro.py
+-rw-r--r--   0        0        0     2427 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.9/pypath/inputs/intogen.py
+-rw-r--r--   0        0        0     1605 2023-11-15 00:54:37.262403 pypath_omnipath-0.16.9/pypath/inputs/ipi.py
+-rw-r--r--   0        0        0     3462 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.9/pypath/inputs/iptmnet.py
+-rw-r--r--   0        0        0     3033 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.9/pypath/inputs/italk.py
+-rw-r--r--   0        0        0     2454 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.9/pypath/inputs/kea.py
+-rw-r--r--   0        0        0    20520 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.9/pypath/inputs/kegg.py
+-rw-r--r--   0        0        0    15410 2023-11-15 00:54:37.259070 pypath_omnipath-0.16.9/pypath/inputs/kegg_api.py
+-rw-r--r--   0        0        0     1829 2023-11-15 00:54:37.219070 pypath_omnipath-0.16.9/pypath/inputs/kinasedotcom.py
+-rw-r--r--   0        0        0     2419 2023-11-15 00:54:37.172403 pypath_omnipath-0.16.9/pypath/inputs/kirouac2010.py
+-rw-r--r--   0        0        0     4224 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.9/pypath/inputs/lambert2018.py
+-rw-r--r--   0        0        0     2071 2023-11-15 00:54:37.159070 pypath_omnipath-0.16.9/pypath/inputs/laudanna.py
+-rw-r--r--   0        0        0     5534 2023-11-15 00:54:37.142403 pypath_omnipath-0.16.9/pypath/inputs/li2012.py
+-rw-r--r--   0        0        0     2522 2023-11-15 00:54:37.265737 pypath_omnipath-0.16.9/pypath/inputs/lincs.py
+-rw-r--r--   0        0        0      494 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.9/pypath/inputs/lipidmaps/__init__.py
+-rw-r--r--   0        0        0     1246 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.9/pypath/inputs/lipidmaps/structures.py
+-rw-r--r--   0        0        0     2823 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.9/pypath/inputs/lmpid.py
+-rw-r--r--   0        0        0     1508 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.9/pypath/inputs/lncdisease.py
+-rw-r--r--   0        0        0     2003 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.9/pypath/inputs/lncrnadb.py
+-rw-r--r--   0        0        0     7781 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.9/pypath/inputs/locate.py
+-rw-r--r--   0        0        0     3489 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.9/pypath/inputs/lrdb.py
+-rw-r--r--   0        0        0     2804 2023-11-15 00:54:37.319070 pypath_omnipath-0.16.9/pypath/inputs/macrophage.py
+-rw-r--r--   0        0        0      468 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.9/pypath/inputs/main.py
+-rw-r--r--   0        0        0     2231 2023-11-15 00:54:37.219070 pypath_omnipath-0.16.9/pypath/inputs/matrisome.py
+-rw-r--r--   0        0        0     4065 2023-11-15 00:54:37.302403 pypath_omnipath-0.16.9/pypath/inputs/matrixdb.py
+-rw-r--r--   0        0        0     1004 2023-11-15 00:54:37.152403 pypath_omnipath-0.16.9/pypath/inputs/mcam.py
+-rw-r--r--   0        0        0     1885 2023-11-15 00:54:37.329070 pypath_omnipath-0.16.9/pypath/inputs/membranome.py
+-rw-r--r--   0        0        0     4193 2023-11-15 00:54:37.319070 pypath_omnipath-0.16.9/pypath/inputs/mimp.py
+-rw-r--r--   0        0        0     1262 2023-11-15 00:54:37.325737 pypath_omnipath-0.16.9/pypath/inputs/mir2disease.py
+-rw-r--r--   0        0        0     3779 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.9/pypath/inputs/mirbase.py
+-rw-r--r--   0        0        0     1639 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.9/pypath/inputs/mirdeathdb.py
+-rw-r--r--   0        0        0     1655 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.9/pypath/inputs/mirecords.py
+-rw-r--r--   0        0        0     2231 2023-11-15 00:54:37.322404 pypath_omnipath-0.16.9/pypath/inputs/mirtarbase.py
+-rw-r--r--   0        0        0      968 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.9/pypath/inputs/mitab.py
+-rw-r--r--   0        0        0     3063 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.9/pypath/inputs/mppi.py
+-rw-r--r--   0        0        0    11388 2023-11-15 00:54:37.185737 pypath_omnipath-0.16.9/pypath/inputs/msigdb.py
+-rw-r--r--   0        0        0     1997 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.9/pypath/inputs/ncrdeathdb.py
+-rw-r--r--   0        0        0     1727 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.9/pypath/inputs/negatome.py
+-rw-r--r--   0        0        0     1655 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.9/pypath/inputs/netbiol.py
+-rw-r--r--   0        0        0     6273 2023-11-15 00:54:37.175737 pypath_omnipath-0.16.9/pypath/inputs/netpath.py
+-rw-r--r--   0        0        0     1862 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.9/pypath/inputs/offsides.py
+-rw-r--r--   0        0        0     7220 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.9/pypath/inputs/oma.py
+-rw-r--r--   0        0        0     3497 2023-11-15 00:54:37.159070 pypath_omnipath-0.16.9/pypath/inputs/ontology.py
+-rw-r--r--   0        0        0     6747 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.9/pypath/inputs/opentargets.py
+-rw-r--r--   0        0        0     2742 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.9/pypath/inputs/opm.py
+-rw-r--r--   0        0        0     2210 2023-11-15 00:54:37.299070 pypath_omnipath-0.16.9/pypath/inputs/oreganno.py
+-rw-r--r--   0        0        0     3900 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.9/pypath/inputs/panglaodb.py
+-rw-r--r--   0        0        0     3426 2023-11-15 00:54:37.145737 pypath_omnipath-0.16.9/pypath/inputs/pathophenodb.py
+-rw-r--r--   0        0        0     4465 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.9/pypath/inputs/pathwaycommons.py
+-rw-r--r--   0        0        0      968 2023-11-15 00:54:37.222403 pypath_omnipath-0.16.9/pypath/inputs/pazar.py
+-rw-r--r--   0        0        0     6230 2023-11-15 00:54:37.165737 pypath_omnipath-0.16.9/pypath/inputs/pdb.py
+-rw-r--r--   0        0        0     2308 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.9/pypath/inputs/pdzbase.py
+-rw-r--r--   0        0        0     6557 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.9/pypath/inputs/pepcyber.py
+-rw-r--r--   0        0        0     8994 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.9/pypath/inputs/pfam.py
+-rw-r--r--   0        0        0     6485 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.9/pypath/inputs/pharos.py
+-rw-r--r--   0        0        0     1514 2023-11-15 00:54:37.175737 pypath_omnipath-0.16.9/pypath/inputs/phobius.py
+-rw-r--r--   0        0        0     2196 2023-11-15 00:54:37.209070 pypath_omnipath-0.16.9/pypath/inputs/phosphatome.py
+-rw-r--r--   0        0        0     3330 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.9/pypath/inputs/phosphoelm.py
+-rw-r--r--   0        0        0     2097 2023-11-15 00:54:37.169070 pypath_omnipath-0.16.9/pypath/inputs/phosphonetworks.py
+-rw-r--r--   0        0        0     1196 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.9/pypath/inputs/phosphopoint.py
+-rw-r--r--   0        0        0    37214 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.9/pypath/inputs/phosphosite.py
+-rw-r--r--   0        0        0     9873 2023-11-15 00:54:37.162403 pypath_omnipath-0.16.9/pypath/inputs/pisa.py
+-rw-r--r--   0        0        0     1747 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.9/pypath/inputs/pro.py
+-rw-r--r--   0        0        0     3086 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.9/pypath/inputs/progeny.py
+-rw-r--r--   0        0        0     7428 2023-11-15 00:54:37.299070 pypath_omnipath-0.16.9/pypath/inputs/proteinatlas.py
+-rw-r--r--   0        0        0     3470 2023-11-15 00:54:37.255737 pypath_omnipath-0.16.9/pypath/inputs/proteins.py
+-rw-r--r--   0        0        0     3705 2023-11-15 00:54:37.229070 pypath_omnipath-0.16.9/pypath/inputs/protmapper.py
+-rw-r--r--   0        0        0     2360 2023-11-15 00:54:37.315737 pypath_omnipath-0.16.9/pypath/inputs/pubchem.py
+-rw-r--r--   0        0        0     3453 2023-11-15 00:54:37.249070 pypath_omnipath-0.16.9/pypath/inputs/pubmed.py
+-rw-r--r--   0        0        0     4315 2023-11-15 00:54:37.239070 pypath_omnipath-0.16.9/pypath/inputs/ramilowski2015.py
+-rw-r--r--   0        0        0     5289 2023-11-15 00:54:37.159070 pypath_omnipath-0.16.9/pypath/inputs/ramp.py
+-rw-r--r--   0        0        0     6393 2023-11-15 00:54:37.232403 pypath_omnipath-0.16.9/pypath/inputs/rdata.py
+-rw-r--r--   0        0        0    40019 2023-11-15 00:54:37.162403 pypath_omnipath-0.16.9/pypath/inputs/reaction.py
+-rw-r--r--   0        0        0     3714 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.9/pypath/inputs/reactome.py
+-rw-r--r--   0        0        0     7578 2023-11-15 00:54:37.225737 pypath_omnipath-0.16.9/pypath/inputs/scconnect.py
+-rw-r--r--   0        0        0     2352 2023-11-15 00:54:37.152403 pypath_omnipath-0.16.9/pypath/inputs/science.py
+-rw-r--r--   0        0        0     4356 2023-11-15 00:54:37.192403 pypath_omnipath-0.16.9/pypath/inputs/sider.py
+-rw-r--r--   0        0        0     5475 2023-11-15 00:54:37.319070 pypath_omnipath-0.16.9/pypath/inputs/signalink.py
+-rw-r--r--   0        0        0    11624 2023-11-15 00:54:37.262403 pypath_omnipath-0.16.9/pypath/inputs/signor.py
+-rw-r--r--   0        0        0     5578 2023-11-15 00:54:37.145737 pypath_omnipath-0.16.9/pypath/inputs/spike.py
+-rw-r--r--   0        0        0     4160 2023-11-15 00:54:37.195737 pypath_omnipath-0.16.9/pypath/inputs/stitch.py
+-rw-r--r--   0        0        0     7188 2023-11-15 00:54:37.179070 pypath_omnipath-0.16.9/pypath/inputs/string.py
+-rw-r--r--   0        0        0     1476 2023-11-15 00:54:37.322404 pypath_omnipath-0.16.9/pypath/inputs/surfaceome.py
+-rw-r--r--   0        0        0     4309 2023-11-15 00:54:37.155737 pypath_omnipath-0.16.9/pypath/inputs/switches_elm.py
+-rw-r--r--   0        0        0     3122 2023-11-15 00:54:37.299070 pypath_omnipath-0.16.9/pypath/inputs/talklr.py
+-rw-r--r--   0        0        0     2513 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.9/pypath/inputs/tcdb.py
+-rw-r--r--   0        0        0     2016 2023-11-15 00:54:37.235737 pypath_omnipath-0.16.9/pypath/inputs/tfcensus.py
+-rw-r--r--   0        0        0     7823 2023-11-15 00:54:37.205737 pypath_omnipath-0.16.9/pypath/inputs/threedcomplex.py
+-rw-r--r--   0        0        0    17262 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.9/pypath/inputs/threedid.py
+-rw-r--r--   0        0        0     3589 2023-11-15 00:54:37.149070 pypath_omnipath-0.16.9/pypath/inputs/topdb.py
+-rw-r--r--   0        0        0     1350 2023-11-15 00:54:37.352403 pypath_omnipath-0.16.9/pypath/inputs/transmir.py
+-rw-r--r--   0        0        0     9801 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.9/pypath/inputs/trip.py
+-rw-r--r--   0        0        0     2158 2023-11-15 00:54:37.145737 pypath_omnipath-0.16.9/pypath/inputs/trrust.py
+-rw-r--r--   0        0        0     1384 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.9/pypath/inputs/twosides.py
+-rw-r--r--   0        0        0     5093 2023-11-15 00:54:37.252403 pypath_omnipath-0.16.9/pypath/inputs/unichem.py
+-rw-r--r--   0        0        0    46655 2023-11-18 00:12:01.136439 pypath_omnipath-0.16.9/pypath/inputs/uniprot.py
+-rw-r--r--   0        0        0     3418 2023-11-15 00:54:37.182403 pypath_omnipath-0.16.9/pypath/inputs/uniprot_db.py
+-rw-r--r--   0        0        0     7499 2023-11-15 00:54:37.215737 pypath_omnipath-0.16.9/pypath/inputs/wang.py
+-rw-r--r--   0        0        0     2068 2023-11-15 00:54:37.212403 pypath_omnipath-0.16.9/pypath/inputs/wojtowicz2020.py
+-rw-r--r--   0        0        0     1516 2023-11-15 00:54:37.162403 pypath_omnipath-0.16.9/pypath/inputs/zhong2015.py
+-rw-r--r--   0        0        0      466 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.9/pypath/internals/__init__.py
+-rw-r--r--   0        0        0    11713 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.9/pypath/internals/annot_formats.py
+-rw-r--r--   0        0        0    25898 2024-02-19 19:49:54.167296 pypath_omnipath-0.16.9/pypath/internals/input_formats.py
+-rw-r--r--   0        0        0    43659 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.9/pypath/internals/intera.py
+-rw-r--r--   0        0        0     7416 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.9/pypath/internals/license.py
+-rw-r--r--   0        0        0     4558 2024-02-19 19:49:54.170629 pypath_omnipath-0.16.9/pypath/internals/maps.py
+-rw-r--r--   0        0        0     4102 2023-11-15 00:54:37.469070 pypath_omnipath-0.16.9/pypath/internals/refs.py
+-rw-r--r--   0        0        0    13178 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.9/pypath/internals/resource.py
+-rw-r--r--   0        0        0      466 2023-11-15 00:54:37.352403 pypath_omnipath-0.16.9/pypath/legacy/__init__.py
+-rw-r--r--   0        0        0     4421 2023-11-15 00:54:37.369070 pypath_omnipath-0.16.9/pypath/legacy/db_categories.py
+-rw-r--r--   0        0        0   556333 2023-11-15 00:54:37.369070 pypath_omnipath-0.16.9/pypath/legacy/main.py
+-rw-r--r--   0        0        0     1580 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/__init__.py
+-rw-r--r--   0        0        0    17814 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/app.py
+-rw-r--r--   0        0        0    16762 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/bel.py
+-rw-r--r--   0        0        0    16578 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/cellphonedb.py
+-rw-r--r--   0        0        0     1290 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/databases/__init__.py
+-rw-r--r--   0        0        0     1660 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/databases/build.py
+-rw-r--r--   0        0        0     1729 2022-12-05 01:12:34.028395 pypath_omnipath-0.16.9/pypath/omnipath/databases/builtins.json
+-rw-r--r--   0        0        0      522 2022-01-24 11:42:01.191613 pypath_omnipath-0.16.9/pypath/omnipath/databases/classes.json
+-rw-r--r--   0        0        0     7366 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/databases/define.py
+-rw-r--r--   0        0        0    30885 2023-11-15 00:55:01.929072 pypath_omnipath-0.16.9/pypath/omnipath/export.py
+-rw-r--r--   0        0        0     4076 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/legacy.py
+-rw-r--r--   0        0        0     1605 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/omnipath/param.py
+-rw-r--r--   0        0        0      466 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.9/pypath/omnipath/server/__init__.py
+-rw-r--r--   0        0        0   122710 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.9/pypath/omnipath/server/_html.py
+-rw-r--r--   0        0        0    10404 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.9/pypath/omnipath/server/build.py
+-rw-r--r--   0        0        0    17053 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.9/pypath/omnipath/server/generate_about_page.py
+-rw-r--r--   0        0        0    11019 2023-11-15 00:54:37.472403 pypath_omnipath-0.16.9/pypath/omnipath/server/legacy.py
+-rw-r--r--   0        0        0    79455 2024-02-19 15:57:30.863932 pypath_omnipath-0.16.9/pypath/omnipath/server/run.py
+-rw-r--r--   0        0        0     4209 2023-11-15 00:54:37.519070 pypath_omnipath-0.16.9/pypath/reader/field.py
+-rw-r--r--   0        0        0     1517 2023-11-15 00:54:37.519070 pypath_omnipath-0.16.9/pypath/reader/network.py
+-rw-r--r--   0        0        0      914 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.9/pypath/resources/__init__.py
+-rw-r--r--   0        0        0    14134 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.9/pypath/resources/controller.py
+-rw-r--r--   0        0        0      466 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.9/pypath/resources/data/__init__.py
+-rw-r--r--   0        0        0      139 2023-01-10 18:56:49.559042 pypath_omnipath-0.16.9/pypath/resources/data/complex_input_template.json
+-rw-r--r--   0        0        0      239 2023-01-10 18:56:35.023580 pypath_omnipath-0.16.9/pypath/resources/data/enz_sub_input_template.json
+-rw-r--r--   0        0        0   179340 2023-09-11 20:49:37.078549 pypath_omnipath-0.16.9/pypath/resources/data/resources.json
+-rw-r--r--   0        0        0   100623 2024-02-19 15:57:30.863932 pypath_omnipath-0.16.9/pypath/resources/data_formats.py
+-rw-r--r--   0        0        0   178871 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.9/pypath/resources/descriptions.py
+-rw-r--r--   0        0        0     2629 2023-11-15 00:54:37.519070 pypath_omnipath-0.16.9/pypath/resources/licenses.py
+-rw-r--r--   0        0        0     5620 2023-11-15 00:54:37.515737 pypath_omnipath-0.16.9/pypath/resources/network.py
+-rw-r--r--   0        0        0    77331 2024-02-19 15:57:30.867265 pypath_omnipath-0.16.9/pypath/resources/urls.py
+-rw-r--r--   0        0        0      465 2023-11-15 00:54:37.439070 pypath_omnipath-0.16.9/pypath/share/__init__.py
+-rw-r--r--   0        0        0     1844 2023-11-18 21:10:57.369047 pypath_omnipath-0.16.9/pypath/share/cache.py
+-rw-r--r--   0        0        0      500 2023-11-15 00:54:37.439070 pypath_omnipath-0.16.9/pypath/share/common.py
+-rw-r--r--   0        0        0      505 2023-11-15 00:54:37.439070 pypath_omnipath-0.16.9/pypath/share/constants.py
+-rw-r--r--   0        0        0    56969 2023-11-15 01:04:39.212440 pypath_omnipath-0.16.9/pypath/share/curl.py
+-rw-r--r--   0        0        0    17263 2023-11-15 00:54:37.435737 pypath_omnipath-0.16.9/pypath/share/lookup/_manytomany.py
+-rw-r--r--   0        0        0     1885 2023-11-15 00:54:37.435737 pypath_omnipath-0.16.9/pypath/share/lookup/_onetomany.py
+-rw-r--r--   0        0        0     2422 2023-11-15 00:54:37.432403 pypath_omnipath-0.16.9/pypath/share/lookup/_onetomany2.py
+-rw-r--r--   0        0        0     5181 2023-11-15 00:54:37.432403 pypath_omnipath-0.16.9/pypath/share/progress.py
+-rw-r--r--   0        0        0      194 2023-11-15 00:54:37.439070 pypath_omnipath-0.16.9/pypath/share/session.py
+-rw-r--r--   0        0        0      112 2023-11-15 00:54:37.442403 pypath_omnipath-0.16.9/pypath/share/settings.py
+-rw-r--r--   0        0        0      465 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.9/pypath/utils/__init__.py
+-rw-r--r--   0        0        0    37070 2023-11-15 00:54:37.482403 pypath_omnipath-0.16.9/pypath/utils/go.py
+-rw-r--r--   0        0        0      503 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/utils/homology.py
+-rw-r--r--   0        0        0   110391 2024-02-19 19:49:54.170629 pypath_omnipath-0.16.9/pypath/utils/mapping.py
+-rw-r--r--   0        0        0      605 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.9/pypath/utils/metabo/__init__.py
+-rw-r--r--   0        0        0     1413 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.9/pypath/utils/metabo/struct/visual.py
+-rw-r--r--   0        0        0    64348 2023-11-15 01:16:43.172484 pypath_omnipath-0.16.9/pypath/utils/orthology.py
+-rw-r--r--   0        0        0     5662 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.9/pypath/utils/pdb.py
+-rw-r--r--   0        0        0    11702 2023-11-15 00:54:37.475737 pypath_omnipath-0.16.9/pypath/utils/proteomicsdb.py
+-rw-r--r--   0        0        0   108984 2023-11-15 01:06:36.305780 pypath_omnipath-0.16.9/pypath/utils/pyreact.py
+-rw-r--r--   0        0        0     6577 2023-11-15 00:59:28.489088 pypath_omnipath-0.16.9/pypath/utils/reflists.py
+-rw-r--r--   0        0        0     8699 2023-11-15 00:54:37.479070 pypath_omnipath-0.16.9/pypath/utils/residues.py
+-rw-r--r--   0        0        0    10600 2023-11-16 03:04:16.587131 pypath_omnipath-0.16.9/pypath/utils/seq.py
+-rw-r--r--   0        0        0    11522 2023-11-15 00:54:37.512403 pypath_omnipath-0.16.9/pypath/utils/taxonomy.py
+-rw-r--r--   0        0        0    11853 2023-11-15 00:54:37.509070 pypath_omnipath-0.16.9/pypath/utils/unichem.py
+-rw-r--r--   0        0        0    17874 2023-11-18 13:41:01.440725 pypath_omnipath-0.16.9/pypath/utils/uniprot.py
+-rw-r--r--   0        0        0      466 2023-11-15 00:54:37.375737 pypath_omnipath-0.16.9/pypath/visual/__init__.py
+-rw-r--r--   0        0        0    26868 2023-11-15 01:06:09.402445 pypath_omnipath-0.16.9/pypath/visual/drawing.py
+-rw-r--r--   0        0        0    20727 2023-11-15 00:54:37.372403 pypath_omnipath-0.16.9/pypath/visual/igraph_drawing/__init__.py
+-rw-r--r--   0        0        0    13435 2023-11-15 00:54:37.372403 pypath_omnipath-0.16.9/pypath/visual/igraph_drawing/edge.py
+-rw-r--r--   0        0        0     5235 2023-11-15 00:54:37.372403 pypath_omnipath-0.16.9/pypath/visual/igraph_drawing/vertex.py
+-rw-r--r--   0        0        0   156062 2023-11-15 00:54:37.379070 pypath_omnipath-0.16.9/pypath/visual/plot.py
+-rw-r--r--   0        0        0     3225 2024-02-19 19:50:19.303964 pypath_omnipath-0.16.9/pyproject.toml
+-rw-r--r--   0        0        0    13834 1970-01-01 00:00:00.000000 pypath_omnipath-0.16.9/PKG-INFO
```

### Comparing `pypath_omnipath-0.16.5/LICENSE` & `pypath_omnipath-0.16.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/README.rst` & `pypath_omnipath-0.16.9/README.rst`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/__init__.py` & `pypath_omnipath-0.16.9/pypath/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/_metadata.py` & `pypath_omnipath-0.16.9/pypath/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 import os
 import pathlib
 import importlib.metadata
 
 import toml
 
-_VERSION = '0.16.5'
+_VERSION = '0.16.9'
 
 
 def get_metadata():
     """
     Basic package metadata.
 
     Retrieves package metadata from the current project directory or from
```

### Comparing `pypath_omnipath-0.16.5/pypath/biocypher/__init__.py` & `pypath_omnipath-0.16.9/pypath/biocypher/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/biocypher/adapter.py` & `pypath_omnipath-0.16.9/pypath/biocypher/adapter.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/annot.py` & `pypath_omnipath-0.16.9/pypath/core/annot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/attrs.py` & `pypath_omnipath-0.16.9/pypath/core/attrs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/common.py` & `pypath_omnipath-0.16.9/pypath/core/common.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/complex.py` & `pypath_omnipath-0.16.9/pypath/core/complex.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/entity.py` & `pypath_omnipath-0.16.9/pypath/core/entity.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/enz_sub.py` & `pypath_omnipath-0.16.9/pypath/core/enz_sub.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/evidence.py` & `pypath_omnipath-0.16.9/pypath/core/evidence.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/interaction.py` & `pypath_omnipath-0.16.9/pypath/core/interaction.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/intercell.py` & `pypath_omnipath-0.16.9/pypath/core/intercell.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/intercell_annot.py` & `pypath_omnipath-0.16.9/pypath/core/intercell_annot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/core/network.py` & `pypath_omnipath-0.16.9/pypath/core/network.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/data/__init__.py` & `pypath_omnipath-0.16.9/pypath/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/data/_data.py` & `pypath_omnipath-0.16.9/pypath/data/_data.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/data/embl_colors` & `pypath_omnipath-0.16.9/pypath/data/embl_colors`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/data/goose_annotations.sql` & `pypath_omnipath-0.16.9/pypath/data/goose_annotations.sql`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/data/www/favicon.ico` & `pypath_omnipath-0.16.9/pypath/data/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/formats/obo.py` & `pypath_omnipath-0.16.9/pypath/formats/obo.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/formats/sdf.py` & `pypath_omnipath-0.16.9/pypath/formats/sdf.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/formats/sqldump.py` & `pypath_omnipath-0.16.9/pypath/formats/sqldump.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/formats/sqlite.py` & `pypath_omnipath-0.16.9/pypath/formats/sqlite.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/formats/xml.py` & `pypath_omnipath-0.16.9/pypath/formats/xml.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/__init__.py` & `pypath_omnipath-0.16.9/pypath/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/abs.py` & `pypath_omnipath-0.16.9/pypath/inputs/abs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/acsn.py` & `pypath_omnipath-0.16.9/pypath/inputs/acsn.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/adhesome.py` & `pypath_omnipath-0.16.9/pypath/inputs/adhesome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/adrecs.py` & `pypath_omnipath-0.16.9/pypath/inputs/adrecs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/almen2009.py` & `pypath_omnipath-0.16.9/pypath/inputs/almen2009.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/baccin2019.py` & `pypath_omnipath-0.16.9/pypath/inputs/baccin2019.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/biogps.py` & `pypath_omnipath-0.16.9/pypath/inputs/biogps.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/biogrid.py` & `pypath_omnipath-0.16.9/pypath/inputs/biogrid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/biomart.py` & `pypath_omnipath-0.16.9/pypath/inputs/biomart.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import re
 import os
 import json
 import collections
 
 import pypath.share.session as session_mod
 import pypath.share.common as common
+import pypath_common.data as _data
 import pypath.share.curl as curl
 import pypath.resources.urls as urls
 import pypath.utils.taxonomy as taxonomy
 
 _logger = session_mod.Logger(name = 'biomart_input')
 
 
@@ -107,15 +108,15 @@
             ),
             ', '.join(_attrs),
         )
     )
 
     rewsp = re.compile(r'\n\s+')
 
-    xml_template_path = os.path.join(common.DATA, 'ensembl_biomart_query.xml')
+    xml_template_path = _data.path('ensembl_biomart_query.xml')
 
     with open(xml_template_path, 'r') as fp:
 
         xml_template = fp.read()
 
     filter_part = ''.join(
         _filter_xml_template % _filter
@@ -130,24 +131,25 @@
         dataset,
         filter_part,
         attr_part,
     )
     xml_query = rewsp.sub('', xml_query)
 
     biomart_url = urls.urls['ensembl']['biomart_url'] % xml_query
-
     c = curl.Curl(biomart_url, large = True, silent = False)
-
     success = False
 
     for line in c.result:
 
         _line = line.strip('\n\r').split('\t')
 
-        success = success or _line[0] == '[success]'
+        if _line[0] == '[success]':
+
+            success = True
+            continue
 
         if line.strip() and len(_line) == len(record._fields):
 
             yield record(*_line)
 
     if not success:
```

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/biomodels.py` & `pypath_omnipath-0.16.9/pypath/inputs/biomodels.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ca1.py` & `pypath_omnipath-0.16.9/pypath/inputs/ca1.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cancercellmap.py` & `pypath_omnipath-0.16.9/pypath/inputs/cancercellmap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cancerdrugsdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/cancerdrugsdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cancersea.py` & `pypath_omnipath-0.16.9/pypath/inputs/cancersea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cell.py` & `pypath_omnipath-0.16.9/pypath/inputs/cell.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cellcall.py` & `pypath_omnipath-0.16.9/pypath/inputs/cellcall.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cellcellinteractions.py` & `pypath_omnipath-0.16.9/pypath/inputs/cellcellinteractions.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cellchatdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/cellchatdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cellinker.py` & `pypath_omnipath-0.16.9/pypath/inputs/cellinker.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cellphonedb.py` & `pypath_omnipath-0.16.9/pypath/inputs/cellphonedb.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,24 +86,24 @@
         '_add': '',
         ' | ': ',',
         ' ': '_',
     }
 
     def get_bool(rec, attr):
 
-        return attr in rec and rec[attr] == 'True'
+        return attr in rec and rec[attr].upper() == 'TRUE'
 
     def get_desc(rec, attr):
 
         desc = '%s_desc' % attr
 
         value = (
             ''
                 if (
-                    attr in rec and rec[attr] == 'False' or
+                    attr in rec and rec[attr].upper() == 'FALSE' or
                     attr not in rec and not rec[desc]
                 ) else
             rec[desc]
                 if rec[desc] else
             attr
         )
 
@@ -260,24 +260,29 @@
             'ligand'
                 if entity in ligands else
             'receptor'
                 if entity in receptors else
             'unknown'
         )
 
+    def get_bool(rec, attr):
+
+        return attr in rec and rec[attr].upper() == 'TRUE'
+
     CellphonedbInteraction = collections.namedtuple(
         'CellphonedbInteraction',
         [
             'id_a',
             'id_b',
             'sources',
             'references',
             'interaction_type',
             'type_a',
             'type_b',
+            'is_ppi',
         ]
     )
 
     repmid = re.compile(r'PMID: ([0-9]+)')
     recomma = re.compile(r'[,;]')
 
     ligands, receptors = cellphonedb_ligands_receptors()
@@ -300,14 +305,15 @@
             rec['partner_a'],
             complexes = complexes,
         )
         _partner_b = _cellphonedb_get_entity(
             rec['partner_b'],
             complexes = complexes,
         )
+        _is_ppi = get_bool(rec, 'is_ppi')
 
         for partner_a, partner_b in itertools.product(_partner_a, _partner_b):
 
             type_a = get_type(partner_a)
             type_b = get_type(partner_b)
             rev = type_b == 'ligand' and type_a == 'receptor'
             _type_a = type_b if rev else type_a
@@ -334,14 +340,15 @@
                     id_a = partner_b if rev else partner_a,
                     id_b = partner_a if rev else partner_b,
                     sources = sources,
                     references = refs,
                     interaction_type = '%s-%s' % (_type_a, _type_b),
                     type_a = _type_a,
                     type_b = _type_b,
+                    is_ppi = _is_ppi,
                 )
             )
 
 
 def cellphonedb_complexes():
 
     annot = cellphonedb_complex_annotations()
```

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/celltalkdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/celltalkdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/celltypist.py` & `pypath_omnipath-0.16.9/pypath/inputs/celltypist.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/chembl.py` & `pypath_omnipath-0.16.9/pypath/inputs/chembl.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/clinvar.py` & `pypath_omnipath-0.16.9/pypath/inputs/clinvar.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/collectri.py` & `pypath_omnipath-0.16.9/pypath/inputs/collectri.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/common.py` & `pypath_omnipath-0.16.9/pypath/inputs/common.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/compath.py` & `pypath_omnipath-0.16.9/pypath/inputs/compath.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/compleat.py` & `pypath_omnipath-0.16.9/pypath/inputs/compleat.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/complexportal.py` & `pypath_omnipath-0.16.9/pypath/inputs/complexportal.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/comppi.py` & `pypath_omnipath-0.16.9/pypath/inputs/comppi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/connectomedb.py` & `pypath_omnipath-0.16.9/pypath/inputs/connectomedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/corum.py` & `pypath_omnipath-0.16.9/pypath/inputs/corum.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cosmic.py` & `pypath_omnipath-0.16.9/pypath/inputs/cosmic.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cpad.py` & `pypath_omnipath-0.16.9/pypath/inputs/cpad.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cpdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/cpdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/credentials.py` & `pypath_omnipath-0.16.9/pypath/inputs/credentials.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/csa.py` & `pypath_omnipath-0.16.9/pypath/inputs/csa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cspa.py` & `pypath_omnipath-0.16.9/pypath/inputs/cspa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ctdbase.py` & `pypath_omnipath-0.16.9/pypath/inputs/ctdbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/cytosig.py` & `pypath_omnipath-0.16.9/pypath/inputs/cytosig.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/dbptm.py` & `pypath_omnipath-0.16.9/pypath/inputs/dbptm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ddinter.py` & `pypath_omnipath-0.16.9/pypath/inputs/ddinter.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/deathdomain.py` & `pypath_omnipath-0.16.9/pypath/inputs/deathdomain.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/depod.py` & `pypath_omnipath-0.16.9/pypath/inputs/depod.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/dgidb.py` & `pypath_omnipath-0.16.9/pypath/inputs/dgidb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/dip.py` & `pypath_omnipath-0.16.9/pypath/inputs/dip.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/diseases.py` & `pypath_omnipath-0.16.9/pypath/inputs/diseases.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/__init__.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_api/__init__.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_api/meta.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_api/meta.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_api/schema.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_api/schema.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_api/simple.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_api/simple.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_auth.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_auth.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_client.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_client.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_field.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_field.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_proc.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_proc.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_records.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_records.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_request.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_request.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_schema.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_schema.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/disgenet/_valid.py` & `pypath_omnipath-0.16.9/pypath/inputs/disgenet/_valid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/domino.py` & `pypath_omnipath-0.16.9/pypath/inputs/domino.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/dorothea.py` & `pypath_omnipath-0.16.9/pypath/inputs/dorothea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/drugbank.py` & `pypath_omnipath-0.16.9/pypath/inputs/drugbank.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/drugcentral.py` & `pypath_omnipath-0.16.9/pypath/inputs/drugcentral.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ebi.py` & `pypath_omnipath-0.16.9/pypath/inputs/ebi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/elm.py` & `pypath_omnipath-0.16.9/pypath/inputs/elm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/embopress.py` & `pypath_omnipath-0.16.9/pypath/inputs/embopress.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/embrace.py` & `pypath_omnipath-0.16.9/pypath/inputs/embrace.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/encode.py` & `pypath_omnipath-0.16.9/pypath/inputs/encode.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ensembl.py` & `pypath_omnipath-0.16.9/pypath/inputs/ensembl.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/eutils.py` & `pypath_omnipath-0.16.9/pypath/inputs/eutils.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/exocarta.py` & `pypath_omnipath-0.16.9/pypath/inputs/exocarta.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/expasy.py` & `pypath_omnipath-0.16.9/pypath/inputs/expasy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/genecards.py` & `pypath_omnipath-0.16.9/pypath/inputs/genecards.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/go.py` & `pypath_omnipath-0.16.9/pypath/inputs/go.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/gpcrdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/gpcrdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/graphviz.py` & `pypath_omnipath-0.16.9/pypath/inputs/graphviz.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/guide2pharma.py` & `pypath_omnipath-0.16.9/pypath/inputs/guide2pharma.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/gutmgene.py` & `pypath_omnipath-0.16.9/pypath/inputs/gutmgene.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/havugimana.py` & `pypath_omnipath-0.16.9/pypath/inputs/havugimana.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hgnc.py` & `pypath_omnipath-0.16.9/pypath/inputs/hgnc.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hippie.py` & `pypath_omnipath-0.16.9/pypath/inputs/hippie.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/__init__.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/common.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/common.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/metabolites.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/metabolites.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/proteins.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/proteins.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/schema/__init__.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/schema/common.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/schema/common.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/schema/metabolites.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/schema/metabolites.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/schema/proteins.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/schema/proteins.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/structures.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/structures.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/visual.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/visual.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hmdb/xml.py` & `pypath_omnipath-0.16.9/pypath/inputs/hmdb/xml.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/homologene.py` & `pypath_omnipath-0.16.9/pypath/inputs/homologene.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def get_homologene():
     """
     Downloads the latest release of the NCBI HomoloGene database.
     Returns file pointer.
     """
 
-    url = urls.urls['homologene']['url']
+    url = urls.urls['homologene']['url_rescued']
 
     c = curl.Curl(
         url = url,
         silent = False,
         large = True,
         timeout = 1800,
         ignore_content_length = True,
```

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hpmr.py` & `pypath_omnipath-0.16.9/pypath/inputs/hpmr.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hpo.py` & `pypath_omnipath-0.16.9/pypath/inputs/hpo.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/hprd.py` & `pypath_omnipath-0.16.9/pypath/inputs/hprd.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/htri.py` & `pypath_omnipath-0.16.9/pypath/inputs/htri.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/humancellmap.py` & `pypath_omnipath-0.16.9/pypath/inputs/humancellmap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/humap.py` & `pypath_omnipath-0.16.9/pypath/inputs/humap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/humsavar.py` & `pypath_omnipath-0.16.9/pypath/inputs/humsavar.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/huri.py` & `pypath_omnipath-0.16.9/pypath/inputs/huri.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/i3d.py` & `pypath_omnipath-0.16.9/pypath/inputs/i3d.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/icellnet.py` & `pypath_omnipath-0.16.9/pypath/inputs/icellnet.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ielm.py` & `pypath_omnipath-0.16.9/pypath/inputs/ielm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/imweb.py` & `pypath_omnipath-0.16.9/pypath/inputs/imweb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/innatedb.py` & `pypath_omnipath-0.16.9/pypath/inputs/innatedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/instruct.py` & `pypath_omnipath-0.16.9/pypath/inputs/instruct.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/intact.py` & `pypath_omnipath-0.16.9/pypath/inputs/intact.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/integrins.py` & `pypath_omnipath-0.16.9/pypath/inputs/integrins.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/interpro.py` & `pypath_omnipath-0.16.9/pypath/inputs/interpro.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/intogen.py` & `pypath_omnipath-0.16.9/pypath/inputs/intogen.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ipi.py` & `pypath_omnipath-0.16.9/pypath/inputs/ipi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/iptmnet.py` & `pypath_omnipath-0.16.9/pypath/inputs/iptmnet.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/italk.py` & `pypath_omnipath-0.16.9/pypath/inputs/italk.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/kea.py` & `pypath_omnipath-0.16.9/pypath/inputs/kea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/kegg.py` & `pypath_omnipath-0.16.9/pypath/inputs/kegg.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/kegg_api.py` & `pypath_omnipath-0.16.9/pypath/inputs/kegg_api.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/kinasedotcom.py` & `pypath_omnipath-0.16.9/pypath/inputs/kinasedotcom.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/kirouac2010.py` & `pypath_omnipath-0.16.9/pypath/inputs/kirouac2010.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/lambert2018.py` & `pypath_omnipath-0.16.9/pypath/inputs/lambert2018.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/laudanna.py` & `pypath_omnipath-0.16.9/pypath/inputs/laudanna.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/li2012.py` & `pypath_omnipath-0.16.9/pypath/inputs/li2012.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/lincs.py` & `pypath_omnipath-0.16.9/pypath/inputs/lincs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/lipidmaps/structures.py` & `pypath_omnipath-0.16.9/pypath/inputs/lipidmaps/structures.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/lmpid.py` & `pypath_omnipath-0.16.9/pypath/inputs/lmpid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/lncdisease.py` & `pypath_omnipath-0.16.9/pypath/inputs/lncdisease.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/lncrnadb.py` & `pypath_omnipath-0.16.9/pypath/inputs/lncrnadb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/locate.py` & `pypath_omnipath-0.16.9/pypath/inputs/locate.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/lrdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/lrdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/macrophage.py` & `pypath_omnipath-0.16.9/pypath/inputs/macrophage.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/matrisome.py` & `pypath_omnipath-0.16.9/pypath/inputs/matrisome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/matrixdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/matrixdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mcam.py` & `pypath_omnipath-0.16.9/pypath/inputs/mcam.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/membranome.py` & `pypath_omnipath-0.16.9/pypath/inputs/membranome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mimp.py` & `pypath_omnipath-0.16.9/pypath/inputs/mimp.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mir2disease.py` & `pypath_omnipath-0.16.9/pypath/inputs/mir2disease.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mirbase.py` & `pypath_omnipath-0.16.9/pypath/inputs/mirbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mirdeathdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/mirdeathdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mirecords.py` & `pypath_omnipath-0.16.9/pypath/inputs/mirecords.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mirtarbase.py` & `pypath_omnipath-0.16.9/pypath/inputs/mirtarbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mitab.py` & `pypath_omnipath-0.16.9/pypath/inputs/mitab.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/mppi.py` & `pypath_omnipath-0.16.9/pypath/inputs/mppi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/msigdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/msigdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ncrdeathdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/ncrdeathdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/negatome.py` & `pypath_omnipath-0.16.9/pypath/inputs/negatome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/netbiol.py` & `pypath_omnipath-0.16.9/pypath/inputs/netbiol.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/netpath.py` & `pypath_omnipath-0.16.9/pypath/inputs/netpath.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/offsides.py` & `pypath_omnipath-0.16.9/pypath/inputs/offsides.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/oma.py` & `pypath_omnipath-0.16.9/pypath/inputs/oma.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ontology.py` & `pypath_omnipath-0.16.9/pypath/inputs/ontology.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/opentargets.py` & `pypath_omnipath-0.16.9/pypath/inputs/opentargets.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/opm.py` & `pypath_omnipath-0.16.9/pypath/inputs/opm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/oreganno.py` & `pypath_omnipath-0.16.9/pypath/inputs/oreganno.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/panglaodb.py` & `pypath_omnipath-0.16.9/pypath/inputs/panglaodb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pathophenodb.py` & `pypath_omnipath-0.16.9/pypath/inputs/pathophenodb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pathwaycommons.py` & `pypath_omnipath-0.16.9/pypath/inputs/pathwaycommons.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pazar.py` & `pypath_omnipath-0.16.9/pypath/inputs/pazar.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/pdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pdzbase.py` & `pypath_omnipath-0.16.9/pypath/inputs/pdzbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pepcyber.py` & `pypath_omnipath-0.16.9/pypath/inputs/pepcyber.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pfam.py` & `pypath_omnipath-0.16.9/pypath/inputs/pfam.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pharos.py` & `pypath_omnipath-0.16.9/pypath/inputs/pharos.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/phobius.py` & `pypath_omnipath-0.16.9/pypath/inputs/phobius.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/phosphatome.py` & `pypath_omnipath-0.16.9/pypath/inputs/phosphatome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/phosphoelm.py` & `pypath_omnipath-0.16.9/pypath/inputs/phosphoelm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/phosphonetworks.py` & `pypath_omnipath-0.16.9/pypath/inputs/phosphonetworks.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/phosphopoint.py` & `pypath_omnipath-0.16.9/pypath/inputs/phosphopoint.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/phosphosite.py` & `pypath_omnipath-0.16.9/pypath/inputs/phosphosite.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pisa.py` & `pypath_omnipath-0.16.9/pypath/inputs/pisa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pro.py` & `pypath_omnipath-0.16.9/pypath/inputs/pro.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/progeny.py` & `pypath_omnipath-0.16.9/pypath/inputs/progeny.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/proteinatlas.py` & `pypath_omnipath-0.16.9/pypath/inputs/proteinatlas.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/proteins.py` & `pypath_omnipath-0.16.9/pypath/inputs/proteins.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/protmapper.py` & `pypath_omnipath-0.16.9/pypath/inputs/protmapper.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pubchem.py` & `pypath_omnipath-0.16.9/pypath/inputs/pubchem.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/pubmed.py` & `pypath_omnipath-0.16.9/pypath/inputs/pubmed.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ramilowski2015.py` & `pypath_omnipath-0.16.9/pypath/inputs/ramilowski2015.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/ramp.py` & `pypath_omnipath-0.16.9/pypath/inputs/ramp.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/rdata.py` & `pypath_omnipath-0.16.9/pypath/inputs/rdata.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/reaction.py` & `pypath_omnipath-0.16.9/pypath/inputs/reaction.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/reactome.py` & `pypath_omnipath-0.16.9/pypath/inputs/reactome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/scconnect.py` & `pypath_omnipath-0.16.9/pypath/inputs/scconnect.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/science.py` & `pypath_omnipath-0.16.9/pypath/inputs/science.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/sider.py` & `pypath_omnipath-0.16.9/pypath/inputs/sider.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/signalink.py` & `pypath_omnipath-0.16.9/pypath/inputs/signalink.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/signor.py` & `pypath_omnipath-0.16.9/pypath/inputs/signor.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/spike.py` & `pypath_omnipath-0.16.9/pypath/inputs/spike.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/stitch.py` & `pypath_omnipath-0.16.9/pypath/inputs/stitch.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/string.py` & `pypath_omnipath-0.16.9/pypath/inputs/string.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/surfaceome.py` & `pypath_omnipath-0.16.9/pypath/inputs/surfaceome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/switches_elm.py` & `pypath_omnipath-0.16.9/pypath/inputs/switches_elm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/talklr.py` & `pypath_omnipath-0.16.9/pypath/inputs/talklr.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/tcdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/tcdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/tfcensus.py` & `pypath_omnipath-0.16.9/pypath/inputs/tfcensus.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/threedcomplex.py` & `pypath_omnipath-0.16.9/pypath/inputs/threedcomplex.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/threedid.py` & `pypath_omnipath-0.16.9/pypath/inputs/threedid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/topdb.py` & `pypath_omnipath-0.16.9/pypath/inputs/topdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/transmir.py` & `pypath_omnipath-0.16.9/pypath/inputs/transmir.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/trip.py` & `pypath_omnipath-0.16.9/pypath/inputs/trip.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/trrust.py` & `pypath_omnipath-0.16.9/pypath/inputs/trrust.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/twosides.py` & `pypath_omnipath-0.16.9/pypath/inputs/twosides.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/unichem.py` & `pypath_omnipath-0.16.9/pypath/inputs/unichem.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/uniprot.py` & `pypath_omnipath-0.16.9/pypath/inputs/uniprot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/uniprot_db.py` & `pypath_omnipath-0.16.9/pypath/inputs/uniprot_db.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/wang.py` & `pypath_omnipath-0.16.9/pypath/inputs/wang.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/wojtowicz2020.py` & `pypath_omnipath-0.16.9/pypath/inputs/wojtowicz2020.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/inputs/zhong2015.py` & `pypath_omnipath-0.16.9/pypath/inputs/zhong2015.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/internals/annot_formats.py` & `pypath_omnipath-0.16.9/pypath/internals/annot_formats.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/internals/input_formats.py` & `pypath_omnipath-0.16.9/pypath/internals/input_formats.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/internals/intera.py` & `pypath_omnipath-0.16.9/pypath/internals/intera.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/internals/license.py` & `pypath_omnipath-0.16.9/pypath/internals/license.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/internals/maps.py` & `pypath_omnipath-0.16.9/pypath/internals/maps.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/internals/refs.py` & `pypath_omnipath-0.16.9/pypath/internals/refs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/internals/resource.py` & `pypath_omnipath-0.16.9/pypath/internals/resource.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/legacy/db_categories.py` & `pypath_omnipath-0.16.9/pypath/legacy/db_categories.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/legacy/main.py` & `pypath_omnipath-0.16.9/pypath/legacy/main.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/__init__.py` & `pypath_omnipath-0.16.9/pypath/omnipath/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/app.py` & `pypath_omnipath-0.16.9/pypath/omnipath/app.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/bel.py` & `pypath_omnipath-0.16.9/pypath/omnipath/bel.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/cellphonedb.py` & `pypath_omnipath-0.16.9/pypath/omnipath/cellphonedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/databases/__init__.py` & `pypath_omnipath-0.16.9/pypath/omnipath/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/databases/build.py` & `pypath_omnipath-0.16.9/pypath/omnipath/databases/build.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/databases/builtins.json` & `pypath_omnipath-0.16.9/pypath/omnipath/databases/builtins.json`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/databases/classes.json` & `pypath_omnipath-0.16.9/pypath/omnipath/databases/classes.json`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/databases/define.py` & `pypath_omnipath-0.16.9/pypath/omnipath/databases/define.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/export.py` & `pypath_omnipath-0.16.9/pypath/omnipath/export.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/legacy.py` & `pypath_omnipath-0.16.9/pypath/omnipath/legacy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/param.py` & `pypath_omnipath-0.16.9/pypath/omnipath/param.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/server/_html.py` & `pypath_omnipath-0.16.9/pypath/omnipath/server/_html.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/server/build.py` & `pypath_omnipath-0.16.9/pypath/omnipath/server/build.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/server/generate_about_page.py` & `pypath_omnipath-0.16.9/pypath/omnipath/server/generate_about_page.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/server/legacy.py` & `pypath_omnipath-0.16.9/pypath/omnipath/server/legacy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/omnipath/server/run.py` & `pypath_omnipath-0.16.9/pypath/omnipath/server/run.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/reader/field.py` & `pypath_omnipath-0.16.9/pypath/reader/field.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/reader/network.py` & `pypath_omnipath-0.16.9/pypath/reader/network.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/resources/__init__.py` & `pypath_omnipath-0.16.9/pypath/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/resources/controller.py` & `pypath_omnipath-0.16.9/pypath/resources/controller.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/resources/data/resources.json` & `pypath_omnipath-0.16.9/pypath/resources/data/resources.json`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/resources/data_formats.py` & `pypath_omnipath-0.16.9/pypath/resources/data_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2941,14 +2941,15 @@
         input = 'cellphonedb.cellphonedb_interactions',
         references = (3, ';'),
         resource = (2, ';'),
         must_have_references = False,
         header = False,
         extra_edge_attrs = {
             'type': 4,
+            'is_ppi': 7,
         },
         extra_node_attrs_a = {
             'cellphonedb_type': 5,
         },
         extra_node_attrs_b = {
             'cellphonedb_type': 6,
         },
```

### Comparing `pypath_omnipath-0.16.5/pypath/resources/descriptions.py` & `pypath_omnipath-0.16.9/pypath/resources/descriptions.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/resources/licenses.py` & `pypath_omnipath-0.16.9/pypath/resources/licenses.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/resources/network.py` & `pypath_omnipath-0.16.9/pypath/resources/network.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/resources/urls.py` & `pypath_omnipath-0.16.9/pypath/resources/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -977,16 +977,17 @@
     'pwcommons': {
         'label': 'PathwayCommons binary SIF files',
         'url': 'https://www.pathwaycommons.org/archives/PC2/v%u/'
             'PathwayCommons%u.%s.hgnc.sif.gz',
     },
     'homologene': {
         'label': 'NCBI HomoloGene data, recent release',
-        'url': 'https://ftp.ncbi.nih.gov/pub/HomoloGene/'
+        'url_original': 'https://ftp.ncbi.nih.gov/pub/HomoloGene/'
             'current/homologene.data',
+        'url_rescued': 'https://rescued.omnipathdb.org/homologene.data',
     },
     'mirbase' : {
         'label': 'miRBase: miRNA main reference database',
         'aliases_old': 'ftp://mirbase.org/pub/mirbase/CURRENT/aliases.txt.gz',
         'aliases': 'https://mirbase.org/ftp/CURRENT/aliases.txt.gz',
     },
     'mir2dis': {
@@ -1424,15 +1425,15 @@
         'label': 'Manually curated ligand-receptor interactions',
         'url': 'http://tcm.zju.edu.cn/celltalkdb/handler/download.php',
         'ref_url': 'http://tcm.zju.edu.cn/celltalkdb/',
         'init_url': 'http://tcm.zju.edu.cn/celltalkdb/download.php',
     },
     'cellchatdb': {
         'label': 'Manually curated ligand-receptor interactions',
-        'url': 'https://raw.githubusercontent.com/sqjin/CellChat/'
+        'url': 'https://raw.githubusercontent.com/jinworks/CellChat/'
             'master/data/%s.rda',
     },
     'connectomedb2020': {
         'label': 'Ligand-receptor interactions from original curation '
             'and from other databases',
         'url': 'https://raw.githubusercontent.com/asrhou/NATMI/'
             'gh-pages/_data/lsps.csv',
```

### Comparing `pypath_omnipath-0.16.5/pypath/share/cache.py` & `pypath_omnipath-0.16.9/pypath/share/cache.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/share/curl.py` & `pypath_omnipath-0.16.9/pypath/share/curl.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/share/lookup/_manytomany.py` & `pypath_omnipath-0.16.9/pypath/share/lookup/_manytomany.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/share/lookup/_onetomany.py` & `pypath_omnipath-0.16.9/pypath/share/lookup/_onetomany.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/share/lookup/_onetomany2.py` & `pypath_omnipath-0.16.9/pypath/share/lookup/_onetomany2.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/share/progress.py` & `pypath_omnipath-0.16.9/pypath/share/progress.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/go.py` & `pypath_omnipath-0.16.9/pypath/utils/go.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/mapping.py` & `pypath_omnipath-0.16.9/pypath/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/metabo/__init__.py` & `pypath_omnipath-0.16.9/pypath/utils/metabo/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/metabo/struct/visual.py` & `pypath_omnipath-0.16.9/pypath/utils/metabo/struct/visual.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/orthology.py` & `pypath_omnipath-0.16.9/pypath/utils/orthology.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/pdb.py` & `pypath_omnipath-0.16.9/pypath/utils/pdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/proteomicsdb.py` & `pypath_omnipath-0.16.9/pypath/utils/proteomicsdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/pyreact.py` & `pypath_omnipath-0.16.9/pypath/utils/pyreact.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/reflists.py` & `pypath_omnipath-0.16.9/pypath/utils/reflists.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/residues.py` & `pypath_omnipath-0.16.9/pypath/utils/residues.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/seq.py` & `pypath_omnipath-0.16.9/pypath/utils/seq.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/taxonomy.py` & `pypath_omnipath-0.16.9/pypath/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/unichem.py` & `pypath_omnipath-0.16.9/pypath/utils/unichem.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/utils/uniprot.py` & `pypath_omnipath-0.16.9/pypath/utils/uniprot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/visual/drawing.py` & `pypath_omnipath-0.16.9/pypath/visual/drawing.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/visual/igraph_drawing/__init__.py` & `pypath_omnipath-0.16.9/pypath/visual/igraph_drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/visual/igraph_drawing/edge.py` & `pypath_omnipath-0.16.9/pypath/visual/igraph_drawing/edge.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/visual/igraph_drawing/vertex.py` & `pypath_omnipath-0.16.9/pypath/visual/igraph_drawing/vertex.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pypath/visual/plot.py` & `pypath_omnipath-0.16.9/pypath/visual/plot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.16.5/pyproject.toml` & `pypath_omnipath-0.16.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pypath-omnipath"
-version = "0.16.5"
+version = "0.16.9"
 description = "Molecular signaling prior knowledge processing"
 license = "GPL-3.0-only"
 authors = [
     "Denes Turei <turei.denes@gmail.com>",
     "Nicolàs Palacio",
     "Sebastian Lobentanzer",
     "Olga Ivanova",
@@ -58,15 +58,15 @@
 lxml = "*"
 matplotlib = "*"
 numpy = "*"
 openpyxl = "*"
 pandas = "*"
 psutil = "*"
 pycurl = "*"
-pypath_common = ">=0.2.0"
+pypath-common = ">=0.2.0"
 pyreadr = "*"
 PyYAML = "*"
 rdata = "*"
 requests = "*"
 scipy = ">=1.9.0"
 sqlparse = "*"
 tabulate = "*"
```

### Comparing `pypath_omnipath-0.16.5/PKG-INFO` & `pypath_omnipath-0.16.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypath-omnipath
-Version: 0.16.5
+Version: 0.16.9
 Summary: Molecular signaling prior knowledge processing
 Home-page: https://omnipathdb.org/
 License: GPL-3.0-only
 Keywords: systems biology,molecular biology,omics,network,signaling
 Author: Denes Turei
 Author-email: turei.denes@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -38,15 +38,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: openbabel ; extra == "metabo"
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: pycurl
-Requires-Dist: pypath_common (>=0.2.0)
+Requires-Dist: pypath-common (>=0.2.0)
 Requires-Dist: pyreadr
 Requires-Dist: pysftp (>=0.2.9,<0.3.0)
 Requires-Dist: python-igraph ; extra == "graph"
 Requires-Dist: rdata
 Requires-Dist: rdkit ; extra == "metabo"
 Requires-Dist: requests
 Requires-Dist: scipy (>=1.9.0)
```

