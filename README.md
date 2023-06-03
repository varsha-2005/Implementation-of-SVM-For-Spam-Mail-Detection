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
Developed by: varsha.g
RegisterNumber: 212222230166

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

x=data["v1"].values

y=data["v2"].values

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
Result output:

![242841614-f02335b4-97d3-4a67-9748-cdc639fd40d4](https://github.com/MavillaPranathi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118343610/cacbf733-6e6b-40a0-9367-fd2ac5598e3c)

data.head()

![242841732-3d99a04d-f230-44d8-a8be-6c255a566833](https://github.com/MavillaPranathi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118343610/c4a1d01e-c00a-443f-b692-86da0d1084ef)

data.info()

![242841857-900fc1b4-5dd7-44d8-afa6-01f8c71cfab4](https://github.com/MavillaPranathi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118343610/3d9f3ae0-a89a-4d6d-b056-b1c9f88553c4)

data.isnull().sum()

![242841940-109c8db0-556b-42d9-a19a-888628ec281e](https://github.com/MavillaPranathi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118343610/992f5e51-47c9-4e19-987f-d402f0eb7456)

y_prediction value

![242842047-42966bc4-a936-49cb-b495-ea2a7ec8905e](https://github.com/MavillaPranathi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118343610/96e1976e-d122-4166-9324-63b9690a9704)

accuracy value

![242842215-5a427e7d-f05e-4656-8d23-9523ca01711e](https://github.com/MavillaPranathi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118343610/fdb280e3-e160-4e6a-9f05-36ba8625a475)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
