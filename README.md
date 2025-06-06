ATM Project (Java) – Using Encapsulation
📌 Project Overview
This is a simple ATM Simulation System developed in Java that demonstrates Object-Oriented Programming (OOP) concepts, particularly Encapsulation. It allows users to perform basic ATM operations like checking balance, withdrawing cash, and depositing money while ensuring proper data hiding and validation.

🔑 Core Features Implemented
✅ Account Creation with private member variables

✅ PIN-based access (Authentication)

✅ View Balance

✅ Deposit Amount

✅ Withdraw Amount with sufficient balance check

✅ Exit System

🛡️ Error Handling & Robustness
Invalid input (e.g., non-numeric or negative amount) handled using try-catch

PIN verification and restricted access with retry logic

Prevents overdraft withdrawals

Graceful termination and error messages

🔗 Integration of Components
Integrated using Java classes and methods:

ATM class (business logic)

ATMMain class (user interface & main execution)

Modular design for better maintainability

🎯 Event Handling & Processing
User input is taken via Scanner object

Each event (choice: withdraw, deposit, etc.) is handled inside a loop

System responds based on switch-case event processing

✅ Data Validation (5 Marks)
Checks for:

Negative amounts

Non-numeric inputs

Exceeding withdrawal limits

Correct PIN entry only allows access

💡 Code Quality & Innovation
Fully Encapsulated design using:

private variables

public getters/setters

Code follows naming conventions and clean structure

Added retry mechanism for login

Easy to extend (e.g., adding transfer, mini-statement features)

📝 Project Documentation
Classes Used:
ATM – Contains balance, PIN, and methods like withdraw(), deposit(), checkBalance().

ATMMain – Contains the main() method and handles user interaction via console.

Example Structure:
public class ATM {
    private double balance;
    private int pin;

    public ATM(int pin) {
        this.pin = pin;
        this.balance = 1000.0; // default balance
    }

    public boolean verifyPin(int inputPin) {
        return this.pin == inputPin;
    }

    public void deposit(double amount) { ... }

    public void withdraw(double amount) { ... }

    public double getBalance() { ... }
}
🔗 GitHub Repository Structure

ATM-Encapsulation-Java/
│
├── README.md              # Project Overview and Details
├── ATM.java               # Encapsulated ATM class
├── ATMMain.java           # Main class with UI and logic
└── LICENSE                # Optional license info
📂 How to Run
Clone the repo:


git clone https://github.com/your-username/ATM-Encapsulation-Java.git
cd ATM-Encapsulation-Java
Compile and run:

javac ATM.java ATMMain.java
java ATMMain
✅ Output Example
markdown

Enter your PIN: ****
1. Check Balance
2. Deposit
3. Withdraw
4. Exit
Enter your choice: 1
Your Balance is: ₹1000.0
✨ Future Scope
GUI using JavaFX or Swing

Transaction History

Bank-to-Bank Fund Transfers

Admin/User login system
