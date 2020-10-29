## **Predicting Credit Card Approval using ML Techniques**

![Cover](https://github.com/mishaisran/Projects/blob/master/Predicting%20Credit%20Card%20Approvals/Images/Cover_CCA.PNG)

**Overview**
---
In this project, I use the Credit Card Approval Dataset from the UCI Machine Learning Repository to build a machine learning model that can predict whether an individual's application for a credit card will be approved or denied. The objective to is decide the outcome of a credit application based on attributes such as income, age, employment status, credit history etc. The process of reviewing applications manually is time-consuming and is prone to error. However, with the power of Machine Learning, we can automate this task. Logistic regression is used because we are predicting binary classes i.e. the probability that a response falls into two possible outcomes of whether an application will be accepted or denied. 

**Dataset**
---
I use the Credit Approval Dataset from the UCI Machine Learning Repo, available here: *http://archive.ics.uci.edu/ml/datasets/credit+approval*. 

| Feature      | Description                                                    | 
| :---         | :---              | 
| **Dataset Characteristics**   | *Multivariate*        | 
| **Attribute Characteristics**     | *Categorical, Integer, Real*          |
| **Number of Instances**     | *690 rows*          | 
| **Number of Attributes**     | *15 columns*          | 
| **Missing Values**    | *Yes*          | 
| **Associated Tasks**     | *Classification*          | 


This dataset is fascinating because there are a good mix of attributes: continuous, nominal with small numbers of values, and nominal with larger numbers of values. Since this data is confidential, the feature names have been anonymized. There are also a few missing values. For numeric values, mean imputation was used to replace the Nan values - a method in which the missing value on a certain variable is replaced by the mean of the available cases to replace these values. For the columns that contained non-numeric data where mean imputation I imputed the missing values with the most frequent values in the respective column. This method allows me to maintain the sample size. 

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
