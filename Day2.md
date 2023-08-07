# Day2

## Datatypes in Java-Script:
1-Primitive Datatypes

2-Objects

---
### Primitive Datatypes:
#### 1-Strings
##### Ex.
"Hello" , '49'

----
#### 2-Numbers
##### Ex.
(46) , (297884) , (-3.256)

---
#### 3-Boolean
##### Ex.
true/false

---
4-Undefined

---
5-Null

---

### typeof operator:
The **typeof** operator returns a string indicating the type of the operands value.

##### Ex.
```javascript
typeof 46 //The output is "number"

typeof true //The output is "boolean"

typeof "true" //The output is "String"

typeof documnet.title //The output is "String"

typeof undefined //The output is "undefined"

typeof null //The output is "object"
```
---

### Characters:
the Strings made of characters

characters is : an Individual units that make up a string.

#### To return the character for using an index from string:
```javascript
"hello"[0] //the output is "h"

"hello"[3] //the output is "l"
```

---

### String properties:
#### 1-indexof:
Return the character for the entered index 
```javascript
"hello".indexof("h")// the output is 0

"hello".indexof("l")// the output is 2// if we have multiple of the same character we gonn find the first one

"hello".indexof("q")//the output is -1 because the character doesnt exist

"hello".indexof("H")//the output is -1 because its case sensitive

"hello".indexof("he")// the output is 0 because the substring begins in the index 0
 
"hello".indexof("heo")// the output is -1 because the substring doesnt exist
```
---


#### 2-inculdes: 
use to know that the string contains the string in the brackets
```javascript
"hello".inculdes("he")// the output is true

"hello".inculdes("hek")// the output is false
```
---
#### 3-stratsWith:
to tell us that the string start with some other string
```javascript
"hello".stratsWith("he")// the output is true

"hello".stratsWith("el")// the output is false
```
---



