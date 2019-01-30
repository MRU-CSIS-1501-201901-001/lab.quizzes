# LAB QUIZ 01 - PRACTICE 02

You should be able to complete this in **35 minutes**.

On the "real" quiz, you are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric for the real quiz is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/01/quiz-01-practice-02` to your home directory.
1. In the `src` directory of `quiz-01-practice-02`, create a source file for a class called `QuarterWrapper` that fulfills the requirements below. (There is already a working `Main` class source file in `src`. You do not need to alter it.)
1. If you want to practice submitting: when done, please submit your `quiz-01-practice-02` directory using `submit1501`. When asked for the task identifier, use `quiz92`.

### REQUIREMENTS

The `QuarterWrapper` class represents a device used to wrap quarters into standard rolls (which hold 40 quarters).

I normally wouldn't tell you this, but for this one, I will: you should make 2 private int instance variables: one for the number of loose quarters this "machine" has, and one for the number of rolls it has. These should both start off as 0.

The `QuarterWrapper` class needs to have 5 **public** methods:

1. **receive**
   - has one parameter: an integer number of quarters this wrapper is to receive (you can assume it will be >= 0)
   - returns nothing
   - should increase the number of loose quarters this machine has by the given amount
1. **wrap**
   - has no parameters
   - returns nothing
   - takes all the loose quarters this machine has and wraps as many as it can; any that can't be wrapped are kept loose (remember there are 40 quarters in a full roll)
     - this sure seems a lot like our egg/egg carton thing...
1. **numRolls**
   - has no parameters
   - returns the number of rolls this machine currently has
1. **numLoose**
   - has no parameters
   - returns the number of loose quarters this machine currently has
1. **toString**
   - like any good class that represents something "real", QuarterWrapper has a toString
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
