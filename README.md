# DATA PREPROCESSING

# 1.Need to import libraries and modules in to the program
 
  import numpy as nm
  import matplotlib.pyplot as mtp
  import pandas as pd
  
# 2.we have to load the dataset
data_set = pd.read_cv("BENGULAR_DATASET")

# 3. Extract the dependent and independent variables into data set for location(iloc: stands for index location)
x = data_set.iloc[::-1]

y = data_set.iloc[::1]
# 4. split the dataset into two parts for testing and training
#sklearn.library

from sklearn.model_selection import train_test_spilt:
x_train,x_test,y_test,y_train = train_test_split(x,y,test_size=0.3, random_state=5)

# 5. FIT THE LINEAR REGRESSIONFOR TRAING DATA
from sklearn.model import Linearregression;
regressor = LinearRegression;
regressor.fit(x_train,y_train)

# 6. predict the value's that correct output or not
y_predict = regressor.predict(x_test)
x_predict = regressor.predict(y_train)

# 7.  we will go for validation for traing dataset;
mtp.scatter()(x_train,y_train,colour = "Green");
mtp.plot(x_train,y_predict,colour = "Red");
mtp.title("bath, totalsqfoot, bhk vs "prices")
mtp.x_label("Toatlsqfoot, bhk, bath");
mtp.y_label("prices");
# 8. then after we have to do the validation on testing the same instead of x_train,y_train we use x_test, y_test;
conclusion: linear regression is the Best fit model execution


![image](https://github.com/manikantareddychamala/PREDICTING-REAL-ESTATE-PRICE-A-COMPARATIVE-ANALYSIS-OF-LINEAR-REGRESSION-AND-SUPPORT-VECTOR-MACHINE/assets/162694056/c65e6102-d161-4bd6-9433-44212d37b59f)


# support vector machine process in machine learning
from sklearn.model import svc(classifer)
classifer = support vector machine
classifier.fit(x_train,y_train)
# 2. predict the values
y_train = classier.fit(x_train)

# 3. validation on train set results
# 4. validation on test set results
[
![image](https://github.com/manikantareddychamala/PREDICTING-REAL-ESTATE-PRICE-A-COMPARATIVE-ANALYSIS-OF-LINEAR-REGRESSION-AND-SUPPORT-VECTOR-MACHINE/assets/162694056/7514b35a-d017-4f07-bbc3-67ac81ab6fec)
](url)


# 5. CONCLUSION : Finally after doing two Algorithm executions we got the best fit model performance is "SUPPORT VECTOR MACHINE"(SVM) . We got the predected values and actual values are equal in svm model

