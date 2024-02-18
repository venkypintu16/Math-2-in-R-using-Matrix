#Math operations on matrixes
A=matrix(c(2,0,1,3), ncol=2)
B=matrix(c(5,2,4,-1), ncol=2)
a = A+B
b = A-B
print(a)
print(b)

#Using the diag() function
X = diag(c(4,1,2,3),nrow=4,ncol=4)
print(X)

#Without using diag()  function.
Y = matrix(c(3,1,1,1,1,2,3,0,0,0,2,0,3,0,0,2,0,0,3,0,2,0,0,0,3),nrow=5,ncol=5)
print(t(Y))


#Using the diag() fuction for advanced.
diag_matrix = diag(2, 5, 5) + matrix(1, 5, 5)
diag_matrix[2:5, 1] = 2
diag_matrix[2,3:5] = 0
diag_matrix[3,2] = 0
diag_matrix[3,4:5] = 0
diag_matrix[4,2:3]= 0
diag_matrix[4,5]=0
diag_matrix[5,2:4]=0
print(diag_matrix)

OUTPUT:

> print(a)
     [,1] [,2]
[1,]    7    5
[2,]    2    2
> print(b)
     [,1] [,2]
[1,]   -3   -3
[2,]   -2    4
 

> print(X)
     [,1] [,2] [,3] [,4]
[1,]    4    0    0    0
[2,]    0    1    0    0
[3,]    0    0    2    0
[4,]    0    0    0    3

> print(t(Y))
     [,1] [,2] [,3] [,4] [,5]
[1,]    3    1    1    1    1
[2,]    2    3    0    0    0
[3,]    2    0    3    0    0
[4,]    2    0    0    3    0
[5,]    2    0    0    0    3
 
> print(diag_matrix)
     [,1] [,2] [,3] [,4] [,5]
[1,]    3    1    1    1    1
[2,]    2    3    0    0    0
[3,]    2    0    3    0    0
[4,]    2    0    0    3    0
[5,]    2    0    0    0    3


###########Explanation for the above R code on Matrix operations:

1. A and B are two matrices defined with matrix() function with specified values and number of columns.
2. a is the result of adding matrices A and B.
3. b is the result of subtracting matrix B from matrix A.
4. print(a) and print(b) display the results of addition and subtraction, respectively.

#Using the diag() Function:
5. X is a matrix created using the diag() function to form a diagonal matrix with the specified values.
6. print(X) displays the resulting matrix.

#Without Using diag() Function:
7. Y is a matrix created directly with specified values and dimensions.
8. t(Y) is the transpose of matrix Y.
9. print(t(Y)) displays the transposed matrix.

#Using the diag() Function for Advanced Operations:
10. diag_matrix is created by adding a diagonal matrix generated using the diag() function with a matrix of all 1s.
11. Various elements of diag_matrix are manually modified to achieve the desired pattern.
12. Finally, print(diag_matrix) displays the modified matrix.
