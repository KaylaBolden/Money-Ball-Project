# Project_FIFA_MoneyBall

![photo](https://github.com/Ironhack-Data-0621-Remote/Project_FIFA_MoneyBall/blob/main/Images/photo.jpg)

# What made you decide to do this project?
After learning classification models I wanted to take this opportunity to practice them.

# Objective 
Utalize the given data set to predict the "Attacking Work Rate" (a/w). Attacking work rate has 3 possible values: high, medium, and low. 
 
 # Used tools 
  Programs: 
  
      1. Jupiter - python
  
  Methods:
  
      1. Logistic Regression
      2. Histograms, distribution plots, heat maps, box-whisker plots
      
  Libraries:
      1. Normalizer
      2. StandardScaler
      3. confusion_matrix
      4. cohen_kappa_score
      5. math
      6. statistics 
      7. matplotlib.pyplot
      8. seaborn
      9. statsmodels.api
      10. train_test_split
      11. one hot encoder
      12. numpy
      13. pandas
      
 # Workflow
      1. Gather the Data
      2. Explore the Data
      3. Clean the Data
          a. Categorical data:
              i.needs to be grouped into fewer buckets
              ii. dropped if there are too many instances
              iii. cleaned if there are various values with the same meaning
          b. Numerical data:
              i. needs to be converted to number if object (may require functions for data transformations)
       4. Dealing with Nulls
       5. Dealing with Outliers
       6. Check Multicolinearity (but no need to modify since logistic regression isn't impacted by multicolinearity)
       7. Normalize and or standarize the data
       8. Apply Train-Test Split
       9. Train Model
       10. Test Model
       
# Results and conlusions 
      The accuracy of the model on test set is: 0.67 and the Kappa of the model is: 0.25. The data availible my not contain all the drivers of a person's attacking work rate. While, 67% of the time it accurately predicts the value, 33% of the time it is incorrect. To make matters worse, when predicting the outcome for individuals with a 'high' attacking work rate, it predicts them to be medium 61% of the time.
![photo](https://github.com/KaylaBolden/Money-Ball-Project/blob/main/Images/Screen%20Shot%202021-10-09%20at%201.07.43%20PM.png)

      
# Improvements
      Remove highly correlated columns and then remove outliers so that fewer rows are filtered out.
      
## Dataset

In this project, you will use the provided [**fifa21_male2.csv**](https://github.com/Ironhack-Data-0621-Remote/Project_FIFA_MoneyBall/tree/main/Data) dataset.

[Here](https://www.kaggle.com/ekrembayar/fifa-21-complete-player-dataset?select=fifa21_male2.csv) details about the dataset can be found here as well. 

This data set includes:

1. **EA Sports FIFA 19 Game** data:

    |   |   |
    |---|---|
    |  Player Name | Club of the Player   |
    | League  | Position  |
    | Pace  |  Shooting |
    |  Passing | Dribbling  |
    | Defending|Physical|
    |||


1. **Transfermarkt** extra info by player:

    |   |   |
    |---|---|
    |  Date of Birth| Nationality   |
    | Height  | Foot  |
    | Day Joined the current club  |  Day of Contract End |
    |  Market Value of the Player |  |
    |||


2. **Instagram and Facebook** data by player:

   - Number of followers on Instagram
   - Number of likes on Facebook of the club in which the player has a contract

4. **ESPN FC** data from the past 5 years performance of each player

   - **GS:** Games Started
   - **SB:** Games Substituted
   - **G:** Goals Scored
   - **A:** Assists
   - **SH:** Shots
   - **SG:** Shots on Goal
   - **FC:** Fouls Committed
   - **FS:** Fouls Suffered
   - **YC:** Yellow Cards
   - **RC:** Red Cards


