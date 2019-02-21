# LAB QUIZ 03 - PRACTICE 01

You should be able to complete this in **35 minutes**.

On the "real" quiz, you are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric for the real quiz is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/03/quiz-03-practice-01` to your home directory.
1. In the `src` directory of `quiz-03-practice-01`, create a source file for a class called `AverageFinder` that fulfills the requirements below. (There is already a working `Main` class source file in `src`. You do not need to alter it - it won't be marked - but if you wish to play with it, be my guest.)
1. If you want to practice submitting, then do the following: when done, please submit your `quiz-03-practice-01` directory using `submit1501`. When asked for the task identifier, use `quiz31`.

### REQUIREMENTS

The `AverageFinder` class creates objects that can calculate the average of a list of positive integers.

The list of numbers to average comes from a `NumberList` object that is passed in to the constructor. If you look in the source file for NumberList, you'll see that it has one public method called `nextNumber` that returns the next number in the NumberList object.

#### Example

Let's say we do the following:

```java
NumberList list = new NumberList("2 5 1 1 -1");
AverageFinder finder = new AverageFinder(list);
double avg = finder.avg(list); 
```

Then the variable `avg` should have a value of **(2+5+1+1) / 4**

#### Methods Needed

The `AverageFinder` class needs to have a constructor and 1 **public** method:

1. **constructor**

   - look at how the constructor is called in the static main to determine what its signature should be

1. **avg**

   - look at how this method is called in the static main to determine what its signature should be
   - should return the average of all numbers in the NumberList except for the final -1 (which denotes the end of numbers in the NumberList)
   - you can assume that every NumberList will always end with a -1
   - a NumberList might **only** have a -1 in it; in this case, `avg` should return -1

#### NOTES

- if you wish to make any helper methods, declare them as **private** and **non-static**
- remember to save and compile often; I would recommend doing so after creating each method
- you can use the Main provided to see if your code is behaving reasonably; if you want to run Main, remember to compile it first
- you may use the command `run tests` from the `quiz-03-practice-01` directory (NOT THE SRC!) to see if your code is behaving as expected
- reading the tests in `tests/AverageFinderTests.java` might be useful

---

## RUBRIC

Marking for the real quiz-03 will be a bit more strict than with quiz-01. You should be having fewer troubles compiling now.

### Grade: A

- compiles
- methods behave as expected, though 1 minor bug may be allowed
- follows all naming conventions (maybe with 1 or 2 minor slips)
- code is easy to read and understand because it is formatted nicely, everything is named expressively, and constants are used when appropriate

### Grade: B

- this is like an A level, but with more logical errors
- also, this is your grade if the code works as expected, but is noticeably (but not significantly) harder to read/understand because of formatting/naming issues and/or lack of convention-following

### Grade: C

- doesn't compile, but the instructor can tell that the methods present would work correctly, if not for some minor syntax issue; otherwise, everything else is at a B level
- you will also get a C level if the code compiles and behaves as expected, but significant slips in convention/formatting/naming make the code confusing and hard to follow

### Grade: D

- like a C level, but the instructor can see that numerous methods are incomplete or off-base

### Grade: F

- no attempt, or the code present is wildly incorrect
