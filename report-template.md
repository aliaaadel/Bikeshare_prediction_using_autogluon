# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: when sunmitting the predictions can't have negative values Thus before sumbmitting the negatice values were removed and replaced with 0 value by going through the predictions and checking its value whether it's less than 0 or not 

### What was the top ranked model that performed?
TODO: top ranking model was the third one after hyperparameter tuning 

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: when plotting the histogram for the features it can be noticed that : most bikerider ride their bikes on workdays and not holidays and datetime feature could be split into multiple features like month,day, hour by turning it to a datetime data . Also weather feature and season can be catogerized


### How much better did your model preform after adding additional features and why do you think that is?
TODO: its performance increased tremendously as the score in the intial model was 1.39 and by adding new features it improved the score as it was 0.56

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: it improved the score of the model a little bit to 0.509 

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: if i were given more time with this dataset i would explore the data more and try to add more features Also try different algorithms on this dataset like KNN, Neural Nets, RF and XGBoost

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|time_limit|epoch|num_boost_round|score|
|--|--|--|--|--|
|initial|600|default|default|1.39|
|add_features|600|default|default|0.56|
|hpo|800|15|160|0.509|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: in this project a regression model is built to predict the bike sharing demand .Bike sharing systems are a means of renting bicycles 
the steps taken to get the predictions outcome:
1- loading data and explore it to get further understanding of the dataset
2-train and evaluate the initail model then submit it 
3-add some new features like (day,month,hour)to the dataset and eliminate uncessary features(datetime)
4-Train and evaluate model it's noticed that the score is improving
5- change the hyperparameters of the model then train it . it's noticed that there's some improvement but not by much  
6- plot graph for each model score and compare between the three models 