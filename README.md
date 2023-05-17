# calculator-pythonn
import math

def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    return x / y

def power(x, y):
    return x ** y

def sqrt(x):
    return math.sqrt(x)

print("Scientific Calculator")
print("---------------------")

while True:
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    print("5. Power")
    print("6. Square Root")
    print("0. Exit")

    choice = input("Enter your choice (0-6): ")

    if choice == '0':
        print("Exiting the calculator...")
        break

    if choice in ['1', '2', '3', '4', '5']:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))

        if choice == '1':
            result = add(num1, num2)
            print("Result:", result)
        elif choice == '2':
            result = subtract(num1, num2)
            print("Result:", result)
        elif choice == '3':
            result = multiply(num1, num2)
            print("Result:", result)
        elif choice == '4':
            result = divide(num1, num2)
            print("Result:", result)
        elif choice == '5':
            result = power(num1, num2)
            print("Result:", result)

    elif choice == '6':
        num = float(input("Enter a number: "))
        result = sqrt(num)
        print("Result:", result)

    else:
        print("Invalid choice. Please try again.")
