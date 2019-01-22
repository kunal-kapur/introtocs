# Scope of Variables

Now that we know what frames are, there comes an interesting question. Can we access all variables from anywhere in the program? The answer is no! These frames designate a sort of hierarchy and we will go over them in this section. An important concept for scopes is the idea of Parent Frames. Just as a review, a frame’s parent is the frame that the function was defined in.

1. Parent frames cannot make direct references to variables in child frames. This makes intuitive sense. You cannot be sure that a function call would occur, as a result, you have no knowledge on if a frame executed or not.
2. Child frames can view variables in parent frames; however, they cannot directly edit those values. There will be exceptions to this which we will go on later.

It is important to note that since functions are essentially variables- just a name defined to some set of operations, these same rules also apply to functions.

We will over a basic example now showing some of the ways the scope of variables can be made a bit tricky.

```text
def marsh(y):
    x = ”gooey”
    def mallow():
        return x
    return mallow () 
x = ”sticky”
x = marsh(x)
```

