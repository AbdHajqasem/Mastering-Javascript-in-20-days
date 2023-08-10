# Day4
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
