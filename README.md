# Digit-Recognition

In Short : 
Recognize Digits (28 x 28 pixels with each pixel having value between 0 to 255) by comparing deviation of each pixel of input from average of each group of training set where training set is divided into 'div' number of groups and returning the digit which appears maximum times in 'knn' lowest deviations.

In Detail : 

1) Taking the MNIST Dataset of digits
2) Taking some data and calling it the training set
3) Define a variable called 'div'. Dividing the training set into 'div' number of groups
4) Taking the average of the pixel values for each digit in each group (Now we have ('div' x 10) average matrices)
5) Define a variable called 'p' i.e. power. Taking Deviation (comparing) each average with the test input (Sum of 'p' of differece of values of each pixel between the test matrix and the respectice average)
6) Define a variable called 'knn'. Finding how many times each digit appears in the lowest 'knn' deviations.
7) Output the digit that appears maximum number of times. (Default output is the digit with lowest deviation)

Accuracy (depends on size of training set, 'div', 'knn', 'p') : Around 85% (75-90% in most cases)
