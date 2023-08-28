## Instance vs Interface
### broaden the further version of instance
as illustrated in the previous one
Python use the abstract and robust class instace or method to reuse the function
Interface refer to the function balanced the abstract and robust feature
In cs61A, there is an example that 
```python
def deposit_all(winners, amount=5):
        for account in winners:
            account.deposit(amount)
```
> **vs**
```python
def deposit_all(winners, amount=5):
        for account in winners:
            account.deposit(account,amount)
```
as you can see the second one is limit to the account instance such that not universal to all class
