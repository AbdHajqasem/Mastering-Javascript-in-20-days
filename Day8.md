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


