# Predict if Kyphosis was cured after surgery

In this repository is used a small dataset which essentially represents a number of patients who had **Kyphosis** which is a spinal condition and then they had an operation. The operation was a corrective spinal surgery and the Kyphosis column basically represents whether the Kyphosis condition was absent or present after the operation.

This data set contains the following features:

- Kyphosis: whether the Kyphosis condition was absent or present after the operation
- Age: the age of the person in months. (As this is data on children)
- Number: number of vertebrae involved in the operation
- Start: the number of the first or top most or vertebrae that was operated on

Not getting much into the medical terminologies, here we really just deal with all these columns as numbers and the Kyphosis as essentially a target *absent* or *present*.

Exploratory Data Analysis visually using **seaborn** by plotting all the variables against each other using pairplot with value colors defined by the column *'Kyphosis'* to check the impact on it with each changing parameter.Scikit learn also has some built-in visualization capabilities for decision trees. The decision tree is visualised using the ```pydotplus``` library and ```export_graphviz``` module which is processed with [graphviz](http://graphviz.org/) .These have to be installed as:
  ```  
      pip install pydotplus
  ```
  
  ```
      conda install -c anaconda graphviz
  ```

A Decision Tree classifier and some Random Forest classifier models are created and then predictions are made for the test data. 

Then the model performance is evaluated by calculating the Classification Report and Confusion matrix for some suitable number of estimators values observed.

# Requirements:
- numpy
- pandas
- matplotlib
- seaborn
- sklearn
- pydotplus
- graphviz




