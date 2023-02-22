
```python

The following metrics are for regression problems

* R-squared

  - can be negative, the model performs poorly
  
  
  - Rule of Thumb for model performance
  
   - 1.0 = perfect fit(suspicious)
   
   - ~0.9 = very good
   
   - < 0.7 = not great
   
   - < 0.4 = Terrible
   
   - < 0 = Model makes no sense for this data


  - idea: R^2 = 1 - (SSres // SStot)
    - SSres = sum(yi - y^i)^2 also name ordinary least square
     
    - SStot = sum(yi - yavg)^2




* adjusted R-squared
  
  - adju R^2 = 1 - (1-R^2) * (n-1)/(n-k-1); k = number of independent variables; n = sample size
    - 如果regression model有多个变量，则adjust r^2 可以用来判断哪些变量是对当前模型有帮助 哪些变量没有帮助
      - 如果对当前模型加了一个新的变量, 且这个变量是有帮助的则, r^2和 adjust r^2的差距会小 否则会大
        - 另外一种判断是: 新变量有用 则 adjust r^2会变大 否则会变小
    




```
