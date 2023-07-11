1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

//function expression
let percentage = function(marks,total){
    return (marks * 100) / total;
}

//arrow function
//function expression
let percentage = (marks,total) =>{
    return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}


let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => (marks * 100) / total;
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

because a function is an object and objects are expressions
example 
```js
let percentage = (marks, total) => (marks * 100) / total;
```

4. Why is a function call an expression in JavaScript?
because it can be assigned a value.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // valid because it assigns a variable that excecutes the fuction with fixed parameters
five = add; // valid the expression is simply assigned the function reference so we can view the function
five = five(10, 11); // if five = add then its valid because five becomes function refference so you can add the parameters and excecute the function
five = function () {
  return 'Hello';
}; // valid five is a function expression which stores a function which when called returns thee string hello, it doesnt take any parameters
```

6. What is the difference between function definition and function call? Explain with an example.
function definition is when the is assigned its task whereas function call is when a function is expected to excecute its task

7. What is the similarities between function definition and function call?
they are both different once is used to define a function while the other is used to excecute the function. only similarity would be the use of the function name


8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid hello is a function when called it excecutes the string hello world, whereas hello.user is a expression that is assigned the string value "sam"
```

9. What is higher order function explain with an example.
a function which can be used to excecute anothr function is generally known as a higher order function. it can take a function as an arguemnt or return a function as a result

exaample 
```js
let name = function(naam){
  return "name";
}

let profession = function(prof){
  return "prof"
}

let resume = function(para1 , para2){
  return `My name is ${para1} and i work as a ${para2}`
}



```
10. Explain what is callback function. Why you can pass a function inside a function?
a callback function is a function that can be added as the argument of another function and lets it be excecuted after the execution of the first function.

