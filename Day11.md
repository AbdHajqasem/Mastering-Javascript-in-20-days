![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/9c56f5e4-4ea2-49fa-b586-67b1e6cf7380)# Day11
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

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/01763525-83f4-4912-8346-4da894b3720e)

##### Ex:
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
---

### Fundamental Objects:
**Built-in Objects**
**Native Functions**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/ce9c9074-78ae-42b7-ab9c-572186909ae4)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/a2092cd4-333e-42fc-9dbd-d415a22e133c)

---

## Coercion:
Abstract Operations :

These operations are not a part of the ECMAScript language; they are defined here to solely to

aid the specification of the semantics of the ECMAScript language. Other, more specialized 

abstract operations are defined throughout this specification. 

Type Conversion :

The ECMAScript language implicitly performs automatic type conversion as needed. To clarify 

the semantics of certain constructs it is useful to define a set of conversion abstractoperations.

The conversion abstract operations are polymorphic; they can accept a value of any ECMAScript 

language type. But no other specification types are used with these operations. 

### ToPrimitive():
**Its an abstract Operation**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/95e9cee9-6aef-4cce-b378-3738ed1249c3)

---

###  ToString():
##### Ex.

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b9192de8-a97a-485c-a49c-db9f2d76cd32)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/87442440-ce41-48c8-9006-07a1cd540f37)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/65120aee-6d8e-417b-a6d8-6f0044ebe3b6)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/166aa489-a973-4260-851c-ca0a8d7bf316)

---
### ToNumber():
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b015d4be-59c9-4af3-8d2d-3dd2270a96c4)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/313f7720-2283-4233-8faa-d788498ecf08)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/af9b968c-7c05-4e46-a57a-ea03eeaf3349)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/ac97dc73-e43e-43af-9d0a-c5b88c7ebb06)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/e87c3fea-6e60-41b3-b2ad-68391d32ec6c)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/2087d79d-5063-4e41-8cba-4821ef4485da)

---

### ToBoolean:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/408764b4-0331-48c2-b3ae-cb68ab9e9b3c)

**Every thing not in the falsy list is Truthy**

**Ex.**
**Empty array :Truthy**

---

### Cases of Coercion:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/40b4790b-868a-4582-9bb8-e5d87990ba59)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/c0a11808-ee78-4e01-a0a2-cd298c2a3ef4)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/9d30be0f-c10f-458b-b777-88bfdacecde0)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/9095aa37-c21d-438e-b75f-8d14d2452723)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/f9cffc69-9e7e-450d-947d-2ada93a852de)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/dba55e65-ab77-445f-8b8e-e707659846f6)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/3c365cb5-b0a7-4dd0-be37-4a19ffd3f18a)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/29137868-cd47-4246-9836-e2e62ae40b79)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/f39bfb11-df73-400e-8538-4819aa5f13db)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/be1df997-9654-4159-a7e5-f966b9ba02e4)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/74183c93-448d-43c1-86b4-10b97e6afa94)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/2a8461f7-3654-4494-8e4e-69ac26968c7e)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/39a447bf-8226-4fd3-b914-cdebe6bf5bd1)

---
### Boxing:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/81d62103-bf7d-4988-b5f3-7179fbfa3c05)

**All programming languages have type conversions, because it's absolutely necessary.** 

---

### Corener Cases:
**Some Ex. on corner cases**
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/290b1465-6c30-459f-8d13-ee06ae1d9ab0)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/c67aee01-dc5a-4799-a43b-e2152b02d241)











































































 

 

















