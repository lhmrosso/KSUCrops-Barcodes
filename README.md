# **KSUCrops-Barcodes**  

Python code to create barcode labels.  
You can adjust the labels to your study.  

**Author:** Luiz Moro Rosso  
**Date:** June 24, 2019    

<br>

1. **Preparing your .csv file**  

Please add a .csv file in the `1. Labels to be done` folder.  
**The .csv file columns and name depends on your label type:**

<br>

## **Plot stakes**  

Label size for plot stakes is 4 x 1 inch. Check how to prepare the information.  
The .csv file needs to be named as `nameofyourlabelset_stake_labels.csv`.  

|*Name:*   |stake_info1      |stake_info2  |stake_info3       |stake_info4     |stake_info5        |stake_info6|
|:--------:|:---------------:|:-----------:|:----------------:|:--------------:|:-----------------:|:---------:|
|*Content:*|*Experiment name*|*Location*   |*Year and student*|*Block or rep.* |*Treatment*        |*Plot code*|
|*Example:*|Azos_Corn        |Ashland (ASH)|2019 MR           |BLOCK A         |Azo-in Full-N Non-S|101        |

<br>

## **Soil sampling** 

Label size for soil samples is 2.25 x 1.25 inch. Check how to prepare the information.  
The .csv file needs to be named as `nameofyourlabelset_soil_labels.csv`.  

|*Name:*   |soil_info1|soil_info2       |soil_info3 |soil_info4  |soil_info5     |soil_info6  |
|:--------:|:--------:|:---------------:|:---------:|:----------:|:-------------:|:----------:|
|*Content:*|*Student* |*Experiment name*|*Location* |*Soil depth*|*Sampling date*|*Main code* |
|*Example:*|Moro Rosso|Azos_Corn        |Ashland, KS|0 - 6 inch  |05 Jun 2019    |ASH AzCr 101|

<br>

## **Biomass sampling**

Label size for biomass sampling is 3 x 2 inch. Check how to prepare the information.  
The .csv file needs to be named as `nameofyourlabelset_biomass_labels.csv`.  

|*Name:*   |biomass_info1        |biomass_info2         |biomass_info3  |biomass_ucode|
|:--------:|:-------------------:|:--------------------:|:-------------:|:-----------:|
|*Content:*|*Sample information* |*Treatment or plant #*|*Sampling date*|*Unique code*|
|*Example:*|ASH_MR AzCr 101 FS V6|Azo-in  Full-N  Non-S |11 Jun 2019    |A00001       |

<br>

## **Plant dry tissue**  

Label size for tissue samples is 2.25 x 1.25 inch. Check how to prepare the information.  
The .csv file needs to be named as `nameofyourlabelset_tissue_labels.csv`.  

|*Name:*   |tissue_info1     |tissue_info2          |tissue_info3|tissue_info4|tissue_info5|tissue_info6   |tissue_ucode |
|:--------:|:---------------:|:--------------------:|:----------:|:----------:|:----------:|:-------------:|:-----------:|
|*Content:*|*Experiment name*|*Location and student*|*Plot code* |*Fraction*  |*Stage*     |*Sampling date*|*Unique code*|
|*Example:*|Azos_Corn        |ASH_MR                |101         |UP          |V6          |11 Jun 2019    |A00001       |

<br>
<br>

2. **Running the code to get the .pdf output**  

Run the cells in the `maincode.ipynb` to generate the labels you want in a .pdf file.  
One .pdf will be created for each .csv, and dropped in the `2. Labels already done` folder.  
