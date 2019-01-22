# Recursion

We know that we can call functions within other functions- this leads us to an interesting point: from one function we can call the same function. If a function calls itself we call that function **recursive**.

If we keep calling a function on itself with the same argument, we know that we will get into infinite recursion- our process will never end! So how do we avoid this? Well we can change our function’s argument so that it gets closer to some terminating condition, and eventually reaches it.

What is one process that we discussed earlier that has a terminating condition with some argument that continually gets smaller? The answer is While Loops! In fact, recursive function can usually be rephrased as while loops and vice versa. So why would we want to use one over the other? There are a few reasons but one of the main ones is that sometimes it can be more natural to write a function one way versus the other.

Say we want are given some number x and we want to find x!. How can we do this? Let’s start off with iteration which may be more intuitive.

```text
def factorial(x):
    sol=1
    while x > 0:
        sol=sol∗x
    x −= 1
    return sol
```

Let’s now go through an example of running through the factorial function with the number 3. We will consider each iteration to be one ”step”. In the first step we multiply our current product \(1\) by 3. We then decrement x by 1, making it 2. We then multiply the current product \(3\) by 2 making it 6. Again we decrement x by 1 making it 1.We then multiply our current product \(6\) by 1 making it 6 and we decrement x to 0. Since x is 0 our while loop is terminated.

Now let’s look at the pattern that this function yielded. We had 3\*2\*1=6. More generally, for some n, we had \(n\)\*\(n-1\)\*\(n-2\)...\(1\).

In this case, we perform our iteration while x is greater than 0. So what is the terminating case? Well we want the function to stop if x ever falls to some number less than or equal to 0 so we can have some conditional in our function that follows the format:

```text
if x<=0:
```

Additionally, we multiplied the value of x at 1 iteration with the value of x in the next iteration and so forth. This means that we should have the following line of code somewhere in our function:

```text
x*factorial(x−1)
```

Now lets put it all together. If we were to call this on 1 we would immediately get to the terminating condition. What would we want to do? Well we need to return something for the function call factorial\(0\) otherwise we would be multiplying 1 by None. So we know we need to return something, but what is it? Well if we return just 0 then we get a problem since 1! is not 0. What do we do then? Well if x is less than or equal to 0 we can simply return 1. We then know our terminating condition or base case will be.

```text
if x <=0:
    return 1
```

Let’s take the value for factorial 2. We know we will have a call 2\*factorial\(1\) = 2\*1\*factorial\(0\). From here we can come up with our recursive function.

```text
def factorial(x):
    if x <= 0:
        return 1
    return x*factorial(x−1)
```

To verify this is correct let’s try it with the argument of 3. We have:

$$
3 ∗ factorial(2) = 3 ∗ (2 ∗ factorial(1)) = 
3 ∗ (2 ∗ (1 ∗ factorial(0))) = 3 ∗ (2 ∗ (1 ∗ 1)) = 6
$$

We can verify that this is correct with a calculator or computation.

In general, coming up with a recursive function involves the following steps:

1.  **Base Cases** Find the base cases. In other words, see when you want your function to terminate
2. **Argument Reduction** Find out what you want to do to your arguments to the function. Somehow get closer to your base case- usually done by some arithmetic.
3. **The Recursive Step:** This step requires you to figure out what you want to do for each argument until the base case. In many recursive cases you want to do something with the combined Recursive steps \(use your problems towards your base case to solve the original problem\).

An optional first step is to write the function iteratively first and convert it to a recursive function; however, as you gain practice with recursion you will find this step to be a bit redundant.

