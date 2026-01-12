# python-prime-numbers

# Python program to generate prime numbers from 1 to N

# Input the range
num = int(input("Enter the range: "))

print("Prime numbers from 1 to", num, "are:")

# Loop through numbers from 2 to num (1 is not prime)
for n in range(2, num + 1):
    # Check if n is divisible by any number from 2 to sqrt(n)
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            break
    else:
        print(n, end=" ")

OUTPUT:


Enter the range: 20
Prime numbers from 1 to 20 are:
2 3 5 7 11 13 17 19
