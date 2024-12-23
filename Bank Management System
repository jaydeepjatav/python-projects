class Account:
    def __init__(self,account_number,account_type,account_balance=0.0):
        self.account_number=account_number
        self.account_type=account_type
        self.account_balance=account_balance
    
    def deposit(self,amount):
        if(amount>0):
            self.account_balance+=amount
            print(f"{amount} credited is account with account number {self.account_number}. Available balance in your account is{self.account_balance}.")
        else:
            print("Please give some valid amount.")

    def withdraw(self,amount):
        if(amount>0 and amount<=self.account_balance):
            self.account_balance-=amount
            print(f"{amount} credited is account with account number {self.account_number}. Available balance in your account is{self.account_balance}.")
        else:
            print("Please give some valid amount.")
            
class Customer:
    def __init__(self,customer_id,customer_name,customer_address):
        self.customer_id=customer_id
        self.customer_name=customer_name
        self.customer_address=customer_address
    
    def openAccount(self,account):
        print(f"Account{account.account_number} is active now")
        
    def closeAccount(self,account_number):
        if(account.account_number==account_number):
            print(f"Account closed for{self.account}.")
            
class Bank:
    def __init__(self,name):
        self.name=name
        self.allCustomers={}
    def add_customers(self,customer):
        self.allCustomers[customer.customer_id]=customer
        print(f"ID:{customer.customer_id} Name:{customer.customer_name} is added successfully to {self.name}.")
    def remove_customers(self,customer_id):
        removed_customer=self.allCustomers.pop(customer_id)
        print(f"ID:{customer_id} Name:{removed_customer.customer_name} is removed successfully from {self.name}.")
    def display_customers(self):
        for customer in self.allCustomers.values():
           print(f"ID:{customer.customer_id},Name:{customer.customer_name},Address:{customer.customer_address}")

if __name__=="__main__":
    bank=Bank("Bank of Baroda")
    
    cust1=Customer("1","Aayushi sharma","Indor,madhya pradesh")
    cust2=Customer("2","jaydeep kumar","mathura,utter pradesh")
    
    bank.add_customers(cust1)
    bank.add_customers(cust2)
    print("")
    bank.display_customers()
    print("")
    
    accnt1=Account(1234,"salary",1000.0)
    accnt2=Account(5678,"saving",1000.0)
    
    cust1.openAccount(accnt1)
    cust2.openAccount(accnt2)
    print("")
    
    accnt1.deposit(500.0)
    accnt2.withdraw(3000.0)
    accnt2.deposit(3000.0)
    print("")
    
    bank.remove_customers("2")
    print("")
    bank.display_customers()
