# Set 5: Loops, Lists & Dictionaries

This set introduces repetition using loops and storing collections of data with lists and dictionaries. You'll also build small interactive programs using these concepts.

## Topics Covered

* `for` loops
* `while` loops
* `range()`
* `break`
* Lists
* Dictionaries
* `enumerate()`
* User input
* Basic functions
* Nested data structures

---

# Question 1 — Count to N

## Problem

Ask the user for a positive integer **N**.

Print all numbers from **1** to **N**.

### Example

```text id="6myy5m"
Enter N: 5

1
2
3
4
5
```

## Concepts

* `for` loop
* `while` loop
* `range()`

---

# Question 2 — Sum of First N Numbers

## Problem

Ask the user for **N**.

Calculate:

```text id="k5y5t8"
1 + 2 + 3 + ... + N
```

Do **not** use the mathematical formula.

Use a loop.

### Example

```text id="w7n8x4"
Enter N: 5

Sum = 15
```

## Concepts

* Loops
* Variables
* Arithmetic

---

# Question 3 — Even Numbers

## Problem

Print all even numbers between **1** and **50**.

Try solving it in **two different ways**.

### Example

```text id="g6m8sq"
2
4
6
...
50
```

## Concepts

* `for` loop
* `range()`
* Modulo operator

---

# Question 4 — Shopping List

## Problem

Create the following list:

```python id="0qks6x"
shopping = ["Milk", "Bread", "Eggs", "Butter"]
```

Print:

```text id="h3g5aq"
1. Milk
2. Bread
3. Eggs
4. Butter
```

> **Hint:** You may need a counter.

## Concepts

* Lists
* `enumerate()`
* Loops

---

# Question 5 — Student Marks

## Problem

Create the dictionary:

```python id="zj2f4w"
marks = {
    "Riya": 90,
    "Rahul": 82,
    "Anjali": 95,
    "Karan": 76
}
```

Ask the user for a student's name.

If the student exists, print their marks.

Otherwise print:

```text id="3wq7j4"
Student not found
```

## Concepts

* Dictionaries
* Membership (`in`)
* User input

---

# Question 6 — Multiplication Table

## Problem

Ask the user for a number.

Print its multiplication table up to **10**.

### Example

```text id="a8k9kz"
7 × 1 = 7
7 × 2 = 14
...
7 × 10 = 70
```

## Concepts

* `for` loop
* `range()`
* Arithmetic

---

# Question 7 — Password Attempts

## Problem

Correct password:

```text id="n3s4f5"
python123
```

The user gets **3 attempts**.

If the password is correct:

```text id="k3v8ez"
Access Granted
```

Otherwise:

```text id="j6p4wd"
Account Locked
```

Use either a **`for`** or **`while`** loop.

## Concepts

* `while` loop
* `break`
* `if/else`

---

# Question 8 — Grocery Bill

## Problem

Create:

```python id="0v9s6c"
prices = {
    "Rice": 60,
    "Milk": 30,
    "Bread": 40,
    "Eggs": 80
}
```

Ask the user for:

* Item
* Quantity

If the item exists, calculate:

```text id="z9b4pc"
Total = Price × Quantity
```

Otherwise print:

```text id="5c9h8j"
Item not available
```

## Concepts

* Dictionaries
* Arithmetic
* `if/else`

---

# Question 9 — Number Guessing Game ⭐

## Problem

Secret number:

```text id="g5z1p3"
7
```

Keep asking the user until they guess correctly.

If the guess is wrong:

```text id="4p9r2a"
Try Again
```

If correct:

```text id="x7q3m5"
Congratulations!
```

Use a **`while`** loop.

## Concepts

* `while` loop
* `break`
* User input

---

# Question 10 — Mini Menu (Challenge)

## Problem

Display this menu repeatedly:

```text id="n4x7w2"
1. Say Hello
2. Add Two Numbers
3. Exit
```

### Rules

#### Option 1

Print:

```text id="q8m2kc"
Hello!
```

#### Option 2

Ask for two numbers and print their sum.

#### Option 3

Exit the program.

If the user enters an invalid option, print:

```text id="f6t9va"
Invalid Choice
```

Continue showing the menu until the user chooses **Exit**.

## Concepts

* `while` loop
* Functions
* Menu-driven programs

---

# ⭐ Bonus Challenge — Student Report Card

## Problem

Store:

```python id="2y5w7m"
students = {
    "Radhika": [90, 85, 88],
    "Aman": [78, 82, 80],
    "Priya": [95, 91, 97]
}
```

Ask the user for a student's name.

If found:

* Print all marks
* Calculate the average **using a loop**
* Print the average

Otherwise print:

```text id="8q4n6v"
Student not found
```

## Concepts

* Lists
* Dictionaries
* Loops
* Functions
* Nested data structures
