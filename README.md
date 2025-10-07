# CSE412-Lab-1

Loop:

Q: Write a python program to find the sum of odd and even numbers from a set of numbers.

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
