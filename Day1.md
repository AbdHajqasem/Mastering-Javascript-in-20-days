# Day1
---
Java-Script Definition:

its a high-level programing language that used for web development, and  help us to modify website

---

DOM stand for:

Document-Object-Model

---
//DOM:
Java-Script create an object(entity) that represnts the document and all of the structure inside of it

//docttype:
defines the document type

```javascript
document.title //Return the title of the document:
```
//Return the body element:
document.body

//Return a group of elements that are inside the body:
document.body.children

Return an element whose ID corresponds to the word in the brackets:
document.getElementById("id")

//To wipe out what i write before:
clear()

//Return an element whose ID or Class or Tagname...etc, corresponds to the word in the brackets:
document.querySelector("#id/.class/tagname")

//Return  a list of element whose Tagname corresponds to the word in the brackets:
document.getElementsByTagName("tagName")

//Return  a list of element whose Tagname or Class-name...etc, corresponds to the word in the brackets:
document.querySelectorAll("tagname/.className")

//Return  a list of element whose Class-name corresponds to the word in the brackets:
document.getElementByClassName("className")

//Appear the number of the elements that return:
document.querySelectorAll("x").length

//Return the text inside the element:
document.getElementById("id").textContent

//Return  a list of element whose Name corresponds to the word in the brackets:
document.getElementsByName("name")

//To change the page title:
document.title="someThing"

//To change the element text:
document.getElementById("id").textContent="name"

//To add  onto text:
document.getElementById("id").append("somthing"):to add  onto text
