# Machine Learning Notes

## Introduction

"A computer program is said to learn from experience E with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P, improves with experience E."

### Supervised Learning

The "right answers" are given.

Examples:
- Interpolating within existing data to predict the price of a given house
- "Regression" problems: trying to predict a continuous valued output
- "Classification" problems: trying to predict a discrete valued output

### Unsupervised Learning

No "right answers" given. Given a data set, can we find some structure in it?

Single value decomposition, clustering

## Model and Cost Function

Notation:
- `m`: Number of training Examples
- `x`: Input variables / features
- `y`: Output / target variables
- `(x^{(i)}, y^{(i)})`: `i`'th training example

Training set => Learning Algorithm => `h`.

h is a _hypothesis_ function, which maps from `x` to `y`.

h_{\\theta}(x) = \\theta_0 + \\theta_1 x

Linear regression in one variable

How do we choose the thetas?
Answer: Minimize the _average of the squares of the residuals_ / 2
This is the "squared error cost function"
(We divide by 2 by convention, because that makes the math easier when we
  take the derivative, because the square term cancels out the 1/2)
