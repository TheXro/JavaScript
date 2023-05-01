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
console.log('i am ' + 23 + 'year old'//behind the scene due to + operator converted 23 into string
// - will trigger opposite i.e. string will be converted into number
2+4+5+'3' == 113;
// js converets so that the expresion can be executed
console.log('23' - '34' + 34); 
== does type coercion **(its loose equality operator)** and === doesn't type coercion **(strict quality operator)**

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

# Functions

```jsx
//defining function
function logger() {
    console.log('My name is Ravi yadav')
}
//calling or function calling / invoking function
logger()

//functions with arguments
function fruitProcessor(apples, orange) {
    console.log(apples, orange);
    const juice = `juice with ${apples} apples and ${orange} oranges.` ;
    return juice;
}

console.log(fruitProcessor(3,2));
//output
3 2
juice with 3 apples and 55 oranges.

// a function to check prime number
function prime(int) {
    var num = int;
    for (let i = 2; i < num; i++) {
        if (num % i == 0) {
            console.log('not prime');
            break;
        }
        else {
            console.log('prime');
            break;
        }
    }
}
prime(5);
```

# Arrow Function

```jsx
const calcAge = birthYear ==> 2037 - birthYear;

// it doesn't require any return statement 

const yearUntilRetirement = (birthYear , firstName) => {
    const age = 2037 - birthYear;
    const retirement = 65 - age;
    // return retirement;
    return `${firstName} retires in ${retirement} years`
}

```

Recursion is a technique in programming where a function calls itself. In JavaScript, a function can be recursive as well. Below is an example of a recursive function in JavaScript:  

```jsx
function factorial(n) {
  if (n === 0) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}

console.log(factorial(5)); // Output: 120

```

This function calculates the factorial of a given number using recursion. The function checks if the given number is 0. If it is, the function returns 1. Otherwise, it multiplies the given number by the factorial of the number minus 1. This process is repeated until the number is 0.

![Screenshot_86.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_86.png)

# Arrays

lets say you want to store your friends data

you will many variables to store the data

to fix this arrays comes in action

you can store data in a single array 

```jsx
const friend1 = 'ankur';
const friend1 = 'prashant';
const friend1 = 'chahat';

// now using arrays
 const friends = ['ankur','prashant','cahhat'];
console.log(friends);
//another way to create array
const years = new Array(2344,2344,2344,2342);

//getting element from a array
console.log(years[1]);
console.log(years[2]); 
console.log(years[3]);

//the arrays index starts from 0 to n-1 where n is number of elements in array

//retrieving the last element from a array whose index you don't know
console.log(years[years.length-1]);

//mutating the array
//this means thier value (of elements) can be changed but the whole array 
//but const remains constant yes they but only primitive ones
years[2] = 2003; //this is legal
years = [1100 , 1232, 1999, 2003]; this is illegal

//arrays can hold any datatype
var variablename = 'devops';
const array = new Arrays(234,234,324,565,767);
const ravi = ['first year','cse',variablename, 2003, array];

**//array methods** 
const friends = ['michael', 'steven', 'peter'];
//add elements
const newLength = friends.push('jay');
//the .push method adds the element at the end of the array and returns the length of the array after adding the element
console.log(friends);
console.log(newLength);
//output 
Array(4) [ "michael", "steven", "peter", "jay" ]
4  

//adding element at the beginning of the array
friends.unshift('john'); //ushift does it
console.log(friends);
//output
[ "john", "michael", "steven", "peter", "jay" ] //output

//remove elements 
friends.pop(); //last
console.log(friends);
//output  
[ "john", "michael", "steven", "peter" ]

//remove element from the beginning of the array
friends.shift();
console.log(friends);
//output
[ "michael", "steven", "peter" ]

//the indexOf method returns the index of the element in the array
console.log(friends.indexOf('steven'));
//output
1

//the includes method returns true if the element is present in the array and false if the element is not present in the array
console.log(friends.includes('steven'));
//output
true
//the includes method is used to check the presence of the element in the array
if (friends.includes('steven')) {
    console.log('you have a friend called steven');
}
//output
you have a friend called steven

```

# Objects

```jsx
//up until now we have been using arrays to store the data but there is a problem you can't assign name to the elements in the arrays or  we can't use the string as the index of the array

//object literal syntax
const ravi = { 
    firstName: 'ravi',
    lastName: 'yadav',
    age: 2003 - 1999,
    job: 'student',
    friends: ['michael', 'steven', 'peter']
};

//here the firstName, lastName, age, job, friends are the keys of the object and the values are the values of the keys

//we can access the values of the keys using the dot notation
console.log(ravi.lastName);

console.log(ravi['lastName']); //we can also access the values of the keys using the bracket notation

// the difference between the dot notation and the bracket notation is that in the dot notation we can only use the string as the key but in the bracket notation we can use the string as well as the variable as the key

const nameKey = 'Name';
console.log(ravi['first' + nameKey]);
console.log(ravi['last' + nameKey]);

//the above code is used to access the values of the keys which are not present in the object but are created dynamically

const favNum = prompt('what is your favourite number?');
// the prompt method is used to take the input from the user and the input is stored in the form of string  

const value = prompt('what do you want to know?');
console.log(ravi[value]);
//the above code is used to access the values of the keys which are not present in the object but are created dynamically

// to check if the key is present in the object or not we use the in operator
if (value in ravi) {
    console.log(ravi[value]);
}
else {
    alert('wrong request');
}

//adding and deleting  the key value pair
ravi.location = 'india';
ravi['twitter'] = '@_ravi_y';
//the above code is used to add the key value pair to the object
//the delete operator is used to delete the key value pair from the object
delete ravi.location; // it will delete the location key value pair

console.log(`${ravi.firstName} has ${ravi.friends.length} friends and his best friend is  ${ravi.friends[0]}`);
//the above code is used to access the values of the keys which are present in the object and are created dynamically
//the precendence of the operators is same as the precendence of the operators in the mathematics i.e. from left to right so ravi.friends is evaluated first and then the length property is evaluated and then the value of the length property is used to access the element from the array

```

## Object Methods

```jsx
//object methods
const ravi = {
    firstName: 'ravi',
    lastName: 'yadav',
    birthYear: 2003,
    job: 'student',
    friends: ['michael', 'steven', 'peter'],
    hasDriversLicense: true,
    
    calcAge: function (birthYear) {
        return 2024 - birthYear;
    }
    //the above code is used to create the method in the object
    //here we need key value pair but the value is a function so we use the function keyword to create the function and then we assign the function to the key
    //the this keyword is used to access the properties of the object inside the method
};
console.log(ravi.calcAge(2003));

console.log(ravi['calcAge'](2003));//we can also access the method using the bracket notation

// this keyword
const ravi = {
    firstName: 'ravi',
    lastName: 'yadav',
    birthYear: 2003,
    job: 'student',
    friends: ['michael', 'steven', 'peter'],
    hasDriversLicense: true,
    calcAge: function () {
        return 2023 - this.birthYear;
    }
};
console.log(ravi.calcAge()); //this will use the birthYear property of the object ravi to calculate the age

// this keyword here refers to the object ravi and the birthYear is the property of the object ravi so this.birthYear is used to access the birthYear property of the object ravi

now a question arises why not use the ravi.birhYear() 
it will violate the don't repeat yourself priciple 
i.e. if for any reason the name of the object is cahnged then you will need to change the function also so we use this .

const ravi = {
    firstName: 'ravi',
    lastName: 'yadav',
    birthYear: 2003,
    job: 'student',
    friends: ['michael', 'steven', 'peter'],
    hasDriversLicense: true,
    calcAge: function () {
        this.age = 2023 - this.birthYear;    
        return this.age;
    }
};
//the above code is used to add the age property to the object ravi and the value of the age property is calculated using the calcAge method 
console.log(ravi.age); //this will not work as function is not called so no age key is present in the ravi object
console.log(ravi.calcAge()); //function called now age is present
console.log(ravi.age); //this will give the age
```

# loops and iteration

```jsx
//loops are used to repeat the same code multiple times
// there are three types of loops in javascript
// for loop
// while loop
// do while loop

// for loop
for (let rep = 1; rep <= 10; rep++) {
    console.log(`lifting weights repetition ${rep}`);
		console.log(`lifting weights repetition ` + rep);
}
// the above code is used to print the string 10 times
// the for loop is used to repeat the same code multiple times

//continue and break statements
//the continue statement is used to skip the current iteration of the loop and continue with the next iteration of the loop and the break statement is used to break the loop and exit the loop and the loop will not be executed further

console.log('---only strings---');
for (let i = 0; i < ravi.length; i++) {
    if (typeof ravi[i] !== 'string') continue;
    console.log(ravi[i], typeof ravi[i]);
}
//the above code is used to print only the strings in the array ravi

console.log('---break with number---');
for (let i = 0; i < ravi.length; i++) {
    if (typeof ravi[i] === 'number') break;
    console.log(ravi[i], typeof ravi[i]);
}
//the above code is used to print the strings in the array ravi until the number is encountered

//looping backwards and loops in loops
const ravi = [
    'ravi',
    'yadav',
    2024 - 2003,
    'student',
    ['michael', 'steven', 'peter'],
    true
];
for (let i = ravi.length - 1; i >= 0; i--) {
    console.log(i, ravi[i]);
}
//the above code is used to print the array ravi in reverse order

for (let r = 1; r < 5; r++){
    console.log(`exercise ${r}`);
    for (let i = 1; i < 11; i++){
        console.log(`rep ${i} of exercise ${r}`); 
    }
}
// the above code is used to print the repitition of the exercise in the loop

//while loop
//while loops is different from the for loop because the for loop is used to repeat the same code for a fixed number of times but the while loop is used to repeat the same code for an unknown number of times

//for example in a dice game the player will keep rolling the dice until the player gets a 6 on the dice

let dice = Math.trunc(Math.random() * 6) + 1;
console.log(dice);
//here math.random gives a number between 0 and 1 and trunc makes the decimal number into an integer
while (dice !== 6) {
    console.log(`you rolled a ${dice}`)
    dice = Math.trunc(Math.random() * 6) + 1;
    if (dice === 6) {
        console.log("loop ends now");
    }
}
//here we don't know when will six come so we used while

prompt("hey whats up give some value");
prompt takes value as string so alwaus change it to whatever you want to use
```

# Console

```jsx
console.log();
//it logs whatever you want it to 

console.warn();
//it is used for warning

console.error();
//it is used for showing error
```

# selecting html tags

```css
"use-strict";

console.log(document.querySelector('.message'));
// for id we use # instead of .

//html
<p class="message" > hey</p>
```

# DOM: Document Object Model Manipulation

IT is a tree structure of all the elements in the html page

- we can select elements using the document object model
- the dom always start with document object
document object is the root of the dom tree or entry point of the dom tree so document.querySelector() is method in the document object
- first child of the document object is the html element
- second child of the document object is the head elemen
- third child of the document object is the body element
- the body element is the parent of all the elements in
- dom and querySelector are not part of javascript but they are part of the browser api(application programming interface)

## DOM ≠ JavaScript

there are three type you can webpack , parser , other one

depen 

jsx 

taskbased and functionbased

we use root.render(”component you want to add”)

### querySelector vs querySelectorAll

querySelectorAll is used to select all the elements having same class

querySelector only selects the first element of the class

### <name>.classList.add or .remove to remove class from elements

use functions to make code shorter if same code is used over and over

```jsx
const closeModal = function () { 
        console.log('Close button clicked');
        modal.classList.add('hidden');
        overlay.classList.add('hidden');
};
btnCloseModal.addEventListener('click', closeModal);
overlay.addEventListener('click', closeModal);
```

## Listening keyboard event

keydown : when we press the key

keyup : when key comes up after pressing

keypress : when key is bieng pressed

we were listening to functions until now but here we need event object to know which key was pressed the object which stores this is “e” and needs to be set as argument in the function

```jsx
document.addEventListener('keydown', function(e) {
	console.log(e.key); // as e will be object
```

# Working of JavaScript

what is javascript?

> 
> 

![Screenshot_103.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_103.png)

## JS engine

that execute js code e.g. chrome has v8 js engine

every js engine contains call stack adn heap(object in memry)

compilation and interpretation 

js uses Just-in-time (JIT) compilation

![Screenshot_104.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_104.png)

## JIT compilation of JS

![Screenshot_106.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_106.png)

## JS runtime

![Screenshot_107.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_107.png)

---

for node web apis are replaced by c++ bindings and tread pool

## global execution context

top level code will be executed i.e. code that isn’t inside a function 

execution context : environment in which piece of js is executed

exactly one global execution context

after that execution  of functions occurs

one ec per funtion : for each function call , a new ec is created

![Screenshot 2023-05-01 at 22-12-37 How JavaScript Works Behind the Scenes Part-11. The Complete JavaScript Course 2023. - YouTube.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_2023-05-01_at_22-12-37_How_JavaScript_Works_Behind_the_Scenes_Part-11._The_Complete_JavaScript_Course_2023._-_YouTube.png)

## Whats inside a execution context

1. Variable Environment
    1. let, const and var decs
    2. functions
    3. arguments objects
    
     
    
2. Scope chain
3. this keyword

these are generated right before execution : creation phase

ec belonging to arrow functions don’t have this and arguments objects

![Screenshot 2023-05-01 at 22-24-21 How JavaScript Works Behind the Scenes Part-11. The Complete JavaScript Course 2023. - YouTube.png](JavaScript%20f429f6da566249eea324f9de476973df/Screenshot_2023-05-01_at_22-24-21_How_JavaScript_Works_Behind_the_Scenes_Part-11._The_Complete_JavaScript_Course_2023._-_YouTube.png)

# The Call Stack

ec gets stacked on top of each other to keep track of where we are in execution

like a map of js execution

![Untitled](JavaScript%20f429f6da566249eea324f9de476973df/Untitled.png)

![Untitled](JavaScript%20f429f6da566249eea324f9de476973df/Untitled%201.png)

![Untitled](JavaScript%20f429f6da566249eea324f9de476973df/Untitled%202.png)

then 

![Untitled](JavaScript%20f429f6da566249eea324f9de476973df/Untitled%203.png)

# Scoping and Scope

it controls how our program’s variables are organized and accessed.

where do variables live?? 

**lexical scoping : scoping is controlled by placement of functions and blocks in the code**

**Scope** : Space or environment on which a certain variable is declared. There is global, function and block scope.

**Scope of variable** : Region of our code where a certain varibale can be accessed.

## Global Scope

outside and function or block

accessible everywhere

## Function scope

`inside the function

also called local scope 

not accessible outside the function

## Block scope

variables are accessible only inside block 

this only applies to let and const

![Untitled](JavaScript%20f429f6da566249eea324f9de476973df/Untitled%204.png)

## Scope chain

![Untitled](JavaScript%20f429f6da566249eea324f9de476973df/Untitled%205.png)

if also have block scope here `decade = 3` `the scope chain only work upward not sideways` 

![Untitled](JavaScript%20f429f6da566249eea324f9de476973df/Untitled%206.png)

if variable in present in the current scope then it will use that variable

# Hoisting

Makes some type of variables accessible/usable in the code before  they are actually declared 

“variables lifted to the top of their scope”

### behind the scenes

before execution code is scanned for varibale declarations and for each varibale a new property is created in the variable environment object 

However, it is important to note that only the declaration is hoisted, not the initialization. This means that if a variable is declared and initialized later in the code, it will not have a value until the initialization statement is reached.

For example, consider the following code:

```jsx
console.log(x); // Output: undefined
var x = 5;
```

In this example, the variable `x` is declared and initialized later in the code, but the console.log statement outputs undefined because only the declaration of `x` is hoisted to the top of the scope.

It's important to be aware of hoisting when writing JavaScript code, as it can lead to unexpected behavior and bugs if not properly understood.

### Temporal dead zone

Each and every let and const variable get there temporal dead zone

![Untitled](JavaScript%20f429f6da566249eea324f9de476973df/Untitled%207.png)