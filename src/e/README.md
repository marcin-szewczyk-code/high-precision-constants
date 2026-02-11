# The Constant e

The mathematical constant **e** is defined as the value of the exponential function at 1:

e = e^1

In this project, the constant is computed using the Maclaurin series expansion of the exponential function:

e = sum_{k=0}^∞ 1/k!

## Numerical Approach

The computation is based on:

- iterative evaluation of successive terms \( 1/k! \)
- accumulation of the partial sum
- stopping criterion based on a prescribed tolerance (epsilon)

Because the factorial grows rapidly, the series converges very quickly and is numerically stable for moderate precision levels.

## Implementation

Current implementation:

- `e_long_double.c` – computation using `long double` precision

Further extensions may include arbitrary-precision arithmetic.
