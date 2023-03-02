
```python
  * what are convolutional neural network?
    - purpose: image classification


    - idea:
      - input image -> cnn -> output label(classify image)
      
      - input image * feature detector(convolution) = many feature map(get the important features from the image) => regard as convolutional layer
        next, adding rectifier as activated function(purpose is to add non-linearity to avoid linearity) -> apply pooling(get the pooling layer)
        -> get the pooled feature map -> step 3
      
      - 对机器学习来说, 照片是一个matrix而且照片中的特征是matrix中的一些数字
      
      
    - how cnn classifies?
      - eg: black and white image -> transfer into 2d array
      
      - eg: green,red,blue image -> transfer into 3d array

    - overall process:
      note:
        - weights and feature detectors both are adjusted in the gradient descent process
    
    
      - step 1: convolution
        
        - convolution operation
        
        - ReLU layer
          - use rectifier as the activated function
      
      - step 2: max pooling
          - benefit:
            - reduce number of parameter to avoid overfitting
            
            - max value of a matrix to capture the feature not matter how the image change
      
      - step 3: flattening
          - convert the pooled feature map into 1 X m matrix as the input layer of a future ANN
      
      - step 4: full connection
         - a type of hidden layer in ANN(in CNN it's fully connected which means each node in hidden layer connects to all nodes in input layer)
         
         - a cost function is calculated by how well our network performs and we try to minimize this cost function
      
         - feature detectors are adjusted(vs how weights are adjusted in ANN)
         
         - neurons in the full connection votes for the categories via the weights(through forward propagation and backward propagation) + iterations + epoches
     
     


```
