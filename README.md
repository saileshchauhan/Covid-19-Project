# Covid-19 Data Engineering Project using Azure Data Factory
## About Project
In this project I have completed Extracting Data from European Union Center for Disease Control website and eurostat website. Then, loaded the data in Azure Data Lake Gen2. Created pipeline for doing copy and web activity. Afterwards, created pipelines for transforming data as required for Data science team and ML team. For transformation, used Data Flow activity and Azure Data Bricks. Finally, created pipeline for copying processed data to Azure SQL Database made it available for PowerBI Visualization. Created Power BI Dashboard.

## About Data
In this project data has been extracted from European Union center for Disease control website and eurostat website. The data is collected on daily basis. The data is categorised as mentioned below.
* EUROSTAT Data Population by age data.
  * Data was extracted in the gzip format from eurostat website. It contains, 12 year wise columns from 2008 to 2019. First, column contains categorization of population of age group with country code. This, data provided info about percentage representation of each age group in total population.
  * key word :- PC_Y0_14,CZ PC_Y0_14 means age group 0-14. CZ is country code for Czech Republic, in EU.
  * [Link to download population_by_age data](https://github.com/cloudboxacademy/covid19/tree/main/eurostat_data)

* ECDC Data:
  1. FILE NAME :- [cases_deaths.csv]
    * COLUMNS IN CASES_DEATHS.CSV FILES
![image](https://user-images.githubusercontent.com/76868785/130584144-662af75f-69c9-4c8c-95ab-3ef3822cd890.png),
![image](https://user-images.githubusercontent.com/76868785/130584225-a4c5d7ce-4993-4a49-98da-fd2a9c37fbef.png),
![image](https://user-images.githubusercontent.com/76868785/130584367-31838d1f-5cca-45c7-8aa7-40244883825c.png),
![image](https://user-images.githubusercontent.com/76868785/130584444-242a4acc-2fd2-40f2-a9ba-056b1ee3543d.png),
![image](https://user-images.githubusercontent.com/76868785/130584541-58c91966-e1c0-4787-a0a2-2f1d42ee5265.png),
![image](https://user-images.githubusercontent.com/76868785/130584697-5d580d04-ecf1-4161-b0c8-179892ff3f0f.png),
![image](https://user-images.githubusercontent.com/76868785/130584722-7996f65c-60ed-497a-9117-e61788e7559f.png),
![image](https://user-images.githubusercontent.com/76868785/130585009-1a25b7aa-a0d2-400b-ab9f-3dd50b983853.png),
![image](https://user-images.githubusercontent.com/76868785/130585063-9e8ecf47-a93a-40c6-8888-4b3b2db5255b.png), containing data of covid-19 cases and deaths statistics of all countries across world, with source of data collection.
[Link to download cases_deaths.csv](https://github.com/cloudboxacademy/covid19/blob/main/ecdc_data/cases_deaths.csv)
  2. FILE NAME :- [hospital_admission.csv]
    * COLUMNS IN HOSPITAL_ADMISSION.CSV FILES
![image](https://user-images.githubusercontent.com/76868785/130589028-eb599562-a15a-41ab-a167-ab7f138c2e63.png),
![image](https://user-images.githubusercontent.com/76868785/130589053-95ee2f4e-d9e5-4839-8943-c188f2d2e445.png),
![image](https://user-images.githubusercontent.com/76868785/130589079-a48f8b5a-7e59-4b7c-95d0-f29cb4898ca5.png),
![image](https://user-images.githubusercontent.com/76868785/130589105-c272e7ee-4174-4c71-adaf-fa6007dcdf7e.png),
![image](https://user-images.githubusercontent.com/76868785/130589129-7076f1cd-a105-4204-ba1d-78d8c44e1d8d.png),
![image](https://user-images.githubusercontent.com/76868785/130589157-57573c2a-5741-4373-bb5f-8b17306c5c0f.png)
[Link to download hospital_admission.csv](https://github.com/cloudboxacademy/covid19/blob/main/ecdc_data/hospital_admissions.csv)

* LOOKUP Data:
  1. FILE NAME :- [country_lookup.csv]
    * COLUMNS IN COUNTRY_LOOKUP.CSV FILES
![image](https://user-images.githubusercontent.com/76868785/130590939-8f9bdae5-cd92-49d1-b8f1-7e373e75c2b0.png),
![image](https://user-images.githubusercontent.com/76868785/130590957-7c9b227c-760f-4ef7-804c-b082094b7297.png),
![image](https://user-images.githubusercontent.com/76868785/130591203-d3477770-6b71-440f-b037-dcfce270488b.png),
![image](https://user-images.githubusercontent.com/76868785/130591250-f2eef8f3-0a0a-4ac8-bbf5-633c5870e6d8.png),
![image](https://user-images.githubusercontent.com/76868785/130591277-a236da77-305e-4468-baf3-f95f8e8f5c4c.png)
[Link to download Look up data](https://github.com/cloudboxacademy/covid19/tree/main/lookup_data)


## Solution Architecture for Covid-19 Reporting Project
![Screenshot (254)](https://user-images.githubusercontent.com/76868785/130610076-1f11545f-a2c2-4897-93de-9fabb4654fd7.png)

## Project Completed in four sections
* Data extraction and ingestion.
* In Part 1 video Data is ingested from Azure blob storage to Azure Data Lake Gen2.
  * [Data Ingestion Video Part 1](https://youtu.be/6WQCjFInpJE)
* In Part 2 video Data is extracted from ecdc website then ingested to Azure Data Lake Gen2. In csv format
  * [Data Ingestion Video Part 2](https://youtu.be/mvFNW-1b-b8)
* Data Transformation.
  * [Data Transformation using DataFlow Part 3](https://youtu.be/lX8TpXP9OOU)
  * [Data Transformation using DataFlow Part 4](https://youtu.be/nsiPC1tYZ-8)
  * [Data Transformation using DataBricks Part 5](https://youtu.be/waGNV52-gsM)
* Copying Processed Data to Azure SQL Database.
  * [Copying Processed Data to Azure SQL Database 6](https://youtu.be/9IqyS9Xmu8Y)
* Power BI Visualization.
  * [Power BI DashBoard](https://youtu.be/mvFNW-1b-b8)
