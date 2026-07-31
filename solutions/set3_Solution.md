# 🐍 Set 3 – Functions & Problem Solving

This document contains the solutions for Set 3 Python practice questions.

---

## Answer 1 – Secret Agent

### 📌 Question

Write a Python program that creates a function `verify_code(code)` to verify a secret code. If the entered code is `"007"`, return `"Access Granted"`; otherwise, return `"Access Denied"`.

### 💡 Explanation

The program defines a function that accepts a code as a parameter. It compares the entered code with the secret code and returns the appropriate message.

### 📝 Solution

```python
def verify_code(code):
    if code == "007":
        return "Access Granted"
    else:
        return "Access Denied"

code = input("Enter the code: ")
result = verify_code(code)
print(result)
```

---

## Answer 2 – Restaurant Discount

### 📌 Question

Write a Python program that asks the user for the bill amount. If the bill is ₹1000 or more, apply a 10% discount; otherwise, no discount is applied.

### 💡 Explanation

The program checks whether the bill amount is greater than or equal to ₹1000. If true, it calculates the discounted bill; otherwise, it displays the original bill.

### 📝 Solution

```python
bill = float(input("Enter the bill amount: "))

if bill >= 1000:
    bill = bill - (bill * 10 / 100)

print(f"Final Bill: ₹{bill}")
```

---

## Answer 3 – Username Strength Checker

### 📌 Question

Write a Python function `check_username(username)` that returns the strength of a username based on its length.

### 💡 Explanation

The function uses the `len()` function to determine the username length and returns `"Weak"`, `"Good"`, or `"Strong"` accordingly.

### 📝 Solution

```python
def check_username(username):
    if len(username) < 5:
        return "Weak"
    elif len(username) <= 10:
        return "Good"
    else:
        return "Strong"

username = input("Enter your username: ")
result = check_username(username)
print(result)
```

---

## Answer 4 – Number Analyzer

### 📌 Question

Write a Python program that asks the user for a number and determines whether it is positive or negative, and whether it is even or odd.

### 💡 Explanation

The program first checks whether the number is positive, negative, or zero. Then it checks whether the number is even or odd using the modulo (`%`) operator.

### 📝 Solution

```python
number = int(input("Enter the number: "))

if number > 0:
    print("Positive")
elif number < 0:
    print("Negative")
else:
    print("Zero")

if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

---

## Answer 5 – Smart Greeting

### 📌 Question

Write a Python function `greet(name)` that displays a special welcome message for `"Radhika"` and a normal greeting for everyone else.

### 💡 Explanation

The function compares the entered name with `"Radhika"` and prints the appropriate greeting.

### 📝 Solution

```python
def greet(name):
    if name == "Radhika":
        print("Welcome back, Radhika!")
    else:
        print(f"Hello, {name}")

name = input("Enter your name: ")
greet(name)
```

---

## Answer 6 – Exam Result Calculator

### 📌 Question

Write a Python function `calculate_grade(marks)` that returns the student's grade based on the given marks.

### 💡 Explanation

The function checks the marks using multiple `elif` conditions and returns the appropriate grade.

### 📝 Solution

```python
def calculate_grade(marks):
    if marks >= 90:
        return "A"
    elif marks >= 80:
        return "B"
    elif marks >= 70:
        return "C"
    else:
        return "Fail"

marks = float(input("Enter the marks: "))
grade = calculate_grade(marks)
print(grade)
```

---

## Answer 7 – Mini ATM

### 📌 Question

Write a Python program that asks the user for the account balance and withdrawal amount. If sufficient balance is available, display the remaining balance; otherwise, display `"Insufficient Funds"`.

### 💡 Explanation

The program compares the withdrawal amount with the available balance and performs the transaction only if enough balance exists.

### 📝 Solution

```python
balance = float(input("Enter your balance: "))
withdraw = float(input("Enter the withdrawal amount: "))

if withdraw > balance:
    print("Insufficient Funds")
else:
    print(f"Remaining Balance: ₹{balance - withdraw}")
```

---

## Answer 8 – Number Comparison Challenge

### 📌 Question

Write a Python function `compare(a, b)` that compares two numbers and returns `"Greater"`, `"Smaller"`, or `"Equal"`.

### 💡 Explanation

The function compares two numbers using conditional statements and returns the appropriate result.

### 📝 Solution

```python
def compare(a, b):
    if a > b:
        return "Greater"
    elif a < b:
        return "Smaller"
    else:
        return "Equal"

num1 = int(input("Enter the first number: "))
num2 = int(input("Enter the second number: "))

print(compare(num1, num2))
```

---

## Answer 9 – Leap Year Checker Function

### 📌 Question

Write a Python function `is_leap(year)` that returns `True` if the given year is a leap year; otherwise, return `False`.

### 💡 Explanation

The function contains the leap year logic, while the main program only displays the result. This separates the program logic from the output.

### 📝 Solution

```python
def is_leap(year):
    if year % 400 == 0 or (year % 4 == 0 and year % 100 != 0):
        return True
    else:
        return False

year = int(input("Enter the year: "))

if is_leap(year):
    print("Leap Year")
else:
    print("Not Leap Year")
```

---

## Answer 10 – FizzBuzz Lite

### 📌 Question

Write a Python program that asks the user for a number and prints `"Fizz"`, `"Buzz"`, `"FizzBuzz"`, or the number based on divisibility rules.

### 💡 Explanation

The program first checks whether the number is divisible by both `3` and `5`. It then checks for divisibility by `3` and `5` individually. The combined condition must always be checked first.

### 📝 Solution

```python
number = int(input("Enter the number: "))

if number % 3 == 0 and number % 5 == 0:
    print("FizzBuzz")
elif number % 3 == 0:
    print("Fizz")
elif number % 5 == 0:
    print("Buzz")
else:
    print(number)
```

---

## ⭐ Bonus Challenge – Login Function

### 📌 Question

Write a Python function `login(username, password)` that returns `"Login Successful"` only if both the username and password are correct.

### 💡 Explanation

The function compares both the username and password using the logical `and` operator. Access is granted only when both conditions are true.

### 📝 Solution

```python
def login(username, password):
    if username == "admin" and password == "python123":
        return "Login Successful"
    else:
        return "Invalid Credentials"

username = input("Enter username: ")
password = input("Enter password: ")

print(login(username, password))
```
