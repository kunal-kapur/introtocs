# Conditionals

Sometimes we would want to do some action only if some condition is fulfilled. In terms of this section, we want to perform an action if some condition is evaluated to True. We know that every item in Python can be evaluated to either True or False. So using a tool called **conditionals**, we can evaluate only certain expressions. There are three conditionals in Python. The particular time when one can be used will be listed directly underneath.

* if

  * Can use at any time.
  * We check the following:

          If so then we evaluate the body following that clause 

* elif
  * Can only use the statement if there was or another elif statement as the conditional before it.
  * If no conditional \(if or elif\) had a condition that evaluated to True and the condition evaluates to True for this one evaluate the body. Looks as follows_:_
* else
  * Use as the closing conditional. Can only be used if an if statement was somewhere above it. It can follow elif statements as well; however, it cannot follow another else statement.
  * If none of the above conditionals had a condition that evaluated to True then just run the body of the else statement.
  * Basically the else statement should be thought of as a net that catches any case that was not accounted for.

Now that we have that out of the way we will go over a few examples of using conditionals.

First, we will look at the case with only an if statement.

```text
def superfan(x):
    if x >= 5:
        return ”It ’s a bit chilly” return ”It’s warm”
superfan (10)
```

In the above case, we run superfan with an argument of 10. The next step s then to check the clause x &gt;= 5 and see if it is valid. In this case it is so then we return the String ”It’s a bit chilly”. It is important to remember that after a return statement, the function is done executing. In this case, when we reach a return statement, the function call superfan\(10\) is equivalent to ”It’s a bit chilly”. That means we do not continue to the line that returns ”It’s warm”.

If we, for example, had the function call of superfan\(2\), we would look at the if clause and see that x &gt;= 5 is not true so we would not go inside of the body of the conditional. We would then continue past the body and return ”It’s warm”.

Next we will look at the case where we have multiple if statements and elif statement\(s\)

```text
def boom(x):
    if(x <=5):
        x +=1
    if(x >=6):
        x −=4
    elif( x <= 5 ):
        x+=10
return boom(4)
```

We run the function call boom\(4\). 

* In the first step of the function, x is equal to 4. We then go to the first clause and check the condition, x &lt;= 5. It is so we go inside of the body and set 2 to x + 1, resulting in x equaling 6. 
* We reach another if statement- this implies that we are finished with the previous ”if” series. We check the clause x &gt;= 7 and it is not True so we move to the elif statement and see if x &lt;=5 then we move to the body. It is so we set x equal to x+10, or 15. 
* We then return x which is 15. Note that the elif corresponds to the closest if statement so it does not matter that x &lt;= 5 evaluates to True. Since the closest if statement evaluated to false, and there were no other elif statements, we evaluate the clause. 
  * However, if x &gt;= 6 had evaluated to true we would not have evaluated the clause x &lt;= 5.

