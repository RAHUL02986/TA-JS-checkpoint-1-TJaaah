1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let average = 0;
let sum = 0;
for (let i = 1; i <= 10; i++) {
  let num = +prompt(`Enter number`);
  sum = sum + num;

}
average = sum / 10;
console.log(average);
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  printIn('hi');
  i++;
}
print is not defined
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getOddEven(max = 10){
  let evenSum = 0;
  for (let i = 1; i<= max; i++) {
    if(i % 2 === 0) {
      evenSum += i;
    }
  }
   return evenSum;
}
getOddEven(20);//110
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum(max = 10){
  let oddSum = 0;
  for (let i = 1; i<= max; i++) {
    if(i % 2 !== 0) {
      oddSum += i;
    }
  }
   return oddSum;
}
getOddEven(20);//100
```
5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.
```js
function getProductOfDigits(num) {
  let product = 1;
if (num < 0){
  return 'not a valid input';
}else {
  while( num != 0){
  product = product * (num % 10) ;
  num = Math.floor(num / 10);

}
return product;
}
}
```

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

check(10); // 'Bigger than 5'
check(1); // 'smaller than 5'
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'
getOutput('John'); // 'You are John'
getOutput(); // 'Who are you'
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya');// you are arya 'who are you
                   
getOutput('John'); // you are John 'who are you
getOutput(); // 'who are you'

ans-- we will console and if statment and also return that that by both the statment will come when we apply this function
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
ans-- function can't take multipul statments. we will given multipul return statment but system always take first one statment.

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
ans-- Both for loop and while loop is used to execute the statements repeatedly while the program runs. The major difference between for loop and the while loop is that for loop is used when the number of iterations is known, whereas execution is done in the while loop until the statement in the program is proved wrong.

