# Factorial

## Basic definition and properties

The factorial of $n\in\N$ is defined as: $$ n! = \prod\limits_{k=1}^{n} k $$

We can easily deduce that $$ n! = n\cdot (n-1)! $$

## Implementation

Here's a recursive `python` implementation
```{python}
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)
```

Let's call this function for $n=4$
```{python}
print(factorial(4))
```