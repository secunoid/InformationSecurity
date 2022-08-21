# Arrays And Array Methods
Tags: #Javascript #arrays #array #methods
Author: Shahid Sharif
Initial Release: 14May2021
Last Update:  14May2021-04:00
Reference: 

---
## Array 
Printing values in array
```js
const person = {
 name: "Max",
 age: 29,
 greet() {
 console.log('Hi, I am ' + this.name)
 }
};

const hobbies = ['Sports','Cooking'];
for (let hobby of hobbies) {
 console.log(hobby);
}
```

Using Methods to print array values
```js
const person = {
 name: "Max",
 age: 29,
 greet() {
 console.log('Hi, I am ' + this.name)
 }
};

const hobbies = ['Sports','Cooking'];
console.log(hobbies.map(hobby => 'Hobby: ' + hobby));
console.log(hobbies);
```