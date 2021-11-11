# CLTV
Superstore data

Content: Files for data analysis using **Excel, poweBI** & **Alteryx** associated with a study of the following questions:

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

### Q1

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

![image](https://user-images.githubusercontent.com/28995474/141244860-16f4d021-00a6-42ea-8069-548049dac18e.png)

![image](https://user-images.githubusercontent.com/28995474/141244875-8b542d1e-ee0e-4425-80a9-7a1f94a27155.png)

### Q2

Similar workflow pipeline as Q1, is followed here as well. Instead of ‘Cross Tab’, the ‘Summarize’ is used for the analysis, as shown below. 

![image](https://user-images.githubusercontent.com/28995474/141244913-09c72b33-2776-40d9-a169-f9d157854b5a.png)

![image](https://user-images.githubusercontent.com/28995474/141244928-38d7136e-2077-4280-a745-7b7ef468777e.png)

### Additional Question/Insight

Although different types of analysis can be performed to gauge the health of the organization. I am focusing on the financial aspects, more specifically on the profit.
It is interesting to observe that the average profit is proportional to the number of customers in a region. This is surprising as one would expect the average profit should stay constant. It is observed that sales per customer and the profit per item is low in ‘Central’ region (as compared to nationwide average).
There can be multiple reasons for this, namely:
1.	More profitable and usually higher cost items are sold in region with higher customer base.
2.	The popularity of the store can be a driving factor in the regions. Customers can be reluctant to buy a costlier product from a less popular retailer.
I believe actions should be taken to identify the cause of this issue, as it can severely impact the profit margins. Increasing the customer base along with popularizing the store should be prioritized. 
Although not included in the discussion, there are several states in the country where the total net profit is negative.

![image](https://user-images.githubusercontent.com/28995474/141244990-dc5b4e89-50a2-40da-891f-833e7754e1c6.png)





