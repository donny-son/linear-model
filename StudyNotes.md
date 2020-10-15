---
title: Linear Models Study Notes
author: Dongook Son
---

# Chapter 1

## Intro

It all comes down to predicting unobserved future events. In order to achieve the objective we would assume the following condition regarding the error term.
$$
 e \sim N(0, \sigma^2I)
$$
Two linear methods are commonly applied.

1.  Regression ($y_i = \beta_0 + \beta_1 x_i + e_i$)
2.  ANOVA ($y_{ij} = \mu + \alpha _i + e_{ij}$)

These are both linear in a sense that the parameters($X$) are linear with the design matrix($X$). The equation comes from the same source($Y= X\beta + e$). For the regression case, the design matrix is a spanned set of {$\mathbf{1}, columns(data)$}. On the other hand, for the ANOVA case, the deisign matrix is spanned from the set {$\mathbf{1}, \mathbf{j}_i$} where $\mathbf{j}_i$ is a vector with value 1 for the i-th element and others being all 0 for $\forall i$. 

## Random Vectors and Matrices

Let $\mathbf{y} = [y_1, y_2, …, y_n]$ where all $y_i$'s are random variables. 
$$
\mathrm{E}(Y)=\mathrm{E}\left[\begin{array}{c}
y_{1} \\
y_{2} \\
\vdots \\
y_{n}
\end{array}\right]=\left[\begin{array}{c}
\mathrm{E} y_{1} \\
\mathrm{E} y_{2} \\
\vdots \\
\mathrm{E} y_{n}
\end{array}\right]=\left[\begin{array}{c}
\mu_{1} \\
\mu_{2} \\
\vdots \\
\mu_{n}
\end{array}\right]=\mu
$$




# Midterm Exam Expected questions


## Chapter 1

### Exercise 1.3

Show that $Cov(Y)$ is nonnegative definite for any random vector $Y$. 

**Note that $Y$ is non-singular iff $Cov(Y)$ is positive definite**. 

### Theorem 1.3.3

If $Y$ is a random vector with $Y \sim N(\mu, I)$ and if $M$ is any perpendicular projection matrix, then $Y' MY \sim \chi^2 (r(M), \mu' M \mu /2)$. 