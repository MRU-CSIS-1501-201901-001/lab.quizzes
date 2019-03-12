# LAB QUIZ 04 - PRACTICE 02

You should be able to complete this in **45 minutes**.

You are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/04/quiz-04-practice-02` to your home directory.
1. In the `src` directory of `quiz-04-practice-02`, create a source file for a class called `RoomInventory` that fulfills the requirements below.
   - There is already a working `Main` class source file in `src`. You do not need to alter it - it won't be marked - but if you wish to play with it, be my guest.
   - There is a also a class called `Room` that has been done for you. You should not alter its code, but you will want to read it, as you need to know what its public methods are in order to complete this practice quiz.
1. If you want to practice submitting, then do the following: when done, please submit your `quiz-04-practice-02` directory using `submit1501`. When asked for the task identifier, use `quiz42`.

### REQUIREMENTS

The `RoomInventory` class creates objects that represent a collection of Rooms that we want to track.

#### Methods Needed

The `RoomInventory` class needs to have the following 4 **public** methods (a constructor is not required, though you may add a no-arg one if you wish):

1. **add(`Room`)**

   - adds the given Room to the end of the current collection of Rooms

1. **numRooms()**

   - returns the number of Rooms in the inventory

1. **roomsWithCapacityAtLeast(`int`)**

   - returns an ArrayList<Room> that contains all Rooms in the inventory that have a capacity AT LEAST as large as the given target capacity
   - if no rooms are in the inventory that fulfill the requirement, this method returns an empty ArrayList

1. **view()**

   - returns a String that is a formatted view of the RoomInventory; see the following section for its format
 
#### About the `view` method

The view method needs to show, for each Room in it, the room's name and capacity. Here's an example:

```java
[T225 (43), Y210 (112)]
```

You may notice that the format of this view is simply the default toString of an ArrayList. Use this to your advantage here....

#### NOTES

- if you wish to make any helper methods, declare them as **private** and **non-static**
- remember to save and compile often; I would recommend doing so after creating each method
- you can use the Main provided to see if your code is behaving reasonably; if you want to run Main, remember to compile it first
- you may use the command `run tests` from the `quiz-04-practice-02` directory (NOT THE SRC!) to see if your code is behaving as expected
- reading the tests in `tests/RoomInventoryTests.java` might be useful

---

## RUBRIC

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
