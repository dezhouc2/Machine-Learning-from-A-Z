
```python

* import data
  - sklearn module and class within module

* data cleaning
  - encoding transformation
    -  convert numeric to categorical for logistic regression
    - convert categorical to numeric for linear regression
  
  - feature scaling(purpose: to avoid the bias within data)
    - * applying the feature scaling after the splitting data into training set and testing set to avoid bias
    - normalization
      - diff: maybe affected by outliers bc predefine the range such as [0,1] or [-1,1] and more fit with normal distribution
      - X` = (X - Xmin) / (Xmax - Xmin)
      - normalize each data within a column in the range [0,1]
    
    - standardization（z-score normalization)
      - diff: may not be affected by the outliers
      - X` = (X - average) / standard deviation.  
      
  - 

* split into training and test sets
  - split dataset into training(80%) and testing(20%) 











```
