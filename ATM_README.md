# ATM Withdrawal System

A Python program that simulates an ATM withdrawal system with balance validation.

---

## How to Run

```
python3 atm_withdrawal.py
```

---

## Logic

* Fixed account balance: **₹5000**
* Takes withdrawal amount as input
* Validates the request before processing

## Validations (in order)

1. Amount must be **greater than 0**
2. Amount must be a **multiple of 500**
3. Account must have **sufficient balance**

---

## Example

**Success Case:**

```
Enter withdrawal amount: 2000
Withdrawal successful. Amount: 2000
Remaining balance: 3000
```

**Failure Cases:**

```
Enter withdrawal amount: -100
Error: Withdrawal amount must be greater than 0
```

```
Enter withdrawal amount: 1200
Error: Withdrawal amount must be multiple of 500
```

```
Enter withdrawal amount: 6000
Error: Insufficient balance. Available: 5000
```

---

## Returns

| Result               | Return Value |
| -------------------- | ------------ |
| Success              | `True`     |
| Any validation fails | `False`    |
