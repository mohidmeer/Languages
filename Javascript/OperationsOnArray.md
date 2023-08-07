# Opeartions On Arrays

## Basic Opearions

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
```

## Concatenate Arrays

```javascript lineons
    let otherArray = [6, 7, 8];
    let combinedArray = myArray.concat(otherArray);
    console.log(combinedArray); // Output: [1, 2, 3, 4, 5, 6, 7, 8]
```

## Slice The Array

```javascript lineons
    // Slice
    let slicedArray = combinedArray.slice(2, 5);
    console.log(slicedArray); // Output: [3, 4, 5]
```

## Remove Items From Array

 Splice this function takes three arguments StartIndex,Number of items to remove and rest of all is items to replace 

```javascript lineons
    
    let removedElements = combinedArray.splice(2, 3, 9, 10);
    console.log(combinedArray); // Output: [1, 2, 9, 10, 6, 7, 8]
    console.log(removedElements); // Output: [3, 4, 5]
```

## Add Items To Array At Specific Index

```javascript lineons
   
    let array = [1, 2, 3, 4, 5];
    let elementsToAdd = [6, 7, 8];
    // Inserts elements 6, 7, and 8 at index 2 without removing any elements.
    let removedElements = array.splice(2, 0, ...elementsToAdd); 
    console.log(array); // Output: [1, 2, 6, 7, 8, 3, 4, 5]
    console.log(removedElements); // Output: []
```

## Searching Items in Array

Searching:

- Finding the index of an element: array.indexOf(element)
  - Searches for the last occurrence of 'element' (9) in the array.
- Finding the last index of an element: array.lastIndexOf(element)
  - Searches for the last occurrence of 'element' 10 in the array.

```javascript lineons
    let otherArray = [6, 7, 8];
    let combinedArray = myArray.concat(otherArray);
    console.log(combinedArray.indexOf(9)); // Output: 2
    console.log(combinedArray.lastIndexOf(10)); // Output: 3
```

## Iteration Over Array

- Using loops (for loop, forEach, for...of) to iterate through the array elements.

```javascript lineons

     yourArray.forEach((element) => {
    
        console.log(element); //Logs Every item
    
    });
```

## Map the Array To New Array

- Creating a new array by applying a function to each element: array.map(callback).
  
It is used to create a new array by applying a given function to each element of the original array. The map() function does not modify the original array; instead, it returns a new array with the transformed elements

```javascript lineons

    let mappedArray = combinedArray.map((element) => element * 2);
    
    console.log(mappedArray); 
    
    // Output: [2, 4, 18, 20, 12, 14, 16]
```

## Filtering the array

 It is used to create a new array containing elements that pass a specific test (condition) based on a provided function. The filter() function does not modify the original array; instead, it returns a new array with the elements that meet the given condition

- Creating a new array with elements that pass a test: array.filter(callback)

```javascript lineons

    let filteredArray = combinedArray.filter((element) => element > 5);
    
    console.log(filteredArray); 
    // Output: [9, 10, 6, 7, 8]

    let numbers = [1, 2, 3, 4, 5, 6];
    
    let filteredArray = numbers.filter((element) => element % 2 === 0);
    
    console.log(filteredArray); // Output: [2, 4, 6]
```

## Reducing the array  

The reduce() function iterates through the array and accumulates the result of applying the provided function to each element. It can be used for various operations such as summing up the elements, finding the maximum or minimum value, concatenating strings

- Reducing the array to a single value: array.reduce(callback)

```javascript lineons

   let sum = combinedArray.reduce((accumulator, currentValue) => accumulator currentValue);
   console.log(sum); // Output: 52
```

## Sorting the array

It is used to sort the elements of an array in place and return the sorted array

### Sorting In Asending

```javascript lineons
    let numbers = [10, 2, 33, 45, 5];
    
    numbers.sort();
    
    console.log(numbers); // Output: [2, 5, 10, 33, 45]

    let fruits = ['banana', 'apple', 'orange', 'grape'];
    
    fruits.sort();

    console.log(fruits); // Output: ['apple', 'banana', 'grape', 'orange']
    
```

### Sorting In Desending

```javascript lineons
    let numbers = [10, 2, 33, 45, 5];
    
    numbers.sort((a, b) => b - a);
    
    console.log(numbers); // Output: [45, 33, 10, 5, 2]

    let fruits = ['banana', 'apple', 'orange', 'grape'];
    
    fruits.sort((a, b) => b.localeCompare(a));
    
    console.log(fruits); // Output: ['orange', 'grape', 'banana', 'apple']
    
```

## Checking For Inclusion in Array  

- Checking if an element is in the array: array.includes(element)

```javascript lineons

   console.log(combinedArray.includes(5)); // Output: false

```

## Reversing the Array  

- Checking if an element is in the array: array.includes(element)

```javascript lineons
    let reversedArray = combinedArray.reverse();
    console.log(reversedArray); 
    // Output: [10, 9, 8, 7, 6, 2, 1]
```