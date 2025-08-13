# **Determine if in-flight entertainment experience leads to higher customer satisfaction using logistic regression**

## **Overview**
In this project, we want to know if a better in-flight entertainment experience leads to higher customer satisfaction ratings for an airline company. We will construct and evaluate a logistic regression model that predicts whether a future customer would be satisfied with the services given previous customer feedback about the flight experience. 

## **Data Dictionary**
This project uses a dataset called `airline_satisfaction.csv` from [Kaggle](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction/data). It represents the details of customer feedback for an airline company.

*Note: The dataset has been modified for this project.*

The dataset contains: 23 columns of customer feedback, each row representing one customer’s response. All the responses were given on a 0 to 5 scale, 0 meaning “not at all satisfied” and 5 meaning “very satisfied”.

The dataset contains:

**129,880 rows** – each row is a different customer response 

**23 columns**

| Column name | Type | Description | 
|-------------|------|-------------|
| Gender | str | Gender of the passengers (Female, Male) | 
| Customer Type | str | The customer type (Loyal customer, disloyal customer) | 
| Age | int64 | The actual age of the passengers |
| Type of Travel | str | Purpose of the flight of the passengers (Personal Travel, Business Travel) |
| Class | str | Travel class in the plane of the passengers (Business, Eco, Eco Plus) |
| Flight distance | int64 | The flight distance of this journey |
| Inflight wifi service | int64 | Satisfaction level of the inflight wifi service (1-5, with 0 meaning "Not Applicable") |
| Departure/Arrival time convenient | int64 | Satisfaction level of Departure/Arrival time convenient |
| Ease of Online booking | int64 | Satisfaction level of online booking |
| Gate location | int64 | Satisfaction level of Gate location |
| Food and drink | int64 | Satisfaction level of Food and drink |
| Online boarding | int64 | Satisfaction level of online boarding |
| Seat comfort | int64 | Satisfaction level of Seat comfort |
| Inflight entertainment | int64 | Satisfaction level of inflight entertainment |
| On-board service | int64 | Satisfaction level of On-board service |
| Leg room service | int64 | Satisfaction level of Leg room service |
| Baggage handling | int64 | Satisfaction level of baggage handling |
| Check-in service | int64 | Satisfaction level of Check-in service |
| Inflight service | int64 | Satisfaction level of inflight service |
| Cleanliness | int64 | Satisfaction level of Cleanliness |
| Departure Delay in Minutes | int64 | Minutes delayed when departure |
| Arrival Delay in Minutes | float64 | Minutes delayed when Arrival |
| Satisfaction | str | Airline satisfaction level (Satisfaction, neutral or dissatisfaction) |


## **Steps**
### **1. Imports**
- Import libraries and packages
- Load the dataset into a dataFrame

### **2. Data exploration, data cleaning, and model preparation**
- Explore the data
- Check for null values in the data
- Modify the data types
- Encode the data
- Create new column
- Create the training and testing data

### **3. Model building**
- Fit the model to the data
- Check parameter estimates
- Create a regression chart of the model

### **4. Results and evaluation**
- Predict the outcome for the test dataset
- Analyze the results
- Produce a confusion matrix

## **Findings**
- There are total of 129,880 rows and 23 columns in this dataset, with each row representing customer feedback.
- There are only 393 missing values out of the total of 129,880 rows, in only one column "Arrival Delay in Minutes".
- There were 56,262 satisfied customers and 73,225 dissatisfied customers.
- 43.5% (56,262/129,487) of customers were satisfied.
- The regression graph seems to indicate that the higher the inflight entertainment value
- Logistic regression accurately predicted satisfaction 69.8% of the time.

## **Recommendations**
- Customers who rated in-flight entertainment highly were more likely to be satisfied. Improving in-flight entertainment should lead to better customer satisfaction.
- The model is 69.8% accurate. This is an improvement over the dataset’s customer satisfaction rate of 43.5%.
- The success of the model suggests that the airline should invest more in model developement to examine if adding more independent variables leads to better results.
- Building this model could not only be useful in predicting whether or not a customer would be satisfied but also lead to a better understanding of what independent variables lead to happier customers.

## **Next steps**
- Using more than a single independent variable in the model training process could improve model performance.
- Other variables, like "Departure Delay in Minutes" seem like they can be potentially influential to customer satisfaction.

## **Possible questions**
- Are all the different flight routes considered for this data? 
- Is this data from from a specific region? (e.g. european flights only or domestic flights only)
- How many different aircraft models does the company operate? What are the aircraft models that the company is operating?
- Where is the flight flying from and what is the destination? 
- Are the customers travelling alone, in a group, with family?
- What is the price of the air ticket?
