# The Building Blocks of Computer Science

This section will go over the basic elements of Computer Science. We generally want to work with some forms of **data**. Our data can be just about anything: numbers, words, types of food, you name it! Just dealing with data by itself can be a bit boring, we want to be able to modify our data. To do this, we can create **functions**.

## Primitives

Some basic types of data that we will discuss early on are numbers like 10,20, 1.1233, or -11000. The next type is the string, which we define as a set of characters in quotations. Below are a few examples of our terminal output if we input some primitives.

```text
>>>1.1
1.1
>>>’hi’ 
’hi
>>>”hi” 
’hi’
```

It may seem confusing that ”hi” and ’hi’ are two different expressions; however, we can easily generalize that any values surrounded by quotes \(either single quotes or double quotes\) is a string. It is important to realize that you cannot mix and match these quotes- that is you cannot do ”hi’ or ’hi”.

One last primitive that we will go over is the boolean. Boolean values are true or false values. An example follows:

```text
>>> True
True
>>>False
False
```

Every single value in Python can be characterized as either True or False, and as we progress through the text, we will see what values are ”True” values and which one are ”False” values.

## Functions

Now that we have defined some basic types of data, we can define some ways to modify them. There are 2 types of functions that we will discuss, **in-built functions** and **user-defined functions**.

Before we get into detail about the various types of functions, we should go over the syntax of a function. To call a function, we would use the following syntax: **function\_name\(argument 1,  
 argument 2...argument n\).** Just as a note, an argument is a specific input for a function.

In-built functions are functions that are already defined for us. What this means is that we don’t know how the function itself works, we just know that it outputs will output something corresponding to our input.

```text
>>>from math import sqrt 
>>>sqrt(64)
8.0
```

In the above case, we imported the square root function. After that, we did that, we will call the function on the argument 64 and then get the output of 8. We do not know exactly what goes on in this function, but we do know that it works and that it outputs the proper square root of a number. This is a very basic example; however, later on, we will see that it is important that we do not know how functions are defined.

We will now go over user-defined functions. To define a function, we use the keyword def. We can do this as follows: **def function\_name\(parameter 1, parameter 2\)**. A parameter is a variable in a method definition. When we call a function, we pass in arguments, these arguments take the place of the parameter. Arguments are basically specific values while parameters are placeholder variables. We will define a basic function.

The first thing that you may notice is that in the line after our def statement, we have a group of spaces/indents. The indented block is what we call the **body of the function**. We define the start and end of the function based off the indentation level. Anything nested by either 1 tab or 4 spaces , your choice, is considered to be in the body of a function. It is very important that you do not mix up tabs and spaces- there are very lively debates about which is better all over the internet, it is up to you to choose a side.

The next syntax that we will go over from the above function is the **return statement**. Return statements terminate your function and associate them with some value. If a function runs its completion and has no return statement then the associated value would be None. In this case, we want to associate the value of 2+x with the function add 2. In line 3, we perform a function call to add 2 with an argument of 10. The argument 10 takes the place of the parameter x inside the function add 2 we would then return 10+2 which would return 12. An important clarification to make is that you can only return values within functions. We will go over why later in this chapter.

