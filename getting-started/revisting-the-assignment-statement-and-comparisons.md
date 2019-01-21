# Revisting the Assignment Statement and Comparisons

When we set a variable equal to some value, we say we are **binding** that variable to a value. However, we can change the values of variables by setting the variable equal to another value, this process is called **reassigning** a variable. Earlier, we could assign some primitive values to variables, and that’s great, but oftentimes we need to use the results of some data manipulation in order to design what we will assign to a variable. So let’s take a step into that direction. Just as a refresher, here is the assignment statement in action.

```text
>>>a=5
>>>a
5
>>>b=10+2
>>>b=12
```

But now that we have functions, our horizons have expanded! We can now use the assignment statement to assign variables to the output of functions. Let’s go through an example:

```text
>>>def multiply_two(x): 
    return x*2
>>>a = multiply_two(10) 
>>>a
20
```

We know we can make variables equal to the output of functions, but let’s try something a little more ground breaking: making variables equal to functions themselves.

```text
>>>def multiply_two(x):
    return x∗2
>>>a = multiply_two
>>>a
<function multiply_two at 0x100662e18>
```

We set the variable a equal to a function; however, since we did not evaluate the function by passing in an argument, the evaluated statement on the right of the equals sign is the function itself. That means that a will be equal to the actual function multiply\_two. Then why, when we ask for a do we not just get the output multiply\_two? Remember this question, we will address it in the following 2 sections.

We know we can assign variables to the outputs of functions but what can functions output? Well we can basically make a function output anything! From strings to numbers to other functions. Anything that a variable can be assigned to can be returned by a function.

