## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input())

temp = num
rev = 0

while temp > 0:
    rev = (10 * rev) + temp % 10
    temp = temp // 10

if rev == num:
    print("Palindrome")
else:
    print("Not a Palindrome")
```

## Output
<img width="1285" height="494" alt="{D021B9BC-80DC-475B-995A-432B2DF6AC48}" src="https://github.com/user-attachments/assets/19aef5bc-478c-4845-a354-5e183800d04a" />

## Result
The program successfully checks whether the given number is a palindrome by reversing its digits and comparing it with the original number.
