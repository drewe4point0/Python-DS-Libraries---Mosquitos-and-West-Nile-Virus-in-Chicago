# Mosquitos and West Nile Virus in Chicago

**Table of Contents:**
- [Introduction, Project Overview](#introduction-project-overview)
- [Problem Area, Those Affected, and Impact](#the-problem-area-and-those-affected)
- [Questions to Explore](#questions-to-explore)
- [Data](#data)
- [Notebooks](#notebooks)





## Introduction, Project Overview

The following is an exploratory data analysis (“EDA”) and statistical analysis (linear and logistic) on mosquito populations in suburban Chicago, and their contributions to the spread of West Nile Virus (“WNV”).

It was performed to showcase my fluency with the use of python and its data science (“DS”) libraries.


#### Goal:

The goal of this project is to:
1. Answer the provided questions below using python and it’s DS libraries.


## The Problem Area and Those Affected

West Nile virus (“WNV”) can have serious health consequences for vulnerable populations.  

Furthering our understanding of the presence of this virus in urban areas serves as a worthwhile public health contribution.


## Questions to Explore


### Questions to Explore (EDA)

#### **Part 1 - Basic Data Wrangling**
- **1.** What is the shape of the dataframe?
- **2.** Convert the 'Date' column to have a datetime format.
- **3.** Pick two numeric and two categorical columns: What data they are storing? How are they distributed?
- **4.** Are there any columns that contain duplicate information? If so, remove the redundant columns.
- **5.** Are there any null values in the dataframe? If so, deal with them appropriately.

#### **Part 2 - Basic EDA**
- **1.** Using an appropriate visual, or visuals, explore the relationship between mosquito number and date.

#### **Part 3 - Advanced EDA**
- **1.** Using an appropriate visual, explore the relationship between mosquito species and WNV prevalence.
- **2.** Using an appropriate visual, explore the relationship between the number of mosquitos caught and trap type.
  *Note: This visual should be a different type of visualization than the previous one.*
- **3.** Using an appropriate visual, come up with an additional insight of your choice.
  *Note: This visual should be a different type of visualization than the previous two.*



### Questions to Explore (Stats and Regression Analyses)

#### **Part 1 - Basic Analysis**
- **1.** Convert the `WNV Present` column into a binary column and create dummy variables from the `Trap type` column.
- **2.** What is the average number of mosquitoes for each month? What trends do you notice?

#### **Part 2 - Statistical Analysis**
- **1.** Is there a statistically significant difference between the different mosquito species when looking at the occurrence of West Nile Virus?
- **2.** Which columns are positively correlated with the number of mosquitoes caught? Which columns are negatively correlated? Are these correlations statistically significant?

#### **Part 3 - Advanced Statistical Analysis**
- **1.** Run a linear regression to determine how the independent variables affect the number of mosquitoes caught. Explain your model construction process. Analyze the model and the results and discuss the model’s limitations. This may end up being an iterative process.
  *Note:*
  - *You will likely see a low R^2 value, that is to be expected.*
  - *This dataset does not respond well to performing VIF analysis, so this is not required.*
  - *`WNV Present` must not be one of your independent variables.*
- **2.** Run a logistic regression to determine how the independent variables affect West Nile Virus presence. Explain your model construction process. Analyze the model and the results and discuss the model’s limitations. This may end up being an iterative process.



## Data: 

The data for this project was sourced from the city of Chicago’s [website](https://data.cityofchicago.org/widgets/jqe8-8r6s).  A .csv of the data used can be found in the data folder of this projects GitHub repository.  


### Data Dictionary:

| COLUMN NAME     | DESCRIPTION                                                                                             | DATA TYPE | NOTES                                                                                                                                                       |
|-----------------|---------------------------------------------------------------------------------------------------------|-----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Year            | Year that the WNV test is performed                                                                     | int64     |                                                                                                                                                             |
| Week            | Week that the WNV test is performed                                                                     | int64     |                                                                                                                                                             |
| Address Block   | Address of the location of trap.                                                                        | string    |                                                                                                                                                             |
| Block           | Block number of address                                                                                | int64     |                                                                                                                                                             |
| Trap            | Id of the trap                                                                                         | string    | Some traps are "satellite traps". These are traps that are set up near (usually within 6 blocks) an established trap to enhance surveillance efforts. Satellite traps are post fixed with letters. For example, T220A is a satellite trap to T220. |
| Trap type       | Type of trap                                                                                           | string    |                                                                                                                                                             |
| Date            | Date and time that the WNV test is performed                                                           | string    | Please note that not all the locations are tested at all times. Also, records exist only when a particular species of mosquitoes is found at a certain trap at a certain time. |
| Mosquito number | Number of mosquitoes caught in this trap                                                               | int64     | These test results are organized in such a way that when the number of mosquitoes exceed 50, they are split into another record (another row in the dataset), such that the number of mosquitoes are capped at 50. |
| Mosquito ID     | Id for Mosquito species                                                                                | string    |                                                                                                                                                             |
| WNV Present     | Whether West Nile Virus was present in these mosquitos                                                 | string    |                                                                                                                                                             |
| Species         | Mosquito species                                                                                       | string    |                                                                                                                                                             |
| Lat             | Latitude of trap                                                                                       | float64   |                                                                                                                                                             |
| Lon             | Longitude of trap                                                                                      | float64   |                                                                                                                                                             |



## Notebooks

This project is spread across two notebooks: The initial EDA is performed in the first notebook, and the statistical analyses are performed in the second notebook. 


## Footer
If you have any questions about this project, I would love to speak with you! Please don't hesitate to reach out:

- **Phone:** +1 778 995 7801
- **Email:** [Drewe.MacIver@gmail.com](mailto:drewe.maciver@gmail.com)
- **LinkedIn:** [Drewe MacIver on LinkedIn](https://www.linkedin.com/in/drewe-maciver/)
- **Website:** [DreweItWithData.com](https://www.dreweitwithdata.com)
