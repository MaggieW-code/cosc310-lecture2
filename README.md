# COSC 310 — Lecture 2

Python exercises for menu filtering, a shopping cart, and business-rule validation.

Run the examples with `python3 exercise1.py`, `python3 exercise2.py`, and
`python3 exercise3.py`.

Create and activate a virtual environment, install the test dependencies, and run
the tests:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
pytest -v
```

The `.venv/` directory is excluded from Git by `.gitignore`.

Exercise 3 enforces its business rules inside `Cart`: `add_item` rejects
quantities below one and unavailable items; `remove_item` rejects missing items.
The executable example demonstrates each rejection with `try/except`.

Exercise 5 tests are in `tests/test_cart.py`. They cover an empty cart, totals for
multiple items, combining duplicate items into one line, rejecting zero quantity,
rejecting unavailable items, and rejecting removal of an absent item. An additional
test checks that removing an item removes its entire quantity, preserves the
remaining item, and updates the total.

Latest test result: **7 passed**.
