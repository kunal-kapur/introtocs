# The Fundamentals

In Computer Science in general, programs are nothing more than instructions. These instructions may initially seem very overwhelming, almost a foreign language; however, all of these instructions fit into one of the following 2 categories.

1. Computing a value
2. Carrying out an action

**Expressions** are generally the vocabulary used to discuss a computation. When we say that Python evaluates an expression, we mean that it computers the value of that expression. For example

```text
>>> 3+5
8
```

We typed 3+5 in the Python interpreter. It then evaluated to the value 8.

On the other hand, a s**tatement** describes carrying out a specific action. An example of a Statement is the Assignment Statement. The Assignment Statement associates some variable with the value of an expression. This is done in the following manner, \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_=\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ . When this occurs, the item on the left will get the value of the expression on the right. For example:

```text
>>> a=3+4+5
>>> a
12
```

We can see that we associated a to the value of ”3+4+5”. Since we evaluated the expression on the right, a was associated with 12. Once we called a we got that value as an output.

Another statement that we will go over is the Import Statement. Oftentimes, there are packages that contain information that we can use. Instead of recreating the wheel each time we want to make a program, we can import information from these packages. Import statements take the following form:  from \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_import \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

A time where this could be useful is when we want a mathematical value, for example pi. Let’s do try the following:

```text
>>> pi
NameError: name ’pi’ is not defined
```

We obviously did not want an error to occur, we wanted the value of pi. So what we can do is utilize the handy math package and do the following.

```text
>>> from math import pi
>>> pi
3.141592653589793
```

Now let’s try a brief example putting together everything that we went over in this lesson.

```text
>>> from math import sqrt
>>> a = sqrt(16)
>>> a
4.0
```

In the above example, we imported the square root function from the math package. Following this, we set a equal to the square root of 16. Since we set a equal to the value of that expression, when we call a we get the output of 4.0.

We will go more in depth with statements and expression in the following lessons, but for now make sure that you have an understanding of the basic definitions.

