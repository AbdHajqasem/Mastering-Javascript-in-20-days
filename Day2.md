# Day2

## Datatypes in Java-Script:
1-Primitive Datatypes

2-Objects

---
### Primitive Datatypes:
#### 1-Strings
##### Ex.
"Hello" , '49'

---

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
The Strings made of characters

characters is : an Individual units that make up a string.

#### To retrieve the character at a specific index from a string:

##### Ex.
```javascript
"hello"[0] //The output is "h"

"hello"[3] //The output is "l"
```

---

### String properties:
#### 1-indexof():
Return the index for the entered character

##### Ex.
```javascript
"hello".indexof("h")// The output is 0

"hello".indexof("l")// The output is 2// if we have multiple of the same character we gonn find the first one

"hello".indexof("q")//The output is -1 because the character doesnt exist

"hello".indexof("H")//The output is -1 because its case sensitive

"hello".indexof("he")// The output is 0 because the substring begins in the index 0
 
"hello".indexof("heo")// The output is -1 because the substring doesnt exist
```
---

#### 2-inculdes(): 
Use to know that the string contains the string in the brackets

##### Ex.
```javascript
"hello".inculdes("he")// The output is true

"hello".inculdes("hek")// The output is false
```
---
#### 3-stratsWith():
To tell us that the string start with some other string

##### Ex.
```javascript
"hello".stratsWith("he")// The output is true

"hello".stratsWith("el")// The output is false
```
---

#### 4-length:
Return the number of characters in the string

##### EX.
```javascript
"hello".length// The output is 5

" ".length// The output is 1 // the space is character
```
---

#### 5-toLowerCase():
Converts a string to lowercase letters

##### EX.
```javascript
"Hello".toLowerCase()// The output is "hello"
```
---

#### 5-toUpperCase():
Converts a string to uppercase letters

##### EX.
```javascript
"hello".toUpperCase()// The output is "Hello"
```
---
### Connecting strings togehter:
**(+)** used to connect strings togehter

##### EX.
```javascript
"hello"+"!"//The output is "hello!"
```
---

## Operators in Java-Script:
1-Arithmetic Operators

2-Comparsion Operators

3-Equality operators

---

### 1-Arithmetic Operators:
#### 1)+ Add
```javascript
3+1 //The output is 4
```
---
#### 2)- Subtract
```javascript
3-1 //The output is 2
```
---
#### 3)* Multiply
```javascript
3*1 //The output is 3
```
---
#### 4)/ Divide
```javascript
3/1 //The output is 3
```
---
### 2-Comparsion Operators:
Return a boolean value(true or false)

#### 1)> Greater than
##### EX.
```javascript
3>1 //The output is true
```
---
#### 2)< Less than
##### EX.
```javascript
3<1 //The output is false
```
---
#### 3)>= Greater than or equal to
##### EX.
```javascript
3>=1 //The output is true
1>=1 //The output is true
```
---
#### 4)<= Less than or equal to
##### EX.
```javascript
3<=1 //The output is false
1<=1 //The output is true
```
---

### 3-Equality operators:
#### 1)===  == equals
#### 2)!==  != does not equal
!== & === its compare the values and the data type
!= & == its just compare the value

##### EX.
```javascript
1===1 // the output is true
1==1 // the output is true
"1"==="1" // the output is true 
"1"=="1" // the output is true
1==="1"// the output is false
1=="1"// the output is true 
```

