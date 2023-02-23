
```python
  * note: while doing feature scaling(standardization), the range is [-3,3]
    training: while doing prediction, the feature needs to be the same format as the training feature
    - for example, if training feature transforms, then the testing features also need to be transformed in order to predict..

  * definition: predict a categorical depdent variable from a number of independent variables
  
  * function: ln(p/1-p) = b0 + b1x1
    - returns probability as output
  
    - p defines as probability
    
    - sigmoid curve
      - x as the input; y as the output for a defined probability
      
      - if this probability >= 50% then "yes"(can be binary 0/1 type), else then "no"
      
    
    - maximum likelihood
      - motivation: while given multiple sigmoid curves
        how do we know which curve is the best one?(like linear regression, can have multiple linear curve)
      
      - comparing the values of many likelihood to find the best curve(highest value)
      
  
   * Confusion Matrix(show us the status how many predicts are true/false)
     - accuracy score: showing the percentage of the correct prediction

    
   * linear classifier:
     - linear boundary 区分0和1的线
     
     - cons: 有一些dp会预测错误


```
