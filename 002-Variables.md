# Variables
One of the main keystones of computer programming, variables are an essential concept to learn and practice.  

## What are Variables?

##### Math
Let's talk about equations for just one second.  Think back to early geometry class.  Consider the equation used to calculate the area of a circle.

![pi * r^2](http://3.bp.blogspot.com/-DLfHKpBTmDM/VnOABBrLdjI/AAAAAAAAA6w/R6H_mNz0GTE/s1600/Capture.PNG)

That's right, the area is equal to pi times the radius squared.  There are actually 2 types of variables in this equation.  One is there because.. well the value is different for every circle; that's the radius `r`.  We know that any radius value will work in this equation, so we put a symbol to represent the radius there.

The second type of variable in this case is pi.  It's only there in place of the real value to make it **easier to read**.

##### Computer programming
In short variables are a space allocated in the computer's memory to store a value.  The variable is given a name which can be used to reference that value in your program.  Here's an example of the same equation as before, the area of a circle, in javascript.

```javascript
var radius;
var area;
var pi = 3.14159;

area = pi * (radius^2);
```

Now the actual syntax and implementaion of variables will be slightly different between technologies.  But there is generally 2 steps.  The first is the **declaration** of the variables, you see that on the top of the example above.  We're telling the computer "hey, I'm going to need a variable with this name, make a spot for it in your memory and get ready to stuff some value into that spot whenever I need you to."

## Readability
The example above could also be written like this
```javascript
var r;
var a;

a = 3.14159 * (r^2);
```

This is a slightly bad example, because of how simple and recognizable this equation is.  But at a glance it might be hard to tell what the heck is going on here.  The same can happen to your real code when your variables are given poor names.

##### Make sure names are expressive
Unless it's a very well known abbreviation **don't abbreviate your variable names**.  The code should be easy to read as a human that knows english words.

##### Avoid magic numbers
Notice also that you could put the _value_ of pi right there in the equation, and in this case that'd be fine.. since pi is an easy to recognize and unchanging number.  But it's better to just assign it to a variable and give it a name that's meaningful.

## Types
It's very hard to talk about the concept of variables without also discussing the concept of **types**.  Types define what _kind_ of values you are allowed to store in a variable.  Let's cover the most basic types:

* **String** - A string of text characters, can't be used in math.  Usually defined using quotations. e.g. `firstName = "Shawn"`
* **Integer** - A whole number, can be used in math.  No quotes necessary. e.g. `numberOfPlayers = 75`
* **Float** - A floating point number.  Things get complicated when you want to store a real numeric value containing a decimal.  This could be the subject of an entire lesson, but for now just know that if you want to store decimals you need a flaoting point number. e.g `pi = 3.14159`

> It's worth noting, that **Integer** and **Float** have numerical specific ranges of numeric values that can be used.  For very large integers there's usually some type of **BigInteger** which can store rediculously large numbers.  Similarly for floating point numbers there is usually a **Double** type which can store a much more precise number than the single float.

There are other types and we'll get into them later.  For now this is all you need to know.

**But wait** in the example above no type was specified.  Yeah, you're right.  Types are implemented differently in different programming languages.  I'm not going to get into that, as it's pretty advanced stuff.  All you need to know is that some languages require you to be explicit about the type of a variable and some languages allow you to be implicit about the type of a variable.

Some languages allow both!  Let's take a look at some C# code.

```cs
// this value is compiled as an integer
var implicitInteger = 5;

// this value is also compiled as an integer
int explicitInteger = 5;
```

## See it in action
Ok open up https://repl.it/languages/QBasic save the new session with some meaningful name, maybe 002-variables.

##### A new keyword DIM
In QBasic the `DIM` keyword is used for defining variables.  Don't worry about the actual meaning of dim and what it stands for.  There's some historical reason that it's used which doesn't make any sense in the modern world, so don't worry about it.

Let's look at some real QBasic code which defines some variables

```
DIM firstName AS STRING
DIM age AS INTEGER
DIM heightInFeet AS SINGLE

firstName = "Shawn"
age = 29
heightInFeet = 6.166666667

PRINT "Hi my name is "; firstName; "."
PRINT "I am "; age; " years old."
PRINT "I am "; heightInFeet; " feet tall."
```

Put that in the editor and hit run ▶, feel free to put in your info instead of mine.  Note that the keyword for a single floating point number in QBasic is `SINGLE` in many other languages this would just be `FLOAT`.

##### Two ways to express variable types in QBasic
QBasic has an interesting feature in which you can define the type of a variable by using special characters at the end of the variable name.

```
DIM firstName$
DIM age%
DIM heightInFeet!

firstName$ = "Shawn"
age% = 29
heightInFeet! = 6.166666667

PRINT "Hi my name is "; firstName$; "."
PRINT "I am "; age%; " years old."
PRINT "I am "; heightInFeet!; " feet tall."
```

This example will work just the same.  For these lessons we will **always use type names** and never use the variable name to express type.  But in the case that you are googling code examples I wanted you to be aware of this type of variable declaration.

## Finished
Play around with variables if you want.  Once your'e done, click the "share" button and send me a link to your repl.it session.