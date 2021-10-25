1. Using loops take 10 inputs from user and find the average of all the numbers.

```js
let sum = 0;
for (let i = 1; i <= 10; i++) {
  num = +prompt(`Please enter the number`);
  sum = sum + num;
}
console.log(sum / 10);
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println("hi");
  i++;
}
///'hi'
///'hi'
///'hi'
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum(max = 10) {
  let sum = 0;
  for (let i = 1; i <= max; i++) {
    if (i % 2 == 0) {
      sum += i;
    }
  }
  return sum;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
function getOddSum(max = 10) {
  let sum = 0;
  for (let i = 1; i <= max; i++) {
    if (i % 2 !== 0) {
      sum += i;
    }
  }
  return sum;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

```js
function sumOrProductOfN(num, operation) {
  if (operation === "product") {
    let product = 1;
    for (let i = 1; i <= num; i++) {
      product *= i;
    }
    return product;
  } else {
    alert("Not a valid Input");
  }
}
```

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return "Bigger than 5";
  }

  if (num < 5) {
    return "Smaller than 5";
  }

  return num;
}

check(10); // Bigger than 5
check(1); // Smaller than 5
check(5); // 5
```

///In each case it is having return keyword which will make our program to terminate and return the value.

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}

getOutput("Arya"); // You are arya
getOutput("John"); // You are john
getOutput(); // Who are you
```

///In each case it is having return keyword which will make our program to terminate and return the value.

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") console.log("You are arya");
  if (name === "John") console.log("You are john");
  return "Who are you";
}

getOutput("Arya"); // You are arya and 'Who are you' will be returned
getOutput("John"); // You are John and 'Who are you' will be returned
getOutput(); // Who are you here we are having console.log which will print the message in screen and also having one return so it give output 'who are you'.
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

```js
function sum(a, b) {
  return a + b;
  return a - b;
}
sum(12, 5);
```

Yes function have multiple return statement but you can only return one output from the function you cannot return more than one output from the fnction

If we tried to return two times in a function the function will return only first return

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

Difference between for loop and while loop is that

while loop has only one input condtion

for loop has input conditions

Both has one breaking condtions.

Example -
Display the number from 0 to 4 using for loop?

```js
for (let i = 0; i < 5; i = i + 1)
 console.log(i);
```

Example -
Display the even numbers between 0 to 10

```js
let i=0
while(i<10){
  if (i%2 === 0){
    console.log (i)
  }
  i= i+1
}
```