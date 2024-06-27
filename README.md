1# Calculate the multiplication of two numbers.
num1 = 20
num2 = 30

print(num1 * num2)
2# Print the sum of current number and previous number
previous_num = 0

for i in range(1, 11):
    sum = i + previous_num
    print("Current Num: ", i, "Previous Num: ", previous_num, "Sum will be: ", sum)
    previous_num = i
3# Print char at index present at even indexes.
x = input("Enter a charater? ")
print(x)

#Here, we convert string into list
y = list[x]
#Here, :: means step value that means it will starts from index 0 and then selects every 2nd value or even value.
for i in x[0::2]:
    print(i)
4# Removing first n character from a string
def remove_chars(starter, n):
    #Here, starter indicates the input and [n:] indicates the removal of n
    return starter[n:]

original_string = "Hello There!"
n = 5
new_str = remove_chars(original_string, n)
print(new_str)
5# Checking is first and last index are same then print True othewise False
def first_last(number):
    return number[0] == number[-1]

number_x = [10, 20, 30, 10]
print(first_last(number_x))

number_y = [20, 25, 14, 50]
print(first_last(number_y))
6# Display number divisible by 5 from a list
nums = [10, 58, 45, 69, 20]
print("Number divisible by 5 are: ")
for num in nums:
    if num % 5 == 0:
        print(num)
7# Write a program to find how many times substring “Emma” appears in the given string.
str_x = "Emma is good developer. Emma is a writer"
y = str_x.count("Emma")
print(y)

8# Print the following pattern
for num in range(5):
    for i in range(num):
#Here, end= ensure that num are prited on same line.
        print(num, end=" ")
    print("\n")

9# Write a program to check if the given number is a palindrome number.
def is_palindrome(number):
    print("Original number is: ", number)
    original_number = number

    reverse_num = 0
    while number > 0:
        remainder = number % 10
        reverse_num = (reverse_num * 10) + remainder
        number = number // 10

    if  original_number == reverse_num:
            print("Number is palindrome")
    else:
            print("Number is'nt palindrome.")

answer = int(input("Enter any +ive no?"))
is_palindrome(answer)

10# Given two list of numbers, write a program to create a new list such that the new list should contain odd numbers from the first list and even numbers from the second list.
list1 = [10, 20, 25, 30, 35]
list2 = [40, 45, 60, 75, 90]

final_list = []

for num in list1:
    if num % 2 == 0:
        final_list.append(num)
    
for num in list2:
    if num % 2 != 0:
        final_list.append(num)

print(final_list)
11# Write a Program to extract each digit from an integer in the reverse order.
number = 7489
print(number)
while number > 0:
    digits = number % 10
    
    number = number // 10
    print(digits, end=" ")

12# Calculate income tax for the given income by adhering to the rules: suppose the taxable income is 45000, and the income tax payable is
10000*0% + 10000*10%  + 25000*20% = $6000.

amount = 45000
tax_pay = 0
print("Total amount is: "amount)

# First 10000$ no tax
if amount <= 10000:
    tax_pay = 0
#Next 10000$ pe 10000 deduct and tax is also implemented.
elif amount <= 20000:
    x = amount = 10000
    tax_pay = x * 0.10
#Next remaning$ pe 20000 deduct and tax is also implemented.
else:
    tax_pay += (amount - 20000) * 0.20

print("Total tax is: ", tax_pay)

13# Print multiplication table from 1 to 10

for i in range(1, 11):
    for j in range(1, 11):
        print(i * j, end= " ")
    print("\t")

15#  Write a function called exponent(base, exp) that returns an int value of base raises to the power of exp
def exponent(base, exp):
# Here, ** means base raise to the power of exponent.
    return base ** exp

base = 2
exp = 5
output = exponent(2, 5)
print(f"The result is: {output}")
                                            # Input and Output Excercise #
1# Write a program to accept two numbers from the user and calculate multiplication.
num1 = int(input("Enter first number?"))
num2 = int(input("Enter second number?"))

result = num1 * num2
print(result)

2#  Display three string “Name”, “Is”, “James” as “Name**Is**James”
print(f"Name", "is", "James", sep="**")
