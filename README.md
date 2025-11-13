# Berkeley_Practical_Application_3
Code and files for Berkeley AI course Practical Application 3 for module 17
##
## 1. Assignment Objective
### To determine the mos accurate classifier model to predict the factors that explain the success
### of campaigns to have a bank client subscribe to a term deposit product offered by a bank.
##
## 2. Data Adjustments -- Missing Values and Feature Modifications for Categorical Variables
### Dropped rows where a column contains a value labeled "unknown"
### Dropped duration column; information suggested discarding duration for a better predictive model 
### Dropped "illiterate" from education column (small number of rows)
### Dropped "nonexistent" from poutcome column (does not contribute to the analysis)
### Dropped contact column; only 7 percent of clients contacted by cellular
### Dropped pdays column; significant overlap with pdays column (large numbers of people not contacted in previous campaign)

### Recode job column to binary 1 = employed 0 = unemployed
### Recode marital column to binary 1 = married 0 = not married
### Recode education column to binary 1 = university or professional 0 = secondary or basic
### Recode default column to binary 1 = credit in default 0 = credit not in default
### Recode housing column to binary 1 = has housing loan 0 = no housing loan
### Recode loan column to binary 1 = has personal loan 0 = no personal loan
### Create dummy variables for each month
### Create dummy variables for each day of the week
### Recode poutcome column to binary 1 = success 0 = failure
###
### recode y (target variable) column to binary 1 = subscribed to term deposit 0 = did not subscribe
##
## 3. 
