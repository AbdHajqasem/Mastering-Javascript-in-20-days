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
