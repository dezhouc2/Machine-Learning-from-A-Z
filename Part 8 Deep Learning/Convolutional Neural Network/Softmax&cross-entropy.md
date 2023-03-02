
```python
  
  Q: how does categories know they need to sum up to 1?
  A: Applying softmax function, each of categories has a Z-score in the range of [0,1] which will add up all categories to 1
  
  * softmax function:
    1. a generalization of logistic function

    2. generate each of the categories in the range of [0,1] that sum up as 1
    
  
  * Cross-entropy:(now the cost function is called lost function)
    - fitness: if it's categorical problem, then we use cross-entropy, use mean squared error if it's regression problem
    
    
    
    Q: why use cross-entropy over mean squared error?
    A: help the CNN to get into optimal state
    

















```
