# Accounting Ledger App

This is a simple console-based accounting ledger built using Java. It lets users record deposits and payments, and view transaction history through a menu-based interface. The data is saved to a CSV file for persistence.

## Features

- Add deposit and payment transactions
- Automatically saves transactions to `transactions.csv`
- View all transactions, deposits only, or payments only
- Generate reports:
  - Month to Date
  - Previous Month
  - Year to Date
  - Previous Year
  - Search by vendor name

## How to Run

1. Make sure you have Java installed (Java 8 or higher).
2. Download or clone this project to your computer.
3. Compile and run the `AccountingLedgerApp.java` file.

```bash
javac AccountingLedgerApp.java
java AccountingLedgerApp
```

4. Use the on-screen menu to add transactions or view reports.

## CSV File Format

All transactions are saved to a file called `transactions.csv` in the same folder. Each entry looks like this:

```
2025-05-04|14:30:00|Lunch with team|Subway|-15.99
```

The order of fields is:
- Date
- Time
- Description
- Vendor
- Amount (positive for deposits, negative for payments)

## Technologies Used

- Java (Standard Edition)
- Java I/O (BufferedReader, BufferedWriter)
- Java Time (LocalDate, LocalTime)
- Collections (ArrayList, List)

## Author Notes

This was created as a capstone project for my Java course. I learned a lot about file handling, classes, and organizing code using object-oriented programming. The project could be improved later by adding features like editing or deleting transactions, better formatting, or a GUI.
