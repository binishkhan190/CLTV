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


![image](https://user-images.githubusercontent.com/28995474/141244454-acbb0e50-8ae3-4c0e-b63f-58172e4f27c5.png)
