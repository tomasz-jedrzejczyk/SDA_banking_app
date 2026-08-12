# SDA_banking_app

Simple **console banking application in Java**, built as teaching material for unit testing training (Software Development Academy). A small, self-contained domain — accounts, deposits, withdrawals — used to demonstrate JUnit basics on plain Java classes.

## What it does

Interactive console menu (via `Scanner`):

1. Open one or more bank accounts (account number, type, holder name, balance)
2. Display all account details
3. Search for an account by account number
4. Deposit an amount
5. Withdraw an amount (with insufficient-balance check)

Data lives in memory only — nothing is persisted.

## Tech stack

- Java 8
- Maven
- JUnit 4.13.2

## Structure

```
src/main/java/
├── BankingApp.java    # main class with the console menu loop
└── BankDetails.java   # account domain class (open, show, deposit, withdraw, search)
src/test/java/
└── Testing.java       # JUnit unit test example (balance getter/setter)
```

## Run it

Run the application:

```
mvn compile exec:java -Dexec.mainClass=BankingApp
```

(or run `BankingApp.main()` directly from your IDE)

Run the tests:

```
mvn test
```
