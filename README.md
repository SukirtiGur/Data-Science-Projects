# Data-Science-Projects
### Exploratory Data Analysis - Uber Case Study

Objective : To extract actionable insights from the data that we have collected over the past 6 months to optimise resources andidentify area of growth and improvement.

Focused majorly on - Variables that influence the pickups, Factors that affects pickups the most and Ways to capitalize the fluctuating demands

The data contains weather information, location and number of pickups

* Performed univariate analysis on variables in the data
* Performed bivariate analysis to better understand the correlation between different variables
* Created Visualizations to explore data and extract the insights

Conclusions
* Uber cabs are most popular in the Manhattan area of New York.    
* Contrary to intuition, weather conditions do not have much impact on the number of Uber pickups.
* The demand for Uber has been increasing steadily over the months (Jan to June).
* The rate of pickups is higher on the weekends as compared to weekdays.
* It is encouraging to see that New Yorkers trust Uber taxi services when they step out to enjoy their evenings.
* We can also conclude that people use Uber for regular office commutes. The demand steadily increases from 6 AM to 10 AM, then declines a little and starts picking up     till midnight. The demand peaks at 7-8 PM.
* We need to further investigate the low demand for Uber on Mondays.

### House Price Prediction - Full Linear Regression, Best Subset , Stepwise Regression and Forward Selection

Objective: Predict the final sales price of each house.

* Implemented the following models - 
Full Regression Model (takes into account all predictor variables) , Best Subset Linear Regression (fits all possible models based on the independent variables that you specify) , Stepwise Regression (successively add or drop variables) and Forward Selection (Start with the constant model and successively add statistically significant variables)

* Performance measure used - Root Mean Squared Error (RMSE)

* Used AIC score to quantify the best model.The AIC is designed to find the model that explains the most variation in the data, while penalizing for models that use an excessive number of parameters 

* In Best Subset Linear Regression  took all possible combinations of 2 predictor variables to save time and chose model which has the least AIC score. The two most important variables for predicting house price is 'GrLivArea' and 'OverallQual'.

* Stepwise Regression .The AIC score of the best model is 23160.908. The model selected 92 variables

* Forward Selection model.  The best forward selection model has the AIC score of 23178.092 and it has 102 variables .

* The stepwise model has the least RMSE of all the models.The subset model has the highest RMSE but we built the model only for 2 variables to save time. We can further explore as many variables as we wish and calculate the RMSE

### Unsupervised Learning

Objective: The purpose of the case study is to classify a given silhouette as one of four different types of vehicle

* Built correlation matrix between 'class' variable and other features to check the relationship. There were few features with strong correlation with the target variable.

* Implemented PCA on our training data set to reduce the dimensionality of the data. We chose the most important principal components that explain the maximum variance in the dataset. In our case we reduced the dimension from 18 to 7 and selected those which explained 95% variance.Principal Components are linear combination of original features which makes them less interpretable. Reducing dimensionality does cause some information loss.

* Applied Random Forest and Support Vector Classifier on the reduced features (dimensions) and got average precision score of 74% and 76% , recall score of 77% and 78% , accuracy score of 77% and 78% respectively. Also applied SVC on the 18 actual features (with interpretability) and saw an accuracy score of 96%, precision (macro) score of 97% and recall (macro) score of 95%, which is a way better score then SVC when applied on principal components.

* Based on learning curve we saw that Random Forest Classifier was overfitting the training set and not performing well on the validation set.

* For SVC with principal components and SVC with original features both training score and validation score increase with the increase in the size of the training data.






