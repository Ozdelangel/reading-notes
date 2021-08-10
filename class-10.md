# Javascript Debugging

- to find an error you first need to know how scripts are processed
- the orfer in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run
- The javascript interpreter uses the concept of an execution context; plus, each function creates a new new exectuion context. They correspond to variable scope.

## execution context
- every statement in a script lives in one of three exectution context

1. global context - code that is in a script, but not in a function. there is only one global context in any page.

2. Function Context - code that is being run within a function has its own function context

3. eval context text is executed like coed in an internal function called `eval()` 

## Variable Scope
- the first two execution contexts correspond with the notion of scope

1. function-level scope
- when a variable is declared within a function, it can only be used within that function. this is because it has function level scope

## The Stack
- the javascript interpreter processes one line of code at a time. when a statement needs data from another function, it stacks the new function on top of current tasks

1. when a statement has to call some other code in order to do its job, the new task goes to the top
2. once the new task has been performed, the interpreter can go back to the task at hand
3. each time a new item is added to the stack it creates a new execution content
4. variables defined in a function are only avvaible in that function