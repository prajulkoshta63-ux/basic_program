# basic_program
# Day 1 (Variables, Data Types, Operators,)
# input two numbers and print their sum
print("/n Enter two numbers to calculate their sum:")
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
sum = num1 + num2
print("Sum:", sum)

# calculate simple interest
print("/n Calculate Simple Interest:")
principal = float(input("Enter principal amount: "))
rate = float(input("Enter rate of interest: "))                                                             
time = float(input("Enter time in years: "))
simple_interest = (principal * rate * time) / 100
print("Simple Interest:", simple_interest)

# Convert Celsius to Fahrenhit
print("/n Convert Celsius to Fahrenheit:")
celsius = float(input("Enter temperature in Celsius: "))
fahrenheit = (celsius * 9/5) + 32
print("Temperature in Fahrenheit:", fahrenheit)

# Write a program to input employee basic salary and calculate HRA(20%)and DA(10%)
print("/n Calculate HRA and DA:")
salary = float(input("Enter employee's basic salary: "))
hra = salary * 0.20
da = salary * 0.10
print("HRA:", hra)
print("DA:", da)

# day 2 ( Conditions)

# Write a program to check whether a number is positive, negative or zero.
print("/n Check whether a number is positive, negative or zero:")
num = float(input("Enter a number: "))

if num > 0:
    print("Positive Number")
elif num < 0:
    print("Negative Number")
else:
    print("Zero")

# Write a program to find the largest among two numbers.
print("/n Find the largest among two numbers:")
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

if a > b:
    print("Largest Number =", a)
else:
    print("Largest Number =", b)


# Write a program to find the largest among three numbers.
print("/n Find the largest among three numbers:")
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))

if a >= b and a >= c:
    print("Largest Number =", a)
elif b >= a and b >= c:
    print("Largest Number =", b)
else:
    print("Largest Number =", c)


# Write a program to check whether a number is even or odd.
print("/n Check whether a number is even or odd:")
num = int(input("Enter a number: "))

if num % 2 == 0:
    print("Even Number")
else:
    print("Odd Number")

# Write a program to check whether a year is leap year or not.
print("/n Check whether a year is leap year or not:")
year = int(input("Enter a year: "))

if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print("Leap Year")
else:
    print("Not a Leap Year")

# day 3 (loops)
# write a program to point number from 1to10
print("/n Print numbers from 1 to 10:")
for i in range(1, 11):
    print(i)

# write a program to print even numbers from 1 to 10
print("/n Print even numbers from 1 to 10:")
for i in range(1, 11):
    if i % 2 == 0:
        print(i)

# write a program to find sum of first n natural numbers
print("/n Find sum of first n natural numbers:")
n = int(input("Enter a number: "))
total = 0
for i in range(1, n + 1):
    total += i
print("Sum of first", n, "natural numbers is:", total)

# write a program to print multiplication table of a number
print("/n Print multiplication table of a number:")
num = int(input("Enter a number: "))
for i in range(1, 11):
    print(num, "x", i, "=", num * i)

# write a program to calculate factorial of a number
print("/n Calculate factorial of a number:")
n = int(input("Enter a number: "))
factorial = 1
for i in range(1, n + 1):
    factorial *= i
print("Factorial of", n, "is:", factorial)
 
#day 4(functions) 
# Write a function to find square of a number.
print("/n Find square of a number:")
def square(num):
    return num * num

n = int(input("Enter a number: "))
print("Square =", square(n))

# Write a function to find maximum of two numbers.
print("/n Find maximum of two numbers:")
def maximum(a, b):
    if a > b:
        return a
    return b

x = int(input("Enter first number: "))
y = int(input("Enter second number: "))
print("Maximum =", maximum(x, y))

# Write a function to calculate simple interest.
print("/n Calculate Simple Interest:")
def simple_interest(p, r, t):
    return (p * r * t) / 100

p = float(input("Enter Principal: "))
r = float(input("Enter Rate: "))
t = float(input("Enter Time: "))

print("Simple Interest =", simple_interest(p, r, t))

# Write a function to check whether a number is even or odd.
print("/n Check whether a number is even or odd:")
def check_even_odd(num):
    if num % 2 == 0:
        return "Even"
    else:
        return "Odd"

n = int(input("Enter a number: "))
print(check_even_odd(n))

# Write a function to calculate area of a circle.
print("/n Calculate area of a circle:")
def area_circle(radius):
    return 3.14 * radius * radius

r = float(input("Enter radius: "))
print("Area =", area_circle(r))

# Write a program to create a list of 10 numbers and print all elements.

print("/n Create a list of 10 numbers and print all elements:")
numbers = [1,2,3,4,5,6,7,8,9,10]

for num in numbers:
    print(num)

# Write a program to find largest element in a list.
print("/n Find largest element in a list:")
numbers = [12, 45, 67, 23, 89, 34]

print("Largest Element =", max(numbers))

# Write a program to count even numbers in a list.

print("/n Count even numbers in a list:")
numbers = [1, 2, 3, 4, 5, 6, 7, 8]

count = 0

for num in numbers:
    if num % 2 == 0:
        count += 1

print("Even Numbers Count =", count)

# Write a program to remove duplicate elements using set.

print("/n Remove duplicate elements using set:")
numbers = [1, 2, 2, 3, 4, 4, 5]

unique_numbers = list(set(numbers))

print("After Removing Duplicates:", unique_numbers)


#10 Mixed Questions

# Write a program to reverse a number.

print("/n Reverse a number:")
num = int(input("Enter a number: "))
reverse = 0

while num > 0:
    digit = num % 10
    reverse = reverse * 10 + digit
    num = num // 10

print("Reversed Number =", reverse)

# Write a program to check whether a number is palindrome.

print("/n Check whether a number is palindrome:")
num = int(input("Enter a number: "))
original = num
reverse = 0

while num > 0:
    digit = num % 10
    reverse = reverse * 10 + digit
    num = num // 10

if original == reverse:
    print("Palindrome Number")
else:
    print("Not a Palindrome Number")

# Write a program to count digits in a number.
print("/n Count digits in a number:")
num = int(input("Enter a number: "))
count = 0

while num > 0:
    count += 1
    num = num // 10

print("Number of Digits =", count)

# Write a program to find sum of digits of a number.
print("/n Find sum of digits of a number:")
num = int(input("Enter a number: "))
total = 0

while num > 0:
    digit = num % 10
    total += digit
    num = num // 10

print("Sum of Digits =", total)

# Write a program to generate Fibonacci series up to N terms.
print("/n Generate Fibonacci series up to N terms:")
n = int(input("Enter number of terms: "))

a, b = 0, 1

for i in range(n):
    print(a, end=" ")
    a, b = b, a + b

# Write a program to check whether a number is prime.
print("/n Check whether a number is prime:")
num = int(input("Enter a number: "))

if num > 1:
    for i in range(2, num):
        if num % i == 0:
            print("Not Prime")
            break
    else:
        print("Prime")
else:
    print("Not Prime")

# Write a program to print all prime numbers between 1 and 50.
print("/n Print all prime numbers between 1 and 50:")
for num in range(2, 51):
    for i in range(2, num):
        if num % i == 0:
            break
    else:
        print(num, end=" ")

# Write a program to count vowels in a string.

print("/n Count vowels in a string:")
text = input("Enter a string: ")

count = 0

for ch in text.lower():
    if ch in "aeiou":
        count += 1

print("Number of Vowels =", count)

# Write a program to reverse a string.

print("/n Reverse a string:")
text = input("Enter a string: ")

print("Reversed String =", text[::-1])

# Write a program to count frequency of each character in a string.

print("/n Count frequency of each character in a string:")  
text = input("Enter a string: ")

freq = {}

for ch in text:
    if ch in freq:
        freq[ch] += 1
    else:
        freq[ch] = 1

print("Character Frequencies:")
for ch in freq:
    print(ch, ":", freq[ch])
