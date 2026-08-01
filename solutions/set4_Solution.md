# 🐍 Set 4 – Mini Projects

This document contains the solutions for Set 4 Python mini projects.

---

# ☕ Project 1 – Coffee Shop

### 📌 Question

Write a Python program to create a coffee shop billing system.

The coffee shop sells:

- Espresso – ₹120
- Latte – ₹180
- Cappuccino – ₹200

Rules:

- Large size adds ₹40.
- Members receive a 10% discount.
- Use at least two functions.

### 💡 Explanation

The program uses one function to return the coffee price and another function to calculate the final bill after adding the large size charge and applying the membership discount.

### 📝 Solution

```python
def get_price(coffee):
    if coffee == "Espresso":
        return 120
    elif coffee == "Latte":
        return 180
    elif coffee == "Cappuccino":
        return 200
    else:
        return 0


def calculate_bill(price, large, member):
    if large == "yes":
        price += 40

    if member == "yes":
        price -= price * 0.10

    return price


coffee = input("Enter coffee name: ")
large = input("Large size? (yes/no): ")
member = input("Member? (yes/no): ")

price = get_price(coffee)

if price == 0:
    print("Invalid Coffee")
else:
    final_bill = calculate_bill(price, large, member)

    print("Coffee:", coffee)
    print("Size:", large)
    print("Member:", member)
    print(f"Final Bill: ₹{final_bill}")
```

---

# 🔐 Project 2 – Simple Login System

### 📌 Question

Write a Python program that checks the username and password.

Rules:

- Username: `admin`
- Password: `python123`

If the username is incorrect, display **Unknown User**.

If the password is incorrect, display **Incorrect Password**.

Otherwise, display **Welcome Admin**.

### 💡 Explanation

The program creates a function that validates both the username and password and returns the appropriate message.

### 📝 Solution

```python
def login(username, password):
    if username == "admin" and password == "python123":
        return "Welcome Admin"

    elif username != "admin":
        return "Unknown User"

    else:
        return "Incorrect Password"


username = input("Enter username: ")
password = input("Enter password: ")

result = login(username, password)
print(result)
```

---

# 🏃 Project 3 – BMI Calculator

### 📌 Question

Write a Python program to calculate the Body Mass Index (BMI) and classify the result.

Formula:

BMI = Weight / Height²

Categories:

- Below 18.5 → Underweight
- 18.5–24.9 → Normal
- 25–29.9 → Overweight
- 30 and above → Obese

Use two functions.

### 💡 Explanation

The first function calculates the BMI, while the second function classifies the BMI into the correct category.

### 📝 Solution

```python
def calculate_bmi(weight, height):
    return weight / (height ** 2)


def classify_bmi(bmi):
    if bmi < 18.5:
        return "Underweight"
    elif bmi < 25:
        return "Normal"
    elif bmi < 30:
        return "Overweight"
    else:
        return "Obese"


weight = float(input("Enter weight (kg): "))
height = float(input("Enter height (m): "))

bmi = calculate_bmi(weight, height)

print(f"BMI: {bmi:.2f}")
print("Category:", classify_bmi(bmi))
```

---

# ⚡ Project 4 – Electricity Bill

### 📌 Question

Write a Python program to calculate an electricity bill.

Rates:

- Below 100 units → ₹5 per unit
- 100–300 units → ₹7 per unit
- Above 300 units → ₹10 per unit

If the bill exceeds ₹2000, apply a ₹200 discount.

### 💡 Explanation

The program calculates the bill based on the number of units consumed and applies a discount if applicable.

### 📝 Solution

```python
def calculate_bill(units):
    if units < 100:
        bill = units * 5
    elif units <= 300:
        bill = units * 7
    else:
        bill = units * 10

    discount = 0

    if bill > 2000:
        discount = 200

    final_bill = bill - discount

    return bill, discount, final_bill


units = int(input("Enter electricity units: "))

bill, discount, final_bill = calculate_bill(units)

print("Units:", units)
print(f"Bill: ₹{bill}")
print(f"Discount: ₹{discount}")
print(f"Final Bill: ₹{final_bill}")
```

---

# 🍕 Project 5 – Restaurant Ordering

### 📌 Question

Write a Python program to calculate the restaurant bill.

Menu:

- Pizza – ₹300
- Burger – ₹180
- Pasta – ₹220

Rules:

- Ask for food item and quantity.
- If quantity is 5 or more, give a 15% discount.

### 💡 Explanation

The program determines the price of the selected food, calculates the total bill, and applies the discount if the quantity is five or more.

### 📝 Solution

```python
def get_price(food):
    if food == "Pizza":
        return 300
    elif food == "Burger":
        return 180
    elif food == "Pasta":
        return 220
    else:
        return 0


food = input("Enter food item: ")
quantity = int(input("Enter quantity: "))

price = get_price(food)

if price == 0:
    print("Food item not available")
else:
    total = price * quantity

    if quantity >= 5:
        total -= total * 0.15

    print(f"Final Bill: ₹{total}")
```

---

# ⭐ Bonus Project – Bank ATM

### 📌 Question

Write a Python program to simulate a simple ATM.

Initial balance:

₹5000

Options:

- Withdraw
- Deposit
- Check Balance

The program should perform one selected operation and then exit.

### 💡 Explanation

The program asks the user to choose an operation. Depending on the user's choice, it either withdraws money, deposits money, or displays the current balance.

### 📝 Solution

```python
balance = 5000

choice = input("Choose (Withdraw/Deposit/Balance): ")

if choice == "Withdraw":
    amount = float(input("Enter amount: "))

    if amount > balance:
        print("Insufficient Balance")
    else:
        balance -= amount
        print(f"Remaining Balance: ₹{balance}")

elif choice == "Deposit":
    amount = float(input("Enter amount: "))
    balance += amount
    print(f"Updated Balance: ₹{balance}")

elif choice == "Balance":
    print(f"Current Balance: ₹{balance}")

else:
    print("Invalid Option")
```

