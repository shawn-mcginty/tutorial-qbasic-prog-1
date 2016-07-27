# Hello World
It's traditional that your first program on a new platform be a "hello world" program.  This is a simple program which will output some text to the user *(namely, it should say "hello world")*. 

##### What we will cover
* Where to find the tools you will need for these lessons
* How to write and run a program using said tools

## Tools
1. Your favorite web browser
2. https://repl.it/languages/qbasic

That's it.  We'll be using repl.it, which is a cool web sandbox for many different programming languages.  In our case we will be working with **QBasic**.  I want to keep tooling to a minimum.  I don't want you getting bogged down with setup, that's not the point of this class.

## QBasic
This is the programming language we'll be using.  It's old, busted, and you'll never use it in real life.

> QBasic (Microsoft Quick Beginners All purpose Symbolic Instruction Code) is an IDE and interpreter for a variety of the BASIC programming language which is based on QuickBASIC. Code entered into the IDE is compiled to an intermediate representation, and this IR is immediately interpreted on demand within the IDE. -- https://en.wikipedia.org/wiki/QBasic

##### Why QBasic for this class?
- **There's no magic** - many modern languages do a bunch of stuff for you behind the scenes.  I want you to understand why the code you're typing gives the results that you see.
- **It's not Object Oriented** - c#, java, and others will all require some object oritned boilerplate code just to run simple non-object-oritned programs.  For this reason, I wanted to use a language without this noise.  Learn the basics first.. then get into object oriented programming.
- **You'll never use it in real life** - this may sound counterproductive but hear me out.  By using a language that you won't find in later course work and in the real world of programming I'm preventing you from getting attached to syntax.  Infact you'll be **forced** to apply the concepts learned here to other languages/technologies.  This is, in my opinion, a critical skill to learn.  Be language agnostic.

## repl.it
Bookmark https://repl.it/languages/qbasic or whatever, we'll be using it for the remainder of this class.  Also it's probably best to create an account.  It's a simple web app that allows you to execute some code and view the output in your browser.  

##### Why repl.it?
So you don't have to install/setup the qbasic tool on your local computer.  Also for non-windows users (qbasic is windows only!).  It also makes it easy for you to share the completed coursework with me.

## The Lesson
##### 1. PRINT
`PRINT` is a built in funciton of QBasic.  It takes in some text and will then output that text to the console for the user to see.

* Open https://repl.it/languages/qbasic
* Name the session, whatever makes it easy for you to keep track of probably something like "001-Hello World"
* In the editor do the following
```purebasic
PRINT "Hello World!"
```
* Click the run ▶ button
* Verify the output on the right

##### 1.1 Semicolons and commas
Try the following on the next line in the editor:
```PureBasic
PRINT "Hello"; " "; "again!"
```

>The semicolon let's print run on multiple inputs.

Try this:
```PureBasic
PRINT 1,2,3,4
```
Commas will put a tab between the arguments, instead of printing them right next to eachother.  Also note that we're using numbers instead of strings here.. `PRINT` doesn't care.

## Finished
Play around with `PRINT` if you want.  Once your'e done, click the "share" button and send me a link to your repl.it session.