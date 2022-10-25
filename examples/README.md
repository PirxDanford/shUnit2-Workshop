# Run the examples locally

In your shell and directory of choosing do
```console
git clone https://github.com/PirxDanford/shUnit2-Workshop.git`
cd shUnit2-Workshop
./examples/shunit2.test
```
if you see errors, please check the setup README.md.

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

# Version checking

In case your scripts depend on certain binary versions, you may want to check the installed versions.

Instead of doing this each time you run a script, this can be done in a central test file to be executed during troubleshooting an environment, or to be included in a precondition check.

To run the example do `./examples/versioncheck/verify_versions.test`

> **Note**
> As version checking depends on a readable version format and changing versions always introduce compatibility uncertainties, the better approach is to test for the required functionality if possible.

# TODO: add more examples

- email ismail nomail (sed test)
- precondition for docker build
