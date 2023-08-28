# Repository: Berkley-ML-AI

## This Repository Contains the Data Analysis and AI model evaluations for "What drives the price of a car?" problem provided in Practical Application Assignment 11.1

### **Overview**
OVERVIEW

In this application, we will explore a dataset from kaggle. The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars to ensure speed of processing. Our goal is to understand what factors make a car more or less expensive. As a result of out analysis, we should provide clear recommendations to our client -- a used car dealership -- as to what consumers value in a used car.

### **Problem Statement:**
Within the dataset encompassing approximately 426K cars, our objective is to determine the influential factors that impact the pricing of used cars for a dealership. To achieve this, a comprehensive analysis of the dataset is imperative. This analysis includes:

**Data Cleaning:** A meticulous review of the dataset to identify and rectify any inconsistencies or inaccuracies.

**Outlier Detection:** Identifying potential outliers and evaluating whether they should be excluded from the analysis.

**Bias Assessment:** Scrutinizing the dataset for any biases and implementing appropriate measures to address them.

**Text Data Transformation:** Converting textual data into a format understandable by the predictive model.

Once these preprocessing steps are accomplished, the subsequent task involves predicting the prices of vehicles within the test dataset, a subset of the provided data. This will be achieved by training various models and subsequently summarizing the impact of distinct car features on used car pricing. The outcome will also encompass identifying the most suitable model for predicting the value of a car, based on the provided feature values.

### **Some insights on Data:**
Original shape of data: (426880, 18)

RangeIndex: 426880 entries, 0 to 426879
Data columns (total 18 columns):
| #   | Column        | Non-Null Count | Dtype    |
| --- | --------------| -------------- | -------- |
| 0   | id            | 426880 non-null| int64    |
| 1   | region        | 426880 non-null| object   |
| 2   | price         | 426880 non-null| int64    |
| 3   | year          | 425675 non-null| float64  |
| 4   | manufacturer  | 409234 non-null| object   |
| 5   | model         | 421603 non-null| object   |
| 6   | condition     | 252776 non-null| object   |
| 7   | cylinders     | 249202 non-null| object   |
| 8   | fuel          | 423867 non-null| object   |
| 9   | odometer      | 422480 non-null| float64  |
| 10  | title_status  | 418638 non-null| object   |
| 11  | transmission  | 424324 non-null| object   |
| 12  | VIN           | 265838 non-null| object   |
| 13  | drive         | 296313 non-null| object   |
| 14  | size          | 120519 non-null| object   |
| 15  | type          | 334022 non-null| object   |
| 16  | paint_color   | 296677 non-null| object   |
| 17  | state         | 426880 non-null| object   |
Dtypes: float64(2), int64(2), object(14)




## **Analysis Report:**                         
#####                                                  Author - Lalitya Sawant
## What drives the price of a car?
#### Python Notebook: https://github.com/LalityaSawant/Berkley-ML-AI-Assignments-2/blob/master/practical_application_II_starter/Berkley-ML-AI-Assignments-2.ipynb
#### Charts folder: https://github.com/LalityaSawant/Berkley-ML-AI-Assignments-2/tree/master/practical_application_II_starter/charts

### **Conclusion:**
  The used car dataset initially encompassed approximately 426,000 car records. However, upon a meticulous examination of the dataset, we identified instances of duplicate records and encountered numerous instances of missing information spread across various columns. Through a thorough process of data cleansing, which entailed either imputing or discarding the incomplete records, we successfully refined the dataset to encompass 286,705 records, while also making the decision to eliminate certain columns.

  Furthermore, we navigated the intricacies of categorical columns by employing an encoder to transform this data into a format compatible with our prediction models. We subjected the dataset to three distinct models, including Linear Regression, Ridge Regression, and Lasso. Remarkably, these models consistently generated predictions that exhibited minimal discrepancies, as evidenced by their closely aligned loss function values.

  Based on our comprehensive analysis, we identified several pivotal features that hold significance for dealerships when making car sales decisions:

  * Fuel type of the car
  * Number of cylinders in the engine
  * Quality of the car's title status
  * Manufacturer of the car
  * Manufacturing year of the car
  * Type of the car
  * Drive configuration of the car (4wd or 2wd)
  * The specific state where the car is sold

   ![Features affecting car prices](https://github.com/LalityaSawant/Berkley-ML-AI-Assignments-2/tree/master/practical_application_II_starter/charts/Features-affecting-used-car-price.jpg)


  These insights serve as valuable guidelines for dealerships, empowering them to make informed decisions during the process of selling cars.
