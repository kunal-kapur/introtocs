# Adding to Lists

Sometimes we want to change our list of data in some manner. The first modification that we will go over is adding to a list. There are three canonical ways to do this: the ”+” operation, ”.append”, and ”.extend”. Each of these methods has their own syntax and unique attributes.





We will use the above block of code to illustrate the differences between adding to a list. The PythonTutor link can be found here.

The ”+” operator adds an arbitrary amount of lists and returns a new list. The outcome of a ”+” operation is shown below. It is extremely important to realize that when we perform the ”+” operation on lists, the original list does not change. This can be seen above where listie is still \[1\], but the new list, lst2, has the value of \[1,2\]



Alternatively we can use the ”.append” method. This method takes in 1 value and adds it to the end of the list. For the same list as above, let’s perform the ”.append” method.  
 Unlike the ”+” operator, the ”.append” method does not return a new list, rather it modifies the original list. In the above visual, we can see that lstie has been modified to include the number 3 at the end and lst2’s value is None. The reason why lst2’s value is None is because the .append function has no return value.



Finally let’s look at the ”.extend” syntax. The ”.extend” function takes in a list of arbitrary length and adds it to the end of the list



**Just like append, extend modifies the actual list**, it does not return a new list like the ”+” operator. The list listie has been modified to include 4 in this step and lst3’s value is None for the same reasons that .append follows this pattern.

