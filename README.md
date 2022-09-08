Car dekho dataset-REGRESSION

1. About the dataset:
According to Car expert magazines, Used car demand at a high, wild prices likely to remain.
During the Covid-19 pandemic their is a shortage of new car production and Individual avoid to public transport and travel for holidays – something that typically involves one’s own car.
But at the same time price of newly manufacturing car is to high. The price of a new car in the industry is fixed by the manufacturer with some additional costs ,advertising cost and incurred by the Government in the form of taxes.
But, due to the increased prices of new cars and the financial incapability of the customers to buy them, Used Car sales are on a global increase.
It found a used vehicle had become 34 per cent more expensive in July 2021 compared to July 2020, and 10 per cent more expensive when compared with the beginning of 2021.

2. Exploratory Data Analysis & Cleaning:
* first  we check the null values and also check the datatypes.

*  Visualize Correlations:
Using the Seaborn library, we can also visualize the correlations between different features. The correlations will only register for the columns with numerical data, but it is still helpful to investigate correlations the relationships between these features.

3.Binarize the Features
* The last step before we can model on the features is to create binary columns for the features that are not numerical. It is hard for the computer to understand the difference in meaning between all the car names, so binarizing simply tells the computer “yes this is a Volvo,” or “no, this is not a Volvo.”

* Binarizing creates a specific column for each car brand, and then each row will have a 0 (not that car brand) or a 1 (it is that car brand). This process of creating binary columns for each feature is also called ‘dummifying’ the variable, and can be done easily with code in Pandas.

* With the dummy/binary columns, the data frame now looks like this — filled with columns of 0s and 1s, except for the three numerical columns. Although there are many more columns, this process makes it possible for the model to understand the information you are providing it with.

4. Split Target & Predictor Variables
* First, we need to define our X and y variables. Y is what we are predicting (sale price) and X is everything we are using to help us make this prediction.
* Train & Test Split:
-> Next we need to create a training and test group for our model. We can use the code below to randomly select 70% of the data as the train group for our model to train on, and 30% will remain as our test group to test the quality of our model.

5. Linear Regression:
* The first model we will try is a simple Linear Regression. It is important to assess the cross validation score, training score, and test score to reflect on how the model is performing.
* Since the training score was much better than the test, it indicates that the model was overfitting to the training data. This means that the model has a very hard time predicting on unseen data — not good! Also, the mean cross validation score is a very large negative number. 

6. at last the model is tested.















