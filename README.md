# Atm-interface-
Atm interface
 
Source code for ATM interface using python  
Import time 
 
Print(“Please insert Your CARD”) 
 
# for card processing 
Time.sleep(5) 
 
Password = 2005 
Pin = int(input(“Enter your ATM PIN: “)) 
Balance = 50000 
 
If pin == password: 
    While True: 
        Print(“”” 
1	== Balance 
2	== Withdraw balance 
3	== Deposit balance 
4	== Exit 
 	 	 	“””) 
        Try: 
            Option = int(input(“Please enter your choice: “))         Except ValueError: 
            Print(“Please enter a valid option”) 
            Continue 
         
        If option == 1: 
            Print(f”Your current balance is {balance}”) 
             
        Elif option == 2: 
            Withdraw_amount = int(input(“Please enter withdraw amount: “))             If withdraw_amount > balance: 
                Print(“Insufficient balance”) 
            Else: 
                Balance -= withdraw_amount 
                Print(f”{withdraw_amount} is debited from your account”) 
                Print(f”Your updated balance is {balance}”) 
                 
        Elif option == 3: 
            Deposit_amount = int(input(“Please enter deposit amount: “)) 
            Balance += deposit_amount 
            Print(f”{deposit_amount} is credited to your account”) 
            Print(f”Your updated balance is {balance}”) 
             
        Elif option == 4: 
            Break         Else: 
            Print(“Invalid option. Please try again.”)
 Else: 
    Print(“Wrong PIN. Please try again.”) 
 
 
 
