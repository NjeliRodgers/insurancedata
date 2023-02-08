# EDA-and-logistic-regression-on-bank-churn-dataset
PROJECT:Using bank chun data set to carry out EDA and logistic regression whether a customer will chun .In simple terms using the data set provided (bank churn data set )am gonna carry out EDA and logistic regression to determine whether a customer will exit or leave the company.


#Data collection
I started by importing all the neccesary liblaries that are required i.e pandas ,seaborn,numpy etc.I then imported and read the data with the code given below: data= pd.read_csv ('Churn_Modelling.csv')


#Learning and understanding the data
In this stage i carried out exploratory data analysis.And i started by understading the data head,the data tail, the data shape ,the data size ,the data columns,the uniqness of the data and the type of variable contained not forgetting the data types.

#Cleaning the data
 At this stage am required to remove unwanted valuess and variables from the data set and get of rid of any irregeulaties in it since such irregulaties can cause adverse effect on our results .I used the code {data.isnull().sum()} to check the missing or null values luckily my data had no null values

#Bulding the logistic regression
I used the code [data.drop(['column_name1', 'column_name2'], axis=1, inplace=True)] to drop columns that were insignificant in carring out our logistic regression .Using the bank churn data set i check the out liars and plotted cutter plots .I then carried out a relationship analysis for the data by plotting a co-relation hit map and pair plot .I removed unnecessary from the data set .The next step was to split data into training and test.I imported logistic regression using the following code [from sklearn.linear_model import LogisticRegression logreg = LogisticRegression() logreg.fit(X_train, y_train) y_pred = logreg.predict(X_test)]then evaluated the prediction accuracyand the raw confusion matrix.
