## Titanic - Machine Learning from Disaster (Kaggle Project)
This is a Kaggle project: Titanic - Machine Learning from Disaster <br>
In this project, I achieved score: 0.79186/1 (0.79%) <br>
<img width="967" alt="Score" src="https://user-images.githubusercontent.com/101066418/156941931-dc8931ae-2cb1-4ec1-9c37-9ae7aeb1a475.png"> <br>
Here is the outline of my notebook:
#### 1. Checking Data 
#### 2. Exploratory Data Analysis
#### 3. Feature Engineering
#### 4. Encoding and Normalization
#### 5. Modeling
#### 6. Prediction
=======================================================================
## 1. Checking Data
- Checking the data type (int, float, object, etc.)
- Checking missing data in both train and test set
- Summary statistics

## 2. Exploratory Data Analysis
- Correlation table and the corresponding heatmap
- Numerical data analysis:
  - Survived Probability of 'SibSp'
  - Count of Survived and Not Survived for 'SibSp'
  - Survived Probability of 'Parch'
  - Count of Survived and Not Survived for 'Parch'
  - Distribution of 'Age' and 'Fare'
- Categorical data analysis:
  - Survived Probability of 'Pclass'
  - Count of Survived and Not Survived for 'Pclass'
  - Survived Probability of 'Sex'
  - Count of Survived and Not Survived for 'Sex'
  - Survived Probability of 'Embarked'
  - Count of Survived and Not Survived for 'Embarked'

## 3. Feature Engineering
- 'Name' and 'Title' Engineering and Analysis
  - Get the title (Mr, Mrs, Ms, Master, etc.) from each entry in 'Name' and create a new feature 'Title'
  - Divide titles into four groups: 'Mr', 'Miss/Ms/Mme/Mlle/Mrs', 'Master', 'Other'
  - Survived Probability of 'Title'
  - Count of Survived and Not Survived for 'Title'
  - Drop the 'Name'
- 'Cabin' Engineering and Analysis
  - Get the first letter from 'Cabin' and assign 'X' to missing data
  - Survived Probability of 'Cabin'
  - Count of Survived and Not Survived for 'Cabin'
- 'Ticket' Engineering and Analysis
  - Get the prefix from 'Ticket' and assign 'X' to entries without prefix
  - Survived Probability of 'Ticket'
  - Count of Survived and Not Survived for 'Ticket'
- 'FamilySize', 'SibSp' and 'Parch' Engineering and Analysis
  - Combine 'SibSp' and 'Parch' and get 'FamilySize'
  - Survived Probability of 'FamilySize'
  - Count of Survived and Not Survived for 'FamilySize'
  - Drop 'SibSp' and 'Parch'

## 4. Encoding and Normalization
- Creating dummy variables for the categorical data
- Apply Min-Max Normalization

## 5. Modeling
- Random Forest Classifier
- Logistic Regression
- Support Vector Classifier
- XGBClassifier
- Evaluate the models by cross validation (K=5)

## 6. Prediction
- Apply Support Vector Classifier as the final model
- GridSearchCV
- Score: 0.79186/1
