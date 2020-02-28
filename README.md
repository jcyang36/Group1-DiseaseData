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

To plot scatter plot and regression curve on same plot:
1. Import both tables into Tableau
2. Open new sheet. 
3. Go to Data>Edit Relationships...
4. Ensure both tables share a column for days
5. Drag Days and Predicted values into columns and rows
6. Drag Confirmed values into rows.
7. Select confirmed values, right-click, and select dual axis
8. Right click on the right axis and click Synchronize Axes
9. Right click on the right axis and disable Show Header

To plot three curves on same plot:
1. Import three tables into Tableau
2. Open new sheet
3. Select one database. Drag days and predicted cases into columns and rows.
4. Select Measure Values in the Measures pane for that database and drag to Rows. A Measure Values pane should appear.
5. Then select a new database, drag predicted values into the new Measure Values pane.
6. Remove any measure values that are not needed. Remove the predicted cases that were put in Rows in step 3.  
7. Ensure that the type of mark in the "Marks" pane drop down menu is "Area".
8. In Analysis>Stack Marks, select Off.
9. Change the type of mark in the "Marks" pane drop down to "Line".
10. To edit the mark labels, on the right legend bar, right click on each label and select "Edit Aliases".
11. To display the mark labels, right click on each curve line, select "Mark Label", and select "Always show".  
