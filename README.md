# Data Analytics Project - Understanding Gender Disparities in Peacekeeping Missions
### An analysis of gender disparities in international peacekeeping missions and their correlation with socio-economic factors.

Welcome to the UN Peacekeeping Contributions Data Analysis project. An end-of-year group project and dissertation completed for the University of Kent's "Year in Data" programme. This repository includes a comprehensive analysis of datasets related to the contributions made by various countries to the United Nations (UN) peacekeeping missions. Upon initial investigation of the data available, we aimed our project at understanding why some countries contribute more personnel to different missions, exploring gender differences in contributions, and analysing various socio-economic characteristics that might influence a country's participation.

## Table of Contents
- [Project Title and Description](#Data-Analytics-Project-Understanding-Gender-Disparities-in-Peacekeeping-Missions)
- [Table of Contents](#table-of-contents)
- [Project Overview](#Project-Overview)
- [Repository Files](#Repository-files)
- [Usage Instructions](#Usage-Instructions)
- [Data Analysis](#data-analysis)
- [Group Contributions](#group-contributions)
- [Individual Contributions](#individual-contributions)
- [License](#license)

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

## Group Contributions
Throughout this project, our group collaborated effectively and worked together to achieve our research objectives. Here are the key group contributions:

- **Project Planning**: We collectively brainstormed and decided on the project's focus, research questions, and objectives.
- **Data Collection and Exploration**: As a team, we acquired and explored the primary dataset on UN peacekeeping contributions, gender breakdowns, and additional characteristics. This involved cleaning and preparing the data for analysis.
- **Literature Review**: We collaboratively conducted a literature review to identify relevant academic research papers and studies related to our topic. This literature review helped us establish a solid theoretical foundation for our analysis.
- **Statistical Analysis**: We divided the statistical analysis into stages and each took responsibility for specific parts:
   - Stage 1: Comparison of total personnel contribution with different characteristics to identify optimal clusters and draw conclusions.
  - Stage 2: Analyzing the percentage of female contributions in relation to various socio-economic characteristics and determining the optimal number of clusters. We collectively drew meaningful conclusions from the results and identified distinct groups.
- **Code Development**: We all contributed to coding tasks such as data cleaning, variable renaming, and ensuring data consistency. Collaboration was key to maintaining code quality and consistency throughout the project.
- **Documentation**: Each team member played a role in documenting our work. This included writing code comments, documenting data cleaning and preprocessing steps, and keeping track of data sources.
- **Editing and Review**: We collectively edited and reviewed the final document, ensuring that it was well-structured, cohesive, and free from errors. We used Google Docs for collaborative editing.

**Individual Contributions**

Here are the specific individual contributions of myself and each group member:

**My Individual Contributions (Corinne Batho-Newton)**:
- Conducted initial exploration of the gender dataset, identifying initial trends over time.
- Programmed a for loop to calculate the average personnel per month for each country.
- Cleaned and preprocessed the secondary characteristics dataset, addressing missing values.
- Calculated the percentage of female personnel and conducted exploratory analysis against socio-economic characteristics.
- Conducted stage 2 of the cluster analysis, comparing the percentage of female contributions to different subgroups of characteristics and drawing meaningful conclusions from the results.

**D. Kaba**:
- Conducted the initial background research on the chosen topic, finding academic papers and ideas for the project.
- Investigated different personnel types within the gender dataset and outlined their contributions to different missions over a decade.
- Ensured data consistency and cleanliness in the additional characteristics dataset.
- Lead the literature review workload to support further analysis, identifying key previous research.
- Conducted stage 1 of the cluster analysis, comparing total personnel contribution with different characteristics and drawing effective conclusions from the results.

**J. Harbour**:
- Renamed columns and conducted initial exploration of datasets.
- Investigated location factors of missions and the geographical proximity of contributing countries.
- Sourced socio-economic and socio-demographic data from the World Bank.
- Worked on the regression modelling part of the statistical analysis, testing different models and checking deviance plots to assess model suitability.
- Assisted with data visualization and project presentation.

Overall, our individual contributions complemented each other, ensuring a comprehensive and well-rounded analysis. Collaboration was essential to the success of this project, with each member bringing unique skills to the team.


## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

