# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import chardet module.
2. Print the sum of null data.
3. Print the data info.
4. Obtain the x and y values.
5. Predict the y values and print the values.
6. Get the accurate value and print them.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Meetha Prabhu
RegisterNumber: 212222240065
**
import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding="Windows-1252")

**
import chardet 
file='/content/spam.csv'
with open(file,'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result

**
print("Data:")
data.head()

**
print("Null Data:")
data.isnull().sum()

**
print("Data Information:")
data.info()
 
**
x=data["v1"].values
y=data["v2"].values
 
**
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

**
from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

**
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
print("Y_Pred")
y_pred

**
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy

**
*/
```

## Output:
![image](https://github.com/Meetha22003992/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119401038/ecbdde5c-0714-4a73-9ce5-b27de9020265)

![image](https://github.com/Meetha22003992/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119401038/7e3752db-b624-4127-839b-3596df2ddf05)

![image](https://github.com/Meetha22003992/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119401038/e90120ff-bcb8-4fc6-9251-c61080d201ca)

![image](https://github.com/Meetha22003992/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119401038/1ee4a558-110b-44ed-9fdc-b252a5c105c0)

![image](https://github.com/Meetha22003992/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119401038/39840318-4532-41bd-92c9-5c4a461aec43)

![image](https://github.com/Meetha22003992/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119401038/fc72ee25-867c-4a98-b089-b4202b0586ee)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
