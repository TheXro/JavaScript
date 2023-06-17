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

