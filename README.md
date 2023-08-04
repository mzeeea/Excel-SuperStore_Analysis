# Excel-SuperStore_Analysis 🏬
![](image.jfif)

## Business Problem 🕴️
The manager at U.S Superstore presented me with the following business problem:
We're entering a new business year, and based on the company's sales performance in the previous year, are there any specific segments, quarters, months, products, or countries where we should pay more attention to? We need these pointers to perform better and make informed decisions in the coming year.

## Questions to answer ❓

After carefully digesting the demands of the business manager and the data available, I have come up with the following questions to potentially find answers to using the available dataset:
- What is the total sales?
- What is the total profit?
- What is the quantity sold?
- What is the average shipping time?
- What is the total sales margin?
- What is the average shipping window for each shipping mode?
- Which states make the most quantity of sales, sales, and profit?
- Which category and sub-categories makes the most profit?
- Which region makes the most profit?
- What category and sub-category offers the most discount?
- What segment makes the most profit?
- What category makes the most quantity of sales?
- What months have the highest sales and profit?
- What quarter has the highest sales, profit, and profit margin?

## Data Cleaning 🧹
The data we retrieved from the company's database was clean so I had no data cleaning to do, so, to answer the questions we posed and ultimately help the manager, I needed to create a few more columns of data from the columns in the original data:
- I created a _ship time_ column by subtracting the _Ship Date_ from the _Order Date_ column. This gave us the number of days it took to ship a product from the day the product was ordered.
- I also created an _Order Quarter_ column which helps to put the dates products were ordered into the 4 different quarters in a year. To do this, I created a _Order month_ column then used the following formula to get the quarter each month falls into `=IFS(W2<=3, "Q1", W2<=6, "Q2", W2<=9, "Q3", W2<=12, "Q4")`
- I calculated the profit margin using the formula `=(U2/R2)*100` and placed it in the _Profit Margin_ column.
- I lastly created the order month column using the formula `=TEXT(C2, "mmmm")`.

## Data Analysis 🧑‍🔧
I created pivot tables to answer the questions and also answered the Key Perfromance Index questions
![](
