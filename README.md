# knn-algorithm
**This a brute force implementation of the KNN algorithm**, utilizing Euclidean Distance & Merge Sort functions. 
The K-Nearest-Neighbors algorithm, also known as KNN algorithm, where k is a number greater than 0, is most known for its usefulness in Machine Learning Applications. 
There are multiple applications of the KNN algorithm. For example, it can be used to solve classification problems, regression problems & missing data imputation problems.
It is considered an instance-based learning algorithm.
## Time Complexity
If n is equal to the number of points in the data set, k is equal to the number of neighbors we consider and d is the number of dimensions in the data set:
- Calculate distance to every other point:<br>
Ө(n)
- Sort all the distances using Merge Sort:<br>
Ө(nlogn)
- Calculate the frequency of each class to find k nearest neighbors:<br>
Ө(1)
- Overall Time Complexity:<br>
Ө(d*n2logn) 
- Note: There is no training phase, all computation is done during prediction phase.<br> 
*Time complexity will vary depending on sorting algorithm used
## Challenges
For this algorithm is important that the data set is distinct set of items. If the data set is not distinct the classification could be false.
If the set of items being classified are not distinct enough: <br>
- Introduce more classification parameters to make items distinct. Ex: Mass, color etc..
- Re-evaluate distances once the K closest items are selected to eliminate outliers.
## Suggestions for Improvment
- When k is an even number and a tie occurs between the k closest classes, introduce a function to determine which class would be better fit by evaluating the closest distances. 
- Using a data structure, like the KD tree or other tree structures, would optimize the algorithm’s overall performance and time complexity. 
- The value of k should be chosen with the data set in mind. If value of k is too large or too small depending on the data set could result in a false classification.
