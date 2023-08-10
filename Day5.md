# Day5
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
## Map & Filter:
### 1-Map:
The map & filter methods also let us process all the items in an array.

map calls a function on each item in an array to create a new array. 
##### Ex.
```javascript
const spices = [
 {name: "Emma", nickname: "Baby"},
 {name: "Geri", nickname: "Ginger"},
 {name: "Mel B", nickname: "Scary"},
 {name: "Mel C", nickname: "Sporty"},
 {name: "Victoria", nickname: "Posh"}
]; 
const nicknames = spices.map(s => s.nickname + " Spice"); 
//Arrow functions are useful for this! 
```
#### Another way to write a String:
String templates are useful too! Make them with backticks and '$ {}', 

'string to insert ${variable} into' 
##### Ex.
```javascript
s => `${s.nickname} Spice'; // In the brackets we can write a javaacript code like 1+2
is equivalent to 
s => s.nickname + " Spice"
```
---
### 2-Filter:
filter calls a true/false function on each item 

and creates a new array with only the items where the function returns true. 

##### Ex.
```javascript
const mels = spices.filter(s => s.name.includes ("mel")); 
```
## Spread(...):
We can use it to put all the items from one array inside another array.
##### Ex.
```javascript
const oldBurns= [("square", "wick")];
const newBurns= [("basic", "dusty", "sus")];
const burnBook [...oldBurns, ...newBurns); 
//equivalent to 
const burnBook = oldBurns.concat(newBurns); 
```
We can also use it to pass all the items from an array as arguments to a function or method.
##### Ex.
```javascript
 const skills = ["HTML", "CSS", "JS")];
 const newSkills = ["React", "TypeScript", "Node")];
 skills.push(...newSkills);
 console.log(...skills);// The output will be HTML CSS JS React  TypeScript Node
```
---
## While loops:
while loops let us run a chunk of code over & over if a (condition) is true.
##### Ex.
```javascript
let fiveRandomNumbers = [];
 while (fiveRandomNumbers.length < 5) {
 fiveRandomNumbers.push(Math.random());
}
```
## (A) synchronous code:
**JS can usually run straight through our program "synchronously"** 

**JS can only do one task at a time ("single-threaded")** 
So when we give JS a task that takes a while, it doesn't stop and wait
##### Ex.
```javascript
console.log("This will print first");
setTimeout(() =>console.log("This will print third"), 1000);
console.log("This will print second");
//it adds the slow task to a "TODO list" and keeps on running our program The task runs some time later, "asynchronously" 
```
---
Some things that take time: 

• Waiting for user events 

• Asking a user to pick a file 

• Getting permission to access the camera/mic

• Loading data from the interwebs 

---












