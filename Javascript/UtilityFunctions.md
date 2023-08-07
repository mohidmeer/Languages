# Utility Functions

## Math Object

The Math object provides mathematical constants and functions for performing mathematical operations in JavaScript

- Generating a random number between 1 and 10.

```javascript lineons
const randomNumber = Math.floor(Math.random() * 10) + 1;

console.log(randomNumber); 
```

- Calculating the square root of a number.

```javascript lineons
const num = 25;

const squareRoot = Math.sqrt(num);

console.log(squareRoot); // Output: 5
```

## Date Object

The Date object is used for working with dates and times in JavaScrip

- Getting the current date and time.

```javascript lineons
const currentDate = new Date();

console.log(currentDate); // Output: Current date and time
```

- Formatting the date as a string.

```javascript lineons
const date = new Date();

const formattedDate = date.toLocaleString('en-US', { weekday: 'long', year: 

'numeric', month: 'long', day: 'numeric' });

console.log(formattedDate); // Output: E.g., "Sunday, August 7, 2023"
```

## RegEx

The RegExp object represents regular expressions, which are used for matching patterns in strings.

- Using a regular expression to check if a string contains a specific pattern
  
```javascript lineons

const text = 'Hello, World!';

const pattern = /Hello/;

const isMatch = pattern.test(text);

console.log(isMatch); // Output: true

```

- Using regular expression to replace all occurrences of a word

```javascript lineons

const text = 'Hello, World! Hello, Universe! Hello, Everyone!';

const pattern = /Hello/g;

const replacedText = text.replace(pattern, 'Hi');

console.log(replacedText); // Output: "Hi, World! Hi, Universe! Hi, Everyone!"

```

## Error

The Error object represents an error that occurs during the execution of JavaScript code.

- Throwing and handling an error

```javascript lineons

function divide(a, b) {
  if (b === 0) {
    throw new Error('Division by zero is not allowed.');
  }
  return a / b;
}

try {
  const result = divide(10, 0);
  console.log(result); // This line will not execute
} catch (error) {
  console.error(error.message); // Output: "Division by zero is not allowed."
}

```


