# Day6
## APIs & Fetch:
URLs point to resources on the web.
### fetch():
lets us use JS to load data from APIs 
##### Ex.
```javascript
fetch("https://dog.ceo/api/breed/hound/list") 
//But if we run it in the console, we see something weird...
```
## Promises:
It takes time to fetch data from the network 
##### Ex.
```javascript
>> fetch("https://dog.ceo/api/breed/hound/list")
>>  Promise { <state>: "pending" }// The output 
//So JS writes us an "IOU" for the data value it doesn't have yet aka a Promise of a value 
```
**Promises can be in 3 possible states:** 
• pending: still waiting for the value, hang tight 

• fulfilled (aka "resolved"): finally got the value, all done 

• rejected: sorry couldn't get the value, all done 

It takes time for Promises to resolve, so they are "asynchronous" 

---
## await:
In the case of a Promise, it waits for it to resolve before continuing with our code. 
##### Ex.
```javascript
let response = await fetch("https://dog.ceo/api/breed/hound/list")
console.log(response); 
//The Promise we get from fetch () resolves to a Response object
``` 
### Calling the . json()method:
on the response parses its body as a JSON object 
##### Ex.
```javascript
response.json() 
//But that gives us another Promise!
```
Let's try again, this time awaiting the JSON Promise too
##### Ex.
```javascript
let response = await fetch("https://dog.ceo/api/breed/hound/ list")
let body = await response.json();
```
**The output**
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/d581ed7c-5940-4fa2-82d7-953cc3b56453)



