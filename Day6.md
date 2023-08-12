# Day6
## APIs & Fetch:
URLs point to resources on the web.
### fetch():
lets us use JS to load data from APIs 
##### Ex.
```javascript
fetch("https://dog.ceo/api/breed/hound/list") 
//But if we run it in the console, we see something weird...
```
## Promises:
It takes time to fetch data from the network 
##### Ex.
```javascript
>> fetch("https://dog.ceo/api/breed/hound/list")
>>  Promise { <state>: "pending" }// The output 
//So JS writes us an "IOU" for the data value it doesn't have yet aka a Promise of a value 
```
**Promises can be in 3 possible states:** 
• pending: still waiting for the value, hang tight 

• fulfilled (aka "resolved"): finally got the value, all done 

• rejected: sorry couldn't get the value, all done 

It takes time for Promises to resolve, so they are "asynchronous" 

---
## await:
In the case of a Promise, it waits for it to resolve before continuing with our code. 
##### Ex.
```javascript
let response = await fetch("https://dog.ceo/api/breed/hound/list")
console.log(response); 
//The Promise we get from fetch () resolves to a Response object
``` 
### Calling the . json()method:
on the response parses its body as a JSON object 
##### Ex.
```javascript
response.json() 
//But that gives us another Promise!
```
Let's try again, this time awaiting the JSON Promise too
##### Ex.
```javascript
let response = await fetch("https://dog.ceo/api/breed/hound/ list")
let body = await response.json();
```
**The output**:
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/d581ed7c-5940-4fa2-82d7-953cc3b56453)

---
## Destructing Objects & Arrays:
Destructuring is a fancy way of declaring multiple variables at once. 

By "extracting" values from an object with their property names
##### Ex.
```javascript
Let {name, nickname} = spices[0]; // spices an array of objects 
```
**If we only care about some of the properties, we can omit the others**:
##### Ex.
```javascript
let{nickname} = spices[2];// spices an array of objects
```
**We can also destructure Arrays, assigning variable for their items:**
##### Ex.
```javascript
let [one, two . three]=[1,2,3]
// The output is one-->1, ywo-->2, three-->3
```
##### Ex.
```javascript
We can ignore the values in the array we don't need 
const [emma, geri) = spices; 
We can use commas to "skip" values 
const (, , me113) = spices; 
```

#### .split():
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/87ad4f3c-f7e6-456b-bacb-091ce11bd61d)

**its like we said split the string whenever you see a space**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/9b1c5d0b-ad9f-4d4d-bc9d-c5e6021aa94e)

---
## Async Functions:
If we try to await something in a regular function... 
##### Ex.
```javascript
function fetchResponse(url){
 const response = await fetch(ur1);
 return response; 
} 
//JS doesn't allow it
```
**We need to make it an async function**
##### Ex.
```javascript
async function fetchResponse(url){
 const response= await fetch(ur1);
 return response; 
}
await fetchResponse("https://frontendmasters.com/courses/javascript-first-steps/async-functions/")
```
**This tells JS to expect to await async operations inside the function**

---
## Modules:
Modules let us split big codebases across multiple files
##### Ex.
```javascript
<script type="module", //... </script> 
//JS modules work differently from JS scripts
```
### Module scope:
Another difference is that modules create their own scope 

Try loading the page and accessing the **BREEDS** variable we declare in the module 

---

### import && export:
**export lets us expose variables from our module's scope to the outside world**
##### Ex.
```javascript
// myModule.js 
const veryUsefulFunction = () => "I came from a module";
export {veryUsefulFunction };
```
**import lets us use an exposed variable from another module**
##### Ex.
```javascript
// otherModule.js
 import {veryUsefulFunction } from './myModule.js' 
 veryUsefulFunction();
```
---
## Debugging:
### Use console . log ( ) (or .warn ( ) or . error ( )):
**is one way to understand what's happening when your program runs** 
##### Ex.
```javascript
function whyIsntThisWorking(input){
 console.log("Well at least we got this far");
 console.log(input);
 return  thingThatDoesntWork(input); 
}
```
---
### use Browser Debugger:
You can also use the browser's debugger to pause JS and inspect what's happening 
##### Ex.
```javascript
function whyIsntThisWorking(input) {
 debugger;
 return thingThatDoesntWork(input); 
} 
The debugger statement creates a breakpoint where JS will pause and let you look around 
```
---
## try & catch:





