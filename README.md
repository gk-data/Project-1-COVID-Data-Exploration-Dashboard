# Global COVID-19 Data Exploration and Dashboard Visualization 

![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Microsoft SQL Server](https://img.shields.io/badge/Microsoft_SQL_Server-8080cc?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![Tableau Public](https://img.shields.io/badge/Tableau_Public-854442?style=for-the-badge&logo=tableau-public&logoColor=white)
![Microsoft Office](https://img.shields.io/badge/Microsoft_Office-D83B01?style=for-the-badge&logo=microsoft-office&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)
![Microsoft Word](https://img.shields.io/badge/Microsoft_Word-2B579A?style=for-the-badge&logo=microsoft-word&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)


## [Full Report](https://github.com/gauravkamble-insights/COVID-Data-Exploration-Dashboard/blob/main/report/Global%20Pandemic%20Impact%20Analysis.pdf)


## Overview
This project provides a comprehensive analysis of the global COVID-19 pandemic by combining SQL-based data exploration with interactive Tableau visualizations. By processing approximately 85,000 records, the project uncovers critical insights into infection rates, mortality probabilities, and vaccination rollouts across various countries and continents. The end goal was to transform raw data from Our World in Data into a professional dashboard that highlights the geographic and temporal impact of the virus.


## Dashboard Preview
The following dashboard was created in Tableau to provide a multi-dimensional view of the pandemic's progression, including global totals and regional infection maps.
<img width="1919" height="1126" alt="Dashboard" src="https://github.com/user-attachments/assets/edf1b545-f3ae-4b0a-8f77-be1e546a63cf" />


## Dataset
The data is sourced from **Our World in Data** and covers the period from early 2020 through early 2021. The analysis utilizes two primary datasets:  
- **CovidDeaths:** Includes total cases, new cases, total deaths, and population figures.
- **CovidVaccinations:** Tracks testing and vaccination progress, including new vaccinations per day.


## Database
A SQL database titled PortfolioProject was established in SQL Server Management Studio (SSMS) to manage approximately 85,000 records. The data is organized into two main tables: CovidDeaths and CovidVaccinations, which are joined on location and date for integrated analysis.


## Data Exploration (SQL)
The raw data underwent several stages of preparation:  
- **Initial Cleaning:** Performed in Excel to reformat columns and separate deaths and vaccinations into distinct workbooks for database ingestion.
- **Joins:** Linking death and vaccination tables on location and date.  
- **Data Transformation:** SQL queries utilized CAST and CONVERT to change data types (e.g., converting nvarchar to int) for accurate mathematical calculations.  
- **Advanced Querying:** Used CTEs (Common Table Expressions) and Temp Tables to calculate complex metrics like rolling vaccination percentages that could not be achieved through simple queries.  
- **Optimization:** Created Views to store processed data for efficient connection to visualization tools like Tableau.


## Key Insights:
**Global Pandemic Summary:** A high-level overview of global cases (150.5 million) and deaths (3.18 million), with a global death percentage of ~2.11%.  
<img width="413" height="51" alt="Global numbers" src="https://github.com/gauravkamble-insights/COVID-Data-Exploration-Dashboard/blob/main/assets/Global%20numbers.png" />


**Infection Rate Comparisons:** Identifying countries with the highest infection rates relative to their population, such as Andorra (17.1%) and Montenegro (15.5%).  
<img width="676" height="402" alt="Infected %" src="https://github.com/gauravkamble-insights/COVID-Data-Exploration-Dashboard/blob/main/assets/Infected%20%25.png" />

**Top Countries by Death Count:** Tracking mortality leaders, showing the United States with the highest death count (576,232) during the study period.  
<img width="319" height="401" alt="Death Count" src="https://github.com/gauravkamble-insights/COVID-Data-Exploration-Dashboard/blob/main/assets/Death%20Count.png" />

**Mortality by Continent:** Breaking down total deaths by region to show the impact on North America, South America, and Asia.  
<img width="311" height="176" alt="Continents Death count" src="https://github.com/gauravkamble-insights/COVID-Data-Exploration-Dashboard/blob/main/assets/Continents%20Death%20count.png" />

**Vaccination Rollout Tracking:** Utilizing Windows Functions (PARTITION BY) to create a rolling count of vaccinations by location and date.


## Visualization Workflow (Tableau)
Due to the limitations of **Tableau Public**, which does not connect directly to SQL databases, SQL views were created and exported to Excel to power the visualizations.
- **Geographic Mapping:** Used to visualize the percentage of the population infected per country.  
- **Time Series & Forecasting:** Leveraged 12 months of historical data to predict future infection trends using Tableau's built-in forecasting tools.


## Tools Used for this project

**Excel:** For initial data cleaning and formatting.

**SQL Server (SSMS):** For advanced data querying, transformation, and exploration.

**Tableau:** For creating interactive dashboards and geographic maps.


## Conclusion
This project demonstrates a full-cycle data analysis workflow, moving from raw, messy data to refined SQL insights and finally to a professional-grade visual dashboard. By leveraging advanced SQL functions and Tableau's visualization suite, the analysis uncovers the varying degrees of the pandemic's impact across the globe, providing a clear, data-driven perspective on public health trends.


## Author
- <b>©2026 Gaurav Kamble.  
- <b>[LinkedIn](https://www.linkedin.com/in/gaurav-kamble/)</b>
- <b>[Tableau Public](https://public.tableau.com/app/profile/datagaurav/vizzes)</b>
- <b>[Kaggle](https://www.kaggle.com/justgk)</b>
- <b>[Email](mailto:gauravksse@gmail.com)</b>

