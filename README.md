# COSC 310 — Lecture 2

Python exercises for menu filtering, a shopping cart, and business-rule validation.

Run the examples with `python3 exercise1.py`, `python3 exercise2.py`, and
`python3 exercise3.py`.

Install test dependencies with `python3 -m pip install -r requirements.txt`,
then run `python3 -m pytest -v`.

Exercise 3 enforces its business rules inside `Cart`: `add_item` rejects
quantities below one and unavailable items; `remove_item` rejects missing items.
The executable example demonstrates each rejection with `try/except`.
