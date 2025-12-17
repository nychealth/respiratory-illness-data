<img width="14484" height="216" alt="image" src="https://github.com/user-attachments/assets/87a58e3e-13ba-422e-895f-6d1956946382" /># NYC Respiratory Illness Data 

This repository contains data on COVID-19 (Coronavirus Disease 2019), influenza, and RSV (respiratory syncytial virus) among New York City residents. 

You can view visualizations of these data on the [NYC Health Department’s Respiratory Illness Data page](https://www.nyc.gov/assets/doh/respiratory-illness-data/index.html#/). These data will also be made available via NYC Open Data.
 
Data are preliminary and subject to change. Information on this page will change as data and documentation are updated. Tables are updated weekly on Thursdays with data through the previous Saturday.

***

This Readme includes:
- How to use this repository
- Key technical notes

***

# How to use this repository

This repository contains CSV (comma separated values) files of data. **To download data**, scroll up to the green button labelled "Code." Clicking this button will start a download of a ZIP file of the entire contents of this repository. Alternatively, you can download a single file. Click on a file you would like to download. Next, click the "Raw" button. Right click and save as a CSV file.

**Questions and custom requests**: We will try to answer questions about the data in this repository as we are able to. If you have a question, please search the Issues to see if it’s already been addressed. Please understand that we might not be able to address all questions in a timely manner. We are not able to accommodate custom data requests placed via Github.  

***

# Key Technical Notes 

## About the data

### Reporting lag

Our data are updated weekly on Thursdays with data through the previous Saturday. These lags are due to standard delays in reporting to the NYC Health Department and are a common limitation of surveillance data. Given the delay, counts in the most recent few days may be artificially small. We delay publishing these data until more reports have come in and the data are more complete.

### Respiratory season

Laboratory-reported cases and deaths are presented by respiratory season and displayed from early September through late August. Traditionally, respiratory season starts at week 40 (in October). Week numbers are defined by the Centers for Disease Control and Prevention to support public health reporting.  

Not all respiratory infections follow a seasonal pattern. Influenza and RSV are seasonal and most prevalent during the fall and winter months. To date, COVID-19 has generally increased during the fall and winter months as well as other times during the year, including the summer.   

### Report date versus date of event

Due to lags common with surveillance data, we receive reports of events (emergency department visits or hospitalizations, laboratory-reported cases, and deaths) that happened on past days. We publish trend data using date of event (date of emergency department visits or hospitalization, date of diagnosis, or date of death), not date of report. This approach may differ from data published by other state and local health departments.

Publishing data by date of event better reflects when things actually happened (e.g., when a person went to the doctor to get tested), as opposed to when the NYC Health Department learned about the event. 

### Changes to reported data

The NYC Health Department updates data for earlier dates after resolving reporting delays. Reported data reflect what we know at the time of publishing on Github, not what occurred in real time. For example, we may find that a person who was originally reported to live in NYC actually resides outside of NYC. This person would be removed from our dataset after their address is updated, and our event count would decrease by one. 

### Trends

Trends in the proportion of emergency department visits and hospitalizations from the emergency department displayed on the webpage represent the percent point change and are calculated as the difference between data from the latest week and data from the previous week. For respiratory illness and COVID-19, changes greater than or equal to 0.01 percentage points compared with the previous week indicate an increasing or decreasing trend. For flu, changes greater than or equal to 0.05 percentage points compared with the previous week indicate an increasing or decreasing trend. For RSV, changes greater than or equal to 0.02 percentage points compared with the previous week indicate an increasing or decreasing trend. 

Trends in laboratory-reported case and death counts displayed on the webpage represent the relative percent change and are calculated by comparing data from the latest week with data from the previous week. Changes greater than or equal to 1% compared with the previous week indicate an increasing or decreasing trend for a given metric. Changes less than 1% are not considered to be increasing or decreasing.

Access to care and other factors can influence the number of emergency department visits as well as laboratory-reported cases received by the NYC Health Department, so these data may not accurately reflect the true amount of illness among NYC residents.

### Differences between City and State values 

Generally, the NYC Health Department and the New York State Department of Health may not have matching numbers for the same metrics, though they report the same general trends. Some reasons for this can include:
- Different data sources for a given metric 
- Different analytical and informatics processes
- Different uses of event date or report date (see above)

## Emergency department visits and hospitalizations from the emergency department 

The NYC Health Department receives near real-time data from all 52 emergency departments in NYC. The emergency departments share diagnosis codes which can be used to identify general respiratory complaints such as cough or illnesses such as pneumonia. This information helps us see trends in illness and care-seeking among NYC residents.

Visits and hospitalizations are mutually exclusive and presented as the percentage of all visits or hospitalizations, respectively, for each week identified with a respiratory illness or a COVID-19, influenza, or RSV diagnosis. For demographic break downs, data are presented as a percent of all emergency department visits or hospitalizations among each group.     

Hospitalizations from the emergency department do not include direct admissions from a doctor's office or outpatient clinic. These hospitalizations differ from hospitalizations previously presented on the COVID-19 data webpage, which identified information on hospitalization status from a number of sources, including Regional Health Information Organizations, NYC public hospitals, non-public hospital systems, remote access to electronic health record systems, the NYC Health Department’s electronic death registry system, and the NYC Health Department's emergency department surveillance system. 

Respiratory illness diagnoses are identified using disease-specific diagnosis codes for general respiratory complaints, such as cough, or illnesses, such as pneumonia. Details on diagnosis codes included for the broad respiratory illness measure can be found here: [CDC_Broad_Acute_Respiratory_.pdf](https://cdn.ymaws.com/www.cste.org/resource/resmgr/pdfs/CDC_Broad_Acute_Respiratory_.pdf). 

Diagnosis codes included for COVID-19, influenza, and RSV are outlined below. 
- **COVID-19**: J12.82 (pneumonia due to coronavirus disease 2019) and U07.1 (COVID-19)
- **Influenza**: J09 (influenza due to certain identified influenza viruses), J10 (influenza due to other identified influenza viruses), and J11 (influenza due to unidentified influenza virus)
- **RSV**: B97.4 (respiratory syncytial virus as the cause of diseases classified elsewhere), J12.1 (respiratory syncytial virus pneumonia), J20.5 (acute bronchitis due to respiratory syncytial virus), and J21.0 (acute bronchiolitis due to respiratory syncytial virus) 

## Respiratory panel results 

The percent of positive test results for each virus is based on the number of tests performed, not the number of people tested. Data are calculated from a subset of respiratory panel tests administered and reported during a given week. These data are collected through passive surveillance and may not be representative of citywide trends.

Other human coronaviruses include NL63, HKU1, OC43, and 229E, and uncategorized human coronaviruses. Results for SARS-CoV-2, the coronavirus that causes COVID-19, are presented separately and not included with the other human coronaviruses. 

## Laboratory-reported cases

The NYC Health Department receives electronic laboratory reports for a number of infectious diseases as required by law in the NYC Health Code. When a specimen is collected from a patient for SARS-CoV-2, influenza, or RSV laboratory testing, the laboratory must report all positive diagnostic test results to the NYC Health Department. Limited demographic information on the person being tested is reported to the NYC Health Department, including name, address, and date of birth.

Differences across respiratory seasons in the volume of positive laboratory reports reflect changes not only in the burden of illness, but also in patient care seeking, testing availability, and laboratory reporting practices. Point-of-care and at-home tests may be conducted in a setting outside of a clinical laboratory; these settings often do not meet the requirements for electronically reporting directly to the NYC Health Department.   

## COVID-19 case definitions

Surveillance case definitions for all notifiable conditions are developed at the national level by the Council of State and Territorial Epidemiologists (CSTE). These standard definitions support public health officials in classifying and counting infections consistently across different states and local jurisdictions. The criteria for reporting a person with COVID-19 infection (“case”) are based on laboratory test results, and include two classifications:

- **Confirmed COVID-19 case**: A person is classified as a confirmed COVID-19 case if they test positive with a molecular (e.g., PCR) test performed at a laboratory
- **Probable COVID-19 case**: A person is classified as a probable COVID-19 case if they meet any of the following criteria with no positive molecular test on record: (a) test positive with an antigen test performed at a laboratory or (b) died and a cause of death is listed as COVID-19 or similar

People who meet the definition of a confirmed or probable COVID-19 case >90 days after a previous positive test (date of first positive test) will be counted as a new case.

## Influenza and RSV case definitions 

The criteria for reporting a person with influenza or RSV infection (“case”) are based on laboratory test results. To be considered a new case of influenza or RSV, an individual would need two positive laboratory test results >90 days apart for influenza or >180 days apart for RSV.  

Clinical laboratories that perform influenza testing on NYC residents may also identify influenza type A, influenza type B, or influenza without specifying type A or B.

## Deaths

### COVID-19 deaths

Citywide all-ages death data are currently only presented for COVID-19 because no national surveillance guidance has been established for influenza- or RSV-related deaths among adults. 

As of April 3, 2023, deaths are counted as a COVID-19 death in NYC if the death certificate lists COVID-19 or an equivalent term as the underlying or a contributing cause of death. 

Pediatric (younger than 18 years of age at time of death) COVID-19 deaths are investigated by the NYC Health Department. These deaths are included in reported data after confirmation that the death is related to COVID-19.     

As of September 1, 2025, pediatric COVID-19 deaths also include children without COVID-19 on the death certificate but who have a positive COVID-19 laboratory test within 30 days of death and for whom investigation has confirmed the death is related to COVID-19.   

The NYC Health Department's Bureau of Vital Statistics is responsible for the registration, analysis, and reporting of all deaths in NYC. More recent data on deaths presented here are provisional, which means that the numbers may change as the NYC Health Department continues to receive and process data. Publishing provisional data allows the NYC Health Department to share data faster, before it is finalized.   

### Influenza-associated pediatric deaths

Deaths among children (younger than 18 years of age) due to suspected or confirmed influenza must be reported to the NYC Health Department . An influenza-associated pediatric death is defined for surveillance purposes as a death resulting from an illness clinically compatible with influenza that is confirmed by an appropriate laboratory test. There should be no period of complete recovery between the illness and death.  Only deaths confirmed to be influenza-associated through investigation are included in reported data.

## Demographic characteristics

The sum of counts by demographic characteristics may not match citywide values due to missing information or cells with counts <5 that are suppressed to protect confidentiality. 

## Residence

Data by borough reflect people's residence at the time of reporting, which is not necessarily the location of diagnosis, hospitalization, or death. 

The data in this repository include patients who reside in congregate facilities, such as correctional facilities and long-term care facilities. While data reported from these facilities may sometimes influence local trends, cases reported from these facilities do not necessarily represent community-based transmission.  

## Age groups

The NYC Health Department reports out data for the following age groups: 0-4, 5-17, 18-44, 45-64, and 65+ years. For data on deaths, age groups 0-4 and 5-17 are collapsed into 0-17 years due to low death counts in this population and to protect confidentiality.

## Race and ethnicity

The NYC Health Department classifies race and ethnicity into the following mutually exclusive categories: Asian/Pacific-Islander, Black/African-American, Hispanic/Latino, and White. Information on people identified as other categories, including Native American/Alaska Native or multi-racial, are not provided in files showing race and ethnicity data due to small counts. The Hispanic/Latino category includes people of any race, and all other categories of race and ethnicity exclude those who identified as Hispanic/Latino.
 
Data received from emergency departments and electronic laboratory reports often lack information on demographic characteristics, such as race and ethnicity. Race and ethnicity information is most complete for COVID-19 cases and deaths, compared with that of case data for other pathogens, due to data augmentation efforts implemented during the COVID-19 pandemic response. 

The NYC Health Department acknowledges this lack of representation in the data is inequitable, and we are committed to developing methods for ensuring more inclusive, equitable representation in the future.  

## Health inequities

Differences in health outcomes among racial and ethnic groups are due to long-term institutional and personal biases against people of color. There is no evidence that these health inequities are due to personal traits. Lasting racism and an inequitable distribution of resources needed for wellness cause these health inequities. These include quality jobs, housing, health care, and food, among others. 

Structural racism — centuries of racist policies and discriminatory practices across institutions, including government agencies, and society — prevents communities of color from accessing vital resources (such as health care, housing, and food) and opportunities (such as employment and education), and negatively affects overall health and well-being.
