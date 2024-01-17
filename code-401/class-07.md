# Variable Scope in Python:

Variable scope refers to the region or context in which a variable is defined and can be accessed.
In Python, there are two main types of variable scope: local scope and global scope.

## Local and Global Scope:

Local Scope: Variables defined within a function are in the local scope. They are only accessible within that function.
Global Scope: Variables defined outside of any function or in a module are in the global scope. They can be accessed throughout the program.

                global_var = 10  # Global variable

                def example_function():
                    local_var = 5  # Local variable
                    print("Local variable:", local_var)
                    print("Global variable:", global_var)

                example_function()
                print("Outside function - Global variable:", global_var)
                # print("Outside function - Local variable:", local_var)  # Raises an error


## Global and Nonlocal Keywords:

Global Keyword: Used to declare a global variable inside a function.
Nonlocal Keyword: Used to indicate that a variable refers to the nearest enclosing scope that is not global.

                    x = 10  # Global variable

                    def example_function():
                        global x
                        x += 5
                        print("Inside function - Global variable:", x)

                    example_function()
                    print("Outside function - Global variable:", x) 

## Big O Notation:

Purpose: Big O notation is a way to describe the efficiency or complexity of an algorithm. It provides an upper bound on the growth rate of an algorithm's time or space complexity.
Importance: Helps in comparing and analyzing the performance of algorithms, especially as input sizes grow.

## Simulating Dice Roll in Python:

Use the random module to generate a random number between 1 and 6 (inclusive) for a standard six-sided die.
Calculate the probability by running the simulation for a large number of trials and counting the occurrences of the desired outcome.

                    import random

                    def simulate_dice_roll(trials, target_number):
                        count = 0
                        for _ in range(trials):
                            roll_result = random.randint(1, 6)
                            if roll_result == target_number:
                                count += 1
                        probability = count / trials
                        return probability

                    target_number = 6
                    trials = 10000
                    probability_of_six = simulate_dice_roll(trials, target_number)
                    print(f"Probability of rolling a {target_number}: {probability_of_six}")



