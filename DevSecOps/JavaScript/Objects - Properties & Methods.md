# Objects - Properties & Methods
Tags: #Javascript #objects #properties #methods
Author: Shahid Sharif
Initial Release: 14May2021
Last Update:  14May2021-04:00
Reference: 

---

## Objects
Objects allow us to group data together
```js
const person = {
 name: "Max",
 age: 29,
};

console.log(person);

```

## Functions in Objects
Functions can be defined in Objects
```js
const person = {
 name: "Max",
	age: 29,
	greet: () \=> {
	console.log('Hi, I am ' + this.name)
	}
};
person.greet();

```

output is 
```
Hi, I am undefined
```

This is because the keyword *this* refers to global scope of variables and not the variables in this function.

To fix this, you can use the old school functions
```js
const person = {
 name: "Max",
 age: 29,
 greet: function() {
	console.log('Hi, I am ' + this.name)
 }
};

person.greet();
```

further simplify it
```js
const person = {
 name: "Max",
 age: 29,
 greet() {
	console.log('Hi, I am ' + this.name)
 }
};

person.greet();
```