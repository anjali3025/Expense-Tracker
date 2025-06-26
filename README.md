# 💰 Expense Tracker

A simple **Expense Tracker** application built with **Python** using **Tkinter** for the GUI and **SQLite** for persistent data storage. It helps users record, view, edit, and manage daily expenses efficiently.

---

## 🚀 Features

- Add, view, edit, and delete expenses
- User-friendly graphical interface (Tkinter)
- SQLite database for local storage
- Calendar widget for easy date selection
- Treeview table to display records
- Sortable and scrollable table view

---

## 🛠️ Tech Stack

- **Python**
- **Tkinter** – GUI library
- **SQLite** – Lightweight database
- **tkcalendar.DateEntry** – Calendar widget for date inputs

---

## 📁 Project Structure

- `Expense Tracker.db` – SQLite database file
- `main.py` – Main Python script containing logic and UI

---

## 📦 How It Works

### 1. **Imports**
The script uses:
- `datetime` – Handle dates and times
- `sqlite3` – Database connection and queries
- `tkinter` – GUI elements
- `tkcalendar` – Calendar input for date selection

### 2. **Database Initialization**
- Connects to `Expense Tracker.db`
- Creates a table `ExpenseTracker` with:
  - `ID`
  - `Date`
  - `Payee`
  - `Description`
  - `Amount`
  - `Mode of Payment`

### 3. **Core Functions**
- `add_another_expense()` – Add new expense
- `edit_expense()` – Update selected expense
- `remove_expense()` – Delete selected entry
- `remove_all_expenses()` – Delete all records
- `list_all_expenses()` – Populate table with data
- `view_expense_details()` – Show selected row’s details
- `clear_fields()` – Clear form inputs

### 4. **GUI Components**
- Structured using `Frames`:
  - Entry section for new data
  - Action buttons (Add, Edit, Delete, Clear)
  - Treeview table to display expenses
- Widgets include `Labels`, `Entry`, `DateEntry`, `OptionMenu`, `Treeview`, and `Buttons`

### 5. **User Interaction**
- Buttons trigger defined functions to interact with the database
- Treeview displays records with scroll support and selection-based interaction

### 6. **Main Event Loop**
- The GUI runs inside `root.mainloop()` to handle events continuously

---

## 📸 Screenshot

*Add a screenshot here if you'd like:*

```bash
📷 Screenshot goes here (e.g., ./screenshots/main_ui.png)

