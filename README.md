# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries .

2.Read the data frame using pandas.

3.Get the information regarding the null values present in the dataframe.

4.Apply label encoder to the non-numerical column inoreder to convert into numerical values.

5.Determine training and test data set.

6.Apply decision tree regression on to the dataframe.

7.Get the values of Mean square error, r2 and data prediction.
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SANDHYA BN
RegisterNumber:  212222040144
data=pd.read_csv("Salary Data.csv")
data.head()
data.tail()
data.info()
data["Gender"]=data["Gender"].astype('category')
data["Education Level"]=data["Education Level"].astype('category')
data["Job Title"]=data["Job Title"].astype('category')
data.info()
data["Gender"]=data["Gender"].cat.codes
data["Education Level"]=data["Education Level"].cat.codes
data["Job Title"]=data["Job Title"].cat.codes
data.info()
data.head()
x=data[['Age','Gender','Education Level','Job Title','Years of Experience']]
x
x.shape
y=data[['Salary']]
y.shape
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(x, y, test_size=0.2, random_state=2)
from sklearn.tree import DecisionTreeRegressor
dtr=DecisionTreeRegressor()
dtr.fit(x_train,y_train)
y_pred=dtr.predict(x_test)
print(y_pred)
x_train.shape
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dtr.predict([[44,0,2,130,20]])
*/
```

## Output:

## READ CSV HEAD FILE:
![71](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/17aaaa4f-6d07-49c2-9bf0-97ba72e80f46)

## TAIL:

![72](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/d4fde397-1baa-42f8-8af9-eddf80365494)

## DATASET INFO:

![73](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/c5cd750a-63ef-4aa2-a88a-ceb976aaedf0)

![74](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/7a84792b-1c85-4aff-9e63-dbb0d0c03749)

![75](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/1588211b-62de-466e-bafd-565237de4cc8)

![76](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/cfd43b49-d659-4943-9291-5800e05919d5)


## X DATA:

![77](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/0b3859bc-a0d4-468d-ad54-70d19806982e)

## DATA SHAPE:

![78](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/2904d79d-9e62-40c2-9c06-c02a4594df32)

## Y PRED:

![79](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/4f163e4c-c38a-4fff-a0cb-22fb4a7b17f4)

## MEAN SQUARED VALUE:

![80](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/a1953d5f-cb6d-475d-aaad-04173e18ea05)

## R2 VALUE:

![81](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/d9a5d312-1efe-4a5f-8294-13869481657e)

## DTR PREDICT:

![82](https://github.com/sandhyabalamurali/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/115525118/6b2d977c-a094-4ea6-b0e3-b6e7e537f212)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
