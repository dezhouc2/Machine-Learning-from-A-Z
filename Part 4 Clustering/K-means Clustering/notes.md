
```python
  
  * definition: grouping unlabelled data
  
  * K-means Clustering intuition:
    - Step1: select the numbers of clusters
    
    - Step2: randomly placed centroid into the plot for each of the cluster;几个cluster = 几个centroid
    
    - Step3: K-means assign each of the data points to the closest centroid
    
    - Step4: draw a line that differentiate the clusters
    
    - Step5: calcualte new centroids for each of the clusters via taking average of X coordinates and average of Y coordinates for each of the data points
             for each cluster
             
    - Step6: repeat step3-5 until the process do not change anything
    
    
  
  * Question: how many clusters to select for the first step?
    * The Elbow method:
      - WCSS: calculate the sum of distance (Pi, C1)^2 for each of the Cluster
      
        - distance(Pi,C1)^2 = distance between each point and Centroid 1
        
        - WCSS will be smaller and smaller(to 0 which is the smallest) as the increase of numbers of clusters
        
        
  * K-means ++:
    
    - definition: based on K-means algo
    
    - Step1: choose the first centroid at random among the data points
    
    - Step2: for each of the remaining data points, compute the distance to the nearest of selected centroids
    
    - Step3: choose next centroid among the remaining data points using eighted random selection - weighted by distance^2
    
    - Step4: repeat Steps 2 and 3 until all k centroids have been selected
    
    - Step5: proceed with standard k-means clustering















```
