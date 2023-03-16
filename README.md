# Uber Data Management & Driver Churn Analysis using Hadoop Big Data Tools
Driver churn analysis based on Uber dataset using big data tools such as Hive, PySpark, Pig, BigQuery, Hbase, and MongoDB.

## Introduction
Uber is a transportation firm with a mobile app that enables customers to request rides and drivers to collect payments for their services. Uber is a ridesharing company that specifically employs independent contractors as drivers. It is one of many services available today that support the sharing economy by offering a way to connect available resources rather than providing the actual resources themselves. The business, which has its headquarters in San Francisco, was established in 2009 by Travis Kalanick and Garrett Camp. Worldwide, the corporation is thought to have 110 million subscribers.
Problem statements(s): In many of the nations it operates, Uber dominates the ride-hailing market. Other regional goliaths have, however, fiercely competed against the corporation. In Asia, Grab, Ola and Didi- Chuxing have given it a run for its money, while Bolt and Yango are strong rivals in Europe and Africa.
Since the ecosystem of the ride-hailing sector is primarily dependent on “Drivers”, who are independent contractors who provide vehicles and services to the consumer market, In the trucking industry, there is a big problem called "driver churn," which happens when drivers resign and start working for a competitor company or in another sector. By analysing the dataset, we would be able to identify these drivers and investigate their income to determine how many of these resignations have happened because of income matters.

## Methodology
The original dataset for this study was obtained from Kaggle (2022). This dataset contains 200,000 records of uber trips made in October 2016. According to the location information, we assume the data is extracted for New York City. The size of the csv file is 16.022MB.
Feature
id
key
driver_id fare_amount pickup_datetime pickup_longitude pickup_latitude dropoff_longitude dropoff_latitude passenger
status
Data Type
int string int
float datetime float float float float
int string
Description
index
a unique identifier for each trip
The id of each driver
The fare amount of each trip
The date and time when pick up the customer
The longitude of the pickup location
The latitude of the pickup location
The longitude of the dropoff longitude
The latitude of the dropoff location
The number of passengers in the trip
The status of the driver whether he/she has resigned
Table 1: Dataset Information
A few selected Hadoop big data tools will be used on top of Hadoop File System (HDFS). Apart from that, we will also be using MongoDB as a comparison to Hadoop technologies. Here are some introductions to the tools used in this project.

## Data Analytics Pipeline

![alt text](https://github.com/[Hosseinglm]/[Uber_driver_churn_analysis_BigData]/[main]/Pipeline.png?raw=true)
