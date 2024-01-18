Python List Comprehension:
List comprehension is a concise way to create lists in Python. The basic syntax is:


new_list = [expression for item in iterable if condition]
expression: The operation to be performed on each item.
item: The variable representing each element in the iterable.
iterable: The iterable (e.g., list, tuple, string) you are iterating over.
condition (optional): An optional filter to include only items that meet a certain condition.
Example of squaring elements using list comprehension:


                    original_list = [1, 2, 3, 4, 5]
                    squared_list = [x**2 for x in original_list]
                    print(squared_list)
                    # Output: [1, 4, 9, 16, 25]
Difference from For Loop:
List comprehension is more concise and often considered more readable than using a for loop to create a list. The equivalent for loop for the above example would be:


                    original_list = [1, 2, 3, 4, 5]
                    squared_list = []
                    for x in original_list:
                        squared_list.append(x**2)
                    print(squared_list)
                    # Output: [1, 4, 9, 16, 25]
Decorator in Python:
In Python, a decorator is a design pattern and a way to extend or modify the behavior of functions or methods without modifying their actual code. Decorators are applied using the @decorator syntax above a function definition.

Concept of Decorators:
Decorators are functions that take another function as an argument, add some functionality, and then return the modified function. They work by wrapping the original function. Common use cases include logging, timing, access control, and more.

Example of a Simple Decorator:


                def my_decorator(func):
                    def wrapper():
                        print("Something is happening before the function is called.")
                        func()
                        print("Something is happening after the function is called.")
                    return wrapper

                @my_decorator
                def say_hello():
                    print("Hello!")

                say_hello()
                # Output:
                # Something is happening before the function is called.
                # Hello!
                # Something is happening after the function is called.
In this example, my_decorator wraps the say_hello function, adding behavior before and after its execution. The @my_decorator syntax is a shorthand way of applying the decorator to the function.





