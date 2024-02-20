# Banking-System

<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZ3NuYndvYndhdXJ2cHN5OGhva2JvMXVyYXViZnFxbmUzOTNxMHpuMyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/3o6ZsXrHsEKbSjKPeg/giphy.gif" height="200">
A simple console-based banking system in C++. It uses classes to model bank accounts and a bank, and it provides basic operations such as opening an account, checking the balance, depositing and withdrawing money, closing an account, and displaying all accounts.
Here's a brief overview of the code structure:

Account Class:

Represents a bank account with attributes like account number, first name, last name, and balance.
Provides methods for depositing and withdrawing money.
Overloaded stream operators (<< and >>) for reading from and writing to files and displaying account details.
Bank Class:

Manages a collection of accounts using a map.
Provides methods for opening an account, checking balance, depositing, withdrawing, closing an account, and displaying all accounts.
The constructor reads existing account data from a file ("Bank.data") to initialize the bank's state. The destructor writes the current account data back to the file.
Main Function:

Displays a menu for the user to choose banking operations.
The user can open an account, check balance, deposit, withdraw, close an account, show all accounts, or quit the program.
File Handling:

The program uses file input/output to persist account data between program runs. The "Bank.data" file is read during the initialization of the Bank class, and it is updated when accounts are modified or new accounts are added.
Static Variable:

The NextAccountNumber is a static variable in the Account class that is used to assign a unique account number to each new account.
Exception Handling:

The InsufficientFunds class is used for exception handling when a withdrawal would result in a balance below the minimum required.
Loop:

The program is implemented in a do-while loop, allowing the user to perform multiple operations until choosing to quit.
