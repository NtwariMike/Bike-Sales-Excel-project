
# Bike Sales Analysis

## Table of content
 - [Project Overview](#project-overview)
 - [Data sources](#data-sources)
 - [Tools](#tools)
 - [Data Cleaning](#data-cleaning)
 - [Exploratory Data Analysis](#exploratory-data-analysis)
 - [Data Analysis](#data-analysis)
 - [Results](#results)
 - [Recommendations](#recommendations)
 - [Limitations](#limitations)
 - [Sharing](#sharing)
### Project Overview

 This data analysis project, iams to provide insights on factors that lead to customers purchasing our bikes or not. By analyzing various factors such as Average income, age group and region. We Will be able to identify trends and provide data-driven recommendations.

Bike-sales Report

 ### Data sources

Bike Sales: The primary data set i used for this activity is " Bike-sales.csv" file, containing detailed information about customers and if purchased the bike or not

### Tools
#### Excel
- Data Cleaning: (Filters, Conditional formatting, Removing Duplicates, IFS)
- Data analysis: (Pivot tables)
- Data Visualization: (Column charts, Line charts)

### Data Cleaning

In the initial data preparation phase, we performed the following,
1. I applied filters to help understand data and easily navigate through data
2. I applied conditional formatting for duplicate values in the ID column
3. I deleted the duplicates
4. For Martital status, I had M and S which sometimes can confuse stakeholders. So I used find and replace (CTR + H) on M to Married and S to Single.
5. For Gender, I had M and F which sometimes can confuse stakeholders. So I used find and replace (CTR + H) on M to Male and F to Female.
6. For the age column, I had to put them into ranges to make it simple when visualizing the data 
     - I inserted a new column called modified-age (21-30) = Adolescent, (31-50) = Adult ,(51-70) = Old, (71-90) = Very old
     - I used =IFS( age >=71, “very old”, age >= 51, “old”, age >= 31, “Adults, age < 31, “Adolescent”)

### Exploratory Data Analysis

EDA involved exploring the bike sales data to answer key questions, such as:
- Which region has high number of purchases and Which country has high number of no purchases
- Whis age group has high number of purchases and which age group has high number of no purchases
- Which commute distance contributes high to our sales
- Which factor has high effect on the customer's purchase

### Data Analysis

In order to understand data properly and answer the questions identified, I used three pivot tables.
1. 1st Pivottable: Average income of people who purchased the bike or not based on gender.
   - Row: Gender, Column: Purchased or not, values: Average income
2. 2nd Pivottable: I created a pivot table for the commute distance and if purchased or not, to see the relationship between distance and buying.
   - Row: Commute distance, column: Purchased or not, values: Count of yes or no
4. 3rd Pivottable: I created a pivot table for age groups to see which age group is our best customer
   - Row: age group, column: Purchased or not, values: Count of yes or no


### Results

- The region with high number of purchases is North America and Europe, And also the region with high number of no purchases is  North America, Europe
- The age group with high number of purchases is Adult(31-50), Old(51-70). And also the age group with high number of no purchases is Adult, Old
- Customers with 2-5 miles are the ones purchasing our bikes a lot.
- People who purchased our bike have higher average income compared to those who did not purchase the bikes, This can be proven using the avaerage income per customer and also people in Adult age group have earn more money compared to other agegroups.

### Recommendations

Based on analysis, we recommend the following
- Invest in marketing and promotions in North America and Europe to maximise revenues - This is because Those regions have high number of no purchases
- Focus more on people within the Adult and old age group - This is because their income is high hence can afford to buy our bikes
- Reduce the cost of bikes by 10% so that people who make low income can afford to buy them also - This will have a positive impact since we will even have people below 30 years old purchasing our products because they will afford the new cost


### Limitations

I had some limitations regarding this project because some of th data was missing, the missing data included
- Selling price for the bike
- Revenue generated by the bikes
- Taxes impoded in each region


### Sharing

After Clearly analyzing the data and answering the questions indentified, I created visuals for each pivot table, I also included slicers to make navigation easy for stakeholders.
