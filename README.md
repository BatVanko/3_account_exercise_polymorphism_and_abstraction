# 3_account_exercise_polymorphism_and_abstraction
Create a single class called Account. Upon initialization, it should receive an owner (str) and a starting amount (int, optional, 0 by default). It should also have an attribute called _transactions (empty list). Create the following methods:
•	add_transaction(amount) - if the amount is not an integer, raise ValueError with the message "please use int for amount". Otherwise, add the amount to the transactions
•	balance() - a property that returns the sum between the amount and all the transactions
•	validate_transaction(account: Account, amount_to_add)
o	If the balance becomes less than zero, raise ValueError with the message "sorry cannot go in debt!" and break the transaction. 
o	Otherwise, complete it and return a message "New balance: {account_balance}"
Implement the correct magic methods so the code in the example below works properly:
•	When you print an account instance, the output should be in the format "Account of {owner} with starting amount: {amount}".
•	When you print a representational string of an account instance, the output should be in the format "Account({owner}, {amount})".
•	When you access the length of an account instance, you should receive the total number of transactions made.
•	You should iterate over an account instance and receive each transaction as a result.
•	You should be able to reverse the order of transactions by reversing an account instance.
•	You should be able to compare (>, <, >=, <=, ==, !=) two account instances by their balance amount.
•	When you concatenate two accounts, you should return a new account with a name - string in the format "{first_owner}&{second_owner}" and starting amount - the sum between their two. Both their transactions should be added to the new account.
