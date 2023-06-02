# JavaScript

This document provides an introduction to JavaScript, including its use for dynamic effects and web applications in browsers. It covers naming conventions, data types, commenting, variable assignments, operators, and conditional statements. It also includes information on the strict mode, which helps avoid errors in code.

# What is JavaScript

JS is a High level Objected oriented multi paradigm programming language

For dynamic effects and webapplications in the browsers

```java
alert("hello world") //will give a msg
// conditions
let js = 'amazing'
if (js == 'amazing') alert{'JavaScript is FUN!')
```

 

![Screenshot_65.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_65.png)

console.log () ; is needed for code in js as you are not writing code in console

```java
let js="amazing";
console.log(30 + 57-43);
console.log('ravi');
```

## Naming convention

camelcase: hereThisIsUsed

no variable name should start with a number : syntax error

no reserved keyword name 

use underscore and dollar sign 

underscore and dollar sign are the only special characters allowed

use descriptive variables e,g. 

```java
let myFirstJob="programmer";
let myCurrentJob="teacher";
```

don’t use variables with capital letters

## Datatypes

![Screenshot_69.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_69.png)

```jsx
let javaScriptIsFun = true;
console.log(javaScriptIsFun);
```

## ‘typeof’ is used to know what type of datatype is

if a var is declared then its value and type will be undefined

## codeCommenting

// is used for commenting  code

```jsx
// console.log(40-233-234+343);
```

## Assigning variables

let  , var, const are used for variable assignments

const are immutable and they cant be intialized without value

it is preferred to use const

## Operators

```jsx
const now = 2037
const ageJonas = now - 1991;
const ageSarah = now - 2018;
console.log(ageJonas, ageSarah);
console.log(ageJonas * 3, ageJonas / 20, 2**3;
// just use + to add strings
let x = 10 + 7;

// Assignment operators
let x = 10 + 5; // 15
x += 20; // x = x + 20 = 35 
x *= 3; // x = x * 3 = 105
x++; // x = x + 1
x--; // x = x - 1n

// comparision operators
// <, >, >=, <=
    
```

```jsx
console.log(`jus a regular string`);
console.log(`hehe this will 
be formatted in this way
hhh1`);
// using vars 
console.log(`hey im ${firstName}, a ${year} year old ${job});
```

```jsx
// type conversion
const inputYear = '3434';
console.log(Number(inputYear), inputYear)
// 3434 "3434"
console.log(inputYear + 28)
// 343428 

 

// type coercion
// when js does type conversion behind the scenes
console.log('i am ' + 23 + 'year old') //behind the scene due to + operator converted 23 into string
// - will trigger opposite i.e. string will be converted into number
2+4+5+'3' == 113;
// js converets so that the expresion can be executed
console.log('23' - '34' + 34); 
// == does type coercion **(its loose equality operator)** and === doesn't type coercion **(strict quality operator)**
```
## Falsy Values
```jsx 
5 falsy values: 0, '', undefined, null, NaN
// these values becomes false when converted into boolean
if (somethingHere){
	do this
} else {
	do this 
}
// if somethingHere is falsy values then if will not work
// so if a varibale is having 0 as a value the it will give false
// if doesn't require {} if code is only of one line  

```

## AND, OR, NOT OPERATORS

```jsx
&&(and)

||(or)

!(not)
```

# Switch

```jsx

const day = 'friday';
switch (day) {
  case 'monday': // day === 'monday'
    console.log('Plan course structure');
    console.log('Go to coding meetup');
    break;
  case 'tuesday':
    console.log('Prepare theory videos');
    break;
  case 'wednesday':
  case 'thursday':
    console.log('Write code examples');
    break;
  case 'friday':
    console.log('Record videos');
    break;
  case 'saturday':
  case 'sunday':
    console.log('Enjoy the weekend :D');
    break;
  default:
    console.log('Not a valid day!');
}
to give  
console.log(`i'm $(<expression>) years old $(name)`) 
these are not inverted commas

```

# Conditional operator

```jsx
const age= 14;
age >= 18 ? console.log('i like to drink wine '):
console.log('i like water'); 
++
console.log('lol');
const bill = 400;
const tip = bill <=300 && bill >=50 ? bill * 0.15 : bill * 0.2;
console.log(`the bill was ${bill}, the tips was ${tip} and the total value ${bill + tip}`) 
// the ? is used to check the condition and : is used to check the else part of the condition
// here we use the ternary operator which is a short hand of if else statement and it is used when we have only one condition to check

//output 
The bill was 400, the tip was 80, and the total value 480
```

# Strict mode

```jsx
--> 'use strict';
it helps in avoiding  errors
give errors on the console
//strict mode is used to check the error in the code and it is used to write the code in a better way
```

