## **Decreasing Traffic Fatality in the U.S**

The United States is one of the busiest countries in terms of road traffic with nearly 280 million vehicles in operation. In 2018, there were some 12 million vehicles involved in crashes in the United States. Road collisions incur huge economic costs at a national level, which includes a burden on the health, insurance and legal systems. Moreover, they can have negative social implications for the families of those involved as well as on local communities.

**Goals**
---
The goal of this project is to group states that have similar profiles in fatal collisions. How can we find such groups in a statistically sound way and communicate the result effectively? Rather, than coming up with a strategy to reduce the no. of incidents of road accidents across the Country, it would be valuable to develop a state-focused plan. Further, I hope to show the total number of drivers involved in an fatal accident by cluster-group. 

**Table and Contents**
---
* [Dataset](https://github.com/mishaisran/Projects/blob/master/Predicting%20Credit%20Card%20Approvals/Data/cc_apps.data) - Retrived from the following [link](http://archive.ics.uci.edu/ml/datasets/credit+approval)
* [Notebook](https://github.com/mishaisran/Projects/blob/master/Predicting%20Credit%20Card%20Approvals/Code/CC_Apps_ML.ipynb) - Jupyter notebook used to clean, organize and analyze data.
* [Readme](https://github.com/mishaisran/Projects/blob/master/Predicting%20Credit%20Card%20Approvals/Readme.MD) - An overview of the dataset, method and summary of analysis.
* [License](https://github.com/mishaisran/Projects/blob/master/LICENSE) - MIT License

**Data**
---
The data set below shows the distribution of fatal car accidents throughout the U.S. This is a sample from 2012 of reported fatal collisions per billion miles including possible causes such as speeding, alcohol impairment, distraction, prior accidents, as well as car insurance premiums and losses incurred by insurance companies. There are 51 rows indicating states and 6 columns indicating the causes.

I use the a dataset created by five-thirty-eight, available [here](https://datahub.io/five-thirty-eight/bad-drivers)

| Field Name      | Type                                                    | 
| :---         | :---              | 
| **state**   | *string (default)*        | 
| **number of drivers involved in fatal collisions per billion miles**     | *number (default)*          |
| **percentage of drivers involved in fatal collisions who were speeding**     | *integer (default)*          | 
| **percentage of drivers involved in fatal collisions who were alcohol-impaired**     | *integer (default)*          | 
| **percentage of drivers involved in fatal collisions who were not distracted**     | *integer (default)*          | 
| **percentage of drivers involved in fatal collisions who had not been involved in any previous accidents**    | *integer (default)*          | 
| **car insurance premiums ($)**     | *number (default)*          | 
| **losses incurred by insurance companies for collisions per insured driver ($)**     | *number (default)          | 

**Packages and Softwares**
---
---
<pre>
Contributor  : <a href=https://github.com/Al-Cap>Misha Isran</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Jupyter Notebook
Libraries    : pandas, numpy, sklearn, labelencoder, logisticregression
</pre>
  </tbody>
</table>
