# Arrays-Objects-Reference Types
Tags: #Javascript #arrays #objects #referencetypes
Author: Shahid Sharif
Initial Release: 14May2021
Last Update:  14May2021-04:00
Reference: 

---
Arrays & Objects are reference types

## Adding elements to array
```js
const person = {
 name: "Max",
 age: 29,
 greet() {
 console.log('Hi, I am ' + this.name)
 }
};

const hobbies = \['Sports','Cooking'\];
hobbies.push('Programming');
console.log(hobbies);
```



