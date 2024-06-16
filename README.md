# Calculate the multiplication of two numbers.
num1 = 20
num2 = 30

print(num1 * num2)
# Print the sum of current number and previous number
previous_num = 0

for i in range(1, 11):
    sum = i + previous_num
    print("Current Num: ", i, "Previous Num: ", previous_num, "Sum will be: ", sum)
    previous_num = i
# Print char at index present at even indexes.
x = input("Enter a charater? ")
print(x)

y = list[x]
#Here, :: means step value that means it will starts from index 0 and then selects every 2nd value or even value.
for i in x[0::2]:
    print(i)
# Removing first n character from a string

