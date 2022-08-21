# Spread Operator And Rest Parameters
Tags: 
Author: Shahid Sharif
Initial Release: 14May2021
Last Update:  14May2021-04:00
Reference: 

---
Immutability, do not update the original array, add new elements to a copy of the array

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

## Slice() to make a copy of the array
```js
const person = {
 name: "Max",
 age: 29,
 greet() {
 console.log('Hi, I am ' + this.name)
 }
};

const hobbies = ['Sports','Cooking'\];
const copiedArray = hobbies.slice();
console.log(copiedArray);
```

## Spread(...) operator to pull objects from an array
```js
const person = {
 name: "Max",
 age: 29,
 greet() {
 console.log('Hi, I am ' + this.name)
 }
};

const hobbies = ['Sports','Cooking'\];

const copiedArray = [...hobbies];
console.log(copiedArray);
```

## Rest(...) operator to merge multiple arguments to an array
```js
const person = {
 name: "Max",
 age: 29,
 greet() {
 console.log('Hi, I am ' + this.name)
 }
};

const copiedPerson = { ...person };
console.log(copiedPerson);

const hobbies = ['Sports','Cooking'\];

const copiedArray = [...hobbies];
console.log(copiedArray);

const toArray = (...args) => {
	return args;
};

console.log(toArray(1,2,3,4));
```