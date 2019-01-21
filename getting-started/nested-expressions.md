# Nested Expressions

When we pass variables into functions, sometimes we want to be able to pass in some modified variable. This means that we need to perform more than one function on this variable. This is the motivation behind Nested Expressions. When we have nested expressions, we would have something of the following form: **func1\(func2\(variable\), func3\(variable\)\)**. We will follow the simple rule of evaluating the most nested item first. Let’s walk through an example.

```text
def adder(x,y):
    return x+y
def square(z):
    return z∗z
a = adder(square(2), square(3))
```

So we have 2 functions defined, adder and square. We then have some variable a that we know will be bound to the result of calling adder on the square of 2 and the square of 3. We will follow our basic rule of evaluating everything to the right of the equals sign before the left, which means we need to evaluate adder\(square\(2\), square\(3\)\).

We will begin by evaluating the most nested expressions from left to right. First we evaluate square\(2\) which is 4 then we evaluate square\(3\) which is 9. This leaves us with the function adder called on 4 and 9 as follows which can be thought of as follows:

```text

def adder(x,y):
    return x+y
def square(z):
    return z∗z
a = adder(4,9)
```

We would call the function on it, which would result in a getting bound the the value of 13. In general, when dealing with nested functions, it is important to simplify the problem. Begin by evaluating nested expressions and ”replacing” the operands in the parent calls with the value of the nested expression. This will help clear your mind and allow you to do these problems systematically.

