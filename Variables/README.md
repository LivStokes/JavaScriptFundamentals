# camelCase

Camel case is the practice of writing phrases without spaces or punctuation, indicating the separation of words with a single capitalized letter, and in this course the rst word will start with a lower-case letter.

# Variables

Variables are containers for storing values.
Assigning a variable does not return a value. Variable names do not have to be a single letter. A variable name can contain letters, digits, underscores, and dollar signs.

# 1. Console Log

JavaScript variables can be declared in 4 ways:
- Using let
- Using const
- Using var (Not Recommended)
- Automatically (Not Recommended)

To open the console log where I can enter code.
- Open Chrome. ctrl, shift, i.

e.g.
let x = 3
let y = 5
let result = x + y

Click the eye, write in result. Then it will display the result = 8.

By using const, we create a variable that cannot be changed. We can see the value, but we can’t change it.
Constants can make your code more robust ensuring values that shouldn’t change can’t be changed.

e.g.
const z = 7
by entering z = 8, an error message will appear.

# Variable Strings

A variable can be a word or a sentence
let myName = "Olivia Stokes"
This variable is called a string.

But what happens if we add together myName and x, a string and a number?
Because myName is a String the plus operation doesn’t try to convert myName to a number, instead it converts x into a String and joins this on the end of myName, giving, Olivia Stokes3.

Can you create 3 variables, rstName, lastName and fullName?  When creating fullName use the variables rstName and lastName and put a space between  them. Put the book down and give it a try.

let firstName = "Olivia"
let lastName = "Stokes"
let fullName = firstName + " " + lastName

to check, enter fullName.