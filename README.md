# Case 3: Personal Finance Tracker

## Project Description

This project is a simple Personal Finance Tracker made in Python.  
The program helps users track their income and expenses.

User can:

- add income
- add expenses
- choose expense category
- check balance
- see category breakdown
- see monthly summary
- detect overspending
- see basic statistics

The data is saved in a JSON file, so after closing the program the information is not lost.

---

## Team Contribution

Our team divided the work like this:

- Zhumabay Aikyn — worked on `manager.py`
- Alikhanov Alizhan — worked on `main.py`
- Seipenov Damir — worked on `models.py` and `storage.py`
- All team members — worked together on `tests.py`

---

## Project Files

### `main.py`

This is the main file of the project.  
It shows the menu and gets input from the user.

The user can choose options like:

1. Add income
2. Add expense
3. Show balance
4. Show category breakdown
5. Show monthly summary
6. Detect overspending
7. Show statistics
8. Exit

---

### `models.py`

This file contains classes for transactions.

Classes:

- `Transaction`
- `Income`
- `Expense`

`Transaction` is the base class.  
`Income` and `Expense` inherit from it.

We used OOP here because income and expense are both transactions, but expense also has a category.

---

### `manager.py`

This file contains the main logic of the project.

It has the `FinanceManager` class.

It can:

- calculate balance
- detect overspending
- calculate category summary
- calculate monthly summary
- show statistics
- get all categories

---

### `storage.py`

This file is used for file handling.

It loads and saves data from `data.json`.

We used JSON because the task input format is JSON and it is easy to read and write in Python.

---

### `tests.py`

This file contains basic tests using `assert`.

The tests check:

- balance calculation
- overspending detection
- category summary
- monthly summary
- statistics
- empty input
- classes `Income` and `Expense`

---

## How to Run the Project

1. Open main.py
2. Start main.py

or

1. Open the project folder.
2. Run this command:

```bash
python main.py
