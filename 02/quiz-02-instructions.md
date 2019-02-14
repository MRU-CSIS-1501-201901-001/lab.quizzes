# LAB QUIZ 02

**WEIGHT: 4%**

You have **35 minutes** to complete the following tasks.

You are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric for this quiz is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/02/quiz-02` to your home directory.
1. In the `src` directory of `quiz-02`, create a source file for a class called `SuperCar` that fulfills the requirements below. (There is already a working `Main` class source file in `src`. You do not need to alter it.)
1. When you are done, please submit your `quiz-02` directory using `submit1501`. When asked for the task identifier, use `quiz2`.

### REQUIREMENTS

The `SuperCar` class creates objects that represent a car with a manual transmission: though most manual transmission cars available today have 4 or 5 gears, the SuperCar cars can have as many gears as the user requires.

When a SuperCar is made, it has a highest gear (which is provided in the constructor) and a lowest gear of -1, which represents Reverse. (0 represents Park).

So, for example, if a SuperCar is made with a highest gear of 3; it has the following gear range available:

- -1: Reverse
- 0: Park
- 1
- 2
- 3 (the highest gear)

The `SuperCar` needs to have a number of instance variables; you should be able to figure out which ones.

The `SuperCar` class needs to have a constructor and 4 **public** methods:

1. **constructor**

   - takes 1 integer parameters: the highest gear the car can use. A new car should start in 0.

1. **shiftUp**

   - takes no parameters
   - returns nothing
   - increases the current gear by 1; if the car is already in its highest gear, nothing happens

1. **shiftDown**

   - takes no parameters
   - returns nothing
   - decreases the current gear by 1; if the car is already in its lowest gear (-1), nothing happens

1. **gear**

   - takes no parameters
   - returns the current gear the car is in; this is **usually** a number, with 2 exceptions:

     - if the car is in gear -1, this method should return "R"
     - if the car is in gear 0, this method should return "P"

1) **toString**
   - making toString for each class you make is a good habit to get into; it comes in very handy for debugging
   - the toString for SuperCar must have at the very least the values of its instance variables

#### NOTES

- if you wish to make any helper methods, declare them as private and non-static
- remember to save and compile often; I would recommend doing so after creating each method
- you can use the Main provided to see if your code is behaving reasonably; if you want to run Main, remember to compile it
- you may use the command `run tests` from the `quiz-02` directory (NOT THE SRC!) to see if your code is behaving as expected

---

## RUBRIC

Marking for the real quiz-02 will be a bit more strict than with quiz-01. You should be having fewer troubles compiling now.

### Grade: A

- compiles
- methods behave as expected, though 1 minor bug may be allowed
- follows all naming conventions (maybe with 1 or 2 minor slips)
- code is easy to read and understand because it is formatted nicely, everything is named expressively, and constants are used when appropriate

### Grade: B

- this is like an A level, but with more logical errors
- also, this is your grade if the code works as expected, but is noticeably (but not significantly) harder to read/understand because of formatting/naming issues and/or lack of convention-following
- OR, if your code is basically an A-level solution...with 1 or 2 **minor** syntax errors

### Grade: C

- doesn't compile, but the instructor can tell that the methods present would work correctly, if not for some minor syntax issue; otherwise, everything else is at a B level
- you will also get a C level if the code compiles and behaves as expected, but significant slips in convention/formatting/naming make the code confusing and hard to follow

### Grade: D

- like a C level, but the instructor can see that numerous methods are incomplete or off-base

### Grade: F

- no attempt, or the code present is wildly incorrect
