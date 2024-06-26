# ETC5512: Assignment 3 - Data Data Deidentification and Modification

This repository includes the work and materials for Assignment 3 of the ETC5512 unit (Wild-caught data).

The assignment focuses on deidentifying a dataset for release as open data, preparing the dataset for computer consumption using the tidyverse, and creating accompanying documentation to facilitate its use.

# Data Origin
The dataset used in this assignment is simulated from the Fannie Mae data set for teaching purposes. It contains loan performance data, including personal information such as names, ages, and other demographic variables, as well as transaction information.

# Files Included

- release-data-Goh-Alexandra.csv: The cleaned and deidentified dataset ready for release.
- data-dictionary-Goh-Alexandra.csv: A detailed data dictionary explaining each variable in the dataset.
- Goh-Alexandra.Rmd: An R Markdown file detailing the data preparation process, including code and justifications for deidentification.
- Goh-Alexandra.html: The HTML version of the R Markdown file, compiled to provide a reproducible report.
- README-Goh-Alexandra.txt: This readme file.

# How to Use the Data

1. **Load the Data**: The deidentified dataset can be loaded using standard R functions, such as read.csv().
2. **Refer to the Data Dictionary**: Use the data dictionary to understand the variables and their transformations.
3. **Review the Analysis**: The R Markdown and HTML files contain the full analysis, including the steps taken for deidentification and the justification for those steps.

## Assumptions

- The data provided is assumed to be the full population data.
- Missing values are represented as NA in the dataset.
- The final decision on variable inclusion or exclusion is based on the need to protect customer privacy while providing useful information for analysis.
