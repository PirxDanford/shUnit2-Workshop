# Using a function

For this example a function is defined, with 2 execution variants.

In random_echo it is being called immediately and the value is being echoed.

In random_silent it is just being defined, so that we can include it and use it as needed.

## random_silent

To include the function as command in your shell, or in another script you can use "." or "source".

Run `./examples/function/random_silent.test` to perform the tests for the function.

If the tests pass we know that awk is working well with the srand function and that our function works as intended.

## random_echo

Extends random_silent and introduces parameters with default values to directly echo a result.

If the tests pass we additionally can be sure that parameters can be used as expected.


# TODO: add more examples

- version check
- email ismail nomail (sed test)
- precondition for docker build
