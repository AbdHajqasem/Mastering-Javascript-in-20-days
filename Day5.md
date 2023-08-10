#Day5
## Conditionals:
### if statements:
let us execute code under a certain condition:
##### Ex.
```javascript
if(you.wannaBeMyLover){
you.gottaGetWithMyFriends = true;
}
code in the if block only runs if the (condition) is true
```
**we can use 'else' to run other code if (condition) is false**
##### Ex.
```javascript
if (you.reallyBug(me)){
 me.say("Goodbye");
}
else{
  me.say("Hello"); 
}
//--------------------------------------------
if (5 > 4){
 console.log("greater than");
}
 else{
 console.log("less than"); // The output is less than
```
**We can chain else and if blocks to account for multiple conditions**
##### Ex.
```javascript
//x=3,y=2;
function compare(x, y) {
 if (x > y){
 console.log(x, "is greater than", y); // the output is 3 is greater than 2
 }
else if (x < y) {
 console.log(x, "is less than", y);
 }
 else {
 console.log(x, "is equal to", y);
 }
}
```
**If it's given some other value, is will convert it to a boolean and decide based on its "truthiness"** 
##### Ex.
```javascript
if("nonempty strings are truthy"){
console.log("this line will run"); // Because its a non-empty string it will convert it to true, the the output is 'this line will run'
}
//--------------------------------------------
if(0){ //will convert the zero to false
 console.log("zero is truthy");
}
else{
console.log("zero is falsy"); //The output is "zero is falsy"
```
**objects is truthy like if i put an empty array in a an 'if' condition it will converts it to true, but an empty strings is falsy, and 'null' will converts to false,and 'undefined' will converts to false**

### Boolean (logical) operators: 
Sometimes we care about the opposite of a value 
##### Ex.
```javascript
let someoneIsAroundYou = false;
if (!someoneIsAroundYou){
 console.log("baby I love you"); 
} 
//The operator negates a boolean (gives its opposite) 
```
**Sometimes we care about the truthiness of more than one value** 
##### Ex.
```javascript
if(you.happy && you.knowlt){
you.clapHands(); 
}
```
### Logical operators:
1- &&

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/97bdd583-9fbc-4892-beab-e50325f02532)

2-||

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/f87b8415-88d7-4539-949b-9258e5263a67)

---

### Conditional ternary operator :
JS also has a "shortcut" operator for writing quick conditionals

it needs 3 values to work:
##### Ex.
```javascript
condition ? valuelfTrue : valueffFalse;
//--------------------------------------------
let mood = forecast === "sunny" ? : "sad"
//is equivalent to 
let mood;
if (forecast === "sunny") {
 mood = "happy";
else {
 mood = "sad"; 
```
---
## Loops:
Loops let us run the same chunk of code multiple times 
##### Ex.
```javascript
for (let rep = 0; rep < 10; rep += 1){
 console.log("now doing rep", rep); // It will print  "now doing rep", rep '10' times from (0-->9)
}
console.log("do you even lift bro"); // print 'do you even lift bro' one time
//this is called iteration 
```
#### for loops require us to:
• declare & initialize a loop counter

• give a condition for the loop to keep running 

• describe how to change (usually increment) the counter each time 
##### Ex.
```javascript
for (let count = 0; count<= 100;  count += 10){
  console.log(count);
}
```
#### for ... of loops:
let us more easily iterate over items in a collection 
##### Ex.
```javascript
const numbers = [1,2,3]; 
for (let i = 0; i < numbers.length; i++)
console.log(number([i]);
} 
for (let n of numbers){
console.log(n); // The output is 1,2,3
} 
```
**We can use for...of to iterate over characters in a string**
##### Ex.
```javascript
for (let char of "ALOHA") {
console.log(char);//The output is A, L, O, H, A
}
//--------------------------------------------
or items in an array 
for (let item of ["pop", 6, "squish"]{
console.log(typeof item);  // The output is string, number, string
}
```




