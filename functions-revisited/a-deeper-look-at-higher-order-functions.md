# A Deeper Look at Higher Order Functions

We talked about nested functions earlier- now we will go more in depth and talk how to utilize them more. Below we have a standard higher order function:

```text
def PB(x):
    def Jelly(x):
        x=x+5 
        return x
    x += 1
    y = Jelly(x+2) 
    return x + y
```

Now look let’s run PB with an argument of 5. Well start off like any other function and set x equal to 3 in the PB frame. We then set the variable Jelly equal to the function Jelly. Finally, we increment x by 1. Now we perform the function call Jelly\(x+2\).  


The function is called with an argument of x+2. We are currently in the f1 frame so we make Jelly’s argument of the value of x, 5, plus 2, or 7.

We are now in the f2 frame. f2 has a variable defined in its scope named x. We define x in this frame to be equal to 7. Note that it is still 5 in the global frame.

We then change x’s value to be x+5. Since x is 7 in this frame we change x to be equal to 12. Now we are done with the function and it returns 10.

We have now exited the function and returned to f1 We are now back in the global frame and we take the return value of our function, 10, and set the variable y equal to it. Finally we return x+y, which is 10+5 or 15.

