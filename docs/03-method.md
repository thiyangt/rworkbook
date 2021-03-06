# Built-in Functions in R

## Lecture slides

<iframe src="https://hellor.netlify.app/slides/l32021.html#1" width="672" height="400px"></iframe>

## Probability Functions

1. A continuous random variable $X$ is said to have the Normal distribution with mean ($\mu$), 5 and variance ($\sigma^2$), 9. Let $f_X(x)$ and $F_X(x)$ denote the probability density function and cumulative distribution function of $X$ respectively. Write R codes to find

    a. $f_X(4)$
    
    b. $F_X(4)$
    
    c. $F_X^{-1}(0.5)$
  
2. Let $X \sim Binomial(6, 0.5)$. Write R codes to calculate the followings:

    a. $P(X=3)$ 
  
    
    b. $P(X \geq 3)$  
    

    c. $P(X \leq 1)$ 
    
<!--(ans. 0.313)-->

<!--(ans. 0.656)-->

<!--(ans. 0.109)-->

3. Write R codes to visualize the probability mass function of $Y \sim Binomial(6, 0.2)$.



## Matrix calculations

The matrices $P$ and $Q$ are defined as follows

$$
	P = \begin{bmatrix} 
	3 & 5 & 4 \\
	3 & 4 & 8\\
	7 & 6 & 5 \\
	\end{bmatrix},
	\quad
	Q = \begin{bmatrix} 
	1 & 5 & 4 \\
	2 & 5 & 7\\
	3 & 6 & 5 \\
	\end{bmatrix}.
$$

1. Write R codes to solve the following problems:

    a. Find the determinant of the matrix $P$.
    
    b. Find the transpose of the matrix $P$.
    
    c. Find the inverse of the matrix $P$.
    
    d. ${P'P}^{-1}$
    
    e. $P + Q$
    
    f. $P - Q$
    
    g. $P \times Q$


2. Write R codes to solve the following problems:
    
    a. Generate a random sample of size 1000 from the $Uniform(0, 5)$ store in a vector called `sample.unif`.
    
    b. Find the number of values greater than 2.5 in the vector `sample.unif`. 
    
    c. Construct a 100x10 matrix to store the values in the vector `sample.unif`.
    
    d. Calculate and store the mean and median of each column of the matrix.


