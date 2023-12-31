# Day3
## Arrays:
#### Arrays let us keep multiple values together in a single collection.
##### EX.
```javascript
let arr= ["abd","khaled"];
```
#### like Strings, Arrays have a length, and each value has an index:
##### EX.
```javascript
let arr= ["abd","khaled"];
arr[1]// the output is "khaled"
arr.length // the output is 2
arr.indexOf("abd") // The output is 0
```
---
#### also like strings, we can check if an array contains a certain value:
##### EX.
```javascript
let arr= ["abd","khaled"];
arr.includes("abd") // The output is true
```
---

##### EX.
```javascript
let arr= ["abd","khaled"];
arr[1]="ahmad" // this command place the string value ahmad in index 1
```
---
### push() & pop():
**push()** is:used to add one or more elements to the end of an array and return the new length for the array.

**pop()** is: used to remove the last element from the end of an array, and return the removed item.
##### EX.
```javascript
let arr= ["abd","khaled"];
let name=arr.pop(); // The value "khaled" located at the last index of the array has been removed, and we have assigned it to the variable named "name".
arr.push("ahmad")// We pushed the string value "ahmad" to the last index in the array.
```
---
#### Arrays can be empty, or hold a single item:
##### EX.
```javascript
let arr= [];// defined an empty array
let arry= ["abd"];// Array with a single item
```
---

#### Arrays can hold any type of items, or mix:
##### EX.
```javascript
let arr= ["abd","khaled", 6 , false];
```
---

### Arrays properties:
#### 1-sort():
##### EX.
```javascript
["c","a","d","b"].sort() //The output is ["a","b","c","d"]
```
---
#### 2-join():
##### EX.
```javascript
["c","a","d","b"].join(" & ") //The output is "c & a & d & b"
```
---
#### 3-concat():
##### EX.
```javascript
[1,2,3].concat([4,5,6]) //The output is [1,2,3,4,5,6]
```
---
### Mutable Vs. Immutable:
**1-Mutable**: data can be edited(e.g. Arrays)
##### EX.
```javascript
let arr=[1,2,3]
arr[1]=5 //The array become [1,5,3]
```
---
**2-Immutable**:data always stays the same (e.g. Strings & other Primitives)
##### EX.
```javascript
let name="abd"
name[1]=f // It will stay abd
```
---
### concat() Vs. push():
**push()**: it's an action **mutate** an array, aka change the array in-place.
##### EX.
```javascript
let arr=[1,2,3]
arr.push("4") // if i print the array "arr" the output is [1,2,3,4], because the change has done in-place.
```
---
**concat**:action do not mutate the original array, but instead create a new copy.
##### EX.
```javascript
let arr=[1,2,3]
[1,2,3].concat([4]) // When printing the array, the output appears as [1, 2, 3]. This is because the modifications were not applied directly to the original array. Instead, a copy of the array was created, and the values were added to it, resulting in [1, 2, 3, 4]. If you want to obtain the modified array, you must use the concatenation operation ([1, 2, 3].concat([4])) and assign it to a new variable in order to reference the new set of values.
```
 ##### EX.
```javascript
let arr=[1,2,3]
let arry=[1,2,3].concat([4])// If i print "arry" the output is [1,2,3,4]
```
---
#### const with arrays:
if i declared an array using 'const' i can  still make modifications to an array declared with const. The const keyword ensures that the variable itself cannot be reassigned to a different value or reference. However, it does not make the value (in this case, the array) immutable.

So, you can modify the contents of the array (add, remove, elements) even if the array is declared with const. The key point is that you cannot reassign the array variable to a completely new array.
 ##### EX.
```javascript
const arr = [1, 2, 3];
arr.push(4);
console.log(arr); // The output is [1, 2, 3, 4]

arr[1] = 10;
console.log(arr); // The output is: [1, 10, 3, 4]

arr = [5, 6, 7]; // This would result in an error because you're trying to reassign the "arr" array, to a new array, which is not allowed with const.
```
---
**Note**:
 ##### EX.
```javascript
ler arr1=[1,2,3];
let arr2=arr1;
arr1[1]=4;// I've changed the value in the index1 in array 'arr1', then it becomes [1,4,3], depending on this change the array 'arr2' will also change to [1,4,3], because the arrays 'arr1'/'arr2' both point the values [1,2,3].
```
---
## Objects:
Objects collect multiple values together to describe more complex data Similar to how we can point at different values using variables in our code, objects let us point at related values using properties in the object. 
 ##### EX.
```javascript
const js ={
  name: "JavaScript",
  abbreviation: "JS",
  isAwesome: true,
  officialSpec: "EcmAscript",
  birthYear: 1995,
  creator: "Brendan Eich"
}:
```
### Getting property values:
 ##### EX.
```javascript
const js ={
  name: "JavaScript",
  abbreviation: "JS",
  isAwesome: true,
  officialSpec: "EcmAscript",
  birthYear: 1995,
  creator: "Brendan Eich"
}:
js.name //The output is "JavaScript", as we can see the output of this is a string so we can do the stringy stuff
//EX.
js.name.startWith("Java")// The output is true
// or we can do
let age =2022-js.birthYear
js.isAwesome // The output is true
```
---
### Reassigning object values:
 ##### EX.
```javascript
const indecisive = { 
lunch:"sandwich"
};
indecisive.lunch = "tacos"; //indecisive.lunch will become 'tacos'
indecisive.snack = "chips"; //We declared a new property call snack

```
**note**:The object is mutable
**note**:Arrays is an object
how is this?
its like the indexes are the name of the properties in the array like index 0 its a property name as 'lunch' is a property name the 'indecisive' object, so like the property 'lunch' point the value 'tacos' and the 'index0' point the item which he corresponds to in the array.

---
##### EX on objects:
```javascript
const abdulkareem = 
{ name: "Abdulkareem", 
home: "Tulkarm",
languages: ["English", "German", "French"],
pet: null,
vehicle: "Vespa",
hobbies: ["travel", "climbing", "gaming", "lindy hop"] 
}; 
```
---
#### .freeze():
The Object.freeze() static method freezes an object. Freezing an object prevents extensions and makes existing properties non-writable and non-configurable. A frozen object can no longer be changed: new properties cannot be added, existing properties cannot be removed, their enumerability, configurability, writability, or value cannot be changed, and the object's prototype cannot be re-assigned. freeze() returns the same object that was passed in.
##### EX:
```javascript
const obj = {
  prop: 42,
};
Object.freeze(obj);
obj.prop = 33; // Throws an error 
console.log(obj.prop); // Expected output: 42
```
---
### Objects & Functions:
Properties can point to functions too We call function-properties "methods" on objects 
##### EX:
```javascript
const dog = { name: "Ein",
 breed: "Corgi",
 speak: function () { console.log("woof woof"); 
} 
} 
dog.speak(); //The output is "woof woof"
```
---
### this.:
'this' in a method lets us reference other properties on the object 
##### EX:
```javascript
const abdulkareem = { 
name: "Abdulkareem"
}
abdulkareem.speak=function(){ console.log("Hi my name is", this.name); 
} 
anjana.speak(); // The output is Hi my name is Abdulkareem
```
---
## Nested objects:
##### EX:
```javascript
const menu = {
 lunch: {
 appetizer: "salad",
 main: "spaghetti",
 dessert: "tiramisu" 
},
dinner:{
 appetizer: "samosa",
 main: "saag paneer",
 dessert: "gulab jamun" 
}
 }; 
const tiramisu = menu.lunch.dessert; // The output is  "tiramisu"
```
---

## Objects in Arrays & Objects:
##### EX:
```javascript
const spices = [
{name: "Emma", nickname: "Baby"},
 {name: "Geri", nickname: "Ginger"},
 {name: "Mel B", nickname: "Scary"},
 (name: "Mel C", nickname: "Sporty"},
 {name: "Victoria", nickname: "Posh"} 
]; 

const spiceGirls = {
 albums: ["Spice", "Spiceworld", "Forever"],
 motto: "Girl Power",
 members: spices 
};
```
---
### Build-In Objects:
#### 1-Document:
#### 2-Console
#### 3-Math
#### 4-Strings(when we use methods and propirties)
##### EX.
```javascript
document.getElementById("id");
document.title;
console.log("hello");
console.warn("oh")// it will print whats inside the brackets but with warning
console.error("danger")// it will print whats inside the brackets but with red exclamation point
Math.PI// the output is 3014459....
Math.random()
let s="abd"
s.toUpperCase()
```
---
### Script tag(<Script>js-code</script>):
Used to write javascript inside it.

---

## Functions:
### Declaring(creating) a function:
##### EX.
```javascript
function half(x){
return x / 2; 
} 
const one = half(2); //calling (using) a function: 
```
---
### Parameters & Arguments
Some functions need more than one value to work 
##### EX.
```javascript
function add(x, y){
return x + y; 
} 
add(2,3); 
```
Some functions don't even need any values 
##### EX.
```javascript
function getRandomNumber() {
return Math.random();
} 
getRandomNumber(); 
```
**parameters are the inputs a function expects**
##### EX.
```javascript
function add3(x, y, z) {
console.log("My parameters are named x, y, z");
console.log("I received the arguments", x, y, z);
return x + y + z; 
} 
coast sum = add3(4,5,6);
```
**what happened if i pass two parameters to function (add3)**
##### EX.
```javascript
 let sum= add3(1,2)//The output will be parameters are named xadd3(1,2)x , y, z/I received the arguments 1 2 undefined /  and if i print sum the outputwill be NaN(because z is undefined)
```
**arguments are the actual values the function is called with**
**Parameters should be named like variables, and behave like variables within the function body** 
##### EX.
```javascript
function doesThisWork("literally a value"){ //error
return true; 
} 
function howAboutThis(lweirdVariable!){ //error because its am invalid variable name
return true;
} 
```
---
### Return values:
Return values A return statement specifies the function's output value 
##### EX.
```javascript
function square(x) {
return x * x; 
} 
const nine = square(3); 
```
**Some functions don't return anything**
##### EX.
```javascript
function sayHello(name) {
console.log("Oh hi, " + name + "I");
} 
sayHello("Marc");
// The value that returned when there's no return is "undefined"
```
##### EX.
```javascript
function sayHello(name) {
return 2+2;
console.log("Oh hi, " + name + "I");
} 
let hi=sayHello("Marc");// The function will not reach the console.log statement and display its contents because the execution of the function is terminated by the return statement. This prevents any subsequent code within the function from being executed, including the console.log statement.
```
**Another way to declare a function**:
##### EX.
```javascript
const yell = function (saying){
 return saying.toUpperCase();
 }
  yell("hello")// The output is "HELLO" 
```
---
### Arrow functions:
The => "fat arrow" lets us create an unnamed function without much code 
##### EX.
```javascript
(x, y) => x + y 
```
Since arrow functions are expressions, we can assign them to a variable 
##### EX.
```javascript
const add=(x,y)=>x+y
//is equivalent to 
function add1(x, y) {
 return x + y;
}
```
**Arrow functions are great when we just want to return value**

**For one-parameter functions, parentheses are optional**
##### EX.
```javascript
X => X*X 
(x) => x*x
```
**If we need to do more than just return a value, we can use curly braces for a "normal" function body In that case, we still need a return**: 
##### EX.
```javascript
const addAndLog = (x, y) => {
let sum = x + y;
 console.log('The sum is', sum);
 return sum;
}
```
---

**to change on the html code**:
#### .setAttribute
##### EX.
```javascript
let button=document.getElementsByName("ture")
let b=button[0];
b.setAttribute("naame","abd")
b.setAttribute("disabled", "")
```
---
#### .removeAttribute
##### EX.
```javascript
let button=document.getElementsByName("ture")
let b=button[0];
b.removeAttribute("disabled)
```
---
**To covert to string**:
#### toString():
##### EX.
```javascript
true.toString()
```
---

