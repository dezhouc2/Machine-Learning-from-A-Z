
```python
- multiple linear regression
  - ^Y = b0 + b1x1 + b2x2 + ... bnxn

- dummy variable trap

- p value
  - p-value is a criterion to check if factor/statement is important
  - confident level = 1 - significant level
  - significant level default as a = 0.05 which means i'm 95% confidence that ....
  
- 5 methods of building models:
  - all in (select all independent variables/use to prepare for backward elimination)
  
  - backward elimination
    - step1 select a significant level such as a = 0.05
    
    - step2 fit the full model with all predictor
    
    - step3 consider predictor with highest p-value and if p-value > significant level then delete this predictor
    
    - step4 fit model without this variable
    
    - step if all predictors' p-value are < significant level then our model is ready
    
  
  - forward selection
    
    - step1 select a significance level to enter the model 
    
    - step2 fit all simple regression model and select the one with lowest p-value
    
    - step3 keep this variable and fit all possible models with one extra predictor
    
    - step4 consider predictor with lowest p-value and if p < significant level then go to step3, else we done this model
  
  - bidirectional elimination
  
    - select a significance level to enter and to stay in the model such as slenter = 0.05, slstay = 0.05
    
    - perform forward selection (new variables needs to p < slenter to enter)
    
    - perform all steps of backward elimination (old variables needs to have p < slstay to stay)
    
    - no new can enter and no old can go, then our model is ready
  
  - score comparison
   - select a criterion 
   
   - build all possible of regression model
   
   - select the one with best criterion











```
