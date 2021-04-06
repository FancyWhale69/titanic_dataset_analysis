# titanic_dataset_analysis
  
# installation  
you will need python, jupiter notebook, and a list of libraries:  
1- pandas  
2- numpy  
3- matplotlib  
4- seaborn  
5- scikit-learn  

# Project Motivation  
The goal is to analyise the [titanic](https://www.kaggle.com/c/titanic/data) data set to answer 3 questions:  
1- does gender affect survival rate?  
2- does ticket class affect survival rate?  
3- does having parent/childe affect survival rate?  
finally you can use the trained model to predict wethier you will survive or not.  

# File Descriptions  
titanic_analysis.ipynb (includes the code for the project)  

titanic folder contains:  
1- train.csv (training data including features and responce)  
2- test.csv (test features)  
3- gender_submission.csv (include the responce for test data)  

# How to Interact with your project  
download the repo to your local device or google colab.  
install needed libraries.  
make sure to run the first two cells (importing libraries and reeading data).  
go ahead and explore the notebook.  

# results Summery  
From my analysis i found that gender is the most important factor for survival in the titanic.  
in all 3 factors i analyised (gender, ticket class, number of parent/child) i found that women had a higher survival rate than men in all 3 of them.  

# acknowledgment  
i would like to thank kaggle for providing a huge amount of data sets for free.  

# CRISP-DM  
1-Business Understanding/questions:  
diving into this data set i had 3 questions:  
  1- which gender survive more  
  2- does ticket class affect survival rate  
  3- does having parent/child on board affect survival  
  
2-Data Understanding:  
Data was downloaded from [kaggle](https://www.kaggle.com/c/titanic/data).  
data was missing some values in the Age, Cabin, and Embarked columns, but the Cabin column was more than 75% missing  
while Age was %20 and Emarked had less than %1 missing.  

3-Prepare Data:  
Some filling was done to the Age and Ebarked columns (details in notebook).  
Cabin and PassengerId were drop.  
feature engeenring was done to the Name column.  
finnaly dummies were made for remaining categorical columns.  

4-Data Modeling:
Logistic regression were used since responce is binary (0= dead, 1=survive)  

5-Evaluate the Results:  
the model achived an accurcy of %95 on test data.










