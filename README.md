# CSE412-Lab-1

Loop:

Q1: Write a python program to find the sum of odd and even numbers from a set of numbers.

numbers = []

# number of elements as input
n = int(input("Enter number of elements: "))

# iterating till the range
for i in range(0, n):
    ele = int(input())
    numbers.append(ele)

# initialize sum variables
sum_even = 0
sum_odd = 0

# loop through the list
for num in numbers:
    if num % 2 == 0:
        sum_even += num
    else:
        sum_odd += num

# display the result
print("Numbers:", numbers)
print("Sum of even numbers:", sum_even)
print("Sum of odd numbers:", sum_odd)



Q2: Write a python program to find the smallest number from a set of numbers.

numbers = []

# number of elements as input
n = int(input("Enter number of elements: "))

# iterating to take input of each number
for i in range(n):
    ele = int(input())
    numbers.append(ele)

# find the smallest number
smallest = numbers[0]
for num in numbers:
    if num < smallest:
        smallest = num

# display the result
print("The smallest number is:", smallest)



Q3: Write a python program to generate Fibonacci series.

n = int(input("Enter the number of terms: "))

# first two terms
a, b = 0, 1

# check if the number of terms is valid
if n <= 0:
    print("Please enter a positive integer.")
elif n == 1:
    print("Fibonacci series up to", n, "term:")
    print(a)
else:
    print("Fibonacci series up to", n, "terms:")
    print(a, end=' ')
    print(b, end=' ')
    for i in range(2, n):
        c = a + b
        print(c, end=' ')
        a = b
        b = c

