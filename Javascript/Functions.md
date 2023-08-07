# Functions

## Declaring Simple A function

``` javascript lineons
    function add(a, b) {
    
    return a + b;
    
    }
    
     let sum=(add(2,3)) //calling the function

     console.log(sum)
```

## Declaring Arrow function

Arrow functions are a concise way to write functions, introduced in ES6. They have a shorter syntax compared to regular functions,

There is a catch arrow function get executed as soon they are declared but a simple function does'nt executes unless called upon

``` javascript lineons
    const add = (a, b) => {
    
    return a + b;
    
    }

     let sum=(add(2,3)) //calling the function

     console.log(sum)
```

## Declaring Asynchronous functions

Async functions are a type of function that allows you to work with asynchronous operations in a more synchronous style. They are defined using the async keyword before the function declaration. Inside an async function, you can use the await keyword to pause the function execution until an asynchronous operation is complete

We need these functions sometimes our reponse or result is not instant and it can lead to undefined results returned from fuction like when we make a server call it can take some time but function returns the undefined value if we dont use the await keyword in it to stop until we get the response back from server

``` javascript lineons
async function fetchData() {
  const response = await fetch('https://api.example.com/data');
  const data = response.json();
  return data;
}
```

## Asynchronous function (Arrow function)

```javascript lineons

cosnt fetchData = async () => {
  const response = await fetch('https://api.example.com/data');
  const data = response.json();
  return data;
}

```

## Promises

it is a special object used to represent the eventual completion (or failure) of an asynchronous operation and its resulting value.
Promises are a part of the ECMAScript 6 (ES6) standard and are designed to simpliy working with asynchronous code and handling asynchronous operations

### A promise can have three states

- **Pending**: The initial state of a Promise. It is neither fulfilled nor rejected.

- **Fulfilled**: The Promise has successfully completed its operation, and a value is available.

- **Rejected**: The Promise encountered an error or failed to complete its operation, and a reason for the failure is available.
  
### A promise have two methods

- **.then()**  : method to handle the successful resolution of the Promise (when it is fulfilled)
- **.catch()** : method to handle any errors that may occur during the Promise's execution (when it is rejected)

``` javascript lineons 
  const promise = new Promise((resolve, reject) => {
        // Asynchronous operation

        // If the operation is successful, call 'resolve(value)'
        
        // If the operation fails, call 'reject(error)'
    });
```

### Example

``` javascript lineons

      const fetchData = new Promise((resolve, reject) => {
      
      // Simulate an asynchronous operation (e.g., API call)
      
      setTimeout(() => {
        const data = { id: 1, name: 'John Doe' };
        // Resolve the Promise with the data
        resolve(data);
        // Or reject the Promise with an error
        // reject(new Error('Failed to fetch data'));
      }, 2000);
    
    });

    // Using .then() and .catch() to handle the Promise
    fetchData.then(data => {
      console.log('Data fetched successfully:', data);
    }).catch(error => {
      console.error('An error occurred:', error);
    });

```

In this example, the **fetchData** Promise simulates an asynchronous operation using setTimeout and resolves the Promise after a delay of 2000 milliseconds. The .then() method handles the successful resolution of the Promise and the .catch() method handles any errors that may occur during the Promise's execution