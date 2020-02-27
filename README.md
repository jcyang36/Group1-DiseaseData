# Group1-DiseaseData

This project studies the occurences of the Coronavirus outside of China from Feb 3 to Feb 23

Dates:
Feb 3
Feb 7
Feb 11
Feb 15
Feb 19
Feb 23

Source: https://www.who.int/emergencies/diseases/novel-coronavirus-2019/situation-reports/


Steps: 

1. Import pdf to Tableau
2. Export Data to CSV
3. Remove extra columns due to separators (1s)
4. Remove Empty Rows
5. Order columns to be consistent
6. Make column names consistent
7. Remove numbers in parentheses
8. Remove row for the cases in China
9. Make country names consistent
10. Upload to Github

Determine Model to Use for Forecast
Use model functions from https://towardsdatascience.com/modeling-functions-78704936477a
1. Exponential
2. Polynomial (degree 3)
3. Polynomial (degree 4)--NOT ACCURATE (End behavior is negative)
4. Power

Perform Regression when crushing growth (taking the data from a country to be static):
Results show that taking out the country with the highest growth (Korea) has a bigger effect than taking out the country with highest count (International Conveyance from Japan).


