## Ms-Excel-Project-One
# **Introduction**

* In this project, a dataset that contains information on bike purchase by diffrent individuals with discrete characteristics is presented.

* Our aim is to clean,transform,analyze and visualize the dataset inorder to draw insights that will guide the bike seller in making informed marketing decisons hence improving his/her bike sales.

# **Purpose of Project**
1). Identify which demographic of our identifiers purchased bikes more compared to their counterparts.

 -This will grant the bike seller insight on which demographic to market more to in order to maximize bike sales.

2). Identify which demographics are underexplored and have a potential to purchase bikes at a high rate.

 -This will guide the bike seller in diverting marketing targets from demographics that are least interested in bike purchase to demographics that have a greater potential to purchase more bikes.
 
 # **Dataset Overview**
* Our dataset is obtained from the open source plattform 'Kaggle' and is accessible to the general public for use.

* At a glance,we observe that the dataset contains 1026 identifiers and 12 variables.

* The variables include:Marital status,Gender,Income,Children,Education,Occupation,Home owner,Cars,Commute,Region,Age,Purchased bike.

* NB:Variables in this case, are the characteristics of identifiers that may have influenced their decision of whether or not to purchase a bike.

# **Dataset Cleaning**
* The first step in data analysis is oftenly data cleaning.In our case,we proceed to data cleaning after data overview.

* Copy and paste the dataset into a new excel sheet,namely,'working sheet'.All our data cleaning and data transformation will take pplace on the working sheet.This allows us to retain our raw data in its original form at the original excel sheet. 

* The first step in data cleaning is removing of any duplicates from the data set.Method: Select whole dataset(ctrl+A) > data> remove duplicates> data has headers.In our data set,26 duplicates exist (and are eliminated) and 1000 unique values remain.

* Check each column for any inconsistancies or in accurracies.

* In our case,no column contains any inconsistecy or inaccurracy.Thus we can now procced to transforming our dataset.

# **Dataset Transformation**
* Check each column for any data type,data value or data format transformation required.

* In 'Marital status' column,replace 'M' data values with 'Married' and also replace 'S' data values with 'Single'.This is because other users may not be familiar with the given abbreviations.It is best to use univerasally known words. Proccess: select column and use the find and replace function available at the home tab. 

* In 'Gender' column,replace 'M' data values with 'Male' and also replace 'F' data values with 'Female'.This is because other users may not be familiar with the given abbrevations.It is best to use commonly known words. Process : select column and use the find and replace function available at the home tab.

* Convert the 'Income' column to cuurrency form. Process: >select column >number > currency. In addittion,make the column data values only whole numbers.

* In the 'Commute' column, replace the '10+ miles' data values with 'More than 10 miles'.This will enable efficient sorting of the data in the column as excel will now  recognize the data values as the greatest in the order. 

* Since the 'Age column' contains alot of distinct data values,it is best to create a new column namely 'Age bracket' , this will ensure that our visualization later on is not crowded. Process: >insert column(right of 'age' column).

* Group the distinct age data values into ranges: 'Old': x>54,'Middle age': X>=31,'Adolescent': x<31.Use the nested IF function to transform the data in 'Age' column i.e =IF(L2>54,"Old",IF(L2>31,"Middle age",IF(L2<31,"Adolescent","Invalid))).Write your code on the 'Age bracket' column first cell,then fill the rest of the column cells with the formula.Thus a new column with only three distict values will have been ccreated thus making visualization easier.

* The other remaining columns do not require any transformation.We can now proceed to analyze the clean and transformed dataset.

# **Dataset Analysis**
* Create a new work sheet namely,'pivot tables'.We shall perfom our all our analysis on this work sheet.Copy all data from the 'working sheet' and paste it ontpo this new sheet.

* In our analysis,we shall answer to the following:
1. Does the level of income of an identifier make a difference in their decision of whether or not to make a bike purchase?
2. Does the commute distance of an identifier make a difference in their decision of whether or not to make a bike purchase?
3. Which age group is more interested in bike purchase?

* For our first analysis,create a pivot table 1 that compares the average income of males versus the average income of females that did or did not purchase a bike.

-Process: >insert pivot table>select dataset from working sheet>rows:Gender>columns:Purchased bike>values:Average of income.

-From our analysis,we note that:

    1. Bikes were purchased by identifiers that have an average higher income compared to the none purchases.This is in both male and female genders.
    
    2. The average income of the male identifiers is higher compared to the average income of the female identifiers.However,the average income of the male identifiers that did not purchase a bike is still higher than the average income of female identifiers that purchased bikes.
    
* For our second analysis,create a pivot table 2 that compares the commute distance of an identifier with thier decision to purchase a bike.

-Process: >insert pivot table>select dataset from working sheet>rows:Commute distance>columns:purchased bike>values:count of purchased bike.Sort commute distance in ascending order.

-From our analysis,we note that:
   
   1. The largest target market lies in the 0-1 miles commute distance identifiers.This is beacuse it contains the highest number of identifiers.
    
   2. As the commute distance increases, the size of the target market decreases.
   
   3. As the commute distance increases,the amount of bike purchases decreases.

* For our third analysis,create a pivot table 3 that compares  age brackets versus thier bike purchase.

-Process: >insert pivot table>select dataset from working sheet>rows:Age Brackets>columns:Purchased bike>values:Count of purchased bike.

-From our analysis,we note that :

    1. The largest target market lies in the 'middle age bracket'(31-49 years).This is because it contains the highest number of identifiers.
    
    2. The 'middle age bracket'(31-49 years) has significantly higher higher bike purchases compared to the 'old'(54 an above years) and 'adolescent'( 30 and below years)           age brackets.
    
-After performing data analysis on the data set and creating pivot tables,we can now proceed to visualizing our findings.
    
# **Dataset Visualization**
* Create a new work sheet namely 'Dashboard'.We shall showcase our data visualization charts on the 'Dahboard' sheet.Remove grid lines from the worksheet and add a header (merge,centre and colour fill the top sheet cells) namely 'BIKE SALES DASHBOARD'.

* From each pivot table created, create corresponding pivot chart.

* For pivot table 1, create a bar chart.For pivot table 2,create a line graph.For pivot table 3,create a bar graph.

* Resize the charts to look presentable.

* Add slicers to the pivort charts i.e Marital Status,Region,Education,Home Owner,Children,Occupation,Cars slicers.Process:Select pivot chart 1>pivot chart tools>analyze>insert slicer>select categories>then add connections to all pivot charts.

* After data analysis and visualization, we can now proceed to deliver reccommendation to the bike seller.

# **Reccommendations To Bike Seller**

    
    
    
    
    
    

    
    
    
    
    
    
    
    








