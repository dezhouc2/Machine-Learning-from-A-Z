
```python
   
   idea: input layers, hidden layers and output layers; how these three layers interact with each other.
   
   - input layer: a combination of many values such as X1,X2....Xm
     - value: each of the values represent a kind of features
   
     - action: weight each of the values and then pass into inner layer
       
     - purpose of weight: denote which values are important
   
   - inner layer: sum of wixi for i = 1,....m and then apply activiation function and then signal pass into output layer
     
     * activation function:
       - sigmoid function: y = 1/(1 + e^(-x))
       
       - thresold function: y = 1 if x >= 0 and y = 0 if x < 0
       
       - rectify function: y = max(x,0)


   - output layer: apply sigmoind function and then output values 
   
   
   Question: how do neural network learn?
   
   Overall component:
      
      input layer X = [X1,X2,...,Xm]; each of the Xi is a feature
      
      Weighted matrix W = [W1,W2,...,Wm]; the weight is the same for all row
      
      hidden layer = sum(wixi) for i = 1,...m
      
      output layer = expected Y = [y^1, y^2, ..., y^m]
      
      real output Y = [y1,y2,...,ym ]
      
      Cost function = 1/2*sum((y^i-yi)^2) for i = 1,...,m 
   
   This whole process is called Back Propagation:
      idea: (find the optimal weights which is minimize the cost function)
        Step1: each of the rows train and result one expected yi

        Step2: calculate each of the cost function i for each (yi^,yi) pair, then calculate the sum of cost function

        Step3: adjust matrix W using sum of cost function 

        Step4: repeat Step 1 - 3
     





```
