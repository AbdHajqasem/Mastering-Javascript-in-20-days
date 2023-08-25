# Day13

## Scope:

**Scope: Where to look for things**

**JavaScript organizes scopes with functions and blocks**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/5b36d016-4ba1-461e-b792-3ffd07d514e0)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/1c79ee35-7b94-49cf-b8bb-730a6758abd8)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/7d090ff8-c4ce-4682-b1d2-587efdd6cc9d)

**Strict mode**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/1ecbe744-005a-4fb0-8a6e-cc7c610aa268)

### Nested Scope:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/99f27cb9-af35-4ecf-b41c-9f0baef632fa)

### Undefined VS. Undeclared:

**Undefined** :means that the variable exist but at the moment it has no value.

**undeclared**: means that never formally declared in any scope that we have accessed to.

---
**Scope Elevator**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/fe817966-64f9-40d9-a562-016cf98e76cb)

---

## Scope & Functions Expressions:

A function expression is a way to define a function by assigning it to a variable, 
allowing functions to be treated as values.

Functions Expressions:

1- Named function expresion

2- Anonymous function expresion

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/75dc8842-0025-4dc9-b804-6da53a9e20a0)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/91cd9df6-94a1-4cbd-82f3-af04d35b4142)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b421ddb9-08ea-4a39-ae0d-4325adefcdaa)

### Arrow Fumctions:
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/d09f7803-89f4-4ef3-942b-889186a5d470)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b07b408f-84cc-4bf3-9e87-cb083e00deee)

---
**Summary**
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/094f314c-1087-4d72-b876-486743768265)

##### Ex.
```javascript
/*Function Expressions

In this exercise, you will be writing some functions and function expressions, to manage the student enrollment records for a workshop.

**Note:** The spirit of this exercise is to use functions wherever possible and appropriate, so consider usage of array utilities `map(..)`, `filter(..)`, `find(..)`, `sort(..)`, and `forEach(..)`.

## Instructions (Part 1)

**Note:** In Part 1, use only function declarations or named function expressions.

You are provided three functions stubs -- `printRecords(..)`, `paidStudentsToEnroll()`, and `remindUnpaid(..)` -- which you must define.

At the bottom of the file you will see these functions called, and a code comment indicating what the console output should be.

1. `printRecords(..)` should:
	- take a list of student Ids
	- retrieve each student record by its student Id (hint: array `find(..)`)
	- sort by student name, ascending (hint: array `sort(..)`)
	- print each record to the console, including `name`, `id`, and `"Paid"` or `"Not Paid"` based on their paid status

2. `paidStudentsToEnroll()` should:
	- look through all the student records, checking to see which ones are paid but **not yet enrolled**
	- collect these student Ids
	- return a new array including the previously enrolled student Ids as well as the to-be-enrolled student Ids (hint: spread `...`)

3. `remindUnpaid(..)` should:
	- take a list of student Ids
	- filter this list of student Ids to only those whose records are in unpaid status
	- pass the filtered list to `printRecords(..)` to print the unpaid reminders

## Instructions (Part 2)

Now that you've completed Part 1, refactor to use **only** `=>` arrow functions.

For `printRecords(..)`, `paidStudentsToEnroll()`, and `remindUnpaid(..)`, assign these arrow functions to variables of such names, so that the execution still works.

As the appeal of `=>` arrow functions is their conciseness, wherever possible try to use only expression bodies (`x => x.id`) instead of full function bodies (`x => { return x.id; }`).*/
```


