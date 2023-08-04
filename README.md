# Make_Up
Analysis of sales data, for sales made by 9 salespersons, over a year. Bar graph of sales made by each person, in each product category (eye liner, foundation, lip gloss, lipstick, mascara), was made using Python. User can input the year he wants to create the graph for, from among the six years 2004, 2005, 2006, 2020, 2021, 2022. The code will check if the user provides valid input from among these 6 years. If the user provides invalid input, the code will exit.

The file MakeUP_IVY_No_VBA_extra_data.xlsx contains an example of a Dynamic Chart in the sheet "Dynamic_Chart". For some background, the data in Sheet1 contains data on 6 salespersons for year 2022. The data contains data on 8 salespersons for the year 2021. The data contains data on 7 salespersons for the year 2020. Once you select the year from the dropdown in Cell C4, the chart will automatically update. Please scroll the sheet if the graph does not appear to be updating due to lack of memory.

The file 'MakeUP_IVY_conditional_formatting_use.xlsx' contains an example of conditional formatting using complex Excel formula. For some background, the file contains data on sales made by different salepersons, for 5 differents products (eye liner, foundation, lip gloss, lipstick, mascara), for the years 2004, 2005, 2006, 2020, 2021 and 2022. There is a gap between the years 2007 and 2019, where there is no data. The business objective is to check whether the amount of sale, given in column I (Total), for a particular product (column F), on a particular date (column C), is less than the average amount of sale (Total) occurring for that particular product over the past 3 months (excluding the current month). If it is less, then that cell will be highlighted in red. So if the Date given in col. C is 07-11-2004, we calculate the average over all transactions for that particular product occurring between 01-08-2004 and 31-10-2004. This is achieved by sorting the data first by Year (col. D) and then by month (col. E), and then using a custom AVERAGEIFS formula for conditional formatting on col. I. Of course, the formula cannot be applied for the months of January, February and March 2004 and the months of January, February and March 2020 because data for earlier months in 2003 and 2019 are not present. I have kept the result of the AVERAGEIFS formula hidden in Column L, for reference. The formula box of conditional formatting does not refer to column L. Whenever the average value of past 3 months is greater than the cell value in col. I (for the cells where the formula is applicable), that cell will be highlighted in red.
