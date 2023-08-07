# Opeartions On Strings

```javascript lineons
    let name = "John";
    let age = 30;

    // String Length
    console.log(myString.length); // Output: 11

    // Accessing Characters As An Array
    console.log(myString[0]); // Output: "H"

    // Substring extracts from specified indexex
    console.log(myString.substring(0, 5)); // Output: "Hello"

    // Substr method extracts a specified number of characters from a string, starting from a specified index
    console.log(myString.substr(6)); // Output: "World"

    // IndexOf method searches for a specified substring within a string and returns the index of the first occurrence of the substring. If the substring is not found, it returns -1.
    console.log(myString.indexOf("World")); // Output: 6

    // LastIndexOf method searches for a specified substring within a string from the end (right to left)
    console.log(myString.lastIndexOf("o")); // Output: 7

    // Trim  method removes leading and trailing whitespace (spaces, tabs, and newlines) from a string
    let trimmedString = "   Hello, World!   ";
    console.log(trimmedString.trim()); // Output: "Hello, World!"

    // Changing Case
    console.log(myString.toUpperCase()); // Output: "HELLO WORLD"
    console.log(myString.toLowerCase()); // Output: "hello world"

    // Replacing method searches for a specified substring in a string and replaces the first occurrence with a new substring
    console.log(myString.replace("World", "Universe")); // Output: "Hello Universe"

    // Split  method is used to split a string into an array of substrings based on a specified separator
    console.log(myString.split(" ")); // Output: ["Hello", "World"]
```
