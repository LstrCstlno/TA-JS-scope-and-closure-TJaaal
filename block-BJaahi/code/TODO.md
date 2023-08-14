For the given code below:

- re-write the code in ways that system will understand

For Example:

1.

```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
```

2.

```js
console.log(username, numbers);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js

// declaration phase
var username = undefined;
let number;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

//excecution
console.log(username, numbers);
username = 'Arya';
number = 21;

message = sayHello(username);
nextMessage = sayHello('Test');

//this returns a refference error;
```

3.

```js
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// declaration phase
let username;
let number;
let sayHello;
let message;
let nextMessage;

//excecution

console.log(username, numbers);
username = "Arya";
number = 21;
message = sayHello(username);
nextMessage = sayHello('Test');

```

4.

```js
let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
//declaration
let username;
let number;
let message;
let sayHello;
var nextMessage = undefined;

//excecution
username = "Arya"
console.log(username, numbers);
number = 21;
message = sayHello(username);
sayHello = function (name) {
  return `Hello ${name}`;
};
nextMessage = sayHello('Test');
```

5.

```js
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
```

<!-- Answer -->

```js
//declaration
var name = undefined;
let age;

//excecution
console.log(name);
console.log(age);
name = "Lydia"
age = 21;
```

6.

```js
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

<!-- Answer -->

```js
//declaration
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

//excecution
sayHi();
//declation
var name = undefined;
let age;

//excecution
console.log(name);
console.log(age);
name = 'Lydia';
age = 21;

```

7.

```js
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

<!-- Answer -->

```js
//declaration
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

//excecution
sayHi();

//declaration
var name = undefined;
let age;

//excecution
  console.log(name);
  console.log(age);
  name = 'Lydia';
  age = 21;
```

8.

```js
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
```

<!-- Answer -->

```js
//declaration
let sayHi;

//excecution
//cannot excecute sayHi without declaration
```

9.

```js
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
```

<!-- Answer -->

```js
// declaration
let num1;
var sum = undefined;
let num2;

//excecution
num1 = 21
console.log(sum);//error
sum = num1 + num2;
num2 = 30;
```

10.

```js
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
```

<!-- Answer -->

```js
//declaration
var num1 = undefined;

let sum2;

let add;

function addAgian(a, b) {
  return a + b;
}

let num2;

let sum;

//excecution
num1 = 21;

sum2 = addAgain(num1, num2, 4, 5, 6);


add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};

num2 = 200;

sum = add(num1, num2, 4, 5, 6);

```

11.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
```

<!-- Answer -->

```js
// declaration
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum;
let add;

//excecution
sum = test(100);
//declaration
var a = undefined;
let num;

//excecution
a = 100;
num1 = 21;
add(a, num1)

add = add = (a, b) => {
  return a + b;
};

```

12.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
```

<!-- Answer -->

```js
// declaration
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum;

function add(a, b) {
  return a + b;
}

//excecution
sum = text(100);

//declaration
let a;
let num1;

//excecution
a = 100;
num1 = 21;

add(a, num1)
//declaration none
//excecution
100 + 21

```
