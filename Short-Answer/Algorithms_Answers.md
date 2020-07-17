#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a)

> **O(n)**

> At first glance, the thought is `O(n*n*n)`, but evaluation of the operation in the loop changes things. The operation adds `n*n` to an accumulator (a) every iteration. because `n*n` is part of the iteration evaluation of `n*n*n`, we can factor that portion out to a constant `1`. As a result, we can rewrite as `O(1*n)` and further condense to `O(n)`.

b)

> **O(n(log n))**

> I initially thought this was `O(n*n)`, but I can see that the inner loop reduces the number of iterations exponentially by adding `2*j`. As a result, I chose `O(n(log n))` as the number of iterations will be greater than `O(n)`, but less than `O(n*n)`

c)

> **O(n)**

> A recursive algorithm that reduces the input by `1` for each call to the itself, and no more calls to itself is inherently `O(n)`. As this function doesn't do anything to the input within, it will run `O(n)` times.

## Exercise II

> I would use a binary-search algorithm

```
- Are min and max search heights the same?
    - Yes: We've found the heighest floor

    - Otherwise...
- set floor f to 1/2 of max search height and min search height
- Drop and egg
- Did the egg break?
    - YES: reduce the max search height to 1 less than floor
    - NO: increase min search height to 1 more that floor
- Repeat

```
