# LAB QUIZ 01 - PRACTICE 01

You should be able to complete this in **35 minutes**.

On the "real" quiz, you are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric for the real quiz is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/quiz-01-practice-01` to your home directory.
1. In the `src` directory of `quiz-01-practice-01`, create a source file for a class called `BitSnake` that fulfills the requirements below. (There is already a working `Main` class source file in `src`. You do not need to alter it.)
1. If you want to practice submitting: when done, please submit your `quiz-01-practice-01` directory using `submit1501`. When asked for the task identifier, use `quiz91`.

### REQUIREMENTS

The `BitSnake` class represents an imaginary animal represented by a String consisting of 0 or more zeroes.

The `BitSnake` class needs to have 3 **public** methods:

1. **grow**
   - has no parameters
   - returns nothing
   - doubles the size of the BitSnake; that is, after growing, the BitSnake has twice as many 0's in it as it did before
1. **slice (no parameter version)**
   - has no parameters
   - returns nothing
   - cuts the BitSnake in half, so that it has 1/2 as many 0's (rounded down) as it did before. For example if our snake looks like **00000**, then:
     - slicing it would give you snake **00**,
     - slicing it again would give you **0**,
     - slicing it again would give you an "empty" snake (the empty String)
1. **slice (1 parameter version)**
   - takes one integer parameter (you can assume it's >=0 and < length of the snake), representing the index where the BitSnake should be "cut"
   - returns nothing
   - cuts the BitSnake at the given index, so that it now has as many 0's as there are from index 0 up to and including the given index. For example if our snake looks like **00000**, then:
     - slicing it at 0 would give you snake **0**,
     - slicing it at 1 would give you snake **00**,
     - slicing it at 2 would give you snake **000**
1. **toString**
   - like any good class that represents something "real", BitSnake has a toString
   - returns a reasonable String - you decide what "reasonable" is

#### NOTES

- all methods are small - only 1 or 2 lines of code
- remember to save and compile often; I would recommend doing so after creating each method
- you can use the Main provided to see if your code is behaving reasonably; if you want to run Main, remember to compile it

---

## RUBRIC

The marking for the real quiz will be different from the subsequent quizzes - we're going to be a bit more relaxed this time around, since it's your first real quiz and all.

### Grade: A

- compiles
- all methods behave as expected
- follows all naming conventions (maybe with 1 or 2 minor slips)
- code is easy to read and understand because it is formatted nicely, everything is named expressively, and constants are used when appropriate

### Grade: B

- this is like an A level, with more slips in convention, or perhaps is noticeably (but not significantly) harder to read/understand because of formatting/naming issues

### Grade: C

- doesn't compile, but the instructor can tell that the methods present would work correctly, if not for some minor syntax issue; otherwise, everything else is at a B level
- you will also get a C level if the code compiles and behaves as expected, but frequent slips in convention/formatting/naming make the code confusing and hard to follow

### Grade: D

- like a C level, but the instructor can see that numerous methods are incomplete or off-base

### Grade: F

- no attempt, or the code present is wildly incorrect