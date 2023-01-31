# Worldwide Sales Data Analysis and Exploration using Zeppelin HDFS and Spark

## Introduction 
In this project, the objective was to analyze a worldwide sales dataset using Zeppelin and HDFS. The data was ingested into Zeppelin and queried using Spark basic Scala commands and SQL. The focus of the analysis was to provide a comprehensive breakdown of the sales data and uncover key insights into sales patterns and trends.

The first step in the analysis was to load the data into a dataframe using Zeppelin and HDFS. The data was then displayed in the dataframe format, allowing for a visual inspection of the data. The next step was to print the schema of the dataframe, providing a structured overview of the variables and data types in the dataset.

To further refine the analysis, the dataframe was filtered to show only those observations where the number of units sold was greater than 8000 and the unit cost was greater than 500. This helped to focus on the most significant sales data and identify the top-performing products and regions.

Finally, the data was grouped by region and the count of observations in each region was calculated. This provided a summary of the sales data by region, allowing the customer to determine the areas where sales were strongest and where they should focus their marketing and sales efforts.

In conclusion, this project demonstrates the power of Zeppelin and HDFS in performing data analysis and uncovering valuable insights from sales data. By using Spark basic Scala commands and SQL, the data was queried and analyzed with ease, providing valuable information for the customer to make informed business decisions.

## Tools Used
- Zeppelin
- Spark
- HDFS
- Scala
- SQL

# Result 

![image](https://user-images.githubusercontent.com/69835617/215882858-b330e3de-137b-491a-b99e-78ac8593f8ee.png)

## Process

- Load data into a Spark dataframe

![image](https://user-images.githubusercontent.com/69835617/215881338-8bb5d21e-1a6a-4a0a-b6c0-14d4e71bb22c.png)

- Print the dataframe schema

![image](https://user-images.githubusercontent.com/69835617/215881419-2a13b5dc-5e3a-467c-839b-58d36a362b26.png)

- Filter the dataframe to show units sold greater than 8000 and unit cost greater than 500 ("&&" operator can be used for multiple "AND" conditions)

![image](https://user-images.githubusercontent.com/69835617/215881965-cbaf49ad-0fd7-4ecb-8146-b5b8ac19b1f0.png)

- Aggregate the dataframe via group by “Region” and count

![image](https://user-images.githubusercontent.com/69835617/215882059-1b115a95-3c6f-4c07-bc0c-bf9406372047.png)

- Saving this new subset dataframe as a csv file into HDFS

![image](https://user-images.githubusercontent.com/69835617/215882158-d75f29c7-656a-42ff-8dde-f25f3e13c8e1.png)

- Using SQL select all from “Regionview” view and show in a line graph

![image](https://user-images.githubusercontent.com/69835617/215882323-ea8a5147-01ce-407d-a605-d447dffb474e.png)

- Using SQL, from the “Salesview” view, Select the region and sum of units sold, and group by region

![image](https://user-images.githubusercontent.com/69835617/215882492-b18ead51-e858-422c-b218-c62c227c8e24.png)

- Using SQL select from the “Salesview” view – the region and sum of total_profit and group by region and display in a Bar chart

![image](https://user-images.githubusercontent.com/69835617/215882570-8c4347ab-c9e8-421e-a6b6-549321ddbb4a.png)

- Using SQL select from the “Salesview” view – show the total profit as profit, the total revenue as revenue and the total cost as cost from “Salesview”, group by region

![image](https://user-images.githubusercontent.com/69835617/215882694-34011ee4-0fb9-4855-a3a7-5c9b0324a9ca.png)

- The client is in the process of opening up a new store and they are looking at the best location to do so - They need to see the avg profit in each region as a percentage (pie chart) compared to other regions

![image](https://user-images.githubusercontent.com/69835617/215882785-c8902106-a95b-4c32-a646-8a9728542e66.png)


