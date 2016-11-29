# User Input
Most of the time a computer needs to take some input from a user in order for it to be useful.  We're going to spend some time looking at different ways this is done.  We'll also implement a simple user input program in QBasic.

## What is User Input?
User input can be almost anything the user does.  It might be mouse clicks, it might be button presses on a game pad, it might be keyboard, it might be microphone.  Whatever your app is intending to do you can bet that you'll need to handle some input from a user.

## See it in action
Ok open up https://repl.it/languages/QBasic save the new session with some meaningful name, maybe 003-user-input.

##### A new keyword INPUT
In a simple command line QBasic application like this, getting input from the user is very simple.  We'll use the `INPUT` keyword.  The format is something like this:

```
INPUT "Message to the user", variable
```

This causes the command line to prompt the user for some input, the input is then stored as the value of `variable`.

##### Simple app
We're going to write a very basic program which will prompt the user for some input, then return the uppercased version of whatever the user typed in.

```
DIM test AS STRING

INPUT "Please type a message to be upper cased:", test

PRINT "Here you go..."
PRINT UCASE$(test)
```

This is all stuff you know already!  Except the new keyword `INPUT` and we are using a **build in** function called `UCASE$` this takes in a string and will output the uppercase version of that string.  Go ahead and ▶ Run.  Type some input into your program and hit enter.

## Finished
Play around with this as much as you want.  Once your'e done, click the "share" button and send me a link to your repl.it session.