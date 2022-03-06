# Credit Risk Analysis - Using Credit Card Data to Analyze Credit Risk Using Python SKLEARN Package
## Summary
We have been given a data set from LendingClub of credit card credit to determine if the information can be used to predict credit risk of customers. With the help of Sklearn in Python, we will look at a few machine learning techniques to see if we can use the data to make reasonable accurate predictions. 
## Results
**1.) Naive Random Oversampling**
![ROS](https://github.com/jraguDataGuy/Credit_Risk_Analysis/blob/main/Resources%20-%20PNG%20Files/Naive%20Random%20Over%20Sampling.png)
This technique takes random selections of our minority classes, add them to the training set until the majority and minority classes are balanced. For our test, our balanced accurracy score was at 64% with precision for our high risk clients as low

**2.) Synthetic Minority Oversampling Technique**
![SOS](https://github.com/jraguDataGuy/Credit_Risk_Analysis/blob/main/Resources%20-%20PNG%20Files/SMOTE%20Over%20Sampling.png)
In SMOTE, th esize of the minority is increased. The key difference betwee the two oversampling techniques lies in how th eminority class is increased in size. Values of the minority classses closest neighbors are selected and new values are then created. Our balance accuracy score was at 62%, with precision still very low for high risk. 

**3.) Undersampling**
![US](https://github.com/jraguDataGuy/Credit_Risk_Analysis/blob/main/Resources%20-%20PNG%20Files/Undersampling.png)
In our oversampling exercise, we continue to see a decline in accuracy, as oversampling comes in at 52%. Precision continues to be an issue for high risk

**4.) Synthetic Minority with Edited Nearest Neighbors**
![Smoteen](https://github.com/jraguDataGuy/Credit_Risk_Analysis/blob/main/Resources%20-%20PNG%20Files/SMOTEEN%20OVer%20and%20Under%20Sampling.png)
This technique has us oversample with SMOTE, then cleans the resulting data with an undersampling strategy. Accurracy is still at 63%, with precision issues staying consistent. 

**5.) Balanced Random Forest**
![Forest](https://github.com/jraguDataGuy/Credit_Risk_Analysis/blob/main/Resources%20-%20PNG%20Files/Balanced%20Random%20Forest%20Classifier.png)
Our accuracy level increases to 78%, with our first spike in high risk precision. However, this change isn't significant enough to warrant celebration. 


**6.) Easy Ensemble AdaBoost**
![Ada](https://github.com/jraguDataGuy/Credit_Risk_Analysis/blob/main/Resources%20-%20PNG%20Files/Easy%20Ensemble%20AdaBoost%20Classifer.png)
Our accuracy level is the highest of the tests at over 92%. Howevr, precision for High Risk still remains low. 

## Conclusion
Ultimately, the precision of the models to accurately capture high risk customers would make me hesitant to recommend any of the models. Our Easy Ensemble AdaBoost model had the best accuracy, but still struggled to be a precise fit for high risk customers, which would be the more valuable of customer to predict. 
