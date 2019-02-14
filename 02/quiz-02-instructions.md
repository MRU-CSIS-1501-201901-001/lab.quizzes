# LAB QUIZ 02

**WEIGHT: 4%**

You have **35 minutes** to complete the following tasks.

You are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric for this quiz is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/quiz-01` to your home directory.
1. In the `src` directory of `quiz-01`, create a source file for a class called `CoffeeCup` that fulfills the requirements below. (There is already a `Main` class source file in `src`.)
1. When done, please submit your `quiz-01` directory using `submit1501`. When asked for the task identifier, use `quiz1`.

### REQUIREMENTS

The CoffeeCup class represents a single cup of coffee. This cup can hold 591 mL of coffee and starts off being full.

The CoffeeCup class needs to have 4 **public** methods:

1. **sip**
   - has a single integer parameter, which is the size of the sip - an integer that you can assume will be 0 or greater
   - returns nothing
   - reduces the amount of coffee in the cup; needs to make sure the amount of coffee in the cup never goes below 0 [hint: might there be a Math method you've seen before that could help you here?....]
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
- you can use the Main provided to see if your code is working reasonably

## RUBRIC

The marking for this quiz is different from the subsequent quizzes - we're going to be a bit more relaxed this time around, since it's your first real quiz and all.

| Mark | What I'm looking for |
| ---- | :------------------: |
| A    |          a           |
| B    |          b           |
| C    |          c           |
| D    |          d           |
| F    |          f           |
