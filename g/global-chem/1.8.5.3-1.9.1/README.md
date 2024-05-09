# Comparing `tmp/global_chem-1.8.5.3.tar.gz` & `tmp/global_chem-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_chem-1.8.5.3.tar", last modified: Thu Feb 22 17:40:48 2024, max compression
+gzip compressed data, was "global_chem-1.9.1.tar", last modified: Thu May  9 19:24:48 2024, max compression
```

## Comparing `global_chem-1.8.5.3.tar` & `global_chem-1.9.1.tar`

### file list

```diff
@@ -1,210 +1,200 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.293907 global_chem-1.8.5.3/
--rw-r--r--   0 sulimansharif   (501) staff       (20)    54028 2024-02-22 17:40:48.293250 global_chem-1.8.5.3/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)    49668 2023-09-25 17:05:47.000000 global_chem-1.8.5.3/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.905481 global_chem-1.8.5.3/global_chem/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7839 2023-11-27 15:26:11.000000 global_chem-1.8.5.3/global_chem/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      238 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/__main__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.913196 global_chem-1.8.5.3/global_chem/animals/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/animals/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.914994 global_chem-1.8.5.3/global_chem/animals/snakes/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/animals/snakes/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    38357 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/animals/snakes/drugs_from_snake_venom.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      321 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/cli.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.917593 global_chem-1.8.5.3/global_chem/education/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/education/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.918870 global_chem-1.8.5.3/global_chem/education/cengage/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/education/cengage/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4602 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.923562 global_chem-1.8.5.3/global_chem/environment/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/environment/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9553 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/environment/alternative_jet_fuels.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2106 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/environment/chemicals_from_biomass.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9696 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/environment/emerging_perfluoroalkyls.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.926561 global_chem-1.8.5.3/global_chem/food/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.938283 global_chem-1.8.5.3/global_chem/food/color_additives/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/color_additives/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5620 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_five.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    26611 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_four.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6232 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_one.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    12448 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_seven.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5657 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_six.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5343 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_three.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5111 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_two.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.939081 global_chem-1.8.5.3/global_chem/food/fruits/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/food/fruits/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.945038 global_chem-1.8.5.3/global_chem/food/fruits/mango/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/food/fruits/mango/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1267 2023-11-27 15:26:11.000000 global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_amino_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1746 2023-11-27 15:26:11.000000 global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_fatty_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1338 2023-11-27 15:26:11.000000 global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_flavonoids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1014 2023-11-27 15:26:11.000000 global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_phenolic_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1151 2023-11-27 15:26:11.000000 global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_phytocompounds.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      962 2023-09-25 16:31:21.000000 global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_vitamins.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.946961 global_chem-1.8.5.3/global_chem/food/salt/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/salt/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2304 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/food/salt/salt.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.947740 global_chem-1.8.5.3/global_chem/food/spices/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-09-25 16:33:30.000000 global_chem-1.8.5.3/global_chem/food/spices/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.954943 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-09-25 16:35:00.000000 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1308 2023-09-25 16:55:40.000000 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/thai_ginger_cyclic_dipeptides.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1206 2023-09-25 16:55:40.000000 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/thai_ginger_diaryl_heptanoids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1490 2023-09-25 16:55:40.000000 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/thai_ginger_fatty_acids_and_esters.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      629 2023-09-25 16:55:40.000000 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/thai_ginger_flavonoids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1613 2023-09-25 16:55:40.000000 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/thai_ginger_phenolics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1099 2023-09-25 16:55:40.000000 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/thai_ginger_polysaccharides.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4130 2023-09-25 17:06:21.000000 global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/thai_ginger_terpenoids.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.955823 global_chem-1.8.5.3/global_chem/formulation/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/formulation/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.956479 global_chem-1.8.5.3/global_chem/formulation/excipients/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/formulation/excipients/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1783 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/formulation/excipients/allergen_inactive_ingredients.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.957834 global_chem-1.8.5.3/global_chem/formulation/excipients/biopharmaceutics_class_three/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/formulation/excipients/biopharmaceutics_class_three/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4134 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.960585 global_chem-1.8.5.3/global_chem/formulation/excipients/monoclonal_antibodies/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/formulation/excipients/monoclonal_antibodies/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4080 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    49412 2023-11-27 15:26:39.000000 global_chem-1.8.5.3/global_chem/global_chem.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.962543 global_chem-1.8.5.3/global_chem/interstellar_space/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/interstellar_space/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      678 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/interstellar_space/asteroid_ryugu.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    10891 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/interstellar_space/interstellar_space.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.963200 global_chem-1.8.5.3/global_chem/materials/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/materials/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.963710 global_chem-1.8.5.3/global_chem/materials/clay/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/materials/clay/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7263 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/materials/clay/montmorillonite_adsorption.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.964940 global_chem-1.8.5.3/global_chem/materials/polymers/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      116 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/materials/polymers/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    18019 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/materials/polymers/common_monomer_repeating_units.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.966215 global_chem-1.8.5.3/global_chem/medicinal_chemistry/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.003734 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5131 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1263 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      535 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_alcohols.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      757 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_aldehydes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1083 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_amino_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      914 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_esters_and_lactones.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      997 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_fatty_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1936 2023-10-12 15:22:02.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_flavanoidglycosides.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2941 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_hydrocarbons.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      959 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_ketones.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1123 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_nitrogenous_compounds.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      540 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_pigments.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    33609 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_proteins_glycoproteins_enzymes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1122 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_steroids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2032 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_sugars.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5409 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_terpenes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      418 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_vitamins.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)   206471 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1321 2023-06-27 14:15:06.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    32010 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.005963 global_chem-1.8.5.3/global_chem/medicinal_chemistry/chinese/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/chinese/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1103 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.009360 global_chem-1.8.5.3/global_chem/medicinal_chemistry/rings/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/rings/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    13832 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2694 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    14543 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/rings/rings_in_drugs.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.026353 global_chem-1.8.5.3/global_chem/medicinal_chemistry/scaffolds/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/scaffolds/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    48105 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    22232 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7459 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.030068 global_chem-1.8.5.3/global_chem/medicinal_chemistry/warheads/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/warheads/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3465 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3181 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.043841 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/access_group_antibiotics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/anaesthetics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/anaphylaxis_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/anticonvulsants.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/antidotes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/antifilarials.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/antischistosomals_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/cysticidal_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/intestinal_anthelminthics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/medical_gases.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/non_steroidal_anti_inflammatory_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/opioid_analgesics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/palliative_care.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/preoperative_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/reserve_group_antibiotics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/medicinal_chemistry/world_health_organization/watch_group_antibiotics.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.047325 global_chem-1.8.5.3/global_chem/miscellaneous/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/miscellaneous/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2139 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/miscellaneous/amino_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9650 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/miscellaneous/open_smiles.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      396 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/miscellaneous/regex_patterns.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3724 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/miscellaneous/vitamins.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.061233 global_chem-1.8.5.3/global_chem/narcotics/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/narcotics/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    41346 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/narcotics/pihkal.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2155 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/narcotics/schedule_five.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    17624 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/narcotics/schedule_four.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    57945 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/narcotics/schedule_one.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4816 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/narcotics/schedule_three.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    14153 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/narcotics/schedule_two.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.065583 global_chem-1.8.5.3/global_chem/organic_synthesis/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/organic_synthesis/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.098417 global_chem-1.8.5.3/global_chem/organic_synthesis/bidendate_phosphine_ligands/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/organic_synthesis/bidendate_phosphine_ligands/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7973 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.116553 global_chem-1.8.5.3/global_chem/organic_synthesis/protecting_groups/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/organic_synthesis/protecting_groups/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    42927 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.176127 global_chem-1.8.5.3/global_chem/organic_synthesis/solvents/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/organic_synthesis/solvents/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5293 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/organic_synthesis/solvents/common_organic_solvents.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.178198 global_chem-1.8.5.3/global_chem/peptides/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/peptides/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3489 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/peptides/lanthipeptides.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.179462 global_chem-1.8.5.3/global_chem/proteins/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/proteins/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.179875 global_chem-1.8.5.3/global_chem/proteins/kinases/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/proteins/kinases/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.180598 global_chem-1.8.5.3/global_chem/proteins/kinases/braf/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/proteins/kinases/braf/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7617 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/proteins/kinases/braf/braf_inhibitors.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.183869 global_chem-1.8.5.3/global_chem/proteins/kinases/scaffolds/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/proteins/kinases/scaffolds/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5167 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.184896 global_chem-1.8.5.3/global_chem/sex/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/sex/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.186224 global_chem-1.8.5.3/global_chem/sex/contraceptives/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/sex/contraceptives/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/sex/contraceptives/oral_contraceptives.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.193624 global_chem-1.8.5.3/global_chem/sex/exsens/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/sex/exsens/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    16558 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/sex/exsens/exsens_products.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9160 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/sex/exsens/lube.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.196333 global_chem-1.8.5.3/global_chem/sex/tainted_sexual_enhancements/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/sex/tainted_sexual_enhancements/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1269 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.204182 global_chem-1.8.5.3/global_chem/skin/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/skin/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.286397 global_chem-1.8.5.3/global_chem/skin/sunscreen/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/skin/sunscreen/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/skin/sunscreen/sunscreen.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.287229 global_chem-1.8.5.3/global_chem/skin/transdermal_and_dermal_delivery/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/skin/transdermal_and_dermal_delivery/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9628 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:48.290258 global_chem-1.8.5.3/global_chem/warfare/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/warfare/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2511 2023-04-11 15:37:28.000000 global_chem-1.8.5.3/global_chem/warfare/organophosphorous_nerve_agents.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-02-22 17:40:47.912471 global_chem-1.8.5.3/global_chem.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)    54028 2024-02-22 17:40:47.000000 global_chem-1.8.5.3/global_chem.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)     8709 2024-02-22 17:40:47.000000 global_chem-1.8.5.3/global_chem.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-02-22 17:40:47.000000 global_chem-1.8.5.3/global_chem.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-02-22 17:40:00.000000 global_chem-1.8.5.3/global_chem.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)      592 2024-02-22 17:40:47.000000 global_chem-1.8.5.3/global_chem.egg-info/requires.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       12 2024-02-22 17:40:47.000000 global_chem-1.8.5.3/global_chem.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-02-22 17:40:48.294091 global_chem-1.8.5.3/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2521 2024-02-22 17:39:51.000000 global_chem-1.8.5.3/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.942093 global_chem-1.9.1/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    54389 2024-05-09 19:24:48.941712 global_chem-1.9.1/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    50166 2024-05-09 19:23:56.000000 global_chem-1.9.1/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.845515 global_chem-1.9.1/global_chem/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7089 2024-05-09 19:23:56.000000 global_chem-1.9.1/global_chem/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      238 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/__main__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.850365 global_chem-1.9.1/global_chem/animals/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/animals/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.850956 global_chem-1.9.1/global_chem/animals/snakes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/animals/snakes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    38357 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/animals/snakes/drugs_from_snake_venom.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      321 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/cli.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.853105 global_chem-1.9.1/global_chem/education/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/education/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.853617 global_chem-1.9.1/global_chem/education/cengage/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/education/cengage/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4602 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.856552 global_chem-1.9.1/global_chem/environment/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/environment/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9553 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/environment/alternative_jet_fuels.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2106 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/environment/chemicals_from_biomass.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9696 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/environment/emerging_perfluoroalkyls.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.857498 global_chem-1.9.1/global_chem/food/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.862571 global_chem-1.9.1/global_chem/food/color_additives/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5620 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_five.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    26611 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_four.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6232 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_one.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    12448 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_seven.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5657 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_six.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5343 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_three.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5111 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/color_additives/fda_list_two.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.863085 global_chem-1.9.1/global_chem/food/fruits/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/food/fruits/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.867639 global_chem-1.9.1/global_chem/food/fruits/mango/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/food/fruits/mango/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1287 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1778 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_fatty_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1367 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_flavonoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      886 2024-05-09 19:23:56.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_phenolic_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5489 2024-05-09 19:18:27.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_phyto_compounds.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1084 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/food/fruits/mango/mango_vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.868604 global_chem-1.9.1/global_chem/food/salt/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/salt/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2304 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/food/salt/salt.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.869217 global_chem-1.9.1/global_chem/formulation/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.870092 global_chem-1.9.1/global_chem/formulation/excipients/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1783 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/allergen_inactive_ingredients.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.871215 global_chem-1.9.1/global_chem/formulation/excipients/biopharmaceutics_class_three/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/biopharmaceutics_class_three/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4134 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.872522 global_chem-1.9.1/global_chem/formulation/excipients/monoclonal_antibodies/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/monoclonal_antibodies/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4080 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    47486 2024-05-09 19:23:56.000000 global_chem-1.9.1/global_chem/global_chem.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.873941 global_chem-1.9.1/global_chem/interstellar_space/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/interstellar_space/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      678 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/interstellar_space/asteroid_ryugu.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    10891 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/interstellar_space/interstellar_space.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.874647 global_chem-1.9.1/global_chem/materials/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.875477 global_chem-1.9.1/global_chem/materials/clay/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/clay/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7263 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/clay/montmorillonite_adsorption.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.876663 global_chem-1.9.1/global_chem/materials/polymers/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      116 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/polymers/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    18019 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/materials/polymers/common_monomer_repeating_units.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.877650 global_chem-1.9.1/global_chem/medicinal_chemistry/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.894596 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1263 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      535 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/alcohols.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      757 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/aldehydes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1083 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5131 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)   206471 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      914 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      997 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1937 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2941 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      959 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/ketones.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1123 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1321 2023-06-27 14:15:06.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    32010 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      540 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/pigments.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    33609 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1122 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/steroids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2032 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/sugars.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5409 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/terpenes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      418 2024-05-09 19:17:05.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.896041 global_chem-1.9.1/global_chem/medicinal_chemistry/chinese/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/chinese/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1103 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.898198 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    13832 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2694 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    14543 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/rings/rings_in_drugs.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.901764 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    48105 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    22232 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7459 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.902997 global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3465 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3181 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.910082 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/access_group_antibiotics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/anaesthetics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/anaphylaxis_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/anticonvulsants.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/antidotes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/antifilarials.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/antischistosomals_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/cysticidal_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/intestinal_anthelminthics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/medical_gases.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/non_steroidal_anti_inflammatory_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/opioid_analgesics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/palliative_care.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/preoperative_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/reserve_group_antibiotics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/medicinal_chemistry/world_health_organization/watch_group_antibiotics.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.913668 global_chem-1.9.1/global_chem/miscellaneous/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2139 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9650 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/open_smiles.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      396 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/regex_patterns.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3724 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/miscellaneous/vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.921409 global_chem-1.9.1/global_chem/narcotics/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      370 2024-05-09 19:17:09.000000 global_chem-1.9.1/global_chem/narcotics/black_market.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    41346 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/pihkal.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2155 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_five.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    17624 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_four.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    57945 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_one.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4816 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_three.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    14153 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/narcotics/schedule_two.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.922047 global_chem-1.9.1/global_chem/organic_synthesis/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.922556 global_chem-1.9.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7973 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.923545 global_chem-1.9.1/global_chem/organic_synthesis/protecting_groups/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/protecting_groups/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    42927 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.924821 global_chem-1.9.1/global_chem/organic_synthesis/solvents/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/solvents/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5293 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/organic_synthesis/solvents/common_organic_solvents.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.925757 global_chem-1.9.1/global_chem/peptides/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/peptides/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3489 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/peptides/lanthipeptides.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.926504 global_chem-1.9.1/global_chem/proteins/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.927057 global_chem-1.9.1/global_chem/proteins/kinases/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.928058 global_chem-1.9.1/global_chem/proteins/kinases/braf/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/braf/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7617 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/braf/braf_inhibitors.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.929138 global_chem-1.9.1/global_chem/proteins/kinases/scaffolds/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/scaffolds/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5167 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.929749 global_chem-1.9.1/global_chem/sex/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.930247 global_chem-1.9.1/global_chem/sex/contraceptives/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/contraceptives/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/contraceptives/oral_contraceptives.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.932170 global_chem-1.9.1/global_chem/sex/exsens/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/exsens/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    16558 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/exsens/exsens_products.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9160 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/exsens/lube.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.934273 global_chem-1.9.1/global_chem/sex/tainted_sexual_enhancements/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/tainted_sexual_enhancements/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1269 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.937329 global_chem-1.9.1/global_chem/skin/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.938150 global_chem-1.9.1/global_chem/skin/sunscreen/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/sunscreen/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/sunscreen/sunscreen.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.939093 global_chem-1.9.1/global_chem/skin/transdermal_and_dermal_delivery/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/transdermal_and_dermal_delivery/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9628 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.940446 global_chem-1.9.1/global_chem/warfare/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/warfare/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2511 2023-04-11 15:37:28.000000 global_chem-1.9.1/global_chem/warfare/organophosphorous_nerve_agents.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-09 19:24:48.850012 global_chem-1.9.1/global_chem.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    54389 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     8056 2024-05-09 19:24:47.000000 global_chem-1.9.1/global_chem.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      592 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/requires.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       12 2024-05-09 19:24:46.000000 global_chem-1.9.1/global_chem.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-09 19:24:48.942274 global_chem-1.9.1/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2371 2024-05-09 19:24:36.000000 global_chem-1.9.1/setup.py
```

### Comparing `global_chem-1.8.5.3/PKG-INFO` & `global_chem-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global_chem
-Version: 1.8.5.3
+Version: 1.9.1
 Summary: UNKNOWN
 Home-page: https://www.github.com/Sulstice/global-chem
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: MPL 2.0
 Description: <h1 align="center">Organizing The Chemical Universe</h1>
         
@@ -169,14 +169,15 @@
         'chemicals_from_biomass': ChemicalsFromBioMass,                           # Anthony Maiorana & Suliman Sharif
         'salt': Salt,                                                             # Suliman Sharif
         'drugs_from_snake_venom': DrugsFromSnakeVenom,                            # Suliman Sharif
         'oral_contraceptives': OralContraceptives,                                # Suliman Sharif
         'surfactants': Surfactants,                                               # Yiling Nan & Suliman Sharif
         'lanthipeptides: LanthiPeptides                                           # Prabin Baral & Suliman Sharif
         'alternative_jet_fuels': AlternativeJetFuels                              # Suliman Sharif
+        'mango_amino_acids': MangoPhytocompounds,                                 # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_amino_acids': MangoAminoAcids,                                     # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_phenolic_acids': MangoPhenolicAcids,                               # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_fatty_acids': MangoFattyAcids,                                     # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_vitamins': MangoVitamins,                                          # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_flavonoids': MangoFlavonoids                                       # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'thai_ginger_cyclic_dipeptides': ThaiGingerCyclicDipeptides,              # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
         'thai_ginger_diaryl_heptanoids': ThaiGingerDiarylHeptanoids,              # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
@@ -233,14 +234,15 @@
         | Cengage Bronsted Acids              | 42           | https://cxp.cengage.com/contentservice/assets/owms01h/references/chemtables/org_chem/pKaTable.html                                                                                                                                                                                                                  |
         | Chemicals From Biomass              | 17           | Wittcoff, Harold A., et al. Industrial Organic Chemicals: Wittcoff/Organic Chemicals. John Wiley & Sons, Inc., 2004                                                                                                                                                                                                 |
         | Drugs From Snake Venom              | 7            | Oliveira, Ana L., et al. “The Chemistry of Snake Venom and Its Medicinal Potential.” Nature Reviews Chemistry, vol. 6, no. 7, July 2022, pp. 451–69                                                                                                                                                                 |
         | Oral Contraceptives                 | 17           | Coleman, William F. “The Molecules of Oral Contraceptives.” Journal of Chemical Education, vol. 87, no. 7, July 2010, pp. 760–61.                                                                                                                                                                                   |
         | Surfactants for Skin                | 36           | Date, Abhijit A., and Vandana B. Patravale. “Microemulsions: Applications in Transdermal and Dermal Delivery.” Critical Reviews&trade; in Therapeutic Drug Carrier Systems, vol. 24, no. 6, 2007.                                                                                                                   |
         | LanthiPeptides                      | 2            | Pokhrel, Rudramani, et al. “Molecular Mechanisms of Pore Formation and Membrane Disruption by the Antimicrobial Lantibiotic Peptide Mutacin 1140.” Physical Chemistry Chemical Physics, vol. 21, no. 23, June 2019, pp. 12530–39.                                                                                   |
         | Alternative Jet Fuels               | 59           | Chemical Composition and Fuel Properties of Alternative Jet Fuels :: BioResources. https://bioresources.cnr.ncsu.edu/.                                                                                                                                                                                              |
+        | Mango Phytocompounds                | 87            | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Amino Acids                   | 19           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Phenoloic Acids               | 10           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Fatty Acids                   | 24           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Vitamins                      | 10           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Flavonoids                    | 11           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Thai Ginger Cyclic Dipeptides       | 6            | Wang, Si-Yu, et al. “Kaempferia Galanga L.: Progresses in Phytochemistry, Pharmacology, Toxicology and Ethnomedicinal Uses.” Frontiers in Pharmacology, vol. 12, 2021.                                                                                                                                              |
         | Thai Ginger Diaryl Heptanoids       | 6            | Wang, Si-Yu, et al. “Kaempferia Galanga L.: Progresses in Phytochemistry, Pharmacology, Toxicology and Ethnomedicinal Uses.” Frontiers in Pharmacology, vol. 12, 2021.                                                                                                                                              |
@@ -411,17 +413,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: graphing
 Provides-Extra: forcefields
 Provides-Extra: bioinformatics
 Provides-Extra: cheminformatics
 Provides-Extra: quantum_chemistry
 Provides-Extra: development_operations
```

### Comparing `global_chem-1.8.5.3/README.md` & `global_chem-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 'chemicals_from_biomass': ChemicalsFromBioMass,                           # Anthony Maiorana & Suliman Sharif
 'salt': Salt,                                                             # Suliman Sharif
 'drugs_from_snake_venom': DrugsFromSnakeVenom,                            # Suliman Sharif
 'oral_contraceptives': OralContraceptives,                                # Suliman Sharif
 'surfactants': Surfactants,                                               # Yiling Nan & Suliman Sharif
 'lanthipeptides: LanthiPeptides                                           # Prabin Baral & Suliman Sharif
 'alternative_jet_fuels': AlternativeJetFuels                              # Suliman Sharif
+'mango_amino_acids': MangoPhytocompounds,                                 # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
 'mango_amino_acids': MangoAminoAcids,                                     # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
 'mango_phenolic_acids': MangoPhenolicAcids,                               # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
 'mango_fatty_acids': MangoFattyAcids,                                     # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
 'mango_vitamins': MangoVitamins,                                          # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
 'mango_flavonoids': MangoFlavonoids                                       # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
 'thai_ginger_cyclic_dipeptides': ThaiGingerCyclicDipeptides,              # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
 'thai_ginger_diaryl_heptanoids': ThaiGingerDiarylHeptanoids,              # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
@@ -225,14 +226,15 @@
 | Cengage Bronsted Acids              | 42           | https://cxp.cengage.com/contentservice/assets/owms01h/references/chemtables/org_chem/pKaTable.html                                                                                                                                                                                                                  |
 | Chemicals From Biomass              | 17           | Wittcoff, Harold A., et al. Industrial Organic Chemicals: Wittcoff/Organic Chemicals. John Wiley & Sons, Inc., 2004                                                                                                                                                                                                 |
 | Drugs From Snake Venom              | 7            | Oliveira, Ana L., et al. “The Chemistry of Snake Venom and Its Medicinal Potential.” Nature Reviews Chemistry, vol. 6, no. 7, July 2022, pp. 451–69                                                                                                                                                                 |
 | Oral Contraceptives                 | 17           | Coleman, William F. “The Molecules of Oral Contraceptives.” Journal of Chemical Education, vol. 87, no. 7, July 2010, pp. 760–61.                                                                                                                                                                                   |
 | Surfactants for Skin                | 36           | Date, Abhijit A., and Vandana B. Patravale. “Microemulsions: Applications in Transdermal and Dermal Delivery.” Critical Reviews&trade; in Therapeutic Drug Carrier Systems, vol. 24, no. 6, 2007.                                                                                                                   |
 | LanthiPeptides                      | 2            | Pokhrel, Rudramani, et al. “Molecular Mechanisms of Pore Formation and Membrane Disruption by the Antimicrobial Lantibiotic Peptide Mutacin 1140.” Physical Chemistry Chemical Physics, vol. 21, no. 23, June 2019, pp. 12530–39.                                                                                   |
 | Alternative Jet Fuels               | 59           | Chemical Composition and Fuel Properties of Alternative Jet Fuels :: BioResources. https://bioresources.cnr.ncsu.edu/.                                                                                                                                                                                              |
+| Mango Phytocompounds                | 87            | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
 | Mango Amino Acids                   | 19           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
 | Mango Phenoloic Acids               | 10           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
 | Mango Fatty Acids                   | 24           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
 | Mango Vitamins                      | 10           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
 | Mango Flavonoids                    | 11           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
 | Thai Ginger Cyclic Dipeptides       | 6            | Wang, Si-Yu, et al. “Kaempferia Galanga L.: Progresses in Phytochemistry, Pharmacology, Toxicology and Ethnomedicinal Uses.” Frontiers in Pharmacology, vol. 12, 2021.                                                                                                                                              |
 | Thai Ginger Diaryl Heptanoids       | 6            | Wang, Si-Yu, et al. “Kaempferia Galanga L.: Progresses in Phytochemistry, Pharmacology, Toxicology and Ethnomedicinal Uses.” Frontiers in Pharmacology, vol. 12, 2021.                                                                                                                                              |
```

### Comparing `global_chem-1.8.5.3/global_chem/__init__.py` & `global_chem-1.9.1/global_chem/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,32 +27,32 @@
 
 from global_chem.warfare.organophosphorous_nerve_agents import OrganoPhosphorousNerveAgents
 
 # Medicinal Chemistry - Cannabinoids
 
 from global_chem.medicinal_chemistry.cannabinoids.phytocannabinoids import PhytoCannabinoids
 from global_chem.medicinal_chemistry.cannabinoids.constituents_of_cannabis_sativa import ConstituentsOfCannabisSativa
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_acids import CannabisAcids
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_alcohols import CannabisAlcohols
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_aldehydes import CannabisAldehydes
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_amino_acids import CannabisAminoAcids
+from global_chem.medicinal_chemistry.cannabinoids.acids import CannabisAcids
+from global_chem.medicinal_chemistry.cannabinoids.alcohols import CannabisAlcohols
+from global_chem.medicinal_chemistry.cannabinoids.aldehydes import CannabisAldehydes
+from global_chem.medicinal_chemistry.cannabinoids.amino_acids import CannabisAminoAcids
 from global_chem.medicinal_chemistry.cannabinoids.cannabinoids import Cannabinoids
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_esters_and_lactones import CannabisEstersAndLactones
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_fatty_acids import CannabisFattyAcids
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_flavanoidglycosides import CannabisFlavanoidGlycosides
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_hydrocarbons import CannabisHydrocarbons
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_ketones import CannabisKetones
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_nitrogenous_compounds import CannabisNitrogenousCompounds
+from global_chem.medicinal_chemistry.cannabinoids.esters_and_lactones import CannabisEstersAndLactones
+from global_chem.medicinal_chemistry.cannabinoids.fatty_acids import CannabisFattyAcids
+from global_chem.medicinal_chemistry.cannabinoids.flavanoidglycosides import CannabisFlavanoidGlycosides
+from global_chem.medicinal_chemistry.cannabinoids.hydrocarbons import CannabisHydrocarbons
+from global_chem.medicinal_chemistry.cannabinoids.ketones import CannabisKetones
+from global_chem.medicinal_chemistry.cannabinoids.nitrogenous_compounds import CannabisNitrogenousCompounds
 from global_chem.medicinal_chemistry.cannabinoids.non_cannabinoids_phenols import NonCannabinoidPhenols
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_pigments import CannabisPigments
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_proteins_glycoproteins_enzymes import CannabisProteinsGlycoproteinsEnzymes
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_steroids import CannabisSteroids
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_sugars import CannabisSugars
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_terpenes import CannabisTerpenes
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_vitamins import CannabisVitamins
+from global_chem.medicinal_chemistry.cannabinoids.pigments import CannabisPigments
+from global_chem.medicinal_chemistry.cannabinoids.proteins_glycoproteins_enzymes import CannabisProteinsGlycoproteinsEnzymes
+from global_chem.medicinal_chemistry.cannabinoids.steroids import CannabisSteroids
+from global_chem.medicinal_chemistry.cannabinoids.sugars import CannabisSugars
+from global_chem.medicinal_chemistry.cannabinoids.terpenes import CannabisTerpenes
+from global_chem.medicinal_chemistry.cannabinoids.vitamins import CannabisVitamins
 
 # Medicinal Chemistry - International
 
 from global_chem.medicinal_chemistry.chinese.how_to_live_longer import HowToLiveLonger
 
 # Medicinal Chemistry - Warheads
 
@@ -89,35 +89,28 @@
 from global_chem.food.color_additives.fda_list_two import FDAListTwo
 from global_chem.food.color_additives.fda_list_three import FDAListThree
 from global_chem.food.color_additives.fda_list_four import FDAListFour
 from global_chem.food.color_additives.fda_list_five import FDAListFive
 from global_chem.food.color_additives.fda_list_six import FDAListSix
 from global_chem.food.color_additives.fda_list_seven import FDAListSeven
 
-# Thai Ginger
-
-from global_chem.food.spices.thai_ginger.thai_ginger_cyclic_dipeptides import ThaiGingerCyclicDipeptides
-from global_chem.food.spices.thai_ginger.thai_ginger_diaryl_heptanoids import ThaiGingerDiarylHeptanoids
-from global_chem.food.spices.thai_ginger.thai_ginger_fatty_acids_and_esters import ThaiGingerFattyAcidsAndEsters
-from global_chem.food.spices.thai_ginger.thai_ginger_flavonoids import ThaiGingerFlavonoids
-from global_chem.food.spices.thai_ginger.thai_ginger_phenolics import ThaiGingerPhenolics
-from global_chem.food.spices.thai_ginger.thai_ginger_polysaccharides import ThaiGingerPolysaccharides
-from global_chem.food.spices.thai_ginger.thai_ginger_terpenoids import ThaiGingerTerpenoids
 
 # Mango
 
-from global_chem.food.fruits.mango.mango_phytocompounds import MangoPhytocompounds
-from global_chem.food.fruits.mango.mango_fatty_acids import MangoFattyAcids
-from global_chem.food.fruits.mango.mango_flavonoids import MangoFlavonoids
+from global_chem.food.fruits.mango.mango_phyto_compounds import MangoPhytocompounds
 from global_chem.food.fruits.mango.mango_phenolic_acids import MangoPhenolicAcids
 from global_chem.food.fruits.mango.mango_vitamins import MangoVitamins
+from global_chem.food.fruits.mango.mango_fatty_acids import MangoFattyAcids
 from global_chem.food.fruits.mango.mango_amino_acids import MangoAminoAcids
+from global_chem.food.fruits.mango.mango_flavonoids import MangoFlavonoids
 
 # Narcotics
 
+from global_chem.narcotics.pihkal import Pihkal
+from global_chem.narcotics.black_market import BlackMarket
 from global_chem.narcotics.schedule_one import ScheduleOne
 from global_chem.narcotics.schedule_two import ScheduleTwo
 from global_chem.narcotics.schedule_three import ScheduleThree
 from global_chem.narcotics.schedule_four import ScheduleFour
 from global_chem.narcotics.schedule_five import ScheduleFive
 
 # Interstellar Space
```

### Comparing `global_chem-1.8.5.3/global_chem/animals/snakes/drugs_from_snake_venom.py` & `global_chem-1.9.1/global_chem/animals/snakes/drugs_from_snake_venom.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py` & `global_chem-1.9.1/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/environment/alternative_jet_fuels.py` & `global_chem-1.9.1/global_chem/environment/alternative_jet_fuels.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/environment/chemicals_from_biomass.py` & `global_chem-1.9.1/global_chem/environment/chemicals_from_biomass.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/environment/emerging_perfluoroalkyls.py` & `global_chem-1.9.1/global_chem/environment/emerging_perfluoroalkyls.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_five.py` & `global_chem-1.9.1/global_chem/food/color_additives/fda_list_five.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_four.py` & `global_chem-1.9.1/global_chem/food/color_additives/fda_list_four.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_one.py` & `global_chem-1.9.1/global_chem/food/color_additives/fda_list_one.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_seven.py` & `global_chem-1.9.1/global_chem/food/color_additives/fda_list_seven.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_six.py` & `global_chem-1.9.1/global_chem/food/color_additives/fda_list_six.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_three.py` & `global_chem-1.9.1/global_chem/food/color_additives/fda_list_three.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/color_additives/fda_list_two.py` & `global_chem-1.9.1/global_chem/food/color_additives/fda_list_two.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_amino_acids.py` & `global_chem-1.9.1/global_chem/food/fruits/mango/mango_amino_acids.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-#!/usr/bin/env python3
-#
-# GlobalChem - Mango Amino Acids
-# -------------------------------
-
 class MangoAminoAcids(object):
 
     def __init__(self):
 
         self.name = 'mango_amino_acids'
 
     @staticmethod
@@ -31,7 +26,17 @@
             'aspartic acid': 'C([C@@H](C(=O)O)N)C(=O)O',
             'alanine': 'C[C@@H](C(=O)O)N',
             'arginine': 'C(C[C@@H](C(=O)O)N)CN=C(N)N',
             'histidine': 'C1=C(NC=N1)C[C@@H](C(=O)O)N'
         }
 
         return smiles
+
+
+    @staticmethod
+    def get_smarts():
+
+      smarts = {
+              
+          }
+      
+      return smarts
```

### Comparing `global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_fatty_acids.py` & `global_chem-1.9.1/global_chem/food/fruits/mango/mango_fatty_acids.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-#!/usr/bin/env python3
-#
-# GlobalChem - Mango Fatty Acids
-# -------------------------------
-
 class MangoFattyAcids(object):
 
     def __init__(self):
 
         self.name = 'mango_fatty_acids'
 
     @staticmethod
@@ -36,7 +31,17 @@
             'linoleic acid': 'CCCCC/C=C\C/C=C\CCCCCCCC(=O)O',
             '9,15-Octadecadienoic acid': 'CC/C=C/CCCC/C=C/CCCCCCCC(=O)O',
             'hepta-2,4(E,E)-dienoic acid': '',
             'linolenic acid': 'CC/C=C\C/C=C\C/C=C\CCCCCCCC(=O)O'
         }
 
         return smiles
+    
+    
+    @staticmethod
+    def get_smarts():
+
+      smarts = {
+              
+          }
+      
+      return smarts
```

### Comparing `global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_flavonoids.py` & `global_chem-1.9.1/global_chem/food/fruits/mango/mango_flavonoids.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-#!/usr/bin/env python3
-#
-# GlobalChem - Mango Flavonoids
-# -----------------------------
-
 class MangoFlavonoids(object):
 
     def __init__(self):
 
         self.name = 'mango_flavonoids'
 
     @staticmethod
@@ -23,7 +18,16 @@
             'catechin': 'C1[C@@H]([C@H](OC2=CC(=CC(=C21)O)O)C3=CC(=C(C=C3)O)O)O',
             'apigenin': 'C1=CC(=CC=C1C2=CC(=O)C3=C(C=C(C=C3O2)O)O)O ',
             'luteolin': 'C1=CC(=C(C=C1C2=CC(=O)C3=C(C=C(C=C3O2)O)O)O)O',
             'kaempferol': 'C1=CC(=CC=C1C2=C(C(=O)C3=C(C=C(C=C3O2)O)O)O)O',
         }
 
         return smiles
+    
+    @staticmethod
+    def get_smarts():
+
+      smarts = {
+              
+          }
+      
+      return smarts
```

### Comparing `global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_phenolic_acids.py` & `global_chem-1.9.1/global_chem/food/fruits/mango/mango_phenolic_acids.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-#!/usr/bin/env python3
-#
-# GlobalChem - Mango Phenolic Acids
-# ----------------------------------
-
-class MangoPhenolicAcids(object):
-
-    def __init__(self):
-
-        self.name = 'mango_phenolic_acids'
-
-    @staticmethod
-    def get_smiles():
-
-        smiles = {
-            'gallic Acid': 'C1=C(C=C(C(=C1O)O)O)C(=O)O',
-            'vanillic acid ': 'COC1=C(C=CC(=C1)C(=O)O)O',
-            'syringic acid ': 'COC1=CC(=CC(=C1O)OC)C(=O)O',
-            'protocatechuic acid': 'C1=CC(=C(C=C1C(=O)O)O)O',
-            'para hydroxybenzoic acid ': 'C1=CC(=CC=C1C(=O)O)O',
-            'paracoumaric acid': 'C1=CC(=CC=C1/C=C/C(=O)O)O',
-            'chlorogenic acid ': 'C1[C@H]([C@H]([C@@H](C[C@@]1(C(=O)O)O)OC(=O)/C=C/C2=CC(=C(C=C2)O)O)O)O',
-            'ferulic acid': 'COC1=C(C=CC(=C1)/C=C/C(=O)O)O',
-            'caffeic acid': 'C1=CC(=C(C=C1/C=C/C(=O)O)O)O',
-            'theogallin': 'C1[C@H]([C@H]([C@@H](C[C@@]1(C(=O)O)O)OC(=O)C2=CC(=C(C(=C2)O)O)O)O)O',
-        }
-
-        return smiles
+class MangoPhenolicAcids(object):
+
+  def __init__(self):
+
+    self.name = 'mango_phenolic_acids'
+
+  @staticmethod
+  def get_smiles():
+
+    smiles = {
+      'gallic Acid': 'C1=C(C=C(C(=C1O)O)O)C(=O)O',
+      'vanillic acid ': 'COC1=C(C=CC(=C1)C(=O)O)O',
+      'syringic acid ': 'COC1=CC(=CC(=C1O)OC)C(=O)O',
+      'protocatechuic acid': 'C1=CC(=C(C=C1C(=O)O)O)O',
+      'para hydroxybenzoic acid ': 'C1=CC(=CC=C1C(=O)O)O',
+      'paracoumaric acid': 'C1=CC(=CC=C1/C=C/C(=O)O)O',
+      'chlorogenic acid ': 'C1[C@H]([C@H]([C@@H](C[C@@]1(C(=O)O)O)OC(=O)/C=C/C2=CC(=C(C=C2)O)O)O)O',
+      'ferulic acid': 'COC1=C(C=CC(=C1)/C=C/C(=O)O)O',
+      'caffeic acid': 'C1=CC(=C(C=C1/C=C/C(=O)O)O)O',
+      'theogallin': 'C1[C@H]([C@H]([C@@H](C[C@@]1(C(=O)O)O)OC(=O)C2=CC(=C(C(=C2)O)O)O)O)O',
+    }
+
+    return smiles
+
+
+
+  @staticmethod
+  def get_smarts():
+
+    smarts = {
+
+    }
+
+    return smarts
```

### Comparing `global_chem-1.8.5.3/global_chem/food/fruits/mango/mango_vitamins.py` & `global_chem-1.9.1/global_chem/food/fruits/mango/mango_vitamins.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,7 +17,17 @@
             'folic acid ': 'C1=CC(=CC=C1C(=O)N[C@@H](CCC(=O)O)C(=O)O)NCC2=CN=C3C(=N2)C(=O)NC(=N3)N',
             'vitamin A': 'CC1=C(C(CCC1)(C)C)/C=C/C(=C/C=C/C(=C/CO)/C)/C',
             'vitamin E': 'CC1=C(C2=C(CC[C@@](O2)(C)CCC[C@H](C)CCC[C@H](C)CCCC(C)C)C(=C1O)C)C',
             'vitamin K': 'CC1=C(C(=O)C2=CC=CC=C2C1=O)C/C=C(\C)/CCCC(C)CCCC(C)CCCC(C)C',
         }
 
         return smiles
+
+
+    @staticmethod
+    def get_smarts():
+
+      smarts = {
+              
+          }
+      
+      return smarts
```

### Comparing `global_chem-1.8.5.3/global_chem/food/salt/salt.py` & `global_chem-1.9.1/global_chem/food/salt/salt.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/food/spices/thai_ginger/thai_ginger_cyclic_dipeptides.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 #!/usr/bin/env python3
 #
-# GlobalChem - Ginger Cyclic Dipeptides
+# GlobalChem - Non-Cannabinoid Phenols
+#
 # -------------------------------------
 
-class ThaiGingerCyclicDipeptides(object):
+class NonCannabinoidPhenols(object):
 
   def __init__(self):
 
-    self.name = 'thai_ginger_cyclic_dipeptides'
+    self.name = 'non_cannabinoid_phenols'
 
   @staticmethod
   def get_smiles():
 
-      '''
-  
-      Missing:
-          'cyclo-(L-Val-L-Val)': '',
-          'cyclo-(L-Ala-L-lle)': '',
-          'cyclo-(L-Ala-L-Phe)': '',
-          'cyclo-(L-Val-L-Ala)': '',
-          'cyclo-(L-Leu-L-Tyr)': '',
-          'cyclo-(L-Val-L-Tyr)': '',
-          'cyclo-(L-Asp-OCH3-L-Phe)': '',
-          'cyclo-(L-Tyr-L-lle)' : '',
-          'cyclo-(L-Glu-OCH3-L-Phe)' : '',
-          'cyclo-(L-Leu-L-lle)' : 'C1CCC(C1)[PbH]'
-      '''
-  
-      smiles = {
-        'cyclo-(L-Val-L-Phe}' : 'CC(C)[C@H]1C(=O)N[C@H](C(=O)N1)CC2=CC=CC=C2',
-        'cyclo-(L-Val-L-Leu)' : 'CC(C)C[C@H]1C(=O)N[C@@H](C(=O)N1)C(C)C',
-        'cyclo-(L-Ala-L-Leu)' : 'C[C@H]1C(=O)N[C@H](C(=O)N1)CC(C)C',
-        'cyclo-(L-Phe-L-Tyr)' : 'C1=CC=C(C=C1)C[C@H]2C(=O)N[C@H](C(=O)N2)CC3=CC=C(C=C3)O',
-        'cyclo-(L-Pro-L-Tyr)' : 'C1C[C@H]2C(=O)N[C@H](C(=O)N2C1)CC3=CC=C(C=C3)O',
-        'cyclo-(L-Leu-L-Phe)' : 'CC(C)C[C@H]1C(=O)N[C@H](C(=O)N1)CC2=CC=CC=C2 ',
-      }
-  
-      return smiles
+    smiles = {
+      'acetylcannabispirol': 'COc1cc2CCC3(CCC(CC3)OC(=O)C)c2c(O)c1',
+      'cannabispiradienone': 'COC1=CC2=C(C(=C1)O)C3(CC2)C=CC(=O)C=C3',
+      'beta cannabispiranol': 'COC1=CC2=C(C(=C1)O)C3(CCC(CC3)O)CC2',
+      'cannabispirenone': 'COC1=CC2=C(C(=C1)O)C3(CCC(=O)C=C3)CC2',
+      'cannabispirenone-isomer': 'COC1=CC2=C(C(=C1)O)C3(CCC(=O)C=C3)CC2',
+      'cannabispirone': 'COC1=CC2=C(C(=C1)O)C3(CCC(=O)CC3)CC2',
+      '3-[2-(4-hydroxyphenyl)ethyl]-5-methoxyphenol': 'COc1cc(O)cc(CCc2ccc(O)cc2)c1',
+      '3-[2-(3-hydroxy-4-methoxyphenyl)ethyl]-5-methoxyphenol': 'COc1cc(O)cc(CCc2ccc(OC)c(O)c2)c1',
+      '3-[2-(3-isoprenyl-4-hydroxy-5-methoxy-phenyl)ethyl]-5-methoxyphenol': 'COc1cc(O)cc(CCc2cc(OC)c(O)c(C=CC(C)=C)c2)c1',
+      'canniprene': 'CC(=CCC1=C(C=CC(=C1O)OC)CCC2=CC(=CC(=C2)OC)O)C',
+      'eugenol': 'COc1cc(CC=C)ccc1O',
+      'isoeugenol': 'COc1cc(C=CC)ccc1O',
+      'anethol': 'COc1ccc(C=CC)cc1',
+      'methyleugenol': 'COc1ccc(CC=C)cc1OC',
+    }
+
+    return smiles
 
   @staticmethod
   def get_smarts():
 
-      smarts = {
-  
-      }
-  
-      return smarts
+    smarts = {
+    }
+
+    return smarts
```

### Comparing `global_chem-1.8.5.3/global_chem/formulation/excipients/allergen_inactive_ingredients.py` & `global_chem-1.9.1/global_chem/formulation/excipients/allergen_inactive_ingredients.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py` & `global_chem-1.9.1/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py` & `global_chem-1.9.1/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/global_chem.py` & `global_chem-1.9.1/global_chem/global_chem.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,32 +44,32 @@
 
 from global_chem.education.cengage.organic_and_inorganic_bronsted_acids import OrganicAndInorganicBronstedAcids
 
 # Medicinal Chemistry - Cannabinoids
 
 from global_chem.medicinal_chemistry.cannabinoids.phytocannabinoids import PhytoCannabinoids
 from global_chem.medicinal_chemistry.cannabinoids.constituents_of_cannabis_sativa import ConstituentsOfCannabisSativa
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_acids import CannabisAcids
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_alcohols import CannabisAlcohols
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_aldehydes import CannabisAldehydes
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_amino_acids import CannabisAminoAcids
+from global_chem.medicinal_chemistry.cannabinoids.acids import CannabisAcids
+from global_chem.medicinal_chemistry.cannabinoids.alcohols import CannabisAlcohols
+from global_chem.medicinal_chemistry.cannabinoids.aldehydes import CannabisAldehydes
+from global_chem.medicinal_chemistry.cannabinoids.amino_acids import CannabisAminoAcids
 from global_chem.medicinal_chemistry.cannabinoids.cannabinoids import Cannabinoids
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_esters_and_lactones import CannabisEstersAndLactones
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_fatty_acids import CannabisFattyAcids
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_flavanoidglycosides import CannabisFlavanoidGlycosides
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_hydrocarbons import CannabisHydrocarbons
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_ketones import CannabisKetones
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_nitrogenous_compounds import CannabisNitrogenousCompounds
+from global_chem.medicinal_chemistry.cannabinoids.esters_and_lactones import CannabisEstersAndLactones
+from global_chem.medicinal_chemistry.cannabinoids.fatty_acids import CannabisFattyAcids
+from global_chem.medicinal_chemistry.cannabinoids.flavanoidglycosides import CannabisFlavanoidGlycosides
+from global_chem.medicinal_chemistry.cannabinoids.hydrocarbons import CannabisHydrocarbons
+from global_chem.medicinal_chemistry.cannabinoids.ketones import CannabisKetones
+from global_chem.medicinal_chemistry.cannabinoids.nitrogenous_compounds import CannabisNitrogenousCompounds
 from global_chem.medicinal_chemistry.cannabinoids.non_cannabinoids_phenols import NonCannabinoidPhenols
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_pigments import CannabisPigments
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_proteins_glycoproteins_enzymes import CannabisProteinsGlycoproteinsEnzymes
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_steroids import CannabisSteroids
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_sugars import CannabisSugars
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_terpenes import CannabisTerpenes
-from global_chem.medicinal_chemistry.cannabinoids.cannabis_vitamins import CannabisVitamins
+from global_chem.medicinal_chemistry.cannabinoids.pigments import CannabisPigments
+from global_chem.medicinal_chemistry.cannabinoids.proteins_glycoproteins_enzymes import CannabisProteinsGlycoproteinsEnzymes
+from global_chem.medicinal_chemistry.cannabinoids.steroids import CannabisSteroids
+from global_chem.medicinal_chemistry.cannabinoids.sugars import CannabisSugars
+from global_chem.medicinal_chemistry.cannabinoids.terpenes import CannabisTerpenes
+from global_chem.medicinal_chemistry.cannabinoids.vitamins import CannabisVitamins
 
 # Medicinal Chemistry - International
 
 from global_chem.medicinal_chemistry.chinese.how_to_live_longer import HowToLiveLonger
 
 # Medicinal Chemistry - Warheads
 
@@ -107,36 +107,30 @@
 from global_chem.food.color_additives.fda_list_two import FDAListTwo
 from global_chem.food.color_additives.fda_list_three import FDAListThree
 from global_chem.food.color_additives.fda_list_four import FDAListFour
 from global_chem.food.color_additives.fda_list_five import FDAListFive
 from global_chem.food.color_additives.fda_list_six import FDAListSix
 from global_chem.food.color_additives.fda_list_seven import FDAListSeven
 
-# Food / Spices / Thai Ginger
 
-from global_chem.food.spices.thai_ginger.thai_ginger_cyclic_dipeptides import ThaiGingerCyclicDipeptides
-from global_chem.food.spices.thai_ginger.thai_ginger_diaryl_heptanoids import ThaiGingerDiarylHeptanoids
-from global_chem.food.spices.thai_ginger.thai_ginger_fatty_acids_and_esters import ThaiGingerFattyAcidsAndEsters
-from global_chem.food.spices.thai_ginger.thai_ginger_flavonoids import ThaiGingerFlavonoids
-from global_chem.food.spices.thai_ginger.thai_ginger_phenolics import ThaiGingerPhenolics
-from global_chem.food.spices.thai_ginger.thai_ginger_polysaccharides import ThaiGingerPolysaccharides
-from global_chem.food.spices.thai_ginger.thai_ginger_terpenoids import ThaiGingerTerpenoids
 
 # Food/Fruits/Mango
 
-from global_chem.food.fruits.mango.mango_phytocompounds import MangoPhytocompounds
-from global_chem.food.fruits.mango.mango_fatty_acids import MangoFattyAcids
-from global_chem.food.fruits.mango.mango_flavonoids import MangoFlavonoids
+
+from global_chem.food.fruits.mango.mango_phyto_compounds import MangoPhytocompounds
 from global_chem.food.fruits.mango.mango_phenolic_acids import MangoPhenolicAcids
 from global_chem.food.fruits.mango.mango_vitamins import MangoVitamins
+from global_chem.food.fruits.mango.mango_fatty_acids import MangoFattyAcids
 from global_chem.food.fruits.mango.mango_amino_acids import MangoAminoAcids
+from global_chem.food.fruits.mango.mango_flavonoids import MangoFlavonoids
 
 # Narcotics
 
 from global_chem.narcotics.pihkal import Pihkal
+from global_chem.narcotics.black_market import BlackMarket
 from global_chem.narcotics.schedule_one import ScheduleOne
 from global_chem.narcotics.schedule_two import ScheduleTwo
 from global_chem.narcotics.schedule_three import ScheduleThree
 from global_chem.narcotics.schedule_four import ScheduleFour
 from global_chem.narcotics.schedule_five import ScheduleFive
 
 # Interstellar Space
@@ -467,15 +461,15 @@
         'cannabis_acids': CannabisAcids,                                                 # Suliman Sharif
         'cannabis_alcohols': CannabisAlcohols,                                           # Suliman Sharif
         'cannabis_aldehydes': CannabisAldehydes,                                         # Suliman Sharif
         'cannabis_amino_acids': CannabisAminoAcids,                                      # Suliman Sharif
         'cannabinoids': Cannabinoids,                                                    # Suliman Sharif
         'cannabis_esters_and_lactones': CannabisEstersAndLactones,                       # Suliman Sharif
         'cannabis_fatty_acids': CannabisFattyAcids,                                      # Suliman Sharif
-        'cannabis_flavanoidglycosides': CannabisFlavanoidGlycosides,                    # Suliman Sharif
+        'cannabis_flavanoid_glycosides': CannabisFlavanoidGlycosides,                    # Suliman Sharif
         'cannabis_hydrocarbons': CannabisHydrocarbons,                                   # Suliman Sharif
         'cannabis_ketones': CannabisKetones,                                             # Suliman Sharif
         'cannabis_nitrogenous_compounds': CannabisNitrogenousCompounds,                  # Suliman Sharif
         'non_cannabinoid_phenols': NonCannabinoidPhenols,                                # Suliman Sharif
         'cannabis_pigments': CannabisPigments,                                           # Suliman Sharif
         'cannabis_proteins_glycoproteins_enzymes': CannabisProteinsGlycoproteinsEnzymes, # Suliman Sharif
         'cannabis_steroids': CannabisSteroids,                                           # Suliman Sharif
@@ -487,27 +481,20 @@
         'chemicals_from_biomass': ChemicalsFromBioMass,                                  # Anthony Maiorana & Suliman Sharif
         'drugs_from_snake_venom': DrugsFromSnakeVenom,                                   # Suliman Sharif
         'oral_contraceptives': OralContraceptives,                                       # Suliman Sharif
         'surfactants': Surfactants,                                                      # Yiling Nan & Suliman Sharif
         'lanthipeptides': LanthiPeptides,                                                # Prabin Baral & Suliman Sharif
         'alternative_jet_fuels': AlternativeJetFuels,                                    # Suliman Sharif
         'common_regex_patterns': CommonRegexPatterns,                                    # Chris Burke & Suliman Sharif
-        'mango_phytocompounds': MangoPhytocompounds,                                     # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
-        'mango_amino_acids': MangoAminoAcids,                                            # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
-        'mango_phenolic_acids': MangoPhenolicAcids,                                      # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
-        'mango_fatty_acids': MangoFattyAcids,                                            # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
-        'mango_vitamins': MangoVitamins,                                                 # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
-        'mango_flavonoids': MangoFlavonoids,                                             # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
-        'thai_ginger_cyclic_dipeptides': ThaiGingerCyclicDipeptides,                     # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
-        'thai_ginger_diaryl_heptanoids': ThaiGingerDiarylHeptanoids,                     # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
-        'thai_ginger_fatty_acids_and_esters': ThaiGingerFattyAcidsAndEsters,             # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
-        'thai_ginger_flavonoids': ThaiGingerFlavonoids,                                  # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
-        'thai_ginger_phenolics': ThaiGingerPhenolics,                                    # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
-        'thai_ginger_polysaccharides': ThaiGingerPolysaccharides,                        # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
-        'thai_ginger_terpenoids': ThaiGingerTerpenoids                                   # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
+        'mango_phytocompounds': MangoPhytocompounds,                                     # Damilola Bodun & Sevien Schulhofff
+        'mango_amino_acids': MangoAminoAcids,                                            # Damilola Bodun & Sevien Schulhofff
+        'mango_phenolic_acids': MangoPhenolicAcids,                                      # Damilola Bodun & Sevien Schulhofff
+        'mango_fatty_acids': MangoFattyAcids,                                            # Damilola Bodun & Sevien Schulhofff
+        'mango_vitamins': MangoVitamins,                                                 # Damilola Bodun & Sevien Schulhofff
+        'mango_flavonoids': MangoFlavonoids                                              # Damilola Bodun & Sevien Schulhofff  
     }
 
     __INCOMPLETE_NODES = {
         # 'named_reactions_in_organic_synthesis': NamedReactionsInOrganicSynthesis # Aziza Frank & Bettina Lier & Suliman Sharif
     }
 
     def __init__(self, verbose=False):
```

### Comparing `global_chem-1.8.5.3/global_chem/interstellar_space/asteroid_ryugu.py` & `global_chem-1.9.1/global_chem/interstellar_space/asteroid_ryugu.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/interstellar_space/interstellar_space.py` & `global_chem-1.9.1/global_chem/interstellar_space/interstellar_space.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/materials/clay/montmorillonite_adsorption.py` & `global_chem-1.9.1/global_chem/materials/clay/montmorillonite_adsorption.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/materials/polymers/common_monomer_repeating_units.py` & `global_chem-1.9.1/global_chem/materials/polymers/common_monomer_repeating_units.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_acids.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_alcohols.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/alcohols.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_aldehydes.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/aldehydes.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_amino_acids.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/amino_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_esters_and_lactones.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_fatty_acids.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_flavanoidglycosides.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # ----------------------------------------
 
 class CannabisFlavanoidGlycosides(object):
 
   def __init__(self):
 
-    self.name = 'cannabis_flavanoidglycosides'
+    self.name = 'cannabis_flavanoid_glycosides'
 
   @staticmethod
   def get_smiles():
 
     smiles = {
       'apigenin-7-O-para coumarylglucoside': r'OC1C(COC(=O)\C=C\C2=CC=C(O)C=C2)OC(OC2=CC(O)=C3C(=O)C=C(OC3=C2)C2=CC=C(O)C=C2)C(O)C1',
       'cosmosioside': 'OCC1OC(Oc2cc(O)c3C(=O)C=C(Oc3c2)c4ccc(O)cc4)C(O)C(O)C1O',
```

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_hydrocarbons.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_ketones.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/ketones.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_nitrogenous_compounds.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_pigments.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/pigments.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_proteins_glycoproteins_enzymes.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_steroids.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/steroids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_sugars.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/sugars.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/cannabis_terpenes.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/terpenes.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/rings/rings_in_drugs.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/rings/rings_in_drugs.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py` & `global_chem-1.9.1/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/miscellaneous/amino_acids.py` & `global_chem-1.9.1/global_chem/miscellaneous/amino_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/miscellaneous/open_smiles.py` & `global_chem-1.9.1/global_chem/miscellaneous/open_smiles.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/miscellaneous/vitamins.py` & `global_chem-1.9.1/global_chem/miscellaneous/vitamins.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/narcotics/pihkal.py` & `global_chem-1.9.1/global_chem/narcotics/pihkal.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/narcotics/schedule_five.py` & `global_chem-1.9.1/global_chem/narcotics/schedule_five.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/narcotics/schedule_four.py` & `global_chem-1.9.1/global_chem/narcotics/schedule_four.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/narcotics/schedule_one.py` & `global_chem-1.9.1/global_chem/narcotics/schedule_one.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/narcotics/schedule_three.py` & `global_chem-1.9.1/global_chem/narcotics/schedule_three.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/narcotics/schedule_two.py` & `global_chem-1.9.1/global_chem/narcotics/schedule_two.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py` & `global_chem-1.9.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py` & `global_chem-1.9.1/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/organic_synthesis/solvents/common_organic_solvents.py` & `global_chem-1.9.1/global_chem/organic_synthesis/solvents/common_organic_solvents.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/peptides/lanthipeptides.py` & `global_chem-1.9.1/global_chem/peptides/lanthipeptides.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/proteins/kinases/braf/braf_inhibitors.py` & `global_chem-1.9.1/global_chem/proteins/kinases/braf/braf_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py` & `global_chem-1.9.1/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/sex/contraceptives/oral_contraceptives.py` & `global_chem-1.9.1/global_chem/sex/contraceptives/oral_contraceptives.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/sex/exsens/exsens_products.py` & `global_chem-1.9.1/global_chem/sex/exsens/exsens_products.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/sex/exsens/lube.py` & `global_chem-1.9.1/global_chem/sex/exsens/lube.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py` & `global_chem-1.9.1/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py` & `global_chem-1.9.1/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem/warfare/organophosphorous_nerve_agents.py` & `global_chem-1.9.1/global_chem/warfare/organophosphorous_nerve_agents.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/global_chem.egg-info/PKG-INFO` & `global_chem-1.9.1/global_chem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global-chem
-Version: 1.8.5.3
+Version: 1.9.1
 Summary: UNKNOWN
 Home-page: https://www.github.com/Sulstice/global-chem
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: MPL 2.0
 Description: <h1 align="center">Organizing The Chemical Universe</h1>
         
@@ -169,14 +169,15 @@
         'chemicals_from_biomass': ChemicalsFromBioMass,                           # Anthony Maiorana & Suliman Sharif
         'salt': Salt,                                                             # Suliman Sharif
         'drugs_from_snake_venom': DrugsFromSnakeVenom,                            # Suliman Sharif
         'oral_contraceptives': OralContraceptives,                                # Suliman Sharif
         'surfactants': Surfactants,                                               # Yiling Nan & Suliman Sharif
         'lanthipeptides: LanthiPeptides                                           # Prabin Baral & Suliman Sharif
         'alternative_jet_fuels': AlternativeJetFuels                              # Suliman Sharif
+        'mango_amino_acids': MangoPhytocompounds,                                 # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_amino_acids': MangoAminoAcids,                                     # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_phenolic_acids': MangoPhenolicAcids,                               # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_fatty_acids': MangoFattyAcids,                                     # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_vitamins': MangoVitamins,                                          # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'mango_flavonoids': MangoFlavonoids                                       # Damilola Bodun & Sevien Schulhofff & Suliman Sharif
         'thai_ginger_cyclic_dipeptides': ThaiGingerCyclicDipeptides,              # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
         'thai_ginger_diaryl_heptanoids': ThaiGingerDiarylHeptanoids,              # Katukoliya Gamage Anuththara Samadhi & Suliman Sharif
@@ -233,14 +234,15 @@
         | Cengage Bronsted Acids              | 42           | https://cxp.cengage.com/contentservice/assets/owms01h/references/chemtables/org_chem/pKaTable.html                                                                                                                                                                                                                  |
         | Chemicals From Biomass              | 17           | Wittcoff, Harold A., et al. Industrial Organic Chemicals: Wittcoff/Organic Chemicals. John Wiley & Sons, Inc., 2004                                                                                                                                                                                                 |
         | Drugs From Snake Venom              | 7            | Oliveira, Ana L., et al. “The Chemistry of Snake Venom and Its Medicinal Potential.” Nature Reviews Chemistry, vol. 6, no. 7, July 2022, pp. 451–69                                                                                                                                                                 |
         | Oral Contraceptives                 | 17           | Coleman, William F. “The Molecules of Oral Contraceptives.” Journal of Chemical Education, vol. 87, no. 7, July 2010, pp. 760–61.                                                                                                                                                                                   |
         | Surfactants for Skin                | 36           | Date, Abhijit A., and Vandana B. Patravale. “Microemulsions: Applications in Transdermal and Dermal Delivery.” Critical Reviews&trade; in Therapeutic Drug Carrier Systems, vol. 24, no. 6, 2007.                                                                                                                   |
         | LanthiPeptides                      | 2            | Pokhrel, Rudramani, et al. “Molecular Mechanisms of Pore Formation and Membrane Disruption by the Antimicrobial Lantibiotic Peptide Mutacin 1140.” Physical Chemistry Chemical Physics, vol. 21, no. 23, June 2019, pp. 12530–39.                                                                                   |
         | Alternative Jet Fuels               | 59           | Chemical Composition and Fuel Properties of Alternative Jet Fuels :: BioResources. https://bioresources.cnr.ncsu.edu/.                                                                                                                                                                                              |
+        | Mango Phytocompounds                | 87            | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Amino Acids                   | 19           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Phenoloic Acids               | 10           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Fatty Acids                   | 24           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Vitamins                      | 10           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Mango Flavonoids                    | 11           | Maldonado-Celis, Maria Elena, et al. “Chemical Composition of Mango (Mangifera Indica L.) Fruit: Nutritional and Phytochemical Compounds.” Frontiers in Plant Science, vol. 10, Oct. 2019, p. 1073.                                                                                                                 |
         | Thai Ginger Cyclic Dipeptides       | 6            | Wang, Si-Yu, et al. “Kaempferia Galanga L.: Progresses in Phytochemistry, Pharmacology, Toxicology and Ethnomedicinal Uses.” Frontiers in Pharmacology, vol. 12, 2021.                                                                                                                                              |
         | Thai Ginger Diaryl Heptanoids       | 6            | Wang, Si-Yu, et al. “Kaempferia Galanga L.: Progresses in Phytochemistry, Pharmacology, Toxicology and Ethnomedicinal Uses.” Frontiers in Pharmacology, vol. 12, 2021.                                                                                                                                              |
@@ -411,17 +413,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: graphing
 Provides-Extra: forcefields
 Provides-Extra: bioinformatics
 Provides-Extra: cheminformatics
 Provides-Extra: quantum_chemistry
 Provides-Extra: development_operations
```

### Comparing `global_chem-1.8.5.3/global_chem.egg-info/SOURCES.txt` & `global_chem-1.9.1/global_chem.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,18 @@
 global_chem/food/color_additives/fda_list_two.py
 global_chem/food/fruits/__init__.py
 global_chem/food/fruits/mango/__init__.py
 global_chem/food/fruits/mango/mango_amino_acids.py
 global_chem/food/fruits/mango/mango_fatty_acids.py
 global_chem/food/fruits/mango/mango_flavonoids.py
 global_chem/food/fruits/mango/mango_phenolic_acids.py
-global_chem/food/fruits/mango/mango_phytocompounds.py
+global_chem/food/fruits/mango/mango_phyto_compounds.py
 global_chem/food/fruits/mango/mango_vitamins.py
 global_chem/food/salt/__init__.py
 global_chem/food/salt/salt.py
-global_chem/food/spices/__init__.py
-global_chem/food/spices/thai_ginger/__init__.py
-global_chem/food/spices/thai_ginger/thai_ginger_cyclic_dipeptides.py
-global_chem/food/spices/thai_ginger/thai_ginger_diaryl_heptanoids.py
-global_chem/food/spices/thai_ginger/thai_ginger_fatty_acids_and_esters.py
-global_chem/food/spices/thai_ginger/thai_ginger_flavonoids.py
-global_chem/food/spices/thai_ginger/thai_ginger_phenolics.py
-global_chem/food/spices/thai_ginger/thai_ginger_polysaccharides.py
-global_chem/food/spices/thai_ginger/thai_ginger_terpenoids.py
 global_chem/formulation/__init__.py
 global_chem/formulation/excipients/__init__.py
 global_chem/formulation/excipients/allergen_inactive_ingredients.py
 global_chem/formulation/excipients/biopharmaceutics_class_three/__init__.py
 global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py
 global_chem/formulation/excipients/monoclonal_antibodies/__init__.py
 global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py
@@ -61,34 +52,34 @@
 global_chem/materials/__init__.py
 global_chem/materials/clay/__init__.py
 global_chem/materials/clay/montmorillonite_adsorption.py
 global_chem/materials/polymers/__init__.py
 global_chem/materials/polymers/common_monomer_repeating_units.py
 global_chem/medicinal_chemistry/__init__.py
 global_chem/medicinal_chemistry/cannabinoids/__init__.py
+global_chem/medicinal_chemistry/cannabinoids/acids.py
+global_chem/medicinal_chemistry/cannabinoids/alcohols.py
+global_chem/medicinal_chemistry/cannabinoids/aldehydes.py
+global_chem/medicinal_chemistry/cannabinoids/amino_acids.py
 global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_acids.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_alcohols.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_aldehydes.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_amino_acids.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_esters_and_lactones.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_fatty_acids.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_flavanoidglycosides.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_hydrocarbons.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_ketones.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_nitrogenous_compounds.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_pigments.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_proteins_glycoproteins_enzymes.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_steroids.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_sugars.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_terpenes.py
-global_chem/medicinal_chemistry/cannabinoids/cannabis_vitamins.py
 global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py
+global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py
+global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py
+global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py
+global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py
+global_chem/medicinal_chemistry/cannabinoids/ketones.py
+global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py
 global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py
 global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py
+global_chem/medicinal_chemistry/cannabinoids/pigments.py
+global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py
+global_chem/medicinal_chemistry/cannabinoids/steroids.py
+global_chem/medicinal_chemistry/cannabinoids/sugars.py
+global_chem/medicinal_chemistry/cannabinoids/terpenes.py
+global_chem/medicinal_chemistry/cannabinoids/vitamins.py
 global_chem/medicinal_chemistry/chinese/__init__.py
 global_chem/medicinal_chemistry/chinese/how_to_live_longer.py
 global_chem/medicinal_chemistry/rings/__init__.py
 global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py
 global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py
 global_chem/medicinal_chemistry/rings/rings_in_drugs.py
 global_chem/medicinal_chemistry/scaffolds/__init__.py
@@ -117,14 +108,15 @@
 global_chem/medicinal_chemistry/world_health_organization/watch_group_antibiotics.py
 global_chem/miscellaneous/__init__.py
 global_chem/miscellaneous/amino_acids.py
 global_chem/miscellaneous/open_smiles.py
 global_chem/miscellaneous/regex_patterns.py
 global_chem/miscellaneous/vitamins.py
 global_chem/narcotics/__init__.py
+global_chem/narcotics/black_market.py
 global_chem/narcotics/pihkal.py
 global_chem/narcotics/schedule_five.py
 global_chem/narcotics/schedule_four.py
 global_chem/narcotics/schedule_one.py
 global_chem/narcotics/schedule_three.py
 global_chem/narcotics/schedule_two.py
 global_chem/organic_synthesis/__init__.py
```

### Comparing `global_chem-1.8.5.3/global_chem.egg-info/requires.txt` & `global_chem-1.9.1/global_chem.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `global_chem-1.8.5.3/setup.py` & `global_chem-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 else:
     long_description = 'GlobalChem - Your Chemical Knowledge Graph for Chemistry'
 
 # exec
 # ----
 setup(
     name="global_chem",
-    version="1.8.5.3",
+    version="1.9.1",
     packages=find_packages(),
     license='MPL 2.0',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/Sulstice/global-chem",
     install_requires=[],
     long_description=long_description,
@@ -64,14 +64,11 @@
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
     ],
     test_suite='tests',
     tests_require=TEST_REQUIREMENTS,
 )
```

