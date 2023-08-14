# Day7
## Java-Script Principles
### Thread of Execution:
When JavaScript code runs, it. 
Goes through the code line-by-line and runs/ 'executes each line known as the **thread of execution** 

Saves 'data' like strings and arrays so we can use that data later - in its memory 
We can even save code **functions** 

---
### Functions:
**functions are a mini program**
Code we save ('define') functions & can use (call/invoke/execute/run) later with the function's name & {}

**Execution context:** 
Created to run the code of a function has 2 parts (we've already seen them)) 

**-Thread of execution**

**-Memory**

---

### Call stack 

1- JavaScript keeps track of what function is currently running **(where's the thread of execution)**:

2-Run a function - add to call stack 

3-Finish running the function - JS removes it from call stack 

4-Whatever is top of the call stack - that's the function were currently running 

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b80d4300-802a-47eb-970c-7f395822f7df)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/3067cca9-bd44-4002-b285-e42f218358fa)


##### Ex:
```javascript
const num = 3;
function multiplyey2(inputNumber){// inputNumber called a parameter, and the value That stored in it which is '3' is called an argument
  const result = inputNumbor*2;
  return result;
}
const output = multiplyBy2(num);
const newOutput = multiplyBy2(10);
// nume=3,  multiplyBy2=->f->, output=multiplyBy2(3)
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/1c7428bd-4f30-4210-bcc6-8ef236d9e402)

---

## Fucntions & Callbacks:
**We can generalize the function to make it reusable** 
##### Ex:
```javascript
funcrion squareNum(num){
  return num*num; 
} 
squareNum(10);
squareNum(9);
squareNum(8);
```
### Generalizing functions: 
'Parameters' (placeholders) meat we don't need to decide what data to run our functionality on until we run the function. 

- Then provide an actual value ('argument') when we run the function
 
Higher order functions follow this same principle.
 -We may not want to decide exactly what some of our functionality is until we 
  run our function
  
  Now suppose we have a function copyArrayAndMultiplyBy2 
  
##### Ex:
```javascript
function copyArrayAndMultiplyBy2(array) {
 const output = [];
 for (let i = 0; i < array.length;i++) {
  output.push(array[1] * 2);
}
  return output;
}
 const myArray = [1,2,3];
 const result =copyArrayAndHultiplyBy2(myarray); 
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/57269a55-9c9d-4ab1-b53d-7b6fa7e78156)

---

### Higher Order Functions:
We could generalize our function - So we pass in our specific instruction only when we run **copyArrayAndManipulate!**.
##### Ex:
```javascript
function copyArrayAndManipulate(array, instructions){// now when i  write instruction(3) it will call the funtion multtplyBY2(3)
 const output =[];
 for (lel i = 0; i < array.lingth;;i++) {
output.push(instructions(array[i]));
 }
return output; 
) 
function mulliplyBy2(Input){
 return input * 2;
}
const result = copyArrayAnditsmiputate([1, 2, 3J, multtplyBY2); 
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/8f981cf7-fc88-48e4-a02a-5365dca9495f)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/8e8c72bd-8817-44b8-943e-90568d35a5a5)






