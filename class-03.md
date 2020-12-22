# Reading and Writing files in Python

- be sure the file you're reading/writing is being read/written with the same Char encoding as it was created with. 
- files have 3 main components: 
    1. header
    1. data
    1. End of File: (EOF) 
- always close a file after you read/write from/to it

## Exceptions
python automatically ends the program when an error occurs; there are two types of error, syntax and exception. 

syntax errors are when the interpreter cannot read/interpret the code written. 
exceptions happen when the interpreter reads the code but some value is not expected. 

you can use `try: except: finally:` to allow the program to continue running even when an exception is raise. `else:` may also be used as part of a try-except block with it's own try-except block. 



[Return to Main index of Notes](./README.md)