// Study Guide: JavaScript Concepts

--------------- INTERPOLATING STRINGS -------------------
// Interpolating strings is the process of embedding expressions within a string literal, using the `${}` syntax. 

const name = 'John Doe';
console.log(`Hello, ${name}!`); 
// Output: "Hello, John Doe!"

--------------- RECURSION BASICS -------------------
// Recursion is a technique in programming where a function calls itself in order to solve a problem. 

function factorial(n) {
  if (n === 0) {
    return 1;
  }
  return n * factorial(n - 1);
}
console.log(factorial(5)); 
// Output: 120

--------------- DEFAULT PARAMETERS -------------------
// Default parameters allow function parameters to be set with a default value in case no value or undefined is passed.

function greet(name = 'John Doe') {
  console.log(`Hello, ${name}!`);
}
greet(); 
// Output: "Hello, John Doe!"

--------------- RECURSION VS ITERATION -------------------
// Recursion and iteration are both methods for repeating a process, but recursion uses function calls, while iteration uses loops.

--------------- RECURSION TIPS -------------------
// When using recursion, it is important to have a base case that will stop the recursion and prevent an infinite loop. 

--------------- IDENTIFYING THE BASE & RECURSIVE CASE -------------------
// The base case is the condition in which the recursion stops, while the recursive case is the process by which the function calls itself.

--------------- IMMEDIATELY-INVOKED FUNCTION EXPRESSION OR IIFE -------------------
// An Immediately-Invoked Function Expression (IIFE) is a function that is executed immediately after it is defined. 

(function () {
  console.log('Hello, World!');
})(); 
// Output: "Hello, World!"

--------------- HOISTING -------------------
// Hoisting is the behavior in JavaScript where variable and function declarations are moved to the top of their scope.

console.log(hoistedVar); 
var hoistedVar = 'I am hoisted!';
// Output: undefined

--------------- FALSEY VALUES -------------------
// Falsey values are values in JavaScript that are considered falsy, meaning they evaluate to false in a boolean context.
// Examples: false, 0, '', null, undefined, NaN

if (!0) {
  console.log('0 is falsy');
} 
// Output: "0 is falsy"

--------------- ASYNCHRONOUS -------------------
// Asynchronous is a term used in programming to describe code that runs in the background, independently of the main code.

setTimeout(() => {
  console.log('Hello, World!');
}, 1000); 
// Output (after 1 second): "Hello, World!"

--------------- TIMEOUTS AND INTERVALS -------------------
// Timeouts and intervals are used in JavaScript to schedule a function to be executed after a certain amount of time has passed.

const intervalId = setInterval(() => {
  console.log('Hello, World!');
}, 1000);

setTimeout(() => {
  clearInterval(intervalId);
}, 5000); 
// Output (every 1 second for 5 seconds): "Hello, World!"