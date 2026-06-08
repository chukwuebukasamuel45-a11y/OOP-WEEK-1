# OOP-WEEK-1
Banye Samuel chukwuebuka 
from bank_account import BankAccount

# Student Information
name = "Banye Samuel Chukwuebuka"
matric_no = "CPE/2023/1039"
department = "Computer Engineering"

print("===== STUDENT DETAILS =====")
print("Name:", name)
print("Matric No:", matric_no)
print("Department:", department)

print("\n===== BANK ACCOUNT TEST =====")

# Create account
account = BankAccount(name, 5000)

print("Initial Account:")
print(account)

# Deposit
account.deposit(2000)
print("\nAfter Depositing ₦2000:")
print(account)

# Withdraw
account.withdraw(1000)
print("\nAfter Withdrawing ₦1000:")
print(account)

# Create account using dictionary
data = {
    "owner": name,
    "balance": 10000
}

account2 = BankAccount.from_dict(data)

print("\nSecond Account Created from Dictionary:")
print(account2)

print("\nRepresentation:")
print(repr(account2))
