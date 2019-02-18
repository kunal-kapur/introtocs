# Iteration Over Lists

Lists are indexible and this means that they are quite natural structures to iterate over. To iterate over lists we can use either while loops or for loops. We will look over how we can return the elements in a list using different formats:

```text
>>>lst = [1,2,3]
>>>counter = 0
>>>sum = 0
>>>while counter < lst.length:
...    sum=sum+ lst[counter]
...    counter+=1
>>>sum
6
```

While this is fine, the for loop can be more concise. We can use the in range syntax to iterate over every number from 0 to the number \(inclusive at the 0 and exclusive at the number\). Note that range has an optional start parameter, but by default it is set to 0.

```text
>>> lst = [1,2,3] 
>>> sum = 0
>>> for i in range(len(lst)):
...    sum = sum + lst[i]
>>> sum
6
```

Finally we can just add all the elements in the list without even indexing. Instead we can use the in syntax to get each element from the list.

