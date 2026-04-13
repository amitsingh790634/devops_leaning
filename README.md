# Python Programming Assignment

---

## Question 1: ATM Withdrawal System

Write a Python program that simulates an ATM withdrawal system. The program should validate the withdrawal request based on multiple conditions before processing it.

### Requirements

- Create a function `atm_withdrawal(withdrawal_amount)` that takes withdrawal amount as input
- The current balance in the account is fixed at **5000**
- The function should validate:
  - **Validation 1:** Withdrawal amount must be greater than 0
    - If invalid: Print `Error: Withdrawal amount must be greater than 0`
  - **Validation 2:** Withdrawal amount must be a multiple of 500
    - If invalid: Print `Error: Withdrawal amount must be multiple of 500`
  - **Validation 3:** Account balance must be sufficient for withdrawal
    - If invalid: Print `Error: Insufficient balance. Available: {current_balance}`
- If all validations pass:
  - Calculate remaining balance
  - Print `Withdrawal successful. Amount: {withdrawal_amount}`
  - Print `Remaining balance: {remaining_balance}`
  - Return `True`
- If any validation fails:
  - Print the specific error message
  - Return `False`
- Accept withdrawal amount from user using `input()` and convert to integer

### Test Case

```
Input: 2000

Withdrawal successful. Amount: 2000
Remaining balance: 3000
Return: True
```

### How to Run

```
python3 atm_withdrawal.py
```

---

## Question 2: Restaurant Bill Calculator

Write a Python program that calculates the total restaurant bill including service charge, tax, and tip.

### Requirements

- Create a function `calculate_restaurant_bill(meal_cost)` that takes meal cost as input
- The tip is fixed at **5%**
- Calculate the following in order:
  1. Service Charge: 10% of meal cost
  2. Amount after Service: Meal cost + Service charge
  3. Tax: 5% of amount after service
  4. Tip: 5% of amount after service
  5. Total Bill: Amount after service + Tax + Tip
- Accept meal cost from user using `input()` and convert to float

### Output Format

```
Meal Cost: {meal_cost}
Service Charge (10%): {service_charge}
Amount after Service: {amount_after_service}
Tax (5%): {tax}
Tip (5%): {tip_amount}
Total Bill: {total}
```

### Test Case

```
Input: 500

Meal Cost: 500.0
Service Charge (10%): 50.0
Amount after Service: 550.0
Tax (5%): 27.5
Tip (5%): 27.5
Total Bill: 605.0
Return: 605.0
```

### How to Run

```
python3 restaurant_bill.py
```

---

## Question 3: Login Authentication System

Write a Python program that validates a user's login credentials based on specific security requirements.

### Requirements

- Create a function `validate_login(username, password)` that takes username and password as input
- The function should validate:
  - **Validation 1:** Username length must be at least 5 characters
    - If invalid: Print `Error: Username must be at least 5 characters.`
    - Return `False`
  - **Validation 2:** Password length must be at least 8 characters
    - If invalid: Print `Error: Password must be at least 8 characters.`
    - Return `False`
  - **Validation 3:** Password must contain at least one digit (0-9)
    - Use a loop to check each character
    - Use the `char.isdigit()` method to check if a character is a digit
    - If invalid: Print `Error: Password must contain at least one digit`
    - Return `False`
- If all validations pass:
  - Print `Login successful.`
  - Return `True`
- Validations should be checked in order — stop at first failure
- Accept username and password from user using `input()`

### Test Case

```
Input:
username: john_doe
password: Pass1234

Login successful
Return: True
```

### How to Run

```
python3 login_auth.py
```

---

## General Instructions

1. Read each question carefully
2. Plan your solution before writing code
3. Test your code with all provided test cases
4. Make sure output format matches exactly
5. Handle all edge cases
6. Write clean, readable code
7. Add meaningful comments
8. Use proper variable names

---

## Project Structure

```
Python/
├── atm_withdrawal.py
├── ATM_README.md
├── restaurant_bill.py
├── Restaurant_README.md
├── login_auth.py
├── Login_README.md
└── README.md
```
