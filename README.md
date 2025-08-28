### Name : S Mohamed Ahsan
### Reg No : 212223240089

# Experiment-3 PRIME NUMBER OR NOT

## Aim: 
Write a python program to check the number is prime or not and inspect for failures. 

## Algorithm
1. Start the program.
2. Get the number to be checked from the user.
3. If the number is less than or equal to 1, return "Not Prime".
4. If the number is 2, return "Prime".
5. Start the iteration from 3, For each iteration:
 - If the number is divisible by the current iteration value, return "Not Prime".
6. If the number is not divisible by any value from 2 to the square root, return "Prime".
7. Stop the program. 

## Program
```python
def is_prime(n):
    if n <= 1:
        return False
    if n == 2:
        return True
    for i in range(2, int(n**0.5) + 1, 2):
        if n % i == 0:
            return False
    return True


num = int(input("Enter a number: "))
if is_prime(num):
    print(num, "is a Prime number.")
else:
    print(num, "is NOT a Prime number.")


```
## Output
<img width="541" height="349" alt="image" src="https://github.com/user-attachments/assets/5e312ebe-7b54-4ef3-8af7-1b05a0512a7a" />


## Result

The program to check whether a given number is prime has been successfully executed.
The result correctly identifies if the entered number is prime or not.
