# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1)Import the required packages.
2)Import the dataset to operate on.
3)Split the dataset.
4)Predict the required output.
5)End the program.


## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: BALAJEE K.S
RegisterNumber:  212222080009
import chardet
file='/content/spam.csv'
with open(file,'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result


import pandas as pd
data=pd.read_csv('/content/spam.csv',encoding='Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values
y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
![SVM For Spam Mail Detection](sam.png)

Result output:
![image](https://github.com/balajeeakm/Implementation-of-SVM-For-Spam-Mail-Detection/assets/131589871/75eb4f13-da68-4d8f-a478-10169b7b72f6)
data.head()
![image](https://github.com/balajeeakm/Implementation-of-SVM-For-Spam-Mail-Detection/assets/131589871/070e8e33-1115-493b-b17f-25668b8cea53)
data.info()

![image](https://github.com/balajeeakm/Implementation-of-SVM-For-Spam-Mail-Detection/assets/131589871/b76a6f40-8337-45ef-bee8-232866405a19)
data.isnull().sum()

![image](https://github.com/balajeeakm/Implementation-of-SVM-For-Spam-Mail-Detection/assets/131589871/a6be1a8e-3cba-4772-a826-175b603bc2bf)
Y_prediction value
![image](https://github.com/balajeeakm/Implementation-of-SVM-For-Spam-Mail-Detection/assets/131589871/2a4bb6a2-e5c2-47d5-a622-bc0c13586d6b)
Accuracy value

![image](https://github.com/balajeeakm/Implementation-of-SVM-For-Spam-Mail-Detection/assets/131589871/5ef8ccb6-98ab-4e9a-ac7a-925abeee593b)











## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
