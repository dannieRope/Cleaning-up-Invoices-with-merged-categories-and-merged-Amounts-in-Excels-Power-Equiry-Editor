INTRODUCTION

Possessing data cleaning skills is crucial for any data analyst. While there isn't a single method for data cleaning in MS Excel, it's essential to acquire diverse techniques and approaches for effectively tidying data within the software.

I came across this disorderly dataset online. Feel free to explore it through this link. The untidy data includes an OrderId column, a Category Column with combined categories, and an Amount column with combined values.

The goal of data cleaning is to separate the merged categories and amounts, extracting the values into individual rows within the respective columns.

The primary tool employed for this cleaning process is Microsoft Excel's Power Query, with key features utilized being Transpose, Split Column, and Fill Down.

DATA CLEANING PROCESS

The initial step in the data cleaning process involves importing the unclean data into the Power Query Editor. To accomplish this:

1. Navigate to the Data tab and select "Get Data."
2. Opt for "From File" and then choose "Excel Workbook."
3. Select the appropriate file and click "Transform" to load the data into the Power Query Editor. 

Once the data is loaded into the Power Query Editor, proceed to the Transform tab and select 'Use First Row as Header'. This action designates the first row of the dataset as the column headers.

Next, proceed to transpose the entire dataset by utilizing the transpose feature. This function alters the arrangement, converting rows into columns and columns into rows. You can locate the transpose feature within the Transform tab.

Now, continue by splitting all four columns using the delimiter "|". After the splitting of the four columns, you should expect approximately 13 columns to be created.

Transpose the entire dataset once more using the transpose feature located in the Transform tab. Subsequently, rename the columns as follows:

- Column A: OrderID
- Column B: Category
- Column C: Amount

Choose the OrderID column and proceed to click on "Fill" and then select "Fill Down" to populate the column's rows downwards.

Lastly, modify the data types of the Category column to "Text" and the Amount column to "Currency".  Congratulations, you now have a thoroughly cleaned dataset.
