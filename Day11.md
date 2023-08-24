# Day11
## Introduction:
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/6c4c867a-d232-4126-84b4-dca505111770)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/0ecf19db-8d7c-4d2b-99a0-3f391d72788c)

Whenever there's a divergence between what your brain thinks is happening,

and what the computer does, that's where bugs enter the code. 

---
## Types:
### Primitive Types:
**6.1 ECMAScript Language Types**

An ECMAScript language type corresponds to values that are directly manipulated by an ECMAScript programmer using the ECMAScript language.

The ECMAScript language types are Undefined, Null, Boolean, String, Symbol, Number, and Object.

An ECMAScript language value is a value that is characterized by an ECMAScript language type. 

**1-Undefined**

**2-String** 

**3-Number** 

**4-boolean**

**5-Object**

**6-symbol**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/7c3379a5-05cf-4fb0-9f7e-63f66bdbdd73)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/3dd2e227-a364-442e-8dc8-903d216f0210)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/1c26e1c7-3040-4e73-918c-678fc37e89e2)

**BigInt**:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/0a2db266-5437-43fa-a068-13853ad2e309)

---

### Undefined Vs. Undeclared:
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/63bdf133-9e6f-4aff-8f4a-5ac00c3345a4)

---
### NaN(not a number) & isNaN:(Special Values)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/9aa38b4f-1f40-4206-a9ca-1e0eaa0fdc38)

**NaN: Invalid Number**

---

### Negative Zero:
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/edf5a67f-d9d9-48c4-b594-804f23c0f505)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b2eae470-9d89-41f3-816f-773a6a7d8b61)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/bf93806f-dab2-4279-b986-c3f51e9330ab)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/6502a5d3-211b-476e-ac57-b306aca6c6ba)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/6e7680f3-87cf-4bab-ba5b-1e270dbec400)

```javascript
if (!Object.is /*|| true*/) {
 Object.is = function ObjectIs(x,y) {
 var xNegZero = isItNegZero(x);
 var yNegZero = isItNegZego(y);
 if (xNegZero || yNegZero) {
   return xNegZero && yNegZero;
}
 else if (isItNaN(x) && isItNaN(y)){
  return true;
}
  else if (x === y) {
 return true;
}
return false;
// ********************** 
function isItNegZero(v) {
 return v == 0 && (1/v) == -Infinity; 
} 
function isItNaN(v) {
 v!== v;
}
```










 

 

















