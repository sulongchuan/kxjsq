import math

def scientific_calculator():
    print("Welcome to the Scientific Calculator!")
    
    while True:
        print("Please select an operation:")
        print("1. Addition")
        print("2. Subtraction")
        print("3. Multiplication")
        print("4. Division")
        print("5. Exponentiation")
        print("6. Square Root")
        print("7. Logarithm")
        print("8. Exit")
        
        choice = input("Enter choice (1-8): ")
        
        if choice == '1':
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            result = num1 + num2
            print("The result is:", result)
        elif choice == '2':
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            result = num1 - num2
            print("The result is:", result)
        elif choice == '3':
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            result = num1 * num2
            print("The result is:", result)
        elif choice == '4':
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            result = num1 / num2
            print("The result is:", result)
        elif choice == '5':
            num1 = float(input("Enter base number: "))
            num2 = float(input("Enter exponent number: "))
            result = num1 ** num2
            print("The result is:", result)
        elif choice == '6':
            num = float(input("Enter a number: "))
            result = math.sqrt(num)
            print("The result is:", result)
        elif choice == '7':
            num = float(input("Enter a number: "))
            base = float(input("Enter the base of the logarithm: "))
            result = math.log(num, base)
            print("The result is:", result)
        elif choice == '8':
            print("Thank you for using the Scientific Calculator!")
            break
        else:
            print("Invalid input. Please enter a number between 1 and 8.")
            
scientific_calculator()
