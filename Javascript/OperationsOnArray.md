# Opeartions On Arrays

```javascript lineons
    let myArray = [1, 2, 3, 4, 5];

    // Accessing Elements
    console.log(myArray[0]); // Output: 1
    console.log(myArray[myArray.length - 1]); // Output: 5

    // Array Length
    console.log(myArray.length); // Output: 5

    // Adding Element To End OF Array
    myArray.push(6);
    console.log(myArray); // Output: [1, 2, 3, 4, 5, 6]

    // Removing Element From End Of Array 
    myArray.pop();
    console.log(myArray); // Output: [1, 2, 3, 4, 5]

    // Adding Element to begning of Array
    myArray.unshift(0);
    console.log(myArray); // Output: [0, 1, 2, 3, 4, 5]

    // Removing Element From  begning of Array
    myArray.shift();
    console.log(myArray); // Output: [1, 2, 3, 4, 5]


    // Concatenation
    let otherArray = [6, 7, 8];
    let combinedArray = myArray.concat(otherArray);
    console.log(combinedArray); // Output: [1, 2, 3, 4, 5, 6, 7, 8]

    // Slice
    let slicedArray = combinedArray.slice(2, 5);
    console.log(slicedArray); // Output: [3, 4, 5]

    //Splice this function takes three arguments StartIndex,Number of items to remove and rest of all is items to replace 
    let removedElements = combinedArray.splice(2, 3, 9, 10);
    console.log(combinedArray); // Output: [1, 2, 9, 10, 6, 7, 8]
    console.log(removedElements); // Output: [3, 4, 5]

    // Another Example Of Splice where we dont remove the elements just add them on specific Index 
    let array = [1, 2, 3, 4, 5];
    let elementsToAdd = [6, 7, 8];
    let removedElements = array.splice(2, 0, ...elementsToAdd); // Inserts elements 6, 7, and 8 at index 2 without removing any elements.
    console.log(array); // Output: [1, 2, 6, 7, 8, 3, 4, 5]
    console.log(removedElements); // Output: []


    // Searching
    //Finding the index of an element
    console.log(combinedArray.indexOf(9)); // Output: 2
    
    console.log(combinedArray.lastIndexOf(10)); // Output: 3


```