# 🐍 Set 1 – Functions, Variables, Strings, Integers & Floats

This document contains the solutions for Set 1 Python practice questions.

---

## Answer 1 – Greeting Program

### Question
Ask the user for their name and print a greeting.

### Solution

```python
name = input("What is your name? ")
print(f"Hello, {name}")
```

---

## Answer 2 – Favorite Language

### Question
Ask the user for their favorite programming language and print a response.

### Solution

```python
language = input("Favorite language: ")
print(f"{language} sounds interesting!")
```

---

## Answer 3 – Age Next Year

### Question
Ask the user for their current age and display their age next year.

### Solution

```python
age = int(input("Age: "))
print(f"Next year you will be {age + 1}")
```

---

## Answer 4 – Simple Calculator

### Question
Ask the user for two numbers and display their sum, difference, and product.

### Solution

```python
num1 = int(input("First number: "))
num2 = int(input("Second number: "))

print(f"Sum: {num1 + num2}")
print(f"Difference: {num1 - num2}")
print(f"Product: {num1 * num2}")
```

---

## Answer 5 – Full Name Formatter

### Question
Ask separately for the first name and last name, then display the full name using an f-string.

### Solution

```python
first_name = input("First name: ")
last_name = input("Last name: ")

print(f"Hello, {first_name} {last_name}")
```

---

## Answer 6 – Bill Splitter

### Question
A restaurant bill is ₹1250. Ask how many friends are sharing it and calculate the amount each person pays.

### Solution

```python
bill = 1250

friends = int(input("Number of friends: "))

share = bill / friends

print(f"Each person pays: {share}")
```

---

## Answer 7 – Temperature Converter

### Question
Ask the user for the temperature in Celsius and convert it to Fahrenheit.

### Solution

```python
celsius = float(input("Celsius: "))

fahrenheit = (celsius * 9 / 5) + 32

print(f"Fahrenheit: {fahrenheit}")
```

---

## Answer 8 – Custom Function

### Question
Create a function that greets the user by name.

### Solution

```python
def greet(name):
    print(f"Hello, {name}")

greet("Radhika")
```

---

## Answer 9 – Return Value

### Question
Create a function that returns the square of a number.

### Solution

```python
def square(n):
    return n * n

print(square(5))
```

---

## Answer 10 – Mini Profile Generator

### Question
Ask for the user's name, age, and city, then display the information using f-strings.

### Solution

```python
name = input("Name: ")
age = int(input("Age: "))
city = input("City: ")

print("----- PROFILE -----")
print(f"Name: {name}")
print(f"Age: {age}")
print(f"City: {city}")
print("-------------------")
```
