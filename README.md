# Python-code-for-P-centre-problem
This python code provide optimal solution for famous P-centre problem in Optimization. Three different codes for three different data sets has been provided.
Problem Statement: Given a set of n points and the distance dij between any two points i and j, find a set of p centers such that the maximum distance from any non-center to its nearest center is minimized. Formulate this problem as an integer program.

Mathematical Model for P-centre problem: Decision variables:
x_ij = 1, if  ith non-center point is defined to jth center point, 0 otherwise.
Where i=1 to N & j=1 to N , Where N is the total number of points.
y_j = 1, if jth is the center point, 0 otherwise.
Where j= 1 to N
Objective function:
Minimization MD
Subject To:
x_ij d_ij≤MD . . . . . .∀ i=1 to N & j=1 to N
∑_(j=1)^n▒x_ij =1 . . . . . ∀ i=1 to N
∑_(j=1)^n▒y_j =p
x_ij≤y_j . . . . . ∀ i=1 to N & j=1 to N
x_ij ∈ {0,1} . . . . . . . . ∀ i=1 to N & j=1 to N
y_j  ∈ {0,1}. . . . . . . . . . . ∀ j=1 to N
