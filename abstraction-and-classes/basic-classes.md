# Basic Classes

In the last section we discussed a way of storing data in the form of lists and list like structures. Now we will go over another way of storing data- one that more powerful and allows us to perform operations on this data and retain the results. The structure that we will go over is called **Classes** and it is part of the **Object Orientated Programming methodology.**

Object Orientated Programming is basically a way of organizing programs in a way that makes sense to Humans. This class abstraction also allows us to perform operations and mutate our data.

To create a class use the following syntax:

```text
class Car:
def __init__ (self , num wheels):
    self .num wheels = num wheels 
    
def lose wheel ():
    if self.numwheels>0:
        self .num wheels −=1
    else:
        return ”There are no wheels to remove”
```

Now, what’s going on above? Basically, we have a class Car. Inside the Car class, we have 2 **methods**, or functions that are a part of a class. One of these methods is an init method and the other is just a normal method. The idea of an **init** method is that when you **instantiate**, or create an instance of a class, you call the init function to set certain attributes for your instance.

