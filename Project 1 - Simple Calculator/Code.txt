print("Simple Calculator")

a = int(input("Enter your first number: "))
b = int(input("Enter your second number: "))

print(f"Your First Number is {a} and your second number is {b}")

print("----- MENU -----")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Exponential")
print("5. Division")
print("6. Floor Division")
print("7. Modulus")

ch = input("Enter your choice (1-7): ")

if ch == '1':
    print("----- Addition -----")
    result = a + b
    print(f"{a} + {b} = {result}")

elif ch == '2':
    print("----- Subtraction -----")
    result = a - b
    print(f"{a} - {b} = {result}")

elif ch == '3':
    print("----- Multiplication -----")
    result = a * b
    print(f"{a} * {b} = {result}")

elif ch == '4':
    print("----- Exponential -----")
    result = a ** b
    print(f"{a} ** {b} = {result}")

elif ch == '5':
    print("----- Division -----")
    if b == 0:
        print("Error: Division by zero is not allowed")
    else:
        result = a / b
        print(f"{a} / {b} = {result}")

elif ch == '6':
    print("----- Floor Division -----")
    if b == 0:
        print("Error: Division by zero is not allowed")
    else:
        result = a // b
        print(f"{a} // {b} = {result}")

elif ch == '7':
    print("----- Modulus -----")
    result = a % b
    print(f"{a} % {b} = {result}")

else:
    print("Invalid choice")
