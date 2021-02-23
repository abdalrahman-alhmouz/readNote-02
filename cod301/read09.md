# Functional Programming

### What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data .

### What makes a function pure?

1. It returns the same result if given the same arguments (it is also referred as deterministic)
2. It does not cause any observable side effects

### Pure functions benefits

1. The code’s definitely easier to test
2. We don’t need to mock anything.
 So we can unit test pure functions with different contexts:
- Given a parameter A → expect the function to return value B
- Given a parameter C → expect the function to return value D

### Functions as first-class entities

* Functions as first-class entities can:

1. refer to it from constants and variables
2. pass it as a parameter to other functions
3. return it as result from other functions

The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.

### Higher-order functions
mean a function that either:
1. takes one or more functions as arguments, or
2. returns a function as its result

like : filter, map, and reduce

### Refactoring JavaScript for Performance and Readability

take long URl and return short URL
