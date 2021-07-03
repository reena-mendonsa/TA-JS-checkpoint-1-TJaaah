1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
-- The first function returns the sum value of a ,b . So when we call the function sum the return value of the sum of two numbers can be saved in a varaible and used in the code .
The second function does not return a value but displays the sum  in the console .So the output of the function here will be undefined.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

first will have the sum of a & b;
second will be undefined.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
sum of first two parameters . ie 12+24 = 36 ;
You can call a Javascript function with any number of parameters, regardless of the function's definition.
Any named parameters that weren't passed will be undefined.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
yes ..because the function is returning the sum value;

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

function sayHello(name)
{
  return `Hello ${name}`;
}

let name = sayHello(Arya);

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1 'John'

showMessage(); // Output 2 'Hello John'

alert(userName); // Output 3 'john'
```

8. What is a Anonymous Function give example of three functions.
An anonymous function is a function without a name. 
let show = function () {
    console.log('Anonymous function');
};

show();

9. Can function declaration be a Anonymous Function? Explain
The main difference between a function expression and a function declaration is the function name, which can be omitted in function expressions to create anonymous functions. 

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.
getFullName(firstName, secondName);
calculateBmi(height,weight);
createShoppingCart();
checkStatus(status);



```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```

