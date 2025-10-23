# VaxxVote MetaData

## Data Summary
The datasets were taken from established public health agencies like the WHO and CDC. Specifically, the WHO has a collection of vaccination coverage data (held as percent of the US population who has received a dose of the specific immunization) and the CDC collects a count dataset on Influenza vaccinations. Each is held as time-series data with a year as a key. From the WHO vaccination coverage, we are using two types of immunization: Rubella and  Diphtheria Tetanus Toxoid and Pertussis (DTP) vaccines. Each of these datasets have a variable number of rows depending on when other agencies collected data (i.e. official data may only be collected every couple of years, so 2021 may have multiple entries). Once cleaned, this data only has 45 rows, representative of the 45 years in our sample. From the CDC vaccination count we are using the Influenza vaccine. This dataset has 45 rows representative of our sample.

## Provenance/License
The datasets for vaccination coverage on DTP and Rubella are from the World Health Organization. Prior to collecting the datasets, specific filters on the WHO website itself must be specified in order to obtain the specific dataset needed. These filters include limiting the country only to the United States,the years to 1980-2024, and only including the WHO/UNICEF Estimates of National Immunization Coverage. The vaccination coverage data is obtained by reporting groups such as the WHO/UNICEF Joint Reporting Form on Immunization (JRF) and the WHO/UNICEF Estimates of National Immunization Coverage (WUENIC). The data was officially completed/recorded on July 15, 2025 with data from the years 1980-2024. In terms of licensing, WHO mentions most of its publications are open under CC BY-NC-SA 3.0 IGO, and uses under these licenses don’t need permission, but we have to attribute properly, and can not imply WHO endorsement/use the WHO logo. The dataset for the Influenza vaccination coverage is from the Center for Disease Control and Prevention (CDC). The data was collected from the National Center for Immunization and Respiratory Diseases (NCIRD). In terms of licensing, the CDC website material is public domain and can be freely used/reproduced with attribution and a clear non-endorsement disclaimer; and similar to WHO, individuals can’t endorse or utilize the CDC logo. 

## Ethical Statement
In terms of ethicality, all the vaccination coverage data provided by both WHO and CDC utilize national level aggregate coverage estimates and explicitly prohibit de-anonymization and misrepresentation, so there are no human-subjects or privacy concerns when using them. Additionally, the information regarding presidential candidates, their party affiliation, and years spent in office are public knowledge with no privacy or legality issues. 

## Data Dictionary

### Table 1: U.S. 1st Dose Vaccination Coverage Data (Rubella, DTP)

| **Column** | **Description** | **Potential Responses** |
|-------------|----------------|--------------------------|
| Group | Area level identifier for data collection | Countries, Global |
| Code | Country abbreviation | USA, BRA |
| Name | Full country name | United States of America, Brazil |
| Year | Year of vaccination data collection | 2023, 2024 |
| Antigen | Vaccine antigen abbreviation | DTPCV1, RCV1 |
| Antigen_description | Full vaccine name and dose number | DTP-containing vaccine, 1st dose; Rubella-containing vaccine, 1st dose |
| Coverage_category | Abbreviation of data source organization name | WUENIC, OFFICIAL |
| Coverage_category_description | Full name of data source | WHO/UNICEF Estimates of National Immunization Coverage; Official Coverage |
| Target_number | Target number of doses administered | *(Dropped in cleaning — blank column)* |
| Doses | Number of doses administered | *(Dropped in cleaning — blank column)* |
| Coverage | Percent of the country vaccinated with specified vaccine | 98, 99 |

---

### Table 2: U.S Dose Totals (Influenza)

| **Column** | **Description** | **Potential Responses** |
|-------------|----------------|--------------------------|
| Date | Year range of vaccination data | 1980–1981, 2000–2001 |
| Millions of doses | Number of administered doses in millions | 12.4, 19.8 |

---

### Table 3: U.S. Presidential Data

| **Column** | **Description** | **Potential Responses** |
|-------------|----------------|--------------------------|
| Year | Year president served in office | 1991, 2024 |
| U.S. President | First and last name of U.S. president | Joe Biden, Jimmy Carter |
| Party | Party of serving president that year | democrat, republican |

## Exploratory Data Plots 

### 1. DTP-containing vaccine, 1st dose Coverage Over Time with US Presidential Party
<img width="821" height="449" alt="f_DTP coverage over time" src="https://github.com/user-attachments/assets/9da48b2d-991b-4e8a-9912-9afcd25a69c1" />


### 3. Rubella-containing vaccine, 1st dose Coverage Over Time with US Presidential Party
<img width="828" height="445" alt="f_Rubella coverage over time" src="https://github.com/user-attachments/assets/31e6d458-441c-436c-92bd-2737f4da54f2" />

### 4. Influenza Vaccine Doses Distributed Over Time with US Presidential Party
<img width="824" height="449" alt="f_influenza dosage over time" src="https://github.com/user-attachments/assets/21ab9e21-0cac-43ef-b70c-f194ba816828" />

