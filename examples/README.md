# Run the examples locally

In your shell and directory of choosing do
```console
git clone https://github.com/PirxDanford/shUnit2-Workshop.git
cd shUnit2-Workshop
./examples/shunit2.test
```
if you see errors when running the shunit2.test, please check the setup README.md.

You might see errors when running the example code, this is fine as it is not meant to be successful on any given machine. For instance when doing the "testMachineArchitecture" test from check_requirements.test we are looking for x86_64, and maybe you are already on a quantum CPU or some ARM device, so it will fail.

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

# Precondition checking

## Version checks

In case your scripts depend on certain binary versions, you may want to check the installed versions.

Instead of doing this each time you run a script, this can be done in a central test file to be executed during troubleshooting an environment, or to be included in a precondition check.

To run the example do `./examples/preconditions/verify_versions.test`

> **Note**
> As version checking depends on a readable version format and changing versions always introduce compatibility uncertainties, the better approach is to test for the required functionality if possible.

## Requirement checks

You might have certain requirements, like directories being writable.

Some simple examples are included in

`./examples/preconditions/check_requirements.test`

# E-Mail checking

In this example we parse two textfiles and perform tests on each line:

`./examples/mailcheck/email_validity.test`

> **Note**
> See https://www.regular-expressions.info/email.html for details about why using regular expressions to match the RFC 5322 standard is error-prone.

# 
