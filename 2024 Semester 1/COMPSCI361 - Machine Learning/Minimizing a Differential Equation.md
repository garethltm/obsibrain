Simple approach to minimizing a differentiable function $f$
1. Take the derivative of $f$
2. Find points w where the derivative $f'(w)$ is equal to 0 (extreme point - max/min)
3. Choose the smallest one (& check that $f''(w)$ is positive)

Note that this problem:
$$f(w) = \textstyle\sum_{i=1}^n(\huge {wx}\tiny {i}-\huge {y}\tiny {i}\normalsize)^2$$
Has the same set of minimizers as this problem:
$$f(w) = \frac {1}{2}\textstyle\sum_{i=1}^n(\huge {wx}\tiny {i}-\huge {y}\tiny {i}\normalsize)^2$$
& this:
$$f(w) = \frac {1}{n}\textstyle\sum_{i=1}^n(\huge {wx}\tiny {i}-\huge {y}\tiny {i}\normalsize)^2$$
& this:
$$f(w) = \frac {1}{2n}\textstyle\sum_{i=1}^n(\huge {wx}\tiny {i}-\huge {y}\tiny {i}\normalsize)^2$$