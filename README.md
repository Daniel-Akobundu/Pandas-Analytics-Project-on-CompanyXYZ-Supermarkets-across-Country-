NB: This is a template to make documentation process easy. You can remove the `To-Do` notes in your final commit

# Analysis of Supermarket Data for Company_XYZ (Abuja, Lagos & Port-Harcourt Branch)

Company_XYZ owns a supermarket chain across the country with its major branch located in three cities: Abuja, Lagos, and Port-Harcourt with the following product lines: Electronic accessories, Home and Lifestyle, Food and beverages, Sports and travel, Health and beauty, Fashion accessories. Descriptive data manipulation, processing, and analysis were performed on the gathered data from all three branches and insights generated to help understand trends and determine growth. 

# Project Steps

### 1. Loading Datasets
This step includes:
    - Importing Libraries (glob, os, pandas)
    - Using the "glob" library to match csv patterns
    - Combining all three datasets from the company using "pd.concat"  
    - Reading the csv file using "pd.read_csv"

### 2. Data Exploration
This step includes:
    - Import needed Libraries (Numpy, Seaborn, Matplolib)
    - Previewing the data using ".head()" method
    - Acessing the dataset to determine it's shape (".shape()") and number of columns (df.columns)
    - Getting the statistical summary of the dataset using ".describe()" method
    - Checking for missing values using ".isnull()" method
    - Using ".info()" method to further explore the data observing the data types of each column and null values

### 3. DateTime Features
From the data exploration steps we observe the Date & Time columns are object data types and converted them to DateTime data type using "to_datetime()" method. 


### 4. Extracting Features from DateTime
- From the Date column, I extracted and appended the Day, Month and Year of each entry using the ".dt.day", ".dt.month" & ".dt.year" fuctions respectively
- From the Time column, I extracted and appended the Hour of each entry using .dt.hour function
- I used "unique()" to check for unique value in the Hour column.

### 5. Unique Values 
- This step includes checking the unique values in each column using "unique()" method. This is to give further insight on the type and of variables in each column

### 6. Value Count
- This step includes counting the number of unique values using "counts.value()" method

### 7. Aggregation by Groupby
- This step includes aggregation of our dataset by grouping them by City and sorting by gross income.

# Insights

Insights uncovered from visualization of the dataset includes: 

- Sales Record - Port Harcourt has the highesth sales record, follwed by Lagos and then Abuja.

- Payment Method - The most used payment method is Epay, followed closely by cash and then Card.

- Product Line - Fashon accessories are the highest selling product line followed by Food & Beverages.

- Produt Line by Payment Method - This shows that people who by Electronic accessories pay more by cash than any other group. People who buy Fahion, Home & Lifestyle & Health & Beauty Accessories pay more using Epay. Those who buy Food & Beverages pay more using card method

- Product Line by Branch - This Shows that the Lagos branch sold more Home & Lifestyle products compared to any other branch. Abuja branch sold more sport & Travel products compared to other branches and Port Hacourt branch sold more Food & Beverages compared to ther branches.

- Branch Rating  - This shows Lagos and Abuja branch have an qual rating above 7 and Abuja branch have a lower rating below 7.

- Product Line by Total sold based on Gender - This shows thast the stores have a higher number of female customers for all product line except Health & Beauty

- Quantity Sold Vs Unit Price - This shows no solid direct relationship between the quantity of items sold based on their unit price as product with a low unit price have low quantity sold. This implies that the quantity of items sold depends on other factors such as need rather than the unit price


# Future Work

To-Do - Suggest tasks you might include in future work to make this project more robust.

# Standout Section

- Total sold by Hour of Day -  This shows that on the average more goods are sold between 18:00 & 20:00 hour of the day followed by between 12:00 & 14:00 hour.
- Total Sales by Month - This shows that more goods were sold in the 1st Month, then the 3rd Month follows next and finally the 2nd Month.
- Gross income by Product Line - This shows that the highest gross income was brought in by Home & Lifestyle.
- Gross Income by Customer Type - Customers with membership card in the stores bring in more gross income than normal customers.
- Quantity sold per product line by customer type - This shows that members buy more food & beverages and health & beauty products compared to other products and regular customers buy more sports & Travel products.
- Gross Income per month by Product Line - This shows that the stores sold more Food & Beverages, Electronics and Home & Lifestyle products in the first month. the stores sold and all time high record of sports & travel products.

# Executive Summary.

- Included in the repository