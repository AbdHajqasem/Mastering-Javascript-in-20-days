# Day8
## Closure:
Closure 
- Closure is the most esoteric of JavaScript concepts
 
- Enables powerful pro-level functions like 'once' and 'memoize'
  
- Many JavaScript design patterns including the module pattern use closure
  
- Build iterators, handle partial application and maintain state in an asynchronous world 
**Functions get a new memory every run/invocation(doesn't remember anything from the old run)**
##### Ex. 
``` javascript
function multiplyBy2 (inputNumber){
 const result = inputNumber*2;
 return result;
 } 
const output = multiplyBy2(7);
const nowOutput = multiplyBy2(10);
```
**Functions can be returned from other functions in JavaScript.**
##### Ex. 
``` javascript
function createFunction(){
 function multiplyBy2(num){
   return num*2; 
}
 return multiplyBy2;
} 
const generatedFunc = createFunction();
const result = generatedFunc(i);
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/4cdbc92d-3899-4313-b581-c042a7c628fa)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/9b51b5e1-cfb4-468a-b0e6-01d958506706)

---
## Nested Function scope:
##### Ex. 
``` javascript
Calling a function in the same function call as it was defined 
function outer (){
 let counter = 0; 
 function incrementCounter(){ 
   counter ++;
 } 
 incrementCounter(); 
}
outer(); 
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/c74ad583-3abe-42d9-82fe-4246ddc5b480)

---
## Reataining Function Memory:
Calling a function outside of the function call in which it was defined 
##### Ex. 
``` javascript
function outer (){
 let counter = 0;
 function incrementCounter (){
  counter ++;
}
 return incrementCounter;
} 
const myNewFunction = outer();
myNewFunction();
myNewFunction();
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/f832ecbc-71fb-4570-924e-c2f15099e27d)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/5259c6cf-a5b3-47c9-a237-f83122e69340)

**when i return  'incrementCounter' iam not just returning the function, i return all the surrounded data out and put it in the backpack**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/2ad6725f-face-45ea-821d-1cfd07b2f0cb)

---
**so the count++ will stored in the count that come with the function when i returned it.**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/2b7227ba-c253-4a2a-a872-4a1f1f483494)

---

**so at the end the count will equal 2**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/c4281c17-808a-44da-ae0a-799b744ecb31)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/61618afb-1876-4af1-9de2-bca88a3c58a3)

---

#### What can we call this 'backpack'? 
-Closed over Variable Environment' (C.O.V.E.)

-Persistent Lexical Scope Referenced Data (P.L.S.R.D.)

-'Backpack'

-'Closure' 

The 'backpack' (or 'closure') of live data is attached incrementCounter (then to myNewFunction) through a hidden property known as ((scope]) which persists when the inner function is returned out.

---

### Multiple Closure Instances:
**Let's run outer again** 
##### Ex. 
``` javascript
function outer (){
 let counter = 0;
 function incrementCounter(){
  counter ++; 
}
 return incrementCounter; 
} 
const myNewFunction = outer();
myNewFunction();
myNewFunction(); 
const anotherFunction = outer();
anotherFunction();
anotherFunction(); 
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/e3f0f1ef-e82d-4ca8-bf58-a6deaeb25e5a)

---

**If i print the counter in 'myNewFunction' the output will be at the first time '1' and at the second time will be '2' and when i print it in the 'anotherFunction' it will be '1' then at the second time will be 2 either becuase they have defferints backpacks from each other.**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/705b5a21-23f7-4180-8222-d10c92f0f8fb)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/8fb0341b-b7b2-4023-b41d-09ff066ee9bc)

---

## Asynchronous Java-Script:
**Promises, Async & the Event Loop** 

-Promises the most signficant ES6 feature
  
- Asynchronicity the feature that makes dynamic web applications possible 
  
- The event loop JavaScript's triage
  
-  Microtask queue. Callback queue and Web Browser features (APIs)

---
  ![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/9f67325c-d2e3-473f-97f2-fed42965784c)

What if we try to delay a function directly using setTimeout? 

setTimeout is a built in function - its first argument is the function to delay followed by ms to delay by 
##### Ex. 
``` javascript
function printHello(){
 console.log("Hello"); 
} 
setTimeout(printHello, 1000);
 console.log("Me first!"); 
//In what order will our console logs appear?
```

**Web Browser Features:**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/43caccc0-12a1-4988-adeb-6d4f7ab372e6)

**The code above will print 'Mefirst' then will print 'Hello' and thats how it works:**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/0a96bbf9-37ff-4176-8425-707cc9b1816d)

---

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/e8509fd7-0476-46ad-89f6-94ffc5c7dadd)






  
  

  































