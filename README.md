# Income-Classification<br/>
The goal of this project is to predict people's income categories, either '>50K' or '<=50K' based on various demographic attributes.<br/>

**Table of Contents<br/>**
• Get the Data<br/>
• Data Cleaning<br/>
• Exploratory Data Analysis<br/>
• Data Preprocessing<br/>
• Feature Selection and Clustering<br/>
• Classifiers
1. Logistic Regression<br/>
2. Decision Tree<br/>
3. Random Forests<br/>
4. Support Vector Classification<br/>
5. K-nearest Neighbors<br/>
6. Gaussian Naive Bayes<br/>
7. Quadratic Discriminant Analysis<br/>
8. AdaBoost<br/>
9. Gradient Boosting<br/>
10. Multi-layer Perceptron Classifier<br/>
  
**Imbalanced Dataset<br/>**
Many learning algorithms were designed assuming well-balanced class distributions, i.e. no significant differences in class prior probabilities. However, this is not always the case in real world data since one class might be represented by a large number of examples, while the others are represented by only a few, and this is the case for this dataset. The target variable "income" has imbalanced distribution with about 25% being '>50K" and 75% being "<=50K".

**The solution to the imbalanced data are mainly two types: data level methods and the algorithmic level methods.<br/>**

**Data level methods<br/>**
Data level methods consist of balancing classes by resampling the original data set, such that under-represented classes are over-sampled, and over-represented classes are under-sampled.

1. Random over-sampling(non-heuristic method)<br/>
It aims to balance class distribution through the random replication of minority class examples. Since it makes exact copies of examples from the minority class, which can increase the likelihood of overfitting.

2. Oversampling(heuristic method)<br/>
There are two approaches supported for generating new data points, Synthetic Minority Over-sampling Technique (SMOTE) and Adaptive Synthetic Sampling (ADASYN). Both techniques use interpolation to generate new datapoints. To be specific, SMOTE is an over-sampling method with synthetic data generation. Its main idea is to form new minority class examples by interpolating between several examples from the minority class that lie together. And ADASYN uses a weighted distribution for different minority class examples according to their level of difficulty in learning, where more synthetic data is generated for minority class examples that are harder to learn compared to those minority examples that are easier to learn.


3. Random under-sampling(non-heuristic method)<br/>
It aims to balance class distribution through the random elimination of majority class examples. But there is critic that under-sampling can eventually discard data potentially important for learning.


4. Undersampling(heuristic method)<br/>
Some heuristic under-sampling methods include NearMiss,Condensed Nearest Neighbor Rule,Tomek links, One-sided selection, Neighborhood Cleaning Rule. I implemented NearMiss, Tomek links and Neighborhood Cleaning Rule in this notebook.<br/>

**Algorithmic level methods:<br/>**
Idea: adapting existing algorithms and techniques to the especial characteristics of imbalanced data. These proposals include cost-sensitive learning, one-class classifiers, and ensembles of classifiers, among others.
