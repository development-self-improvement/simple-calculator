Simple Calculator
========================

The purpose of this exercise is to make a simple C# calculator which will help the developer to start getting used to the language.

To start this project, make a fork of this repository into your public repository.

## Project 1 - Get it Working

Create a C# Console application which receives input from the command prompt (after start up).  The input should be in the form of an equation.

For example:

```
Please Enter an Equation:
> 1 + 2
```

The operations which are needed for this exercise are the following:
 - addition (+)
 - subtraction (-)
 - multiplication (*)
 - division (/)
 - exponents (^)

You should not be restricted to a simple equation.  For example, the following is a valid submission:

```
Please Enter an Equation:
> 1 + 2 + 3
```

After hitting the "Enter" key, we should see the answer displayed (ignore order of operations).

```
Please Enter an Equation:
> 1 + 2 + 3
Answer: 6
```

If the user specifies an operator that doesn't exist, you should give them an error saying it is an unrecognized operator.

**This project should reside in a folder named "project-1".**

## Project 2 - Improve Usability

This is an extension of the previous project.  However, in this project our focus will be on two things:
 - Order of Operations
 - Making a custom exception

### Order of Operations

Now that you have a simple calculator built, let's expand it so we follow the correct order of operations.  This means that you will need to walk through the entire equation that the user specifies in order to process it in the correct order.  Following the rules laid out by BEDMAS.

```
Please Enter an Equation:
> 1 + 2 * 3
Answer: 7
```

### Custom Exception

In the previous exercise, we simply gave the user an error message when something failed.  Now, it would be nice make our own exception which explicitly calls out the error.  More specifically, make a "InvalidOperatorException" get thrown if a person enters an unexpected operator.

**This project should reside in a folder named "project-2".**

## Project 3 - Improve Quality

The main objective for this project is to improve the overall quality of the application.  To do this, we must add unit tests to the project.  These tests will run through the calculator with known inputs, and validate that the output from our calculator meets expectations.

The test cases should go automatically run through and correctly calculate the following cases:

 - 5 + 2
 - 5+2
 - -2 + 3
 - 1
 - 5 * 2 + 3/4
 - 2 ^ 2
 - 5 * 2 ^ 0