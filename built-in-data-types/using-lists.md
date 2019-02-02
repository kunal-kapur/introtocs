# Using Lists

We can also interact with lists in a few ways that make them very natural to use when manipulating data. For example, we can get the 1st element of our list that we created in the previous section by performing the following call:

```text
>>> lst = [1, 2, 10, ”Kettle Corn”] 
>>> lst[1]
2
```

A somewhat tricky part about this syntax is that the 1st element in the list occurs after the 0th- that is, our list is zero indexed.

Another useful function that Python has provided us to deal with lists is the len function. If we call len on a list, we will get the length of the list. Using the same list as above:

```text
>>>len(lst)
4
```

Note how the length of the list is not 0 indexed- an empty list has a length of 0, a list with only 1 element has a length of 1, and this list above has a length of 4. 

Now what values can we store in a list? Well just about any. We can store numbers, Strings, and even other lists. Storing lists inside lists may seem a bit strange, but it can be useful. For example, we would use this is we wanted to store the longitude and latitude of the 5 nearest airports. Below is the syntax for putting a list inside of a list:

```text
>>> coords = [[102.355 , 101.111] , [54 , 32]]
>>> coords
[[102.355 , 101.111] , [54 , 32]] 
>>> coords[1]
[54 ,32]
>>> coords [1][0]
54
```

In the first statement, we make a nested list. In the second call we see the values of the list coords which is \[\[102.355 , 101.111\] , \[54 , 32\]\] . In the third call, we access the element at the first index of coords which is \[54,32\] \(remember lists are 0 indexed\). In the final call we get the 1st index of coords and the 0th index from that element- since the first element is \[54,32\], the 0th element would be 32.



