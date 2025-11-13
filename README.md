# Berkeley_Practical_Application_3
Code and files for Berkeley AI course Practical Application 3 for Module 17
##
## 1. Assignment Objective
### To determine the mos accurate classifier model to predict the factors that explain the success
### of campaigns to have a bank client subscribe to a term deposit product offered by a bank.
##
## 2a. Data Adjustments -- Missing Values
### a. Dropped rows where a column contains a value labeled "unknown"
### b. Dropped duration column; information suggested discarding duration for a better predictive model 
### c. Dropped "illiterate" from education column (small number of rows)
### d. Dropped "nonexistent" from poutcome column (does not contribute to the analysis)
### e. Dropped contact column; only 7 percent of clients contacted by cellular
### f. Dropped pdays column; significant overlap with pdays column (large numbers of people not contacted in previous campaign)
##
## 2b. Feature Modifications for Categorical Variables
### a. Recode job column to binary 1 = employed 0 = unemployed
### b. Recode marital column to binary 1 = married 0 = not married
### c. Recode education column to binary 1 = university or professional 0 = secondary or basic
### d. Recode default column to binary 1 = credit in default 0 = credit not in default
### e. Recode housing column to binary 1 = has housing loan 0 = no housing loan
### f. Recode loan column to binary 1 = has personal loan 0 = no personal loan
### g. Create dummy variables for each month
### h. Create dummy variables for each day of the week
### i. Recode poutcome column to binary 1 = success 0 = failure
###
### recode y (target variable) column to binary 1 = subscribed to term deposit 0 = did not subscribe
##
## 3. Analysis Performed
### a. Developed a baseline model designed to predict the most frequent class for the training data (accuracy score = 0.7207)
### b. Develop set of four basic classifier models using Logistic Regression, K Nearest Neighbors, Decision Trees, and Support Vector Machine.
###    Compared accuracy scores for the four models
###    All 4 models had higher accuracy scores than the baseline model.
###    However, some models such as Decision Tree and SVM appeared to be substantially overfit.
### c. Used Grid Search and scaling to find more optimal parameters for the four models.
### d. Tuning KNN did not result in significant accuracy score improvement, though it appears to correct for overfitting of the training data.
### e. The optimized Decision Tree and Logistic Regression models had very similar accuracy scores.
### f. Technical difficulties prevented proper tuning of the basic SVM model.
##
## 4. Overall Findings
### a. Logistic Regression and Decision Tree provide the highest accuracy scores for the optimized models.
### b. The coefficients with the greatest predictive power overlap between the Logistic Regression and Decision Tree models.
###     In particular, the outcome of the previous marketing campaign was a strong
###     positive predictor of a client subscribing to a term deposit project in a more recent campaign.
