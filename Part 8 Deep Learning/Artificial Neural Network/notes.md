
```python
   * Practical:
     - deep learning MUST implement Feature scaling
   
   
     - difference between onehotencoder and labelencoder?
       
       - labelencoder only binary 0 or 1
       
       - onehotencoder contains multiple categorics

   
   Fitness: Artificial Netrual Network can be used for both regression and classification problems.
   
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
    
    
    * Gradient Descent(sometimes called batch Gradient Descent):
      Q: how these weights adjust?
      A: using Gradient Descent to find out the position of the optimal weights(minimize the cost function) by determining which way the slope goes
      
      
    * Stochastic Gradient Descent
      
      Q: what if the cost function if not convex?(not 1/2(expected y - y)^2) we can only find the local optimal but not global optimal
      A: using SDG 
      
      definition: for each of the row, run one time and then adjust the weight until finish running all of the rows
         - compare to gradient descent
            - run all of the rows and then update the weights
            
            - each time gradient descent runs, each of the rows gets the same result
      
      advantages:
         - avoid finding the local optimal but finding the global optimal instead
         - faster than GD
         
         
     * mini batch gradient descent:
         - run batches of 5,10 or 100 rows, run this number of rows at a time and then update the weights
      
     neutral network training process:
     * forward propagation:
         - get output layer from input layer and then hidden layer, then get the predicted Y and then calculate cost function 
         
     * backward propagation:
         - from cost function update weights via hidden layers
         
         - main key: able to adjust all of the weights at the same time(for each batch)
     
     
     * Training the Artificial Neural Network with Stochatic Gradient Descent:
         - Step1: randomly set the weights to small number close to 0 but not 0
         
         - Step2: input data, each feature for each row
         
         - Step3: forward propagation: from left to right, via weights, inner layer and outer layer to get the predict Y
         
         - Step4: compare the predicted result and the actual result. measure the generated error
         
         - step 5: backward propagation: from right to left, update the weights according to how much they are responsible for. 
                  Learning rates decides how much we update the weights.
          
         - Step 6: repeat step 1-5 and update weights after each row(Reinforcement Learning); or repeat step 1-5 but update the weights
                  after a batch of rows(batch learning)

         - step 7: when the whole training set passed via ANN, this makes an epoch. Redo more epochs.

```
