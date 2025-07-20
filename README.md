# La-Liga-Statistics-
Predicting Future Performance of Soccer Players Using Data Analysis

Introduction

This report encapsulates the methodologies and findings of my python, analytical project aimed at predicting future performance of La Liga soccer players for the 2019-2020 season. Using previous historical data, the project integrates exploratory analysis, feature engineering, predictive modeling, and validation techniques to gain insights into player performances and forecast future outcomes of individual players in every team in the 2019-2020 season.

Methodology

1. Data Collection: The data was sourced from Kaggle, containing detailed player statistics for 570 players, including metrics like goals scored, assists, and minutes played.
   
2. Exploratory Data Analysis: Initial analysis involved summarizing statistics, visualizing distributions, and understanding the relationships between variables through correlation matrices.

3. Feature Engineering: New features like 'Duels won', 'Duels contested', and 'Performance index' were derived from existing data to enhance the modeling process.

4. Predictive Modeling:
    - A linear regression model was used to predict the performance index based on selected features.
    - A Random Forest regressor was necessary to forecast the full season's goals, leveraging mid-season data as a proxy for prediction since players statistics were needed with this technique.

5. Validation and Testing
    - The models were trained on a split dataset, 80/20,  and validated using R-squared and Mean Squared Error (MSE).
    - Model robustness was assessed by comparing actual versus predicted outcomes.

Results

My project achieved an R-squared value of 0.87 for the linear regression model, indicating a high level of accuracy in predicting the performance index. The Random Forest model emulator showed true results in accurately forecasting player goals, with a low MSE, leading to minimal change from the actual values.

Discussion

The findings I found show a strong correlation between playing time and player performance metrics such as goals and assists. Feature engineering here played an important role also in enhancing model predictions when I put incorporating composite metrics that capture more unique aspects of performance on these La Liga players. It shows goals of course, I could use K-nearest neighbors if I had more years to see which statistics align with different poisitions in the seasonal trends.

Conclusion

The predictive models developed in this project resemble some significant potential in forecasting player performance in soccer of this caliber in the La Liga. These tools I used can aid team management in strategic planning and performance optimization. Of couse, I didn't have access to multiple season of data in La Liga to provide a more consistent modeling visual, but this can still optimize performance with the parameters of performance mentioned. Perhaps for future improvements building off multiple years and multiple leagues for more comparison predictive analysis may also be helpful too. 


References

Brownlee, Jason. “How to Avoid Data Leakage When Performing Data Preparation.” MachineLearningMastery.com, August 17, 2020. https://machinelearningmastery.com/data-preparation-without-data-leakage/. 

Prabhat. “Laliga Player Stats.” Kaggle, April 5, 2021. https://www.kaggle.com/datasets/thegreatcoder/laliga-player-stats.

“Sklearn.Impute.SimpleImputer.” scikit, 2024. https://scikit-learn.org/stable/modules/generated/sklearn.impute.SimpleImputer.html.  
