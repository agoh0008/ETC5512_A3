**Author:** Alexandra Goh Jia Xin
**Date of release:** 12 May 2023

**Data Description**

The data included in this file was provided by ABC Bank, which is based in the U.S. This dataset covers the full population of loan performance data and contains some demographic variables as well as loan transaction information.


**Files Included**

This data set includes the following files:
- [release-data-Goh-Alexandra.csv] : the full loan performance dataset which is stored in the "data" folder
- [data-dictionary-Goh-Alexandra.csv] : provides detailed information about each variable in the dataset such as variable name, label, item-specific information, type, format, variable number, range (for numeric variables), units/levels, number observed in each unit/level, as well as percentage of population. This is stored in the "data" folder - use this as a reference guide.
- [Goh-Alexandra.Rmd] : this Rmarkdown file contains the codes used to modify the original data and deidentify observations in the dataset. Justification for the steps taken are also provided. This file can later be knitted into a .html file, both of which are located in the "analysis" folder.


**Using the Data**

To use this loan performance dataset, you will need to load the dataset in R by loading the "readr" package and using "read_csv", as the data is provided in .csv format. An example will be "read_csv("release-data-Goh-Alexandra.csv")". Once you have loaded the dataset, you can explore the data (e.g. using the "summary" function to get a summary of the dataset) and create visualizations by using packages such as "ggplot2" (e.g. if you want to visualize the distribution of loan amounts by state). Additionally, you can also use this loan performance dataset for modeling, such as building a predictive model to identify factors that influence loan default.


**Assumptions**

There are a few assumptions to be aware of when using this dataset: 
- The dataset is assumed to represent the full population data of USA borrowers/loans (randomly sampled).
- All states are assumed to have all property types, thereby allowing for the zip code swapping method. 
- The age break "3" used in aggregating customer age is used due to the "30-45" age range currently present in the dataset - if this range increases, a higher age break can be deployed.
- For most age groups (with the exception of a few), income data is approximately symmetric and not highly skewed. We can therefore assume that income distributions within each age group are relatively balanced.

