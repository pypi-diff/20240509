# Comparing `tmp/blasttools-0.1.11.tar.gz` & `tmp/blasttools-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blasttools-0.1.11.tar", max compression
+gzip compressed data, was "blasttools-0.1.12.tar", max compression
```

## Comparing `blasttools-0.1.11.tar` & `blasttools-0.1.12.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-10-11 02:44:22.861784 blasttools-0.1.11/LICENSE
--rw-r--r--   0        0        0     2983 2024-05-09 01:30:40.236863 blasttools-0.1.11/README.md
--rw-r--r--   0        0        0        0 2023-10-11 02:44:42.585932 blasttools-0.1.11/blasttools/__init__.py
--rw-r--r--   0        0        0      290 2023-11-10 01:48:55.422665 blasttools-0.1.11/blasttools/__main__.py
--rw-r--r--   0        0        0    21682 2024-05-09 01:14:55.714936 blasttools-0.1.11/blasttools/blastapi.py
--rw-r--r--   0        0        0     8031 2024-05-09 01:14:28.614641 blasttools-0.1.11/blasttools/blastxml.py
--rw-r--r--   0        0        0     7313 2024-05-09 01:28:31.143529 blasttools-0.1.11/blasttools/cli.py
--rw-r--r--   0        0        0     2441 2023-12-06 01:23:32.917966 blasttools-0.1.11/blasttools/columns.py
--rw-r--r--   0        0        0      126 2024-04-19 05:53:19.292568 blasttools-0.1.11/blasttools/config.py
--rw-r--r--   0        0        0     1677 2023-11-10 01:43:26.653552 blasttools-0.1.11/blasttools/exact.py
--rw-r--r--   0        0        0     9842 2024-02-06 03:22:46.165796 blasttools-0.1.11/blasttools/plants.py
--rw-r--r--   0        0        0     7541 2024-05-09 01:14:29.802654 blasttools-0.1.11/blasttools/plants_ui.py
--rw-r--r--   0        0        0        0 2023-10-12 03:37:43.243775 blasttools-0.1.11/blasttools/py.typed
--rw-r--r--   0        0        0      558 2024-05-09 01:13:47.682193 blasttools-0.1.11/blasttools/translate.py
--rw-r--r--   0        0        0     1346 2024-05-09 01:02:38.839352 blasttools-0.1.11/blasttools/utils.py
--rw-r--r--   0        0        0      800 2024-05-09 01:31:27.589352 blasttools-0.1.11/pyproject.toml
--rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 blasttools-0.1.11/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-10-11 02:44:22.861784 blasttools-0.1.12/LICENSE
+-rw-r--r--   0        0        0     2983 2024-05-09 01:30:40.236863 blasttools-0.1.12/README.md
+-rw-r--r--   0        0        0        0 2023-10-11 02:44:42.585932 blasttools-0.1.12/blasttools/__init__.py
+-rw-r--r--   0        0        0      290 2023-11-10 01:48:55.422665 blasttools-0.1.12/blasttools/__main__.py
+-rw-r--r--   0        0        0    20571 2024-05-09 02:05:45.622412 blasttools-0.1.12/blasttools/blastapi.py
+-rw-r--r--   0        0        0     8081 2024-05-09 01:32:30.185998 blasttools-0.1.12/blasttools/blastxml.py
+-rw-r--r--   0        0        0     7355 2024-05-09 01:53:56.743166 blasttools-0.1.12/blasttools/cli.py
+-rw-r--r--   0        0        0     2441 2023-12-06 01:23:32.917966 blasttools-0.1.12/blasttools/columns.py
+-rw-r--r--   0        0        0      126 2024-04-19 05:53:19.292568 blasttools-0.1.12/blasttools/config.py
+-rw-r--r--   0        0        0     1754 2024-05-09 02:10:12.165137 blasttools-0.1.12/blasttools/exact.py
+-rw-r--r--   0        0        0     1207 2024-05-09 02:05:36.010314 blasttools-0.1.12/blasttools/options.py
+-rw-r--r--   0        0        0     9842 2024-02-06 03:22:46.165796 blasttools-0.1.12/blasttools/plants.py
+-rw-r--r--   0        0        0     7657 2024-05-09 02:05:36.010314 blasttools-0.1.12/blasttools/plants_ui.py
+-rw-r--r--   0        0        0        0 2023-10-12 03:37:43.243775 blasttools-0.1.12/blasttools/py.typed
+-rw-r--r--   0        0        0      409 2024-05-09 02:05:36.302317 blasttools-0.1.12/blasttools/translate.py
+-rw-r--r--   0        0        0     1647 2024-05-09 02:05:36.370317 blasttools-0.1.12/blasttools/utils.py
+-rw-r--r--   0        0        0      800 2024-05-09 02:02:56.956687 blasttools-0.1.12/pyproject.toml
+-rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 blasttools-0.1.12/PKG-INFO
```

### Comparing `blasttools-0.1.11/LICENSE` & `blasttools-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.11/README.md` & `blasttools-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.11/blasttools/blastapi.py` & `blasttools-0.1.12/blasttools/blastapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
-import sys
 import gzip
 import os
 import subprocess
+import sys
 from dataclasses import dataclass
 from functools import cache
 from pathlib import Path
 from shutil import which
 from typing import Any
 from typing import Iterator
 from typing import Sequence
 from uuid import uuid4
 
 import click
 import pandas as pd
-from Bio import SeqIO  # type: ignore
-from Bio.Seq import Seq  # type: ignore
-from Bio.SeqRecord import SeqRecord  # type: ignore
+from Bio import SeqIO
+from Bio.Seq import Seq
+from Bio.SeqRecord import SeqRecord
 from pandas.errors import UndefinedVariableError
 
 
 @cache
 def safe_which(cmd: str) -> str:
     r = which(cmd)
     if r is None:
@@ -57,18 +57,22 @@
     path: str | Path,
     with_description: bool = False,
     without_query_seq: bool = False,
 ) -> pd.DataFrame:
     """Read a Fasta file into a pandas dataframe"""
 
     def todict1(rec: SeqRecord) -> dict[str, str]:
-        return dict(id=rec.id, seq=str(rec.seq).upper())
+        return dict(id=rec.id or "", seq=str(rec.seq).upper())
 
     def todict2(rec: SeqRecord) -> dict[str, str]:
-        return dict(id=rec.id, seq=str(rec.seq).upper(), description=rec.description)
+        return dict(
+            id=rec.id or "",
+            seq=str(rec.seq).upper(),
+            description=rec.description,
+        )
 
     todict = todict2 if with_description else todict1
     qdf = pd.DataFrame([todict(rec) for rec in read_fasta(path)])
 
     if not qdf["id"].is_unique:
         raise click.ClickException(
             f'sequences IDs are not unique for query file "{path}"',
@@ -198,15 +202,17 @@
         blastdbs: Sequence[tuple[str, str | Path]],
         *,
         config,
     ) -> pd.DataFrame:
         res = []
         for species, blastdb in blastdbs:
             rdf = self.run(
-                queryfasta, blastdb, needs_translation=config.needs_translation
+                queryfasta,
+                blastdb,
+                needs_translation=config.needs_translation,
             )
 
             if config.with_subject_seq and "saccver" in rdf.columns:
                 saccver = list(set(rdf["saccver"]))
                 sdf = fetch_seq_df(saccver, blastdb)
                 rdf = pd.merge(rdf, sdf, left_on="saccver", right_on="saccver")
 
@@ -639,58 +645,14 @@
     """don't retain query sequence column (as seq)"""
     xml: bool = False
     """Use blast xml output to obtain match, query, sbjct sequences"""
     needs_translation: bool = False
     """query fasta contains mixed rna/dna/rna sequences too"""
 
 
-def blast_options(f):
-    f = click.option(
-        "--needs-translation",
-        is_flag=True,
-        help="query fasta contains rna/dna/cdna sequences too",
-    )(f)
-    f = click.option(
-        "--without-query-seq",
-        is_flag=True,
-        help="don't output query sequence",
-    )(f)
-    f = click.option("--xml", is_flag=True, help="run with xml output (for matches)")(f)
-    f = click.option(
-        "-t",
-        "--num-threads",
-        help="number of threads to use for blast",
-        default=1,
-    )(f)
-    f = click.option(
-        "--expr",
-        help="expression to minimize when looking for --best. e.g. ",
-        default=EVALUE,
-        show_default=True,
-    )(f)
-    f = click.option(
-        "-d",
-        "--with-description",
-        is_flag=True,
-        help="include query description in output",
-    )(f)
-    f = click.option(
-        "--with-seq",
-        "with_subject_seq",
-        is_flag=True,
-        help="add subject sequence data to output",
-    )(f)
-    f = click.option(
-        "--best",
-        default=0,
-        help="best (lowest) evalues [=0 take all]  (see also --expr)",
-    )(f)
-    return f
-
-
 def blastall(
     queryfasta: str,
     blastdbs: Sequence[str],
     *,
     config: BlastConfig = BlastConfig(),
 ) -> pd.DataFrame:
     from .blastxml import BlastXML
```

### Comparing `blasttools-0.1.11/blasttools/blastxml.py` & `blasttools-0.1.12/blasttools/blastxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-import sys
 import re
 import subprocess
+import sys
 from collections.abc import Sequence
 from dataclasses import asdict
 from dataclasses import dataclass
 from dataclasses import fields
 from pathlib import Path
 from typing import Any
 from typing import Iterator
@@ -105,16 +105,18 @@
     ) -> pd.DataFrame:
         todict = self.todict
         return pd.DataFrame(
             [
                 todict(hit)
                 for hit in hits(
                     self.runner(
-                        queryfasta, blastdb, needs_translation=needs_translation
-                    )
+                        queryfasta,
+                        blastdb,
+                        needs_translation=needs_translation,
+                    ),
                 )
             ],
         )
 
 
 def out5_to_df(xmlfile: str) -> pd.DataFrame:
     def run() -> Iterator[Blast]:
```

### Comparing `blasttools-0.1.11/blasttools/cli.py` & `blasttools-0.1.12/blasttools/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from __future__ import annotations
 
 from collections.abc import Sequence
 
 import click
 
-from .blastapi import blast_options
-from .blastapi import blastall
-from .blastapi import BlastConfig
-from .blastapi import buildall
-from .blastapi import check_ext
-from .blastapi import fasta_merge
-from .blastapi import fasta_xref
-from .blastapi import list_out
-from .blastapi import read_df
-from .blastapi import save_df
-from .blastapi import test_save
-from .blastapi import toblastdb
+from .options import blast_options
 
 
 @click.group(
-    epilog=click.style("Commands for turning blast queries into pandas dataframes.\n", fg="magenta"),
+    epilog=click.style(
+        "Commands for turning blast queries into pandas dataframes.\n",
+        fg="magenta",
+    ),
 )
 @click.version_option()
 def blast() -> None:
     pass
 
 
 @blast.command()
@@ -42,28 +34,31 @@
 
 @blast.command(name="fasta-merge")
 @click.argument("fasta1", type=click.Path(exists=True, dir_okay=False))
 @click.argument("fasta2", type=click.Path(exists=True, dir_okay=False))
 @click.argument("outfasta", type=click.Path(exists=False, dir_okay=False))
 def fasta_merge_cmd(fasta1: str, fasta2: str, outfasta: str) -> None:
     """merge 2 fasta files based on sequence identity"""
+    from .blastapi import fasta_merge
+
     fasta_merge(fasta1, fasta2, outfasta)
 
 
 @blast.command(name="fasta-xref")
 @click.option(
     "--out",
     help="output filename (default is to write CSV to stdout)",
     type=click.Path(dir_okay=False),
 )
 @click.argument("fasta1", type=click.Path(exists=True, dir_okay=False))
 @click.argument("fasta2", type=click.Path(exists=True, dir_okay=False))
 def fasta_xref_cmd(fasta1: str, fasta2: str, out: str | None) -> None:
     """match IDs based on sequence identity"""
     import sys
+    from .blastapi import fasta_xref, save_df, test_save
 
     if out is not None:
         test_save(out)
     df = fasta_xref(fasta1, fasta2)
 
     if out is not None:
         save_df(df, out)
@@ -93,14 +88,16 @@
 def build_cmd(
     fastas: Sequence[str],
     builddir: str | None,
     merge: str | None,
     nucl: bool,
 ) -> None:
     """Build blast databases from fasta files"""
+    from .blastapi import buildall
+
     buildall(fastas, builddir=builddir, merge=merge, blastp=not nucl)
 
 
 @blast.command(name="blast")
 @click.option(
     "--out",
     help="output filename (default is to write <query>.csv)",
@@ -128,15 +125,24 @@
     num_threads: int,
     with_description: bool,
     expr: str,
     without_query_seq: bool,
     needs_translation: bool,
 ) -> None:
     """Run a blast query over specified databases"""
-    from .blastapi import mkheader, has_pdatabase
+    from .blastapi import (
+        mkheader,
+        has_pdatabase,
+        blastall,
+        save_df,
+        test_save,
+        check_ext,
+        toblastdb,
+        BlastConfig,
+    )
 
     if len(blastdbs) == 0:
         return
 
     if out is not None:
         check_ext(out)  # fail early
         test_save(out)
@@ -201,14 +207,15 @@
     type=click.Path(dir_okay=False),
 )
 @click.argument("dataframes", nargs=-1, type=click.Path(dir_okay=False, exists=True))
 def concat_cmd(dataframes: Sequence[str], out: str | None) -> None:
     """Concatenate multiple saved DataFrames"""
     import sys
     import pandas as pd
+    from .blastapi import read_df, save_df, test_save, check_ext
 
     if out is not None:
         check_ext(out)
         test_save(out)
 
     dfs = []
     for df in dataframes:
@@ -247,14 +254,15 @@
     batch: int,
     fmt: str | None,
     directory: str | None,
     use_null: bool,
 ) -> None:
     """Split a fasta file into batches"""
     from .utils import split_fasta
+    from .blastapi import list_out
 
     ret = split_fasta(fastafile, batch, target_dir=directory, fmt=fmt)
     if ret is None:
         raise click.ClickException(f"Can't split fasta file {fastafile}")
     # So you can do say:
     # fastas=$(blasttools fasta-split fastafile.fa.gz 20000)
     # parallel blasttools blast --out=my{}.pkl ::: $fastas ::: blastdb
```

### Comparing `blasttools-0.1.11/blasttools/columns.py` & `blasttools-0.1.12/blasttools/columns.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.11/blasttools/exact.py` & `blasttools-0.1.12/blasttools/exact.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from collections.abc import Sequence
 from typing import Any
+from typing import TYPE_CHECKING
 
 import click
-import pandas as pd
 
-from .blastapi import check_ext
-from .blastapi import fasta_to_df
-from .blastapi import read_fasta
-from .blastapi import save_df
-from .blastapi import test_save
 from .cli import blast
 
+if TYPE_CHECKING:
+    import pandas
+
+
+def exact(query: str, subjects: Sequence[str]) -> pandas.DataFrame:
+    import pandas as pd
+    from .blastapi import read_fasta, fasta_to_df
 
-def exact(query: str, subjects: Sequence[str]) -> pd.DataFrame:
     df = fasta_to_df(query, with_description=True)
     dd = defaultdict(list)
     for subject in subjects:
         for rec in read_fasta(subject):
             for r in df.itertuples():
                 if str(r.seq).upper() in str(rec.seq).upper():
                     dd[r.id].append(rec.id)
@@ -27,16 +28,15 @@
     ret: dict[str, list[Any]] = dict(id=[], description=[], exact=[], subject=[])
     for r in df.itertuples():
         found = r.id in dd
         ret["id"].append(r.id)
         ret["description"].append(r.description)
         ret["exact"].append(found)
         if found:
-            ret["subject"].append(", ".join(dd[r.id]))
-        else:
+            ret["subject"].append(", ".join(str(s) for s in dd[r.id]))
             ret["subject"].append("")
 
     return pd.DataFrame(ret)
 
 
 @blast.command("exact")
 @click.option(
@@ -44,14 +44,18 @@
     help="output filename (default is to write <query>.csv)",
     type=click.Path(dir_okay=False),
 )
 @click.argument("query", type=click.Path(exists=True, dir_okay=False))
 @click.argument("fastas", nargs=-1)
 def exact_cmd(query: str, fastas: Sequence[str], out: str | None) -> None:
     "Try and match sequences exactly"
+    from .blastapi import check_ext
+    from .blastapi import save_df
+    from .blastapi import test_save
+
     if out is not None:
         check_ext(out)
         test_save(out)
     df = exact(query, fastas)
     if out is None:
         out = query + ".csv"
     save_df(df, out, index=False)
```

### Comparing `blasttools-0.1.11/blasttools/plants.py` & `blasttools-0.1.12/blasttools/plants.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.11/blasttools/plants_ui.py` & `blasttools-0.1.12/blasttools/plants_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Sequence
 
 import click
 
-from .blastapi import blast_options
-from .blastapi import BlastConfig
-from .blastapi import check_ext
-from .blastapi import mkheader
-from .blastapi import save_df
-from .blastapi import test_save
 from .cli import blast
 from .config import RELEASE
-from .plants import blastall
-from .plants import build
-from .plants import fetch_fastas
-from .plants import find_fasta_names
-from .plants import find_species
-from .plants import orthologs
+from .options import blast_options
 
 
 @dataclass
 class Config:
     release: int = RELEASE
 
 
@@ -67,14 +56,16 @@
     type=click.Path(file_okay=False, dir_okay=True),
     help="build all 'ensembleblast-{release}' directories in this directory",
 )
 @click.argument("species", nargs=-1)
 @pass_config
 def build_cmd(cfg: Config, species: Sequence[str], builddir: str | None) -> None:
     """Download and build blast databases"""
+    from .plants import build
+
     build(species, release=cfg.release, path=builddir)
 
 
 @plants.command(name="blast")
 @click.option(
     "--out",
     help="output filename (default is to write <query>.csv)",
@@ -128,14 +119,20 @@
     without_query_seq: bool,
     xml: bool,
     needs_translation: bool,
 ) -> None:
     """Run blast on query fasta file"""
     from .plants import available_species
     from .columns import VALID
+    from .blastapi import BlastConfig
+    from .blastapi import check_ext
+    from .blastapi import mkheader
+    from .blastapi import save_df
+    from .blastapi import test_save
+    from .plants import blastall
 
     if len(species) == 0 and not all_db:
         return
     if out is not None:
         check_ext(out)
         test_save(out)
 
@@ -173,28 +170,31 @@
 
 
 @plants.command(name="fasta-fetch")
 @click.argument("species", nargs=-1)
 @pass_config
 def fasta_fetch_cmd(cfg: Config, species: Sequence[str]) -> None:
     """Download fasta files from FTP site"""
+    from .plants import fetch_fastas
+
     fetch_fastas(species, release=cfg.release)
 
 
 @plants.command("fasta-filenames")
 @click.option("-f", "--full", is_flag=True, help="show full URL to file")
 @click.argument("species", nargs=-1)
 @pass_config
 def fasta_filenames_cmd(
     cfg: Config,
     species: Sequence[str],
     full: bool,
 ) -> None:
     """Find fasta filenames for plant species"""
     from .plants import ENSEMBL
+    from .plants import find_fasta_names
 
     for info in find_fasta_names(species, release=cfg.release):
         if info.fasta is None:
             click.secho(f"{info.species}: no fasta!", fg="red", bold=True)
         else:
             if full:
                 fasta = ENSEMBL.format(
@@ -207,14 +207,16 @@
                 click.secho(f"{info.species}: {info.fasta}")
 
 
 @plants.command(name="species")
 @pass_config
 def species_cmd(cfg: Config) -> None:
     """Available species at Ensembl"""
+    from .plants import find_species
+
     sl = find_species(cfg.release)
     for s in sorted(sl):
         click.echo(s)
 
 
 @plants.command(name="releases")
 @click.option("--max", "max_only", help="max version", is_flag=True)
@@ -250,14 +252,17 @@
     with_description: bool,
     expr: str,
     without_query_seq: bool,
     xml: bool,
     needs_translation: bool,
 ) -> None:
     """Create an ortholog DataFrame between two species"""
+    from .blastapi import BlastConfig, check_ext, test_save, save_df
+    from .plants import orthologs
+
     config = BlastConfig(
         best=best,
         with_subject_seq=with_subject_seq,
         header=None,
         num_threads=num_threads,
         with_description=with_description,
         expr=expr,
```

### Comparing `blasttools-0.1.11/blasttools/utils.py` & `blasttools-0.1.12/blasttools/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from itertools import chain
 from itertools import islice
-
-
 from os.path import splitext
 from pathlib import Path
 from typing import Iterator
 from typing import TypeVar
 
+from Bio.SeqRecord import SeqRecord
+
 from .blastapi import read_fasta
 from .blastapi import write_fasta_iter
 
 sentinel = object()
 
 T = TypeVar("T")
 
@@ -50,7 +50,15 @@
         write_fasta_iter(sname, it)
 
     return ret
 
 
 def is_rna(s: str) -> bool:
     return set(s).issubset({"A", "C", "G", "U", "T"})
+
+
+def translate(fasta: str | Path) -> Iterator[SeqRecord]:
+    for rec in read_fasta(fasta):
+        if is_rna(str(rec.seq)):
+            rec.seq = rec.seq.transcribe().translate()
+            # print('translated', rec.id,rec.seq, file=sys.stderr)
+        yield rec
```

### Comparing `blasttools-0.1.11/pyproject.toml` & `blasttools-0.1.12/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blasttools"
-version = "0.1.11"
+version = "0.1.12"
 description = "Commands for turning blast queries into pandas dataframes."
 authors = ["Ian Castleden <ian.castleden@uwa.edu.au>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
```

### Comparing `blasttools-0.1.11/PKG-INFO` & `blasttools-0.1.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blasttools
-Version: 0.1.11
+Version: 0.1.12
 Summary: Commands for turning blast queries into pandas dataframes.
 License: MIT
 Author: Ian Castleden
 Author-email: ian.castleden@uwa.edu.au
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

