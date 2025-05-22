# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start the program
2. Import the python pandas library as pd
3. Read the contents of the Spam csv file
4. Display the first 5 rows of the dataset using head()
5. Assign x as v1 values and y as v2 values
6. From sklearn library select the feature extraction and import CountVectorizer
7. CountVectorizer will convert the Text to Numerical Data
8. From sklearn library import Support Vector Classifier (ie. SVC)
9. Predict the x_test using SVC
10. Print the accuracy of the SVM Model 11.Stop the program
## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Haarish V
RegisterNumber: 212223230067
*/
```
```
/*
import chardet
file='/content/spam.csv'
with open(file, 'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result

import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding = 'Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v2"].values

y=data["v1"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv = CountVectorizer()

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

## 1. Result output
![Screenshot 2025-05-22 161119](https://github.com/user-attachments/assets/ea3485af-dbca-4600-a713-f779a0af1a3c)

## 2. data.head()
![Screenshot 2025-05-22 161114](https://github.com/user-attachments/assets/089d0378-4965-477b-b651-1ee4c5d67340)

## 3. data.info()
![Screenshot 2025-05-22 161109](https://github.com/user-attachments/assets/f699a906-246c-46d2-9f54-0cdeecf76324)

## 4. data.isnull().sum()
![Screenshot 2025-05-22 161100](https://github.com/user-attachments/assets/8bf53d9f-bd13-4856-877c-2b0fe2b167a7)

## 5. Y_prediction value
![Screenshot 2025-05-22 161443](https://github.com/user-attachments/assets/079b8a0c-610a-4f3a-922f-b70b0a595063)

## 6. Accuracy value
![Screenshot 2025-05-22 161437](https://github.com/user-attachments/assets/5b1447f6-5e73-4cbb-aaf1-6cd3815d7e56)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
