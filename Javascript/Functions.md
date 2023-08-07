# Functions

## Declaring Simple A function

``` javascript lineons
    function add(a, b) {
    
    return a + b;
    
    }
```

## Declaring Arrow function

Arrow functions are a concise way to write functions, introduced in ES6. They have a shorter syntax compared to regular functions,

There is a catch arrow function get executed as soon they are declared but a simple function does'nt executes unless called upon

``` javascript lineons
    const add = (a, b) => {
    
    return a + b;
    
    }
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

## Calling A function

``` javascript lineons
    
    let sum=(add(2,3))
     
     console.log(sum)
     
     //outputs 5 
```

