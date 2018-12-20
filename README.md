# CIBC_Hackathon
## Problem
Teams were provided an insurance claims data set and asked with finding fraudulent claim records and medical providers.  The claims data (claims_final.csv) contains 1 year of sample medical claims.
The claims data format is a comma-separated file with the following columns
1. Patient Family ID
2. Patient Family Member ID
3. Provider ID
4. Provider Type
5. State Code
6. Date of Service
7. Medical Procedure Code
8. Dollar Amount of Claim

Some definitions:
1. Unique medical providers (i.e. doctors) are identified by a provider id.
2. The type of provider is identified by the provider type (i.e. medical specialty)
3. The state code identifies which state the provider practices in
4. Unique patient families are identified by a family id
5. A unique patient is identified by combination of family id and family member id.
6. A unique doctor visit is identified by a unique combination of columns 1,2,3,6 from the above list.

## Tasks
Return two csv files with the doctor visits and doctors ranked according to degree of outlying behavior.
 
File 1 – A CSV file Outlying providers containing all provider records sorted by Outlier Rank.
1)     Provider Id
2)     Outlier Rank (1 being the worst outlier)
 
File 2 – A CSV file Outlying visits containing the top 100 outlying visits for each provider type. Entries sorted based on outlier Rank first and then provider type second.
1)     Family ID
2)     Family Member ID
3)     Provider ID
4)     Date of Service
5)     Provider Type
6)     Outlier Rank (1 being the worst outlier)

## Notes on the code
Our team consisted of five students including me. I wrote CIBC_AI_scratch_work.ipynb and File2.ipynb while explore.ipynb was written by my teammates. File2.ipynb was used as a backup in case another approach had failed to complete task 2.
You may have to modify the file path of claims_final.csv to run the code.