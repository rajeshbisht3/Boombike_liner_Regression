# Boombike_liner_Regression
BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

# To achive goal 
Required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

#Data Preparation:
variables like 'weathersit' and 'season' have values as 1, 2, 3, 4 which have specific labels associated with them (as can be seen in the data dictionary). These numeric values associated with the labels may indicate that there is some order to them - which is actually not the case (Check the data dictionary and think why). So, it is advisable to convert such feature values into categorical string values before proceeding with model building. Please refer the data dictionary to get a better understanding of all the independent variables.

column 'yr' with two values 0 and 1 indicating the years 2018 and 2019 respectively. At the first instinct, you might think it is a good idea to drop this column as it only has two values so it might not be a value-add to the model. But in reality, since these bike-sharing systems are slowly gaining popularity, the demand for these bikes is increasing every year proving that the column 'yr' might be a good variable for prediction. So think twice before dropping it. 
#Outlier check 
![image](https://user-images.githubusercontent.com/84132394/208235052-df47bd8b-6fe2-4ed0-9e77-040dc9d38769.png)

# Conslusions: 
The graph clearly shows the qualitative distributions of the data, now if the model suggests the important predictors, using these graphs we can be more confident about the predictions of the model.
For the variable season, we can clearly see that the category 3 : Fall, has the highest median, which shows that the demand was high during this season. It is least for 1: spring .
The year 2019 had a higher count of users as compared to the year 2018
The bike demand is almost constant throughout the week.
The count of total users is in between 4000 to 6000 (~5500) during clear weather
The count is highest in the month of August
The count of users is less during the holidays

# Linear Relationship 

![image](https://user-images.githubusercontent.com/84132394/208235257-6c0f061e-7ea8-4a0e-a100-34431e96ae70.png)

# Conclusion : 
By visualising the numeric variables, we can conclude that a linear model can be considered in this case because there are atleast some independent variables like atemp , temp etc. that show a positive correlation with the target variable cnt 

# HeatMap Correlation 
![image](https://user-images.githubusercontent.com/84132394/208235307-eb9e19db-0b0a-4a1f-b92d-2b59ab43257e.png)
Conclusion: 
As can be seen from the map, atemp and temp seems to be correlated to the target variable cnt. Since, not much can be stated about the other independent variables , hence we'll build a model using all the columns.




# Final Recommendations for the Company:
The months - Jan , Jul , Sep , Nov , Dec should be considered by the company as they have a higher demand as compared to other months.
With an increase in temperature the demand also increases, hence it should keep track of the weather conditions.
During the Winter season the demand rises, hence it should be well prepared to meet the high demand
