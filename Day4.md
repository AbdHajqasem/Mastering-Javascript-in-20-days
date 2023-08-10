
## Scope:
In JS it doesn't just matter what variables we declare, 

It also matters where we declare them.

Scope determines where variables are "in play".

##### Ex.
```javascript
function declareBankruptcy() {
 let bankruptcy = true; 
} 
declareBankruptcy();
console.log(bankruptcy); // error (bankruptcy is not definfed)
```
**Scopes are nested within the program The widest scope is the global scope, 
Each function gets its own new scope within the scope where it was declared**.

##### Ex.
```javascript
let planet = "Jupiter"; 
function scopeOut(){
 let planet = "Mars";
 console.log("Inner planets", planet); // The output is Inner planets: Mars
} 
scopeOut();
console.log("Outer planets", planet); // The output is Outer planets: Jupiter
```
**Within each scope, you can access variables declared in a wider scope (e.g. global scope)
But not those declared in a narrower scope(e.g. function scope)**.
##### Ex.
```javascript
let globalVariable = "I live in global scope";
function narrowerScopc() {
 console.log(globalVariable);// The output is "I live in global scope"
 let localVariable = "I live in the function scope"; 
} 
narrowerScope();
console.log( localVariable);// error
```
### let & scope:
Variables declared with let can be modified from within a 

narrower scope This can be useful, but also dangerous! 
##### Ex.
```javascript
let feeling ="free"; 
function trap(){
feeling = "boxedln"; 
} 
trap();
console.log( feeling); // The output is "boxedln"
```
### let Vs. var:
**We can reassign 'var' variables like 'let' variables**
**1- A variable declared with 'let' in a local scope(function/block scope) is limited to that scope, so if you attempt to use it in the global scope or any other local scope, it will result in an error.**
**2- A variable declared with 'var' in a local scope (function scope) is limited to that specific scope like 'let'. However, if you declare it in a (block scope), you can access it both within the global scope and within other local scopes, without encountering an error**.

---
#### Briefly:
1-let is a Function-scoped and Blocked-scope
2-var is a Function-scoped but not Bloacked-scope

**const like let but the difference that const cann't reassign it**

---

## Event & Handlers:
The web browser fires events when certain things happen on the page For example,

when the user clicks somewhere on the page,

a click event is fired.
We can detect events with JS using an event listener The '.addEventListener( )' method lets us listen for events on a 'DOM element'.
##### Ex.
```javascript
document.addEventListener("click", () => {
console.log("clicked")});
```
#### '.addEventListener( )' takes 2 parameters: 
**•The name of the event to listen to (e.g. "click")** 

**•A handler function that JS calls when that event is fired on this element** 
'event.target' is the element the event fired on (in this case, which element was clicked)
##### Ex.
```javascript
document.addEventListener("click", (event) => console.log(event.target); 
```
**"click" isn't the only type of event we can handle** 
**• "dblclick"** 

**• "mouseover"** 

**• "mouseout"** 

...and lots more!** 



