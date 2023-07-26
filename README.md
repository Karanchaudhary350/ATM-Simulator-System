# ATM Simulator System

The ATM Simulator System is a Java-based project that simulates an ATM machine. It includes various functionalities like balance inquiry, deposit, fast cash withdrawal, mini statement, and more. The system uses Java for its core logic, GUI and windows builder for the user interface, and MySQL for database management.

## Features

The ATM Simulator System offers the following features:

1. Login: Users can log in using their credentials to access their account.
2. Balance Inquiry: Users can check their account balance.
3. Deposit: Users can deposit money into their account.
4. Fast Cash: Provides predefined amounts for quick withdrawals.
5. Mini Statement: Displays a mini statement of recent transactions.
6. PIN Management: Allows users to change their PIN for added security.
7. Signup: New users can create an account by signing up.

## Requirements

To run the ATM Simulator System, you need the following:

1. Java Development Kit (JDK): To compile and run the Java code.
2. Eclipse or any Java IDE: To open and manage the project files.
3. MySQL Database: To store user account information and transaction history.
4. Windows Builder Plugin: To design and create the GUI interface.

## Installation and Setup

Follow these steps to set up and run the ATM Simulator System:

1. **Clone or download the project files from the repository.**

2. **Set up the MySQL database:**
   - Install MySQL on your machine if you haven't already.
   - Create a new database and name it "atm_simulator_db" (you can choose a different name if you prefer).
   - Create two tables: "users" and "transactions" using the provided schema.

   ```sql
   CREATE TABLE users (
     id INT AUTO_INCREMENT PRIMARY KEY,
     account_number VARCHAR(10) NOT NULL,
     pin VARCHAR(4) NOT NULL,
     name VARCHAR(50) NOT NULL,
     balance DOUBLE NOT NULL
   );

   CREATE TABLE transactions (
     id INT AUTO_INCREMENT PRIMARY KEY,
     account_number VARCHAR(10) NOT NULL,
     transaction_type VARCHAR(20) NOT NULL,
     amount DOUBLE NOT NULL,
     transaction_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );
3. Import the project into your Java IDE (e.g., Eclipse).
4. Install and configure the Windows Builder plugin to edit the GUI components.
5. Update the `Conn.java` file with the correct database connection settings (e.g., database URL, username, password).
6. Compile and run the `Login.java` file to launch the ATM Simulator System.

## Usage

1. Launch the ATM Simulator System by running the `Login.java` file.
2. If you are an existing user, enter your account number and PIN to log in.
3. If you are a new user, click on the "Sign Up" button to create an account.
4. After logging in, you will be presented with various options on the ATM interface.
5. Choose the desired option (e.g., Balance Inquiry, Deposit, Withdrawal) by clicking on the corresponding button.
6. Follow the on-screen instructions to complete the transaction.
7. For security reasons, ensure to log out after finishing your transactions.

 ## Contribution

Contributions to the ATM Simulator System project are welcome. If you find any bugs or want to add new features, feel free to fork the repository and submit a pull request.


## Acknowledgments

Special thanks to all contributors and developers who have helped build and improve the ATM Simulator System.

## Contributors
<table>
<tr>
    <td align="center">
        <a href="https://github.com/Adityasinghsiddhartha">
            <img src="https://avatars.githubusercontent.com/u/106505506?v=4" width="100;" alt="akhilmhdh"/>
            <br />
            <sub><b>Aditya .</b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/kaushik0703">
            <img src="https://avatars.githubusercontent.com/u/106008167?v=4" width="100;" alt="akhilmhdh"/>
            <br />
            <sub><b>Kaushik Moralwar</b></sub>
        </a>
    </td>
     <td align="center">
        <a href="https://github.com/Karanchaudhary350">
            <img src="https://avatars.githubusercontent.com/u/78443850?v=4" width="100;" alt="shufo"/>
            <br />
            <sub><b>Karan Chaudhary</b></sub>
        </a>
    </td></tr>
</table>
readme: contributors -end -->

