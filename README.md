# computase
an algorithm that groups proteins based on their characteristics 
###### Input:
computase works by taking in proteins in a vector form and running one of the algorithms listed below.
Each protein can be encoded as a "characteristic vector." The vector will have dimension n, with each dimension representing a pivotal component of the protein. For example, protein x could be encoded as [15, 20, 2, 0.1, ...], where 15 could represent its location, 2 could represent its optimal pH, etc. 
###### Machine Learning Approach:
The first method be to use the standard machine learning model of multiplying an input by a weight and bias matrix and rezizing its dimension as an m dimensional vector. For example, after passing through a series of weight and bias matricies, the output for a protein could be [a = 0.8, b = 0.2, c = 0.1, d = 0.1], which would indicate that the protein functions as "a." A significant challange with this approach is its reliance on a training data set to determine the values in the weights and bias matrix.
###### Density Based Approach:
The second method involves graphing the vectors in n-dimensional space, and using a standard clustering algorithm (such as DBSCAN) to group them based on density. A flaw in this method is a lack of a guarantee of proper grouping. 
