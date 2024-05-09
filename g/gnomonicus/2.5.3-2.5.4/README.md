# Comparing `tmp/gnomonicus-2.5.3.tar.gz` & `tmp/gnomonicus-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnomonicus-2.5.3.tar", last modified: Wed Mar 27 12:55:40 2024, max compression
+gzip compressed data, was "gnomonicus-2.5.4.tar", last modified: Thu May  9 07:41:49 2024, max compression
```

## Comparing `gnomonicus-2.5.3.tar` & `gnomonicus-2.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:55:40.614308 gnomonicus-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-03-27 12:54:47.000000 gnomonicus-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-03-27 12:55:40.614308 gnomonicus-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-27 12:54:47.000000 gnomonicus-2.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:55:40.610309 gnomonicus-2.5.3/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-27 12:54:47.000000 gnomonicus-2.5.3/bin/gbkToPkl
--rwxr-xr-x   0 runner    (1001) docker     (127)    10910 2024-03-27 12:54:47.000000 gnomonicus-2.5.3/bin/gnomonicus
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-27 12:54:47.000000 gnomonicus-2.5.3/bin/gnomonicus-table-update
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:55:40.610309 gnomonicus-2.5.3/gnomonicus/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-27 12:54:47.000000 gnomonicus-2.5.3/gnomonicus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78395 2024-03-27 12:54:47.000000 gnomonicus-2.5.3/gnomonicus/gnomonicus_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:55:40.614308 gnomonicus-2.5.3/gnomonicus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-03-27 12:55:40.000000 gnomonicus-2.5.3/gnomonicus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-27 12:55:40.000000 gnomonicus-2.5.3/gnomonicus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 12:55:40.000000 gnomonicus-2.5.3/gnomonicus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 12:54:57.000000 gnomonicus-2.5.3/gnomonicus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-27 12:55:40.000000 gnomonicus-2.5.3/gnomonicus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 12:55:40.000000 gnomonicus-2.5.3/gnomonicus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-27 12:54:47.000000 gnomonicus-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-27 12:55:40.614308 gnomonicus-2.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:41:49.855774 gnomonicus-2.5.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/bin/gbkToPkl
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10910 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/bin/gnomonicus
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/bin/gnomonicus-table-update
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/gnomonicus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/gnomonicus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79237 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/gnomonicus/gnomonicus_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/gnomonicus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:41:09.000000 gnomonicus-2.5.4/gnomonicus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/setup.cfg
```

### Comparing `gnomonicus-2.5.3/LICENSE` & `gnomonicus-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.3/PKG-INFO` & `gnomonicus-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnomonicus
-Version: 2.5.3
+Version: 2.5.4
 Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 Home-page: https://github.com/oxfordmmm/gnomonicus
 Author: Philip W Fowler, Jeremy Westhead
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford License, see LICENSE
 Keywords: gnomonicus,piezo,lodestone,clockwork,TB
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gnomonicus-2.5.3/README.md` & `gnomonicus-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.3/bin/gbkToPkl` & `gnomonicus-2.5.4/bin/gbkToPkl`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.3/bin/gnomonicus` & `gnomonicus-2.5.4/bin/gnomonicus`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.3/bin/gnomonicus-table-update` & `gnomonicus-2.5.4/bin/gnomonicus-table-update`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.3/gnomonicus/__init__.py` & `gnomonicus-2.5.4/gnomonicus/__init__.py`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.3/gnomonicus/gnomonicus_lib.py` & `gnomonicus-2.5.4/gnomonicus/gnomonicus_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import logging
 import os
 import pickle
 import re
 import traceback
 import warnings
 import io
-from collections import defaultdict
+from collections import defaultdict, OrderedDict
 from typing import Dict, List, Tuple
 
 import gumpy
 import numpy as np
 import pandas as pd
 import piezo
 from tqdm import tqdm
@@ -1266,15 +1266,15 @@
                 new_mutations.append((None, multi))
     if just_joined:
         return new_mutations
     return mutations_ + new_mutations
 
 
 def getMutations(
-    mutations_df: pd.DataFrame,
+    mutations_df: pd.DataFrame | None,
     catalogue: piezo.ResistanceCatalogue,
     referenceGenes: Dict,
 ) -> List[Tuple[str | None, str]]:
     """Get all of the mutations (including multi-mutations) from the mutations df
     Multi-mutations currently only exist within the converted WHO catalogue, and are a highly specific combination
         of mutations which must all be present for a single resistance value.
 
@@ -1282,14 +1282,16 @@
         mutations_df (pd.DataFrame): Mutations dataframe
         catalogue (piezo.ResistanceCatalogue): The resistance catalogue. Used to find which multi-mutations we care about
         referenceGenes (dict): Dictionary of geneName->gumpy.Gene
 
     Returns:
         List[Tuple[str | None, str]]: List of [gene, mutation] or in the case of multi-mutations, [None, multi-mutation]
     """
+    if mutations_df is None:
+        return []
     mutations: List[Tuple[str | None, str]] = list(
         zip(mutations_df["gene"], mutations_df["mutation"])
     )
     # Grab the multi-mutations from the catalogue
     # By doing this, we can check a fixed sample space rather than every permutation of the mutations
     # This makes the problem tractable, but does not address a possible issue with multi-mutations not encapsulating full codons
     multis = set(
@@ -1638,136 +1640,138 @@
     effects = {}
     effectsCounter = 0
 
     # Default prediction values are RFUS but use piezo catalogue's values if existing
     values = resistanceCatalogue.catalogue.values
 
     # only try and build an effects table if there are mutations
-    if mutations is not None:
-        sample_mutations = getMutations(mutations, resistanceCatalogue, referenceGenes)
-        for gene, mutation in tqdm(sample_mutations):
-            # Ensure its a valid mutation
-            if gene is not None and not referenceGenes[gene].valid_variant(mutation):
-                logging.error(f"Not a valid mutation {gene}@{mutation}")
-                raise InvalidMutationException(gene, mutation)
+    sample_mutations = getMutations(mutations, resistanceCatalogue, referenceGenes)
+    for gene, mutation in tqdm(sample_mutations):
+        # Ensure its a valid mutation
+        if gene is not None and not referenceGenes[gene].valid_variant(mutation):
+            logging.error(f"Not a valid mutation {gene}@{mutation}")
+            raise InvalidMutationException(gene, mutation)
+
+        # Get the prediction
+        if gene is not None:
+            prediction = resistanceCatalogue.predict(
+                gene + "@" + mutation, show_evidence=True
+            )
+        else:
+            # This is a multi-mutation so is already of required format
+            prediction = resistanceCatalogue.predict(mutation, show_evidence=True)
 
-            # Get the prediction
-            if gene is not None:
-                prediction = resistanceCatalogue.predict(
-                    gene + "@" + mutation, show_evidence=True
-                )
-            else:
-                # This is a multi-mutation so is already of required format
-                prediction = resistanceCatalogue.predict(mutation, show_evidence=True)
+        # If the prediction is interesting, iter through drugs to find predictions
+        if prediction != "S" and not isinstance(prediction, str):
+            for drug in prediction.keys():
+                drug_pred = prediction[drug]
+                if isinstance(drug_pred, str):
+                    # This shouldn't happen because we're showing evidence
+                    # Adding to appease mypy...
+                    pred: str = drug_pred
+                    evidence: Dict = {}
+                else:
+                    pred, evidence = drug_pred
+                # Prioritise values based on order within the values list
+                if values.index(pred) < values.index(phenotype[drug]):
+                    # The prediction is closer to the start of the values list, so should take priority
+                    phenotype[drug] = pred
 
-            # If the prediction is interesting, iter through drugs to find predictions
-            if prediction != "S" and not isinstance(prediction, str):
-                for drug in prediction.keys():
-                    drug_pred = prediction[drug]
-                    if isinstance(drug_pred, str):
-                        # This shouldn't happen because we're showing evidence
-                        # Adding to appease mypy...
-                        pred: str = drug_pred
-                        evidence: Dict = {}
-                    else:
-                        pred, evidence = drug_pred
-                    # Prioritise values based on order within the values list
-                    if values.index(pred) < values.index(phenotype[drug]):
-                        # The prediction is closer to the start of the values list, so should take priority
-                        phenotype[drug] = pred
+                # Add to the dict
+                effects[effectsCounter] = [
+                    vcfStem,
+                    gene,
+                    mutation,
+                    resistanceCatalogue.catalogue.name,
+                    drug,
+                    pred,
+                    evidence,
+                ]
+                # Increment counter
+                effectsCounter += 1
 
-                    # Add to the dict
-                    effects[effectsCounter] = [
-                        vcfStem,
-                        gene,
-                        mutation,
-                        resistanceCatalogue.catalogue.name,
-                        drug,
-                        pred,
-                        evidence,
-                    ]
-                    # Increment counter
-                    effectsCounter += 1
+    # Check for epistasis rules (which ignore prediction heirarchy)
+    effectsCounter = epistasis(
+        sample_mutations,
+        resistanceCatalogue,
+        phenotype,
+        effects,
+        effectsCounter,
+        vcfStem,
+    )
 
-        # Check for epistasis rules (which ignore prediction heirarchy)
-        effectsCounter = epistasis(
-            sample_mutations,
-            resistanceCatalogue,
-            phenotype,
+    if fasta is not None and reference is not None:
+        # Implicitly uses `effects` and `pheotype` for returns
+        new_mutations = fasta_adjudication(
+            vcfStem,
+            fasta,
             effects,
             effectsCounter,
-            vcfStem,
+            resistanceCatalogue,
+            referenceGenes,
+            reference,
+            phenotype,
         )
-
-        if fasta is not None and reference is not None:
-            # Implicitly uses `effects` and `pheotype` for returns
-            new_mutations = fasta_adjudication(
-                vcfStem,
-                fasta,
-                effects,
-                effectsCounter,
-                resistanceCatalogue,
-                referenceGenes,
-                reference,
-                phenotype,
-            )
+        if mutations is not None:
             mutations = pd.concat([mutations, new_mutations])
-            mutations.reset_index(inplace=True)
-            if make_mutations_csv:
-                write_mutations_csv(
-                    mutations,
-                    os.path.join(outputDir, f"{vcfStem}.mutations.csv"),
-                    filter=False,
-                )
+        else:
+            mutations = new_mutations
+        mutations.reset_index(inplace=True)
+        if make_mutations_csv:
+            write_mutations_csv(
+                mutations,
+                os.path.join(outputDir, f"{vcfStem}.mutations.csv"),
+                filter=False,
+            )
 
-        # Build the DataFrame
-        effects_df = pd.DataFrame.from_dict(
-            effects,
-            orient="index",
-            columns=[
-                "uniqueid",
-                "gene",
-                "mutation",
-                "catalogue_name",
-                "drug",
-                "prediction",
-                "evidence",
-            ],
-        )
-        effects_df = effects_df[
-            [
-                "uniqueid",
-                "gene",
-                "mutation",
-                "drug",
-                "prediction",
-                "catalogue_name",
-                "evidence",
-            ]
+    # Build the DataFrame
+    effects_df = pd.DataFrame.from_dict(
+        effects,
+        orient="index",
+        columns=[
+            "uniqueid",
+            "gene",
+            "mutation",
+            "catalogue_name",
+            "drug",
+            "prediction",
+            "evidence",
+        ],
+    )
+    effects_df = effects_df[
+        [
+            "uniqueid",
+            "gene",
+            "mutation",
+            "drug",
+            "prediction",
+            "catalogue_name",
+            "evidence",
         ]
-        effects_df["catalogue_version"] = resistanceCatalogue.catalogue.version
-        effects_df["prediction_values"] = "".join(resistanceCatalogue.catalogue.values)
+    ]
+    effects_df["catalogue_version"] = resistanceCatalogue.catalogue.version
+    effects_df["prediction_values"] = "".join(resistanceCatalogue.catalogue.values)
 
-        # Save as CSV
-        if len(effects) > 0 and make_csv:
-            if append:
-                # Check to see if there's anything there already
-                try:
-                    old_effects = pd.read_csv(
-                        os.path.join(outputDir, f"{vcfStem}.effects.csv")
-                    )
-                    effects_df = pd.concat([old_effects, effects_df])
-                except FileNotFoundError:
-                    pass
+    # Save as CSV
+    if len(effects) > 0 and make_csv:
+        if append:
+            # Check to see if there's anything there already
+            try:
+                old_effects = pd.read_csv(
+                    os.path.join(outputDir, f"{vcfStem}.effects.csv")
+                )
+                effects_df = pd.concat([old_effects, effects_df])
+            except FileNotFoundError:
+                pass
 
-            effects_df.to_csv(
-                os.path.join(outputDir, f"{vcfStem}.effects.csv"), index=False
-            )
+        effects_df.to_csv(
+            os.path.join(outputDir, f"{vcfStem}.effects.csv"), index=False
+        )
 
-        effects_df.reset_index(inplace=True)
+    effects_df.reset_index(inplace=True)
 
     if make_prediction_csv:
         # We need to construct a simple table here
         predictions = [phenotype[drug] for drug in resistanceCatalogue.catalogue.drugs]
         vals = {
             "uniqueid": vcfStem,
             "drug": resistanceCatalogue.catalogue.drugs,
@@ -1801,15 +1805,15 @@
     )
 
 
 def saveJSON(
     variants,
     mutations,
     effects,
-    phenotypes,
+    phenotypes: dict[str, str],
     path: str,
     guid: str,
     catalogue: piezo.ResistanceCatalogue,
     gnomonicusVersion: str,
     time_taken: float,
     reference: gumpy.Genome,
     vcf_path: str,
@@ -1888,108 +1892,149 @@
         reference (gumpy.Genome): Reference genome object
         vcf_path (str): Path to the VCF file used for this run
         reference_path (str): Path to the reference genome used for this run
         catalogue_path (str): Path to the catalogue used for this run
         minor_errors (dict): Mapping of gene name --> stack trace of any errors occurring when parsing minor mutations
     """
     # Define some metadata for the json
-    meta = {
-        "status": "success",
-        "workflow_name": "gnomonicus",
-        "workflow_version": gnomonicusVersion,  # gnomonicus version used
-        "workflow_task": "resistance_prediction",  # TODO: Update this when we know how to detect a virulence catalogue
-        "guid": guid,  # Sample GUID
-        "UTC-datetime-completed": datetime.datetime.utcnow().isoformat(),  # ISO datetime run
-        "time_taken_s": time_taken,
-        "reference": reference.name,
-        "catalogue_file": catalogue_path,
-        "reference_file": reference_path,
-        "vcf_file": vcf_path,
-    }
+    meta = OrderedDict(
+        {
+            "status": "success",
+            "workflow_name": "gnomonicus",
+            "workflow_version": gnomonicusVersion,  # gnomonicus version used
+            "workflow_task": "resistance_prediction",  # TODO: Update this when we know how to detect a virulence catalogue
+            "guid": guid,  # Sample GUID
+            "UTC-datetime-completed": datetime.datetime.utcnow().isoformat(),  # ISO datetime run
+            "time_taken_s": time_taken,
+            "reference": reference.name,
+            "catalogue_file": catalogue_path,
+            "reference_file": reference_path,
+            "vcf_file": vcf_path,
+        }
+    )
     if catalogue is not None:
         meta["catalogue_type"] = "".join(catalogue.catalogue.values)
         meta["catalogue_name"] = catalogue.catalogue.name
         meta["catalogue_version"] = catalogue.catalogue.version
     else:
         meta["catalogue_type"] = None
         meta["catalogue_name"] = None
         meta["catalogue_version"] = None
-    data: Dict = {}
+
+    # Main data collection
+    data: Dict = OrderedDict()
+
+    # Antibigram field
+    data["antibiogram"] = OrderedDict(
+        [(key, phenotypes[key]) for key in sorted(phenotypes.keys())]
+    )
+
     # Variants field
     _variants = []
     for _, variant in variants.iterrows():
-        row = {
-            "variant": variant["variant"] if pd.notnull(variant["variant"]) else None,
-            "nucleotide_index": (
-                variant["nucleotide_index"]
-                if pd.notnull(variant["nucleotide_index"])
-                else None
-            ),
-            "gene_name": variant["gene"] if pd.notnull(variant["gene"]) else None,
-            "gene_position": (
-                variant["gene_position"]
-                if pd.notnull(variant["gene_position"])
-                else None
-            ),
-            "codon_idx": (
-                variant["codon_idx"] if pd.notnull(variant["codon_idx"]) else None
-            ),
-            "vcf_evidence": json.loads(variant["vcf_evidence"]),
-            "vcf_idx": variant["vcf_idx"] if pd.notnull(variant["vcf_idx"]) else None,
-        }
+        row = OrderedDict(
+            {
+                "variant": (
+                    variant["variant"] if pd.notnull(variant["variant"]) else None
+                ),
+                "nucleotide_index": (
+                    variant["nucleotide_index"]
+                    if pd.notnull(variant["nucleotide_index"])
+                    else None
+                ),
+                "gene_name": variant["gene"] if pd.notnull(variant["gene"]) else None,
+                "gene_position": (
+                    variant["gene_position"]
+                    if pd.notnull(variant["gene_position"])
+                    else None
+                ),
+                "codon_idx": (
+                    variant["codon_idx"] if pd.notnull(variant["codon_idx"]) else None
+                ),
+                "vcf_evidence": json.loads(variant["vcf_evidence"]),
+                "vcf_idx": (
+                    variant["vcf_idx"] if pd.notnull(variant["vcf_idx"]) else None
+                ),
+            }
+        )
         _variants.append(row)
+    _variants = sorted(
+        _variants,
+        key=lambda x: x["variant"],
+    )
     data["variants"] = _variants
 
     # Depending on mutations/effects, populate
     _mutations = []
     if mutations is not None:
         for _, mutation in mutations.iterrows():
-            row = {
-                "mutation": (
-                    mutation["mutation"] if pd.notnull(mutation["mutation"]) else None
-                ),
-                "gene": mutation["gene"] if pd.notnull(mutation["gene"]) else None,
-                "gene_position": (
-                    mutation["gene_position"]
-                    if pd.notnull(mutation["gene_position"])
-                    else None
-                ),
-            }
+            row = OrderedDict(
+                {
+                    "gene": mutation["gene"] if pd.notnull(mutation["gene"]) else None,
+                    "gene_position": (
+                        mutation["gene_position"]
+                        if pd.notnull(mutation["gene_position"])
+                        else None
+                    ),
+                    "mutation": (
+                        mutation["mutation"]
+                        if pd.notnull(mutation["mutation"])
+                        else None
+                    ),
+                }
+            )
             if mutation["mutation"][0].isupper() or mutation["mutation"][0] == "!":
                 # Only add codon ref/alt for AA changes
                 row["ref"] = mutation["ref"] if pd.notnull(mutation["ref"]) else None
                 row["alt"] = mutation["alt"] if pd.notnull(mutation["alt"]) else None
             _mutations.append(row)
+
+    _mutations = sorted(
+        _mutations,
+        key=lambda x: (x["gene"] or "z", x["gene_position"] or 0),
+    )
     data["mutations"] = _mutations
 
     _effects = defaultdict(list)
     if effects is not None and len(effects) > 0:
         for _, effect in effects.iterrows():
-            prediction = {
-                "gene": effect["gene"] if pd.notnull(effect["gene"]) else None,
-                "mutation": (
-                    effect["mutation"] if pd.notnull(effect["mutation"]) else None
-                ),
-                "prediction": (
-                    effect["prediction"] if pd.notnull(effect["prediction"]) else None
-                ),
-                "evidence": effect["evidence"],
-            }
+            prediction = OrderedDict(
+                {
+                    "gene": effect["gene"] if pd.notnull(effect["gene"]) else None,
+                    "mutation": (
+                        effect["mutation"] if pd.notnull(effect["mutation"]) else None
+                    ),
+                    "prediction": (
+                        effect["prediction"]
+                        if pd.notnull(effect["prediction"])
+                        else None
+                    ),
+                    "evidence": effect["evidence"],
+                }
+            )
             _effects[effect["drug"]].append(prediction)
 
     for drug in _effects.keys():
-        _effects[drug].append({"phenotype": phenotypes[drug]})
+        _effects[drug] = sorted(
+            _effects[drug],
+            key=lambda x: (x["gene"] or "z", x["mutation"] or "z"),
+        )
+        _effects[drug].append(OrderedDict({"phenotype": phenotypes[drug]}))
 
-    data["effects"] = _effects
-    data["antibiogram"] = phenotypes
+    data["effects"] = OrderedDict(
+        [(key, _effects[key]) for key in sorted(_effects.keys())]
+    )
 
     # Convert fields to a list so it can be json serialised
-    with open(os.path.join(path, f"{guid}.gnomonicus-out.json"), "w") as f:
+    with open(
+        os.path.join(path, f"{guid}.gnomonicus-out.json"), "w", encoding="utf-8"
+    ) as f:
         # Add errors (if any)
         if len(minor_errors) > 0:
             f.write(
                 json.dumps(
-                    {"meta": meta, "data": data, "errors": minor_errors}, indent=2
+                    {"meta": meta, "data": data, "errors": minor_errors},
+                    indent=2,
                 )
             )
         else:
             f.write(json.dumps({"meta": meta, "data": data}, indent=2))
```

### Comparing `gnomonicus-2.5.3/gnomonicus.egg-info/PKG-INFO` & `gnomonicus-2.5.4/gnomonicus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnomonicus
-Version: 2.5.3
+Version: 2.5.4
 Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 Home-page: https://github.com/oxfordmmm/gnomonicus
 Author: Philip W Fowler, Jeremy Westhead
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford License, see LICENSE
 Keywords: gnomonicus,piezo,lodestone,clockwork,TB
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gnomonicus-2.5.3/setup.cfg` & `gnomonicus-2.5.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gnomonicus
-version = 2.5.3
+version = 2.5.4
 author = Philip W Fowler, Jeremy Westhead
 author_email = philip.fowler@ndm.ox.ac.uk
 description = Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/oxfordmmm/gnomonicus
 keywords = gnomonicus, piezo, lodestone, clockwork, TB
```

