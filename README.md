# Heart Diseases Prediction

Problem Statement:

To predict potential Heart Diseases in people using Machine Learning algorithms. The algorithms include K Neighbours Classifier, Support Vector Classifier, Decision Tree Classifier and Random Forest Classifier. The dataset was retrieved from Kaggle - https://www.kaggle.com/ronitf/heart-disease-uci.

Libraries used for this project are:

1. numpy
2. pandas
3. matplotlib
4. warnings
5. train_test_split
6. StandardScaler

After importing the above libraries, I imported the required ML algorithms:

from sklearn.model_selection import train_test_split

from sklearn.preprocessing import StandardScaler

from sklearn.neighbors import KNeighborsClassifier
from sklearn.svm import SVC
from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier

Next, we import the dataset:
    After reading the data using read_csv() looking at the data using the info() method, it can be observed that there are a total of 13 features and 1 target variable. There were no missing values and hence we did not need to take care of any null values.

Now, we move on to understanding the data:
    We first use the Correlation Matrix to find that there is no single feature that has a very high correlation with our target value. Additionally, some of the features have a negative correlation with the target value while some have positive.

    Now we use a simple command of dataset.hist() to get so much information in return in the form of Histograms. I observed that each feature and label is distributed along different ranges, which means we will need to scale.