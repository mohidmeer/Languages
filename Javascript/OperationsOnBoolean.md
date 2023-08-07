# Opeartions On Booleans

```javascript lineons
    let myBoolean = true;

    // Logical AND (&&)
    console.log(myBoolean && true); // Output: true

    // Logical OR (||)
    console.log(myBoolean || false); // Output: true

    // Logical NOT (!)
    console.log(!myBoolean); // Output: false

    // Comparison Operators
    console.log(myBoolean === true); // Output: true
    console.log(myBoolean !== false); // Output: true
    console.log(myBoolean > false); // Output: true
    console.log(myBoolean >= true); // Output: true
    console.log(myBoolean < false); // Output: false
    console.log(myBoolean <= true); // Output: true

    // Conditional (ternary) Operator
    let result = myBoolean ? "It's true" : "It's false";
    console.log(result); // Output: "It's true"

    // Logical Operators with Other Data Types
    console.log(myBoolean && "Hello"); // Output: "Hello"
    // if myboolean is false then it outputs the second operand
    console.log(myBoolean || "World"); // Output: true

    // Boolean Functions
    let array = [1, 2, 3];
    console.log(array.includes(2)); // Output: true

```