# Conditional Statements

## if statement

The if statement allows you to execute a block of code if a certain condition is true.

``` javascript lineons
   
    if (condition) {
    // code to be executed if the condition is true
    } else {
    // code to be executed if the condition is false
    }

```

## else if statement

The else if statement allows you to check multiple conditions in sequence. It is used when you have more than two possible outcomes.
Syntax:

``` javascript lineons

if (condition1) {
  // code to be executed if condition1 is true
} else if (condition2) {
  // code to be executed if condition2 is true
} else {
  // code to be executed if none of the conditions are true
}


```

## switch statement

The switch statement provides a way to select one of many code blocks to be executed based on the value of an expression. It is often used when there are multiple possible cases.

``` javascript lineons
    switch (expression) {
        case value1:
            // code to be executed if expression matches value1
            break;
        case value2:
            // code to be executed if expression matches value2
            break;
        default:
        // code to be executed if expression does not match any case
    }

```

These conditional statements allow you to control the flow of your program based on certain conditions, making your code more flexible and capable of handling different scenarios

## Conditions Possible Values Inside If(condition)

Truthy values are any values that are considered "true" when evaluated in a boolean context. Falsy values, on the other hand, are values that are considered "false" in a boolean context. In JavaScript, the following values are considered falsy:

``` javascript lineons
let condition = false ;

let condition = null  ;

let condition =  undefined;

let condition = 0;

let condition = NaN

let condtion = ""
 
```

In JavaScript, the following values are considered Truthy:

``` javascript lineons
let condition = true ;

let condition = 'AnyStringOtherThanEmpty'  ;

let condition =  {} ;

let condition = [];

let condition = 1

let condtion =  2.1  //Any number other than zero 

let condtion = -2.1  

```

## Examples For If Statements

### Truthy Values

```javascript lineons
    if ("hello") {
    console.log("This is truthy"); // Output: This is truthy
    }

    if (42) {
    console.log("This is truthy"); // Output: This is truthy
    }

    if ({}) {
    console.log("This is truthy"); // Output: This is truthy
    }

    if (new Date()) {
    console.log("This is truthy"); // Output: This is truthy
    }

    if (function() {}) {
    console.log("This is truthy"); // Output: This is truthy
    }
```

### False Value

```javascript lineons
   if (false) {
    console.log("This is falsy"); // Not executed
    }

    if (0) {
    console.log("This is falsy"); // Not executed
    }

    if ("") {
    console.log("This is falsy"); // Not executed
    }

    if (null) {
    console.log("This is falsy"); // Not executed
    }

    if (undefined) {
    console.log("This is falsy"); // Not executed
    }

    if (NaN) {
    console.log("This is falsy"); // Not executed
    }
```

## Examples For Switch Statement

```javascript lineons

let dayOfWeek = 2;
let dayName;

switch (dayOfWeek) {
  case 1:
    dayName = "Sunday";
    break;
  case 2:
    dayName = "Monday";
    break;
  case 3:
    dayName = "Tuesday";
    break;
  case 4:
    dayName = "Wednesday";
    break;
  case 5:
    dayName = "Thursday";
    break;
  case 6:
    dayName = "Friday";
    break;
  case 7:
    dayName = "Saturday";
    break;
  default:
    dayName = "Invalid day";
}

console.log(dayName); // Output: Monday
```

