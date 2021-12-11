### Reading and Writing Files In Python
- A file is a set of bytes used to store data
- they are then translated to 1 and 0 to be easier for the computer to read
- it comprised of three parts 
    1. header - metadata about the contents of the file
    2. data - contents fo the file as written by the creator or editor
    3. End of file special character tha indicates the end of a file
- the data represented needs and extension
### file paths 
- when you access a file on an operating system a file path is required 
- its a string that represents a location
   1. Folder path - the file folder location 
   2. File Name - the actual name of the file
   3. Extension - the end of the file path pre-pended with a period used to indicate the file type

### Opening and Closing a File in Python
- to open a file in python you would use the `open()` function 
- it has a sing required argument which is the file path 
   - `file = open(dog_breeds.txt)`
- next is learning how to close it and its your responsibility to close it
- first way is to use a try-finally block
`reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()`
- next is a with statement
`with open('dog_breeds.txt') as reader:
    # Further file processing goes here`
- it automatically closes it when it leaves the with block


### Python Exceptions
- a python program terminates when an error occurs either a syntax error or an exception will do this
- a syntax error occurs when the parser detects an incorrect statement
- we can use raise to throw an exception if a condition occurs the statement can be complemented with a custon exception
- Assertion error - we can assert the condition is met and if its true the program wont brake
- we can also use try and except block