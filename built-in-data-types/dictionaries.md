# Dictionaries

Sometimes, we want to store key value pairs- in other words, we want to associate some key to a property. An example of where this method would be useful is associating students to their grades in a particular class. The name of the student would be a String and the grade would be an integer. An important thing to note is that each student is unique but their grades may not be. For example, John and Jim could both have 90% in the class. Additionally we may want to change someone’s grade from a 90 to 95.

The above observations help us form the intuition for a Dictionary. Dictionaries are made up of 2 components, an immutable key \(a key that cannot change\) and a value that can change. Additionally, key’s must be unique. That is if you insert 2 keys into a dictionary, the more recent one’s value will be the value in the dictionary. A side note about dictionaries is that they are inherently unordered- instead of get a value by index, we get a value by its key. **insert example here**

