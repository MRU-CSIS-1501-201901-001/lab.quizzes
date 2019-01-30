# LAB QUIZ 01

**WEIGHT: 3%**

You have **35 minutes** to complete the following tasks.

You are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric for this quiz is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/01/quiz-01` to your home directory.
1. In the `src` directory of `quiz-01`, create a source file for a class called `CoffeeCup` that fulfills the requirements below. (There is already a working `Main` class source file in `src`. You do not need to alter it.)
1. When done, please submit your `quiz-01` directory using `submit1501`. When asked for the task identifier, use `quiz1`.

### REQUIREMENTS

The `CoffeeCup` class represents a single cup of coffee. This cup can hold 591 mL of coffee and starts off being full.

The `CoffeeCup` class needs to have 4 **public** methods:

1. **sip**
   - has a single integer parameter, which is the size of the sip - an integer that you can assume will be 0 or greater
   - returns nothing
   - reduces the amount of coffee in the cup; needs to make sure the amount of coffee in the cup never goes below 0 [hint: might there be a Math method you've seen before that will help you here....]
1. **topUp**
   - has no parameters
   - returns nothing
   - sets the amount of coffee in the cup back to its starting amount (of 591 mL)
1. **amountLeft**
   - has no parameters
   - returns the amount of coffee currently in the cup
1. **toString**
   - like any good class that represents something "real", CoffeeCup has a toString
   - returns a reasonable String - you decide what "reasonable" is

#### NOTES

- most methods are only 1 line of code; `sip` will likely be 2
- remember to save and compile often; I would recommend doing so after creating each method
- you can use the Main provided to see if your code is behaving reasonably; if you want to run Main, remember to compile it

---

## RUBRIC

The marking for this quiz is different from the subsequent quizzes - we're going to be a bit more relaxed this time around, since it's your first real quiz and all.

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