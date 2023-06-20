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



# Destructuring Arrays

This section covers the use of destructuring arrays in JavaScript. Destructuring arrays is a way to unpack the values of an array into separate variables. It provides a concise and readable way to extract values from an array.

To destructure an array, simply wrap the variables you want to assign the values to in square brackets `[]`, and assign them to the array you want to destructure. For example:

```jsx
const myArray = [1, 2, 3];
const [a, b, c] = myArray;

console.log(a); // Output: 1
console.log(b); // Output: 2
console.log(c); // Output: 3

```

In the above example, we have an array `myArray` with three values. We then use destructuring to assign each value to a separate variable `a`, `b`, and `c`.

You can also use destructuring to assign default values to variables in case the array does not have enough values to assign to all the variables. For example:

```jsx
const myArray = [1];
const [a, b = 2, c = 3] = myArray;

console.log(a); // Output: 1
console.log(b); // Output: 2
console.log(c); // Output: 3

```

In the above example, we have an array `myArray` with only one value. We use destructuring to assign the first value to `a`, and assign default values of `2` and `3` to `b` and `c` respectively.

Destructuring arrays can be particularly useful when working with functions that return arrays. For example:

```jsx
function returnArray() {
  return [1, 2, 3];
}

const [a, b, c] = returnArray();

console.log(a); // Output: 1
console.log(b); // Output: 2
console.log(c); // Output: 3

```

In the above example, we have a function `returnArray()` that returns an array with three values. We use destructuring to assign each value to a separate variable `a`, `b`, and `c`.

You can also skip the values in a array by just leaving that place blank

```jsx
categories: ['Italian', 'Pizzeria', 'Vegetarian', 'Organic'];

//to skip elements
let [main,/* this is left blank*/, secondary] = categories;
console.log(main, secondary); // Italian Vegetarian
```

To swap the elements using destructuring → Start by creating the inverted array of the variables and assign it to the original array of variables

```jsx
[main, secondary] = [secondary, main];
console.log(main, secondary); // Vegetarian Italian

//receive 2 return values from a function
const [starter, mainCourse] = restaurant.order(2, 0);
console.log(starter, mainCourse);

```

### Nested Destructuring

```jsx
//Just destructure inside the destructuring
//nested destructuring
const nested = [2, 4, [5, 6]];
const [i, , [j, k]] = nested;
console.log(i, j,k); // 2 5 6
```

If you passed an extra variable  then it’s value will be undefined


## The forof Loop: the smart way to loop over an array
It is used to loop over all the values of an iterable object: arrays, strings, maps, sets
It is the modern replacement for the for loop and forEach() method			     

```jsx				     
				     // the smart way to loop over an array
const menu = [...restaurant.mainMenu, ...restaurant.starterMenu];

//the forof loop can be used to loop over the keys of an object 
// for (const item of menu) console.log(item);
// console.log(item); // ReferenceError: item is not defined // item is scoped to the for of loop

//here item is the current element in the loop.
for (const item of menu.entries()) {
  console.log(item);
}

//Output: 
// Array [ 0, "Pizza" ]
// Array [ 1, "Pasta" ]
// Array [ 2, "Risotto" ]
// Array [ 3, "Focaccia" ]
// Array [ 4, "Bruschetta" ]
// Array [ 5, "GarlicBread" ]
// Array [ 6, "Caprese Salad" ]

//as its Output is array we can use this for destructuring 
for (const [i, el] of menu.entries()) {
  console.log(`${i + 1}: ${el}`); 
}//
1: Pizza 
2: Pasta 
3: Risotto 
4: Focaccia 
5: Bruschetta 
6: GarlicBread 
7: Caprese Salad

// console.log([...menu.entries()]);

const fruits = ['🍎','🍌','🍊'];

for (const fruit of fruits) {
console.log(fruit);
}
```
		
	
	 
