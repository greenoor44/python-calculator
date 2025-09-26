# Python Calculator

It is a basic python calculator which can perform basic arithmetic operations like addition, subtraction, multiplication. Python 3.8 is used for the implementation.

## Approach

* User enter number (single digit or n character) to perform a specific operation like 1, 2, 3, 4 and n (n is to cancel calculation operation) are valid.
* Taking two numbers as inputs and used branching if elif else to perform a particular section.
* Using functions add(), subtract(), multiply() to perform specific task after given data to the system.

## Code
```
# Program make a basic calculator
# Author @inforkgodara

# Function adds two numbers
def add(first_number, second_number):
    return first_number + second_number


# Function subtracts two numbers
def subtract(first_number, second_number):
    return first_number - second_number


# Function multiplies two numbers
def multiply(first_number, second_number):
    return first_number * second_number


# Function divides two numbers
def divide(first_number, second_number):
    return first_number / second_number


print('Select options.')
print('1. Add')
print('2. Subtract')
print('3. Multiply')
print('4. Divide')

while True:
    # Take input from the console
    choice = input('Enter choice(1/2/3/4 or n to cancel): ')
    # Check if choice is one of the five options
    if choice in ('1', '2', '3', '4'):
        first_number = float(input('Enter first number: '))
        second_number = float(input('Enter second number: '))

        if choice == '1':
            print(first_number, '+', second_number, '=', add(first_number, second_number))

        elif choice == '2':
            print(first_number, '-', second_number, '=', subtract(first_number, second_number))

        elif choice == '3':
            print(first_number, '*', second_number, '=', multiply(first_number, second_number))

        elif choice == '4':
            print(first_number, '/', second_number, '=', divide(first_number, second_number))
    elif choice == 'n':
        print('Your are successfully logged out!')
        break
    else:
        print('Please enter correct input among these 1/2/3/4/n')

```
## My Interpretation

**What the program does (2–3 lines):**
- … The program defines 4 arithmetic functions: add(), subtract(), multiply(), and divide() that take two numbers as parameters to perform calculations. Then it runs a while loop which takes input from the user. If the user enters 1,2,3, or 4, it performs the specific calculation. Otherwise, if the user wishes to exit the program, he/she enters 'n'. If the user enters any other input, it gives the message to enter correct input.
**Functions (inputs → outputs):**
- add(x, y) → takes two numbers x and y and adds them
- subtract(x, y) → takes two numbers x and y and subtracts them
- multiply(x, y) → takes two numbers x and y and multiplies them
- divide(x, y) → takes two numbers x and y and divides them

**Control flow (2–4 lines):**
-The code begins with a while loop that takes input from the user as 1, 2, 3,4 or n. It then takes two numbers as input from the user.  It then runs an if, elif and else statement that performs the calculation corresponding to the number entered. If input is 1, it adds the two numbers. If 2, it subtracts them, If 3, it multiplies and if 4, it divides them. The program terminates if the user enters n.Otherwise, if the input is other than this, an error message is printed. 