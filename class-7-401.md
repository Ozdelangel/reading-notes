The concept of scope rules how variables and names are looked up in your code.
Determines the visibility of a variable in your code
Python scope concept is generally presented using a rule known as the LEGB rule.
It stands for local, enclosing, global, and built in scopes.
Global scope - the names that you define in this scope are available to all your code
Local Scope - the names that you define in this scope are only available or visible to the code within the scope
Python scope is closely related to the concept of the namespace
Python scope determines where in the program a name is visible
Python scopes are implemented as dictionaries that map names to objects
They are commonly called name spaces
These are the concrete mechanisms that python uses to store names. They’re stored in a special attribute called __dict__
After you import sys you can use .keys() to inspect the keys of the sys.__dict__ this return a list with names. 
This is a concrete representation of the module scope.

There are two ways to access something which is defined in the sys 
Using dot notation module.name
Using subscription operation on .__dict__ in the form of module.__dict__[‘name’]
Using the LEGB Rule

Local - is the code block or body of any python function or lambda expression. This python scope contains the names that you define inside the function. These names will only be visible from the code of the function. 

Enclosing scope - is a special scope the only exists for nested functions

Global scope -  is the top most scope in a pythons program, script, or module. This python scope contains all of that names that you define at the top level of a program

Built in scope - is a special python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contain names such as keywords, functions, and expressions.

The local scope or function scope is created at function calls
Every def or lambda expression as a blueprint for new local scopes
By default parameters an names that you assign inside a function exist only within the function or local scope
Nested functions: the enclosing scope
Is observed when you nest functions inside other functions
Names that you define in the enclosing python scope are commonly known as non local names 
Modules: the global scope
Python turns you program main script into a module names __main__ to hold the main programs execution
The namespace of this module is the main global scope of you program
Builtins: the built in scope
The built in scope is a special python scope thats implemented as a standard library
Built ins are always loaded into you global python scope
