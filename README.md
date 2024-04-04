# temperature-and-herbivory
Exploring how herbivory is impacted by changes in mean annual temperature, aridity and stoichiometry

The supplementary files consist of the following major parts:

1.	FILE “all site summary.xlsx”: Summary data of all the fossil sites used in the study. This is an MS Excel file and has three sheets, namely:

a.	All_sites: This sheet lists various metadata related to each of the 39 fossil sites used in this study. The name of the site is listed as ‘Flora’, and each site has the following data associated with it: Epoch, Latitude Bin, Region, Geographic location, Lat(itude), Long(itude), Depositional.Environment, Age, Age.error, MAT.C (Mean Annual Temperature in degrees C), MAT.Error, MAP.mm.yr (Mean Annual Precipitation in mm), MAP.error, and No.Leaves (number of leaf specimens). 

b.	PEB sites list (Bighorn): This sheet specifically lists the 8 Paleocene-Eocene boundary (PEB) sites from the Bighorn basin along with relevant metadata. These sites are also present in the All_sites tab.

c.	PEB sites list (Hanna): This sheet lists the 2 Hanna Basin sites from the PEB with relevant metadata. 


2.	FOLDER “fossil site herbivory data”: This folder contains the leaf-level herbivory data from all the fossil sites used in this study (including the PEB sites from Hanna Basin) in .csv format. Each file has the following data structure: the first column lists the morphotaxa name of the leaf and the subsequent columns represent whether a particular DT (Damage Type, represented by individual column names) is present (1) or absent (0/NA) in that leaf.


3.	FOLDER “modern site herbivory data”: This folder contains the leaf-level level herbivory data from all the modern sites used in this study in .txt format. “presab_data_HFmatrix” is the data from the three sites in Harvard Forest, “presab_data_LSmatrix” from three sites in La Selva and “presab_data_SERCmatrix” from the three sites in the Smithsonian Environmental Research Center. The quarry number is the name of the site in each file. The rest of the structure is same as fossil data: the second column lists the taxa name for the leaf and the subsequent columns represent whether a particular DT (Damage Type, represented by individual column names) is present (1) or absent (0/NA) in that leaf.


4.	FOLDER “masks for FFGs”: This folder has two files, namely:

a.	“ffgdef_DT.csv”: This file lists which Functional Feeding Group does each DT belong to. Oviposition =0, Skeletonization=1, Surface feeding =2, Galling=3, Hole Feeding=4, Mining =5, Margin Feeding =6,  Piercing and Sucking=7.

b.	“mask_DT.csv”: This file lists whether a given DT is a herbivory damage, a specialized damage, gall or mining damage (T/F). 


5.	FOLDER “N2_fixing_site_level_taxa”: This folder contains 8 files in .csv format corresponding to each of the 8 PEB Bighorn Basin sites. Each file has the same structure: the first column corresponds to a specific morphotaxa and the next column indicates whether it is a N2 fixing plant (1) or not (0). 

6. FILE "Analysis_base.Rmd" contains all the basic code to replicate the analysis.
