# PREMIER-LEAGE-PREDICTION

Introduction:

The Premier League is considered one of the most competitive and exciting football leagues in the world, with billions of fans tuning in to watch the matches every year. As a fan of the Premier League, I created a machine learning model to predict the outcomes of matches in the league. The league is known for its competitiveness and unpredictability, making it an exciting league to follow. This analysis and machine learning model should be useful in gaining insights on match predictions in the Premier League.

Data:

As mentioned above, I collect the data from the Kaggle platform. The match statistics are from the 2000/2001 season to the 2018/2019 season. There are in total 6839 data points with no missing data in any fields. After uploading the data file, I pre-processed it, choosing only the features that
I considered highly impactful (justification below) to ensure the accuracy of the model. The get_dummies function in Pandas was also used to convert the categorical values into numerical ones.

Feature justification
- Host team: It does matter which team is gonna host the match. Hosting give the club advantage of not having to travel, a familiar playground, and of course, fan encouragement.
- HTP, ATP: HTP (Home Team Point) and APT (Away Team Point) indicate the average point that the team earns in that season. This is a good reflection of the corresponding position between the two teams at the moment.
- HTGD, ATGD: HTGD (Home Team Goal Difference) and ATDG (Away Team Goal Difference) is the average of the goal the team scored and conceded in that season. In football, the team that scores more goals is the winner; therefore, I believe these two features are strong indicators of the team’s winning probability.
- DiffPts: Difference of current season points between two teams (home’s – away’s): The team result can vary significantly among different seasons due to reasons such as changes in line-up. It’s important to take into account how the team are performing in this season to predict their future matches
- DiffFormpPTS (H1 – H5, A1 – A5): Result of the last 5 matches of the team. This will help us know how the team is performing recently.Furthermore, I also visualize the data by using the scatterplot and all of the features show a strong correlation with what we’re trying to predict – the ‘Result’


Methodology:

I used various machine learning techniques, including Logistic Regression and Decision Tree Classifier to build a model that predicts the outcome of Premier League matches. I also performed feature engineering and feature selection to improve the model's performance.

Result:

The final model achieved an accuracy of 70% on the test set, which is promising for its application in football prediction.

Conclusion:

My problem try to predict whether the host team will win or not in a football match in the England Football Division. According to the Results section, I have chosen the Logistic Regression as my final method (justification above) because of the smaller difference between training and validation datasets. This makes sense as due to the simplistic assumption of linear decision boundaries, the Logistic Regression algorithm has been known to be less prone to overfitting. 

The code for this project was written in Python 3.8 and requires the following libraries:

Pandas

Numpy

Sklearn

Matplotlib

Usage:

To run the code for this project, clone the repository and run the Jupyter Notebook file.
