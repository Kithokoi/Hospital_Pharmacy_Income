Hospital-Pharmacy-Income-Analysis - power BI
-All columns were formatted correctly using power query--all names and IDs were formatted to text.
-In order to create a data model, dimension tables were derived from the three provided tables. Here are the dimension tables I created:-
1. DimDate derived from the Visits Table containing Date details i.e. month, quarter and year.
2. DimVisits derived from Visits Table containing visit_ID, diagnosis and department.
3. DimDrugs derived from Pharmacy_Transactions table containing Drug_ID, Drug name and Drug category
4. DimPatients derived from Patients Table containing patient_ID, patient_name, Gender, Age

-Two Fact Tables were created:
1.  FactsVisits table
2. FactTransactions table. 

-A star schema was developed where all the dimensions tables were connected to the “FactVisits” table except the “DimDrugs” table which was connected to the “FactTransactions” table. Finally the FactTransactions table was connected to the FactVisits table.

All the relationships were verified before visualizing.

Key Insights:
-Kiambu had the highest total number of diseases diagnosed thus more investment is required in Kiambu county.
-Flu was the most prevalent disease with a total of 56 cases across all counties, followed by typhoid and diabetes respectively. More effort should be put in the management and containment of flu, investment on medications should be increased in the following capitation.
-Kiambu recorded the highest total number of diabetes and typhoid cases while Kisumu recorded highest hypertension cases. In Uasin Gishu, the most prevalent disease was flu. County specific efforts are needed to manage the respective diseases.
-The inpatient department generated the highest revenue at Ksh94,759, followed closely by the emergency department thus increasing inpatient capacity would be necessary as well as equipping the emergency department to be able to handle more cases.
-The age group between 60 to 90 years consume more medications (total of 43-44 medications) compared to the other groups. Patients aged 41 to 50 consume least number of medications (total of 25 medications).
-Diagnosis like flu and hypertension have higher total number of hospital stay days compared to the pharmacy revenue they generate. Malaria has the least number of hospital stay days.
-More effort is required to manage flu and avoid its spread.
-Malaria medications generated the highest revenue for the pharmacy that year. This calls for stocking more malaria drugs
