1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let num =new Array(10);
var sum =0 ,avg=0;
for (let i=0 ;i<num.length ;i++)
{ 
  
  num[i] = +prompt("Enter the number");
  sum = sum+ num[i];
}
console.log(sum);
avg = sum/10;
console.log(avg);
```
2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```//output Error: println is not defined.

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
let sum=0;
function getEvenSum(max)
{
  for (let i=0 ; i<=max ;i++)
  {
     if(i%2 ==0)
     {
       sum = sum +i;
     }
  }
  console.log(sum);
}

getEvenSum(10);
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
let sum=0;
function getOddSum(max)
{
  for (let i=0 ; i<=max ;i++)
  {
     if(i%2 !=0)
     {
       sum = sum +i;
     }
  }
  console.log(sum);
}

getOddSum(10);
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.
```js

function getProductOfDigits(num)
{
  
    let product = 1;
    
    let digits = Number(num);
   
    while (digits > 1)
    {
        product = product * (digits % 10);
        digits = Math.floor(digits / 10);
         console.log(digits);
    }
    console.log(product);
    return product;
}

getProductOfDigits(`123`);
```
- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // output 'Bigger than 5'
check(1); // output   'Smaller than 5' 
check(5); // output    5
```


7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // what will be the output 'You are arya'
getOutput('John'); // what will be the output 'You are John'
getOutput(); // what will be the output  'Who are you';
```
=== is strict comparison so whenever the conditon is satisfied only that o/p will be returned.


8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // what will be the output 'You are arya'
getOutput('John'); // what will be the output 'You are John'
getOutput(); // what will be the output  'Who are you';
```
=== is strict comparison so whenever the conditon is satisfied only that o/p will be returned.

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
No a function can have onnly one return statement, a return statement causes execution to leave the current subroutine .If we need more than one return staments we need to use conditons , at a time only one value can be returned .

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
--
The 'for' loop used only when we already knew the number of iterations.	The 'while' loop used only when the number of iteration are not exactly known.
The 'for loop ' has a initialisation , conditon and iteration ,
while loop just has a condition.