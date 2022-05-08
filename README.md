# Tape Equilibrium test

Ref: https://www.youtube.com/watch?v=gTgRfjIQMYw&list=PLZAjJcBlySRiNm4GMxbHQaAOzTr7iAf6c

A non-empty array A consisting of N intergers is given. Array A represents numbers on a tape.
Any integer P, such that 0<P<N splits this tape inte two non-empty parts:
A[0], A[1], ... , A[P-1] and A[P], A[P+1], ... , A[N-1]

The difference between the two parts is the value of 
|A[0], A[1], ... , A[P-1] - A[P], A[P+1], ... , A[N-1]|

In other words, it is the absolute difference between the sum of the first part and the sum of the last part. 

For example, consider array A such that:
A[0]=3
A[1]=1
A[2]=2
A[3]=4
A[4]=3

We can split the tape in four places:
P=1, difference = |3-10|=7
P=2, difference = |4-9|= 5
P=3, difference = |6-7|= 1
P=4, difference = |10-3|=7

Write a function:
    def solution(A)

that, given a non-empty array A of N integers, return the minimal difference that can be achieved. 

With the given A array the minimum absolute sum difference will be 1. 

Write an efficient algorithm for the following assumptions:
-N is an integer within the range [ 2.,100000 ]
-each element of array A is an integer within the range [-1000,1000]

#/////////////////////////////////////////////////////////////////////
Solution 
For efficient code do not use sum in a for loop solution , replace it with a matrix multiplication solution.
