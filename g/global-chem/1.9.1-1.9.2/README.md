# Comparing `tmp/global_chem-1.9.1.tar.gz` & `tmp/global_chem-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_chem-1.9.1.tar", last modified: Thu May  9 19:24:48 2024, max compression
+gzip compressed data, was "global_chem-1.9.2.tar", last modified: Thu May  9 20:10:22 2024, max compression
```

## Comparing `global_chem-1.9.1.tar` & `global_chem-1.9.2.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.942093 global_chem-1.9.1/
--rw-r--r--   0 sulimansharif   (501) staff       (20)    54389 2024-05-09 19:24:48.941712 global_chem-1.9.1/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)    50166 2024-05-09 19:23:56.000000 global_chem-1.9.1/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.845515 global_chem-1.9.1/global_chem/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7089 2024-05-09 19:23:56.000000 global_chem-1.9.1/global_chem/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      238 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/__main__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.850365 global_chem-1.9.1/global_chem/animals/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/animals/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.850956 global_chem-1.9.1/global_chem/animals/snakes/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/animals/snakes/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    38357 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/animals/snakes/drugs_from_snake_venom.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      321 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/cli.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.853105 global_chem-1.9.1/global_chem/education/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/education/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.853617 global_chem-1.9.1/global_chem/education/cengage/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/education/cengage/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4602 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.856552 global_chem-1.9.1/global_chem/environment/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/environment/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9553 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/environment/alternative_jet_fuels.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2106 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/environment/chemicals_from_biomass.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9696 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/environment/emerging_perfluoroalkyls.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.857498 global_chem-1.9.1/global_chem/food/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.862571 global_chem-1.9.1/global_chem/food/color_additives/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5620 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_five.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    26611 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_four.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6232 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_one.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    12448 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_seven.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5657 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_six.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5343 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_three.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5111 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_two.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.863085 global_chem-1.9.1/global_chem/food/fruits/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/food/fruits/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.867639 global_chem-1.9.1/global_chem/food/fruits/mango/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/food/fruits/mango/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1287 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_amino_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1778 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_fatty_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1367 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_flavonoids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      886 2024-05-09 19:23:56.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_phenolic_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5489 2024-05-09 19:18:27.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_phyto_compounds.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1084 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_vitamins.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.868604 global_chem-1.9.1/global_chem/food/salt/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/salt/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2304 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/salt/salt.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.869217 global_chem-1.9.1/global_chem/formulation/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.870092 global_chem-1.9.1/global_chem/formulation/excipients/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1783 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/allergen_inactive_ingredients.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.871215 global_chem-1.9.1/global_chem/formulation/excipients/biopharmaceutics_class_three/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/biopharmaceutics_class_three/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4134 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.872522 global_chem-1.9.1/global_chem/formulation/excipients/monoclonal_antibodies/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/monoclonal_antibodies/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4080 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    47486 2024-05-09 19:23:56.000000 global_chem-1.9.1/global_chem/global_chem.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.873941 global_chem-1.9.1/global_chem/interstellar_space/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/interstellar_space/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      678 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/interstellar_space/asteroid_ryugu.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    10891 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/interstellar_space/interstellar_space.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.874647 global_chem-1.9.1/global_chem/materials/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.875477 global_chem-1.9.1/global_chem/materials/clay/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/clay/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7263 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/clay/montmorillonite_adsorption.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.876663 global_chem-1.9.1/global_chem/materials/polymers/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      116 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/polymers/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    18019 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/polymers/common_monomer_repeating_units.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.877650 global_chem-1.9.1/global_chem/medicinal_chemistry/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.894596 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1263 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      535 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/alcohols.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      757 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/aldehydes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1083 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/amino_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5131 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)   206471 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      914 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      997 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1937 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2941 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      959 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/ketones.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1123 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1321 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    32010 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      540 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/pigments.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    33609 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1122 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/steroids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2032 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/sugars.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5409 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/terpenes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      418 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/vitamins.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.896041 global_chem-1.9.1/global_chem/medicinal_chemistry/chinese/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/chinese/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1103 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.898198 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    13832 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2694 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    14543 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/rings_in_drugs.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.901764 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    48105 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    22232 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7459 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.902997 global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3465 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3181 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.910082 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/access_group_antibiotics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/anaesthetics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/anaphylaxis_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/anticonvulsants.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/antidotes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/antifilarials.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/antischistosomals_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/cysticidal_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/intestinal_anthelminthics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/medical_gases.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/non_steroidal_anti_inflammatory_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/opioid_analgesics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/palliative_care.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/preoperative_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/reserve_group_antibiotics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/watch_group_antibiotics.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.913668 global_chem-1.9.1/global_chem/miscellaneous/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2139 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/amino_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9650 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/open_smiles.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      396 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/regex_patterns.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3724 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/vitamins.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.921409 global_chem-1.9.1/global_chem/narcotics/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      370 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/narcotics/black_market.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    41346 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/pihkal.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2155 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_five.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    17624 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_four.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    57945 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_one.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4816 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_three.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    14153 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_two.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.922047 global_chem-1.9.1/global_chem/organic_synthesis/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.922556 global_chem-1.9.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7973 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.923545 global_chem-1.9.1/global_chem/organic_synthesis/protecting_groups/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/protecting_groups/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    42927 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.924821 global_chem-1.9.1/global_chem/organic_synthesis/solvents/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/solvents/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5293 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/solvents/common_organic_solvents.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.925757 global_chem-1.9.1/global_chem/peptides/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/peptides/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3489 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/peptides/lanthipeptides.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.926504 global_chem-1.9.1/global_chem/proteins/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.927057 global_chem-1.9.1/global_chem/proteins/kinases/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.928058 global_chem-1.9.1/global_chem/proteins/kinases/braf/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/braf/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7617 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/braf/braf_inhibitors.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.929138 global_chem-1.9.1/global_chem/proteins/kinases/scaffolds/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/scaffolds/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5167 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.929749 global_chem-1.9.1/global_chem/sex/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.930247 global_chem-1.9.1/global_chem/sex/contraceptives/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/contraceptives/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/contraceptives/oral_contraceptives.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.932170 global_chem-1.9.1/global_chem/sex/exsens/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/exsens/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    16558 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/exsens/exsens_products.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9160 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/exsens/lube.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.934273 global_chem-1.9.1/global_chem/sex/tainted_sexual_enhancements/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/tainted_sexual_enhancements/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1269 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.937329 global_chem-1.9.1/global_chem/skin/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.938150 global_chem-1.9.1/global_chem/skin/sunscreen/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/sunscreen/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/sunscreen/sunscreen.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.939093 global_chem-1.9.1/global_chem/skin/transdermal_and_dermal_delivery/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/transdermal_and_dermal_delivery/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9628 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.940446 global_chem-1.9.1/global_chem/warfare/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/warfare/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2511 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/warfare/organophosphorous_nerve_agents.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.850012 global_chem-1.9.1/global_chem.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)    54389 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)     8056 2024-05-09 19:24:47.000000 global_chem-1.9.1/global_chem.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)      592 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/requires.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       12 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-09 19:24:48.942274 global_chem-1.9.1/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2371 2024-05-09 19:24:36.000000 global_chem-1.9.1/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.741930 global_chem-1.9.2/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    54389 2024-05-09 20:10:22.741422 global_chem-1.9.2/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    50166 2024-05-09 19:23:56.000000 global_chem-1.9.2/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.603684 global_chem-1.9.2/global_chem/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7089 2024-05-09 19:23:56.000000 global_chem-1.9.2/global_chem/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      238 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/__main__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.611221 global_chem-1.9.2/global_chem/animals/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/animals/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.612002 global_chem-1.9.2/global_chem/animals/snakes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/animals/snakes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    38357 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/animals/snakes/drugs_from_snake_venom.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      321 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/cli.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.613131 global_chem-1.9.2/global_chem/education/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/education/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.614361 global_chem-1.9.2/global_chem/education/cengage/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/education/cengage/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4602 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.619427 global_chem-1.9.2/global_chem/environment/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/environment/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9553 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/environment/alternative_jet_fuels.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2106 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/environment/chemicals_from_biomass.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9696 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/environment/emerging_perfluoroalkyls.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.622699 global_chem-1.9.2/global_chem/food/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.629151 global_chem-1.9.2/global_chem/food/color_additives/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/color_additives/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5620 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/color_additives/fda_list_five.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    26611 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/color_additives/fda_list_four.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6232 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/color_additives/fda_list_one.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    12448 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/color_additives/fda_list_seven.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5657 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/color_additives/fda_list_six.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5343 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/color_additives/fda_list_three.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5111 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/color_additives/fda_list_two.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.629824 global_chem-1.9.2/global_chem/food/fruits/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.9.2/global_chem/food/fruits/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.638591 global_chem-1.9.2/global_chem/food/fruits/mango/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.9.2/global_chem/food/fruits/mango/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1287 2024-05-09 19:17:09.000000 global_chem-1.9.2/global_chem/food/fruits/mango/mango_amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1778 2024-05-09 19:17:09.000000 global_chem-1.9.2/global_chem/food/fruits/mango/mango_fatty_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1367 2024-05-09 19:17:09.000000 global_chem-1.9.2/global_chem/food/fruits/mango/mango_flavonoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      886 2024-05-09 19:23:56.000000 global_chem-1.9.2/global_chem/food/fruits/mango/mango_phenolic_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5488 2024-05-09 20:09:58.000000 global_chem-1.9.2/global_chem/food/fruits/mango/mango_phyto_compounds.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1084 2024-05-09 19:17:09.000000 global_chem-1.9.2/global_chem/food/fruits/mango/mango_vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.640018 global_chem-1.9.2/global_chem/food/salt/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/salt/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2304 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/food/salt/salt.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.640705 global_chem-1.9.2/global_chem/formulation/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/formulation/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.641838 global_chem-1.9.2/global_chem/formulation/excipients/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/formulation/excipients/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1783 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/formulation/excipients/allergen_inactive_ingredients.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.643083 global_chem-1.9.2/global_chem/formulation/excipients/biopharmaceutics_class_three/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/formulation/excipients/biopharmaceutics_class_three/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4134 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.644416 global_chem-1.9.2/global_chem/formulation/excipients/monoclonal_antibodies/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/formulation/excipients/monoclonal_antibodies/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4080 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    47486 2024-05-09 19:23:56.000000 global_chem-1.9.2/global_chem/global_chem.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.646358 global_chem-1.9.2/global_chem/interstellar_space/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/interstellar_space/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      678 2023-06-27 14:15:06.000000 global_chem-1.9.2/global_chem/interstellar_space/asteroid_ryugu.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    10891 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/interstellar_space/interstellar_space.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.646921 global_chem-1.9.2/global_chem/materials/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/materials/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.647732 global_chem-1.9.2/global_chem/materials/clay/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/materials/clay/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7263 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/materials/clay/montmorillonite_adsorption.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.648803 global_chem-1.9.2/global_chem/materials/polymers/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      116 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/materials/polymers/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    18019 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/materials/polymers/common_monomer_repeating_units.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.649615 global_chem-1.9.2/global_chem/medicinal_chemistry/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.674541 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1263 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      535 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/alcohols.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      757 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/aldehydes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1083 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5131 2023-06-27 14:15:06.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)   206471 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      914 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      997 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1937 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2941 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      959 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/ketones.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1123 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1321 2023-06-27 14:15:06.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    32010 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      540 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/pigments.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    33609 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1122 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/steroids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2032 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/sugars.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5409 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/terpenes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      418 2024-05-09 19:17:05.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.675607 global_chem-1.9.2/global_chem/medicinal_chemistry/chinese/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/chinese/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1103 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.678242 global_chem-1.9.2/global_chem/medicinal_chemistry/rings/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/rings/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    13832 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2694 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    14543 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/rings/rings_in_drugs.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.684732 global_chem-1.9.2/global_chem/medicinal_chemistry/scaffolds/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/scaffolds/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    48105 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    22232 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7459 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.695727 global_chem-1.9.2/global_chem/medicinal_chemistry/warheads/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/warheads/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3465 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3181 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.710658 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/access_group_antibiotics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/anaesthetics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/anaphylaxis_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/anticonvulsants.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/antidotes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/antifilarials.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/antischistosomals_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/cysticidal_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/intestinal_anthelminthics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/medical_gases.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/non_steroidal_anti_inflammatory_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/opioid_analgesics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/palliative_care.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/preoperative_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/reserve_group_antibiotics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/medicinal_chemistry/world_health_organization/watch_group_antibiotics.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.714087 global_chem-1.9.2/global_chem/miscellaneous/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/miscellaneous/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2139 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/miscellaneous/amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9650 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/miscellaneous/open_smiles.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      396 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/miscellaneous/regex_patterns.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3724 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/miscellaneous/vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.721701 global_chem-1.9.2/global_chem/narcotics/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/narcotics/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      370 2024-05-09 19:17:09.000000 global_chem-1.9.2/global_chem/narcotics/black_market.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    41346 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/narcotics/pihkal.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2155 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/narcotics/schedule_five.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    17624 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/narcotics/schedule_four.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    57945 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/narcotics/schedule_one.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4816 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/narcotics/schedule_three.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    14153 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/narcotics/schedule_two.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.723781 global_chem-1.9.2/global_chem/organic_synthesis/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/organic_synthesis/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.724627 global_chem-1.9.2/global_chem/organic_synthesis/bidendate_phosphine_ligands/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/organic_synthesis/bidendate_phosphine_ligands/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7973 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.725984 global_chem-1.9.2/global_chem/organic_synthesis/protecting_groups/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/organic_synthesis/protecting_groups/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    42927 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.728144 global_chem-1.9.2/global_chem/organic_synthesis/solvents/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/organic_synthesis/solvents/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5293 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/organic_synthesis/solvents/common_organic_solvents.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.729434 global_chem-1.9.2/global_chem/peptides/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/peptides/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3489 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/peptides/lanthipeptides.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.730028 global_chem-1.9.2/global_chem/proteins/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/proteins/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.730371 global_chem-1.9.2/global_chem/proteins/kinases/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/proteins/kinases/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.730977 global_chem-1.9.2/global_chem/proteins/kinases/braf/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/proteins/kinases/braf/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7617 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/proteins/kinases/braf/braf_inhibitors.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.731730 global_chem-1.9.2/global_chem/proteins/kinases/scaffolds/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/proteins/kinases/scaffolds/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5167 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.732222 global_chem-1.9.2/global_chem/sex/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/sex/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.733057 global_chem-1.9.2/global_chem/sex/contraceptives/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/sex/contraceptives/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/sex/contraceptives/oral_contraceptives.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.734679 global_chem-1.9.2/global_chem/sex/exsens/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/sex/exsens/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    16558 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/sex/exsens/exsens_products.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9160 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/sex/exsens/lube.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.735389 global_chem-1.9.2/global_chem/sex/tainted_sexual_enhancements/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/sex/tainted_sexual_enhancements/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1269 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.736241 global_chem-1.9.2/global_chem/skin/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/skin/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.737649 global_chem-1.9.2/global_chem/skin/sunscreen/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/skin/sunscreen/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/skin/sunscreen/sunscreen.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.739098 global_chem-1.9.2/global_chem/skin/transdermal_and_dermal_delivery/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/skin/transdermal_and_dermal_delivery/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9628 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.740148 global_chem-1.9.2/global_chem/warfare/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/warfare/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2511 2023-04-11 15:37:28.000000 global_chem-1.9.2/global_chem/warfare/organophosphorous_nerve_agents.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 20:10:22.610627 global_chem-1.9.2/global_chem.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    54389 2024-05-09 20:10:21.000000 global_chem-1.9.2/global_chem.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     8056 2024-05-09 20:10:21.000000 global_chem-1.9.2/global_chem.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-09 20:10:21.000000 global_chem-1.9.2/global_chem.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-09 20:10:21.000000 global_chem-1.9.2/global_chem.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      592 2024-05-09 20:10:21.000000 global_chem-1.9.2/global_chem.egg-info/requires.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       12 2024-05-09 20:10:21.000000 global_chem-1.9.2/global_chem.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-09 20:10:22.742107 global_chem-1.9.2/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2371 2024-05-09 20:10:14.000000 global_chem-1.9.2/setup.py
```

### Comparing `global_chem-1.9.1/PKG-INFO` & `global_chem-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global_chem
-Version: 1.9.1
+Version: 1.9.2
 Summary: UNKNOWN
 Home-page: https://www.github.com/Sulstice/global-chem
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: MPL 2.0
 Description: <h1 align="center">Organizing The Chemical Universe</h1>
```

### Comparing `global_chem-1.9.1/README.md` & `global_chem-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/__init__.py` & `global_chem-1.9.2/global_chem/__init__.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/animals/snakes/drugs_from_snake_venom.py` & `global_chem-1.9.2/global_chem/animals/snakes/drugs_from_snake_venom.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py` & `global_chem-1.9.2/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/environment/alternative_jet_fuels.py` & `global_chem-1.9.2/global_chem/environment/alternative_jet_fuels.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/environment/chemicals_from_biomass.py` & `global_chem-1.9.2/global_chem/environment/chemicals_from_biomass.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/environment/emerging_perfluoroalkyls.py` & `global_chem-1.9.2/global_chem/environment/emerging_perfluoroalkyls.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/color_additives/fda_list_five.py` & `global_chem-1.9.2/global_chem/food/color_additives/fda_list_five.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/color_additives/fda_list_four.py` & `global_chem-1.9.2/global_chem/food/color_additives/fda_list_four.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/color_additives/fda_list_one.py` & `global_chem-1.9.2/global_chem/food/color_additives/fda_list_one.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/color_additives/fda_list_seven.py` & `global_chem-1.9.2/global_chem/food/color_additives/fda_list_seven.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/color_additives/fda_list_six.py` & `global_chem-1.9.2/global_chem/food/color_additives/fda_list_six.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/color_additives/fda_list_three.py` & `global_chem-1.9.2/global_chem/food/color_additives/fda_list_three.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/color_additives/fda_list_two.py` & `global_chem-1.9.2/global_chem/food/color_additives/fda_list_two.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/fruits/mango/mango_amino_acids.py` & `global_chem-1.9.2/global_chem/food/fruits/mango/mango_amino_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/fruits/mango/mango_fatty_acids.py` & `global_chem-1.9.2/global_chem/food/fruits/mango/mango_fatty_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/fruits/mango/mango_flavonoids.py` & `global_chem-1.9.2/global_chem/food/fruits/mango/mango_flavonoids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/fruits/mango/mango_phenolic_acids.py` & `global_chem-1.9.2/global_chem/food/fruits/mango/mango_phenolic_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/fruits/mango/mango_phyto_compounds.py` & `global_chem-1.9.2/global_chem/food/fruits/mango/mango_phyto_compounds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 class MangoPhytocompounds(object):
     
   def __init__(self):
       
-      self.name = 'mango_phytocompounds'
-
+      self.name = 'mango_phyto_compounds'
 
   @staticmethod
   def get_smiles():
 
       smiles = {
         'arginine': 'C(CC(C(=O)O)N)CN=C(N)N',
         'cysteine': 'C([C@@H](C(=O)O)N)S',
```

### Comparing `global_chem-1.9.1/global_chem/food/fruits/mango/mango_vitamins.py` & `global_chem-1.9.2/global_chem/food/fruits/mango/mango_vitamins.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/food/salt/salt.py` & `global_chem-1.9.2/global_chem/food/salt/salt.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/formulation/excipients/allergen_inactive_ingredients.py` & `global_chem-1.9.2/global_chem/formulation/excipients/allergen_inactive_ingredients.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py` & `global_chem-1.9.2/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py` & `global_chem-1.9.2/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/global_chem.py` & `global_chem-1.9.2/global_chem/global_chem.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/interstellar_space/asteroid_ryugu.py` & `global_chem-1.9.2/global_chem/interstellar_space/asteroid_ryugu.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/interstellar_space/interstellar_space.py` & `global_chem-1.9.2/global_chem/interstellar_space/interstellar_space.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/materials/clay/montmorillonite_adsorption.py` & `global_chem-1.9.2/global_chem/materials/clay/montmorillonite_adsorption.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/materials/polymers/common_monomer_repeating_units.py` & `global_chem-1.9.2/global_chem/materials/polymers/common_monomer_repeating_units.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/acids.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/alcohols.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/alcohols.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/aldehydes.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/aldehydes.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/amino_acids.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/amino_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/ketones.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/ketones.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/pigments.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/pigments.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/steroids.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/steroids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/sugars.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/sugars.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/terpenes.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/cannabinoids/terpenes.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/rings/rings_in_drugs.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/rings/rings_in_drugs.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py` & `global_chem-1.9.2/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/miscellaneous/amino_acids.py` & `global_chem-1.9.2/global_chem/miscellaneous/amino_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/miscellaneous/open_smiles.py` & `global_chem-1.9.2/global_chem/miscellaneous/open_smiles.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/miscellaneous/vitamins.py` & `global_chem-1.9.2/global_chem/miscellaneous/vitamins.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/narcotics/pihkal.py` & `global_chem-1.9.2/global_chem/narcotics/pihkal.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/narcotics/schedule_five.py` & `global_chem-1.9.2/global_chem/narcotics/schedule_five.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/narcotics/schedule_four.py` & `global_chem-1.9.2/global_chem/narcotics/schedule_four.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/narcotics/schedule_one.py` & `global_chem-1.9.2/global_chem/narcotics/schedule_one.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/narcotics/schedule_three.py` & `global_chem-1.9.2/global_chem/narcotics/schedule_three.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/narcotics/schedule_two.py` & `global_chem-1.9.2/global_chem/narcotics/schedule_two.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py` & `global_chem-1.9.2/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py` & `global_chem-1.9.2/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/organic_synthesis/solvents/common_organic_solvents.py` & `global_chem-1.9.2/global_chem/organic_synthesis/solvents/common_organic_solvents.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/peptides/lanthipeptides.py` & `global_chem-1.9.2/global_chem/peptides/lanthipeptides.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/proteins/kinases/braf/braf_inhibitors.py` & `global_chem-1.9.2/global_chem/proteins/kinases/braf/braf_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py` & `global_chem-1.9.2/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/sex/contraceptives/oral_contraceptives.py` & `global_chem-1.9.2/global_chem/sex/contraceptives/oral_contraceptives.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/sex/exsens/exsens_products.py` & `global_chem-1.9.2/global_chem/sex/exsens/exsens_products.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/sex/exsens/lube.py` & `global_chem-1.9.2/global_chem/sex/exsens/lube.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py` & `global_chem-1.9.2/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py` & `global_chem-1.9.2/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem/warfare/organophosphorous_nerve_agents.py` & `global_chem-1.9.2/global_chem/warfare/organophosphorous_nerve_agents.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem.egg-info/PKG-INFO` & `global_chem-1.9.2/global_chem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global-chem
-Version: 1.9.1
+Version: 1.9.2
 Summary: UNKNOWN
 Home-page: https://www.github.com/Sulstice/global-chem
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: MPL 2.0
 Description: <h1 align="center">Organizing The Chemical Universe</h1>
```

### Comparing `global_chem-1.9.1/global_chem.egg-info/SOURCES.txt` & `global_chem-1.9.2/global_chem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/global_chem.egg-info/requires.txt` & `global_chem-1.9.2/global_chem.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `global_chem-1.9.1/setup.py` & `global_chem-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 else:
     long_description = 'GlobalChem - Your Chemical Knowledge Graph for Chemistry'
 
 # exec
 # ----
 setup(
     name="global_chem",
-    version="1.9.1",
+    version="1.9.2",
     packages=find_packages(),
     license='MPL 2.0',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/Sulstice/global-chem",
     install_requires=[],
     long_description=long_description,
```

