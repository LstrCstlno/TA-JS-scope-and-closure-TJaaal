Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // output
```
since const is a variable defined inside parennthisis, it isnnt available in the global scope as a result console.log wont have access to username and hense itl get an error. `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output
```
let is blocked scope so its value will remain within parenthisis and console.log doesnt have access to it and it causes it to throw an error

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // Arya
```
var is global scopped so it gets a acess to username and logged "Arya"

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // syntax error username already declared
```
username is already assigned by let so it cannot be reassigned to var

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); // John
```
let cannot be reassigned but it follows block scope so as a result it gets username from the global scope

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); //john
```
let doesnt have funtion scope, jut box scope as a result username will get its info from the memory of the global scope that is jhon

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
since var is global scope within the if loop well get i = 1 - 9 with the string first next to it.
once it exsists the loop we have i = 10 with string second next to it

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // identifier error
}
console.log(i, 'Second'); // output
```
in this case since let is box scope it only works within the loop and well have i = 1 - 9 with first
the console log outside the loop will not have access to the value of i and hence well get a refference error i not defined.
