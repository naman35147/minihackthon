# Smart Canteen Billing System

A menu-driven **C programming project** that simulates billing in a college canteen. Users can select food items, enter quantities, and generate an itemised bill.

## Features
- Menu with five food items and fixed prices.
- Supports multiple items and repeated orders of the same item.
- Validates quantities (must be greater than zero).
- Applies a **10% discount** when the subtotal is **more than Rs. 500** (exactly Rs. 500 gets no discount).
- Displays itemised orders, subtotal, discount, and final bill.
- Handles invalid menu choices by displaying an error and repeating the menu.

## Menu
| Option | Item | Price |
|---|---|---:|
| 1 | Burger | Rs. 80 |
| 2 | Pizza | Rs. 120 |
| 3 | Sandwich | Rs. 60 |
| 4 | Fries | Rs. 70 |
| 5 | Cold Drink | Rs. 40 |
| 6 | Generate Bill | — |

## C Concepts Used
- Variables and data types (`int`, `float`)
- Arithmetic, relational, logical, and compound-assignment operators
- `printf()` and `scanf()` for input/output
- `if` / nested `if` for validation and discount logic
- `switch-case` for menu handling
- `do-while` loop to repeat the menu
- `continue` for invalid quantity handling

## How to Compile and Run
Using GCC:

```bash
gcc canteen_billing.c -o canteen_billing
./canteen_billing
```

On Windows, run:

```bash
canteen_billing.exe
```

## Discount Rule
If the subtotal is greater than Rs. 500, the discount is 10% of the subtotal. Otherwise, the discount is Rs. 0.

**Example:** Subtotal = Rs. 540 → Discount = Rs. 54 → Final bill = Rs. 486.

## Testing
The project was tested with:
- A normal order without discount
- Multiple items with discount
- Boundary case (subtotal exactly Rs. 500)
- Invalid quantity
- Invalid menu choice
- Mixed valid and invalid inputs
- Generating a bill without ordering

All listed test cases passed in the project report.

## Limitations and Future Scope
- Non-numeric input is not handled yet.
- Menu prices and item counters are hard-coded.
- Bills are not saved to a file.

Possible improvements include using arrays or structures, handling non-numeric input, and adding file handling to save bills.

## Project Team
- Naman Agrawal
- Yuvraj Singh
- Vansh Tyagi

## Submitted To
Manish Giri
