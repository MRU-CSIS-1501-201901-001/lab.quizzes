# LAB QUIZ 02 - PRACTICE 01

You should be able to complete this in **35 minutes**.

On the "real" quiz, you are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric for the real quiz is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/02/quiz-02-practice-01` to your home directory.
1. In the `src` directory of `quiz-02-practice-01`, create a source file for a class called `TicketVendor` that fulfills the requirements below. (There is already a working `Main` class source file in `src`. You do not need to alter it - it won't be marked - but if you wish to play with it, be my guest.)
1. If you want to practice submitting, then do the following: when done, please submit your `quiz-02-practice-01` directory using `submit1501`. When asked for the task identifier, use `quiz921`.

### REQUIREMENTS

The `TicketVendor` class creates objects that can calculate the cost of a ticket based on the age of the ticket's target user and a given tax rate.

Think of the situation you see at a typical movie theatre in Calgary:

- if your age is under 14, you pay one price (a **child** price)
- if your age between 14 and 64 (inclusive), you pay another price (an **adult** price)
- if your age is 65+, you pay another price (a **senior** price)

For your TicketVendor class, you **must** use the following for age limits:

- an adult is anyone from 14 to 64 years old, inclusive
- a child is anyone **under** 14
- a senior is anyone **over** 64

The `TicketVendor` needs to have 3 instance variables; you should be able to figure out which ones. (I'll give you a hint: it's **not** the age thresholds, because they're always the same for our purposes.)

The `TicketVendor` class needs to have a constructor and 2 **public** methods:

1. **constructor**

   - takes 3 double parameters: the price or a child ticket, the price of an adult ticket, and the price of a senior ticket

1. **ticketPrice**

   - takes 2 parameters: the age of the person the ticket is for in whole years, and the tax rate as a whole number - for example, for a tax rate of 12%, this parameter **would be 12, not 0.12**
   - returns the price (as a double) of the correct kind of ticket **including the tax**

1. **toString**
   - making toString for each class you make is a good habit to get into; it comes in very handy for debugging - the current main() uses the toString (do you see where?)
   - the toString for TicketVendor must have at the very least the values of the 3 ticket prices to **3 decimal places**

#### NOTES

- if you wish to make any helper methods, declare them as **private** and **non-static**
- remember to save and compile often; I would recommend doing so after creating each method
- you can use the Main provided to see if your code is behaving reasonably; if you want to run Main, remember to compile it first
- you may use the command `run tests` from the `quiz-02-practice-01` directory (NOT THE SRC!) to see if your code is behaving as expected

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

### Grade: C

- doesn't compile, but the instructor can tell that the methods present would work correctly, if not for some minor syntax issue; otherwise, everything else is at a B level
- you will also get a C level if the code compiles and behaves as expected, but significant slips in convention/formatting/naming make the code confusing and hard to follow

### Grade: D

- like a C level, but the instructor can see that numerous methods are incomplete or off-base

### Grade: F

- no attempt, or the code present is wildly incorrect
