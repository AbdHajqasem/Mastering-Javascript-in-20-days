# Learning sprint (1), week (3), day (2) delieverables

### QUESTION #1

Consider the following JavaScript code:

```javascript
let a = 0;
let b = "0";
let c = false;
let d = "false";

console.log(a == b);
console.log(b === c);
console.log(!!d);
```

What will be the output of each console.log statement? **_You MUST explain WHY_**.

1- true(Because == just compare the values and does not compare the data type and its convert the string to number)

2- false(The === operator performs a comparison between both the value and the data type of the operands without any type coercion)

3- true(Because the (d) is a string and when i use (!) it convert the string to boolean and a non-empty string is true in boolean so the first (!) make it false and the second return it to true)

-------------------------------------------------------------------

### QUESTION #2:


Consider the following JavaScript expression:

```javascript
console.log(4 + 5 * "7");
```

What will be the output of this expression? **_You MUST explain the steps of evaluation taken by JS_**.

39(when you try to perform an operation between a number and a string,the Java-Script convert the string to number so the string  "7" become a number, and the priority in arithmetic operation for multiply )

-------------------------------------------------------------------

### QUESTION #3:

Evaluate the following expression:

```javascript
let result = 5 + 2 * 3 - 1;
```

What will be the output of this expression? **_You MUST explain the steps of evaluation taken by JS_**.

10

-------------------------------------------------------------------

### QUESTION #4:

Consider the following code:

```javascript
let x = 10;
let y = '10';
console.log(x == y);
console.log(x === y);
```
What will be the output of each `console.log` statement? **_You MUST explain WHY_**.

1-true (Because == just compare the values and does not compare the data type and its convert the string to number) 

2-false(The === operator performs a comparison between both the value and the data type of the operands without any type coercion)

-------------------------------------------------------------------

### QUESTION #5:

Given the code below:

```javascript
let num = "15";
let isPositive = true;
let result = (num > 10 && isPositive) || num < 0;
console.log(result);
```

What is the value of result? **_You MUST explain the steps of evaluation taken by JS_**

true(Because the comparison operations convert the data type to boolean so the num is string and a non-empty string will converts to true and isPositive is already a boolean and its true and when we use && the result is true if the two sides is true then the final answer from the && is true and if the first side of the || is true the result of it is true so the final result is **true** )
