# Restaurant Bill Calculator

A Python program that calculates the total restaurant bill including service charge, tax, and tip.

---

## How to Run

```
python3 restaurant_bill.py
```

---

## Logic

* Takes meal cost as input
* Calculates service charge, tax, and tip step by step
* Prints full bill breakdown

## Calculation Order

| Step | What                 | Rate                             |
| ---- | -------------------- | -------------------------------- |
| 1    | Service Charge       | 10% of meal cost                 |
| 2    | Amount after Service | Meal cost + Service charge       |
| 3    | Tax                  | 5% of amount after service       |
| 4    | Tip                  | 5% of amount after service       |
| 5    | Total Bill           | Amount after service + Tax + Tip |

---

## Example

```
Enter meal cost: 500
Meal Cost: 500.0
Service Charge (10%): 50.0
Amount after Service: 550.0
Tax (5%): 27.5
Tip (5%): 27.5
Total Bill: 605.0
```

---

## Returns

Total bill amount as a float value.
