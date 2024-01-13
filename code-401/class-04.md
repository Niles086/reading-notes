# Class-04 Notes and answers 

1. Classes and objects in Python provide a way to structure code, organize data, and encapsulate functionality. Classes define the blueprint, and objects are instances created based on that blueprint. Instances have their own state (attributes) and behavior (methods), making them versatile and reusable in different parts of a program.

## 2. Recursion in Python:

Definition:
Recursion is a programming concept where a function calls itself in its own definition. In a recursive approach, a problem is broken down into smaller sub-problems that are solved independently, leading to a solution for the original problem.

Example:
A classic example of recursion is the calculation of the factorial of a number. The factorial of a non-negative integer n, denoted as n!, is the product of all positive integers up to n.

                def factorial(n):
                    if n == 0 or n == 1:
                        return 1
                    else:
                        return n * factorial(n - 1)

                # Example usage
                result = factorial(5)
                print(result)  # Output: 120

Best Practices for Recursive Functions:

Base Case:

Ensure there is a base case that defines the simplest scenario where the function can return a result without making a recursive call.
The base case prevents the function from entering an infinite loop and serves as the stopping condition.
Progress Toward Base Case:

Ensure that each recursive call brings the problem closer to the base case.
The input to the recursive calls should gradually move toward a state where the base case can be reached.
Memory Consideration:

Be mindful of memory usage, as excessive recursion can lead to a stack overflow. Each recursive call consumes stack space.
In Python, there is a limit to the number of recursive calls due to the maximum recursion depth.
Clarity and Readability:

Use recursion when it enhances code clarity and simplifies the problem-solving approach.
Some problems are naturally suited for recursive solutions, while others may be clearer with iterative approaches.

## 3. Pytest Fixtures:

Purpose:

Pytest fixtures are a way to set up preconditions and share common test data or resources across multiple test functions.
They allow you to define reusable components that can be used by multiple tests, enhancing the organization and readability of your test suite.
Usage:

Fixtures are defined as functions marked with the @pytest.fixture decorator.
They are invoked by test functions as arguments, automatically managing the setup and teardown of resources.

Code Coverage:

Purpose:

Code coverage measures the percentage of code that is executed during the testing process.
It helps identify untested parts of the codebase, ensuring that tests are comprehensive.
Usage:

Code coverage tools analyze the codebase and provide reports on which lines or branches of code were executed during testing.
Example:

Tools like pytest-cov can be used with Pytest to generate code coverage reports.

By combining Pytest fixtures and code coverage analysis, you can create a robust testing environment. Fixtures ensure a consistent and well-prepared test environment, while code coverage reports guide you in enhancing your test suite's completeness. This approach contributes to the overall quality and maintainability of a project by fostering a testing culture and helping catch potential issues early in the development process.