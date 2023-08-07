# INTRODUCTION

![clean](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/969fca3a-5143-40a9-b395-f25c667efb47)


Possessing data cleaning skills is crucial for any data analyst. While there isn't a single method for data cleaning in MS Excel, it's essential to acquire diverse techniques and approaches for effectively tidying data within the software.

I came across this disorderly dataset online. Feel free to explore it through this [link](https://foresightbi.com.ng/microsoft-power-bi/dirty-data-samples-to-practice-on/). The untidy data includes an OrderId column, a Category Column with combined categories, and an Amount column with combined values.

![DATASET](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/54c03274-f3c6-48f0-9d9a-76907097c7df)


The goal of data cleaning is to separate the merged categories and amounts, extracting the values into individual rows within the respective columns.

The primary tool employed for this cleaning process is Microsoft Excel's Power Query, with key features utilized being Transpose, Split Column, and Fill Down.

## DATA CLEANING PROCESS

The initial step in the data cleaning process involves importing the unclean data into the Power Query Editor. To accomplish this:

1. Navigate to the Data tab and select "Get Data."
2. Opt for "From File" and then choose "Excel Workbook."
3. Select the appropriate file and click "Transform" to load the data into the Power Query Editor.

   ![getdata](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/7d7b6a00-635e-48c1-84b2-8e08dac40d84)


Once the data is loaded into the Power Query Editor, proceed to the Transform tab and select 'Use First Row as Header'. This action designates the first row of the dataset as the column headers.

![firstrowasheader](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/2c3946ba-5adf-450f-8a7c-da930a5a76d8)


Next, proceed to transpose the entire dataset by utilizing the transpose feature. This function alters the arrangement, converting rows into columns and columns into rows. You can locate the transpose feature within the Transform tab.

![TRANSPOSE](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/9cf8d6cd-6261-47bd-9996-a4c3263f10a8)


Now, continue by splitting all four columns using the split column feature and choosing the delimiter "|". After the splitting of the four columns, you should expect approximately 13 columns to be created.

![SPLIT](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/01ef647c-ebcf-48f2-9669-1cd8e6c11571)


Transpose the entire dataset once more using the transpose feature located in the Transform tab. Subsequently, rename the columns as follows:

- Column A: OrderID
- Column B: Category
- Column C: Amount

![transposeagain](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/5829d246-37c2-4704-a52d-c7a77e1ad8be)


Choose the OrderID column and proceed to click on "Fill" and then select "Fill Down" to populate the column's rows downwards.

![fill down](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/e2c0b9a3-9882-4495-8a0b-b879541dc2a7)


Lastly, modify the data types of the Category column to "Text" and the Amount column to "Currency".  

![Final](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/dcb7b388-817b-4ece-992d-e024a9a4a49c)


Congratulations, you now have a thoroughly cleaned dataset.

![thanks](https://github.com/dannieRope/Cleaning-up-Invoices-with-merged-categories-and-merged-Amounts-in-Excels-Power-Equiry-Editor/assets/132214828/2f120a5e-b733-4260-804d-b7f072cad510)
