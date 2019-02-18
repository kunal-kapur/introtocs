# Comprehensions

Sometimes, it can be useful to condense a for loop over a list structure. This is where comprehensions can come in handy. Comprehensions allow us to generate a new list structure by looping over some set other list or tuple. An example of a list comprehension is in the following we would return a list with every number in the previous list incremented by 1.

```text
>>>lst = [1,2,3]
>>>lst2 = [i+1 for i inlst]
[2,3,4]
```

An easy way to think about this is as a for loop that is iterating over a list and creating a new list for each element in the list. There are a few complicated operations that you can do with list comprehensions.

One such example is the conditional statement that goes within list comprehensions. This takes the following form.

```text
>>>lst = [2,15,50,3]
>>>lst2 = [i + 1 if i < 10 else i+3 for i in lst]
>>>lst2
[3,18,53,4]
```

While list comprehensions do reduce the amount of code that needs to be written it can sometimes be at the cost of readability. As a programmer it is important that you not only make your code for yourself but others who may stumble upon it.

