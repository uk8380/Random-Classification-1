### EX NO:01
### DATE: 04.04.2022
# RANDOM CLASSIFICATION
## AIM:
To write a python program to perform random classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## Related Theoritical Concept:
Random classifier: It creates a set of decision trees from randomly selected subset of training set. It then aggregates the votes from different decision trees to decide the final class of the test object. Random Forest is suitable for situations when we have a large dataset, and interpretability is not a major concern.

Purpose of Random classifier: One of the most important features of the Random Forest Algorithm is that it can handle the data set containing continuous variables as in the case of regression and categorical variables as in the case of classification.

## Algorithm
1.In Random forest n number of random records are taken from the data set having k number of records.<br/>
2.Individual decision trees are constructed for each sample.<br/>
3.Each decision tree will generate an output.<br/>
4.Final output is considered based on Majority Voting or Averaging for Classification and regression respectively.<br/>

## Program:
```
/*
Program to implement random classification.
Developed by   : SHAIK KHADAR BASHA
Register Number : 212220230045
*/
import matplotlib.pyplot as plt
from sklearn import datasets
x,y=datasets.make_blobs(n_samples=100,n_features=2,centers=2,cluster_std=1.05,random_state=2)
fig=plt.figure(figsize=(10,8))
plt.plot(x[:,0][y==0],x[:,1][y==0],'r^')
plt.plot(x[:,0][y==1],x[:,1][y==1],'bs')
plt.xlabel("feature 1")
plt.ylabel("feature 2")
plt.title('Random Classification Data with 2 classes')
```

## Output:

![NN(1)](https://user-images.githubusercontent.com/75235233/164286781-d6776f27-aa8e-4039-8d30-82e76880845c.png)


## Result:
Thus the random classifier was successfully implemented using python programming.
