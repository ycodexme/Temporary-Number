# Temporary-Number
Scrape Numbers and Messages from https://temporary-phone-number.com
## ⚙️Installation
```
pip install temporary-number
```
## 📚Examples
### Get Random Number
Code:
```py
import temporary_number

number = temporary_number.get_number()
print(number)
number2 = temporary_number.get_number(country="Finland")
print(number2)
```
Result:
```
+447893985537
+3584573983862
```
### Get Messages of Number
Code:
```py
import temporary_number

messages = temporary_number.get_messages("+447893985537")
for message in messages:
  print(f"{message.time} | From {message.frm}")
  print(message.content)
```
Result:
