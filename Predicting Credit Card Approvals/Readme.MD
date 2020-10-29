## **Predicting Credit Card Approval using Machine Learning**

![Cover](https://github.com/mishaisran/Projects/blob/master/Predicting%20Credit%20Card%20Approvals/Images/Cover_CCA.PNG)

**Navigating this Repo**
---
* [Dataset](https://github.com/mishaisran/Projects/blob/master/Predicting%20Credit%20Card%20Approvals/Data/cc_apps.data) - Retrived from the following [link](http://archive.ics.uci.edu/ml/datasets/credit+approval)
* [Notebook](https://github.com/mishaisran/Projects/blob/master/Predicting%20Credit%20Card%20Approvals/Code/CC_Apps_ML_.ipynb) - Jupyter notebook used to clean, organize and analyze data.
* [Readme](https://github.com/mishaisran/Projects/blob/master/Predicting%20Credit%20Card%20Approvals/Readme.MD) - An overview of the dataset, method and summary of analysis.
* [License](https://github.com/mishaisran/Projects/blob/master/LICENSE) - MIT License

**Motivation and Background**
---
In this project, I use the Credit Card Approval Dataset from the UCI Machine Learning Repository to build a machine learning model that can predict whether an individual's application for a credit card will be approved or denied. The objective to is decide the outcome of a credit card application based on attributes such as income, age, employment status, credit history etc. 

The process of reviewing applications manually is time-consuming and is prone to error. However, with the power of Machine Learning, we can automate this task. Predicting whether an individual has been approved for a credit card is a classification problem. Logistic regression is used because we are predicting binary classes i.e. the probability that a response falls into two possible outcomes of whether an application will be approved or denied. 

**Dataset**
---
I use the Credit Approval Dataset from the UCI Machine Learning Repo, available [here](http://archive.ics.uci.edu/ml/datasets/credit+approval)

| Feature      | Description                                                    | 
| :---         | :---              | 
| **Dataset Characteristics**   | *Multivariate*        | 
| **Attribute Characteristics**     | *Categorical, Integer, Real*          |
| **Number of Instances**     | *690 rows*          | 
| **Number of Attributes**     | *15 columns*          | 
| **Missing Values**    | *Yes*          | 
| **Associated Tasks**     | *Classification*          | 


This dataset is fascinating because there are a good mix of attributes: continuous, nominal with small numbers of values, and nominal with larger numbers of values. Since this data is confidential, the feature names have been anonymized. There are also a few missing values. For numeric values, mean imputation was used to replace the NaN values - a method in which the missing value on a certain variable is replaced by the mean of the available cases to replace these values. For the columns that contained non-numeric data where mean imputation I imputed the missing values with the most frequent values in the respective column. This method allows me to maintain the sample size. We drop two columns, DriversLicense and ZipCode, as they are not essential features for determining approval for a credit card. 

**Conclusion**
---
I used a confusion matrix to describe the performance of this classification model as it is important to check whether our machine learning model is able to predict the approval status of the applications as denied that had originally been denied. The first analysis was made by calculating the confusion matrix function from sklearn.metrics for predicting credit card approval and disapproval status, the results obtained were ([[60, 10],[13, 55]]) and accuracy of logistic regression classifier: 0.8333333333333334 ~ 84%. This is a good percentage reflecting high accuracy. 

However, to improve the model’s ability to predict credit card approvals, a grid search was performed on two parameters: tolerance for stopping criteria and maximum number of iterations. The values inputted were: tol = [0.01, 0.001 ,0.0001] and max_iter = [100, 150, 200]. Grid Search used a five-fold cross-validation and the best score achieved was 0.852174 ~ 85%.

**Project Info**
---
<pre>
Contributor  : <a href=https://github.com/Al-Cap>Misha Isran</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Google Collab
Libraries    : pandas, numpy, sklearn, labelencoder, logisticregression
</pre>
  </tbody>
</table>
