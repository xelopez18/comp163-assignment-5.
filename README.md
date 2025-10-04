COMP 163: Assignment 5 – Loop Mastery
This repository contains solutions to three programming challenges focused on mastering different loop constructs in Python: while, for, and nested for loops. Each challenge was designed to highlight the strengths of a specific loop type and reinforce algorithmic thinking.

🔁 Loop Design Rationale
Challenge 1: Collatz Sequence – while Loop
Why while? The number of iterations is unknown in advance. The loop continues until the value reaches 1, which depends on the input and cannot be predetermined.

How it works:

Start with a user-provided positive integer.

Repeatedly apply the Collatz rules:

If even → divide by 2

If odd → multiply by 3 and add 1

Print each number in the sequence and count the steps until reaching 1.

Challenge 2: Prime Checker – for Loop
Why for? The range of possible divisors (2 to n-1) is known ahead of time, making a for loop ideal for iterating through a fixed set of values.

How it works:

Accept a positive integer greater than 1.

Loop through all integers from 2 to n-1.

Check if any divide evenly into n using the modulo operator.

If a divisor is found, report that the number is not prime.

If no divisors are found, confirm the number is prime.

Challenge 3: Multiplication Grid – Nested for Loops
Why nested for loops? A multiplication table is a 2D structure. You need one loop to iterate over rows and another to iterate over columns.

How it works:

Print a header row from 1 to 10.

For each row (1 to 10), print the row label.

Inside that, loop through columns (1 to 10) and print the product of row × column.

Use formatted spacing for clean alignment.

🧠 AI Assistance
Used for:

Clarifying loop selection rationale.

Reviewing formatting techniques (e.g., print(f"{product:4}", end="")).

Debugging logic and edge cases.

Optimizing readability and structure of explanations.

Not used for:

Writing core algorithms or solving the challenges directly.

Copy-pasting solutions without understanding.

All code was written independently, with AI used strictly for conceptual guidance and refinement in line with the assignment’s AI usage policy
