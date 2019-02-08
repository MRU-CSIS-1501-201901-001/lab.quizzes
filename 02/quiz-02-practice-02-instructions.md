# LAB QUIZ 02 - PRACTICE 02

This one might require you longer than 35 minutes - not much longer, hopefully. The actual quiz will be slightly easier than this one.

On the "real" quiz, you are free to use any resources you want, _with the exception of any other person, online or otherwise_.

The rubric for the real quiz is provided at the bottom of this document.

## YOUR TASK

Log onto INS and do the following:

1. Copy the directory `/users/library/csis/comp1501/quizzes/02/quiz-02-practice-02` to your home directory.
1. In the `src` directory of `quiz-02-practice-02`, create a source file for a class called `Redactor` that fulfills the requirements below. (There is already a working `Main` class source file in `src`. You do not need to alter it - it won't be marked - but if you want to play with it, be my guest.)
1. If you want to practice submitting: when done, please submit your `quiz-02-practice-02` directory using `submit1501`. When asked for the task identifier, use `quiz92`.

### REQUIREMENTS

The `Redactor` class was last seen in a week-01 drill. We're going to revisit it, but this time, give it some state. (That's fancytalk for "give it some instance variables".)

The behaviour of objects from this class will be much like we found in the drill - you can use Redactor objects to redact words out of a block of text. The differences this time around:

- a Redactor object always uses the same symbol (we'll call it the _overstrike symbol_) to overwrite text. This symbol is provided in the constructor call.
- a Redactor object now, instead of replacing only single symbols with overstrike symbols, can replace whole words.
  - for example, you could replace all instances of 'the' with '\*\*\*'
- a Redactor object can tell you whether the text you've given it has been **heavily redacted**, which we will take to mean **more than 50% of the characters in the text have been redacted**

What instance variables will the class have? You'll need to think about that; I **will** say you'll need more than the obvious one. Also, although the overstrike character comes in as a character, you might find it useful to store it as a String. The method you can use to do this is **Character.toString**. [for example, Character.toString('h') returns "h"]

The `Redactor` class needs to have a constructor and 4 **public** methods:

1. **constructor**

   - has one parameter: a **character** that will be used as the overstrike symbol

1. **redact**

   - has 2 parameters: the original text that will be redacted, and the word to redact
   - returns nothing
   - will replace all instances of the word to redact in the original text with the proper number of overstrike symbols
     - for example, in a redactor that has been created using `*` as the overstrike symbol, redacting the word "king" from the text "my kingdom for a horse" would result in "my \*\*\*\*dom for a horse"
     - in the `src` directory, there is a file called `helper.txt` - it contains a helper method you should use to help you with this, so copy and paste it into your class

1. **redactedText**

   - takes no parameters
   - returns the redacted text
   - if redact hasn't been called yet, returns an **empty string**

1. **heavilyRedacted**

   - takes no parameters
   - returns true if **more** than 50% of the characters in the original text have been redacted and false otherwise
   - **hint:** if you have a redacted String, like "my ####dom for a horse", and removed all the overstrike sybmols, you'd get "my dom for a horse". Is there some way of calculating the number of '#' there are from these 2 Strings?....

1. **toString**

   - making toString for each class you make is a good habit to get into; it comes in very handy for debugging
   - the toString for Redactor must have at the very least the value of the overstrike symbol present

#### NOTES

- if you wish to make any helper methods, declare them as **private** and **non-static**
- remember to save and compile often; I would recommend doing so after creating each method
- you can use the Main provided to see if your code is behaving reasonably; if you want to run Main, remember to compile it
- you may use the command `run tests` from the `quiz-02-practice-02` directory (NOT THE SRC!) to see if your code is behaving as expected

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
