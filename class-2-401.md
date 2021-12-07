# Unit tests and TDD
- Unit tests are some pieces of code to excercise the input and output of code
- TDD is test driven development it is a strategy to think and write tests first
- The first example the article talked about how there may be something you are working on that needs to get as users name, email, and gender. so you have to take small steps in writing tdd
- The test is input name, and output female.
- The test should be your alive documentation - be descriptive
- it should be the same as the module name `gender.py` should be `test_gender.py`
- Arrange - you need to organize the data needed to execute that piece of code
- Act- here you will execute the code being tested
- Assert after executing the code you will check if the result or output is the same as you were expecting
## The Cycle 
- write a unit test and make it fail
- write the feature and make the test pass
- refactor the code
### USE BABY STEPS

# What does if __name__ == '__main__' do?

- before executing code Python interpreter reads source file and define few special variables/global variables
- if the interpreter is running that module as the main program it sets the special name variable to have a value of main
- if the file is being imported from another module name will be set to the modules name

- when we execute to the interpreter we use `python script.py` or whatever the module is

# Recursion
What does do something recursively mean? its the difference of doing something iteratively but just changing the variable of say `n` it works within itself.