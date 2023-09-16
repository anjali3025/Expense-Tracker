# expense-tracker
The provided Python script is an Expense Tracker application with a graphical user interface (GUI) built using the Tkinter library, and it uses SQLite as the database to store and manage 
expense records. 
1) Imports:The script starts by importing necessary modules:
datetime: Used for working with date and time.
sqlite3: Used for connecting to and manipulating the SQLite database.
tkcalendar.DateEntry: A custom Tkinter widget for date input.
tkinter: The primary library for creating the GUI.
tkinter.messagebox: Used for displaying message boxes.
tkinter.ttk: Provides access to the themed Tkinter widgets.

2) Database Connection: It connects to an SQLite database named "Expense Tracker.db" and creates a cursor for executing SQL commands.
The script also creates an "ExpenseTracker" table if it doesn't exist already. This table is used to store expense records with columns for ID, Date, Payee, Description, Amount, and
Mode of Payment.

3) Functions: The code defines several functions for various actions related to the Expense Tracker application, including adding, editing, deleting, and listing expenses.
Functions like list_all_expenses, view_expense_details, clear_fields, remove_expense, remove_all_expenses, add_another_expense, edit_expense, and others handle different aspects of 
managing expenses in the application.

4) GUI Creation: The GUI is created using Tkinter and consists of various frames, labels, buttons, and an interactive table (Treeview).
The main window (root) is initialized with a title and fixed dimensions.
Different frames (data_entry_frame, buttons_frame, tree_frame) are created to organize the layout of widgets.
Widgets such as labels, entry fields, buttons, and dropdown menus are added to the frames.
The Treeview widget (table) is used to display and manipulate expense records in a tabular format.

5)bWidget Configuration: Widgets are configured with appropriate fonts, colors, and event handlers.
For example, the DateEntry widget is used to input dates, and the OptionMenu widget is used for selecting the mode of payment.

6) Button Actions: Buttons placed in the GUI trigger various actions when clicked. For instance, the "Add expense" button calls the add_another_expense function to add a new expense
   record to the database.
   
7) Database Operations: Functions like add_another_expense, edit_existing_expense, remove_expense, and remove_all_expenses interact with the SQLite database by executing SQL commands
   to add, edit, or delete records.
   
8) Treeview (Table): The Treeview widget (table) is used to display expense records fetched from the database.
It supports features like scrolling, column headings, and selection of rows.
The list_all_expenses function populates this table with data from the database.

9) Main Loop: The script enters the main event loop (root.mainloop()) to start the GUI application. This loop listens for user interactions and responds accordingly.
