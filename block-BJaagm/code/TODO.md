1. What does thread of execution means in JavaScript?
the threaad of excecution means the sequence through which a javascript code gets excecuted

2. Where the JavaScript code gets executed?
 in theglobal excecution context

3. What does context means in Global Execution Context?
the entirity or environment of the js code

4. When do you create a global execution context.
when a js code is written

5. Execution context consists of what all things?
memory and exceccution

6. What are the different types of execution context?
global excecution context and function excecution context

7. When global and function execution context gets created?
when a js code is written it gets created in global excecution context and when a function is executed, it is created in a funtion excecution context

8. Function execution gets created during function execution or while declaring a function.
during excecution


9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](/TA-JS-scope-and-closure-TJaaal/block-BJaagm/media/Gec(1).jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](/TA-JS-scope-and-closure-TJaaal/block-BJaagm/media/Gec2.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](/TA-JS-scope-and-closure-TJaaal/block-BJaagm/media/Gec3.jpg)
