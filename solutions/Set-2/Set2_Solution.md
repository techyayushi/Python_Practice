# 🐍 Set 2 – Conditional Statements

This document contains the solutions for Set 2 Python practice questions.

---

## Answer 1 – Positive, Negative, or Zero

### 📌 Question

Write a Python program that asks the user to enter a number and determines whether the number is positive, negative, or zero.

### 💡 Explanation

The program accepts a number from the user and uses `if`, `elif`, and `else` statements to compare the value with zero and determine its type.

### 📝 Solution

```python
number = float(input("Enter the number: "))

if number > 0:
    print("Positive")
elif number < 0:
    print("Negative")
else:
    print("Zero")
```

---

## Answer 2 – Even or Odd

### 📌 Question

Write a Python program that asks the user to enter an integer and determines whether it is even or odd.

### 💡 Explanation

The program uses the modulo (`%`) operator to check whether the remainder after dividing the number by `2` is `0`. If it is, the number is even; otherwise, it is odd.

### 📝 Solution

```python
number = int(input("Enter the number: "))

if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

---

## Answer 3 – Voting Eligibility

### 📌 Question

Write a Python program that asks the user for their age and determines whether they are eligible to vote.

### 💡 Explanation

The program compares the entered age with the minimum voting age of `18`. If the age is `18` or above, the user is eligible to vote; otherwise, they are not.

### 📝 Solution

```python
age = int(input("Enter your age: "))

if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible to vote")
```

---

## Answer 4 – Password Checker

### 📌 Question

Write a Python program that asks the user to enter a password and checks whether it matches the predefined password.

### 💡 Explanation

The program stores the correct password in a variable and compares it with the user's input using an `if-else` statement.

### 📝 Solution

```python
password = "python123"

user_password = input("Enter the password: ")

if user_password == password:
    print("Access Granted")
else:
    print("Access Denied")
```

---

## Answer 5 – Largest of Two Numbers

### 📌 Question

Write a Python program that asks the user to enter two numbers and displays the larger number.

### 💡 Explanation

The program compares both numbers using an `if-else` statement and prints the larger value.

### 📝 Solution

```python
num1 = int(input("Enter the first number: "))
num2 = int(input("Enter the second number: "))

if num1 > num2:
    print(num1, "is larger")
else:
    print(num2, "is larger")
```

---

## Answer 6 – Grade Calculator

### 📌 Question

Write a Python program that asks the user to enter marks and prints the corresponding grade.

### 💡 Explanation

The program checks the entered marks against different ranges using multiple `elif` conditions and assigns the appropriate grade.

### 📝 Solution

```python
marks = float(input("Enter the marks: "))

if marks >= 90:
    print("A")
elif marks >= 80:
    print("B")
elif marks >= 70:
    print("C")
elif marks >= 60:
    print("D")
else:
    print("F")
```

---

## Answer 7 – Leap Year Lite

### 📌 Question

Write a Python program that asks the user to enter a year and checks whether it is a leap year using the simplified rule (`year % 4 == 0`).

### 💡 Explanation

The program uses the modulo (`%`) operator to determine whether the year is divisible by `4`. If it is, the year is considered a leap year for this simplified version.

### 📝 Solution

```python
year = int(input("Enter the year: "))

if year % 4 == 0:
    print("Leap Year")
else:
    print("Not Leap Year")
```

---

## Answer 8 – Movie Ticket Price

### 📌 Question

Write a Python program that asks the user for their age and displays the ticket price based on the given age criteria.

### 💡 Explanation

The program uses `if`, `elif`, and `else` statements to determine the ticket price according to the user's age.

### 📝 Solution

```python
age = int(input("Enter the age: "))

if age < 12:
    print("Ticket Price is ₹100")
elif age < 60:
    print("Ticket Price is ₹200")
else:
    print("Ticket Price is ₹150")
```

---

## Answer 9 – Username Validation

### 📌 Question

Write a Python program that asks the user to enter a username and checks whether its length is at least five characters.

### 💡 Explanation

The program uses the `len()` function to count the number of characters in the username. If the length is less than `5`, it displays an error message; otherwise, it accepts the username.

### 📝 Solution

```python
username = input("Enter your username: ")

if len(username) >= 5:
    print("Valid username")
else:
    print("Username too short")
```

---

## Answer 10 – Mini Calculator

### 📌 Question

Write a Python program that asks the user to enter two numbers and an operator (`+`, `-`, `*`, `/`), then performs the corresponding calculation.

### 💡 Explanation

The program accepts two numbers and an arithmetic operator from the user. It uses `if`, `elif`, and `else` statements to determine which operation to perform and then displays the result.

### 📝 Solution

```python
num1 = float(input("Enter the first number: "))
operator = input("Enter the operator (+, -, *, /): ")
num2 = float(input("Enter the second number: "))

if operator == "+":
    print(num1 + num2)
elif operator == "-":
    print(num1 - num2)
elif operator == "*":
    print(num1 * num2)
elif operator == "/":
    print(num1 / num2)
else:
    print("Invalid operator")
```
