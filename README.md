# Data Analytics Project - Understanding Gender Disparities in Peacekeeping Missions
### An analysis of gender disparities in international peacekeeping missions and their correlation with socio-economic factors.

Welcome to the UN Peacekeeping Contributions Data Analysis project. An end-of-year group project and dissertation completed for the University of Kent's "Year in Data" programme. This repository includes a comprehensive analysis of datasets related to the contributions made by various countries to the United Nations (UN) peacekeeping missions. Upon initial investigation of the data available, we aimed our project at understanding why some countries contribute more personnel to different missions, exploring gender differences in contributions, and analysing various socio-economic characteristics that might influence a country's participation.

## Table of Contents
- [Project Title and Description](#Data-Analytics-Project-Understanding-Gender-Disparities-in-Peacekeeping-Missions)
- [Table of Contents](#table-of-contents)
- [Project Overview]
- [Repository Files]
- [Usage Instructions]
- [Data Analysis]
- [Personal Contributions]
- [Skills Demonstrated]
- [License]

## Project Overview

The United Nations (UN) deploys police and military personnel from over 100 countries to maintain international peace and security. These personnel carry out missions aimed at protecting populations and creating safer environments. This project focuses on analyzing data to understand why some countries contribute more personnel to UN peacekeeping missions than others.

Previous research indicates that some countries participate in peacekeeping operations for self-interest, political, and economic reasons. We explore how a country's wealth correlates with its contributions to peacekeeping missions and investigate the impact of gender equality on personnel contributions. Our analysis revealed several patterns related to personnel contributions, including the influence of factors like population, GDP, military expenditure, and gender demographics.

### Types of Analysis Conducted
**1. Exploratory Data Analysis:** We explore the data to gain initial insights and identify patterns related to personnel contributions.
**2. Cluster Analysis:** We group countries based on socio-economic and socio-demographic variables to identify common characteristics among countries with high and low personnel contributions.
**3. Regression Analysis:** We build regression models to predict the number of personnel a country contributes to UN peacekeeping missions based on various factors.

For the full dissertation and detailed analysis, please refer to the [./MA5957_Year_in_Data_Analytics_Project_Dissertation.pdf]

## Data Sources
We used 2 primary datasets from the UN Peacekeeping open data portal, and a secondary dataset of socioeconomic characteristics of countries from the World Bank Data.

- Peacekeeping Tropp and Police Contributions Data: [Link to Dataset](https://peacekeeping.un.org/en/data-troop-and-police-contributions)
- Women & Peacekeeping Data: [Link to Dataset](https://peacekeeping.un.org/en/women-peacekeeping)
- Socio-Economic Characteristics Data: [Link to Dataset](https://peacekeeping.un.org/en/data-troop-and-police-contributions)

## Repository Files
The repository contains several files relevant to the data analysis and presentation of findings.

1. [CountryByYear.csv](./CountryByYear.csv)
   - This file contains data on average monthly contributions per country, broken down by gender and total personnel. It was calculated in the R code using a for loop.
     
2. [Dataset_EDA_UN_Peacekeeping.Rmd](./Dataset_EDA_UN_Peacekeeping.Rmd)
   - An extensive R code file containing all of the analysis, data manipulation and calculations performed on the datasets.

3. [Gender.csv](./Gender.csv)
   - Obtained from the United Nations Peacekeeping open data portal, this dataset titled 'Gender' provides a comprehensive overview of contributions to missions from 146 countries since July 2002. It includes data on personnel contributions by each country per month, specifying the type of personnel contributed, their gender, and the mission they were assigned to. This dataset allowed us to dive deep into gender and country-based contributions.

4. [MA5957_Year_in_Data_Analytics_Project_Dissertation.pdf](./MA5957_Year_in_Data_Analytics_Project_Dissertation.pdf)
   - This PDF document is our group's final write-up. It presents and discusses the results of our analysis and outlines the methodology we followed throughout the project.
     
5. [Rank.csv](./Rank.csv)
   - Another primary dataset from the UN Peacekeeping open data portal. Ranks the total contributions of 122 countries, broken down into Female and Male personnel.

6. [characteristics.csv](./characteristics.csv)
   - To investigate the relationship between country characteristics and UN peacekeeping contributions, we created this dataset. It matches World Bank data with relevant countries for each year between 2010 and 2020. It contains data on the number of male and female personnel contributed per year per country, as well as the total number of personnel contributed. Additionally, it calculates the percentage of female contributions, which was useful for further analysis techniques.

## Usage Instructions
To replicate this analysis, or expand it with your own further additions, follow these steps:
1. **Clone the Repository**: 
   - Clone this repository to your local machine using `git clone [https://github.com/corinnee/UN_Peacekeeping_Analytics]`.
2. **Navigate to the Analysis Script**:
   - Locate the `/Dataset_EDA_UN_Peacekeeping.Rmd` file within the cloned repository.
3. **Open in R Studio or Preferred IDE**:
   - Open the `Dataset_EDA_UN_Peacekeeping.Rmd` file in your preferred IDE such as R Studio.
4. **Install Required Libraries and Packages**:
   - Ensure you have the necessary R packages installed by running any package installation commands provided within the script. This can usually be done using the `install.packages("package_name")` function.
5. **Set Working Directory**:
   - Confirm that your working directory is set to the location of the source file. You can set the working directory in R using `setwd("path/to/working/directory")`.
6. **Run the Code Scripts**:
   - Execute the code scripts within the `Dataset_EDA_UN_Peacekeeping.Rmd` file in sequential order. This will perform the exploratory data analysis and generate the results.
     
**Note**: Ensure you have R and RStudio (or your preferred R IDE) installed on your local machine before proceeding with the analysis.

   
