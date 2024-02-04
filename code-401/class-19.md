## In Python, the primary module for working with regular expressions is re. It provides a set of functions for working with regular expressions. Here's a simple example:

                    import re

                    text = "Hello, my email is john@example.com and my phone number is 123-456-7890."

                    # Search for an email address
                    email_pattern = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'
                    email_match = re.search(email_pattern, text)

                    if email_match:
                        print("Email found:", email_match.group())
                    else:
                        print("No email found.")


This example uses the re.search() function to find an email address in a given text using a regular expression pattern.

# shutil module:

The shutil module in Python provides a higher-level interface for file operations and directory management. One common use case is for copying, moving, and deleting files or directories.

Example:

                    import shutil

                    # Copy a file
                    shutil.copy('source_file.txt', 'destination_folder/')

                    # Move a file
                    shutil.move('source_file.txt', 'new_location/')

                    # Remove a file
                    shutil.remove('file_to_remove.txt')

## In this example, the shutil.copy() function copies a file, shutil.move() moves a file, and shutil.remove() deletes a file.

## os vs. shutil:

os module:

Lower-level module, provides basic operating system functions.
Functions like os.listdir(), os.rename(), os.remove() work with files and directories.
Useful for simple operations on files and directories.
shutil module:

Higher-level module, builds on top of os and provides more convenient file operations.
Functions like shutil.copy(), shutil.move(), shutil.rmtree() offer more advanced file and directory management.
When to choose:

If you need basic file and directory operations, os might be sufficient.
If you need more complex operations, especially involving copying, moving, or removing entire directories, shutil provides more convenient functions.
In general, if you are dealing with more complex file operations, shutil is often the better choice due to its higher-level functions.