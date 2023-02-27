
```python
  * supervised vs un-supervised:
    supervised: know what to predict
    
    un-supervisd: do not know what to predict

  * Confusion Matrix
    第二个index是跟着 prediction的neg/pos走的
      
                      Prediction
                    NEG                            POS 
A      NEG       TRUE/NEG                    FALSE/POS (type I error)

Ctual  POS       FALSE/NEG(type II error)        TRUE/POS


    * accuracy rate = correct(TN + TP) / total
    
      error rate = incorrect(FP + FN) / total = 1 - accuracy rate



    * CAP curve vs  ROC curve
    
      q1: how to use CAP curve to demonstrate how good the model is?
      a1: calculate Area P(perfect model) from the top / Area in the bottom; usually it's a percentage between 0 and 1 


```
