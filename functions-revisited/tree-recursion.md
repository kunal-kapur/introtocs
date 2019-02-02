# Tree Recursion

There are a special class of recursive functions that are called **Tree Recursive**. These are functions that call themselves more than once per call. Such a function may look like the following:

```text
def tree_recurs(n):
    if n == 1:
        return 1
    return tree_recurs(n−1)+tree_recurs(n−1)
```

Tree Recursion is given its name because each function call would have more than 1 function call come out of it and ”branch out”. Tree recursion can be tricky and it can be useful to write out the recursive relations that we did earlier for factorial.

