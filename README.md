# Pet Supplies with PBI
A DataCamp project: inspecting sales at a pet supply store using Power BI (PBI)
-  Please see the attached files for full project details.  There is a .csv file showing the data used for the PBI visualizations.  As well, there is a pdf showcasing the project instructions.  Below, you can find the actual project analysis.

## Task 1
The original data has 8 columns and 1500 rows. After validation, 1500 rows remained as the only column requested to remove missing values was "repeat_purchases." However, this column has no missing values. And here is a review of all data cleaning performed for each of the 8 columns:
- Product ID: there are 1500 unique identifiers in this column, with no missing data, as expected.
- Category: this column has 6 unique values (Accessory, Equipment, Food, Housing, Medicine, Toys), as expected. There were 25 missing values, which were changed to "Unknown". This left the original 1500 rows intact, but now with 25 "Unknown" values in the category column.
- Animal: this column has 4 categories (Bird, Dog, Cat, Fish), as expected. No missing values were found.
- Size: as expected, this column has 3 unique values (Small, Medium, Large) with no missing items.
- Price: the price column contains product prices with values ranging from 12.85 to 54.16 dollars. There are 150 missing values. Missing values were replaced to the overall median price of $28.07.
- Sales: this column contains values ranging from 286.94 to 2,255.96 dollars. All values are positive and there are no missing values
- Rating: this column contains values ranging from 1 to 10. There were 150 missing values. Missing values were replaced with 0. There were originally no 0's.
- Repeat Purchase: this column contains two values, 0 or 1, respectively. 1 represents repeat customer purchases. There are no missing values in this column. There are 906 repeat purchases (1) and 594 non-repeat purchases (0).

## Task 2
- At a count of 221 repeat purchases, the category with the most repeat purchases is "Equipment" (identified by "1" on the x-axis below). The categories Food, Housing, Medicine, and Toys, are relatively balanced across repeat purchases (with counts 151, 152, 153, 145, respectively). At lower counts of 70 and 14, the categories Accessory and Unknown are less balanced among the other categories, respectively. At a high of 221, the Equipment category is a bit of an outlier.
- For non-repeat purchases (marked as "0" on x-axis), there is much more variation across categories. At a count of 149, Equipment is also the dominant catgory for non-repeat purchases, whereas Food, Housing, Medicine, and Toy counts are much more varied compared to repeat purchases. Similar to repeat purchaes, the Accessory and Unknown categories have much lower counts in non-repeat purchases.
  
![image](https://github.com/user-attachments/assets/bfbb79f8-3ce9-4494-96b8-95929c98b0b5)

## Task 3

The distribution of all sales is represented by the histogram below. The solid green bars represent the count of sales on the left y-axis and total sales amount in US dollars on the x-axis. The right y-axis is corresponds to the blue dotted line graph; the blue dots are an alternative method representing total sales in dollars. The majority of sales occur between 600 and 1500 dollars with a few higher sales above 2,100 dollars. The distribution of sales is mostly a normal distribution with a slight right-skew due to a smaller count of sales happening above 1500 dollars.

![image](https://github.com/user-attachments/assets/ccf49070-1e91-4bde-a266-7a6cd3af8f9e)

## Task 4

Within the scatter plot below, repeat purchases (1) are marked navy blue and non-repeat purchases (0) orange. As mentioned in TASK 1, at a count of 906, there are more repeat purchases than non-repeat, with a count of 594. This is clearly evidenced in the scatter plot which is dominated by blue dots and only a few orange dots scattered among the blue. There tends to be a postive linear correlation between sales and price. This is shown where sales amount steadily increases as the price increases. The number of repeat sales (dark blue) thins out slightly in prices >$40, but still maintains a positive trend. Non-repeat sales (orange) also reflects a positive linear trend as prices increases. Thus, both repeat and non-repeat sales have a postive linear relationsihp with price, with the exception that repeat purchaess greatly outnumber non-repeat purchases.

Beyond this, there is also a grouping of sales on price $28.07 which represents the median value that was imputed over missing values (as described in TASK 1).

![image](https://github.com/user-attachments/assets/091bc042-8c5d-4258-95f5-3cfa3712f3a0)

**REFERENCES**
1) DataCamp Certification Page: https://app.datacamp.com/certification/get-started/associate-data-analyst/overview

