# CLTV
Superstore data
Contains Excel, poweBI, Alteryx file associated with a data to study the following questions:

1.	In the city of Alexandria, what percent of Sales ($) in the “Second Class” Ship Mode were from the “Corporate” Segment?
2.	What is the most profitable Furniture item in the State of Alabama?


# Solution

## Using Excel:

### Q1

Steps involved:
1.	Firstly, I created a pivot table with 
  a.	Row labels as “Second class” 
  b.	Column labels as “Consumer and Corporate” 
  c.	Within city “Alexandria”, which is set as the variable for filter field in pivot tables.

2.	In the field for ‘Values’ in pivot table, I included ‘Sales’ variable and aggregated the data via summing for the respective categories in the pivot table.

3.	Further, for formatting the numeric data of the table in proper format, I modified the ‘Value field settings’, by showing the values as ‘% of Column total’.
 
Thus, from the table it can be seen that 98.13% of Sales in “Second Class” ship mode were from “Corporate Segment” in the city of Alexandria.
Also attached is a bar plot exhibiting the same information.

![image](https://user-images.githubusercontent.com/28995474/141244512-e7f61820-55b6-4bb2-b4e6-92ecbb4e1e41.png)

![image](https://user-images.githubusercontent.com/28995474/141244454-acbb0e50-8ae3-4c0e-b63f-58172e4f27c5.png)


### Q2.

Similar steps as in Q1, were performed for this problem as well. However, instead of aggregating the data through sum, average values are used, since we are interested in Profit per item.

The most profitable item in Alabama under the ‘Furniture’ catalog is “Tables”. As can be seen, the average profit made over each ‘table’ item sold is 185.36 $.

![image](https://user-images.githubusercontent.com/28995474/141244674-299bd3ec-6eab-4626-9707-2d7271eb563c.png)

![image](https://user-images.githubusercontent.com/28995474/141244689-b9092549-be02-4cb1-928e-ee8136010670.png)

## Using Alteryx

### Q2

In Alteryx, the following steps were performed:
1.	Load the data using ‘Input Data’ tool.
2.	Used ‘Select’ tool to drop the features/columns not needed for analysis. Retained:
  a.	City
  b.	Ship Mode
  c.	Segment
  d.	Sales
3.	Since the analysis is to be performed for only records associated with ‘Alexandria’ city, a ‘filter’ tool is used to select the relevant rows.
4.	A ‘Cross Tab’ tool is used to perform the appropriate grouping and aggregating of variables for analysis.
The output of Cross Tab tool is shown below.


![image](https://user-images.githubusercontent.com/28995474/141244753-3f37bd86-4656-4847-b0e8-7258ea3e2b7f.png)




