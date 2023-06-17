
# loops and iteration


loops are used to repeat the same code multiple times

there are three types of loops in javascript
- for loop
- while loop
- do while loop
```jsx
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
