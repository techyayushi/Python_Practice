# Set 5: Loops, Lists & Dictionaries — Solutions

## Question 1 — Count to N

### Question

Ask the user for a positive integer **N** and print all numbers from **1** to **N**.

### Answer

```python
n = int(input("Enter N: "))

for i in range(1, n + 1):
    print(i)
```

---

## Question 2 — Sum of First N Numbers

### Question

Ask the user for **N** and calculate the sum of all numbers from **1** to **N** using a loop.

### Answer

```python
n = int(input("Enter N: "))

total = 0

for i in range(1, n + 1):
    total = total + i

print(f"Sum = {total}")
```

---

## Question 3 — Even Numbers

### Question

Print all even numbers between **1** and **50** using two different methods.

### Answer — Method 1

```python
for i in range(1, 51):
    if i % 2 == 0:
        print(i)
```

### Answer — Method 2

```python
for i in range(2, 51, 2):
    print(i)
```

---

## Question 4 — Shopping List

### Question

Create the following list:

```python
shopping = ["Milk", "Bread", "Eggs", "Butter"]
```

Print each item with its number.

### Answer

```python
shopping = ["Milk", "Bread", "Eggs", "Butter"]

for index, item in enumerate(shopping, start=1):
    print(f"{index}. {item}")
```

---

## Question 5 — Student Marks

### Question

Create the given dictionary and ask the user for a student's name. If the student exists, print their marks. Otherwise, print `"Student not found"`.

### Answer

```python
marks = {
    "Riya": 90,
    "Rahul": 82,
    "Anjali": 95,
    "Karan": 76
}

name = input("Enter student name: ")

if name in marks:
    print(f"Marks: {marks[name]}")
else:
    print("Student not found")
```

---

## Question 6 — Multiplication Table

### Question

Ask the user for a number and print its multiplication table up to **10**.

### Answer

```python
number = int(input("Enter number: "))

for i in range(1, 11):
    print(f"{number} × {i} = {number * i}")
```

---

## Question 7 — Password Attempts

### Question

The correct password is `"python123"`. Give the user **3 attempts**. If the password is correct, print `"Access Granted"`. Otherwise, print `"Account Locked"`.

### Answer

```python
correct_password = "python123"

for attempt in range(3):
    password = input("Enter password: ")

    if password == correct_password:
        print("Access Granted")
        break
else:
    print("Account Locked")
```

---

## Question 8 — Grocery Bill

### Question

Create the given price dictionary. Ask the user for an item and quantity. If the item exists, calculate the total. Otherwise, print `"Item not available"`.

### Answer

```python
prices = {
    "Rice": 60,
    "Milk": 30,
    "Bread": 40,
    "Eggs": 80
}

item = input("Enter item: ")
quantity = int(input("Enter quantity: "))

if item in prices:
    total = prices[item] * quantity
    print(f"Total = ₹{total}")
else:
    print("Item not available")
```

---

## Question 9 — Number Guessing Game ⭐

### Question

The secret number is **7**. Keep asking the user to guess until they guess correctly. Print `"Try Again"` for a wrong guess and `"Congratulations!"` for the correct guess.

### Answer

```python
secret_number = 7

while True:
    guess = int(input("Enter your guess: "))

    if guess == secret_number:
        print("Congratulations!")
        break
    else:
        print("Try Again")
```

---

## Question 10 — Mini Menu

### Question

Display the following menu repeatedly:

```text
1. Say Hello
2. Add Two Numbers
3. Exit
```

Handle each option and continue until the user chooses Exit.

### Answer

```python
while True:
    print("\n1. Say Hello")
    print("2. Add Two Numbers")
    print("3. Exit")

    choice = input("Enter your choice: ")

    if choice == "1":
        print("Hello!")

    elif choice == "2":
        first = int(input("Enter first number: "))
        second = int(input("Enter second number: "))

        print(f"Sum = {first + second}")

    elif choice == "3":
        print("Exiting...")
        break

    else:
        print("Invalid Choice")
```

---

# ⭐ Bonus Challenge — Student Report Card

### Question

Store student names and their marks in a dictionary. Ask for a student's name. If found, print all marks and calculate the average using a loop. Otherwise, print `"Student not found"`.

### Answer

```python
students = {
    "Radhika": [90, 85, 88],
    "Aman": [78, 82, 80],
    "Priya": [95, 91, 97]
}

name = input("Enter student name: ")

if name in students:
    marks = students[name]

    print("Marks:")

    total = 0

    for mark in marks:
        print(mark)
        total = total + mark

    average = total / len(marks)

    print(f"Average: {average:.2f}")

else:
    print("Student not found")
```
