# Day3
## Arrays:
#### Arrays let us keep multiple values together in a single collection.
##### EX.
```javascript
let arr= ["abd","khaled"];
```
#### like Strings, Arrays have a length, and each value has an index:
##### EX.
```javascript
let arr= ["abd","khaled"];
arr[1]// the output is "khaled"
arr.length // the output is 2
arr.indexOf("abd") // The output is 0
```
---
#### also like strings, we can check if an array contains a certain value:
##### EX.
```javascript
let arr= ["abd","khaled"];
arr.includes("abd") // The output is true
```
---

##### EX.
```javascript
let arr= ["abd","khaled"];
arr[1]="ahmad" // this command place the string value ahmad in index 1
```
---
### push() & pop():
**push()** is:used to add one or more elements to the end of an array and return the new length for the array.

**pop()** is: used to remove the last element from the end of an array, and return the removed item.
##### EX.
```javascript
let arr= ["abd","khaled"];
let name=arr.pop(); // The value "khaled" located at the last index of the array has been removed, and we have assigned it to the variable named "name".
arr.push("ahmad")// We pushed the string value "ahmad" to the last index in the array.
```
---
#### Arrays can be empty, or hold a single item:
##### EX.
```javascript
let arr= [];// defined an empty array
let arry= ["abd"];// Array with a single item
```
---

#### Arrays can hold any type of items, or mix:
##### EX.
```javascript
let arr= ["abd","khaled", 6 , false];
```
---

### Arrays properties:
#### 1-sort():
##### EX.
```javascript
["c","a","d","b"].sort() //The output is ["a","b","c","d"]
```
---
#### 2-join():
##### EX.
```javascript
["c","a","d","b"].join(" & ") //The output is "c & a & d & b"
```
---
#### 3-concat():
##### EX.
```javascript
[1,2,3].concat([4,5,6]) //The output is [1,2,3,4,5,6]
```
---
### Mutable Vs. Immutable:
**1-Mutable**: data can be edited(e.g. Arrays)
##### EX.
```javascript
let arr=[1,2,3]
arr[1]=5 //The array become [1,5,3]
```
---
**2-Immutable**:data always stays the same (e.g. Strings & other Primitives)
##### EX.
```javascript
let name="abd"
name[1]=f // It will stay abd
```
---
### concat() Vs. push():
**push()**: it's an action **mutate** an array, aka change the array in-place.
##### EX.
```javascript
let arr=[1,2,3]
arr.push("4") // if i print the array "arr" the output is [1,2,3,4], because the change has done in-place.
```
---
**concat**:action do not mutate the original array, but instead create a new copy.
##### EX.
```javascript
let arr=[1,2,3]
[1,2,3].concat([4]) // When printing the array, the output appears as [1, 2, 3]. This is because the modifications were not applied directly to the original array. Instead, a copy of the array was created, and the values were added to it, resulting in [1, 2, 3, 4]. If you want to obtain the modified array, you must use the concatenation operation ([1, 2, 3].concat([4])) and assign it to a new variable in order to reference the new set of values.
```
 ##### EX.
```javascript
let arr=[1,2,3]
let arry=[1,2,3].concat([4])// If i print "arry" the output is [1,2,3,4]
```
---
#### const with arrays:
if i declared an array using 'const' i can  still make modifications to an array declared with const. The const keyword ensures that the variable itself cannot be reassigned to a different value or reference. However, it does not make the value (in this case, the array) immutable.

So, you can modify the contents of the array (add, remove, elements) even if the array is declared with const. The key point is that you cannot reassign the array variable to a completely new array.
 ##### EX.
```javascript
const arr = [1, 2, 3];
arr.push(4);
console.log(arr); // The output is [1, 2, 3, 4]

arr[1] = 10;
console.log(arr); // The output is: [1, 10, 3, 4]

arr = [5, 6, 7]; // This would result in an error because you're trying to reassign the "arr" array, to a new array, which is not allowed with const.
```
---
**Note**:
 ##### EX.
```javascript
ler arr1=[1,2,3];
let arr2=arr1;
arr1[1]=4;// I've changed the value in the index1 in array 'arr1', then it becomes [1,4,3], depending on this change the array 'arr2' will also change to [1,4,3], because the arrays 'arr1'/'arr2' both point the values [1,2,3].
```
---
## Objects:
Objects collect multiple values together to describe more complex data Similar to how we can point at different values using variables in our code, objects let us point at related values using properties in the object. 
 ##### EX.
```javascript
const js ={
  name: "JavaScript",
  abbreviation: "JS",
  isAwesome: true,
  officialSpec: "EcmAscript",
  birthYear: 1995,
  creator: "Brendan Eich"
}:
```
### Getting property values:
 ##### EX.
```javascript
const js ={
  name: "JavaScript",
  abbreviation: "JS",
  isAwesome: true,
  officialSpec: "EcmAscript",
  birthYear: 1995,
  creator: "Brendan Eich"
}:
js.name //The output is "JavaScript", as we can see the output of this is a string so we can do the stringy stuff
//EX.

js.name.startWith("Java")// The output is true
// or we can do
let age =2022-js.birthYear
js.isAwesome // The output is true
```









