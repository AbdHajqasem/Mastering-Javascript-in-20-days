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

## String properties:
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
##### Ex.
```javascript
3+1 //The output is 4
```
---
#### 2)- Subtract
##### Ex.
```javascript
3-1 //The output is 2
```
---
#### 3)* Multiply
##### Ex.
```javascript
3*1 //The output is 3
```
---
#### 4)/ Divide
##### Ex.
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
#### 1)=== / == equals
#### 2)!== / != does not equal
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
---
## Expressions:
Expressions is:a valid set of literals, variables, operators, and expressions that evaluate a single value
##### Ex.
```javascript
4/2*10 // The output is 20
"Frontend" + "Masters" // The output is 'FrontendMasters'
5 > 4 !== 3 > 4 // The output is true
```
---

## Variables
variables point to values(its a pointer)
### 1-let
Special keyword that allow us to create or declare a variable
##### Ex.
```javascript
let x=5; // This command assigns the value of 5 to the variable named "x".
let name ="Abdulkareem"; // This command assigns the string value "Abdulkareem" to the variable named "name"
```
---

#### Declaring Variables:
##### EX.
```javascript
let age; // If i print this variable the output will be undefined
```
---

#### Assigning Variables:
##### EX.
```javascript
let age;
age = 18; //I declared a variable with the name "age," and I assigned the value 18 to this variable
```

---

#### Declaring & Assigning at the same time:
##### EX.
```javascript
let age=18;
```
---

### 2-Const:
Used to declares & assigns a **constant**
aka a variable can't be changed
##### EX.
```javascript
const age = 21; // I declared a variable with the name "age," and I assigned the value 21 to this variable, and i can't assign another value for it, like i cant say (age = 15)
```
---

#### Variables in Expressions:
##### EX.
```javascript
let age=45;
age-2 // the out is 43
```
---

####  Structure for variables name:
The common structure for variables name is a camelCase structure
##### EX.
```javascript
let validVariable;
```
##### note:
I cant start the variable name with number

---

##### EX.
```javascript
let age=(4*2)+3; // The output if i print age is 11
let name="abd";
let myName;
myName=name; // The output if i print myName is "abd"
```
---
### Expression VS. Statments:
#### 1-Expression: 
aks Java-Script for a particular value
##### EX.
```javascript
6+4
document.getElementById("board")
```
----

### 2-Statment:
A statment tells Java-Script to do somthing, like (declare/assign a variable & for statment...etc)
##### EX.
```javascript
let ten=6+4;
maAge=18;
name="Abdulkareem";
```


