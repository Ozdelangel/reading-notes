# Classes and Objects
- objects are an encapsulations of variables and functions into a single entity

example: class MyClass:
            variable = "blah"

            def function(self):
                 print("this message inside the class")

- the variable my objectx holds an object of the class "MyClass" that contains the variable and the function defined within the class called Myclass

# Accessing Object Variables 
- to access the variables inside the class you would use dot notation 
example: `myobjectx.variable`

- you can create multiple different  objects that are of the same class however each object contains independent copies of the variables defined in the class

# Accessing Object Functions

- to access a function inside of an object you use notation similar to accessing a variable

# Thinking recursively
### A santa example to think recursively
1. appoint an elf and give all the work to him
2. assign titles and responsibilities to the elves based on the number of houses for which they are responsible
- 1 he is a manager and can appoint two elves and divide his work among them

- = 1 he is a worker and has to deliver the presents to the house assigned to him

# recursive functions in python
- a recursive function is a function defined in terms of itself via self-referential expressions
- the function will repeat itself until some conditions are met to return a result
