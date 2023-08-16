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






  
