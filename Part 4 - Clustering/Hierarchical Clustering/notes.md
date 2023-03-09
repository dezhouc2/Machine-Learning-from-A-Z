
```python
  
  * Agglomerative Hierarchical clustering:
    - Step1: make each data point as a single point cluster => forms N clusters
    
    - Step2: take two cloest data points and make them one cluster => forms N-1 clusters
    
    - Step3: take two cloest clusters and make them one cluster => form N-2 clusters
      - Q: distance between two clusters
        - option1: calculate the euclidean distance between two cloest points from two clusters
        
        - option2: calculate the euclidean distance between two centroids from two clusters
    
    - Step4: repeat step3 until only one cluster left
  
  * Dendograms:
    
    - finding the optimal number of clusters via 
      1. find the largest distance within the diagram
      2. drawing a horizontal line crossing the distance and see #numbers of intersections(#nums of clusters)
      
    
    




```
