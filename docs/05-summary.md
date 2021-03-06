# Writing Functions in R


## Lecture slides

<iframe src="https://hellor.netlify.app/slides/l52021.html#1" width="672" height="400px"></iframe>

## Problems



1. Write an R function to compute the sample excess kurtosis.

2. Write an R function to convert a vector of numeric values to the corresponding z-score vector.

3. Write an R function to generate $n$ random numbers from a normal distribution **and** $m$ random numbers from a uniform distribution. 

4. The secant method for finding the solution of an equation of the form $f(x)=0$ is

$$x_n=x_{n-1} - \frac{(x_{n-1}-x_{n-2})f(x_{n-1})}{f(x_{n-1})-f(x_{n-2})},$$

where two initial guesses $x_1$ and $x_2$ must be specified beforehand.

The `secant` function given below can be used to find the solutions of a functions using the secant method.


```r
secant <- function(x1, x2, f){

fx1 <- f(x1)
xdiff <- x2 - x1
repeat{
fx2 <- f(x2)

if (abs(fx2) < 1e-8) break
x <- x2 - xdiff*fx2/(fx2 - fx1)
xdiff <- x - x2
x2 <- x
fx1 <- fx2
}
x
}

```



a. Write a function named `f1` which takes a single argument $x$ and returns the values of the function below

$$f(x) = e^{-x} - x.$$


b. Apply the `secant` function to find the solution of $e^{-x} - x = 0.$ Help: Use -1.5 and -0.5 as your starting guess.
