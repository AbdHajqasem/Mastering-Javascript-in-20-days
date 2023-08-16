# Day9
## Promises:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/cadb953c-3857-4ecb-9992-1d63730043a8)

##### Ex.
```javascript
function display(data){
 console.log(data);
 } 
const futureData = fetch('https://twitter.com/will/tweets/1');
futureDdtd.thon(display);

console.log("me first!"); 
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/2e6918f6-9fb6-4739-aeab-7515dada8487)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/cdab34e9-1458-4353-a1ef-9bc4c083121d)

---
**then method and functionality to call on completion** 

1-Any code we want to run on the returned data must also be saved on the promise object 

2-Added using .then method to the hidden property 'onFulfilment' 

3-Promise objects will automatically trigger the attached function to run (with its input being the returned data )

---
**But we need to know how our promise-deferred functionality gets back into JavaScript to be run**
##### Ex.
```javascript
function display(data){
 console.log(data)
}
function printHello(){
 console.log("Hello");
}
function blockFor300ms(){ }

setTimeout(printHello, 0);

const futureData = fetch('https://twitter.com/will/tweets/1')
futureData.then(display)

blockFor300ms();
console.log("Me first!");
```

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/749b33fc-c305-4f90-b541-a85b672f2d02)

---

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/ff374cdc-1bb9-47a8-b909-bdfe2aaf16cf)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/7d58ef07-9f64-4d14-ae98-898aff01befa)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/41330168-55e9-4e23-ae97-0f8444588794)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/add66f20-f3d8-4ece-ada5-e9114f09360a)


**Promises**
Problems 99% of developers have no idea how they're working under the hood

Debugging becomes super-hard as a result 

Developers fail technicalinterviews 

**Benefits**
Cleaner readable style with pseudo-synchronous style code

Nice error handling process 

---

**We have rules for the execution of our asynchronously delayed code** 

Hold promise-deferred functions in a microtask queue and callback function in a task queue (Callback queue) when the Web Browser Feature (API) finishes

Add the function to the Call stack (i.e. run the function) when: 

- Call stack is empty & all global code run (Have the Event Loop check this condition)

Prioritize functions in the microtask queue over the Callback queue 

---

**Promises, Web APIs, the Callback & Microtask Queues and Event loop enable:**

**Non-blocking applications**: This means we don't have to wait in the single thread and don't block further code from running 

**However long it takes**: We cannot predict when our Browser features work will finish so we let IS handle automatically running the function on its completion 

**Web applications**: Asynchronous lavaScript is the backbone of the modern web -letting us build fast 'non-blocking' applications 













