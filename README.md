# Python-Codes
#### Here are Some Helpful Python Codes :


1. Python Password Generator - [Click Me](https://github.com/AmmError/Python-Codes/blob/main/PassGen/main.py)

Code Preview Here (Without Comments):
```
import secrets
import string

letters = string.ascii_letters
digits = string.digits
special_chars = string.punctuation

alphabet = letters + digits + special_chars

pwd_length = 12 # Change This to increase/decrese the length of the password

pwd = ''
for i in range(pwd_length):
  pwd += ''.join(secrets.choice(alphabet))

print(pwd)

while True:
  pwd = ''
  for i in range(pwd_length):
    pwd += ''.join(secrets.choice(alphabet))

  if (any(char in special_chars for char in pwd) and 
      sum(char in digits for char in pwd)>=2):
          break
print(pwd)```
