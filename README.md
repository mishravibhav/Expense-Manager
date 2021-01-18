# Expensemanager

Features

- Signup
    - Register with Name, Email & Password
    - If the email already exists show a message “Account already exists”
    - This message must be shown below the register button
    - Validation Rules
        - Name - Min 4 Characters
        - Email - Valid Email
        - Password - Min 6 Characters
    - If the validation fails show the message below the input box
- Login
    - Login with Email & Password
    - If the email doesn’t exists show a message “Account doesn’t exists”
    - If the Email & Password doesn’t match show a message “Wrong Password”
    - This messages must be shown below the login button
- Dashboard
    - Total Income - (Sum of all credit)
    - Total Expenses - (Sum of all debits)
    - Balance - (Credit - Debit)
    - Transaction - (List of last five recent transactions)
    - Enter Transaction
        - Title - (Min 3 Characters)
        - Type - (Credit/Debit - Radio)
        - Amount
        - On submission the details will be stored along with the timestamp
- Ledger
    - Show list of all transaction entries
    - Navigation on the top (All, Credit, Debit)
        - By default All is selected showing all transactions
        - Clicking Credit will show all the credit transactions
        - Clicking Debit will show all the debit transactions

Technical Specs

- Use local-storage to store the data of users and their transactions
- Sample data storage JSON format 
    [
      {
        "name": "Vibhav",
        "email": "mishravibhav1910@gmail.com",
        "password": "123456",
        "transactions": [
          {"title": "Salary", "type": "credit", "amount": 10000, "timestamp": "2020-10-01 09:00"},
          {"title": "Rent", "type": "debit", "amount": 5000, "timestamp": "2020-10-02 09:00"}
        ]
      },
      {
        "name": "Aman",
        "email": "Aman@gmail.com",
        "password": "123456",
        "transactions": [
          {"title": "Salary", "type": "credit", "amount": 10000, "timestamp": "2020-10-01 09:00"},
          {"title": "Rent", "type": "debit", "amount": 5000, "timestamp": "2020-10-02 09:00"}
        ]
      }
    ]
