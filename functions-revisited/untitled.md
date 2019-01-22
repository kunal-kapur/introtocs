# Iteration

We have dealt with simple functions; however, the power of functions can be displayed through a concept called **iteration**. Iteration is a way with dealing with repetition within a function. For example say you want to find the sum of the first n numbers. We would want to iterate over each number and keep track of a sum, and for each number, we would add it to the sum.

We can use the while statement to help us loop over elements. While loops take the following format:

```text
while some condition :
    statements that occur is the condition is true
(optional) statements that occur after the condition is evaluated to false
```

The statement that occurs in the while block will occur over and over until the statement becomes false. This usually means that at each step of the while loop, we want to somehow get closer to terminating the loop- by enumeration or some other method.

In the prior example, we stated that we wanted to sum over the first n numbers. Our condition in this case would be while our current number is not greater than n and at each step in the while loop, we would want to increment our sum by the number we are currently on. More concretely:

```text
def sumofN(n):
    i=0
    sum = 0 
    while i < n:
        i=i+1 
        sum=sum+ i
    return sum
```

To step through this code press [here](http://pythontutor.com/visualize.html#code=def%20sumofN%28n%29%3A%0A%20%20%20%20i%20%3D%200%0A%20%20%20%20sum%20%3D%200%0A%20%20%20%20while%20i%20%3C%3Dn%3A%0A%20%20%20%20%20%20%20%20i%2B%3D1%0A%20%20%20%20%20%20%20%20sum%20%2B%3D%20i%0A%20%20%20%20return%20sum%0AsumofN%283%29&cumulative=false&curInstr=0&heapPrimitives=false&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false). You can change the arguments to any number over 0 and get a feel for what’s going on.

It is important to realize that on line 6 we evaluate i+1 and then set that equal to i. Similarly we rebind the variable sum to the sum of the variable sum and i.

When dealing with loops, it can be easy to fall in the trap of ”off by one errors”. These are basically errors that result when you overcount or undercount your expected terminating condition. For example, in the abovecode consider what would happen if we set the while loop to i &lt;= n instead of i &lt;n.

Additionally, it is possible that your while loop never terminates. If you never get any closer to a terminating condition, your loop will go on forever. This can happen in the following case

```text
def infinite():
    i=1
    sum = 0 
    while i > 0:
        i=i+1 
        sum=sum+ i
    return sum
```

Since i is always increasing, it will never approach 0 and as a result, it will never be able to exit from the loop. If you ever get stuck in an infinite loop, press control c on your computer and you can exit from the loop.

