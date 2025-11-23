# FizzBuzz Challenge

## Exercise Overview

Create a program that prints numbers 1-100, but prints "Fizz" for multiples of 3, "Buzz" for multiples of 5, and "FizzBuzz" for multiples of both.

## Objectives

- Use loops to iterate through a range of numbers
- Implement conditional logic with if/else statements
- Understand the modulo operator for checking divisibility
- Practice a classic programming interview question

## Key Concepts

- For loops
- Conditional statements (if/else if/else)
- Modulo operator (%)
- Logical operators (&&)

## Rules

1. Loop through numbers 1 to 100
2. If a number is divisible by both 3 and 5, print "FizzBuzz"
3. If a number is divisible by 3 only, print "Fizz"
4. If a number is divisible by 5 only, print "Buzz"
5. Otherwise, print the number itself

## Tasks

1. Create a for loop that iterates from 1 to 100
2. Use conditional statements to check divisibility
3. Output the appropriate value for each number
4. Test your solution to ensure it works correctly

## Tips

- The modulo operator (%) returns the remainder of division
- `number % 3 === 0` checks if a number is divisible by 3
- Check for "FizzBuzz" (divisible by both) FIRST, before checking for "Fizz" or "Buzz" individually
- Use `console.log()` to output each result

## Expected Output (first 20 lines)

```
1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz
16
17
Fizz
19
Buzz
```

## Extension Challenges

- Display the output on the webpage instead of just the console
- Allow users to input custom range and divisors
- Add styling with different colors for Fizz, Buzz, and FizzBuzz
- Create a more general solution that works with any divisors
- Add a fourth condition (e.g., "Jazz" for multiples of 7)
