# Temperature Converter

## Exercise Overview

Build a function that converts Celsius to Fahrenheit and vice versa.

## Objectives

- Create functions with parameters and return values
- Understand mathematical operations in JavaScript
- Learn to call functions and use their return values
- Practice working with numbers and calculations

## Key Concepts

- Function declaration
- Parameters and arguments
- Return statements
- Mathematical operators
- Temperature conversion formulas

## Conversion Formulas

- **Celsius to Fahrenheit**: `F = (C × 9/5) + 32`
- **Fahrenheit to Celsius**: `C = (F - 32) × 5/9`

## Tasks

1. Create a function `celsiusToFahrenheit(celsius)` that converts Celsius to Fahrenheit
2. Create a function `fahrenheitToCelsius(fahrenheit)` that converts Fahrenheit to Celsius
3. Test both functions with various temperature values
4. Display results in the console

## Tips

- Use descriptive function names and parameter names
- Remember to use the `return` keyword to return the calculated value
- Test with known values (e.g., 0°C = 32°F, 100°C = 212°F)
- Round results to 1-2 decimal places using `toFixed()` for cleaner output

## Example Usage

```javascript
console.log(celsiusToFahrenheit(0));    // Should output 32
console.log(celsiusToFahrenheit(100));  // Should output 212
console.log(fahrenheitToCelsius(32));   // Should output 0
console.log(fahrenheitToCelsius(212));  // Should output 100
```

## Extension Challenges

- Add input fields and buttons to create an interactive converter UI
- Add conversion to/from Kelvin
- Display the result on the webpage instead of just the console
- Add input validation to ensure only numbers are entered
