# Reading answers 

## 1. Purpose of the 'with' Statement in Python File Handling:

The 'with' statement in Python is used for resource management, particularly when working with file objects. It simplifies the code and ensures that certain operations are performed before and after the execution of a block of code. When used with file handling, the 'with' statement automatically takes care of opening and closing the file, which is crucial for resource management.

## 2. Difference between 'read()' and 'readline()' Methods for File Objects:

read() method:

Reads the entire content of the file as a single string.
Suitable for small to moderately-sized files.
readline() method:

Reads a single line from the file and returns it as a string.
Useful when processing files line by line.

## 3.  Exception Handling in Python:

Exception handling in Python allows you to gracefully handle errors during the execution of a program. The 'try', 'except', and 'finally' blocks are used for this purpose.

try block: Contains the code that might raise an exception.
except block: Handles specific exceptions that may occur within the 'try' block.
finally block: Contains code that will be executed whether an exception occurs or not. Useful for cleanup operations.