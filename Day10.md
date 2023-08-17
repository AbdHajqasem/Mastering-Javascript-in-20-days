# Day10
## Class & Prototypes:
**Classes, Prototypes - Object Oriented JavaScript** 

- An enormously popular paradigm for structuring our complex code
  
- Prototype chain - the feature behind-the-scenes that enables emulation of OOP but is a compelling tool in itself

- Understanding the difference between _proto_ and prototype

- The new and class keywords as tools to automate our object & method creation

  ---

  **Core of development (and running code)**
  
1. Save data (e.g. in a quiz game the scores of userl and user2)
  
2. Run code (functions) using that data (e.g. increase user 2's score)

**Easy! So why is development hard?**

In a quiz game I need to save lots of users, but also admins, quiz questions. quiz 
outcomes, league tables - all have data and associated functionality 

**In 100.000 lines of code**

Where is the functionality when I need it How do I make sure the functionality is only used on the right data! 

---

**Objects - store functions with their associated data!**

This is the pnnople of encapsulation - and n's gong to transferal how we can 'reason about' our code 

##### Ex.
```javascript
const user1 = {
 name: "Will",
 score: 3,
 increment: function() { userl.score++; }
};
userl.increnent0;

//Let's keep creating our obtects What alternative techniques do we have for creating obpects?
```

**Creating user2 user dot notation**

Declare an empty object and add properties with dot notation 
##### Ex.
```javascript
coast user2 = {}; 
user2.name = "Tim";
user2.score = 6;
user2.ineregalt = functIon() { user2.score++; };
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/493ffe2b-6cfc-4c9f-80c7-b64082a87e24)

---

Creating user3 using **Object.create**  

Object create is going to gwe us fine •grained control over our object later on 
##### Ex.
```javascript
const user3 = Object .create(null); 
user3.name = "Eva";
user3.score = 9;
 user3.increment = function(){
user3.score++;
};
```
---

### Generating Objects Using a Functio: 
##### Ex.
```javascript
function userCreator(name, score){
 const newUser = {};
 newUser.name=neme;
 newUser.score =score;
 newUser.incrementt=function () {
  newUser.score++;
};
 return newUser; 
}; 
const userl =userCreator(will"; 3);
const user2 = userCrestor("Tim", 5);
user1.increment()
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/3c917519-22e0-47af-b2d1-68d74793384f)

Problems: Each time we create a new user we make space in our computer's memory for all our data and functions. But our functions are just copies 

Is there a better way!

Benefits: Its simple and easy to reason about! 

---
### Solution 2: Using the prototype chain
Store the increment function in just one object and have the interpreter, if it doesn't find the function on user1, look up to that object to check if its there

Link user1 and functionStore so the interpreter, on not finding .increment, makes sure to check up in functionStore where it would find it

Make the link with object.create( ) technique 

##### Ex.
```javascript
function userCreator (name, score) {
const newUser = Object.create(userFunctionStore); newUser.name = name;
 newUser.score = score;
 return newUser; 
}; 
const userFunctionStore = {
increment: function(){this.score++;},
 Login: function(){console.log("Logged in");}
}; 
const users1 =userCreator("Will", 3);
const user2 = userCreator("Tim", 5);
userl.increment();
```
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/e28d8e11-d4b7-4b82-aa95-de2ac8d781f2)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/5d4b0d04-6944-4f64-b47c-f53e65b14f15)

















  
