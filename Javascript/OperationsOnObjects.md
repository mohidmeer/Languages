# Opeartions On Objects

## Accessing properties

You can access the value of a property using dot notation or square bracket

```javascript lineons
    let person = { name: 'John',age: 30};

    console.log(person.name); // Output: John
    
    console.log(person['age']); // Output: 30

```

## Adding Or Updating Property

You can add or update properties to an object using dot notation or square bracket

```javascript lineons
    let person = { name: 'John', age: 30 };
    
    person.gender = 'Male'; // Adding a new property

    person['age'] = 31; // Updating an existing property

```

## Delete Property

You can delete properties from an object using the delete keyword

```javascript lineons

    let person = { name: 'John', age: 30 };
    delete person.age;

```

## Checking If Property Exists

You can delete properties from an object using the delete keyword

```javascript lineons

    let person = { name: 'John', age: 30 };
    
    console.log('name' in person); // Output: true
    
    onsole.log(person.hasOwnProperty('age')); // Output: true

```

## Looping Through Object properties

You can loop through the properties of an object using for...in loop or Object.keys(), Object.values(), or Object.entries()

```javascript lineons

   let person = { name: 'John', age: 30 };
    for (let key in person) {
        console.log(key, person[key]);
    }
    // Output:
    // name John
    // age 30
    let keys = Object.keys(person);
    console.log(keys); // Output: ['name', 'age']

```

## Cloning or merging objects

You can clone or merge objects using Object.assign() or the spread operator (...)

```javascript lineons

    let person = { name: 'John', age: 30 };

    let clone = Object.assign({}, person); // Cloning

    let additionalData = { gender: 'Male' };
    
    let merged = { ...person, ...additionalData }; // Merging

```

## Checking object type

```javascript lineons
    
    let person = { name: 'John', age: 30 };

    console.log(typeof person === 'object'); // Output: true

```

## Calling methods

```javascript lineons
    
    const person = {
        name: 'John',
        sayHello: function() {
        console.log('Hello, my name is ' + this.name);
        }
    };
person.sayHello(); // Output: Hello, my name is John

```
## Maping Over Array Of Objects And Updating One

``` javascript Lineons

 let comments = [{_id:1,content='this is a comment' },
                 {_id:2,content='this is a comment2' }]
    
    let commentId=1;
    
    let updatedComments= comments.map(comment =>{ 
        if (comment._id===commentId){
            return {...comment , content: 'THIS IS UPDATED COMMENT' };
           }
           return comment
      })

  console.log(updatedComments)
  // Outputs[{_id:1,content='THIS IS UPDATED COMMENT' },  {_id:2,content='this is a comment2' }]
```

## Removing One Item From array Of objects

```javascript lineons
   let comments = [{_id:1,content='this is a comment' },
                  {_id:2,content='this is a comment2' }]

  cosnt NewArray =  comments.filter(c =>c._id !== 1)

  console.log(NewArray)
  //outputs [{_id:2,content='this is a comment2' }]

```