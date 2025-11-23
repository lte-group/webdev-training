# Password Validator

## Exercise Overview

Write a function that checks if a password meets certain criteria (length, special characters, etc.).

## Objectives

- Work with string methods and properties
- Use regular expressions for pattern matching
- Implement multiple validation rules
- Provide user feedback on password strength
- Practice conditional logic

## Key Concepts

- String length (`string.length`)
- Regular expressions
- String methods (`includes()`, `match()`)
- Boolean logic
- Validation rules

## Password Requirements

Common criteria to validate:
1. Minimum length (e.g., 8 characters)
2. At least one uppercase letter
3. At least one lowercase letter
4. At least one number
5. At least one special character (!@#$%^&*, etc.)
6. No spaces

## Tasks

1. Create a function `validatePassword(password)` that checks all criteria
2. Return whether the password is valid and which requirements are met/failed
3. Create a UI with an input field and real-time validation feedback
4. Display which criteria are met with visual indicators (✓ or ✗)

## Tips

- Use `password.length` to check length
- Use regular expressions to check for character types:
  - Uppercase: `/[A-Z]/`
  - Lowercase: `/[a-z]/`
  - Numbers: `/[0-9]/` or `/\d/`
  - Special chars: `/[!@#$%^&*(),.?":{}|<>]/`
- Use `.test()` method with regex: `regex.test(password)`
- Update validation feedback in real-time as the user types
- Use CSS classes to show valid/invalid states

## Example Validation Function

```javascript
function validatePassword(password) {
    const minLength = password.length >= 8;
    const hasUppercase = /[A-Z]/.test(password);
    const hasLowercase = /[a-z]/.test(password);
    const hasNumber = /\d/.test(password);
    const hasSpecialChar = /[!@#$%^&*(),.?":{}|<>]/.test(password);
    
    return {
        valid: minLength && hasUppercase && hasLowercase && hasNumber && hasSpecialChar,
        criteria: {
            minLength,
            hasUppercase,
            hasLowercase,
            hasNumber,
            hasSpecialChar
        }
    };
}
```

## Suggested HTML Structure

```html
<div class="validator-container">
    <input type="password" id="password-input" placeholder="Enter password">
    <ul class="requirements-list">
        <li id="length">At least 8 characters</li>
        <li id="uppercase">At least one uppercase letter</li>
        <li id="lowercase">At least one lowercase letter</li>
        <li id="number">At least one number</li>
        <li id="special">At least one special character</li>
    </ul>
</div>
```

## Extension Challenges

- Add a password strength meter (weak, medium, strong)
- Add a "show/hide password" toggle button
- Check against common weak passwords
- Add a "confirm password" field with matching validation
- Estimate password crack time based on complexity
- Add a password generator button
- Implement a visual progress bar showing password strength
- Add debouncing to validation for better performance
