# Comparing `tmp/CTG_Utils-1.1.5.tar.gz` & `tmp/CTG_Utils-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTG_Utils-1.1.5.tar", last modified: Thu May 16 15:51:27 2024, max compression
+gzip compressed data, was "CTG_Utils-1.1.6.tar", last modified: Fri May 17 12:33:35 2024, max compression
```

## Comparing `CTG_Utils-1.1.5.tar` & `CTG_Utils-1.1.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.165170 CTG_Utils-1.1.5/
-drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.113063 CTG_Utils-1.1.5/CTG_Utils/
-drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.130551 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/
--rw-rw-rw-   0        0        0     9358 2024-05-15 14:59:23.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTGClasses.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.142522 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/
--rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
--rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
--rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
--rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
--rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
--rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
--rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
--rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
--rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
--rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
--rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
--rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_config.py
--rw-rw-rw-   0        0        0    19497 2024-05-16 15:18:28.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_effectif.py
--rw-rw-rw-   0        0        0    11917 2024-05-16 10:06:26.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_plot.py
--rw-rw-rw-   0        0        0    15863 2024-05-16 13:51:41.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_synthese.py
--rw-rw-rw-   0        0        0     4328 2024-05-16 11:35:42.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_utility.py
--rw-rw-rw-   0        0        0      214 2024-05-15 06:16:14.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.164173 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/
--rw-rw-rw-   0        0        0    16064 2024-05-14 08:52:29.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/GUI_Globals.py
--rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageDivers.py
--rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageEffectif.py
--rw-rw-rw-   0        0        0    11622 2024-05-16 07:23:59.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageSorties.py
--rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageSynthese.py
--rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageTendance.py
--rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Page_Classes.py
--rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Useful_Classes.py
--rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Useful_Functions.py
--rw-rw-rw-   0        0        0      221 2024-05-15 06:17:11.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.123741 CTG_Utils-1.1.5/CTG_Utils.egg-info/
--rw-rw-rw-   0        0        0      681 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1304 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.5/LICENSE
--rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      681 2024-05-16 15:51:27.165170 CTG_Utils-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 15:51:27.165170 CTG_Utils-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1367 2024-05-16 15:50:18.000000 CTG_Utils-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:33:35.513429 CTG_Utils-1.1.6/
+drwxrwxrwx   0        0        0        0 2024-05-17 12:33:35.456981 CTG_Utils-1.1.6/CTG_Utils/
+drwxrwxrwx   0        0        0        0 2024-05-17 12:33:35.477712 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/
+-rw-rw-rw-   0        0        0     9766 2024-05-17 09:17:02.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTGClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:33:35.489680 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/
+-rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
+-rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
+-rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
+-rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
+-rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
+-rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
+-rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
+-rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
+-rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
+-rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
+-rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
+-rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_config.py
+-rw-rw-rw-   0        0        0    18399 2024-05-17 12:19:34.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_effectif.py
+-rw-rw-rw-   0        0        0    11562 2024-05-17 09:25:57.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_plot.py
+-rw-rw-rw-   0        0        0    15508 2024-05-17 09:25:57.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_synthese.py
+-rw-rw-rw-   0        0        0     3865 2024-05-17 09:08:39.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_utility.py
+-rw-rw-rw-   0        0        0      214 2024-05-15 06:16:14.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_Func/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:33:35.512398 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/
+-rw-rw-rw-   0        0        0    16064 2024-05-14 08:52:29.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/GUI_Globals.py
+-rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageDivers.py
+-rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageEffectif.py
+-rw-rw-rw-   0        0        0    11622 2024-05-16 07:23:59.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageSorties.py
+-rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageSynthese.py
+-rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageTendance.py
+-rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/Page_Classes.py
+-rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/Useful_Classes.py
+-rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/Useful_Functions.py
+-rw-rw-rw-   0        0        0      221 2024-05-15 06:17:11.000000 CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:33:35.471124 CTG_Utils-1.1.6/CTG_Utils.egg-info/
+-rw-rw-rw-   0        0        0      681 2024-05-17 12:33:34.000000 CTG_Utils-1.1.6/CTG_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1304 2024-05-17 12:33:34.000000 CTG_Utils-1.1.6/CTG_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 12:33:34.000000 CTG_Utils-1.1.6/CTG_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-17 12:33:34.000000 CTG_Utils-1.1.6/CTG_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-17 12:33:34.000000 CTG_Utils-1.1.6/CTG_Utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      681 2024-05-17 12:33:35.512398 CTG_Utils-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 12:33:35.513429 CTG_Utils-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2024-05-17 12:31:02.000000 CTG_Utils-1.1.6/setup.py
```

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTGClasses.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTGClasses.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         self.effectif_1 = df_1  # effectif year moins un
 
         self.moy_age_entrants, self.nbr_nouveaux_licencié, self.nouveaux_licenciés_noms = self.nouveaux_entrants()
         self.moy_age_sortants, self.nbr_sortants, self.sortants_noms = self.sortants() 
         
         self.cotisation_licence,self.cotisation_totale, self.cotisation_ctg = self.cotisation()
         
+        self.membres_sympathisants, self.nbr_membres_sympathisants = self.membres_sympathisants()
+        
     @staticmethod
     def distance_(row,dh):
     
         # Standard library imports
         from math import asin, cos, radians, sin, sqrt
         
         # Third party imports        
@@ -56,17 +58,14 @@
         return np.round(dist,1)
     
     def stat(self):
     
         # Standard library imports
         from pathlib import Path
         from tkinter import messagebox
-        
-        # Internal imports
-        from CTG_Utils.CTG_Func.CTG_utility import read_correction_effectifs
 
         da = self.effectif.groupby('Sexe')['Age'].agg(['count','median','max','min'])
         res = self.effectif['Age'].agg(['count','median','max','min']).tolist()
         stat = []
         stat.append(f"Année : {self.year}")
         stat.append(" ")
         nbr_membres = round(res[0],0)
@@ -83,23 +82,17 @@
         stat.append(f"Age médian des hommes : {round(da.loc['M','median'],1)} ans")
         stat.append(f"Age maximum des femmes : {round(da.loc['F','max'],1)} ans")
         stat.append(f"Age maximum des hommes : {round(da.loc['M','max'],1)} ans")
         stat.append(f"Age minimum des femmes : {round(da.loc['F','min'],1)} ans")
         stat.append(f"Age minimum des hommes : {round(da.loc['M','min'],1)} ans")
         stat.append(' ')
         
-        correction = read_correction_effectifs(self.year,self.ctg_path)
-        if correction["dic_part_club"] is not None:
-            part_club_dic = correction["dic_part_club"]
-            stat.append(f'Nombre de membres sympatisant : {len(part_club_dic)}')
-            part_club_list = '; '.join([f"{x.split(',')[0][0]}. {x.split(',')[1]}"  
-                                        for x in correction['dic_part_club']])
-            stat.append(f'Membres sympatisants : {part_club_list}')
-        else:
-            stat.append(f'Nombre de membres sympatisants : inconnu ')
+        
+        stat.append(f'Nombre de membres sympatisant : {self.nbr_membres_sympathisants}')  
+        stat.append(f'Membres sympatisants : {self.membres_sympathisants}')
         stat.append(' ')
         
         
         stat.append(f"{self.nbr_nouveaux_licencié} nouveaux licenciés de moyenne d'âge de {round(self.moy_age_entrants,1)} ans")
         stat.append(f"Liste des nouveaux :\n{self.nouveaux_licenciés_noms}")
         stat.append(f"{self.nbr_sortants} licences non renouvellées de moyenne d'âge de {round(self.moy_age_sortants,1)} ans")
         stat.append(f"Liste des sortants :\n{self.sortants_noms}")
@@ -120,15 +113,15 @@
             stat.append(f'{pratique} : {da[pratique]}')
         stat.append(' ')
         
         self.effectif = self.effectif.rename(columns={'\n\t\t\t\tAbonnements':'Abonnements'})
         nbr_abonnements = len(self.effectif.query('Abonnements == "Oui"'))
         stat.append(f"Nombre d'abonnés à la revue FFCT : {nbr_abonnements} ({round(100*nbr_abonnements/nbr_membres)} %)")
         stat.append(f"\ncotisation licence ffct : {self.cotisation_licence} €")
-        stat.append(f"cotisation assurence : {self.cotisation_totale-self.cotisation_licence} €")
+        stat.append(f"cotisation totale : {self.cotisation_totale} €")
         stat.append(f"cotisation CTG : {self.cotisation_ctg} €")
         path_info_effectif = self.ctg_path / Path(str(self.year)) / Path('STATISTIQUES')/Path(f'info_effectif_{self.year}.txt')
         stat.append(f"\n Ces information sont disponibles dans le fichier : \n{path_info_effectif}")
         stat ='\n'.join(stat)
         messagebox.showinfo(f'Statistique {self.year}',stat)
         
         
@@ -146,14 +139,32 @@
         nouveaux_licenciés_list = []
         for idx,row in dg.iterrows():
             nouveaux_licenciés_list.append(f"{row['Prénom'][0]}. {row['Nom']}")
         nouveaux_licenciés_noms = '; '.join(nouveaux_licenciés_list)
         nbr_nouveaux_licencié = len(dg)
 
         return moy_age_entrants, nbr_nouveaux_licencié, nouveaux_licenciés_noms
+        
+    def membres_sympathisants(self):
+    
+        import os
+        from pathlib import Path
+        import pandas as pd 
+        
+        file_path = self.ctg_path / Path(str(self.year))/Path('DATA')/ Path('membres_sympatisants.xlsx')
+        if os.path.isfile(file_path):
+            membres_sympathisants_df = pd.read_excel(file_path)
+            membres_sympathisants_df['Nom_Prenom'] = membres_sympathisants_df['Nom']+" "+membres_sympathisants_df['Prénom'].str[0]
+            membres_sympathisants = ', '.join(membres_sympathisants_df['Nom_Prenom'].tolist())
+            nbr_membres_sympathisants = len(membres_sympathisants_df)
+        else:
+            nbr_membres_sympathisants = 'inconnu'
+            membres_sympathisants = 'inconnu'
+            
+        return membres_sympathisants, nbr_membres_sympathisants
 
     def sortants(self):
         sortants_id = set(self.effectif_1["N° Licencié"]) - set(self.effectif["N° Licencié"])
         
         dg = self.effectif_1[self.effectif_1['N° Licencié'].isin(sortants_id)]
         
         moy_age_sortants = dg['Age'].mean() + 1
```

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_effectif.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_effectif.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,55 @@
-__all__ = ['correction_effectif',
-           'count_participation',
+__all__ = ['count_participation',
            'inscrit_sejour',
            'parse_date',
            'read_effectif',
            'read_effectif_corrected',
            'evolution_effectif',
            'builds_excel_presence_au_club',
            'statistique_vae',
            'anciennete_au_club',]
                       
 
-def read_effectif_corrected(dic_correction_licence, list_non_licencie, part_club, ctg_path, year=None):
+def read_effectif_corrected(ctg_path, year=None):
     
     '''Lecture du fichier effectif et correction
     '''
     # Standard library imports
     from pathlib import Path
     import datetime
    
     # 3rd party imports
-    import numpy as np
     import pandas as pd
     
     if year is not None:
         file_effectif = str(year) + '.xlsx'
     else:
         currentDateTime = datetime.datetime.now()
         date = currentDateTime.date()
         year = date.strftime("%Y")
         file_effectif = year + '.xlsx'
-    df_effectif = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path(file_effectif))
-    df_effectif = df_effectif[['N° Licencié', 'Nom','Prénom','Sexe','Pratique VAE']]
-    
         
-    for num_licence in dic_correction_licence.keys():
-        idx = df_effectif[df_effectif["N° Licencié"]==num_licence].index
-        df_effectif.loc[idx,'Prénom'] = dic_correction_licence[num_licence]['Prénom']
-        df_effectif.loc[idx,'Nom'] = dic_correction_licence[num_licence]['Nom']
-        
-    prenom, nom, sexe = zip(*part_club)
-    part_club = {'N° Licencié':list(range(len(part_club))), 'Prénom':prenom,'Nom':nom,'Sexe':sexe}
-    df_part_club = pd.DataFrame.from_dict(part_club)
-    df_effectif = pd.concat([df_effectif, df_part_club], ignore_index=True, axis=0)
-    
-    if list_non_licencie:
-        prenom, nom, sexe = zip(*list_non_licencie)
-        dict_non_licencie = {'N° Licencié':np.array(range(len(nom)))+10, 'Prénom':prenom,'Nom':nom,'Sexe':sexe}
+    effectif_df = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path(file_effectif))
+    effectif_df = effectif_df[['N° Licencié', 'Nom','Prénom','Sexe','Pratique VAE']]
+    
+    correction_effectif = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path('correction_effectif.xlsx'))
+    correction_effectif.index = correction_effectif['N° Licencié']
+    membres_sympathisants_df = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path('membres_sympatisants.xlsx'))
     
-        df_non_licencie = pd.DataFrame.from_dict(dict_non_licencie)
-        df_effectif = pd.concat([df_effectif, df_non_licencie], ignore_index=True, axis=0)
+    for num_licence in correction_effectif.index:
+        idx = effectif_df[effectif_df["N° Licencié"]==num_licence].index
+        effectif_df.loc[idx,'Prénom'] = correction_effectif.loc[num_licence,'Prénom']
+        effectif_df.loc[idx,'Nom'] = correction_effectif.loc[num_licence,'Nom']
     
-    df_effectif['Prénom1'] = df_effectif['Prénom'].str[0]
-    df_effectif['Prénom'] = df_effectif['Prénom'].str.replace(' ','-')
+    effectif_df = pd.concat([effectif_df, membres_sympathisants_df], ignore_index=True, axis=0)
     
-    return df_effectif
+    effectif_df['Prénom1'] = effectif_df['Prénom'].str[0]
+    effectif_df['Prénom'] = effectif_df['Prénom'].str.replace(' ','-')
+    
+    return effectif_df
 
 def inscrit_sejour(file,no_match,df_effectif):
 
     # Standard library import
     import functools
     import os
     import unicodedata
@@ -125,39 +117,14 @@
         else:
             dg = pd.DataFrame([[None,None,None,None,sejour,]], columns=['N° Licencié','Nom','Prénom','Sexe','sejour',])
     else:
         dg = pd.DataFrame([[None,None,None,None,sejour,]], columns=['N° Licencié','Nom','Prénom','Sexe','sejour',])
     
     return dg
 
-def correction_effectif(year,ctg_path):
-    
-    # Standard library import
-    from pathlib import Path
-    
-    #3rd party import
-    import yaml
-    
-    #path_cor_yaml = Path(__file__).parent / Path('CTG_RefFiles/CTG_correction.yaml')
-    path_cor_yaml = ctg_path / Path(str(year)) / Path('DATA') / Path('CTG_correction.yaml')
-    
-    with open(path_cor_yaml, "r",encoding='utf8') as stream:
-        data_list_dict = yaml.safe_load(stream)
-    
-    list_non_licencie  = []   
-    if data_list_dict['list_non_licencie']:
-        list_non_licencie = [(x.split(',')[0].strip(),x.split(',')[1].strip(),x.split(',')[2].strip())
-                             for x in data_list_dict['list_non_licencie']]
-    dic_part_club = [(x.split(',')[0].strip(),x.split(',')[1].strip(),x.split(',')[2].strip()) 
-                         for x in data_list_dict['dic_part_club']]
-    dic_correction_licence = data_list_dict['dic_correction_licence']
-    dic_correction_licence = {list(x.keys())[0] : list(x.values())[0] for x in dic_correction_licence}
-    
-    return list_non_licencie, dic_correction_licence, dic_part_club
-
     
 def count_participation(path,ctg_path,year,info_rando):
     
     import os
     import re
     from pathlib import Path
 
@@ -165,23 +132,27 @@
     
     flag_sejour = False
     if os.path.split(path)[-1] == 'SEJOUR' : 
         flag_sejour = True
 
     type_sortie_default = os.path.basename(path)
     type_sortie_default = type_sortie_default.split('.', 1)[0]
-    list_non_licencie, dic_correction_licence, dic_part_club = correction_effectif(year,ctg_path)
 
-    df_effectif = read_effectif_corrected(dic_correction_licence, list_non_licencie, dic_part_club,ctg_path,year)
+    df_effectif = read_effectif_corrected(ctg_path,year)
 
     no_match = []
     df_list = [] 
+    info_sejours = []
     sejours = [x for x in os.listdir( path / Path('CSV')) if x.endswith('.csv')]
     
-    
+    sejours_xlsx = [x for x in os.listdir( path / Path('EXCEL')) if x.endswith('.xlsx')]
+    for sejours_xlsx in sejours_xlsx:
+        path_file_xlsx = path / Path('EXCEL') / Path(sejours_xlsx)
+        os.remove(path_file_xlsx)
+        
     nbr_moyen_participants = 0
     counter = 1
     for sejour in sejours:
         dg = inscrit_sejour( path / Path('CSV') /Path(sejour),no_match,df_effectif)
         
         if re.findall(r'^\d{4}[-_]',sejour):
             date = sejour[2:10].replace('_','-')
@@ -202,20 +173,26 @@
                 dg['nbr_jours'] = dh['nbr_jours'].tolist()[0]    
             
         if dg.reset_index().loc[0,'Nom'] is not None:
             nbr_inscrits = len(dg)
             if nbr_inscrits != 0:
                 nbr_moyen_participants = nbr_moyen_participants + (nbr_inscrits - nbr_moyen_participants)/counter
                 counter += 1
-                print(f"{os.path.split(path)[-1]} :{sejour}, Nombre d'inscrits : {nbr_inscrits}")
+                info_sejours.append(f"{os.path.split(path)[-1]} :{sejour}, Nombre d'inscrits : {nbr_inscrits}")
+               
         df_list.append(dg)
         file_store = os.path.splitext(sejour)[0]+'.xlsx'
         dg.to_excel(path / Path('EXCEL') / Path(file_store))
+       
+    info_sejours.append(f"Nombre d'évènenements : {counter-1}. Nombre moyen de participants : {nbr_moyen_participants}")
+    info_sejours = '\n'.join(info_sejours)
+    info_sejours_path = ctg_path / Path(str(year)) / Path('STATISTIQUES')/ Path(type_sortie_default+'.txt')
+    with open(info_sejours_path,'w') as f:
+        f.write(info_sejours)
         
-    print(f"Nombre d'évènenements : {counter-1}. Nombre moyen de participants : {nbr_moyen_participants}")
     nbr_evenement = counter-1 
     if counter-1 > 0 :  #
         df_total = pd.concat(df_list,ignore_index=True)
     else:
         return (None, None, None)
 
 
@@ -429,15 +406,15 @@
     dic['date'] = list_date_
     
     df = pd.DataFrame.from_dict(dic)
     split_df = pd.DataFrame(df['date'].tolist(), columns=list_date)
     
     df = pd.concat([df, split_df], axis=1)
     df = df.drop('date',axis=1)
-    out_path = ctg_path / Path(str(list_date[-1])) / Path('DATA') / Path('effectif_history.xlsx')
+    out_path = ctg_path / Path(str(list_date[-1])) / Path('STATISTIQUES') / Path('effectif_history.xlsx')
     df.to_excel(out_path)
     return out_path
     
 def statistique_vae(ctg_path):
 
     from datetime import datetime
     from pathlib import Path
@@ -495,15 +472,15 @@
             if y[i] != 0:
                 plt.text(x[i]-0.2,y[i]+offset,round(y[i],1),size=15)
                 
     currentDateTime = datetime.datetime.now()
     date = currentDateTime.date()
     current_year = int(date.strftime("%Y"))
     
-    in_path = ctg_path / Path(str(current_year)) / Path('DATA') / Path('effectif_history.xlsx')
+    in_path = ctg_path / Path(str(current_year)) / Path('STATISTIQUES') / Path('effectif_history.xlsx')
     df = pd.read_excel(in_path)
     eff = []
     
     years = list(range(2012,current_year+1))
     for year in years:
         dg = df.dropna(subset=[year,current_year])
         eff.append(len(dg))
```

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_plot.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,14 @@
     
     # Third party imports
     import matplotlib.pyplot as plt 
     import pandas as pd
     
     # Internal imports
     from CTG_Utils.CTG_Func.CTG_effectif import read_effectif
-    from CTG_Utils.CTG_Func.CTG_effectif import correction_effectif
     from CTG_Utils.CTG_Func.CTG_effectif import read_effectif_corrected
     from CTG_Utils.CTG_Func.CTG_effectif import count_participation
     from CTG_Utils.CTG_Func.CTG_effectif import parse_date
     
     def addlabels(x,y):
         import os
         for i in range(len(x)):
@@ -221,19 +220,15 @@
         if len(text_message) : messagebox.showinfo('WARNING',text_message )
     
     if year is None:
         currentDateTime = datetime.datetime.now()
         date = currentDateTime.date()
         year = date.strftime("%Y")
         
-    list_non_licencie, dic_correction_licence, dic_part_club = correction_effectif(year,ctg_path)
-    df_effectif = read_effectif_corrected(dic_correction_licence,
-                                          list_non_licencie,
-                                          dic_part_club,
-                                          ctg_path,
+    df_effectif = read_effectif_corrected(ctg_path,
                                           year)
     
     dic_sexe = dict(zip(df_effectif['N° Licencié'], df_effectif['Sexe']))
     dic_sexe[None] = 'irrelevant'
     dic_vae =dict(zip(df_effectif['N° Licencié'],df_effectif['Pratique VAE']))
 
     df_total['sexe'] = df_total['N° Licencié'].map(dic_sexe)
```

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_synthese.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_synthese.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,984 +9,962 @@
 00000080: 7479 2069 6d70 6f72 7473 2020 2020 0d0a  ty imports    ..
 00000090: 2020 2020 696d 706f 7274 2070 616e 6461      import panda
 000000a0: 7320 6173 2070 640d 0a20 2020 200d 0a20  s as pd..    .. 
 000000b0: 2020 2023 2049 6e74 6572 6e61 6c20 696d     # Internal im
 000000c0: 706f 7274 730d 0a20 2020 2066 726f 6d20  ports..    from 
 000000d0: 4354 475f 5574 696c 732e 4354 475f 4675  CTG_Utils.CTG_Fu
 000000e0: 6e63 2e43 5447 5f65 6666 6563 7469 6620  nc.CTG_effectif 
-000000f0: 696d 706f 7274 2063 6f72 7265 6374 696f  import correctio
-00000100: 6e5f 6566 6665 6374 6966 0d0a 2020 2020  n_effectif..    
-00000110: 6672 6f6d 2043 5447 5f55 7469 6c73 2e43  from CTG_Utils.C
-00000120: 5447 5f46 756e 632e 4354 475f 6566 6665  TG_Func.CTG_effe
-00000130: 6374 6966 2069 6d70 6f72 7420 7265 6164  ctif import read
-00000140: 5f65 6666 6563 7469 665f 636f 7272 6563  _effectif_correc
-00000150: 7465 640d 0a20 2020 200d 0a0d 0a20 2020  ted..    ....   
-00000160: 200d 0a20 2020 200d 0a20 2020 2070 6174   ..    ..    pat
-00000170: 685f 6469 725f 6c69 7374 203d 205b 6374  h_dir_list = [ct
-00000180: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
-00000190: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
-000001a0: 2753 4f52 5449 4553 2044 5520 5341 4d45  'SORTIES DU SAME
-000001b0: 4449 2729 202f 2050 6174 6828 2745 5843  DI') / Path('EXC
-000001c0: 454c 2729 2c0d 0a20 2020 2020 2020 2020  EL'),..         
-000001d0: 2020 2020 2020 2020 2020 2020 6374 675f              ctg_
-000001e0: 7061 7468 202f 2050 6174 6828 7374 7228  path / Path(str(
-000001f0: 7965 6172 2929 202f 2050 6174 6828 2753  year)) / Path('S
-00000200: 4f52 5449 4553 2044 5520 4449 4d41 4e43  ORTIES DU DIMANC
-00000210: 4845 2729 202f 2050 6174 6828 2745 5843  HE') / Path('EXC
-00000220: 454c 2729 2c0d 0a20 2020 2020 2020 2020  EL'),..         
-00000230: 2020 2020 2020 2020 2020 2020 6374 675f              ctg_
-00000240: 7061 7468 202f 2050 6174 6828 7374 7228  path / Path(str(
-00000250: 7965 6172 2929 202f 2050 6174 6828 2753  year)) / Path('S
-00000260: 4f52 5449 4553 2044 5520 4a45 5544 4927  ORTIES DU JEUDI'
-00000270: 2920 2f20 5061 7468 2827 4558 4345 4c27  ) / Path('EXCEL'
-00000280: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00000290: 2020 2020 2020 2020 2063 7467 5f70 6174           ctg_pat
-000002a0: 6820 2f20 5061 7468 2873 7472 2879 6561  h / Path(str(yea
-000002b0: 7229 2920 2f20 5061 7468 2827 534f 5254  r)) / Path('SORT
-000002c0: 4945 5320 4849 5645 5227 2920 2f20 5061  IES HIVER') / Pa
-000002d0: 7468 2827 4558 4345 4c27 292c 0d0a 2020  th('EXCEL'),..  
-000002e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002f0: 2020 2063 7467 5f70 6174 6820 2f20 5061     ctg_path / Pa
-00000300: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
-00000310: 5061 7468 2827 534f 5254 4945 5320 4455  Path('SORTIES DU
-00000320: 204c 554e 4449 2729 2f20 5061 7468 2827   LUNDI')/ Path('
-00000330: 4558 4345 4c27 292c 0d0a 2020 2020 2020  EXCEL'),..      
-00000340: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000350: 7467 5f70 6174 6820 2f20 5061 7468 2873  tg_path / Path(s
-00000360: 7472 2879 6561 7229 2920 2f20 5061 7468  tr(year)) / Path
-00000370: 2827 5345 4a4f 5552 2729 202f 2050 6174  ('SEJOUR') / Pat
-00000380: 6828 2745 5843 454c 2729 5d0d 0a0d 0a20  h('EXCEL')].... 
-00000390: 2020 206c 6973 745f 6466 203d 205b 5d0d     list_df = [].
-000003a0: 0a20 2020 2066 6f72 2070 6174 685f 6469  .    for path_di
-000003b0: 7220 696e 2070 6174 685f 6469 725f 6c69  r in path_dir_li
-000003c0: 7374 3a0d 0a20 2020 2020 2020 2069 6620  st:..        if 
-000003d0: 6f73 2e70 6174 682e 6973 6469 7228 7061  os.path.isdir(pa
-000003e0: 7468 5f64 6972 293a 0d0a 2020 2020 2020  th_dir):..      
-000003f0: 2020 2020 2020 6669 6c65 7320 3d20 5b78        files = [x
-00000400: 2066 6f72 2078 2069 6e20 6f73 2e6c 6973   for x in os.lis
-00000410: 7464 6972 2870 6174 685f 6469 7229 2069  tdir(path_dir) i
-00000420: 6620 782e 656e 6473 7769 7468 2827 2e78  f x.endswith('.x
-00000430: 6c73 7827 2920 616e 6420 227e 2422 206e  lsx') and "~$" n
-00000440: 6f74 2069 6e20 785d 200d 0a20 2020 2020  ot in x] ..     
-00000450: 2020 2020 2020 206c 6973 745f 6466 2e65         list_df.e
-00000460: 7874 656e 6428 5b70 642e 7265 6164 5f65  xtend([pd.read_e
-00000470: 7863 656c 2870 6174 685f 6469 7220 2f20  xcel(path_dir / 
-00000480: 5061 7468 2866 696c 6529 2c20 656e 6769  Path(file), engi
-00000490: 6e65 3d27 6f70 656e 7079 786c 2729 2066  ne='openpyxl') f
-000004a0: 6f72 2066 696c 6520 696e 2066 696c 6573  or file in files
-000004b0: 5d29 0d0a 2020 2020 0d0a 2020 2020 6466  ])..    ..    df
-000004c0: 5f74 6f74 616c 203d 2070 642e 636f 6e63  _total = pd.conc
-000004d0: 6174 286c 6973 745f 6466 2c20 6967 6e6f  at(list_df, igno
-000004e0: 7265 5f69 6e64 6578 3d54 7275 6529 0d0a  re_index=True)..
-000004f0: 2020 2020 0d0a 2020 2020 6c69 7374 5f6e      ..    list_n
-00000500: 6f6e 5f6c 6963 656e 6369 652c 2064 6963  on_licencie, dic
-00000510: 5f63 6f72 7265 6374 696f 6e5f 6c69 6365  _correction_lice
-00000520: 6e63 652c 2064 6963 5f70 6172 745f 636c  nce, dic_part_cl
-00000530: 7562 203d 2063 6f72 7265 6374 696f 6e5f  ub = correction_
-00000540: 6566 6665 6374 6966 2879 6561 722c 6374  effectif(year,ct
-00000550: 675f 7061 7468 290d 0a20 2020 2064 665f  g_path)..    df_
-00000560: 6566 6665 6374 6966 203d 2072 6561 645f  effectif = read_
-00000570: 6566 6665 6374 6966 5f63 6f72 7265 6374  effectif_correct
-00000580: 6564 2864 6963 5f63 6f72 7265 6374 696f  ed(dic_correctio
-00000590: 6e5f 6c69 6365 6e63 652c 0d0a 2020 2020  n_licence,..    
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005c0: 2020 2020 2020 6c69 7374 5f6e 6f6e 5f6c        list_non_l
-000005d0: 6963 656e 6369 652c 0d0a 2020 2020 2020  icencie,..      
-000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000600: 2020 2020 6469 635f 7061 7274 5f63 6c75      dic_part_clu
-00000610: 622c 0d0a 2020 2020 2020 2020 2020 2020  b,..            
-00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000630: 2020 2020 2020 2020 2020 2020 2020 6374                ct
-00000640: 675f 7061 7468 290d 0a20 2020 200d 0a20  g_path)..    .. 
-00000650: 2020 2064 665f 746f 7461 6c5b 2750 7261     df_total['Pra
-00000660: 7469 7175 6520 5641 4527 5d2e 6669 6c6c  tique VAE'].fill
-00000670: 6e61 2827 4e6f 6e27 2c69 6e70 6c61 6365  na('Non',inplace
-00000680: 3d54 7275 6529 0d0a 2020 2020 0d0a 2020  =True)..    ..  
-00000690: 2020 2320 6e6f 6d62 7265 206d 6f79 656e    # nombre moyen
-000006a0: 2064 6520 7061 7274 6963 6970 616e 7420   de participant 
-000006b0: 7061 7220 6163 7469 7669 74c3 a90d 0a20  par activit.... 
-000006c0: 2020 2066 6f72 2078 2069 6e20 6466 5f74     for x in df_t
-000006d0: 6f74 616c 2e67 726f 7570 6279 285b 2754  otal.groupby(['T
-000006e0: 7970 6527 5d29 3a0d 0a20 2020 2020 2020  ype']):..       
-000006f0: 2070 7269 6e74 2878 5b30 5d2c 6c65 6e28   print(x[0],len(
-00000700: 785b 315d 292c 6c65 6e28 7365 7428 785b  x[1]),len(set(x[
-00000710: 315d 5b27 7365 6a6f 7572 275d 2929 2c6c  1]['sejour'])),l
-00000720: 656e 2878 5b31 5d29 2f6c 656e 2873 6574  en(x[1])/len(set
-00000730: 2878 5b31 5d5b 2773 656a 6f75 7227 5d29  (x[1]['sejour'])
-00000740: 2929 0d0a 2020 2020 0d0a 2020 2020 6669  ))..    ..    fi
-00000750: 6c65 203d 2063 7467 5f70 6174 6820 2f20  le = ctg_path / 
-00000760: 5061 7468 2873 7472 2879 6561 7229 2920  Path(str(year)) 
-00000770: 2f20 5061 7468 2827 5354 4154 4953 5449  / Path('STATISTI
-00000780: 5155 4553 2729 202f 2050 6174 6828 2773  QUES') / Path('s
-00000790: 796e 7468 6573 652e 786c 7378 2729 0d0a  ynthese.xlsx')..
-000007a0: 2020 2020 6466 5f74 6f74 616c 2e74 6f5f      df_total.to_
-000007b0: 6578 6365 6c28 6669 6c65 290d 0a0d 0a64  excel(file)....d
-000007c0: 6566 2070 6c6f 745f 7069 655f 7379 6e74  ef plot_pie_synt
-000007d0: 6865 7365 2879 6561 722c 6374 675f 7061  hese(year,ctg_pa
-000007e0: 7468 293a 0d0a 2020 2020 0d0a 2020 2020  th):..    ..    
-000007f0: 2320 5374 616e 6461 7264 206c 6962 7261  # Standard libra
-00000800: 7279 2069 6d70 6f72 7473 0d0a 2020 2020  ry imports..    
-00000810: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
-00000820: 6f72 7420 5061 7468 0d0a 2020 2020 0d0a  ort Path..    ..
-00000830: 2020 2020 2320 5468 6972 6420 7061 7274      # Third part
-00000840: 7920 696d 706f 7274 730d 0a20 2020 2069  y imports..    i
-00000850: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-00000860: 700d 0a20 2020 2069 6d70 6f72 7420 6d61  p..    import ma
-00000870: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
-00000880: 6173 2070 6c74 0d0a 2020 2020 696d 706f  as plt..    impo
-00000890: 7274 2070 616e 6461 7320 6173 2070 640d  rt pandas as pd.
-000008a0: 0a20 2020 200d 0a20 2020 2064 6566 2066  .    ..    def f
-000008b0: 756e 6328 7063 742c 2061 6c6c 7661 6c75  unc(pct, allvalu
-000008c0: 6573 293a 0d0a 2020 2020 2020 2020 6162  es):..        ab
-000008d0: 736f 6c75 7465 203d 2072 6f75 6e64 2870  solute = round(p
-000008e0: 6374 202f 2031 3030 2e2a 6e70 2e73 756d  ct / 100.*np.sum
-000008f0: 2861 6c6c 7661 6c75 6573 292c 3029 0d0a  (allvalues),0)..
-00000900: 2020 2020 2020 2020 2372 6574 7572 6e20          #return 
-00000910: 227b 3a2e 3166 7d25 5c6e 287b 3a64 7d29  "{:.1f}%\n({:d})
-00000920: 222e 666f 726d 6174 2870 6374 2c20 6162  ".format(pct, ab
-00000930: 736f 6c75 7465 290d 0a20 2020 2020 2020  solute)..       
-00000940: 2072 6574 7572 6e20 2066 227b 696e 7428   return  f"{int(
-00000950: 726f 756e 6428 6162 736f 6c75 7465 2c31  round(absolute,1
-00000960: 2929 7d5c 6e7b 726f 756e 6428 7063 742c  ))}\n{round(pct,
-00000970: 3129 7d20 2522 0d0a 2020 2020 2020 2020  1)} %"..        
-00000980: 0d0a 2020 2020 6669 6c65 5f69 6e20 3d20  ..    file_in = 
-00000990: 6374 675f 7061 7468 202f 2050 6174 6828  ctg_path / Path(
-000009a0: 7374 7228 7965 6172 2929 202f 2050 6174  str(year)) / Pat
-000009b0: 6828 2753 5441 5449 5354 4951 5545 5327  h('STATISTIQUES'
-000009c0: 2920 2f20 5061 7468 2827 7379 6e74 6865  ) / Path('synthe
-000009d0: 7365 2e78 6c73 7827 290d 0a20 2020 2064  se.xlsx')..    d
-000009e0: 665f 746f 7461 6c20 3d20 7064 2e72 6561  f_total = pd.rea
-000009f0: 645f 6578 6365 6c28 6669 6c65 5f69 6e29  d_excel(file_in)
-00000a00: 0d0a 2020 2020 6466 5f74 6f74 616c 203d  ..    df_total =
-00000a10: 2064 665f 746f 7461 6c2e 6472 6f70 6e61   df_total.dropna
-00000a20: 2873 7562 7365 743d 5b27 5479 7065 275d  (subset=['Type']
-00000a30: 2920 0d0a 2020 2020 6466 5f74 6f74 616c  ) ..    df_total
-00000a40: 203d 2064 665f 746f 7461 6c2e 6472 6f70   = df_total.drop
-00000a50: 6e61 2873 7562 7365 743d 5b27 4e6f 6d27  na(subset=['Nom'
-00000a60: 5d29 0d0a 0d0a 2020 2020 6461 6767 203d  ])....    dagg =
-00000a70: 2064 665f 746f 7461 6c2e 6772 6f75 7062   df_total.groupb
-00000a80: 7928 2754 7970 6527 295b 276e 6272 5f6a  y('Type')['nbr_j
-00000a90: 6f75 7273 275d 2e61 6767 2873 756d 290d  ours'].agg(sum).
-00000aa0: 0a0d 0a20 2020 200d 0a20 2020 200d 0a20  ...    ..    .. 
-00000ab0: 2020 2065 7870 6c6f 6465 5f64 6963 203d     explode_dic =
-00000ac0: 207b 2752 414e 444f 4e4e 4545 273a 302e   {'RANDONNEE':0.
-00000ad0: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
-00000ae0: 2020 2020 2020 2027 5345 4a4f 5552 273a         'SEJOUR':
-00000af0: 302e 302c 200d 0a20 2020 2020 2020 2020  0.0, ..         
-00000b00: 2020 2020 2020 2020 2020 2753 4f52 5449            'SORTI
-00000b10: 4553 2044 5520 4449 4d41 4e43 4845 273a  ES DU DIMANCHE':
-00000b20: 302e 322c 0d0a 2020 2020 2020 2020 2020  0.2,..          
-00000b30: 2020 2020 2020 2020 2027 534f 5254 4945           'SORTIE
-00000b40: 5320 4455 204a 4555 4449 273a 302e 322c  S DU JEUDI':0.2,
-00000b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000b60: 2020 2020 2027 534f 5254 4945 5320 4455       'SORTIES DU
-00000b70: 204c 554e 4449 273a 302e 322c 200d 0a20   LUNDI':0.2, .. 
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 2020 2753 4f52 5449 4553 2044 5520 5341    'SORTIES DU SA
-00000ba0: 4d45 4449 273a 302e 322c 0d0a 2020 2020  MEDI':0.2,..    
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000bc0: 534f 5254 4945 5320 4849 5645 5227 3a30  SORTIES HIVER':0
-00000bd0: 2e32 7d0d 0a0d 0a20 2020 2064 6174 6120  .2}....    data 
-00000be0: 3d20 5b5d 0d0a 2020 2020 736f 7274 6965  = []..    sortie
-00000bf0: 7320 3d20 5b5d 0d0a 2020 2020 666f 7220  s = []..    for 
-00000c00: 7479 7065 5f73 656a 6f75 722c 206e 6272  type_sejour, nbr
-00000c10: 2069 6e20 7a69 7028 6461 6767 2e69 6e64   in zip(dagg.ind
-00000c20: 6578 2c64 6167 672e 746f 6c69 7374 2829  ex,dagg.tolist()
-00000c30: 293a 0d0a 2020 2020 2020 2020 6966 206e  ):..        if n
-00000c40: 6272 213d 303a 0d0a 2020 2020 2020 2020  br!=0:..        
-00000c50: 2020 2020 6461 7461 2e61 7070 656e 6428      data.append(
-00000c60: 6e62 7229 0d0a 2020 2020 2020 2020 2020  nbr)..          
-00000c70: 2020 736f 7274 6965 732e 6170 7065 6e64    sorties.append
-00000c80: 2874 7970 655f 7365 6a6f 7572 290d 0a0d  (type_sejour)...
-00000c90: 0a20 2020 2065 7870 6c6f 6465 203d 205b  .    explode = [
-00000ca0: 6578 706c 6f64 655f 6469 635b 7479 705d  explode_dic[typ]
-00000cb0: 2066 6f72 2074 7970 2069 6e20 736f 7274   for typ in sort
-00000cc0: 6965 735d 0d0a 2020 2020 0d0a 2020 2020  ies]..    ..    
-00000cd0: 0d0a 2020 2020 2320 4372 6561 7469 6e67  ..    # Creating
-00000ce0: 2070 6c6f 740d 0a20 2020 2066 6967 203d   plot..    fig =
-00000cf0: 2070 6c74 2e66 6967 7572 6528 6669 6773   plt.figure(figs
-00000d00: 697a 6520 3d28 3130 2c20 3729 290d 0a20  ize =(10, 7)).. 
-00000d10: 2020 205f 2c20 5f2c 2061 7574 6f74 6578     _, _, autotex
-00000d20: 7473 203d 2070 6c74 2e70 6965 2864 6174  ts = plt.pie(dat
-00000d30: 612c 0d0a 2020 2020 2020 2020 2020 2020  a,..            
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 2020 6c61 6265 6c73 203d 2073 6f72 7469    labels = sorti
-00000d60: 6573 2c0d 0a20 2020 2020 2020 2020 2020  es,..           
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2061 7574 6f70 6374 203d 206c 616d     autopct = lam
-00000d90: 6264 6120 7063 743a 2066 756e 6328 7063  bda pct: func(pc
-00000da0: 742c 2064 6174 6129 2c0d 0a20 2020 2020  t, data),..     
-00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dc0: 2020 2020 2020 2020 2065 7870 6c6f 6465           explode
-00000dd0: 203d 2065 7870 6c6f 6465 2c0d 0a20 2020   = explode,..   
-00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000df0: 2020 2020 2020 2020 2020 2074 6578 7470             textp
-00000e00: 726f 7073 3d7b 2766 6f6e 7473 697a 6527  rops={'fontsize'
-00000e10: 3a20 3138 7d29 0d0a 2020 2020 706c 742e  : 18})..    plt.
-00000e20: 7469 746c 6528 7374 7228 7965 6172 292c  title(str(year),
-00000e30: 2070 6164 3d35 302c 2066 6f6e 7473 697a   pad=50, fontsiz
-00000e40: 653d 3230 290d 0a20 2020 200d 0a20 2020  e=20)..    ..   
-00000e50: 205f 203d 2070 6c74 2e73 6574 7028 6175   _ = plt.setp(au
-00000e60: 746f 7465 7874 732c 202a 2a7b 2763 6f6c  totexts, **{'col
-00000e70: 6f72 273a 276b 272c 2027 7765 6967 6874  or':'k', 'weight
-00000e80: 273a 2762 6f6c 6427 2c20 2766 6f6e 7473  ':'bold', 'fonts
-00000e90: 697a 6527 3a31 347d 290d 0a20 2020 200d  ize':14})..    .
-00000ea0: 0a20 2020 2070 6c74 2e74 6967 6874 5f6c  .    plt.tight_l
-00000eb0: 6179 6f75 7428 290d 0a20 2020 2070 6c74  ayout()..    plt
-00000ec0: 2e73 686f 7728 290d 0a20 2020 200d 0a20  .show()..    .. 
-00000ed0: 2020 2066 6967 5f66 696c 6520 3d20 2753     fig_file = 'S
-00000ee0: 4f52 5449 4553 5f50 4945 2e70 6e67 270d  ORTIES_PIE.png'.
-00000ef0: 0a20 2020 2070 6c74 2e73 6176 6566 6967  .    plt.savefig
-00000f00: 2863 7467 5f70 6174 6820 2f20 5061 7468  (ctg_path / Path
-00000f10: 2873 7472 2879 6561 7229 2920 2f20 5061  (str(year)) / Pa
-00000f20: 7468 2827 5354 4154 4953 5449 5155 4553  th('STATISTIQUES
-00000f30: 2729 202f 2050 6174 6828 6669 675f 6669  ') / Path(fig_fi
-00000f40: 6c65 292c 6262 6f78 5f69 6e63 6865 733d  le),bbox_inches=
-00000f50: 2774 6967 6874 2729 090d 0a0d 0a20 2020  'tight').....   
-00000f60: 2072 6574 7572 6e20 090d 0a09 0d0a 0d0a   return ........
-00000f70: 6465 6620 7379 6e74 6865 7365 5f61 6468  def synthese_adh
-00000f80: 6572 656e 7428 7965 6172 2c63 7467 5f70  erent(year,ctg_p
-00000f90: 6174 6829 3a0d 0a0d 0a20 2020 2023 2053  ath):....    # S
-00000fa0: 7461 6e64 6172 6420 6c69 6272 6172 7920  tandard library 
-00000fb0: 696d 706f 7274 730d 0a20 2020 2066 726f  imports..    fro
-00000fc0: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
-00000fd0: 2050 6174 680d 0a20 2020 200d 0a20 2020   Path..    ..   
-00000fe0: 2023 2054 6869 7264 2070 6172 7479 2069   # Third party i
-00000ff0: 6d70 6f72 7473 0d0a 2020 2020 696d 706f  mports..    impo
-00001000: 7274 2070 616e 6461 7320 6173 2070 640d  rt pandas as pd.
-00001010: 0a20 2020 200d 0a20 2020 2023 2049 6e74  .    ..    # Int
-00001020: 6572 6e61 6c20 696d 706f 7274 730d 0a20  ernal imports.. 
-00001030: 2020 2066 726f 6d20 4354 475f 5574 696c     from CTG_Util
-00001040: 732e 4354 475f 4675 6e63 2e43 5447 436c  s.CTG_Func.CTGCl
-00001050: 6173 7365 7320 696d 706f 7274 2045 6666  asses import Eff
-00001060: 6563 7469 6643 7467 0d0a 2020 2020 0d0a  ectifCtg..    ..
-00001070: 2020 2020 6669 6c65 5f69 6e20 3d20 6374      file_in = ct
-00001080: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
-00001090: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
-000010a0: 2753 5441 5449 5354 4951 5545 5327 2920  'STATISTIQUES') 
-000010b0: 2f20 5061 7468 2827 7379 6e74 6865 7365  / Path('synthese
-000010c0: 2e78 6c73 7827 290d 0a20 2020 2064 665f  .xlsx')..    df_
-000010d0: 746f 7461 6c20 3d20 7064 2e72 6561 645f  total = pd.read_
-000010e0: 6578 6365 6c28 6669 6c65 5f69 6e29 0d0a  excel(file_in)..
-000010f0: 2020 2020 6466 5f74 6f74 616c 203d 2064      df_total = d
-00001100: 665f 746f 7461 6c2e 6472 6f70 6e61 2873  f_total.dropna(s
-00001110: 7562 7365 743d 5b27 5479 7065 275d 290d  ubset=['Type']).
-00001120: 0a20 2020 206e 6272 6520 3d20 7b7d 0d0a  .    nbre = {}..
-00001130: 2020 2020 0d0a 2020 2020 666f 7220 6964      ..    for id
-00001140: 5f6c 6963 656e 6365 2c20 6467 2069 6e20  _licence, dg in 
-00001150: 6466 5f74 6f74 616c 2e67 726f 7570 6279  df_total.groupby
-00001160: 2827 4ec2 b020 4c69 6365 6e63 69c3 a927  ('N.. Licenci..'
-00001170: 293a 0d0a 2020 2020 2020 2020 0d0a 2020  ):..        ..  
-00001180: 2020 2020 2020 6e62 7265 5b69 645f 6c69        nbre[id_li
-00001190: 6365 6e63 655d 3d5b 6467 5b27 4e6f 6d27  cence]=[dg['Nom'
-000011a0: 5d2e 756e 6971 7565 2829 5b30 5d2c 6467  ].unique()[0],dg
-000011b0: 5b27 5072 c3a9 6e6f 6d27 5d2e 756e 6971  ['Pr..nom'].uniq
-000011c0: 7565 2829 5b30 5d5d 0d0a 2020 2020 0d0a  ue()[0]]..    ..
-000011d0: 2020 2020 2020 2020 6e62 5f73 6f72 7469          nb_sorti
-000011e0: 655f 6469 6d61 6e63 6865 203d 206c 656e  e_dimanche = len
-000011f0: 2864 672e 7175 6572 7928 2254 7970 652e  (dg.query("Type.
-00001200: 7374 722e 636f 6e74 6169 6e73 2827 534f  str.contains('SO
-00001210: 5254 4945 5320 4455 2044 494d 414e 4348  RTIES DU DIMANCH
-00001220: 4527 2922 2929 0d0a 2020 2020 2020 2020  E')"))..        
-00001230: 6e62 7265 5b69 645f 6c69 6365 6e63 655d  nbre[id_licence]
-00001240: 203d 206e 6272 655b 6964 5f6c 6963 656e   = nbre[id_licen
-00001250: 6365 5d20 2b20 5b6e 625f 736f 7274 6965  ce] + [nb_sortie
-00001260: 5f64 696d 616e 6368 655d 0d0a 2020 2020  _dimanche]..    
-00001270: 0d0a 2020 2020 2020 2020 6e62 5f73 6f72  ..        nb_sor
-00001280: 7469 655f 7361 6d65 6469 203d 206c 656e  tie_samedi = len
-00001290: 2864 672e 7175 6572 7928 2254 7970 652e  (dg.query("Type.
-000012a0: 7374 722e 636f 6e74 6169 6e73 2827 534f  str.contains('SO
-000012b0: 5254 4945 5320 4455 2053 414d 4544 4927  RTIES DU SAMEDI'
-000012c0: 2922 2929 0d0a 2020 2020 2020 2020 6e62  )"))..        nb
-000012d0: 7265 5b69 645f 6c69 6365 6e63 655d 203d  re[id_licence] =
-000012e0: 206e 6272 655b 6964 5f6c 6963 656e 6365   nbre[id_licence
-000012f0: 5d20 2b20 5b6e 625f 736f 7274 6965 5f73  ] + [nb_sortie_s
-00001300: 616d 6564 695d 0d0a 2020 2020 0d0a 2020  amedi]..    ..  
-00001310: 2020 2020 2020 6e62 5f73 6f72 7469 655f        nb_sortie_
-00001320: 6a65 7564 6920 3d20 6c65 6e28 6467 2e71  jeudi = len(dg.q
-00001330: 7565 7279 2822 5479 7065 2e73 7472 2e63  uery("Type.str.c
-00001340: 6f6e 7461 696e 7328 2753 4f52 5449 4553  ontains('SORTIES
-00001350: 2044 5520 4a45 5544 4927 2922 2929 0d0a   DU JEUDI')"))..
-00001360: 2020 2020 2020 2020 6e62 7265 5b69 645f          nbre[id_
-00001370: 6c69 6365 6e63 655d 203d 206e 6272 655b  licence] = nbre[
-00001380: 6964 5f6c 6963 656e 6365 5d20 2b20 5b6e  id_licence] + [n
-00001390: 625f 736f 7274 6965 5f6a 6575 6469 5d0d  b_sortie_jeudi].
-000013a0: 0a20 2020 200d 0a20 2020 2020 2020 206e  .    ..        n
-000013b0: 625f 7261 6e64 6f20 3d20 6c65 6e28 6467  b_rando = len(dg
-000013c0: 2e71 7565 7279 2822 5479 7065 2e73 7472  .query("Type.str
-000013d0: 2e63 6f6e 7461 696e 7328 2752 414e 444f  .contains('RANDO
-000013e0: 4e4e 4545 2729 2229 290d 0a20 2020 2020  NNEE')"))..     
-000013f0: 2020 206e 6272 655b 6964 5f6c 6963 656e     nbre[id_licen
-00001400: 6365 5d20 3d20 6e62 7265 5b69 645f 6c69  ce] = nbre[id_li
-00001410: 6365 6e63 655d 202b 205b 6e62 5f72 616e  cence] + [nb_ran
-00001420: 646f 5d0d 0a20 2020 200d 0a20 2020 2020  do]..    ..     
-00001430: 2020 206e 625f 7365 6a6f 7572 5f6a 6f75     nb_sejour_jou
-00001440: 7273 203d 2073 756d 2864 672e 7175 6572  rs = sum(dg.quer
-00001450: 7928 2254 7970 652e 7374 722e 636f 6e74  y("Type.str.cont
-00001460: 6169 6e73 2827 5345 4a4f 5552 2729 2229  ains('SEJOUR')")
-00001470: 5b27 6e62 725f 6a6f 7572 7327 5d2e 746f  ['nbr_jours'].to
-00001480: 6c69 7374 2829 290d 0a20 2020 2020 2020  list())..       
-00001490: 206e 6272 655b 6964 5f6c 6963 656e 6365   nbre[id_licence
-000014a0: 5d20 3d20 6e62 7265 5b69 645f 6c69 6365  ] = nbre[id_lice
-000014b0: 6e63 655d 202b 205b 6e62 5f73 656a 6f75  nce] + [nb_sejou
-000014c0: 725f 6a6f 7572 735d 0d0a 0d0a 2020 2020  r_jours]....    
-000014d0: 2020 2020 6e62 5f73 656a 6f75 7220 3d20      nb_sejour = 
-000014e0: 6c65 6e28 6467 2e71 7565 7279 2822 5479  len(dg.query("Ty
-000014f0: 7065 2e73 7472 2e63 6f6e 7461 696e 7328  pe.str.contains(
-00001500: 2753 454a 4f55 5227 2922 295b 2773 656a  'SEJOUR')")['sej
-00001510: 6f75 7227 5d2e 756e 6971 7565 2829 290d  our'].unique()).
-00001520: 0a20 2020 2020 2020 206e 6272 655b 6964  .        nbre[id
-00001530: 5f6c 6963 656e 6365 5d20 3d20 6e62 7265  _licence] = nbre
-00001540: 5b69 645f 6c69 6365 6e63 655d 202b 205b  [id_licence] + [
-00001550: 6e62 5f73 656a 6f75 725d 0d0a 2020 2020  nb_sejour]..    
-00001560: 0d0a 2020 2020 2020 2020 6e62 5f68 6976  ..        nb_hiv
-00001570: 6572 203d 206c 656e 2864 672e 7175 6572  er = len(dg.quer
-00001580: 7928 2254 7970 652e 7374 722e 636f 6e74  y("Type.str.cont
-00001590: 6169 6e73 2827 534f 5254 4945 5320 4849  ains('SORTIES HI
-000015a0: 5645 5227 2922 2929 0d0a 2020 2020 2020  VER')"))..      
-000015b0: 2020 6e62 7265 5b69 645f 6c69 6365 6e63    nbre[id_licenc
-000015c0: 655d 203d 206e 6272 655b 6964 5f6c 6963  e] = nbre[id_lic
-000015d0: 656e 6365 5d20 2b20 5b6e 625f 6869 7665  ence] + [nb_hive
-000015e0: 725d 0d0a 2020 2020 0d0a 2020 2020 2020  r]..    ..      
-000015f0: 2020 6e62 725f 6576 656e 656d 656e 7473    nbr_evenements
-00001600: 203d 205b 6e62 5f73 6f72 7469 655f 6469   = [nb_sortie_di
-00001610: 6d61 6e63 6865 202b 0d0a 2020 2020 2020  manche +..      
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 6e62 5f73 6f72 7469 655f 7361      nb_sortie_sa
-00001640: 6d65 6469 202b 200d 0a20 2020 2020 2020  medi + ..       
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 206e 625f 736f 7274 6965 5f6a 6575     nb_sortie_jeu
-00001670: 6469 202b 0d0a 2020 2020 2020 2020 2020  di +..          
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 6e62 5f72 616e 646f 202b 0d0a 2020 2020  nb_rando +..    
-000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016b0: 2020 2020 2020 6e62 5f73 656a 6f75 725f        nb_sejour_
-000016c0: 6a6f 7572 7320 2b0d 0a20 2020 2020 2020  jours +..       
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 206e 625f 6869 7665 725d 0d0a 2020     nb_hiver]..  
-000016f0: 2020 2020 2020 6e62 7265 5b69 645f 6c69        nbre[id_li
-00001700: 6365 6e63 655d 203d 206e 6272 655b 6964  cence] = nbre[id
-00001710: 5f6c 6963 656e 6365 5d20 2b20 6e62 725f  _licence] + nbr_
-00001720: 6576 656e 656d 656e 7473 0d0a 2020 2020  evenements..    
-00001730: 0d0a 2020 2020 6467 203d 2070 642e 4461  ..    dg = pd.Da
-00001740: 7461 4672 616d 652e 6672 6f6d 5f64 6963  taFrame.from_dic
-00001750: 7428 6e62 7265 292e 540d 0a20 2020 2064  t(nbre).T..    d
-00001760: 672e 636f 6c75 6d6e 7320 3d20 5b0d 0a20  g.columns = [.. 
-00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001780: 274e 6f6d 272c 0d0a 2020 2020 2020 2020  'Nom',..        
-00001790: 2020 2020 2020 2020 2027 5072 c3a9 6e6f           'Pr..no
-000017a0: 6d27 2c0d 0a20 2020 2020 2020 2020 2020  m',..           
-000017b0: 2020 2020 2020 2753 4f52 5449 4520 4455        'SORTIE DU
-000017c0: 2044 494d 414e 4348 4520 434c 5542 272c   DIMANCHE CLUB',
-000017d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000017e0: 2020 2027 534f 5254 4945 2044 5520 5341     'SORTIE DU SA
-000017f0: 4d45 4449 2043 4c55 4227 2c0d 0a20 2020  MEDI CLUB',..   
-00001800: 2020 2020 2020 2020 2020 2020 2020 2753                'S
-00001810: 4f52 5449 4520 4455 204a 4555 4449 2043  ORTIE DU JEUDI C
-00001820: 4c55 4227 2c0d 0a20 2020 2020 2020 2020  LUB',..         
-00001830: 2020 2020 2020 2020 2752 414e 444f 4e4e          'RANDONN
-00001840: 4545 272c 0d0a 2020 2020 2020 2020 2020  EE',..          
-00001850: 2020 2020 2020 2027 5345 4a4f 5552 2d4a         'SEJOUR-J
-00001860: 4f55 5227 2c0d 0a20 2020 2020 2020 2020  OUR',..         
-00001870: 2020 2020 2020 2020 274e 6272 5f53 454a          'Nbr_SEJ
-00001880: 4f55 5253 272c 0d0a 2020 2020 2020 2020  OURS',..        
-00001890: 2020 2020 2020 2020 2027 534f 5254 4945           'SORTIE
-000018a0: 2048 4956 4552 272c 0d0a 2020 2020 2020   HIVER',..      
-000018b0: 2020 2020 2020 2020 2020 2027 544f 5441             'TOTA
-000018c0: 4c27 2c0d 0a20 2020 2020 2020 2020 2020  L',..           
-000018d0: 2020 2020 2020 5d0d 0a20 2020 200d 0a20        ]..    .. 
-000018e0: 2020 2065 6666 6563 7469 6620 3d20 4566     effectif = Ef
-000018f0: 6665 6374 6966 4374 6728 7965 6172 2c63  fectifCtg(year,c
-00001900: 7467 5f70 6174 6829 0d0a 2020 2020 6466  tg_path)..    df
-00001910: 5f65 6666 6563 7469 6620 3d20 6566 6665  _effectif = effe
-00001920: 6374 6966 2e65 6666 6563 7469 660d 0a20  ctif.effectif.. 
-00001930: 2020 2064 665f 6566 6665 6374 6966 2e69     df_effectif.i
-00001940: 6e64 6578 203d 2064 665f 6566 6665 6374  ndex = df_effect
-00001950: 6966 5b27 4ec2 b020 4c69 6365 6e63 69c3  if['N.. Licenci.
-00001960: a927 5d0d 0a20 2020 206f 7270 6861 6e20  .']..    orphan 
-00001970: 3d20 7365 7428 6466 5f65 6666 6563 7469  = set(df_effecti
-00001980: 662e 696e 6465 7829 202d 2073 6574 2864  f.index) - set(d
-00001990: 672e 696e 6465 7829 0d0a 2020 2020 6466  g.index)..    df
-000019a0: 5f6f 7270 6861 6e20 3d20 6466 5f65 6666  _orphan = df_eff
-000019b0: 6563 7469 662e 6c6f 635b 6c69 7374 286f  ectif.loc[list(o
-000019c0: 7270 6861 6e29 5d5b 5b27 4e6f 6d27 2c27  rphan)][['Nom','
-000019d0: 5072 c3a9 6e6f 6d27 5d5d 0d0a 2020 2020  Pr..nom']]..    
-000019e0: 6466 5f6f 7270 6861 6e5b 5b27 534f 5254  df_orphan[['SORT
-000019f0: 4945 2044 5520 4449 4d41 4e43 4845 2043  IE DU DIMANCHE C
-00001a00: 4c55 4227 2c0d 0a20 2020 2020 2020 2020  LUB',..         
-00001a10: 2020 2020 2020 2753 4f52 5449 4520 4455        'SORTIE DU
-00001a20: 2053 414d 4544 4920 434c 5542 272c 0d0a   SAMEDI CLUB',..
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001a40: 534f 5254 4945 2044 5520 4a45 5544 4920  SORTIE DU JEUDI 
-00001a50: 434c 5542 272c 0d0a 2020 2020 2020 2020  CLUB',..        
-00001a60: 2020 2020 2020 2027 5241 4e44 4f4e 4e45         'RANDONNE
-00001a70: 4527 2c0d 0a20 2020 2020 2020 2020 2020  E',..           
-00001a80: 2020 2020 2753 454a 4f55 522d 4a4f 5552      'SEJOUR-JOUR
-00001a90: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00001aa0: 2020 2027 4e62 725f 5345 4a4f 5552 5327     'Nbr_SEJOURS'
-00001ab0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001ac0: 2020 2753 4f52 5449 4520 4849 5645 5227    'SORTIE HIVER'
-00001ad0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001ae0: 2020 2754 4f54 414c 275d 5d20 3d20 5b30    'TOTAL']] = [0
-00001af0: 2c30 2c30 2c30 2c30 2c30 2c30 2c30 5d0d  ,0,0,0,0,0,0,0].
-00001b00: 0a20 2020 200d 0a20 2020 2064 6720 3d20  .    ..    dg = 
-00001b10: 7064 2e63 6f6e 6361 7428 5b64 672c 2064  pd.concat([dg, d
-00001b20: 665f 6f72 7068 616e 5d2c 2061 7869 733d  f_orphan], axis=
-00001b30: 3029 0d0a 2020 2020 0d0a 2020 2020 6669  0)..    ..    fi
-00001b40: 6c65 5f6f 7574 203d 2063 7467 5f70 6174  le_out = ctg_pat
-00001b50: 6820 2f20 5061 7468 2873 7472 2879 6561  h / Path(str(yea
-00001b60: 7229 2920 2f20 5061 7468 2827 5354 4154  r)) / Path('STAT
-00001b70: 4953 5449 5155 4553 2729 202f 2050 6174  ISTIQUES') / Pat
-00001b80: 6828 2773 796e 7468 6573 655f 6164 6865  h('synthese_adhe
-00001b90: 7265 6e74 2e78 6c73 7827 290d 0a20 2020  rent.xlsx')..   
-00001ba0: 2064 672e 746f 5f65 7863 656c 2866 696c   dg.to_excel(fil
-00001bb0: 655f 6f75 7429 0d0a 2020 2020 0d0a 6465  e_out)..    ..de
-00001bc0: 6620 7379 6e74 6865 7365 5f72 616e 646f  f synthese_rando
-00001bd0: 6e6e 6565 2879 6561 722c 6374 675f 7061  nnee(year,ctg_pa
-00001be0: 7468 293a 0d0a 0d0a 2020 2020 2320 5374  th):....    # St
-00001bf0: 616e 6461 7264 206c 6962 7261 7279 2069  andard library i
-00001c00: 6d70 6f72 7473 0d0a 2020 2020 6672 6f6d  mports..    from
-00001c10: 2070 6174 686c 6962 2069 6d70 6f72 7420   pathlib import 
-00001c20: 5061 7468 0d0a 2020 2020 0d0a 2020 2020  Path..    ..    
-00001c30: 2320 5468 6972 6420 7061 7274 7920 696d  # Third party im
-00001c40: 706f 7274 730d 0a20 2020 2069 6d70 6f72  ports..    impor
-00001c50: 7420 6d61 7470 6c6f 746c 6962 2e70 7970  t matplotlib.pyp
-00001c60: 6c6f 7420 6173 2070 6c74 0d0a 2020 2020  lot as plt..    
-00001c70: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-00001c80: 2070 640d 0a20 2020 200d 0a20 2020 2064   pd..    ..    d
-00001c90: 6566 2061 6464 6c61 6265 6c73 2878 2c79  ef addlabels(x,y
-00001ca0: 2c6f 6666 7365 7429 3a0d 0a20 2020 2020  ,offset):..     
-00001cb0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00001cc0: 6528 6c65 6e28 7829 293a 0d0a 2020 2020  e(len(x)):..    
-00001cd0: 2020 2020 2020 2020 6966 2079 5b69 5d20          if y[i] 
-00001ce0: 213d 2030 3a0d 0a20 2020 2020 2020 2020  != 0:..         
-00001cf0: 2020 2020 2020 2070 6c74 2e74 6578 7428         plt.text(
-00001d00: 785b 695d 2c79 5b69 5d2b 6f66 6673 6574  x[i],y[i]+offset
-00001d10: 2c72 6f75 6e64 2879 5b69 5d2c 3129 2c73  ,round(y[i],1),s
-00001d20: 697a 653d 3130 290d 0a20 2020 2020 2020  ize=10)..       
-00001d30: 200d 0a20 2020 200d 0a20 2020 2066 696c   ..    ..    fil
-00001d40: 655f 696e 203d 2050 6174 6828 6374 675f  e_in = Path(ctg_
-00001d50: 7061 7468 2920 2f20 5061 7468 2873 7472  path) / Path(str
-00001d60: 2879 6561 7229 2920 2f20 5061 7468 2827  (year)) / Path('
-00001d70: 5354 4154 4953 5449 5155 4553 2729 202f  STATISTIQUES') /
-00001d80: 2050 6174 6828 2773 796e 7468 6573 652e   Path('synthese.
-00001d90: 786c 7378 2729 0d0a 2020 2020 6466 5f74  xlsx')..    df_t
-00001da0: 6f74 616c 203d 2070 642e 7265 6164 5f65  otal = pd.read_e
-00001db0: 7863 656c 2866 696c 655f 696e 290d 0a20  xcel(file_in).. 
-00001dc0: 2020 2064 665f 746f 7461 6c20 3d20 6466     df_total = df
-00001dd0: 5f74 6f74 616c 2e64 726f 706e 6128 7375  _total.dropna(su
-00001de0: 6273 6574 3d5b 274e 6f6d 275d 2920 0d0a  bset=['Nom']) ..
-00001df0: 2020 2020 6467 203d 2064 665f 746f 7461      dg = df_tota
-00001e00: 6c2e 7175 6572 7928 2754 7970 653d 3d22  l.query('Type=="
-00001e10: 5241 4e44 4f4e 4e45 4522 2729 2e67 726f  RANDONNEE"').gro
-00001e20: 7570 6279 2827 7365 6a6f 7572 2729 2e61  upby('sejour').a
-00001e30: 6767 2827 636f 756e 7427 295b 274e c2b0  gg('count')['N..
-00001e40: 204c 6963 656e 6369 c3a9 275d 0d0a 2020   Licenci..']..  
-00001e50: 2020 0d0a 2020 2020 6669 6720 3d20 706c    ..    fig = pl
-00001e60: 742e 6669 6775 7265 2829 0d0a 2020 2020  t.figure()..    
-00001e70: 706c 742e 6261 7228 7261 6e67 6528 6c65  plt.bar(range(le
-00001e80: 6e28 6467 2929 2c64 672e 746f 6c69 7374  n(dg)),dg.tolist
-00001e90: 2829 290d 0a20 2020 2061 6464 6c61 6265  ())..    addlabe
-00001ea0: 6c73 286c 6973 7428 7261 6e67 6528 6c65  ls(list(range(le
-00001eb0: 6e28 6467 2929 292c 6467 2e74 6f6c 6973  n(dg))),dg.tolis
-00001ec0: 7428 292c 302e 3229 0d0a 2020 2020 706c  t(),0.2)..    pl
-00001ed0: 742e 7874 6963 6b73 2872 616e 6765 286c  t.xticks(range(l
-00001ee0: 656e 2864 6729 292c 2064 672e 696e 6465  en(dg)), dg.inde
-00001ef0: 782c 2072 6f74 6174 696f 6e3d 2776 6572  x, rotation='ver
-00001f00: 7469 6361 6c27 290d 0a20 2020 2070 6c74  tical')..    plt
-00001f10: 2e74 6963 6b5f 7061 7261 6d73 2861 7869  .tick_params(axi
-00001f20: 733d 2778 272c 2072 6f74 6174 696f 6e3d  s='x', rotation=
-00001f30: 3930 2c20 6c61 6265 6c73 697a 653d 3130  90, labelsize=10
-00001f40: 290d 0a20 2020 2070 6c74 2e74 6963 6b5f  )..    plt.tick_
-00001f50: 7061 7261 6d73 2861 7869 733d 2779 272c  params(axis='y',
-00001f60: 6c61 6265 6c73 697a 653d 3130 290d 0a20  labelsize=10).. 
-00001f70: 2020 200d 0a20 2020 205f 203d 2070 6c74     ..    _ = plt
-00001f80: 2e74 6974 6c65 2866 2723 2072 616e 646f  .title(f'# rando
-00001f90: 7320 3a20 7b6c 656e 2864 6729 7d20 2c20  s : {len(dg)} , 
-00001fa0: 2320 7061 7274 6963 6970 616e 7473 203a  # participants :
-00001fb0: 207b 7375 6d28 6467 297d 2729 0d0a 2020   {sum(dg)}')..  
-00001fc0: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
-00001fd0: 7574 2829 0d0a 2020 2020 706c 742e 7368  ut()..    plt.sh
-00001fe0: 6f77 2829 0d0a 2020 2020 0d0a 2020 2020  ow()..    ..    
-00001ff0: 6669 675f 6669 6c65 203d 2027 5359 4e54  fig_file = 'SYNT
-00002000: 4845 5345 5f52 414e 444f 4e4e 4545 532e  HESE_RANDONNEES.
-00002010: 706e 6727 0d0a 2020 2020 706c 742e 7361  png'..    plt.sa
-00002020: 7665 6669 6728 6374 675f 7061 7468 202f  vefig(ctg_path /
-00002030: 2050 6174 6828 7374 7228 7965 6172 2929   Path(str(year))
-00002040: 202f 2050 6174 6828 2753 5441 5449 5354   / Path('STATIST
-00002050: 4951 5545 5327 2920 2f20 5061 7468 2866  IQUES') / Path(f
-00002060: 6967 5f66 696c 6529 2c62 626f 785f 696e  ig_file),bbox_in
-00002070: 6368 6573 3d27 7469 6768 7427 290d 0a20  ches='tight').. 
-00002080: 2020 200d 0a64 6566 206e 6272 5f73 656a     ..def nbr_sej
-00002090: 6f75 7273 5f61 6468 6572 656e 7428 7965  ours_adherent(ye
-000020a0: 6172 2c20 6374 675f 7061 7468 293a 0d0a  ar, ctg_path):..
-000020b0: 0d0a 2020 2020 2320 5374 616e 6461 7264  ..    # Standard
-000020c0: 206c 6962 7261 7279 2069 6d70 6f72 7473   library imports
-000020d0: 0d0a 2020 2020 6672 6f6d 2063 6f6c 6c65  ..    from colle
-000020e0: 6374 696f 6e73 2069 6d70 6f72 7420 436f  ctions import Co
-000020f0: 756e 7465 720d 0a20 2020 2066 726f 6d20  unter..    from 
-00002100: 7061 7468 6c69 6220 696d 706f 7274 2050  pathlib import P
-00002110: 6174 680d 0a20 2020 200d 0a20 2020 2023  ath..    ..    #
-00002120: 2054 6869 7264 2070 6172 7479 2069 6d70   Third party imp
-00002130: 6f72 7473 0d0a 2020 2020 696d 706f 7274  orts..    import
-00002140: 206d 6174 706c 6f74 6c69 622e 7079 706c   matplotlib.pypl
-00002150: 6f74 2061 7320 706c 740d 0a20 2020 2069  ot as plt..    i
-00002160: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-00002170: 7064 0d0a 2020 2020 0d0a 2020 2020 706c  pd..    ..    pl
-00002180: 742e 7374 796c 652e 7573 6528 2767 6770  t.style.use('ggp
-00002190: 6c6f 7427 290d 0a20 2020 200d 0a20 2020  lot')..    ..   
-000021a0: 2023 2066 756e 6374 696f 6e20 746f 2061   # function to a
-000021b0: 6464 2076 616c 7565 206c 6162 656c 730d  dd value labels.
-000021c0: 0a20 2020 2064 6566 2061 6464 6c61 6265  .    def addlabe
-000021d0: 6c73 2878 2c79 293a 0d0a 2020 2020 2020  ls(x,y):..      
-000021e0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-000021f0: 286c 656e 2878 2929 3a0d 0a20 2020 2020  (len(x)):..     
-00002200: 2020 2020 2020 2070 6c74 2e74 6578 7428         plt.text(
-00002210: 785b 695d 2d30 2e32 2c79 5b69 5d2b 312c  x[i]-0.2,y[i]+1,
-00002220: 795b 695d 2c73 697a 653d 6c61 6265 6c5f  y[i],size=label_
-00002230: 7369 7a65 290d 0a20 2020 206c 6162 656c  size)..    label
-00002240: 5f73 697a 6520 3d20 3135 0d0a 2020 2020  _size = 15..    
-00002250: 6669 6c65 5f69 6e20 3d20 6374 675f 7061  file_in = ctg_pa
-00002260: 7468 202f 2050 6174 6828 7374 7228 7965  th / Path(str(ye
-00002270: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
-00002280: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
-00002290: 7468 2827 7379 6e74 6865 7365 5f61 6468  th('synthese_adh
-000022a0: 6572 656e 742e 786c 7378 2729 0d0a 2020  erent.xlsx')..  
-000022b0: 2020 6466 5f74 6f74 616c 203d 2070 642e    df_total = pd.
-000022c0: 7265 6164 5f65 7863 656c 2866 696c 655f  read_excel(file_
-000022d0: 696e 290d 0a20 2020 200d 0a20 2020 2063  in)..    ..    c
-000022e0: 203d 2043 6f75 6e74 6572 2829 0d0a 2020   = Counter()..  
-000022f0: 2020 6320 3d20 436f 756e 7465 7228 6466    c = Counter(df
-00002300: 5f74 6f74 616c 5b27 4e62 725f 5345 4a4f  _total['Nbr_SEJO
-00002310: 5552 5327 5d2e 746f 6c69 7374 2829 290d  URS'].tolist()).
-00002320: 0a20 2020 2063 203d 2063 2e6d 6f73 745f  .    c = c.most_
-00002330: 636f 6d6d 6f6e 2829 0d0a 0d0a 2020 2020  common()....    
-00002340: 782c 2079 203d 207a 6970 282a 6329 0d0a  x, y = zip(*c)..
-00002350: 2020 2020 7820 3d20 6c69 7374 2878 290d      x = list(x).
-00002360: 0a20 2020 2079 203d 206c 6973 7428 7929  .    y = list(y)
-00002370: 0d0a 2020 2020 0d0a 2020 2020 6669 672c  ..    ..    fig,
-00002380: 2061 7820 3d20 706c 742e 7375 6270 6c6f   ax = plt.subplo
-00002390: 7473 2866 6967 7369 7a65 3d28 352c 3529  ts(figsize=(5,5)
-000023a0: 290d 0a20 2020 2070 6c74 2e62 6172 285b  )..    plt.bar([
-000023b0: 7374 7228 785f 7329 2066 6f72 2078 5f73  str(x_s) for x_s
-000023c0: 2069 6e20 785d 2c79 290d 0a20 2020 2070   in x],y)..    p
-000023d0: 6c74 2e78 6c61 6265 6c28 274e 6f6d 6272  lt.xlabel('Nombr
-000023e0: 6520 6465 2070 6172 7469 6369 7061 7469  e de participati
-000023f0: 6f6e 20c3 a020 6465 7320 73c3 a96a 6f75  on .. des s..jou
-00002400: 7273 2729 0d0a 2020 2020 706c 742e 796c  rs')..    plt.yl
-00002410: 6162 656c 2827 4e6f 6d62 7265 2064 6520  abel('Nombre de 
-00002420: 6c69 6365 6e63 6965 7273 2729 0d0a 2020  licenciers')..  
-00002430: 2020 706c 742e 7469 636b 5f70 6172 616d    plt.tick_param
-00002440: 7328 6178 6973 3d27 7827 2c20 6c61 6265  s(axis='x', labe
-00002450: 6c73 697a 653d 6c61 6265 6c5f 7369 7a65  lsize=label_size
-00002460: 290d 0a20 2020 2070 6c74 2e74 6963 6b5f  )..    plt.tick_
-00002470: 7061 7261 6d73 2861 7869 733d 2779 272c  params(axis='y',
-00002480: 206c 6162 656c 7369 7a65 3d6c 6162 656c   labelsize=label
-00002490: 5f73 697a 6529 0d0a 2020 2020 706c 742e  _size)..    plt.
-000024a0: 7469 746c 6528 7374 7228 7965 6172 292c  title(str(year),
-000024b0: 7061 643d 3230 2c20 666f 6e74 7369 7a65  pad=20, fontsize
-000024c0: 3d32 3029 0d0a 2020 2020 0d0a 2020 2020  =20)..    ..    
-000024d0: 6178 2e73 6574 5f78 6c61 6265 6c28 274e  ax.set_xlabel('N
-000024e0: 2073 c3a9 6a6f 7572 7327 2c20 666f 6e74   s..jours', font
-000024f0: 7369 7a65 203d 206c 6162 656c 5f73 697a  size = label_siz
-00002500: 6529 0d0a 2020 2020 6178 2e73 6574 5f79  e)..    ax.set_y
-00002510: 6c61 6265 6c28 274e 6f6d 6272 6520 6465  label('Nombre de
-00002520: 2043 5447 2061 7961 6e74 205c 6e20 7061   CTG ayant \n pa
-00002530: 7274 6963 6970 c3a9 20c3 a020 4e20 73c3  rticip.. .. N s.
-00002540: a96a 6f75 7273 272c 2066 6f6e 7473 697a  .jours', fontsiz
-00002550: 6520 3d20 6c61 6265 6c5f 7369 7a65 290d  e = label_size).
-00002560: 0a20 2020 200d 0a20 2020 2078 2e73 6f72  .    ..    x.sor
-00002570: 7428 290d 0a20 2020 2061 6464 6c61 6265  t()..    addlabe
-00002580: 6c73 2878 2c79 290d 0a20 2020 2070 6c74  ls(x,y)..    plt
-00002590: 2e74 6967 6874 5f6c 6179 6f75 7428 290d  .tight_layout().
-000025a0: 0a20 2020 2070 6c74 2e73 686f 7728 290d  .    plt.show().
-000025b0: 0a0d 0a20 2020 2066 6967 5f66 696c 6520  ...    fig_file 
-000025c0: 3d20 2753 454a 4f55 5253 5f53 5441 545f  = 'SEJOURS_STAT_
-000025d0: 5041 5254 4943 4950 4154 494f 4e2e 706e  PARTICIPATION.pn
-000025e0: 6727 0d0a 2020 2020 706c 742e 7361 7665  g'..    plt.save
-000025f0: 6669 6728 6374 675f 7061 7468 202f 2050  fig(ctg_path / P
-00002600: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
-00002610: 2050 6174 6828 2753 5441 5449 5354 4951   Path('STATISTIQ
-00002620: 5545 5327 2920 2f20 5061 7468 2866 6967  UES') / Path(fig
-00002630: 5f66 696c 6529 2c62 626f 785f 696e 6368  _file),bbox_inch
-00002640: 6573 3d27 7469 6768 7427 290d 0a20 2020  es='tight')..   
-00002650: 200d 0a64 6566 2072 6561 645f 6d65 6d6f   ..def read_memo
-00002660: 7279 5f73 6f72 7469 6573 2829 3a0d 0a0d  ry_sorties():...
-00002670: 0a20 2020 2023 2053 7461 6e64 6172 6420  .    # Standard 
-00002680: 6c69 6272 6172 7920 696d 706f 7274 730d  library imports.
-00002690: 0a20 2020 2069 6d70 6f72 7420 6f73 2e70  .    import os.p
-000026a0: 6174 680d 0a20 2020 2066 726f 6d20 7061  ath..    from pa
-000026b0: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
-000026c0: 680d 0a0d 0a20 2020 2023 2033 7264 2070  h....    # 3rd p
-000026d0: 6172 7479 2069 6d70 6f72 7473 0d0a 2020  arty imports..  
-000026e0: 2020 696d 706f 7274 2079 616d 6c0d 0a20    import yaml.. 
-000026f0: 2020 200d 0a20 2020 2023 2052 6561 6473     ..    # Reads
-00002700: 2074 6865 2064 6566 6175 6c74 2050 5663   the default PVc
-00002710: 6861 7261 6374 6572 697a 6174 696f 6e2e  haracterization.
-00002720: 7961 6d6c 2063 6f6e 6669 6720 6669 6c65  yaml config file
-00002730: 0d0a 2020 2020 7061 7468 5f63 6f6e 6669  ..    path_confi
-00002740: 675f 6669 6c65 203d 2050 6174 6828 5f5f  g_file = Path(__
-00002750: 6669 6c65 5f5f 292e 7061 7265 6e74 2e70  file__).parent.p
-00002760: 6172 656e 7420 2f20 5061 7468 2827 4354  arent / Path('CT
-00002770: 475f 4675 6e63 2729 202f 2050 6174 6828  G_Func') / Path(
-00002780: 2743 5447 5f52 6566 4669 6c65 7327 2920  'CTG_RefFiles') 
-00002790: 2f20 5061 7468 2827 6d65 6d6f 7279 5f73  / Path('memory_s
-000027a0: 6f72 7469 6573 2e79 6d6c 2729 0d0a 2020  orties.yml')..  
-000027b0: 2020 7769 7468 206f 7065 6e28 7061 7468    with open(path
-000027c0: 5f63 6f6e 6669 675f 6669 6c65 2920 6173  _config_file) as
-000027d0: 2066 696c 653a 0d0a 2020 2020 2020 2020   file:..        
-000027e0: 6d65 6d6f 7279 203d 2079 616d 6c2e 7361  memory = yaml.sa
-000027f0: 6665 5f6c 6f61 6428 6669 6c65 290d 0a20  fe_load(file).. 
-00002800: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002810: 0d0a 2020 2020 7265 7475 726e 206d 656d  ..    return mem
-00002820: 6f72 790d 0a20 2020 200d 0a64 6566 2065  ory..    ..def e
-00002830: 766f 6c75 7469 6f6e 5f73 6f72 7469 6573  volution_sorties
-00002840: 2874 7970 652c 6374 675f 7061 7468 293a  (type,ctg_path):
-00002850: 0d0a 0d0a 2020 2020 2320 5374 616e 6461  ....    # Standa
-00002860: 7264 206c 6962 7261 7279 2069 6d70 6f72  rd library impor
-00002870: 7420 2020 200d 0a20 2020 2069 6d70 6f72  t    ..    impor
-00002880: 7420 6461 7465 7469 6d65 0d0a 2020 2020  t datetime..    
-00002890: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
-000028a0: 6f72 7420 5061 7468 0d0a 2020 2020 6672  ort Path..    fr
-000028b0: 6f6d 2063 6f6c 6c65 6374 696f 6e73 2069  om collections i
-000028c0: 6d70 6f72 7420 6e61 6d65 6474 7570 6c65  mport namedtuple
-000028d0: 0d0a 0d0a 2020 2020 2320 5468 6972 6420  ....    # Third 
-000028e0: 7061 7274 7920 6c69 6272 6172 7920 696d  party library im
-000028f0: 706f 7274 2020 2020 200d 0a20 2020 2069  port     ..    i
-00002900: 6d70 6f72 7420 6d61 7470 6c6f 746c 6962  mport matplotlib
-00002910: 2e70 7970 6c6f 7420 6173 2070 6c74 0d0a  .pyplot as plt..
-00002920: 2020 2020 696d 706f 7274 2070 616e 6461      import panda
-00002930: 7320 6173 2070 640d 0a20 2020 2020 200d  s as pd..      .
-00002940: 0a20 2020 2023 2049 6e74 6572 6e61 6c20  .    # Internal 
-00002950: 696d 706f 7274 0d0a 2020 2020 696d 706f  import..    impo
-00002960: 7274 2043 5447 5f55 7469 6c73 2061 7320  rt CTG_Utils as 
-00002970: 6374 670d 0a20 2020 2066 726f 6d20 4354  ctg..    from CT
-00002980: 475f 5574 696c 732e 4354 475f 4755 492e  G_Utils.CTG_GUI.
-00002990: 4755 495f 476c 6f62 616c 7320 696d 706f  GUI_Globals impo
-000029a0: 7274 2041 4354 4956 4954 455f 4c49 5354  rt ACTIVITE_LIST
-000029b0: 200d 0a20 2020 200d 0a20 2020 2064 6566   ..    ..    def
-000029c0: 2061 6464 5f6d 656d 6f72 7928 7374 6174   add_memory(stat
-000029d0: 5f64 6963 2c79 6561 7273 293a 0d0a 2020  _dic,years):..  
-000029e0: 2020 2020 2020 6d65 6d6f 7279 203d 2072        memory = r
-000029f0: 6561 645f 6d65 6d6f 7279 5f73 6f72 7469  ead_memory_sorti
-00002a00: 6573 2829 0d0a 2020 2020 0d0a 2020 2020  es()..    ..    
-00002a10: 0d0a 2020 2020 2020 2020 666f 7220 7965  ..        for ye
-00002a20: 6172 2c76 2069 6e20 6d65 6d6f 7279 5b27  ar,v in memory['
-00002a30: 6d65 6d6f 7279 275d 2e69 7465 6d73 2829  memory'].items()
-00002a40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00002a70: 2020 2020 2020 2020 2020 2020 7374 6174              stat
-00002a80: 5f64 6963 5b73 7472 2879 6561 7229 5d20  _dic[str(year)] 
-00002a90: 3d20 7374 6174 7965 6172 2876 5b27 5041  = statyear(v['PA
-00002aa0: 5254 4943 4950 4154 494f 4e5f 5345 4a4f  RTICIPATION_SEJO
-00002ab0: 5552 5327 5d2c 2020 2020 2020 2020 2020  URS'],          
-00002ac0: 2020 2020 2020 2320 6e62 725f 7365 6a6f        # nbr_sejo
-00002ad0: 7572 730d 0a20 2020 2020 2020 2020 2020  urs..           
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000000f0: 696d 706f 7274 2072 6561 645f 6566 6665  import read_effe
+00000100: 6374 6966 5f63 6f72 7265 6374 6564 0d0a  ctif_corrected..
+00000110: 2020 2020 0d0a 0d0a 2020 2020 0d0a 2020      ....    ..  
+00000120: 2020 0d0a 2020 2020 7061 7468 5f64 6972    ..    path_dir
+00000130: 5f6c 6973 7420 3d20 5b63 7467 5f70 6174  _list = [ctg_pat
+00000140: 6820 2f20 5061 7468 2873 7472 2879 6561  h / Path(str(yea
+00000150: 7229 2920 2f20 5061 7468 2827 534f 5254  r)) / Path('SORT
+00000160: 4945 5320 4455 2053 414d 4544 4927 2920  IES DU SAMEDI') 
+00000170: 2f20 5061 7468 2827 4558 4345 4c27 292c  / Path('EXCEL'),
+00000180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000190: 2020 2020 2020 2063 7467 5f70 6174 6820         ctg_path 
+000001a0: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
+000001b0: 2920 2f20 5061 7468 2827 534f 5254 4945  ) / Path('SORTIE
+000001c0: 5320 4455 2044 494d 414e 4348 4527 2920  S DU DIMANCHE') 
+000001d0: 2f20 5061 7468 2827 4558 4345 4c27 292c  / Path('EXCEL'),
+000001e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000001f0: 2020 2020 2020 2063 7467 5f70 6174 6820         ctg_path 
+00000200: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
+00000210: 2920 2f20 5061 7468 2827 534f 5254 4945  ) / Path('SORTIE
+00000220: 5320 4455 204a 4555 4449 2729 202f 2050  S DU JEUDI') / P
+00000230: 6174 6828 2745 5843 454c 2729 2c0d 0a20  ath('EXCEL'),.. 
+00000240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000250: 2020 2020 6374 675f 7061 7468 202f 2050      ctg_path / P
+00000260: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
+00000270: 2050 6174 6828 2753 4f52 5449 4553 2048   Path('SORTIES H
+00000280: 4956 4552 2729 202f 2050 6174 6828 2745  IVER') / Path('E
+00000290: 5843 454c 2729 2c0d 0a20 2020 2020 2020  XCEL'),..       
+000002a0: 2020 2020 2020 2020 2020 2020 2020 6374                ct
+000002b0: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
+000002c0: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
+000002d0: 2753 4f52 5449 4553 2044 5520 4c55 4e44  'SORTIES DU LUND
+000002e0: 4927 292f 2050 6174 6828 2745 5843 454c  I')/ Path('EXCEL
+000002f0: 2729 2c0d 0a20 2020 2020 2020 2020 2020  '),..           
+00000300: 2020 2020 2020 2020 2020 6374 675f 7061            ctg_pa
+00000310: 7468 202f 2050 6174 6828 7374 7228 7965  th / Path(str(ye
+00000320: 6172 2929 202f 2050 6174 6828 2753 454a  ar)) / Path('SEJ
+00000330: 4f55 5227 2920 2f20 5061 7468 2827 4558  OUR') / Path('EX
+00000340: 4345 4c27 295d 0d0a 0d0a 2020 2020 6c69  CEL')]....    li
+00000350: 7374 5f64 6620 3d20 5b5d 0d0a 2020 2020  st_df = []..    
+00000360: 666f 7220 7061 7468 5f64 6972 2069 6e20  for path_dir in 
+00000370: 7061 7468 5f64 6972 5f6c 6973 743a 0d0a  path_dir_list:..
+00000380: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+00000390: 7468 2e69 7364 6972 2870 6174 685f 6469  th.isdir(path_di
+000003a0: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
+000003b0: 2066 696c 6573 203d 205b 7820 666f 7220   files = [x for 
+000003c0: 7820 696e 206f 732e 6c69 7374 6469 7228  x in os.listdir(
+000003d0: 7061 7468 5f64 6972 2920 6966 2078 2e65  path_dir) if x.e
+000003e0: 6e64 7377 6974 6828 272e 786c 7378 2729  ndswith('.xlsx')
+000003f0: 2061 6e64 2022 7e24 2220 6e6f 7420 696e   and "~$" not in
+00000400: 2078 5d20 0d0a 2020 2020 2020 2020 2020   x] ..          
+00000410: 2020 6c69 7374 5f64 662e 6578 7465 6e64    list_df.extend
+00000420: 285b 7064 2e72 6561 645f 6578 6365 6c28  ([pd.read_excel(
+00000430: 7061 7468 5f64 6972 202f 2050 6174 6828  path_dir / Path(
+00000440: 6669 6c65 292c 2065 6e67 696e 653d 276f  file), engine='o
+00000450: 7065 6e70 7978 6c27 2920 666f 7220 6669  penpyxl') for fi
+00000460: 6c65 2069 6e20 6669 6c65 735d 290d 0a20  le in files]).. 
+00000470: 2020 200d 0a20 2020 2064 665f 746f 7461     ..    df_tota
+00000480: 6c20 3d20 7064 2e63 6f6e 6361 7428 6c69  l = pd.concat(li
+00000490: 7374 5f64 662c 2069 676e 6f72 655f 696e  st_df, ignore_in
+000004a0: 6465 783d 5472 7565 290d 0a20 2020 200d  dex=True)..    .
+000004b0: 0a20 2020 2064 665f 6566 6665 6374 6966  .    df_effectif
+000004c0: 203d 2072 6561 645f 6566 6665 6374 6966   = read_effectif
+000004d0: 5f63 6f72 7265 6374 6564 2863 7467 5f70  _corrected(ctg_p
+000004e0: 6174 6829 0d0a 2020 2020 0d0a 2020 2020  ath)..    ..    
+000004f0: 6466 5f74 6f74 616c 5b27 5072 6174 6971  df_total['Pratiq
+00000500: 7565 2056 4145 275d 2e66 696c 6c6e 6128  ue VAE'].fillna(
+00000510: 274e 6f6e 272c 696e 706c 6163 653d 5472  'Non',inplace=Tr
+00000520: 7565 290d 0a20 2020 200d 0a20 2020 2023  ue)..    ..    #
+00000530: 206e 6f6d 6272 6520 6d6f 7965 6e20 6465   nombre moyen de
+00000540: 2070 6172 7469 6369 7061 6e74 2070 6172   participant par
+00000550: 2061 6374 6976 6974 c3a9 0d0a 2020 2020   activit....    
+00000560: 666f 7220 7820 696e 2064 665f 746f 7461  for x in df_tota
+00000570: 6c2e 6772 6f75 7062 7928 5b27 5479 7065  l.groupby(['Type
+00000580: 275d 293a 0d0a 2020 2020 2020 2020 7072  ']):..        pr
+00000590: 696e 7428 785b 305d 2c6c 656e 2878 5b31  int(x[0],len(x[1
+000005a0: 5d29 2c6c 656e 2873 6574 2878 5b31 5d5b  ]),len(set(x[1][
+000005b0: 2773 656a 6f75 7227 5d29 292c 6c65 6e28  'sejour'])),len(
+000005c0: 785b 315d 292f 6c65 6e28 7365 7428 785b  x[1])/len(set(x[
+000005d0: 315d 5b27 7365 6a6f 7572 275d 2929 290d  1]['sejour']))).
+000005e0: 0a20 2020 200d 0a20 2020 2066 696c 6520  .    ..    file 
+000005f0: 3d20 6374 675f 7061 7468 202f 2050 6174  = ctg_path / Pat
+00000600: 6828 7374 7228 7965 6172 2929 202f 2050  h(str(year)) / P
+00000610: 6174 6828 2753 5441 5449 5354 4951 5545  ath('STATISTIQUE
+00000620: 5327 2920 2f20 5061 7468 2827 7379 6e74  S') / Path('synt
+00000630: 6865 7365 2e78 6c73 7827 290d 0a20 2020  hese.xlsx')..   
+00000640: 2064 665f 746f 7461 6c2e 746f 5f65 7863   df_total.to_exc
+00000650: 656c 2866 696c 6529 0d0a 0d0a 6465 6620  el(file)....def 
+00000660: 706c 6f74 5f70 6965 5f73 796e 7468 6573  plot_pie_synthes
+00000670: 6528 7965 6172 2c63 7467 5f70 6174 6829  e(year,ctg_path)
+00000680: 3a0d 0a20 2020 200d 0a20 2020 2023 2053  :..    ..    # S
+00000690: 7461 6e64 6172 6420 6c69 6272 6172 7920  tandard library 
+000006a0: 696d 706f 7274 730d 0a20 2020 2066 726f  imports..    fro
+000006b0: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
+000006c0: 2050 6174 680d 0a20 2020 200d 0a20 2020   Path..    ..   
+000006d0: 2023 2054 6869 7264 2070 6172 7479 2069   # Third party i
+000006e0: 6d70 6f72 7473 0d0a 2020 2020 696d 706f  mports..    impo
+000006f0: 7274 206e 756d 7079 2061 7320 6e70 0d0a  rt numpy as np..
+00000700: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
+00000710: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
+00000720: 706c 740d 0a20 2020 2069 6d70 6f72 7420  plt..    import 
+00000730: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
+00000740: 2020 0d0a 2020 2020 6465 6620 6675 6e63    ..    def func
+00000750: 2870 6374 2c20 616c 6c76 616c 7565 7329  (pct, allvalues)
+00000760: 3a0d 0a20 2020 2020 2020 2061 6273 6f6c  :..        absol
+00000770: 7574 6520 3d20 726f 756e 6428 7063 7420  ute = round(pct 
+00000780: 2f20 3130 302e 2a6e 702e 7375 6d28 616c  / 100.*np.sum(al
+00000790: 6c76 616c 7565 7329 2c30 290d 0a20 2020  lvalues),0)..   
+000007a0: 2020 2020 2023 7265 7475 726e 2022 7b3a       #return "{:
+000007b0: 2e31 667d 255c 6e28 7b3a 647d 2922 2e66  .1f}%\n({:d})".f
+000007c0: 6f72 6d61 7428 7063 742c 2061 6273 6f6c  ormat(pct, absol
+000007d0: 7574 6529 0d0a 2020 2020 2020 2020 7265  ute)..        re
+000007e0: 7475 726e 2020 6622 7b69 6e74 2872 6f75  turn  f"{int(rou
+000007f0: 6e64 2861 6273 6f6c 7574 652c 3129 297d  nd(absolute,1))}
+00000800: 5c6e 7b72 6f75 6e64 2870 6374 2c31 297d  \n{round(pct,1)}
+00000810: 2025 220d 0a20 2020 2020 2020 200d 0a20   %"..        .. 
+00000820: 2020 2066 696c 655f 696e 203d 2063 7467     file_in = ctg
+00000830: 5f70 6174 6820 2f20 5061 7468 2873 7472  _path / Path(str
+00000840: 2879 6561 7229 2920 2f20 5061 7468 2827  (year)) / Path('
+00000850: 5354 4154 4953 5449 5155 4553 2729 202f  STATISTIQUES') /
+00000860: 2050 6174 6828 2773 796e 7468 6573 652e   Path('synthese.
+00000870: 786c 7378 2729 0d0a 2020 2020 6466 5f74  xlsx')..    df_t
+00000880: 6f74 616c 203d 2070 642e 7265 6164 5f65  otal = pd.read_e
+00000890: 7863 656c 2866 696c 655f 696e 290d 0a20  xcel(file_in).. 
+000008a0: 2020 2064 665f 746f 7461 6c20 3d20 6466     df_total = df
+000008b0: 5f74 6f74 616c 2e64 726f 706e 6128 7375  _total.dropna(su
+000008c0: 6273 6574 3d5b 2754 7970 6527 5d29 200d  bset=['Type']) .
+000008d0: 0a20 2020 2064 665f 746f 7461 6c20 3d20  .    df_total = 
+000008e0: 6466 5f74 6f74 616c 2e64 726f 706e 6128  df_total.dropna(
+000008f0: 7375 6273 6574 3d5b 274e 6f6d 275d 290d  subset=['Nom']).
+00000900: 0a0d 0a20 2020 2064 6167 6720 3d20 6466  ...    dagg = df
+00000910: 5f74 6f74 616c 2e67 726f 7570 6279 2827  _total.groupby('
+00000920: 5479 7065 2729 5b27 6e62 725f 6a6f 7572  Type')['nbr_jour
+00000930: 7327 5d2e 6167 6728 7375 6d29 0d0a 0d0a  s'].agg(sum)....
+00000940: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+00000950: 6578 706c 6f64 655f 6469 6320 3d20 7b27  explode_dic = {'
+00000960: 5241 4e44 4f4e 4e45 4527 3a30 2e31 2c0d  RANDONNEE':0.1,.
+00000970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000980: 2020 2020 2753 454a 4f55 5227 3a30 2e30      'SEJOUR':0.0
+00000990: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+000009a0: 2020 2020 2020 2027 534f 5254 4945 5320         'SORTIES 
+000009b0: 4455 2044 494d 414e 4348 4527 3a30 2e32  DU DIMANCHE':0.2
+000009c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000009d0: 2020 2020 2020 2753 4f52 5449 4553 2044        'SORTIES D
+000009e0: 5520 4a45 5544 4927 3a30 2e32 2c0d 0a20  U JEUDI':0.2,.. 
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2020 2753 4f52 5449 4553 2044 5520 4c55    'SORTIES DU LU
+00000a10: 4e44 4927 3a30 2e32 2c20 0d0a 2020 2020  NDI':0.2, ..    
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000a30: 534f 5254 4945 5320 4455 2053 414d 4544  SORTIES DU SAMED
+00000a40: 4927 3a30 2e32 2c0d 0a20 2020 2020 2020  I':0.2,..       
+00000a50: 2020 2020 2020 2020 2020 2020 2753 4f52              'SOR
+00000a60: 5449 4553 2048 4956 4552 273a 302e 327d  TIES HIVER':0.2}
+00000a70: 0d0a 0d0a 2020 2020 6461 7461 203d 205b  ....    data = [
+00000a80: 5d0d 0a20 2020 2073 6f72 7469 6573 203d  ]..    sorties =
+00000a90: 205b 5d0d 0a20 2020 2066 6f72 2074 7970   []..    for typ
+00000aa0: 655f 7365 6a6f 7572 2c20 6e62 7220 696e  e_sejour, nbr in
+00000ab0: 207a 6970 2864 6167 672e 696e 6465 782c   zip(dagg.index,
+00000ac0: 6461 6767 2e74 6f6c 6973 7428 2929 3a0d  dagg.tolist()):.
+00000ad0: 0a20 2020 2020 2020 2069 6620 6e62 7221  .        if nbr!
+00000ae0: 3d30 3a0d 0a20 2020 2020 2020 2020 2020  =0:..           
+00000af0: 2064 6174 612e 6170 7065 6e64 286e 6272   data.append(nbr
+00000b00: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00000b10: 6f72 7469 6573 2e61 7070 656e 6428 7479  orties.append(ty
+00000b20: 7065 5f73 656a 6f75 7229 0d0a 0d0a 2020  pe_sejour)....  
+00000b30: 2020 6578 706c 6f64 6520 3d20 5b65 7870    explode = [exp
+00000b40: 6c6f 6465 5f64 6963 5b74 7970 5d20 666f  lode_dic[typ] fo
+00000b50: 7220 7479 7020 696e 2073 6f72 7469 6573  r typ in sorties
+00000b60: 5d0d 0a20 2020 200d 0a20 2020 200d 0a20  ]..    ..    .. 
+00000b70: 2020 2023 2043 7265 6174 696e 6720 706c     # Creating pl
+00000b80: 6f74 0d0a 2020 2020 6669 6720 3d20 706c  ot..    fig = pl
+00000b90: 742e 6669 6775 7265 2866 6967 7369 7a65  t.figure(figsize
+00000ba0: 203d 2831 302c 2037 2929 0d0a 2020 2020   =(10, 7))..    
+00000bb0: 5f2c 205f 2c20 6175 746f 7465 7874 7320  _, _, autotexts 
+00000bc0: 3d20 706c 742e 7069 6528 6461 7461 2c0d  = plt.pie(data,.
+00000bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000be0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00000bf0: 6162 656c 7320 3d20 736f 7274 6965 732c  abels = sorties,
+00000c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c20: 6175 746f 7063 7420 3d20 6c61 6d62 6461  autopct = lambda
+00000c30: 2070 6374 3a20 6675 6e63 2870 6374 2c20   pct: func(pct, 
+00000c40: 6461 7461 292c 0d0a 2020 2020 2020 2020  data),..        
+00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c60: 2020 2020 2020 6578 706c 6f64 6520 3d20        explode = 
+00000c70: 6578 706c 6f64 652c 0d0a 2020 2020 2020  explode,..      
+00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c90: 2020 2020 2020 2020 7465 7874 7072 6f70          textprop
+00000ca0: 733d 7b27 666f 6e74 7369 7a65 273a 2031  s={'fontsize': 1
+00000cb0: 387d 290d 0a20 2020 2070 6c74 2e74 6974  8})..    plt.tit
+00000cc0: 6c65 2873 7472 2879 6561 7229 2c20 7061  le(str(year), pa
+00000cd0: 643d 3530 2c20 666f 6e74 7369 7a65 3d32  d=50, fontsize=2
+00000ce0: 3029 0d0a 2020 2020 0d0a 2020 2020 5f20  0)..    ..    _ 
+00000cf0: 3d20 706c 742e 7365 7470 2861 7574 6f74  = plt.setp(autot
+00000d00: 6578 7473 2c20 2a2a 7b27 636f 6c6f 7227  exts, **{'color'
+00000d10: 3a27 6b27 2c20 2777 6569 6768 7427 3a27  :'k', 'weight':'
+00000d20: 626f 6c64 272c 2027 666f 6e74 7369 7a65  bold', 'fontsize
+00000d30: 273a 3134 7d29 0d0a 2020 2020 0d0a 2020  ':14})..    ..  
+00000d40: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
+00000d50: 7574 2829 0d0a 2020 2020 706c 742e 7368  ut()..    plt.sh
+00000d60: 6f77 2829 0d0a 2020 2020 0d0a 2020 2020  ow()..    ..    
+00000d70: 6669 675f 6669 6c65 203d 2027 534f 5254  fig_file = 'SORT
+00000d80: 4945 535f 5049 452e 706e 6727 0d0a 2020  IES_PIE.png'..  
+00000d90: 2020 706c 742e 7361 7665 6669 6728 6374    plt.savefig(ct
+00000da0: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
+00000db0: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
+00000dc0: 2753 5441 5449 5354 4951 5545 5327 2920  'STATISTIQUES') 
+00000dd0: 2f20 5061 7468 2866 6967 5f66 696c 6529  / Path(fig_file)
+00000de0: 2c62 626f 785f 696e 6368 6573 3d27 7469  ,bbox_inches='ti
+00000df0: 6768 7427 2909 0d0a 0d0a 2020 2020 7265  ght').....    re
+00000e00: 7475 726e 2009 0d0a 090d 0a0d 0a64 6566  turn ........def
+00000e10: 2073 796e 7468 6573 655f 6164 6865 7265   synthese_adhere
+00000e20: 6e74 2879 6561 722c 6374 675f 7061 7468  nt(year,ctg_path
+00000e30: 293a 0d0a 0d0a 2020 2020 2320 5374 616e  ):....    # Stan
+00000e40: 6461 7264 206c 6962 7261 7279 2069 6d70  dard library imp
+00000e50: 6f72 7473 0d0a 2020 2020 6672 6f6d 2070  orts..    from p
+00000e60: 6174 686c 6962 2069 6d70 6f72 7420 5061  athlib import Pa
+00000e70: 7468 0d0a 2020 2020 0d0a 2020 2020 2320  th..    ..    # 
+00000e80: 5468 6972 6420 7061 7274 7920 696d 706f  Third party impo
+00000e90: 7274 730d 0a20 2020 2069 6d70 6f72 7420  rts..    import 
+00000ea0: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
+00000eb0: 2020 0d0a 2020 2020 2320 496e 7465 726e    ..    # Intern
+00000ec0: 616c 2069 6d70 6f72 7473 0d0a 2020 2020  al imports..    
+00000ed0: 6672 6f6d 2043 5447 5f55 7469 6c73 2e43  from CTG_Utils.C
+00000ee0: 5447 5f46 756e 632e 4354 4743 6c61 7373  TG_Func.CTGClass
+00000ef0: 6573 2069 6d70 6f72 7420 4566 6665 6374  es import Effect
+00000f00: 6966 4374 670d 0a20 2020 200d 0a20 2020  ifCtg..    ..   
+00000f10: 2066 696c 655f 696e 203d 2063 7467 5f70   file_in = ctg_p
+00000f20: 6174 6820 2f20 5061 7468 2873 7472 2879  ath / Path(str(y
+00000f30: 6561 7229 2920 2f20 5061 7468 2827 5354  ear)) / Path('ST
+00000f40: 4154 4953 5449 5155 4553 2729 202f 2050  ATISTIQUES') / P
+00000f50: 6174 6828 2773 796e 7468 6573 652e 786c  ath('synthese.xl
+00000f60: 7378 2729 0d0a 2020 2020 6466 5f74 6f74  sx')..    df_tot
+00000f70: 616c 203d 2070 642e 7265 6164 5f65 7863  al = pd.read_exc
+00000f80: 656c 2866 696c 655f 696e 290d 0a20 2020  el(file_in)..   
+00000f90: 2064 665f 746f 7461 6c20 3d20 6466 5f74   df_total = df_t
+00000fa0: 6f74 616c 2e64 726f 706e 6128 7375 6273  otal.dropna(subs
+00000fb0: 6574 3d5b 2754 7970 6527 5d29 0d0a 2020  et=['Type'])..  
+00000fc0: 2020 6e62 7265 203d 207b 7d0d 0a20 2020    nbre = {}..   
+00000fd0: 200d 0a20 2020 2066 6f72 2069 645f 6c69   ..    for id_li
+00000fe0: 6365 6e63 652c 2064 6720 696e 2064 665f  cence, dg in df_
+00000ff0: 746f 7461 6c2e 6772 6f75 7062 7928 274e  total.groupby('N
+00001000: c2b0 204c 6963 656e 6369 c3a9 2729 3a0d  .. Licenci..'):.
+00001010: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00001020: 2020 206e 6272 655b 6964 5f6c 6963 656e     nbre[id_licen
+00001030: 6365 5d3d 5b64 675b 274e 6f6d 275d 2e75  ce]=[dg['Nom'].u
+00001040: 6e69 7175 6528 295b 305d 2c64 675b 2750  nique()[0],dg['P
+00001050: 72c3 a96e 6f6d 275d 2e75 6e69 7175 6528  r..nom'].unique(
+00001060: 295b 305d 5d0d 0a20 2020 200d 0a20 2020  )[0]]..    ..   
+00001070: 2020 2020 206e 625f 736f 7274 6965 5f64       nb_sortie_d
+00001080: 696d 616e 6368 6520 3d20 6c65 6e28 6467  imanche = len(dg
+00001090: 2e71 7565 7279 2822 5479 7065 2e73 7472  .query("Type.str
+000010a0: 2e63 6f6e 7461 696e 7328 2753 4f52 5449  .contains('SORTI
+000010b0: 4553 2044 5520 4449 4d41 4e43 4845 2729  ES DU DIMANCHE')
+000010c0: 2229 290d 0a20 2020 2020 2020 206e 6272  "))..        nbr
+000010d0: 655b 6964 5f6c 6963 656e 6365 5d20 3d20  e[id_licence] = 
+000010e0: 6e62 7265 5b69 645f 6c69 6365 6e63 655d  nbre[id_licence]
+000010f0: 202b 205b 6e62 5f73 6f72 7469 655f 6469   + [nb_sortie_di
+00001100: 6d61 6e63 6865 5d0d 0a20 2020 200d 0a20  manche]..    .. 
+00001110: 2020 2020 2020 206e 625f 736f 7274 6965         nb_sortie
+00001120: 5f73 616d 6564 6920 3d20 6c65 6e28 6467  _samedi = len(dg
+00001130: 2e71 7565 7279 2822 5479 7065 2e73 7472  .query("Type.str
+00001140: 2e63 6f6e 7461 696e 7328 2753 4f52 5449  .contains('SORTI
+00001150: 4553 2044 5520 5341 4d45 4449 2729 2229  ES DU SAMEDI')")
+00001160: 290d 0a20 2020 2020 2020 206e 6272 655b  )..        nbre[
+00001170: 6964 5f6c 6963 656e 6365 5d20 3d20 6e62  id_licence] = nb
+00001180: 7265 5b69 645f 6c69 6365 6e63 655d 202b  re[id_licence] +
+00001190: 205b 6e62 5f73 6f72 7469 655f 7361 6d65   [nb_sortie_same
+000011a0: 6469 5d0d 0a20 2020 200d 0a20 2020 2020  di]..    ..     
+000011b0: 2020 206e 625f 736f 7274 6965 5f6a 6575     nb_sortie_jeu
+000011c0: 6469 203d 206c 656e 2864 672e 7175 6572  di = len(dg.quer
+000011d0: 7928 2254 7970 652e 7374 722e 636f 6e74  y("Type.str.cont
+000011e0: 6169 6e73 2827 534f 5254 4945 5320 4455  ains('SORTIES DU
+000011f0: 204a 4555 4449 2729 2229 290d 0a20 2020   JEUDI')"))..   
+00001200: 2020 2020 206e 6272 655b 6964 5f6c 6963       nbre[id_lic
+00001210: 656e 6365 5d20 3d20 6e62 7265 5b69 645f  ence] = nbre[id_
+00001220: 6c69 6365 6e63 655d 202b 205b 6e62 5f73  licence] + [nb_s
+00001230: 6f72 7469 655f 6a65 7564 695d 0d0a 2020  ortie_jeudi]..  
+00001240: 2020 0d0a 2020 2020 2020 2020 6e62 5f72    ..        nb_r
+00001250: 616e 646f 203d 206c 656e 2864 672e 7175  ando = len(dg.qu
+00001260: 6572 7928 2254 7970 652e 7374 722e 636f  ery("Type.str.co
+00001270: 6e74 6169 6e73 2827 5241 4e44 4f4e 4e45  ntains('RANDONNE
+00001280: 4527 2922 2929 0d0a 2020 2020 2020 2020  E')"))..        
+00001290: 6e62 7265 5b69 645f 6c69 6365 6e63 655d  nbre[id_licence]
+000012a0: 203d 206e 6272 655b 6964 5f6c 6963 656e   = nbre[id_licen
+000012b0: 6365 5d20 2b20 5b6e 625f 7261 6e64 6f5d  ce] + [nb_rando]
+000012c0: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
+000012d0: 6e62 5f73 656a 6f75 725f 6a6f 7572 7320  nb_sejour_jours 
+000012e0: 3d20 7375 6d28 6467 2e71 7565 7279 2822  = sum(dg.query("
+000012f0: 5479 7065 2e73 7472 2e63 6f6e 7461 696e  Type.str.contain
+00001300: 7328 2753 454a 4f55 5227 2922 295b 276e  s('SEJOUR')")['n
+00001310: 6272 5f6a 6f75 7273 275d 2e74 6f6c 6973  br_jours'].tolis
+00001320: 7428 2929 0d0a 2020 2020 2020 2020 6e62  t())..        nb
+00001330: 7265 5b69 645f 6c69 6365 6e63 655d 203d  re[id_licence] =
+00001340: 206e 6272 655b 6964 5f6c 6963 656e 6365   nbre[id_licence
+00001350: 5d20 2b20 5b6e 625f 7365 6a6f 7572 5f6a  ] + [nb_sejour_j
+00001360: 6f75 7273 5d0d 0a0d 0a20 2020 2020 2020  ours]....       
+00001370: 206e 625f 7365 6a6f 7572 203d 206c 656e   nb_sejour = len
+00001380: 2864 672e 7175 6572 7928 2254 7970 652e  (dg.query("Type.
+00001390: 7374 722e 636f 6e74 6169 6e73 2827 5345  str.contains('SE
+000013a0: 4a4f 5552 2729 2229 5b27 7365 6a6f 7572  JOUR')")['sejour
+000013b0: 275d 2e75 6e69 7175 6528 2929 0d0a 2020  '].unique())..  
+000013c0: 2020 2020 2020 6e62 7265 5b69 645f 6c69        nbre[id_li
+000013d0: 6365 6e63 655d 203d 206e 6272 655b 6964  cence] = nbre[id
+000013e0: 5f6c 6963 656e 6365 5d20 2b20 5b6e 625f  _licence] + [nb_
+000013f0: 7365 6a6f 7572 5d0d 0a20 2020 200d 0a20  sejour]..    .. 
+00001400: 2020 2020 2020 206e 625f 6869 7665 7220         nb_hiver 
+00001410: 3d20 6c65 6e28 6467 2e71 7565 7279 2822  = len(dg.query("
+00001420: 5479 7065 2e73 7472 2e63 6f6e 7461 696e  Type.str.contain
+00001430: 7328 2753 4f52 5449 4553 2048 4956 4552  s('SORTIES HIVER
+00001440: 2729 2229 290d 0a20 2020 2020 2020 206e  ')"))..        n
+00001450: 6272 655b 6964 5f6c 6963 656e 6365 5d20  bre[id_licence] 
+00001460: 3d20 6e62 7265 5b69 645f 6c69 6365 6e63  = nbre[id_licenc
+00001470: 655d 202b 205b 6e62 5f68 6976 6572 5d0d  e] + [nb_hiver].
+00001480: 0a20 2020 200d 0a20 2020 2020 2020 206e  .    ..        n
+00001490: 6272 5f65 7665 6e65 6d65 6e74 7320 3d20  br_evenements = 
+000014a0: 5b6e 625f 736f 7274 6965 5f64 696d 616e  [nb_sortie_diman
+000014b0: 6368 6520 2b0d 0a20 2020 2020 2020 2020  che +..         
+000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014d0: 206e 625f 736f 7274 6965 5f73 616d 6564   nb_sortie_samed
+000014e0: 6920 2b20 0d0a 2020 2020 2020 2020 2020  i + ..          
+000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001500: 6e62 5f73 6f72 7469 655f 6a65 7564 6920  nb_sortie_jeudi 
+00001510: 2b0d 0a20 2020 2020 2020 2020 2020 2020  +..             
+00001520: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
+00001530: 7261 6e64 6f20 2b0d 0a20 2020 2020 2020  rando +..       
+00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001550: 2020 206e 625f 7365 6a6f 7572 5f6a 6f75     nb_sejour_jou
+00001560: 7273 202b 0d0a 2020 2020 2020 2020 2020  rs +..          
+00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001580: 6e62 5f68 6976 6572 5d0d 0a20 2020 2020  nb_hiver]..     
+00001590: 2020 206e 6272 655b 6964 5f6c 6963 656e     nbre[id_licen
+000015a0: 6365 5d20 3d20 6e62 7265 5b69 645f 6c69  ce] = nbre[id_li
+000015b0: 6365 6e63 655d 202b 206e 6272 5f65 7665  cence] + nbr_eve
+000015c0: 6e65 6d65 6e74 730d 0a20 2020 200d 0a20  nements..    .. 
+000015d0: 2020 2064 6720 3d20 7064 2e44 6174 6146     dg = pd.DataF
+000015e0: 7261 6d65 2e66 726f 6d5f 6469 6374 286e  rame.from_dict(n
+000015f0: 6272 6529 2e54 0d0a 2020 2020 6467 2e63  bre).T..    dg.c
+00001600: 6f6c 756d 6e73 203d 205b 0d0a 2020 2020  olumns = [..    
+00001610: 2020 2020 2020 2020 2020 2020 2027 4e6f               'No
+00001620: 6d27 2c0d 0a20 2020 2020 2020 2020 2020  m',..           
+00001630: 2020 2020 2020 2750 72c3 a96e 6f6d 272c        'Pr..nom',
+00001640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001650: 2020 2027 534f 5254 4945 2044 5520 4449     'SORTIE DU DI
+00001660: 4d41 4e43 4845 2043 4c55 4227 2c0d 0a20  MANCHE CLUB',.. 
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2753 4f52 5449 4520 4455 2053 414d 4544  'SORTIE DU SAMED
+00001690: 4920 434c 5542 272c 0d0a 2020 2020 2020  I CLUB',..      
+000016a0: 2020 2020 2020 2020 2020 2027 534f 5254             'SORT
+000016b0: 4945 2044 5520 4a45 5544 4920 434c 5542  IE DU JEUDI CLUB
+000016c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000016d0: 2020 2020 2027 5241 4e44 4f4e 4e45 4527       'RANDONNEE'
+000016e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000016f0: 2020 2020 2753 454a 4f55 522d 4a4f 5552      'SEJOUR-JOUR
+00001700: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001710: 2020 2020 2027 4e62 725f 5345 4a4f 5552       'Nbr_SEJOUR
+00001720: 5327 2c0d 0a20 2020 2020 2020 2020 2020  S',..           
+00001730: 2020 2020 2020 2753 4f52 5449 4520 4849        'SORTIE HI
+00001740: 5645 5227 2c0d 0a20 2020 2020 2020 2020  VER',..         
+00001750: 2020 2020 2020 2020 2754 4f54 414c 272c          'TOTAL',
+00001760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001770: 2020 205d 0d0a 2020 2020 0d0a 2020 2020     ]..    ..    
+00001780: 6566 6665 6374 6966 203d 2045 6666 6563  effectif = Effec
+00001790: 7469 6643 7467 2879 6561 722c 6374 675f  tifCtg(year,ctg_
+000017a0: 7061 7468 290d 0a20 2020 2064 665f 6566  path)..    df_ef
+000017b0: 6665 6374 6966 203d 2065 6666 6563 7469  fectif = effecti
+000017c0: 662e 6566 6665 6374 6966 0d0a 2020 2020  f.effectif..    
+000017d0: 6466 5f65 6666 6563 7469 662e 696e 6465  df_effectif.inde
+000017e0: 7820 3d20 6466 5f65 6666 6563 7469 665b  x = df_effectif[
+000017f0: 274e c2b0 204c 6963 656e 6369 c3a9 275d  'N.. Licenci..']
+00001800: 0d0a 2020 2020 6f72 7068 616e 203d 2073  ..    orphan = s
+00001810: 6574 2864 665f 6566 6665 6374 6966 2e69  et(df_effectif.i
+00001820: 6e64 6578 2920 2d20 7365 7428 6467 2e69  ndex) - set(dg.i
+00001830: 6e64 6578 290d 0a20 2020 2064 665f 6f72  ndex)..    df_or
+00001840: 7068 616e 203d 2064 665f 6566 6665 6374  phan = df_effect
+00001850: 6966 2e6c 6f63 5b6c 6973 7428 6f72 7068  if.loc[list(orph
+00001860: 616e 295d 5b5b 274e 6f6d 272c 2750 72c3  an)][['Nom','Pr.
+00001870: a96e 6f6d 275d 5d0d 0a20 2020 2064 665f  .nom']]..    df_
+00001880: 6f72 7068 616e 5b5b 2753 4f52 5449 4520  orphan[['SORTIE 
+00001890: 4455 2044 494d 414e 4348 4520 434c 5542  DU DIMANCHE CLUB
+000018a0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000018b0: 2020 2027 534f 5254 4945 2044 5520 5341     'SORTIE DU SA
+000018c0: 4d45 4449 2043 4c55 4227 2c0d 0a20 2020  MEDI CLUB',..   
+000018d0: 2020 2020 2020 2020 2020 2020 2753 4f52              'SOR
+000018e0: 5449 4520 4455 204a 4555 4449 2043 4c55  TIE DU JEUDI CLU
+000018f0: 4227 2c0d 0a20 2020 2020 2020 2020 2020  B',..           
+00001900: 2020 2020 2752 414e 444f 4e4e 4545 272c      'RANDONNEE',
+00001910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001920: 2027 5345 4a4f 5552 2d4a 4f55 5227 2c0d   'SEJOUR-JOUR',.
+00001930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001940: 274e 6272 5f53 454a 4f55 5253 272c 0d0a  'Nbr_SEJOURS',..
+00001950: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001960: 534f 5254 4945 2048 4956 4552 272c 0d0a  SORTIE HIVER',..
+00001970: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001980: 544f 5441 4c27 5d5d 203d 205b 302c 302c  TOTAL']] = [0,0,
+00001990: 302c 302c 302c 302c 302c 305d 0d0a 2020  0,0,0,0,0,0]..  
+000019a0: 2020 0d0a 2020 2020 6467 203d 2070 642e    ..    dg = pd.
+000019b0: 636f 6e63 6174 285b 6467 2c20 6466 5f6f  concat([dg, df_o
+000019c0: 7270 6861 6e5d 2c20 6178 6973 3d30 290d  rphan], axis=0).
+000019d0: 0a20 2020 200d 0a20 2020 2066 696c 655f  .    ..    file_
+000019e0: 6f75 7420 3d20 6374 675f 7061 7468 202f  out = ctg_path /
+000019f0: 2050 6174 6828 7374 7228 7965 6172 2929   Path(str(year))
+00001a00: 202f 2050 6174 6828 2753 5441 5449 5354   / Path('STATIST
+00001a10: 4951 5545 5327 2920 2f20 5061 7468 2827  IQUES') / Path('
+00001a20: 7379 6e74 6865 7365 5f61 6468 6572 656e  synthese_adheren
+00001a30: 742e 786c 7378 2729 0d0a 2020 2020 6467  t.xlsx')..    dg
+00001a40: 2e74 6f5f 6578 6365 6c28 6669 6c65 5f6f  .to_excel(file_o
+00001a50: 7574 290d 0a20 2020 200d 0a64 6566 2073  ut)..    ..def s
+00001a60: 796e 7468 6573 655f 7261 6e64 6f6e 6e65  ynthese_randonne
+00001a70: 6528 7965 6172 2c63 7467 5f70 6174 6829  e(year,ctg_path)
+00001a80: 3a0d 0a0d 0a20 2020 2023 2053 7461 6e64  :....    # Stand
+00001a90: 6172 6420 6c69 6272 6172 7920 696d 706f  ard library impo
+00001aa0: 7274 730d 0a20 2020 2066 726f 6d20 7061  rts..    from pa
+00001ab0: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
+00001ac0: 680d 0a20 2020 200d 0a20 2020 2023 2054  h..    ..    # T
+00001ad0: 6869 7264 2070 6172 7479 2069 6d70 6f72  hird party impor
+00001ae0: 7473 0d0a 2020 2020 696d 706f 7274 206d  ts..    import m
+00001af0: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
+00001b00: 2061 7320 706c 740d 0a20 2020 2069 6d70   as plt..    imp
+00001b10: 6f72 7420 7061 6e64 6173 2061 7320 7064  ort pandas as pd
+00001b20: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00001b30: 6164 646c 6162 656c 7328 782c 792c 6f66  addlabels(x,y,of
+00001b40: 6673 6574 293a 0d0a 2020 2020 2020 2020  fset):..        
+00001b50: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00001b60: 656e 2878 2929 3a0d 0a20 2020 2020 2020  en(x)):..       
+00001b70: 2020 2020 2069 6620 795b 695d 2021 3d20       if y[i] != 
+00001b80: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00001b90: 2020 2020 706c 742e 7465 7874 2878 5b69      plt.text(x[i
+00001ba0: 5d2c 795b 695d 2b6f 6666 7365 742c 726f  ],y[i]+offset,ro
+00001bb0: 756e 6428 795b 695d 2c31 292c 7369 7a65  und(y[i],1),size
+00001bc0: 3d31 3029 0d0a 2020 2020 2020 2020 0d0a  =10)..        ..
+00001bd0: 2020 2020 0d0a 2020 2020 6669 6c65 5f69      ..    file_i
+00001be0: 6e20 3d20 5061 7468 2863 7467 5f70 6174  n = Path(ctg_pat
+00001bf0: 6829 202f 2050 6174 6828 7374 7228 7965  h) / Path(str(ye
+00001c00: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
+00001c10: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
+00001c20: 7468 2827 7379 6e74 6865 7365 2e78 6c73  th('synthese.xls
+00001c30: 7827 290d 0a20 2020 2064 665f 746f 7461  x')..    df_tota
+00001c40: 6c20 3d20 7064 2e72 6561 645f 6578 6365  l = pd.read_exce
+00001c50: 6c28 6669 6c65 5f69 6e29 0d0a 2020 2020  l(file_in)..    
+00001c60: 6466 5f74 6f74 616c 203d 2064 665f 746f  df_total = df_to
+00001c70: 7461 6c2e 6472 6f70 6e61 2873 7562 7365  tal.dropna(subse
+00001c80: 743d 5b27 4e6f 6d27 5d29 200d 0a20 2020  t=['Nom']) ..   
+00001c90: 2064 6720 3d20 6466 5f74 6f74 616c 2e71   dg = df_total.q
+00001ca0: 7565 7279 2827 5479 7065 3d3d 2252 414e  uery('Type=="RAN
+00001cb0: 444f 4e4e 4545 2227 292e 6772 6f75 7062  DONNEE"').groupb
+00001cc0: 7928 2773 656a 6f75 7227 292e 6167 6728  y('sejour').agg(
+00001cd0: 2763 6f75 6e74 2729 5b27 4ec2 b020 4c69  'count')['N.. Li
+00001ce0: 6365 6e63 69c3 a927 5d0d 0a20 2020 200d  cenci..']..    .
+00001cf0: 0a20 2020 2066 6967 203d 2070 6c74 2e66  .    fig = plt.f
+00001d00: 6967 7572 6528 290d 0a20 2020 2070 6c74  igure()..    plt
+00001d10: 2e62 6172 2872 616e 6765 286c 656e 2864  .bar(range(len(d
+00001d20: 6729 292c 6467 2e74 6f6c 6973 7428 2929  g)),dg.tolist())
+00001d30: 0d0a 2020 2020 6164 646c 6162 656c 7328  ..    addlabels(
+00001d40: 6c69 7374 2872 616e 6765 286c 656e 2864  list(range(len(d
+00001d50: 6729 2929 2c64 672e 746f 6c69 7374 2829  g))),dg.tolist()
+00001d60: 2c30 2e32 290d 0a20 2020 2070 6c74 2e78  ,0.2)..    plt.x
+00001d70: 7469 636b 7328 7261 6e67 6528 6c65 6e28  ticks(range(len(
+00001d80: 6467 2929 2c20 6467 2e69 6e64 6578 2c20  dg)), dg.index, 
+00001d90: 726f 7461 7469 6f6e 3d27 7665 7274 6963  rotation='vertic
+00001da0: 616c 2729 0d0a 2020 2020 706c 742e 7469  al')..    plt.ti
+00001db0: 636b 5f70 6172 616d 7328 6178 6973 3d27  ck_params(axis='
+00001dc0: 7827 2c20 726f 7461 7469 6f6e 3d39 302c  x', rotation=90,
+00001dd0: 206c 6162 656c 7369 7a65 3d31 3029 0d0a   labelsize=10)..
+00001de0: 2020 2020 706c 742e 7469 636b 5f70 6172      plt.tick_par
+00001df0: 616d 7328 6178 6973 3d27 7927 2c6c 6162  ams(axis='y',lab
+00001e00: 656c 7369 7a65 3d31 3029 0d0a 2020 2020  elsize=10)..    
+00001e10: 0d0a 2020 2020 5f20 3d20 706c 742e 7469  ..    _ = plt.ti
+00001e20: 746c 6528 6627 2320 7261 6e64 6f73 203a  tle(f'# randos :
+00001e30: 207b 6c65 6e28 6467 297d 202c 2023 2070   {len(dg)} , # p
+00001e40: 6172 7469 6369 7061 6e74 7320 3a20 7b73  articipants : {s
+00001e50: 756d 2864 6729 7d27 290d 0a20 2020 2070  um(dg)}')..    p
+00001e60: 6c74 2e74 6967 6874 5f6c 6179 6f75 7428  lt.tight_layout(
+00001e70: 290d 0a20 2020 2070 6c74 2e73 686f 7728  )..    plt.show(
+00001e80: 290d 0a20 2020 200d 0a20 2020 2066 6967  )..    ..    fig
+00001e90: 5f66 696c 6520 3d20 2753 594e 5448 4553  _file = 'SYNTHES
+00001ea0: 455f 5241 4e44 4f4e 4e45 4553 2e70 6e67  E_RANDONNEES.png
+00001eb0: 270d 0a20 2020 2070 6c74 2e73 6176 6566  '..    plt.savef
+00001ec0: 6967 2863 7467 5f70 6174 6820 2f20 5061  ig(ctg_path / Pa
+00001ed0: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
+00001ee0: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
+00001ef0: 4553 2729 202f 2050 6174 6828 6669 675f  ES') / Path(fig_
+00001f00: 6669 6c65 292c 6262 6f78 5f69 6e63 6865  file),bbox_inche
+00001f10: 733d 2774 6967 6874 2729 0d0a 2020 2020  s='tight')..    
+00001f20: 0d0a 6465 6620 6e62 725f 7365 6a6f 7572  ..def nbr_sejour
+00001f30: 735f 6164 6865 7265 6e74 2879 6561 722c  s_adherent(year,
+00001f40: 2063 7467 5f70 6174 6829 3a0d 0a0d 0a20   ctg_path):.... 
+00001f50: 2020 2023 2053 7461 6e64 6172 6420 6c69     # Standard li
+00001f60: 6272 6172 7920 696d 706f 7274 730d 0a20  brary imports.. 
+00001f70: 2020 2066 726f 6d20 636f 6c6c 6563 7469     from collecti
+00001f80: 6f6e 7320 696d 706f 7274 2043 6f75 6e74  ons import Count
+00001f90: 6572 0d0a 2020 2020 6672 6f6d 2070 6174  er..    from pat
+00001fa0: 686c 6962 2069 6d70 6f72 7420 5061 7468  hlib import Path
+00001fb0: 0d0a 2020 2020 0d0a 2020 2020 2320 5468  ..    ..    # Th
+00001fc0: 6972 6420 7061 7274 7920 696d 706f 7274  ird party import
+00001fd0: 730d 0a20 2020 2069 6d70 6f72 7420 6d61  s..    import ma
+00001fe0: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
+00001ff0: 6173 2070 6c74 0d0a 2020 2020 696d 706f  as plt..    impo
+00002000: 7274 2070 616e 6461 7320 6173 2070 640d  rt pandas as pd.
+00002010: 0a20 2020 200d 0a20 2020 2070 6c74 2e73  .    ..    plt.s
+00002020: 7479 6c65 2e75 7365 2827 6767 706c 6f74  tyle.use('ggplot
+00002030: 2729 0d0a 2020 2020 0d0a 2020 2020 2320  ')..    ..    # 
+00002040: 6675 6e63 7469 6f6e 2074 6f20 6164 6420  function to add 
+00002050: 7661 6c75 6520 6c61 6265 6c73 0d0a 2020  value labels..  
+00002060: 2020 6465 6620 6164 646c 6162 656c 7328    def addlabels(
+00002070: 782c 7929 3a0d 0a20 2020 2020 2020 2066  x,y):..        f
+00002080: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00002090: 6e28 7829 293a 0d0a 2020 2020 2020 2020  n(x)):..        
+000020a0: 2020 2020 706c 742e 7465 7874 2878 5b69      plt.text(x[i
+000020b0: 5d2d 302e 322c 795b 695d 2b31 2c79 5b69  ]-0.2,y[i]+1,y[i
+000020c0: 5d2c 7369 7a65 3d6c 6162 656c 5f73 697a  ],size=label_siz
+000020d0: 6529 0d0a 2020 2020 6c61 6265 6c5f 7369  e)..    label_si
+000020e0: 7a65 203d 2031 350d 0a20 2020 2066 696c  ze = 15..    fil
+000020f0: 655f 696e 203d 2063 7467 5f70 6174 6820  e_in = ctg_path 
+00002100: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
+00002110: 2920 2f20 5061 7468 2827 5354 4154 4953  ) / Path('STATIS
+00002120: 5449 5155 4553 2729 202f 2050 6174 6828  TIQUES') / Path(
+00002130: 2773 796e 7468 6573 655f 6164 6865 7265  'synthese_adhere
+00002140: 6e74 2e78 6c73 7827 290d 0a20 2020 2064  nt.xlsx')..    d
+00002150: 665f 746f 7461 6c20 3d20 7064 2e72 6561  f_total = pd.rea
+00002160: 645f 6578 6365 6c28 6669 6c65 5f69 6e29  d_excel(file_in)
+00002170: 0d0a 2020 2020 0d0a 2020 2020 6320 3d20  ..    ..    c = 
+00002180: 436f 756e 7465 7228 290d 0a20 2020 2063  Counter()..    c
+00002190: 203d 2043 6f75 6e74 6572 2864 665f 746f   = Counter(df_to
+000021a0: 7461 6c5b 274e 6272 5f53 454a 4f55 5253  tal['Nbr_SEJOURS
+000021b0: 275d 2e74 6f6c 6973 7428 2929 0d0a 2020  '].tolist())..  
+000021c0: 2020 6320 3d20 632e 6d6f 7374 5f63 6f6d    c = c.most_com
+000021d0: 6d6f 6e28 290d 0a0d 0a20 2020 2078 2c20  mon()....    x, 
+000021e0: 7920 3d20 7a69 7028 2a63 290d 0a20 2020  y = zip(*c)..   
+000021f0: 2078 203d 206c 6973 7428 7829 0d0a 2020   x = list(x)..  
+00002200: 2020 7920 3d20 6c69 7374 2879 290d 0a20    y = list(y).. 
+00002210: 2020 200d 0a20 2020 2066 6967 2c20 6178     ..    fig, ax
+00002220: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
+00002230: 6669 6773 697a 653d 2835 2c35 2929 0d0a  figsize=(5,5))..
+00002240: 2020 2020 706c 742e 6261 7228 5b73 7472      plt.bar([str
+00002250: 2878 5f73 2920 666f 7220 785f 7320 696e  (x_s) for x_s in
+00002260: 2078 5d2c 7929 0d0a 2020 2020 706c 742e   x],y)..    plt.
+00002270: 786c 6162 656c 2827 4e6f 6d62 7265 2064  xlabel('Nombre d
+00002280: 6520 7061 7274 6963 6970 6174 696f 6e20  e participation 
+00002290: c3a0 2064 6573 2073 c3a9 6a6f 7572 7327  .. des s..jours'
+000022a0: 290d 0a20 2020 2070 6c74 2e79 6c61 6265  )..    plt.ylabe
+000022b0: 6c28 274e 6f6d 6272 6520 6465 206c 6963  l('Nombre de lic
+000022c0: 656e 6369 6572 7327 290d 0a20 2020 2070  enciers')..    p
+000022d0: 6c74 2e74 6963 6b5f 7061 7261 6d73 2861  lt.tick_params(a
+000022e0: 7869 733d 2778 272c 206c 6162 656c 7369  xis='x', labelsi
+000022f0: 7a65 3d6c 6162 656c 5f73 697a 6529 0d0a  ze=label_size)..
+00002300: 2020 2020 706c 742e 7469 636b 5f70 6172      plt.tick_par
+00002310: 616d 7328 6178 6973 3d27 7927 2c20 6c61  ams(axis='y', la
+00002320: 6265 6c73 697a 653d 6c61 6265 6c5f 7369  belsize=label_si
+00002330: 7a65 290d 0a20 2020 2070 6c74 2e74 6974  ze)..    plt.tit
+00002340: 6c65 2873 7472 2879 6561 7229 2c70 6164  le(str(year),pad
+00002350: 3d32 302c 2066 6f6e 7473 697a 653d 3230  =20, fontsize=20
+00002360: 290d 0a20 2020 200d 0a20 2020 2061 782e  )..    ..    ax.
+00002370: 7365 745f 786c 6162 656c 2827 4e20 73c3  set_xlabel('N s.
+00002380: a96a 6f75 7273 272c 2066 6f6e 7473 697a  .jours', fontsiz
+00002390: 6520 3d20 6c61 6265 6c5f 7369 7a65 290d  e = label_size).
+000023a0: 0a20 2020 2061 782e 7365 745f 796c 6162  .    ax.set_ylab
+000023b0: 656c 2827 4e6f 6d62 7265 2064 6520 4354  el('Nombre de CT
+000023c0: 4720 6179 616e 7420 5c6e 2070 6172 7469  G ayant \n parti
+000023d0: 6369 70c3 a920 c3a0 204e 2073 c3a9 6a6f  cip.. .. N s..jo
+000023e0: 7572 7327 2c20 666f 6e74 7369 7a65 203d  urs', fontsize =
+000023f0: 206c 6162 656c 5f73 697a 6529 0d0a 2020   label_size)..  
+00002400: 2020 0d0a 2020 2020 782e 736f 7274 2829    ..    x.sort()
+00002410: 0d0a 2020 2020 6164 646c 6162 656c 7328  ..    addlabels(
+00002420: 782c 7929 0d0a 2020 2020 706c 742e 7469  x,y)..    plt.ti
+00002430: 6768 745f 6c61 796f 7574 2829 0d0a 2020  ght_layout()..  
+00002440: 2020 706c 742e 7368 6f77 2829 0d0a 0d0a    plt.show()....
+00002450: 2020 2020 6669 675f 6669 6c65 203d 2027      fig_file = '
+00002460: 5345 4a4f 5552 535f 5354 4154 5f50 4152  SEJOURS_STAT_PAR
+00002470: 5449 4349 5041 5449 4f4e 2e70 6e67 270d  TICIPATION.png'.
+00002480: 0a20 2020 2070 6c74 2e73 6176 6566 6967  .    plt.savefig
+00002490: 2863 7467 5f70 6174 6820 2f20 5061 7468  (ctg_path / Path
+000024a0: 2873 7472 2879 6561 7229 2920 2f20 5061  (str(year)) / Pa
+000024b0: 7468 2827 5354 4154 4953 5449 5155 4553  th('STATISTIQUES
+000024c0: 2729 202f 2050 6174 6828 6669 675f 6669  ') / Path(fig_fi
+000024d0: 6c65 292c 6262 6f78 5f69 6e63 6865 733d  le),bbox_inches=
+000024e0: 2774 6967 6874 2729 0d0a 2020 2020 0d0a  'tight')..    ..
+000024f0: 6465 6620 7265 6164 5f6d 656d 6f72 795f  def read_memory_
+00002500: 736f 7274 6965 7328 293a 0d0a 0d0a 2020  sorties():....  
+00002510: 2020 2320 5374 616e 6461 7264 206c 6962    # Standard lib
+00002520: 7261 7279 2069 6d70 6f72 7473 0d0a 2020  rary imports..  
+00002530: 2020 696d 706f 7274 206f 732e 7061 7468    import os.path
+00002540: 0d0a 2020 2020 6672 6f6d 2070 6174 686c  ..    from pathl
+00002550: 6962 2069 6d70 6f72 7420 5061 7468 0d0a  ib import Path..
+00002560: 0d0a 2020 2020 2320 3372 6420 7061 7274  ..    # 3rd part
+00002570: 7920 696d 706f 7274 730d 0a20 2020 2069  y imports..    i
+00002580: 6d70 6f72 7420 7961 6d6c 0d0a 2020 2020  mport yaml..    
+00002590: 0d0a 2020 2020 2320 5265 6164 7320 7468  ..    # Reads th
+000025a0: 6520 6465 6661 756c 7420 5056 6368 6172  e default PVchar
+000025b0: 6163 7465 7269 7a61 7469 6f6e 2e79 616d  acterization.yam
+000025c0: 6c20 636f 6e66 6967 2066 696c 650d 0a20  l config file.. 
+000025d0: 2020 2070 6174 685f 636f 6e66 6967 5f66     path_config_f
+000025e0: 696c 6520 3d20 5061 7468 285f 5f66 696c  ile = Path(__fil
+000025f0: 655f 5f29 2e70 6172 656e 742e 7061 7265  e__).parent.pare
+00002600: 6e74 202f 2050 6174 6828 2743 5447 5f46  nt / Path('CTG_F
+00002610: 756e 6327 2920 2f20 5061 7468 2827 4354  unc') / Path('CT
+00002620: 475f 5265 6646 696c 6573 2729 202f 2050  G_RefFiles') / P
+00002630: 6174 6828 276d 656d 6f72 795f 736f 7274  ath('memory_sort
+00002640: 6965 732e 796d 6c27 290d 0a20 2020 2077  ies.yml')..    w
+00002650: 6974 6820 6f70 656e 2870 6174 685f 636f  ith open(path_co
+00002660: 6e66 6967 5f66 696c 6529 2061 7320 6669  nfig_file) as fi
+00002670: 6c65 3a0d 0a20 2020 2020 2020 206d 656d  le:..        mem
+00002680: 6f72 7920 3d20 7961 6d6c 2e73 6166 655f  ory = yaml.safe_
+00002690: 6c6f 6164 2866 696c 6529 0d0a 2020 2020  load(file)..    
+000026a0: 2020 2020 0d0a 2020 2020 2020 200d 0a20      ..       .. 
+000026b0: 2020 2072 6574 7572 6e20 6d65 6d6f 7279     return memory
+000026c0: 0d0a 2020 2020 0d0a 6465 6620 6576 6f6c  ..    ..def evol
+000026d0: 7574 696f 6e5f 736f 7274 6965 7328 7479  ution_sorties(ty
+000026e0: 7065 2c63 7467 5f70 6174 6829 3a0d 0a0d  pe,ctg_path):...
+000026f0: 0a20 2020 2023 2053 7461 6e64 6172 6420  .    # Standard 
+00002700: 6c69 6272 6172 7920 696d 706f 7274 2020  library import  
+00002710: 2020 0d0a 2020 2020 696d 706f 7274 2064    ..    import d
+00002720: 6174 6574 696d 650d 0a20 2020 2066 726f  atetime..    fro
+00002730: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
+00002740: 2050 6174 680d 0a20 2020 2066 726f 6d20   Path..    from 
+00002750: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
+00002760: 7274 206e 616d 6564 7475 706c 650d 0a0d  rt namedtuple...
+00002770: 0a20 2020 2023 2054 6869 7264 2070 6172  .    # Third par
+00002780: 7479 206c 6962 7261 7279 2069 6d70 6f72  ty library impor
+00002790: 7420 2020 2020 0d0a 2020 2020 696d 706f  t     ..    impo
+000027a0: 7274 206d 6174 706c 6f74 6c69 622e 7079  rt matplotlib.py
+000027b0: 706c 6f74 2061 7320 706c 740d 0a20 2020  plot as plt..   
+000027c0: 2069 6d70 6f72 7420 7061 6e64 6173 2061   import pandas a
+000027d0: 7320 7064 0d0a 2020 2020 2020 0d0a 2020  s pd..      ..  
+000027e0: 2020 2320 496e 7465 726e 616c 2069 6d70    # Internal imp
+000027f0: 6f72 740d 0a20 2020 2069 6d70 6f72 7420  ort..    import 
+00002800: 4354 475f 5574 696c 7320 6173 2063 7467  CTG_Utils as ctg
+00002810: 0d0a 2020 2020 6672 6f6d 2043 5447 5f55  ..    from CTG_U
+00002820: 7469 6c73 2e43 5447 5f47 5549 2e47 5549  tils.CTG_GUI.GUI
+00002830: 5f47 6c6f 6261 6c73 2069 6d70 6f72 7420  _Globals import 
+00002840: 4143 5449 5649 5445 5f4c 4953 5420 0d0a  ACTIVITE_LIST ..
+00002850: 2020 2020 0d0a 2020 2020 6465 6620 6164      ..    def ad
+00002860: 645f 6d65 6d6f 7279 2873 7461 745f 6469  d_memory(stat_di
+00002870: 632c 7965 6172 7329 3a0d 0a20 2020 2020  c,years):..     
+00002880: 2020 206d 656d 6f72 7920 3d20 7265 6164     memory = read
+00002890: 5f6d 656d 6f72 795f 736f 7274 6965 7328  _memory_sorties(
+000028a0: 290d 0a20 2020 200d 0a20 2020 200d 0a20  )..    ..    .. 
+000028b0: 2020 2020 2020 2066 6f72 2079 6561 722c         for year,
+000028c0: 7620 696e 206d 656d 6f72 795b 276d 656d  v in memory['mem
+000028d0: 6f72 7927 5d2e 6974 656d 7328 293a 0d0a  ory'].items():..
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00002910: 2020 2020 2020 2020 2073 7461 745f 6469           stat_di
+00002920: 635b 7374 7228 7965 6172 295d 203d 2073  c[str(year)] = s
+00002930: 7461 7479 6561 7228 765b 2750 4152 5449  tatyear(v['PARTI
+00002940: 4349 5041 5449 4f4e 5f53 454a 4f55 5253  CIPATION_SEJOURS
+00002950: 275d 2c20 2020 2020 2020 2020 2020 2020  '],             
+00002960: 2020 2023 206e 6272 5f73 656a 6f75 7273     # nbr_sejours
+00002970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2020 2020 2020 2020 2020 2020 2030 2c20               0, 
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 2020 2020 2020 2020 2023 206a 6f75 7273           # jours
+000029c0: 5f73 656a 6f75 720d 0a20 2020 2020 2020  _sejour..       
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 2020 765b 2753 4f52 5449 4553 5f43      v['SORTIES_C
+00002a00: 4c55 425f 4449 4d41 4e43 4845 275d 2c20  LUB_DIMANCHE'], 
+00002a10: 2320 736f 7274 6965 5f64 696d 616e 6368  # sortie_dimanch
+00002a20: 655f 636c 7562 0d0a 2020 2020 2020 2020  e_club..        
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 2020 2076 5b27 534f 5254 4945 535f 434c     v['SORTIES_CL
+00002a60: 5542 5f53 414d 4544 4927 5d2c 2020 2023  UB_SAMEDI'],   #
+00002a70: 2073 6f72 7469 655f 7361 6d65 6469 5f63   sortie_samedi_c
+00002a80: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ab0: 765b 2753 4f52 5449 4553 5f48 4956 4552  v['SORTIES_HIVER
+00002ac0: 275d 2c20 2020 2020 2020 2020 2320 736f  '],         # so
+00002ad0: 7274 6965 5f68 6976 6572 5f63 6c75 620d  rtie_hiver_club.
+00002ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 302c 2020 2020 2020 2020 2020 2020 2020  0,              
-00002b10: 2020 2020 2020 2020 2020 2020 2320 6a6f              # jo
-00002b20: 7572 735f 7365 6a6f 7572 0d0a 2020 2020  urs_sejour..    
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b00: 2020 2020 2020 2020 2020 2020 765b 2753              v['S
+00002b10: 4f52 5449 4553 5f43 4c55 425f 4a45 5544  ORTIES_CLUB_JEUD
+00002b20: 4927 5d2c 2020 2020 2320 736f 7274 6965  I'],    # sortie
+00002b30: 5f6a 6575 6469 5f63 6c75 620d 0a20 2020  _jeudi_club..   
 00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 2020 2020 2076 5b27 534f 5254 4945         v['SORTIE
-00002b60: 535f 434c 5542 5f44 494d 414e 4348 4527  S_CLUB_DIMANCHE'
-00002b70: 5d2c 2023 2073 6f72 7469 655f 6469 6d61  ], # sortie_dima
-00002b80: 6e63 6865 5f63 6c75 620d 0a20 2020 2020  nche_club..     
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b60: 2020 2020 2020 2020 765b 2752 414e 444f          v['RANDO
+00002b70: 4e4e 4545 5327 5d2c 2020 2020 2020 2020  NNEES'],        
+00002b80: 2020 2020 2320 7261 6e64 6f6e 6e65 650d      # randonnee.
+00002b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2020 2020 2020 765b 2753 4f52 5449 4553        v['SORTIES
-00002bc0: 5f43 4c55 425f 5341 4d45 4449 275d 2c20  _CLUB_SAMEDI'], 
-00002bd0: 2020 2320 736f 7274 6965 5f73 616d 6564    # sortie_samed
-00002be0: 695f 636c 7562 0d0a 2020 2020 2020 2020  i_club..        
+00002bb0: 2020 2020 2020 2020 2020 2020 765b 274e              v['N
+00002bc0: 6f6d 6272 655f 7365 6a6f 7572 7327 5d2c  ombre_sejours'],
+00002bd0: 2020 2020 2020 2020 2320 6e62 725f 7365          # nbr_se
+00002be0: 6a6f 7572 730d 0a20 2020 2020 2020 2020  jours..         
 00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2076 5b27 534f 5254 4945 535f 4849     v['SORTIES_HI
-00002c20: 5645 5227 5d2c 2020 2020 2020 2020 2023  VER'],         #
-00002c30: 2073 6f72 7469 655f 6869 7665 725f 636c   sortie_hiver_cl
-00002c40: 7562 0d0a 2020 2020 2020 2020 2020 2020  ub..            
+00002c10: 2020 302c 2920 2020 2020 2020 2020 2020    0,)           
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00002c30: 6e62 725f 6a6f 7572 735f 7365 6a6f 7572  nbr_jours_sejour
+00002c40: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
 00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00002c70: 5b27 534f 5254 4945 535f 434c 5542 5f4a  ['SORTIES_CLUB_J
-00002c80: 4555 4449 275d 2c20 2020 2023 2073 6f72  EUDI'],    # sor
-00002c90: 7469 655f 6a65 7564 695f 636c 7562 0d0a  tie_jeudi_club..
-00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00002c80: 0a20 2020 2020 2020 2020 2020 2079 6561  .            yea
+00002c90: 7273 2e61 7070 656e 6428 7374 7228 7965  rs.append(str(ye
+00002ca0: 6172 2929 0d0a 2020 2020 2020 2020 2020  ar))..          
 00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 2020 2020 2020 2076 5b27 5241             v['RA
-00002cd0: 4e44 4f4e 4e45 4553 275d 2c20 2020 2020  NDONNEES'],     
-00002ce0: 2020 2020 2020 2023 2072 616e 646f 6e6e         # randonn
-00002cf0: 6565 0d0a 2020 2020 2020 2020 2020 2020  ee..            
-00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00002d20: 5b27 4e6f 6d62 7265 5f73 656a 6f75 7273  ['Nombre_sejours
-00002d30: 275d 2c20 2020 2020 2020 2023 206e 6272  '],        # nbr
-00002d40: 5f73 656a 6f75 7273 0d0a 2020 2020 2020  _sejours..      
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 2020 2020 2030 2c29 2020 2020 2020 2020       0,)        
-00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d90: 2023 206e 6272 5f6a 6f75 7273 5f73 656a   # nbr_jours_sej
-00002da0: 6f75 7273 0d0a 2020 2020 2020 2020 2020  ours..          
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00002df0: 7965 6172 732e 6170 7065 6e64 2873 7472  years.append(str
-00002e00: 2879 6561 7229 290d 0a20 2020 2020 2020  (year))..       
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e20: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
-00002e30: 6566 2066 696c 6c5f 7374 6174 5f79 6561  ef fill_stat_yea
-00002e40: 7228 7965 6172 293a 0d0a 2020 2020 0d0a  r(year):..    ..
-00002e50: 2020 2020 2020 2020 2320 496e 7465 726e          # Intern
-00002e60: 616c 206c 6962 7261 7279 2069 6d70 6f72  al library impor
-00002e70: 7473 0d0a 2020 2020 2020 2020 6672 6f6d  ts..        from
-00002e80: 2043 5447 5f55 7469 6c73 2e43 5447 5f46   CTG_Utils.CTG_F
-00002e90: 756e 632e 4354 475f 7574 696c 6974 7920  unc.CTG_utility 
-00002ea0: 696d 706f 7274 2067 6574 5f73 656a 6f75  import get_sejou
-00002eb0: 725f 696e 666f 0d0a 2020 2020 2020 2020  r_info..        
-00002ec0: 0d0a 2020 2020 2020 2020 7365 6a6f 7572  ..        sejour
-00002ed0: 5f69 6e66 6f20 3d20 6765 745f 7365 6a6f  _info = get_sejo
-00002ee0: 7572 5f69 6e66 6f28 6374 675f 7061 7468  ur_info(ctg_path
-00002ef0: 2c79 6561 7229 0d0a 2020 2020 2020 2020  ,year)..        
-00002f00: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00002f10: 2020 2020 6669 6c65 5f69 6e20 3d20 6374      file_in = ct
-00002f20: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
-00002f30: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
-00002f40: 2753 5441 5449 5354 4951 5545 5327 2920  'STATISTIQUES') 
-00002f50: 2f20 5061 7468 2827 7379 6e74 6865 7365  / Path('synthese
-00002f60: 5f61 6468 6572 656e 742e 786c 7378 2729  _adherent.xlsx')
-00002f70: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00002f80: 2020 2020 6466 203d 2070 642e 7265 6164      df = pd.read
-00002f90: 5f65 7863 656c 2866 696c 655f 696e 290d  _excel(file_in).
-00002fa0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00002fb0: 2020 2073 7461 745f 7965 6172 203d 2073     stat_year = s
-00002fc0: 7461 7479 6561 7228 6466 5b27 4e62 725f  tatyear(df['Nbr_
-00002fd0: 5345 4a4f 5552 5327 5d2e 7375 6d28 292c  SEJOURS'].sum(),
-00002fe0: 2020 2020 2020 2020 2020 2020 2023 206e               # n
-00002ff0: 6272 5f6a 6f75 7273 5f70 6172 7469 6369  br_jours_partici
-00003000: 7061 7469 6f6e 5f73 656a 6f75 7273 0d0a  pation_sejours..
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 2020 2020 2020 2020 2020 2020 2064 665b               df[
-00003030: 2753 454a 4f55 522d 4a4f 5552 275d 2e73  'SEJOUR-JOUR'].s
-00003040: 756d 2829 2c20 2020 2020 2020 2020 2020  um(),           
-00003050: 2020 2320 6e62 725f 7061 7274 6963 6970    # nbr_particip
-00003060: 6174 696f 6e73 5f73 656a 6f75 720d 0a20  ations_sejour.. 
+00002cc0: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
+00002cd0: 6669 6c6c 5f73 7461 745f 7965 6172 2879  fill_stat_year(y
+00002ce0: 6561 7229 3a0d 0a20 2020 200d 0a20 2020  ear):..    ..   
+00002cf0: 2020 2020 2023 2049 6e74 6572 6e61 6c20       # Internal 
+00002d00: 6c69 6272 6172 7920 696d 706f 7274 730d  library imports.
+00002d10: 0a20 2020 2020 2020 2066 726f 6d20 4354  .        from CT
+00002d20: 475f 5574 696c 732e 4354 475f 4675 6e63  G_Utils.CTG_Func
+00002d30: 2e43 5447 5f75 7469 6c69 7479 2069 6d70  .CTG_utility imp
+00002d40: 6f72 7420 6765 745f 7365 6a6f 7572 5f69  ort get_sejour_i
+00002d50: 6e66 6f0d 0a20 2020 2020 2020 200d 0a20  nfo..        .. 
+00002d60: 2020 2020 2020 2073 656a 6f75 725f 696e         sejour_in
+00002d70: 666f 203d 2067 6574 5f73 656a 6f75 725f  fo = get_sejour_
+00002d80: 696e 666f 2863 7467 5f70 6174 682c 7965  info(ctg_path,ye
+00002d90: 6172 290d 0a20 2020 2020 2020 200d 0a20  ar)..        .. 
+00002da0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002db0: 2066 696c 655f 696e 203d 2063 7467 5f70   file_in = ctg_p
+00002dc0: 6174 6820 2f20 5061 7468 2873 7472 2879  ath / Path(str(y
+00002dd0: 6561 7229 2920 2f20 5061 7468 2827 5354  ear)) / Path('ST
+00002de0: 4154 4953 5449 5155 4553 2729 202f 2050  ATISTIQUES') / P
+00002df0: 6174 6828 2773 796e 7468 6573 655f 6164  ath('synthese_ad
+00002e00: 6865 7265 6e74 2e78 6c73 7827 290d 0a20  herent.xlsx').. 
+00002e10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002e20: 2064 6620 3d20 7064 2e72 6561 645f 6578   df = pd.read_ex
+00002e30: 6365 6c28 6669 6c65 5f69 6e29 0d0a 2020  cel(file_in)..  
+00002e40: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002e50: 7374 6174 5f79 6561 7220 3d20 7374 6174  stat_year = stat
+00002e60: 7965 6172 2864 665b 274e 6272 5f53 454a  year(df['Nbr_SEJ
+00002e70: 4f55 5253 275d 2e73 756d 2829 2c20 2020  OURS'].sum(),   
+00002e80: 2020 2020 2020 2020 2020 2320 6e62 725f            # nbr_
+00002e90: 6a6f 7572 735f 7061 7274 6963 6970 6174  jours_participat
+00002ea0: 696f 6e5f 7365 6a6f 7572 730d 0a20 2020  ion_sejours..   
+00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ec0: 2020 2020 2020 2020 2020 6466 5b27 5345            df['SE
+00002ed0: 4a4f 5552 2d4a 4f55 5227 5d2e 7375 6d28  JOUR-JOUR'].sum(
+00002ee0: 292c 2020 2020 2020 2020 2020 2020 2023  ),             #
+00002ef0: 206e 6272 5f70 6172 7469 6369 7061 7469   nbr_participati
+00002f00: 6f6e 735f 7365 6a6f 7572 0d0a 2020 2020  ons_sejour..    
+00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f20: 2020 2020 2020 2020 2064 665b 2753 4f52           df['SOR
+00002f30: 5449 4520 4455 2044 494d 414e 4348 4520  TIE DU DIMANCHE 
+00002f40: 434c 5542 275d 2e73 756d 2829 2c20 2320  CLUB'].sum(), # 
+00002f50: 736f 7274 6965 5f64 696d 616e 6368 655f  sortie_dimanche_
+00002f60: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f80: 2020 2064 665b 2753 4f52 5449 4520 4455     df['SORTIE DU
+00002f90: 2053 414d 4544 4920 434c 5542 275d 2e73   SAMEDI CLUB'].s
+00002fa0: 756d 2829 2c20 2020 2320 736f 7274 6965  um(),   # sortie
+00002fb0: 5f73 616d 6564 695f 636c 7562 0d0a 2020  _samedi_club..  
+00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fd0: 2020 2020 2020 2020 2020 2064 665b 2753             df['S
+00002fe0: 4f52 5449 4520 4849 5645 5227 5d2e 7375  ORTIE HIVER'].su
+00002ff0: 6d28 292c 2020 2020 2020 2020 2020 2020  m(),            
+00003000: 2320 736f 7274 6965 5f68 6976 6572 5f63  # sortie_hiver_c
+00003010: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 6466 5b27 534f 5254 4945 2044 5520    df['SORTIE DU 
+00003040: 4a45 5544 4920 434c 5542 275d 2e73 756d  JEUDI CLUB'].sum
+00003050: 2829 2c20 2020 2023 2073 6f72 7469 655f  (),    # sortie_
+00003060: 6a65 7564 695f 636c 7562 0d0a 2020 2020  jeudi_club..    
 00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003080: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
-00003090: 534f 5254 4945 2044 5520 4449 4d41 4e43  SORTIE DU DIMANC
-000030a0: 4845 2043 4c55 4227 5d2e 7375 6d28 292c  HE CLUB'].sum(),
-000030b0: 2023 2073 6f72 7469 655f 6469 6d61 6e63   # sortie_dimanc
-000030c0: 6865 5f63 6c75 620d 0a20 2020 2020 2020  he_club..       
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 2020 2020 2020 6466 5b27 534f 5254 4945        df['SORTIE
-000030f0: 2044 5520 5341 4d45 4449 2043 4c55 4227   DU SAMEDI CLUB'
-00003100: 5d2e 7375 6d28 292c 2020 2023 2073 6f72  ].sum(),   # sor
-00003110: 7469 655f 7361 6d65 6469 5f63 6c75 620d  tie_samedi_club.
-00003120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003130: 2020 2020 2020 2020 2020 2020 2020 6466                df
-00003140: 5b27 534f 5254 4945 2048 4956 4552 275d  ['SORTIE HIVER']
-00003150: 2e73 756d 2829 2c20 2020 2020 2020 2020  .sum(),         
-00003160: 2020 2023 2073 6f72 7469 655f 6869 7665     # sortie_hive
-00003170: 725f 636c 7562 0d0a 2020 2020 2020 2020  r_club..        
-00003180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003190: 2020 2020 2064 665b 2753 4f52 5449 4520       df['SORTIE 
-000031a0: 4455 204a 4555 4449 2043 4c55 4227 5d2e  DU JEUDI CLUB'].
-000031b0: 7375 6d28 292c 2020 2020 2320 736f 7274  sum(),    # sort
-000031c0: 6965 5f6a 6575 6469 5f63 6c75 620d 0a20  ie_jeudi_club.. 
-000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031e0: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
-000031f0: 5241 4e44 4f4e 4e45 4527 5d2e 7375 6d28  RANDONNEE'].sum(
-00003200: 292c 2020 2020 2020 2020 2020 2020 2020  ),              
-00003210: 2023 2072 616e 646f 6e6e 6565 0d0a 2020   # randonnee..  
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 2020 2020 2073 656a 6f75             sejou
-00003240: 725f 696e 666f 2e6e 6272 5f73 656a 6f75  r_info.nbr_sejou
-00003250: 7273 2c20 2020 2020 2020 2020 2020 2020  rs,             
-00003260: 2320 6e62 725f 7365 6a6f 7572 7320 0d0a  # nbr_sejours ..
-00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003280: 2020 2020 2020 2020 2020 2020 2073 656a               sej
-00003290: 6f75 725f 696e 666f 2e6e 6272 5f6a 6f75  our_info.nbr_jou
-000032a0: 7273 2920 2020 2020 2020 2020 2020 2020  rs)             
-000032b0: 2020 2320 6e62 725f 6a6f 7572 735f 7365    # nbr_jours_se
-000032c0: 6a6f 7572 7320 2020 2020 2020 2020 2020  jours           
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003300: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
-00003310: 726e 2073 7461 745f 7965 6172 0d0a 2020  rn stat_year..  
-00003320: 2020 0d0a 2020 2020 6465 6620 6164 646c    ..    def addl
-00003330: 6162 656c 7328 782c 792c 6f66 6673 6574  abels(x,y,offset
-00003340: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
-00003350: 6920 696e 2072 616e 6765 286c 656e 2878  i in range(len(x
-00003360: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00003370: 2070 6c74 2e74 6578 7428 785b 695d 2c79   plt.text(x[i],y
-00003380: 5b69 5d2b 6f66 6673 6574 2c72 6f75 6e64  [i]+offset,round
-00003390: 2879 5b69 5d2c 3129 2c73 697a 653d 3130  (y[i],1),size=10
-000033a0: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-000033b0: 0a20 2020 2064 6566 2070 6c6f 745f 7374  .    def plot_st
-000033c0: 6174 2879 6561 7273 2c6e 625f 7061 7274  at(years,nb_part
-000033d0: 6963 6970 616e 7473 2c74 6974 6c65 2c6c  icipants,title,l
-000033e0: 6162 656c 5f79 293a 0d0a 2020 2020 2020  abel_y):..      
-000033f0: 2020 706c 742e 6669 6775 7265 2866 6967    plt.figure(fig
-00003400: 7369 7a65 3d28 382c 2036 2929 0d0a 2020  size=(8, 6))..  
-00003410: 2020 2020 2020 636f 6c6f 7273 203d 205b        colors = [
-00003420: 2723 6664 6161 3438 275d 200d 0a20 2020  '#fdaa48'] ..   
-00003430: 2020 2020 2073 697a 655f 6c61 6265 6c20       size_label 
-00003440: 3d20 3230 0d0a 2020 2020 2020 2020 706c  = 20..        pl
-00003450: 742e 6261 7228 7965 6172 732c 6e62 5f70  t.bar(years,nb_p
-00003460: 6172 7469 6369 7061 6e74 732c 636f 6c6f  articipants,colo
-00003470: 723d 636f 6c6f 7273 290d 0a20 2020 2020  r=colors)..     
-00003480: 2020 2070 6c74 2e79 6c61 6265 6c28 6c61     plt.ylabel(la
-00003490: 6265 6c5f 792c 7369 7a65 3d73 697a 655f  bel_y,size=size_
-000034a0: 6c61 6265 6c29 0d0a 2020 2020 2020 2020  label)..        
-000034b0: 6164 646c 6162 656c 7328 7965 6172 732c  addlabels(years,
-000034c0: 6e62 5f70 6172 7469 6369 7061 6e74 732c  nb_participants,
-000034d0: 3129 0d0a 2020 2020 2020 2020 706c 742e  1)..        plt.
-000034e0: 7874 6963 6b73 2872 6f74 6174 696f 6e3d  xticks(rotation=
-000034f0: 3930 290d 0a20 2020 2020 2020 2070 6c74  90)..        plt
-00003500: 2e74 6963 6b5f 7061 7261 6d73 2861 7869  .tick_params(axi
-00003510: 733d 2778 272c 206c 6162 656c 7369 7a65  s='x', labelsize
-00003520: 3d73 697a 655f 6c61 6265 6c29 0d0a 2020  =size_label)..  
-00003530: 2020 2020 2020 706c 742e 7469 636b 5f70        plt.tick_p
-00003540: 6172 616d 7328 6178 6973 3d27 7927 2c20  arams(axis='y', 
-00003550: 6c61 6265 6c73 697a 653d 7369 7a65 5f6c  labelsize=size_l
-00003560: 6162 656c 290d 0a20 2020 2020 2020 2070  abel)..        p
-00003570: 6c74 2e74 6974 6c65 2874 6974 6c65 2c66  lt.title(title,f
-00003580: 6f6e 7473 697a 653d 3138 290d 0a20 2020  ontsize=18)..   
-00003590: 2020 2020 2070 6c74 2e74 6967 6874 5f6c       plt.tight_l
-000035a0: 6179 6f75 7428 290d 0a20 2020 2020 2020  ayout()..       
-000035b0: 2070 6c74 2e73 686f 7728 290d 0a20 2020   plt.show()..   
-000035c0: 200d 0a20 2020 2073 7461 7479 6561 7220   ..    statyear 
-000035d0: 3d20 6e61 6d65 6474 7570 6c65 2827 6163  = namedtuple('ac
-000035e0: 7469 7669 7465 272c 2041 4354 4956 4954  tivite', ACTIVIT
-000035f0: 455f 4c49 5354 290d 0a20 0d0a 2020 2020  E_LIST).. ..    
-00003600: 706c 742e 7374 796c 652e 7573 6528 2767  plt.style.use('g
-00003610: 6770 6c6f 7427 290d 0a20 2020 2079 6561  gplot')..    yea
-00003620: 7273 203d 205b 5d0d 0a20 2020 2073 7461  rs = []..    sta
-00003630: 745f 6469 6320 3d20 7b7d 0d0a 2020 2020  t_dic = {}..    
-00003640: 6164 645f 6d65 6d6f 7279 2873 7461 745f  add_memory(stat_
-00003650: 6469 632c 7965 6172 7329 0d0a 0d0a 2020  dic,years)....  
-00003660: 2020 746f 6461 7920 3d20 6461 7465 7469    today = dateti
-00003670: 6d65 2e64 6174 6574 696d 652e 6e6f 7728  me.datetime.now(
-00003680: 290d 0a20 2020 2079 6561 7273 5f6e 6577  )..    years_new
-00003690: 203d 205b 7374 7228 7965 6172 2920 666f   = [str(year) fo
-000036a0: 7220 7965 6172 2069 6e20 7261 6e67 6528  r year in range(
-000036b0: 3230 3232 2c74 6f64 6179 2e79 6561 722b  2022,today.year+
-000036c0: 3129 5d0d 0a20 2020 2066 6f72 2079 6561  1)]..    for yea
-000036d0: 7220 696e 2079 6561 7273 5f6e 6577 3a0d  r in years_new:.
-000036e0: 0a20 2020 2020 2020 2073 7461 745f 6469  .        stat_di
-000036f0: 635b 7965 6172 5d20 3d20 6669 6c6c 5f73  c[year] = fill_s
-00003700: 7461 745f 7965 6172 2879 6561 7229 0d0a  tat_year(year)..
-00003710: 2020 2020 2020 2020 0d0a 2020 2020 7965          ..    ye
-00003720: 6172 7320 3d20 7965 6172 7320 2b20 7965  ars = years + ye
-00003730: 6172 735f 6e65 7720 2020 0d0a 2020 2020  ars_new   ..    
-00003740: 0d0a 2020 2020 0d0a 2020 2020 6966 2074  ..    ..    if t
-00003750: 7970 6520 3d3d 2027 6e62 725f 6a6f 7572  ype == 'nbr_jour
-00003760: 735f 7061 7274 6963 6970 6174 696f 6e5f  s_participation_
-00003770: 7365 6a6f 7572 7327 3a0d 0a20 2020 2020  sejours':..     
-00003780: 2020 2070 6c6f 745f 7374 6174 2879 6561     plot_stat(yea
-00003790: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
-000037a0: 2020 2020 2020 205b 7374 6174 5f64 6963         [stat_dic
-000037b0: 5b79 6561 725d 2e6e 6272 5f6a 6f75 7273  [year].nbr_jours
-000037c0: 5f70 6172 7469 6369 7061 7469 6f6e 5f73  _participation_s
-000037d0: 656a 6f75 7273 2066 6f72 2079 6561 7220  ejours for year 
-000037e0: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
-000037f0: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-00003800: 7065 2c0d 0a20 2020 2020 2020 2020 2020  pe,..           
-00003810: 2020 2020 2020 2074 7970 6529 0d0a 2020         type)..  
-00003820: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
-00003830: 2773 6f72 7469 655f 6469 6d61 6e63 6865  'sortie_dimanche
-00003840: 5f63 6c75 6227 3a0d 0a20 2020 2020 2020  _club':..       
-00003850: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-00003860: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003870: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
-00003880: 6561 725d 2e73 6f72 7469 655f 6469 6d61  ear].sortie_dima
-00003890: 6e63 6865 5f63 6c75 6220 666f 7220 7965  nche_club for ye
-000038a0: 6172 2069 6e20 7965 6172 735d 2c0d 0a20  ar in years],.. 
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 2074 7970 652c 0d0a 2020 2020 2020 2020   type,..        
-000038d0: 2020 2020 2020 2020 2020 2723 7061 7274            '#part
-000038e0: 6963 6970 616e 7473 2729 0d0a 2020 2020  icipants')..    
-000038f0: 656c 6966 2020 7479 7065 203d 3d20 2773  elif  type == 's
-00003900: 6f72 7469 655f 7361 6d65 6469 5f63 6c75  ortie_samedi_clu
-00003910: 6227 3a0d 0a20 2020 2020 2020 2070 6c6f  b':..        plo
-00003920: 745f 7374 6174 2879 6561 7273 2c0d 0a20  t_stat(years,.. 
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 205b 7374 6174 5f64 6963 5b79 6561 725d   [stat_dic[year]
-00003950: 2e73 6f72 7469 655f 7361 6d65 6469 5f63  .sortie_samedi_c
-00003960: 6c75 6220 666f 7220 7965 6172 2069 6e20  lub for year in 
-00003970: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
-00003980: 2020 2020 2020 2020 2020 2074 7970 652c             type,
-00003990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000039a0: 2020 2020 2723 7061 7274 6963 6970 616e      '#participan
-000039b0: 7473 2729 0d0a 2020 2020 656c 6966 2020  ts')..    elif  
-000039c0: 7479 7065 203d 3d20 2773 6f72 7469 655f  type == 'sortie_
-000039d0: 6a65 7564 695f 636c 7562 273a 0d0a 2020  jeudi_club':..  
-000039e0: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
-000039f0: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
-00003a00: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
-00003a10: 6469 635b 7965 6172 5d2e 736f 7274 6965  dic[year].sortie
-00003a20: 5f6a 6575 6469 5f63 6c75 6220 666f 7220  _jeudi_club for 
-00003a30: 7965 6172 2069 6e20 7965 6172 735d 2c0d  year in years],.
-00003a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a50: 2020 2074 7970 652c 0d0a 2020 2020 2020     type,..      
-00003a60: 2020 2020 2020 2020 2020 2020 2723 7061              '#pa
-00003a70: 7274 6963 6970 616e 7473 2729 2020 0d0a  rticipants')  ..
-00003a80: 2020 2020 656c 6966 2020 7479 7065 203d      elif  type =
-00003a90: 3d20 2772 616e 646f 6e6e 6565 273a 0d0a  = 'randonnee':..
-00003aa0: 2020 2020 2020 2020 706c 6f74 5f73 7461          plot_sta
-00003ab0: 7428 7965 6172 732c 0d0a 2020 2020 2020  t(years,..      
-00003ac0: 2020 2020 2020 2020 2020 2020 5b73 7461              [sta
-00003ad0: 745f 6469 635b 7965 6172 5d2e 7261 6e64  t_dic[year].rand
-00003ae0: 6f6e 6e65 6520 666f 7220 7965 6172 2069  onnee for year i
-00003af0: 6e20 7965 6172 735d 2c0d 0a20 2020 2020  n years],..     
-00003b00: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-00003b10: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00003b20: 2020 2020 2020 2723 7061 7274 6963 6970        '#particip
-00003b30: 616e 7473 2729 2020 0d0a 2020 2020 656c  ants')  ..    el
-00003b40: 6966 2020 7479 7065 203d 3d20 276e 6272  if  type == 'nbr
-00003b50: 5f70 6172 7469 6369 7061 7469 6f6e 735f  _participations_
-00003b60: 7365 6a6f 7572 7327 3a0d 0a20 2020 2020  sejours':..     
-00003b70: 2020 2070 6c6f 745f 7374 6174 2879 6561     plot_stat(yea
-00003b80: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
-00003b90: 2020 2020 2020 205b 7374 6174 5f64 6963         [stat_dic
-00003ba0: 5b79 6561 725d 2e6e 6272 5f70 6172 7469  [year].nbr_parti
-00003bb0: 6369 7061 7469 6f6e 735f 7365 6a6f 7572  cipations_sejour
-00003bc0: 7320 666f 7220 7965 6172 2069 6e20 7965  s for year in ye
-00003bd0: 6172 735d 2c0d 0a20 2020 2020 2020 2020  ars],..         
-00003be0: 2020 2020 2020 2020 2027 4e6f 6d62 7265           'Nombre
-00003bf0: 2064 6520 7061 7274 6963 6970 6174 696f   de participatio
-00003c00: 6e73 2061 7578 2073 c3a9 6a6f 7572 7327  ns aux s..jours'
-00003c10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003c20: 2020 2020 2027 2320 7061 7274 6963 6970       '# particip
-00003c30: 6174 696f 6e73 2061 7578 2073 c3a9 6a6f  ations aux s..jo
-00003c40: 7572 7327 2920 0d0a 2020 2020 656c 6966  urs') ..    elif
-00003c50: 2020 7479 7065 203d 3d20 276e 6272 5f73    type == 'nbr_s
-00003c60: 656a 6f75 7273 273a 0d0a 2020 2020 2020  ejours':..      
-00003c70: 2020 706c 6f74 5f73 7461 7428 7965 6172    plot_stat(year
-00003c80: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00003c90: 2020 2020 2020 5b73 7461 745f 6469 635b        [stat_dic[
-00003ca0: 7965 6172 5d2e 6e62 725f 7365 6a6f 7572  year].nbr_sejour
-00003cb0: 7320 666f 7220 7965 6172 2069 6e20 7965  s for year in ye
-00003cc0: 6172 735d 2c0d 0a20 2020 2020 2020 2020  ars],..         
-00003cd0: 2020 2020 2020 2020 2027 4e6f 6d62 7265           'Nombre
-00003ce0: 2064 6520 73c3 a96a 6f75 7273 272c 0d0a   de s..jours',..
-00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d00: 2020 2723 2073 c3a9 6a6f 7572 7327 290d    '# s..jours').
-00003d10: 0a20 2020 2065 6c69 6620 2074 7970 6520  .    elif  type 
-00003d20: 3d3d 2027 6e62 725f 6a6f 7572 735f 7365  == 'nbr_jours_se
-00003d30: 6a6f 7572 7327 3a0d 0a20 2020 2020 2020  jours':..       
-00003d40: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-00003d50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003d60: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
-00003d70: 6561 725d 2e6e 6272 5f6a 6f75 7273 5f73  ear].nbr_jours_s
-00003d80: 656a 6f75 7273 2066 6f72 2079 6561 7220  ejours for year 
-00003d90: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
-00003da0: 2020 2020 2020 2020 2020 2020 2020 274e                'N
-00003db0: 6f6d 6272 6520 6465 206a 6f75 7273 2073  ombre de jours s
-00003dc0: c3a9 6a6f 7572 7327 2c0d 0a20 2020 2020  ..jours',..     
-00003dd0: 2020 2020 2020 2020 2020 2020 2027 2320               '# 
-00003de0: 6a6f 7572 7320 73c3 a96a 6f75 7227 2920  jours s..jour') 
-00003df0: 2020 2020 2020 20                               
+00003080: 2020 2020 2020 2020 2064 665b 2752 414e           df['RAN
+00003090: 444f 4e4e 4545 275d 2e73 756d 2829 2c20  DONNEE'].sum(), 
+000030a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000030b0: 7261 6e64 6f6e 6e65 650d 0a20 2020 2020  randonnee..     
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 2020 2020 2020 2020 7365 6a6f 7572 5f69          sejour_i
+000030e0: 6e66 6f2e 6e62 725f 7365 6a6f 7572 732c  nfo.nbr_sejours,
+000030f0: 2020 2020 2020 2020 2020 2020 2023 206e               # n
+00003100: 6272 5f73 656a 6f75 7273 200d 0a20 2020  br_sejours ..   
+00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003120: 2020 2020 2020 2020 2020 7365 6a6f 7572            sejour
+00003130: 5f69 6e66 6f2e 6e62 725f 6a6f 7572 7329  _info.nbr_jours)
+00003140: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00003150: 206e 6272 5f6a 6f75 7273 5f73 656a 6f75   nbr_jours_sejou
+00003160: 7273 2020 2020 2020 2020 2020 2020 2020  rs              
+00003170: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00003180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003190: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000031a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000031b0: 7374 6174 5f79 6561 720d 0a20 2020 200d  stat_year..    .
+000031c0: 0a20 2020 2064 6566 2061 6464 6c61 6265  .    def addlabe
+000031d0: 6c73 2878 2c79 2c6f 6666 7365 7429 3a0d  ls(x,y,offset):.
+000031e0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+000031f0: 6e20 7261 6e67 6528 6c65 6e28 7829 293a  n range(len(x)):
+00003200: 0d0a 2020 2020 2020 2020 2020 2020 706c  ..            pl
+00003210: 742e 7465 7874 2878 5b69 5d2c 795b 695d  t.text(x[i],y[i]
+00003220: 2b6f 6666 7365 742c 726f 756e 6428 795b  +offset,round(y[
+00003230: 695d 2c31 292c 7369 7a65 3d31 3029 0d0a  i],1),size=10)..
+00003240: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00003250: 2020 6465 6620 706c 6f74 5f73 7461 7428    def plot_stat(
+00003260: 7965 6172 732c 6e62 5f70 6172 7469 6369  years,nb_partici
+00003270: 7061 6e74 732c 7469 746c 652c 6c61 6265  pants,title,labe
+00003280: 6c5f 7929 3a0d 0a20 2020 2020 2020 2070  l_y):..        p
+00003290: 6c74 2e66 6967 7572 6528 6669 6773 697a  lt.figure(figsiz
+000032a0: 653d 2838 2c20 3629 290d 0a20 2020 2020  e=(8, 6))..     
+000032b0: 2020 2063 6f6c 6f72 7320 3d20 5b27 2366     colors = ['#f
+000032c0: 6461 6134 3827 5d20 0d0a 2020 2020 2020  daa48'] ..      
+000032d0: 2020 7369 7a65 5f6c 6162 656c 203d 2032    size_label = 2
+000032e0: 300d 0a20 2020 2020 2020 2070 6c74 2e62  0..        plt.b
+000032f0: 6172 2879 6561 7273 2c6e 625f 7061 7274  ar(years,nb_part
+00003300: 6963 6970 616e 7473 2c63 6f6c 6f72 3d63  icipants,color=c
+00003310: 6f6c 6f72 7329 0d0a 2020 2020 2020 2020  olors)..        
+00003320: 706c 742e 796c 6162 656c 286c 6162 656c  plt.ylabel(label
+00003330: 5f79 2c73 697a 653d 7369 7a65 5f6c 6162  _y,size=size_lab
+00003340: 656c 290d 0a20 2020 2020 2020 2061 6464  el)..        add
+00003350: 6c61 6265 6c73 2879 6561 7273 2c6e 625f  labels(years,nb_
+00003360: 7061 7274 6963 6970 616e 7473 2c31 290d  participants,1).
+00003370: 0a20 2020 2020 2020 2070 6c74 2e78 7469  .        plt.xti
+00003380: 636b 7328 726f 7461 7469 6f6e 3d39 3029  cks(rotation=90)
+00003390: 0d0a 2020 2020 2020 2020 706c 742e 7469  ..        plt.ti
+000033a0: 636b 5f70 6172 616d 7328 6178 6973 3d27  ck_params(axis='
+000033b0: 7827 2c20 6c61 6265 6c73 697a 653d 7369  x', labelsize=si
+000033c0: 7a65 5f6c 6162 656c 290d 0a20 2020 2020  ze_label)..     
+000033d0: 2020 2070 6c74 2e74 6963 6b5f 7061 7261     plt.tick_para
+000033e0: 6d73 2861 7869 733d 2779 272c 206c 6162  ms(axis='y', lab
+000033f0: 656c 7369 7a65 3d73 697a 655f 6c61 6265  elsize=size_labe
+00003400: 6c29 0d0a 2020 2020 2020 2020 706c 742e  l)..        plt.
+00003410: 7469 746c 6528 7469 746c 652c 666f 6e74  title(title,font
+00003420: 7369 7a65 3d31 3829 0d0a 2020 2020 2020  size=18)..      
+00003430: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
+00003440: 7574 2829 0d0a 2020 2020 2020 2020 706c  ut()..        pl
+00003450: 742e 7368 6f77 2829 0d0a 2020 2020 0d0a  t.show()..    ..
+00003460: 2020 2020 7374 6174 7965 6172 203d 206e      statyear = n
+00003470: 616d 6564 7475 706c 6528 2761 6374 6976  amedtuple('activ
+00003480: 6974 6527 2c20 4143 5449 5649 5445 5f4c  ite', ACTIVITE_L
+00003490: 4953 5429 0d0a 200d 0a20 2020 2070 6c74  IST).. ..    plt
+000034a0: 2e73 7479 6c65 2e75 7365 2827 6767 706c  .style.use('ggpl
+000034b0: 6f74 2729 0d0a 2020 2020 7965 6172 7320  ot')..    years 
+000034c0: 3d20 5b5d 0d0a 2020 2020 7374 6174 5f64  = []..    stat_d
+000034d0: 6963 203d 207b 7d0d 0a20 2020 2061 6464  ic = {}..    add
+000034e0: 5f6d 656d 6f72 7928 7374 6174 5f64 6963  _memory(stat_dic
+000034f0: 2c79 6561 7273 290d 0a0d 0a20 2020 2074  ,years)....    t
+00003500: 6f64 6179 203d 2064 6174 6574 696d 652e  oday = datetime.
+00003510: 6461 7465 7469 6d65 2e6e 6f77 2829 0d0a  datetime.now()..
+00003520: 2020 2020 7965 6172 735f 6e65 7720 3d20      years_new = 
+00003530: 5b73 7472 2879 6561 7229 2066 6f72 2079  [str(year) for y
+00003540: 6561 7220 696e 2072 616e 6765 2832 3032  ear in range(202
+00003550: 322c 746f 6461 792e 7965 6172 2b31 295d  2,today.year+1)]
+00003560: 0d0a 2020 2020 666f 7220 7965 6172 2069  ..    for year i
+00003570: 6e20 7965 6172 735f 6e65 773a 0d0a 2020  n years_new:..  
+00003580: 2020 2020 2020 7374 6174 5f64 6963 5b79        stat_dic[y
+00003590: 6561 725d 203d 2066 696c 6c5f 7374 6174  ear] = fill_stat
+000035a0: 5f79 6561 7228 7965 6172 290d 0a20 2020  _year(year)..   
+000035b0: 2020 2020 200d 0a20 2020 2079 6561 7273       ..    years
+000035c0: 203d 2079 6561 7273 202b 2079 6561 7273   = years + years
+000035d0: 5f6e 6577 2020 200d 0a20 2020 200d 0a20  _new   ..    .. 
+000035e0: 2020 200d 0a20 2020 2069 6620 7479 7065     ..    if type
+000035f0: 203d 3d20 276e 6272 5f6a 6f75 7273 5f70   == 'nbr_jours_p
+00003600: 6172 7469 6369 7061 7469 6f6e 5f73 656a  articipation_sej
+00003610: 6f75 7273 273a 0d0a 2020 2020 2020 2020  ours':..        
+00003620: 706c 6f74 5f73 7461 7428 7965 6172 732c  plot_stat(years,
+00003630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003640: 2020 2020 5b73 7461 745f 6469 635b 7965      [stat_dic[ye
+00003650: 6172 5d2e 6e62 725f 6a6f 7572 735f 7061  ar].nbr_jours_pa
+00003660: 7274 6963 6970 6174 696f 6e5f 7365 6a6f  rticipation_sejo
+00003670: 7572 7320 666f 7220 7965 6172 2069 6e20  urs for year in 
+00003680: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
+00003690: 2020 2020 2020 2020 2020 2074 7970 652c             type,
+000036a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000036b0: 2020 2020 7479 7065 290d 0a20 2020 2065      type)..    e
+000036c0: 6c69 6620 2074 7970 6520 3d3d 2027 736f  lif  type == 'so
+000036d0: 7274 6965 5f64 696d 616e 6368 655f 636c  rtie_dimanche_cl
+000036e0: 7562 273a 0d0a 2020 2020 2020 2020 706c  ub':..        pl
+000036f0: 6f74 5f73 7461 7428 7965 6172 732c 0d0a  ot_stat(years,..
+00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003710: 2020 5b73 7461 745f 6469 635b 7965 6172    [stat_dic[year
+00003720: 5d2e 736f 7274 6965 5f64 696d 616e 6368  ].sortie_dimanch
+00003730: 655f 636c 7562 2066 6f72 2079 6561 7220  e_club for year 
+00003740: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
+00003750: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+00003760: 7065 2c0d 0a20 2020 2020 2020 2020 2020  pe,..           
+00003770: 2020 2020 2020 2027 2370 6172 7469 6369         '#partici
+00003780: 7061 6e74 7327 290d 0a20 2020 2065 6c69  pants')..    eli
+00003790: 6620 2074 7970 6520 3d3d 2027 736f 7274  f  type == 'sort
+000037a0: 6965 5f73 616d 6564 695f 636c 7562 273a  ie_samedi_club':
+000037b0: 0d0a 2020 2020 2020 2020 706c 6f74 5f73  ..        plot_s
+000037c0: 7461 7428 7965 6172 732c 0d0a 2020 2020  tat(years,..    
+000037d0: 2020 2020 2020 2020 2020 2020 2020 5b73                [s
+000037e0: 7461 745f 6469 635b 7965 6172 5d2e 736f  tat_dic[year].so
+000037f0: 7274 6965 5f73 616d 6564 695f 636c 7562  rtie_samedi_club
+00003800: 2066 6f72 2079 6561 7220 696e 2079 6561   for year in yea
+00003810: 7273 5d2c 0d0a 2020 2020 2020 2020 2020  rs],..          
+00003820: 2020 2020 2020 2020 7479 7065 2c0d 0a20          type,.. 
+00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003840: 2027 2370 6172 7469 6369 7061 6e74 7327   '#participants'
+00003850: 290d 0a20 2020 2065 6c69 6620 2074 7970  )..    elif  typ
+00003860: 6520 3d3d 2027 736f 7274 6965 5f6a 6575  e == 'sortie_jeu
+00003870: 6469 5f63 6c75 6227 3a0d 0a20 2020 2020  di_club':..     
+00003880: 2020 2070 6c6f 745f 7374 6174 2879 6561     plot_stat(yea
+00003890: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
+000038a0: 2020 2020 2020 205b 7374 6174 5f64 6963         [stat_dic
+000038b0: 5b79 6561 725d 2e73 6f72 7469 655f 6a65  [year].sortie_je
+000038c0: 7564 695f 636c 7562 2066 6f72 2079 6561  udi_club for yea
+000038d0: 7220 696e 2079 6561 7273 5d2c 0d0a 2020  r in years],..  
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038f0: 7479 7065 2c0d 0a20 2020 2020 2020 2020  type,..         
+00003900: 2020 2020 2020 2020 2027 2370 6172 7469           '#parti
+00003910: 6369 7061 6e74 7327 2920 200d 0a20 2020  cipants')  ..   
+00003920: 2065 6c69 6620 2074 7970 6520 3d3d 2027   elif  type == '
+00003930: 7261 6e64 6f6e 6e65 6527 3a0d 0a20 2020  randonnee':..   
+00003940: 2020 2020 2070 6c6f 745f 7374 6174 2879       plot_stat(y
+00003950: 6561 7273 2c0d 0a20 2020 2020 2020 2020  ears,..         
+00003960: 2020 2020 2020 2020 205b 7374 6174 5f64           [stat_d
+00003970: 6963 5b79 6561 725d 2e72 616e 646f 6e6e  ic[year].randonn
+00003980: 6565 2066 6f72 2079 6561 7220 696e 2079  ee for year in y
+00003990: 6561 7273 5d2c 0d0a 2020 2020 2020 2020  ears],..        
+000039a0: 2020 2020 2020 2020 2020 7479 7065 2c0d            type,.
+000039b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000039c0: 2020 2027 2370 6172 7469 6369 7061 6e74     '#participant
+000039d0: 7327 2920 200d 0a20 2020 2065 6c69 6620  s')  ..    elif 
+000039e0: 2074 7970 6520 3d3d 2027 6e62 725f 7061   type == 'nbr_pa
+000039f0: 7274 6963 6970 6174 696f 6e73 5f73 656a  rticipations_sej
+00003a00: 6f75 7273 273a 0d0a 2020 2020 2020 2020  ours':..        
+00003a10: 706c 6f74 5f73 7461 7428 7965 6172 732c  plot_stat(years,
+00003a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003a30: 2020 2020 5b73 7461 745f 6469 635b 7965      [stat_dic[ye
+00003a40: 6172 5d2e 6e62 725f 7061 7274 6963 6970  ar].nbr_particip
+00003a50: 6174 696f 6e73 5f73 656a 6f75 7273 2066  ations_sejours f
+00003a60: 6f72 2079 6561 7220 696e 2079 6561 7273  or year in years
+00003a70: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00003a80: 2020 2020 2020 274e 6f6d 6272 6520 6465        'Nombre de
+00003a90: 2070 6172 7469 6369 7061 7469 6f6e 7320   participations 
+00003aa0: 6175 7820 73c3 a96a 6f75 7273 272c 0d0a  aux s..jours',..
+00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ac0: 2020 2723 2070 6172 7469 6369 7061 7469    '# participati
+00003ad0: 6f6e 7320 6175 7820 73c3 a96a 6f75 7273  ons aux s..jours
+00003ae0: 2729 200d 0a20 2020 2065 6c69 6620 2074  ') ..    elif  t
+00003af0: 7970 6520 3d3d 2027 6e62 725f 7365 6a6f  ype == 'nbr_sejo
+00003b00: 7572 7327 3a0d 0a20 2020 2020 2020 2070  urs':..        p
+00003b10: 6c6f 745f 7374 6174 2879 6561 7273 2c0d  lot_stat(years,.
+00003b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b30: 2020 205b 7374 6174 5f64 6963 5b79 6561     [stat_dic[yea
+00003b40: 725d 2e6e 6272 5f73 656a 6f75 7273 2066  r].nbr_sejours f
+00003b50: 6f72 2079 6561 7220 696e 2079 6561 7273  or year in years
+00003b60: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00003b70: 2020 2020 2020 274e 6f6d 6272 6520 6465        'Nombre de
+00003b80: 2073 c3a9 6a6f 7572 7327 2c0d 0a20 2020   s..jours',..   
+00003b90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00003ba0: 2320 73c3 a96a 6f75 7273 2729 0d0a 2020  # s..jours')..  
+00003bb0: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
+00003bc0: 276e 6272 5f6a 6f75 7273 5f73 656a 6f75  'nbr_jours_sejou
+00003bd0: 7273 273a 0d0a 2020 2020 2020 2020 706c  rs':..        pl
+00003be0: 6f74 5f73 7461 7428 7965 6172 732c 0d0a  ot_stat(years,..
+00003bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c00: 2020 5b73 7461 745f 6469 635b 7965 6172    [stat_dic[year
+00003c10: 5d2e 6e62 725f 6a6f 7572 735f 7365 6a6f  ].nbr_jours_sejo
+00003c20: 7572 7320 666f 7220 7965 6172 2069 6e20  urs for year in 
+00003c30: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
+00003c40: 2020 2020 2020 2020 2020 2027 4e6f 6d62             'Nomb
+00003c50: 7265 2064 6520 6a6f 7572 7320 73c3 a96a  re de jours s..j
+00003c60: 6f75 7273 272c 0d0a 2020 2020 2020 2020  ours',..        
+00003c70: 2020 2020 2020 2020 2020 2723 206a 6f75            '# jou
+00003c80: 7273 2073 c3a9 6a6f 7572 2729 2020 2020  rs s..jour')    
+00003c90: 2020 2020
```

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_utility.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_Func/CTG_utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,31 +83,14 @@
     
     y = year%100
     c = int(year/100)
     m = month_dict[month]
     if m>10 : y = y-1
 
     return days_dict[(day + int(2.6*m - 0.2) - 2*c + y + int(c/4) + int(y/4))%7] # [1] thm 6.12
-    
-def read_correction_effectifs(year,ctg_path):
-
-    # Standard library imports
-    import os.path
-    from pathlib import Path
-
-    # 3rd party imports
-    import yaml
-    
-    # Reads the default PVcharacterization.yaml config file
-    path_config_file = ctg_path / Path(str(year)) / Path('DATA') / Path('CTG_correction.yaml')
-    with open(path_config_file) as file:
-        memory = yaml.safe_load(file)
-        
-       
-    return memory
 
 def yamlinfo_randos2df(ctg_path,year):
     
     # Standard library imports
     import os
     from pathlib import Path
```

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/GUI_Globals.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/GUI_Globals.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageDivers.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageDivers.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageEffectif.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageEffectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageSorties.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageSorties.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageSynthese.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageSynthese.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageTendance.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/PageTendance.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Page_Classes.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/Page_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Useful_Classes.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/Useful_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Useful_Functions.py` & `CTG_Utils-1.1.6/CTG_Utils/CTG_GUI/Useful_Functions.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/CTG_Utils.egg-info/PKG-INFO` & `CTG_Utils-1.1.6/CTG_Utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG-Utils
-Version: 1.1.5
+Version: 1.1.6
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.5/CTG_Utils.egg-info/SOURCES.txt` & `CTG_Utils-1.1.6/CTG_Utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/LICENSE` & `CTG_Utils-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.5/PKG-INFO` & `CTG_Utils-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG_Utils
-Version: 1.1.5
+Version: 1.1.6
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.5/setup.py` & `CTG_Utils-1.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 install_requires = open(path.join(this_directory, 'requirements.txt'), encoding='utf-8').read().strip().split('\n') 
 
 # This setup is suitable for "python setup.py develop".
 
 setup(name='CTG_Utils',
-      version='1.1.5',
+      version='1.1.6',
       description='A toolbox for ctg statistics analysis',
       long_description=long_description,
       long_description_content_type='text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
```

