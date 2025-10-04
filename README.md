# comp163-assignment-5

# Challenge 1: Collatz Conjecture Sequence
# I'm using a while loop here because I don't know how many steps it'll take to reach 1.
# The loop will keep going until the current number becomes 1.

current_number = int(input("Enter starting number: "))
step_count = 0

print("Sequence:", end=" ")

while current_number != 1:
    # Print the current number in the sequence
    print(current_number, end=" ")
    if current_number % 2 == 0:  
        # If the number is even, divide it by 2
        current_number = current_number // 2
    else:  
        # If the number is odd, multiply by 3 and add 1
        current_number = 3 * current_number + 1
    # Count how many steps we’ve taken
    step_count += 1

# Finally, print the last number (1) and how many steps it took
print(1)
print("Steps:", step_count + 1)


# Challenge 2: Prime Number Checker
# Here I’m using a for loop because I know the range of possible divisors (from 2 up to the number-1).
# The goal is to test if the number can be divided evenly by anything other than 1 and itself.

number = int(input("Enter a number: "))

print(f"Testing divisors from 2 to {number-1}...")

is_prime = True
for divisor in range(2, number):
    if number % divisor == 0:
        # If the number divides evenly, it’s not prime
        print(f"{number} is not prime (divisible by {divisor})")
        is_prime = False
        break  # no need to check further

# If nothing divided evenly, then the number is prime
if is_prime:
    print(f"{number} is prime!")


# Challenge 3: Multiplication Table Grid
# For this one, I need nested loops: one loop for the rows and another for the columns.
# It will build a full 10x10 multiplication table.

print("Multiplication Table:")

# Print the top row with column labels
print("   ", end="")
for col in range(1, 11):
    print(f"{col:4}", end="")
print()

# Loop through each row
for row in range(1, 11):
    # Print the row label first
    print(f"{row:2}", end="")
    # Then loop through the columns to print the products
    for col in range(1, 11):
        product = row * col
        print(f"{product:4}", end="")
    # Move to the next line after finishing a row
    print()
