# Day1

#### Java-Script Definition:

its a high-level programing language that used for web development, and  help us to modify website

---

#### DOM stand for:

Document-Object-Model

---
#### DOM:

Java-Script create an object(entity) that represnts the document and all of the structure inside of it

---
#### docttype:

defines the document type

---
# Print sentence
```javascript
console.log("Hello!")
```
---
#### Return the page title:

```javascript
document.title //Return the title of the document:
```
---
#### Return the body:
```javascript
document.body //Return the body element
```
---
### Return whats elements inside the body:
```javascript
document.body.children //Return a group of elements that are inside the body:
```
---
# Finding Elements
##### 1-Using ID

### 
```javascript
document.getElementById("id") //Return an element whose ID corresponds to the word in the brackets
```

or

```javascript
document.querySelector("id") //Return an element whose ID corresponds to the word in the brackets
```

---
##### 2-Using Class-Name:
```javascript
document.getElementByClassName("className") //Return  a list of element whose Class-name corresponds to the word in the brackets
```

or
```javascript
document.querySelector("classname") //Return an element whose Class-name corresponds to the word in the brackets
```
or 

```javascript
document.querySelectorAll("classname") //Return a list of element whose Class-name corresponds to the word in the brackets
```
---

##### Using Tag-Name:
```javascript
document.getElementsByTagName("tagName") //Return  a list of element whose Tag-name corresponds to the word in the brackets
```

or

```javascript
document.querySelector("tagname") //Return an element whose Tag-name corresponds to the word in the brackets
```

or

```javascript
document.querySelectorAll("tagname") //Return a list of element whose Tag-name corresponds to the word in the brackets
```
---
##### using Name
```javascript
document.getElementsByName("name") //Return  a list of element whose Name corresponds to the word in the brackets
```

or 

```javascript
document.querySelector("tagname") //Return an element whose Name corresponds to the word in the brackets
```

or

```javascript
document.querySelectorAll("name") //Return a list of element whose Name corresponds to the word in the brackets
```
---
# Make Changes:
#### 1-change the page title:
```javascript
document.title="someThing"
```
#### 2-change the element text:
```javascript
document.getElementById("id").textContent="name"
```
---
# Another commands

```javascript
document.querySelectorAll("x").length //Appear the number of the elements that return
```


```javascript
document.getElementById("id").textContent //Return the text inside the element
```


```javascript
document.getElementById("id").append("somthing") //to add  onto text
```

```javascript
clear() //to wipe out what i write before
```
---
#### MDN-Mozilla link:

https://developer.mozilla.org/en-US/


