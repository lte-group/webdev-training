# Basic Calculator

## Exercise Overview

Write functions to add, subtract, multiply, and divide two numbers.

## Objectives

- Create multiple functions that perform mathematical operations
- Work with function parameters
- Practice returning values from functions
- Handle edge cases (like division by zero)

## Key Concepts

- Function declaration
- Multiple parameters
- Return statements
- Arithmetic operators (+, -, *, /)
- Error handling

## Tasks

1. Create an `add(a, b)` function that returns the sum of two numbers
2. Create a `subtract(a, b)` function that returns the difference
3. Create a `multiply(a, b)` function that returns the product
4. Create a `divide(a, b)` function that returns the quotient
5. Test all functions with various number pairs
6. Handle division by zero appropriately

## Tips

- Keep functions simple and focused on one task
- Use meaningful parameter names
- Test with positive numbers, negative numbers, and decimals
- For division, check if the divisor is zero before dividing
- Consider rounding results to a reasonable number of decimal places

## Example Usage

```javascript
console.log(add(5, 3));        // Should output 8
console.log(subtract(10, 4));  // Should output 6
console.log(multiply(6, 7));   // Should output 42
console.log(divide(20, 5));    // Should output 4
console.log(divide(10, 0));    // Should handle error
```

## Extension Challenges

- Create a UI with input fields and buttons for each operation
- Add additional operations (modulo, exponentiation, square root)
- Create a more advanced calculator with operator precedence
- Add a calculation history feature
- Implement keyboard support for number entry
- Style the calculator to look like a real calculator
