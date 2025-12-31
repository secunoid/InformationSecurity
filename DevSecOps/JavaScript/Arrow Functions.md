# Arrow Functions
Tags: #Javascript ; #functions; #arrowfunctions 
Author: Shahid Sharif
Initial Release: 14May2021
Last Update:  14May2021-04:00
Reference: 

---
All functions below are the same, just different implementations

## Normal Function
```js
function summarizeUser(userName, userAge, userHasHobby) {
 return (
 	"Name is " +
 	userName +
 	", age is " +
 	userAge +
 	" and the user has hobbies: " +
 	userHasHobby
 	);
}
```

## Anonymous Function
```js
const summarizeUser = function (userName, userAge, userHasHobby) {
 return (
 	"Name is " +
 	userName +
 	", age is " +
 	userAge +
 	" and the user has hobbies: " +
 	userHasHobby
 	);
}
```

## Arrow Function
```js
const summarizeUser =  (userName, userAge, userHasHobby) => {
 return (
 	"Name is " +
	 userName +
	", age is " +
 	userAge +
	" and the user has hobbies: " +
	userHasHobby
 );
}
```

---
## Arrow Function with only one statement
```js
const add = (a, b) => {
 return a + b;
};
```

## Same arrow function simplified
```js
const add = (a, b) => a + b;
```

---
## Arrow function with one variable
```js
const addOne = (a) => a + 1;
```

## Same arrow function simplified
```js
const addOne = a => a + 1;
```

---
## Arrow functions with no variables
```js
const addRandom = () => 1 + 2;
```